# Comparing `tmp/hi-ml-cpath-0.2.9.tar.gz` & `tmp/hi-ml-cpath-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hi-ml-cpath-0.2.9.tar", last modified: Wed Nov  9 17:14:35 2022, max compression
+gzip compressed data, was "hi-ml-cpath-0.3.0.tar", last modified: Sun May  7 19:21:48 2023, max compression
```

## Comparing `hi-ml-cpath-0.2.9.tar` & `hi-ml-cpath-0.3.0.tar`

### file list

```diff
@@ -1,62 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.534194 hi-ml-cpath-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     4270 2022-11-09 17:14:35.534194 hi-ml-cpath-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 17:14:35.534194 hi-ml-cpath-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3966 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/health_cpath/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/health_cpath/configs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/
--rw-r--r--   0 runner    (1001) docker     (121)    17817 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/BaseMIL.py
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/DeepSMILECrck.py
--rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/DeepSMILEPanda.py
--rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/DeepSMILESlidesPandaBenchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/configs/run_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/health_cpath/datamodules/
--rw-r--r--   0 runner    (1001) docker     (121)    16980 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datamodules/base_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datamodules/panda_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datamodules/panda_module_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datamodules/tcga_crck_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/health_cpath/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)    11711 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datasets/dataset_return_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datasets/default_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     5986 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datasets/panda_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     6303 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datasets/panda_tiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datasets/tcga_crck_tiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/datasets/tcga_prad_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/health_cpath/models/
--rw-r--r--   0 runner    (1001) docker     (121)    19266 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/models/deepmil.py
--rw-r--r--   0 runner    (1001) docker     (121)     7153 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/models/encoders.py
--rw-r--r--   0 runner    (1001) docker     (121)     8438 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/models/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/health_cpath/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)    10372 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/preprocessing/create_panda_tiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    14906 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/preprocessing/create_tiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5629 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/preprocessing/loading.py
--rw-r--r--   0 runner    (1001) docker     (121)     6392 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/preprocessing/tiling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.530194 hi-ml-cpath-0.2.9/src/health_cpath/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     4756 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/scripts/aggregate_metrics_crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (121)    14143 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/scripts/generate_crossval_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/scripts/mount_azure_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/scripts/tcga_dataset_prep.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.534194 hi-ml-cpath-0.2.9/src/health_cpath/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    13754 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/analysis_plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7257 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/deepmil_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    21168 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/girder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/heatmap_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (121)    19290 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/output_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10447 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/plots_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12579 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/tcga_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    17763 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/tiles_selection_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10681 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-09 17:14:17.000000 hi-ml-cpath-0.2.9/src/health_cpath/utils/wsi_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 17:14:35.534194 hi-ml-cpath-0.2.9/src/hi_ml_cpath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4270 2022-11-09 17:14:35.000000 hi-ml-cpath-0.2.9/src/hi_ml_cpath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-11-09 17:14:35.000000 hi-ml-cpath-0.2.9/src/hi_ml_cpath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 17:14:35.000000 hi-ml-cpath-0.2.9/src/hi_ml_cpath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-09 17:14:35.000000 hi-ml-cpath-0.2.9/src/hi_ml_cpath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-09 17:14:35.000000 hi-ml-cpath-0.2.9/src/hi_ml_cpath.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3562 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/configs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)    17055 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/BaseMIL.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4326 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILECrck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILEPanda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7824 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILESlidesPandaBenchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/run_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/
+-rw-r--r--   0 runner    (1001) docker     (122)    17147 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2885 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/panda_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/panda_module_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/tcga_crck_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)    13476 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/dataset_return_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/default_paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/panda_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5579 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/panda_tiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/tcga_crck_tiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/tcga_prad_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/models/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/models/deepmil.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22673 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/models/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17693 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/models/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)    10310 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/create_panda_tiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15042 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/create_tiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19956 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/loading.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13827 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/tiff_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6353 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/tiling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     4594 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/aggregate_metrics_crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/create_montage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/generate_checkpoint_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15779 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/generate_crossval_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/mount_azure_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/tcga_dataset_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/src/health_cpath/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14187 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/analysis_plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27643 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13078 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/deepmil_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25803 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/girder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/heatmap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/montage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/montage_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21122 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/package_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21647 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/plots_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14679 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/tcga_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6717 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/tiff_conversion_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17727 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/tiles_selection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14170 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5868 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/wsi_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/top_level.txt
```

### Comparing `hi-ml-cpath-0.2.9/PKG-INFO` & `hi-ml-cpath-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-cpath
-Version: 0.2.9
+Version: 0.3.0
 Summary: Microsoft Health Futures package for deep learning on histopathology images
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Keywords: Health Futures,Health Intelligence,Computational Pathology,AzureML
 Platform: UNKNOWN
```

### Comparing `hi-ml-cpath-0.2.9/README.md` & `hi-ml-cpath-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.2.9/setup.py` & `hi-ml-cpath-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # See also:
 # https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 # https://github.com/pypa/gh-action-pypi-publish
 GITHUB_REF_TAG_COMMIT = "refs/tags/v"
 
 github_ref = os.getenv("GITHUB_REF")
 if github_ref and github_ref.startswith(GITHUB_REF_TAG_COMMIT):
-    version = github_ref[len(GITHUB_REF_TAG_COMMIT):]
+    version = github_ref[len(GITHUB_REF_TAG_COMMIT) :]
 
 # Otherwise, if running from a GitHub Action, but not a tagged commit then GITHUB_RUN_NUMBER will be populated.
 # Use this as a post release number. For example if GITHUB_RUN_NUMBER = 124 then the version string will be
 # "99.99.post124". Although this is discouraged, see:
 # https://www.python.org/dev/peps/pep-0440/#post-releases
 # it is necessary here to avoid duplicate packages in Test.PyPI.
 if not version:
@@ -74,15 +74,15 @@
     author="Biomedical Imaging Team @ Microsoft Health Futures",
     author_email="innereyedev@microsoft.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7"
+        "Programming Language :: Python :: 3.7",
     ],
     keywords="Health Futures, Health Intelligence, Computational Pathology, AzureML",
     license="MIT License",
     packages=find_namespace_packages(where="src", include=["health_cpath.*"]),
     package_dir={"": "src"},
     include_package_data=False,
     install_requires=install_requires,
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/BaseMIL.py` & `hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/BaseMIL.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,282 +1,349 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 
 import os
-import logging
 import param
+import logging
+import warnings
 from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Union
 
 from pathlib import Path
 from monai.transforms import Compose
 from pytorch_lightning.callbacks import Callback
 from pytorch_lightning.callbacks.model_checkpoint import ModelCheckpoint
 
 from health_azure.utils import create_from_matching_params
+from health_cpath.preprocessing.loading import LoadingParams
+from health_cpath.utils.callbacks import LossAnalysisCallback, LossCallbackParams
+from health_cpath.utils.wsi_utils import TilingParams
 
-from health_ml.utils import fixed_paths
 from health_ml.deep_learning_config import OptimizerParams
 from health_ml.lightning_container import LightningContainer
-from health_ml.utils.checkpoint_utils import get_best_checkpoint_path
-from health_ml.utils.common_utils import DEFAULT_AML_CHECKPOINT_DIR
+from health_ml.utils.checkpoint_utils import CheckpointParser
 
 from health_cpath.datamodules.base_module import CacheLocation, CacheMode, HistoDataModule
 from health_cpath.datasets.base_dataset import SlidesDataset
-from health_cpath.models.deepmil import TilesDeepMILModule, SlidesDeepMILModule, BaseDeepMILModule
+from health_cpath.models.deepmil import DeepMILModule
 from health_cpath.models.transforms import EncodeTilesBatchd, LoadTilesBatchd
-from health_cpath.utils.deepmil_utils import EncoderParams, PoolingParams
+from health_cpath.utils.deepmil_utils import ClassifierParams, EncoderParams, PoolingParams
 from health_cpath.utils.output_utils import DeepMILOutputsHandler
 from health_cpath.utils.naming import MetricsKey, PlotOption, SlideKey, ModelKey
 from health_cpath.utils.tiles_selection_utils import TilesSelector
 
 
-class BaseMIL(LightningContainer, EncoderParams, PoolingParams):
+class BaseMIL(LightningContainer, LoadingParams, EncoderParams, PoolingParams, ClassifierParams, LossCallbackParams):
     """BaseMIL is an abstract container defining basic functionality for running MIL experiments in both slides and
     tiles settings. It is responsible for instantiating the encoder and pooling layer. Subclasses should define the
     full DeepMIL model depending on the type of dataset (tiles/slides based).
     """
-    dropout_rate: Optional[float] = param.Number(None, bounds=(0, 1), doc="Pre-classifier dropout rate.")
-    class_names: Optional[Sequence[str]] = param.List(None, item_type=str, doc="List of class names. If `None`, "
-                                                                               "defaults to `('0', '1', ...)`.")
+
+    class_names: Optional[Sequence[str]] = param.List(
+        None, item_type=str, doc="List of class names. If `None`, defaults to `('0', '1', ...)`."
+    )
     # Data module parameters:
     batch_size: int = param.Integer(16, bounds=(1, None), doc="Number of slides to load per batch.")
-    max_bag_size: int = param.Integer(1000, bounds=(0, None),
-                                      doc="Upper bound on number of tiles in each loaded bag during training stage. "
-                                          "If 0 (default), will return all samples in each bag. "
-                                          "If > 0, bags larger than `max_bag_size` will yield "
-                                          "random subsets of instances.")
-    max_bag_size_inf: int = param.Integer(0, bounds=(0, None),
-                                          doc="Upper bound on number of tiles in each loaded bag during "
-                                          "validation and test stages."
-                                          "If 0 (default), will return all samples in each bag. "
-                                          "If > 0 , bags larger than `max_bag_size_inf` will yield "
-                                          "random subsets of instances.")
-    # local_dataset (used as data module root_path) is declared in DatasetParams superclass
-    level: int = param.Integer(1, bounds=(0, None), doc="The whole slide image level at which the image is extracted."
-                                                        "Whole slide images are represented in a pyramid consisting of"
-                                                        "multiple images at different resolutions."
-                                                        "If 1 (default), will extract baseline image at the resolution"
-                                                        "at level 1.")
+    batch_size_inf: int = param.Integer(16, bounds=(1, None), doc="Number of slides per batch during inference.")
+    max_bag_size: int = param.Integer(
+        1000,
+        bounds=(0, None),
+        doc="Upper bound on number of tiles in each loaded bag during training stage. "
+        "If 0 (default), will return all samples in each bag. "
+        "If > 0, bags larger than `max_bag_size` will yield "
+        "random subsets of instances.",
+    )
+    max_bag_size_inf: int = param.Integer(
+        0,
+        bounds=(0, None),
+        doc="Upper bound on number of tiles in each loaded bag during "
+        "validation and test stages."
+        "If 0 (default), will return all samples in each bag. "
+        "If > 0 , bags larger than `max_bag_size_inf` will yield "
+        "random subsets of instances.",
+    )
     # Outputs Handler parameters:
-    num_top_slides: int = param.Integer(10, bounds=(0, None), doc="Number of slides to select when saving top and "
-                                                                  "bottom tiles. If set to 10 (default), it selects 10 "
-                                                                  "top and 10 bottom slides. To disable tiles plots "
-                                                                  "saving, set `num_top_slides=0`")
-    num_top_tiles: int = param.Integer(12, bounds=(1, None), doc="Number of tiles to select when saving top and bottom"
-                                                                 "tiles. If set to 12 (default), it saves 12 top and 12"
-                                                                 "bottom tiles.")
-    primary_val_metric: MetricsKey = param.ClassSelector(default=MetricsKey.AUROC, class_=MetricsKey,
-                                                         doc="Primary validation metric to track for checkpointing and "
-                                                             "generating outputs.")
-    maximise_primary_metric: bool = param.Boolean(True, doc="Whether the primary validation metric should be "
-                                                            "maximised (otherwise minimised).")
-    ssl_checkpoint_run_id: str = param.String(default="", doc="Optional run id from which to load checkpoint if "
-                                              "using SSLEncoder")
-    max_num_workers: int = param.Integer(10, bounds=(0, None),
-                                         doc="The maximum number of worker processes for dataloaders. Dataloaders use"
-                                             "a heuristic num_cpus/num_gpus to set the number of workers, which can be"
-                                             "very high for small num_gpus. This parameters sets an upper bound.")
+    num_top_slides: int = param.Integer(
+        10,
+        bounds=(0, None),
+        doc="Number of slides to select when saving top and "
+        "bottom tiles. If set to 10 (default), it selects 10 "
+        "top and 10 bottom slides. To disable tiles plots "
+        "saving, set `num_top_slides=0`",
+    )
+    num_top_tiles: int = param.Integer(
+        12,
+        bounds=(1, None),
+        doc="Number of tiles to select when saving top and bottom"
+        "tiles. If set to 12 (default), it saves 12 top and 12"
+        "bottom tiles.",
+    )
+    primary_val_metric: MetricsKey = param.ClassSelector(
+        default=MetricsKey.AUROC,
+        class_=MetricsKey,
+        doc="Primary validation metric to track for checkpointing and generating outputs.",
+    )
+    maximise_primary_metric: bool = param.Boolean(
+        True, doc="Whether the primary validation metric should be maximised (otherwise minimised)."
+    )
+    max_num_workers: int = param.Integer(
+        10,
+        bounds=(0, None),
+        doc="The maximum number of worker processes for dataloaders. Dataloaders use"
+        "a heuristic num_cpus/num_gpus to set the number of workers, which can be"
+        "very high for small num_gpus. This parameters sets an upper bound.",
+    )
+    save_intermediate_outputs: bool = param.Boolean(
+        True, doc="Whether to save intermediate validation outputs during training."
+    )
+    stratify_plots_by: Optional[str] = param.String(
+        None, doc="Name of metadata field to stratify output plots (PR curve, ROC curve)."
+    )
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.run_extra_val_epoch = True  # Enable running an additional validation step to save tiles/slides thumbnails
         metric_optim = "max" if self.maximise_primary_metric else "min"
         self.best_checkpoint_filename = f"checkpoint_{metric_optim}_val_{self.primary_val_metric.value}"
         self.best_checkpoint_filename_with_suffix = self.best_checkpoint_filename + ".ckpt"
+        self.validate()
+        if not self.pl_replace_sampler_ddp and self.max_num_gpus > 1:
+            logging.info(
+                "Replacing sampler with `DistributedSampler` is disabled. Make sure to set your own DDP sampler"
+            )
+        self.ignore_pl_warnings()
+
+    def validate(self) -> None:
+        super().validate()
+        EncoderParams.validate(self)
+        if not any([self.tune_encoder, self.tune_pooling, self.tune_classifier]) and not self.run_inference_only:
+            raise ValueError(
+                "At least one of the encoder, pooling or classifier should be fine tuned. Turn on one of the tune "
+                "arguments `tune_encoder`, `tune_pooling`, `tune_classifier`. Otherwise, activate inference only "
+                "mode via `run_inference_only` flag."
+            )
+        if (
+            any([self.pretrained_encoder, self.pretrained_pooling, self.pretrained_classifier])
+            and not self.src_checkpoint
+        ):
+            raise ValueError(
+                "You need to specify a source checkpoint, to use a pretrained encoder, pooling or classifier."
+                f" {CheckpointParser.INFO_MESSAGE}"
+            )
+        if (
+            self.tune_encoder
+            and self.encoding_chunk_size < self.max_bag_size
+            and self.pl_sync_batchnorm
+            and self.max_num_gpus > 1
+        ):
+            raise ValueError(
+                "The encoding chunk size should be at least as large as the maximum bag size when fine tuning the "
+                "encoder. You might encounter Batch Norm synchronization issues if the chunk size is smaller than "
+                "the maximum bag size causing the processes to hang silently. This is due to the encoder being called "
+                "different number of times on each device, which cause Batch Norm running statistics to be updated "
+                "inconsistently across processes. In case you can't increase the `encoding_chunk_size` any further, set"
+                " `pl_sync_batchnorm=False` to simply skip Batch Norm synchronization across devices. Note that this "
+                "might come with some performance penalty."
+            )
 
     @property
     def cache_dir(self) -> Path:
         return Path(f"/tmp/himl_cache/{self.__class__.__name__}-{self.encoder_type}/")
 
     def get_test_plot_options(self) -> Set[PlotOption]:
         options = {PlotOption.HISTOGRAM, PlotOption.CONFUSION_MATRIX}
         if self.num_top_slides > 0:
-            options.add(PlotOption.TOP_BOTTOM_TILES)
+            options.update([PlotOption.TOP_BOTTOM_TILES, PlotOption.ATTENTION_HISTOGRAM])
         return options
 
     def get_val_plot_options(self) -> Set[PlotOption]:
+        """Override this method if you want to produce validation plots at each epoch. By default, at the end of the
+        training an extra validation epoch is run where val_plot_options = test_plot_options
+        """
         return set()
 
     def get_outputs_handler(self) -> DeepMILOutputsHandler:
         n_classes = self.data_module.train_dataset.n_classes
         outputs_handler = DeepMILOutputsHandler(
             outputs_root=self.outputs_folder,
             n_classes=n_classes,
             tile_size=self.tile_size,
-            level=self.level,
             class_names=self.class_names,
             primary_val_metric=self.primary_val_metric,
             maximise=self.maximise_primary_metric,
             val_plot_options=self.get_val_plot_options(),
             test_plot_options=self.get_test_plot_options(),
+            loading_params=create_from_matching_params(self, LoadingParams),
+            save_intermediate_outputs=self.save_intermediate_outputs,
+            stratify_plots_by=self.stratify_plots_by,
         )
         if self.num_top_slides > 0:
             outputs_handler.tiles_selector = TilesSelector(
                 n_classes=n_classes, num_slides=self.num_top_slides, num_tiles=self.num_top_tiles
             )
         return outputs_handler
 
     def get_callbacks(self) -> List[Callback]:
-        return [*super().get_callbacks(),
-                ModelCheckpoint(dirpath=self.checkpoint_folder,
-                                monitor=f"{ModelKey.VAL}/{self.primary_val_metric}",
-                                filename=self.best_checkpoint_filename,
-                                auto_insert_metric_name=False,
-                                mode="max" if self.maximise_primary_metric else "min")]
+        callbacks = [
+            *super().get_callbacks(),
+            ModelCheckpoint(
+                dirpath=self.checkpoint_folder,
+                monitor=f"{ModelKey.VAL}/{self.primary_val_metric}",
+                filename=self.best_checkpoint_filename,
+                auto_insert_metric_name=False,
+                mode="max" if self.maximise_primary_metric else "min",
+            ),
+        ]
+        if self.analyse_loss:
+            callbacks.append(
+                LossAnalysisCallback(
+                    outputs_folder=self.outputs_folder,
+                    max_epochs=self.max_epochs,
+                    patience=self.loss_analysis_patience,
+                    epochs_interval=self.loss_analysis_epochs_interval,
+                    num_slides_scatter=self.num_slides_scatter,
+                    num_slides_heatmap=self.num_slides_heatmap,
+                    save_tile_ids=self.save_tile_ids,
+                    log_exceptions=self.log_exceptions,
+                )
+            )
+        return callbacks
 
     def get_checkpoint_to_test(self) -> Path:
         """
         Returns the full path to a checkpoint file that was found to be best during training, whatever criterion
-        was applied there. This is necessary since for some models the checkpoint is in a subfolder of the checkpoint
-        folder.
+        was applied there. Note that the checkpoint file might not (yet) exist, for example in the case of
+        preempted jobs.
         """
-        # absolute path is required for registering the model.
-        absolute_checkpoint_path = Path(fixed_paths.repository_root_directory(),
-                                        DEFAULT_AML_CHECKPOINT_DIR,
-                                        self.best_checkpoint_filename_with_suffix)
-        if absolute_checkpoint_path.is_file():
-            return absolute_checkpoint_path
-
-        absolute_checkpoint_path_parent = Path(fixed_paths.repository_root_directory().parent,
-                                               DEFAULT_AML_CHECKPOINT_DIR,
-                                               self.best_checkpoint_filename_with_suffix)
-        if absolute_checkpoint_path_parent.is_file():
-            return absolute_checkpoint_path_parent
-
-        checkpoint_path = get_best_checkpoint_path(self.checkpoint_folder)
-        if checkpoint_path.is_file():
-            return checkpoint_path
-
-        raise ValueError("Path to best checkpoint not found")
+        checkpoint_path = Path(self.checkpoint_folder, self.best_checkpoint_filename_with_suffix)
+        return checkpoint_path
 
     def get_dataloader_kwargs(self) -> dict:
         num_cpus = os.cpu_count()
         assert num_cpus is not None  # for mypy
         logging.info(f"os.cpu_count()={num_cpus}")
         num_devices = self.num_gpus_per_node()
         # We ensure num_devices is not 0 for non-GPU machines
         # to avoid division by zero error when computing `workers_per_gpu`
         workers_per_gpu = num_cpus // (num_devices or 1)
         workers_per_gpu = min(self.max_num_workers, workers_per_gpu)
-        print(f"Using {workers_per_gpu} data loader worker processes per GPU")
+        logging.info(f"Using {workers_per_gpu} data loader worker processes per GPU")
         dataloader_kwargs = dict(num_workers=workers_per_gpu, pin_memory=True)
         return dataloader_kwargs
 
     def get_transforms_dict(self, image_key: str) -> Optional[Dict[ModelKey, Union[Callable, None]]]:
         """Returns the image transforms that the training, validation, and test dataloaders should use.
 
         For reproducible results, those may need to be made deterministic via setting a fixed
         random see. See `SlidesDataModule` for an example how to achieve that."""
         return None
 
-    def create_model(self) -> BaseDeepMILModule:
-        raise NotImplementedError
+    def get_encoder_params(self) -> EncoderParams:
+        return create_from_matching_params(self, EncoderParams)
+
+    def create_model(self) -> DeepMILModule:
+        self.data_module = self.get_data_module()
+        outputs_handler = self.get_outputs_handler()
+        deepmil_module = DeepMILModule(
+            label_column=self.get_label_column(),
+            n_classes=self.data_module.train_dataset.n_classes,
+            class_names=self.class_names,
+            class_weights=self.data_module.class_weights,
+            outputs_folder=self.outputs_folder,
+            encoder_params=self.get_encoder_params(),
+            pooling_params=create_from_matching_params(self, PoolingParams),
+            classifier_params=create_from_matching_params(self, ClassifierParams),
+            optimizer_params=create_from_matching_params(self, OptimizerParams),
+            outputs_handler=outputs_handler,
+            analyse_loss=self.analyse_loss,
+        )
+        deepmil_module.transfer_weights(self.trained_weights_path)
+        outputs_handler.set_slides_dataset_for_plots_handlers(self.get_slides_dataset())
+        outputs_handler.set_extra_slides_dataset_for_plots_handlers(self.get_extra_slides_dataset_for_plotting())
+        return deepmil_module
 
     def get_data_module(self) -> HistoDataModule:
         raise NotImplementedError
 
     def get_slides_dataset(self) -> Optional[SlidesDataset]:
         return None
 
+    def get_extra_slides_dataset_for_plotting(self) -> Optional[SlidesDataset]:
+        return None
+
+    def ignore_pl_warnings(self) -> None:
+        # Pytorch Lightning prints a warning if the batch size is not consistent across all batches. The way PL infers
+        # the batch size is not compatible with our data loaders. It searches for the first item in the batch that is a
+        # tensor and uses its size[0] as the batch size. However, in our case, the batch is a list of tensors, so it
+        # thinks that the batch size is the bag_size which can be different for each WSI in the batch. This is why we
+        # ignore this warning to avoid noisy logs.
+        warnings.filterwarnings("ignore", ".*Trying to infer the `batch_size` from an ambiguous collection.*")
+
+    def get_label_column(self) -> str:
+        """Slides and Tiles pipeline use different label columns."""
+        raise NotImplementedError
+
 
 class BaseMILTiles(BaseMIL):
     """BaseMILTiles is an abstract subclass of BaseMIL for running MIL experiments on tiles datasets. It is responsible
     for instantiating the full DeepMIL model in tiles settings. Subclasses should define their datamodules and
     configure experiment-specific parameters.
     """
+
     # Tiles Data module parameters:
-    cache_mode: CacheMode = param.ClassSelector(default=CacheMode.MEMORY, class_=CacheMode,
-                                                doc="The type of caching to perform: "
-                                                    "'memory' (default), 'disk', or 'none'.")
-    precache_location: CacheLocation = param.ClassSelector(default=CacheLocation.CPU, class_=CacheLocation,
-                                                           doc="Whether to pre-cache the entire transformed dataset "
-                                                               "upfront and save it to disk and if re-load in cpu or "
-                                                               "gpu. Options: `none`,`cpu` (default), `gpu`")
+    cache_mode: CacheMode = param.ClassSelector(
+        default=CacheMode.MEMORY,
+        class_=CacheMode,
+        doc="The type of caching to perform: 'memory' (default), 'disk', or 'none'.",
+    )
+    precache_location: CacheLocation = param.ClassSelector(
+        default=CacheLocation.CPU,
+        class_=CacheLocation,
+        doc="Whether to pre-cache the entire transformed dataset "
+        "upfront and save it to disk and if re-load in cpu or "
+        "gpu. Options: `none`,`cpu` (default), `gpu`",
+    )
+
+    def get_label_column(self) -> str:
+        return self.data_module.train_dataset.label_column
 
     def setup(self) -> None:
         super().setup()
         # Fine-tuning requires tiles to be loaded on-the-fly, hence, caching is disabled by default.
-        # When is_finetune and is_caching are both set, below lines should disable caching automatically.
-        if self.is_finetune:
+        # When tune_encoder and is_caching are both set, below lines should disable caching automatically.
+        if self.tune_encoder:
             self.is_caching = False
         if not self.is_caching:
             self.cache_mode = CacheMode.NONE
             self.precache_location = CacheLocation.NONE
 
     def get_dataloader_kwargs(self) -> dict:
         if self.is_caching:
             dataloader_kwargs = dict(num_workers=0, pin_memory=False)
         else:
             dataloader_kwargs = super().get_dataloader_kwargs()
         return dataloader_kwargs
 
     def get_transforms_dict(self, image_key: str) -> Dict[ModelKey, Union[Callable, None]]:
         if self.is_caching:
-            encoder = create_from_matching_params(self, EncoderParams).get_encoder(self.ssl_checkpoint_run_id,
-                                                                                   self.outputs_folder)
-            transform = Compose([
-                LoadTilesBatchd(image_key, progress=True),
-                EncodeTilesBatchd(image_key, encoder, chunk_size=self.encoding_chunk_size)  # type: ignore
-            ])
+            encoder = create_from_matching_params(self, EncoderParams).get_encoder(self.outputs_folder)
+            transform = Compose(
+                [
+                    LoadTilesBatchd(image_key, progress=False),
+                    EncodeTilesBatchd(image_key, encoder, chunk_size=self.encoding_chunk_size),  # type: ignore
+                ]
+            )
         else:
-            transform = LoadTilesBatchd(image_key, progress=True)  # type: ignore
+            transform = LoadTilesBatchd(image_key, progress=False)  # type: ignore
         # in case the transformations for training contain augmentations, val and test transform will be different
         return {ModelKey.TRAIN: transform, ModelKey.VAL: transform, ModelKey.TEST: transform}
 
-    def create_model(self) -> TilesDeepMILModule:
-        self.data_module = self.get_data_module()
-        outputs_handler = self.get_outputs_handler()
-        deepmil_module = TilesDeepMILModule(label_column=self.data_module.train_dataset.label_column,
-                                            n_classes=self.data_module.train_dataset.n_classes,
-                                            class_names=self.class_names,
-                                            class_weights=self.data_module.class_weights,
-                                            dropout_rate=self.dropout_rate,
-                                            outputs_folder=self.outputs_folder,
-                                            ssl_ckpt_run_id=self.ssl_checkpoint_run_id,
-                                            encoder_params=create_from_matching_params(self, EncoderParams),
-                                            pooling_params=create_from_matching_params(self, PoolingParams),
-                                            optimizer_params=create_from_matching_params(self, OptimizerParams),
-                                            outputs_handler=outputs_handler)
-        outputs_handler.set_slides_dataset_for_plots_handlers(self.get_slides_dataset())
-        return deepmil_module
-
 
-class BaseMILSlides(BaseMIL):
+class BaseMILSlides(BaseMIL, TilingParams):
     """BaseSlidesMIL is an abstract subclass of BaseMIL for running MIL experiments on slides datasets. It is
     responsible for instantiating the full DeepMIL model in slides settings. Subclasses should define their datamodules
     and configure experiment-specific parameters.
     """
-    # Slides Data module parameters:
-    tile_size: int = param.Integer(224, bounds=(0, None), doc="Size of the square tile, defaults to 224.")
-    step: int = param.Integer(None, bounds=(0, None),
-                              doc="Step size to define the offset between tiles."
-                              "If None (default), it takes the same value as tile_size."
-                              "If step < tile_size, it creates overlapping tiles."
-                              "If step > tile_size, it skips some chunks in the wsi.")
-    random_offset: bool = param.Boolean(False, doc="If True, randomize position of the grid, instead of starting at"
-                                                   "the top-left corner,")
-    pad_full: bool = param.Boolean(False, doc="If True, pad image to the size evenly divisible by tile_size")
-    background_val: int = param.Integer(255, bounds=(0, None),
-                                        doc="Threshold to estimate the foreground in a whole slide image.")
-    filter_mode: str = param.String("min", doc="mode must be in ['min', 'max', 'random']. If total number of tiles is"
-                                               "greater than tile_count, then sort by intensity sum, and take the "
-                                               "smallest (for min), largest (for max) or random (for random) subset, "
-                                               "defaults to 'min' (which assumes background is high value).")
 
-    def create_model(self) -> SlidesDeepMILModule:
-        self.data_module = self.get_data_module()
-        outputs_handler = self.get_outputs_handler()
-        deepmil_module = SlidesDeepMILModule(label_column=SlideKey.LABEL,
-                                             n_classes=self.data_module.train_dataset.n_classes,
-                                             class_names=self.class_names,
-                                             class_weights=self.data_module.class_weights,
-                                             dropout_rate=self.dropout_rate,
-                                             outputs_folder=self.outputs_folder,
-                                             ssl_ckpt_run_id=self.ssl_checkpoint_run_id,
-                                             encoder_params=create_from_matching_params(self, EncoderParams),
-                                             pooling_params=create_from_matching_params(self, PoolingParams),
-                                             optimizer_params=create_from_matching_params(self, OptimizerParams),
-                                             outputs_handler=outputs_handler)
-        outputs_handler.set_slides_dataset_for_plots_handlers(self.get_slides_dataset())
-        return deepmil_module
+    def get_label_column(self) -> str:
+        return SlideKey.LABEL
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/DeepSMILECrck.py` & `hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILECrck.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,41 +7,43 @@
 
 For convenience, this module also defines encoder-specific containers e.g.TcgaCrckImageNetMIL
 
 Reference:
 - Schirris (2021). DeepSMILE: Self-supervised heterogeneity-aware multiple instance learning for DNA
 damage response defect classification directly from H&E whole-slide images. arXiv:2107.09405
 """
-from typing import Any
+from typing import Any, Set
 
 from health_ml.networks.layers.attention_layers import AttentionLayer
 from health_cpath.configs.run_ids import innereye_ssl_checkpoint_crck_4ws
 from health_cpath.datamodules.base_module import TilesDataModule
 from health_cpath.datamodules.tcga_crck_module import TcgaCrckTilesDataModule
 from health_cpath.datasets.default_paths import TCGA_CRCK_DATASET_ID
 from health_cpath.models.encoders import (
     HistoSSLEncoder,
-    ImageNetEncoder,
     ImageNetSimCLREncoder,
+    Resnet18,
     SSLEncoder,
 )
 from health_cpath.configs.classification.BaseMIL import BaseMILTiles
 from health_cpath.datasets.tcga_crck_tiles_dataset import TcgaCrck_TilesDataset
+from health_cpath.utils.naming import PlotOption
+from health_ml.utils.checkpoint_utils import CheckpointParser
 
 
 class DeepSMILECrck(BaseMILTiles):
     def __init__(self, **kwargs: Any) -> None:
         # Define dictionary with default params that can be overridden from subclasses or CLI
         default_kwargs = dict(
             # declared in BaseMIL:
             pool_type=AttentionLayer.__name__,
             num_transformer_pool_layers=4,
             num_transformer_pool_heads=4,
             encoding_chunk_size=60,
-            is_finetune=False,
+            tune_encoder=False,
             is_caching=True,
             num_top_slides=0,
             azure_datasets=[TCGA_CRCK_DATASET_ID],
             # declared in TrainerParams:
             max_epochs=50,
             # declared in WorkflowParams:
             crossval_count=5,
@@ -51,45 +53,52 @@
             adam_betas=(0.9, 0.99),
         )
         default_kwargs.update(kwargs)
         super().__init__(**default_kwargs)
 
     def setup(self) -> None:
         super().setup()
-        # If no SSL checkpoint is provided, use the default one
-        self.ssl_checkpoint_run_id = self.ssl_checkpoint_run_id or innereye_ssl_checkpoint_crck_4ws
 
     def get_data_module(self) -> TilesDataModule:
         return TcgaCrckTilesDataModule(
             root_path=self.local_datasets[0],
             max_bag_size=self.max_bag_size,
             batch_size=self.batch_size,
+            batch_size_inf=self.batch_size_inf,
             max_bag_size_inf=self.max_bag_size_inf,
             transforms_dict=self.get_transforms_dict(TcgaCrck_TilesDataset.IMAGE_COLUMN),
             cache_mode=self.cache_mode,
             precache_location=self.precache_location,
             cache_dir=self.cache_dir,
             crossval_count=self.crossval_count,
             crossval_index=self.crossval_index,
             dataloader_kwargs=self.get_dataloader_kwargs(),
             seed=self.get_effective_random_seed(),
+            pl_replace_sampler_ddp=self.pl_replace_sampler_ddp,
         )
 
+    def get_test_plot_options(self) -> Set[PlotOption]:
+        plot_options = super().get_test_plot_options()
+        plot_options.add(PlotOption.PR_CURVE)
+        return plot_options
+
 
 class TcgaCrckImageNetMIL(DeepSMILECrck):
     def __init__(self, **kwargs: Any) -> None:
-        super().__init__(encoder_type=ImageNetEncoder.__name__, **kwargs)
+        super().__init__(encoder_type=Resnet18.__name__, **kwargs)
 
 
 class TcgaCrckImageNetSimCLRMIL(DeepSMILECrck):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(encoder_type=ImageNetSimCLREncoder.__name__, **kwargs)
 
 
 class TcgaCrckSSLMIL(DeepSMILECrck):
     def __init__(self, **kwargs: Any) -> None:
+        # If no SSL checkpoint is provided, use the default one
+        self.ssl_checkpoint = self.ssl_checkpoint or CheckpointParser(innereye_ssl_checkpoint_crck_4ws)
         super().__init__(encoder_type=SSLEncoder.__name__, **kwargs)
 
 
 class TcgaCrckHistoSSLMIL(DeepSMILECrck):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(encoder_type=HistoSSLEncoder.__name__, **kwargs)
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/DeepSMILEPanda.py` & `hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILEPanda.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,119 +1,123 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 from typing import Any, Optional, Set
-
-from health_azure.utils import is_running_in_azure_ml
-from health_ml.networks.layers.attention_layers import AttentionLayer
+from health_azure.utils import is_running_in_azure_ml, create_from_matching_params
+from health_cpath.configs.classification.BaseMIL import BaseMIL, BaseMILSlides, BaseMILTiles
 from health_cpath.configs.run_ids import innereye_ssl_checkpoint_binary
-from health_cpath.datamodules.panda_module import (
-    PandaSlidesDataModule,
-    PandaTilesDataModule)
-from health_cpath.datasets.panda_tiles_dataset import PandaTilesDataset
-from health_cpath.models.encoders import (
-    HistoSSLEncoder,
-    ImageNetEncoder,
-    ImageNetSimCLREncoder,
-    SSLEncoder)
-from health_cpath.configs.classification.BaseMIL import BaseMILSlides, BaseMILTiles, BaseMIL
+from health_cpath.datamodules.panda_module import PandaSlidesDataModule, PandaTilesDataModule
+from health_cpath.datasets.default_paths import PANDA_5X_TILES_DATASET_ID, PANDA_DATASET_ID
 from health_cpath.datasets.panda_dataset import PandaDataset
-from health_cpath.datasets.default_paths import (
-    PANDA_DATASET_ID,
-    PANDA_5X_TILES_DATASET_ID)
-from health_cpath.utils.naming import PlotOption
+from health_cpath.datasets.panda_tiles_dataset import PandaTilesDataset
+from health_cpath.models.encoders import HistoSSLEncoder, ImageNetSimCLREncoder, Resnet18, SSLEncoder
+from health_cpath.preprocessing.loading import LoadingParams, ROIType, WSIBackend
+from health_cpath.utils.naming import PlotOption, SlideKey
+from health_cpath.utils.wsi_utils import TilingParams
+from health_ml.networks.layers.attention_layers import AttentionLayer
+from health_ml.utils.checkpoint_utils import CheckpointParser
 
 
 class BaseDeepSMILEPanda(BaseMIL):
     """Base class for DeepSMILEPanda common configs between tiles and slides piplines."""
 
     def __init__(self, **kwargs: Any) -> None:
         default_kwargs = dict(
             # declared in BaseMIL:
             pool_type=AttentionLayer.__name__,
             num_transformer_pool_layers=4,
             num_transformer_pool_heads=4,
-            is_finetune=False,
+            tune_encoder=False,
             # average number of tiles is 56 for PANDA
             encoding_chunk_size=60,
             max_bag_size=56,
             max_bag_size_inf=0,
             # declared in TrainerParams:
             max_epochs=200,
             # declared in OptimizerParams:
             l_rate=5e-4,
             weight_decay=1e-4,
-            adam_betas=(0.9, 0.99))
+            adam_betas=(0.9, 0.99),
+            # loading params:
+            backend=WSIBackend.CUCIM,
+            roi_type=ROIType.WHOLE,
+            image_key=SlideKey.IMAGE,
+            mask_key=SlideKey.MASK,
+        )
         default_kwargs.update(kwargs)
         super().__init__(**default_kwargs)
         self.class_names = ["ISUP 0", "ISUP 1", "ISUP 2", "ISUP 3", "ISUP 4", "ISUP 5"]
         if not is_running_in_azure_ml():
             self.max_epochs = 2
 
+    def get_test_plot_options(self) -> Set[PlotOption]:
+        plot_options = super().get_test_plot_options()
+        plot_options.update([PlotOption.SLIDE_THUMBNAIL, PlotOption.ATTENTION_HEATMAP])
+        return plot_options
+
 
 class DeepSMILETilesPanda(BaseMILTiles, BaseDeepSMILEPanda):
-    """ DeepSMILETilesPanda is derived from BaseMILTiles and BaseDeepSMILEPanda to inherit common behaviors from both
+    """DeepSMILETilesPanda is derived from BaseMILTiles and BaseDeepSMILEPanda to inherit common behaviors from both
     tiles basemil and panda specific configuration.
 
-    `is_finetune` sets the fine-tuning mode. `is_finetune` sets the fine-tuning mode. For fine-tuning, batch_size = 2
+    `tune_encoder` sets the fine-tuning mode of the encoder. For fine-tuning the encoder, batch_size = 2
     runs on multiple GPUs with ~ 6:24 min/epoch (train) and ~ 00:50 min/epoch (validation).
     """
 
     def __init__(self, **kwargs: Any) -> None:
         default_kwargs = dict(
             # declared in BaseMILTiles:
             is_caching=False,
             batch_size=8,
-            azure_datasets=[PANDA_5X_TILES_DATASET_ID, PANDA_DATASET_ID])
+            batch_size_inf=8,
+            azure_datasets=[PANDA_5X_TILES_DATASET_ID, PANDA_DATASET_ID],
+        )
         default_kwargs.update(kwargs)
         super().__init__(**default_kwargs)
 
     def setup(self) -> None:
         BaseMILTiles.setup(self)
-        # If no SSL checkpoint is provided, use the default one
-        self.ssl_checkpoint_run_id = self.ssl_checkpoint_run_id or innereye_ssl_checkpoint_binary
 
     def get_data_module(self) -> PandaTilesDataModule:
         return PandaTilesDataModule(
             root_path=self.local_datasets[0],
-            max_bag_size=self.max_bag_size,
             batch_size=self.batch_size,
+            batch_size_inf=self.batch_size_inf,
+            max_bag_size=self.max_bag_size,
             max_bag_size_inf=self.max_bag_size_inf,
             transforms_dict=self.get_transforms_dict(PandaTilesDataset.IMAGE_COLUMN),
             cache_mode=self.cache_mode,
             precache_location=self.precache_location,
             cache_dir=self.cache_dir,
             crossval_count=self.crossval_count,
             crossval_index=self.crossval_index,
             dataloader_kwargs=self.get_dataloader_kwargs(),
             seed=self.get_effective_random_seed(),
+            pl_replace_sampler_ddp=self.pl_replace_sampler_ddp,
         )
 
     def get_slides_dataset(self) -> Optional[PandaDataset]:
-        return PandaDataset(root=self.local_datasets[1])                             # type: ignore
-
-    def get_test_plot_options(self) -> Set[PlotOption]:
-        plot_options = super().get_test_plot_options()
-        plot_options.add(PlotOption.SLIDE_THUMBNAIL_HEATMAP)
-        return plot_options
+        return PandaDataset(root=self.local_datasets[1])  # type: ignore
 
 
 class TilesPandaImageNetMIL(DeepSMILETilesPanda):
     def __init__(self, **kwargs: Any) -> None:
-        super().__init__(encoder_type=ImageNetEncoder.__name__, **kwargs)
+        super().__init__(encoder_type=Resnet18.__name__, **kwargs)
 
 
 class TilesPandaImageNetSimCLRMIL(DeepSMILETilesPanda):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(encoder_type=ImageNetSimCLREncoder.__name__, **kwargs)
 
 
 class TilesPandaSSLMIL(DeepSMILETilesPanda):
     def __init__(self, **kwargs: Any) -> None:
+        # If no SSL checkpoint is provided, use the default one
+        self.ssl_checkpoint = self.ssl_checkpoint or CheckpointParser(innereye_ssl_checkpoint_binary)
         super().__init__(encoder_type=SSLEncoder.__name__, **kwargs)
 
 
 class TilesPandaHistoSSLMIL(DeepSMILETilesPanda):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(encoder_type=HistoSSLEncoder.__name__, **kwargs)
 
@@ -121,69 +125,62 @@
 class DeepSMILESlidesPanda(BaseMILSlides, BaseDeepSMILEPanda):
     """DeepSMILESlidesPanda is derived from BaseMILSlides and BaseDeeppSMILEPanda to inherits common behaviors from both
     slides basemil and panda specific configuration.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         default_kwargs = dict(
-            # declared in BaseMILSlides:
             level=1,
             tile_size=224,
-            random_offset=True,
             background_val=255,
-            azure_datasets=[PANDA_DATASET_ID],)
+            azure_datasets=[PANDA_DATASET_ID],
+        )
         default_kwargs.update(kwargs)
         super().__init__(**default_kwargs)
 
     def setup(self) -> None:
         BaseMILSlides.setup(self)
-        # If no SSL checkpoint is provided, use the default one
-        self.ssl_checkpoint_run_id = self.ssl_checkpoint_run_id or innereye_ssl_checkpoint_binary
 
     def get_dataloader_kwargs(self) -> dict:
-        return dict(
-            multiprocessing_context="spawn",
-            **super().get_dataloader_kwargs()
-        )
+        return dict(multiprocessing_context="spawn", **super().get_dataloader_kwargs())
 
     def get_data_module(self) -> PandaSlidesDataModule:
         return PandaSlidesDataModule(
             root_path=self.local_datasets[0],
             batch_size=self.batch_size,
-            level=self.level,
+            batch_size_inf=self.batch_size_inf,
             max_bag_size=self.max_bag_size,
             max_bag_size_inf=self.max_bag_size_inf,
-            tile_size=self.tile_size,
-            step=self.step,
-            random_offset=self.random_offset,
+            tiling_params=create_from_matching_params(self, TilingParams),
+            loading_params=create_from_matching_params(self, LoadingParams),
             seed=self.get_effective_random_seed(),
-            pad_full=self.pad_full,
-            background_val=self.background_val,
-            filter_mode=self.filter_mode,
-            transforms_dict=self.get_transforms_dict(PandaDataset.IMAGE_COLUMN),
+            transforms_dict=self.get_transforms_dict(SlideKey.IMAGE),
             crossval_count=self.crossval_count,
             crossval_index=self.crossval_index,
             dataloader_kwargs=self.get_dataloader_kwargs(),
+            pl_replace_sampler_ddp=self.pl_replace_sampler_ddp,
         )
 
     def get_slides_dataset(self) -> PandaDataset:
-        return PandaDataset(root=self.local_datasets[0])                             # type: ignore
+        return PandaDataset(root=self.local_datasets[0])  # type: ignore
 
 
 class SlidesPandaImageNetMIL(DeepSMILESlidesPanda):
     def __init__(self, **kwargs: Any) -> None:
-        super().__init__(encoder_type=ImageNetEncoder.__name__, **kwargs)
+        super().__init__(encoder_type=Resnet18.__name__, **kwargs)
 
 
 class SlidesPandaImageNetSimCLRMIL(DeepSMILESlidesPanda):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(encoder_type=ImageNetSimCLREncoder.__name__, **kwargs)
 
 
 class SlidesPandaSSLMIL(DeepSMILESlidesPanda):
     def __init__(self, **kwargs: Any) -> None:
+        # If no SSL checkpoint is provided, use the default one
+        self.ssl_checkpoint = self.ssl_checkpoint or CheckpointParser(innereye_ssl_checkpoint_binary)
         super().__init__(encoder_type=SSLEncoder.__name__, **kwargs)
 
 
 class SlidesPandaHistoSSLMIL(DeepSMILESlidesPanda):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(encoder_type=HistoSSLEncoder.__name__, **kwargs)
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/configs/classification/DeepSMILESlidesPandaBenchmark.py` & `hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILESlidesPandaBenchmark.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,156 +3,163 @@
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 
 
 from typing import Any, Dict, Callable, Union
 from torch import optim
 from monai.transforms import Compose, ScaleIntensityRanged, RandRotate90d, RandFlipd
-
+from health_cpath.configs.run_ids import innereye_ssl_checkpoint_binary
 from health_azure.utils import create_from_matching_params
-from health_ml.networks.layers.attention_layers import (
-    TransformerPooling,
-    TransformerPoolingBenchmark
-)
+from health_cpath.models.transforms import MetaTensorToTensord
+from health_cpath.preprocessing.loading import LoadingParams
+from health_cpath.utils.wsi_utils import TilingParams
+from health_ml.networks.layers.attention_layers import TransformerPooling, TransformerPoolingBenchmark
+from health_ml.utils.checkpoint_utils import CheckpointParser
 from health_ml.deep_learning_config import OptimizerParams
-from health_cpath.datasets.panda_dataset import PandaDataset
 from health_cpath.datamodules.panda_module_benchmark import PandaSlidesDataModuleBenchmark
 from health_cpath.models.encoders import (
     HistoSSLEncoder,
-    ImageNetEncoder_Resnet50,
     ImageNetSimCLREncoder,
+    Resnet50_NoPreproc,
     SSLEncoder,
 )
 from health_cpath.configs.classification.DeepSMILEPanda import DeepSMILESlidesPanda
-from health_cpath.models.deepmil import SlidesDeepMILModule
-from health_cpath.utils.deepmil_utils import EncoderParams, PoolingParams
+from health_cpath.models.deepmil import DeepMILModule
+from health_cpath.utils.deepmil_utils import ClassifierParams, EncoderParams, PoolingParams
 from health_cpath.utils.naming import MetricsKey, ModelKey, SlideKey
 
 
-class PandaSlidesDeepMILModuleBenchmark(SlidesDeepMILModule):
+class PandaSlidesDeepMILModuleBenchmark(DeepMILModule):
     """
     Myronenko et al. 2021 uses a cosine LR scheduler which needs to be defined in the PL module
-    Hence, inherited `PandaSlidesDeepMILModuleBenchmark` from `SlidesDeepMILModule`
+    Hence, inherited `PandaSlidesDeepMILModuleBenchmark` from `DeepMILModule`
     """
 
     def __init__(self, n_epochs: int, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.save_hyperparameters()
         self.n_epochs = n_epochs
 
-    def configure_optimizers(self) -> Dict[str, Any]:           # type: ignore
-        optimizer = optim.AdamW(self.parameters(), lr=self.optimizer_params.l_rate,
-                                weight_decay=self.optimizer_params.weight_decay)
+    def configure_optimizers(self) -> Dict[str, Any]:  # type: ignore
+        optimizer = optim.AdamW(
+            self.parameters(), lr=self.optimizer_params.l_rate, weight_decay=self.optimizer_params.weight_decay
+        )
         scheduler = optim.lr_scheduler.CosineAnnealingLR(optimizer=optimizer, T_max=self.n_epochs, eta_min=0)
         return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
 
 class DeepSMILESlidesPandaBenchmark(DeepSMILESlidesPanda):
     """
     Configuration for PANDA experiments from Myronenko et al. 2021:
     (https://link.springer.com/chapter/10.1007/978-3-030-87237-3_32)
-    `is_finetune` sets the fine-tuning mode. For fine-tuning,
-    batch_size = 2 runs on 8 GPUs with
-    ~ 6:24 min/epoch (train) and ~ 00:50 min/epoch (validation).
+    `tune_encoder` sets the fine-tuning mode of the encoder. For fine-tuning, batch_size = 2 runs on 8 GPUs
+    with ~ 6:24 min/epoch (train) and ~ 00:50 min/epoch (validation).
     """
 
     def __init__(self, **kwargs: Any) -> None:
         default_kwargs = dict(
             pool_type=TransformerPoolingBenchmark.__name__,
             num_transformer_pool_layers=4,
             num_transformer_pool_heads=8,
             pool_hidden_dim=2048,
             encoding_chunk_size=60,
             max_bag_size=56,
             batch_size=8,  # effective batch size = batch_size * num_GPUs
+            batch_size_inf=8,
             max_epochs=50,
             l_rate=3e-4,
             weight_decay=0,
-            primary_val_metric=MetricsKey.ACC)
+            primary_val_metric=MetricsKey.ACC,
+        )
         default_kwargs.update(kwargs)
         super().__init__(**default_kwargs)
 
     def setup(self) -> None:
         # Params specific to transformer pooling
         if self.pool_type in [TransformerPoolingBenchmark.__name__, TransformerPooling.__name__]:
             self.l_rate = 3e-5
             self.weight_decay = 0.1
         # Params specific to fine-tuning
-        if self.is_finetune:
+        if self.tune_encoder:
             self.batch_size = 2
+            self.batch_size_inf = 2
         super().setup()
 
     def get_transforms_dict(self, image_key: str) -> Dict[ModelKey, Union[Callable, None]]:
         # Use same transforms as demonstrated in
         # https://github.com/Project-MONAI/tutorials/blob/master/pathology/multiple_instance_learning/panda_mil_train_evaluate_pytorch_gpu.py
-        transform_train = Compose([
-            RandFlipd(keys=image_key, spatial_axis=0, prob=0.5),
-            RandFlipd(keys=image_key, spatial_axis=1, prob=0.5),
-            RandRotate90d(keys=image_key, prob=0.5),
-            ScaleIntensityRanged(keys=image_key, a_min=0.0, a_max=255.0)
-        ])
-        transform_inf = Compose([
-            ScaleIntensityRanged(keys=image_key, a_min=0.0, a_max=255.0)
-        ])
+        transform_train = Compose(
+            [
+                RandFlipd(keys=image_key, spatial_axis=0, prob=0.5),
+                RandFlipd(keys=image_key, spatial_axis=1, prob=0.5),
+                RandRotate90d(keys=image_key, prob=0.5),
+                ScaleIntensityRanged(keys=image_key, a_min=0.0, a_max=255.0),
+                MetaTensorToTensord(keys=image_key),  # rotate transforms add some metadata to affine matrix
+            ]
+        )
+        transform_inf = Compose(
+            [
+                ScaleIntensityRanged(keys=image_key, a_min=0.0, a_max=255.0),
+            ]
+        )
         return {ModelKey.TRAIN: transform_train, ModelKey.VAL: transform_inf, ModelKey.TEST: transform_inf}
 
     def get_data_module(self) -> PandaSlidesDataModuleBenchmark:  # type: ignore
         # Myronenko et al. 2021 uses 80-20 cross-val split and no hold-out test set
         # Hence, inherited `PandaSlidesDataModuleBenchmark` from `SlidesDataModule`
         return PandaSlidesDataModuleBenchmark(
             root_path=self.local_datasets[0],
-            max_bag_size=self.max_bag_size,
             batch_size=self.batch_size,
+            batch_size_inf=self.batch_size_inf,
+            max_bag_size=self.max_bag_size,
             max_bag_size_inf=self.max_bag_size_inf,
-            level=self.level,
-            tile_size=self.tile_size,
-            step=self.step,
-            random_offset=self.random_offset,
+            tiling_params=create_from_matching_params(self, TilingParams),
+            loading_params=create_from_matching_params(self, LoadingParams),
             seed=self.get_effective_random_seed(),
-            pad_full=self.pad_full,
-            background_val=self.background_val,
-            filter_mode=self.filter_mode,
-            transforms_dict=self.get_transforms_dict(PandaDataset.IMAGE_COLUMN),
+            transforms_dict=self.get_transforms_dict(SlideKey.IMAGE),
             crossval_count=self.crossval_count,
             crossval_index=self.crossval_index,
             dataloader_kwargs=self.get_dataloader_kwargs(),
+            pl_replace_sampler_ddp=self.pl_replace_sampler_ddp,
         )
 
-    def create_model(self) -> SlidesDeepMILModule:
+    def create_model(self) -> DeepMILModule:
         self.data_module = self.get_data_module()
         outputs_handler = self.get_outputs_handler()
         deepmil_module = PandaSlidesDeepMILModuleBenchmark(
             n_epochs=self.max_epochs,
             label_column=SlideKey.LABEL,
             n_classes=self.data_module.train_dataset.n_classes,
             class_names=self.class_names,
             class_weights=self.data_module.class_weights,
-            dropout_rate=self.dropout_rate,
             outputs_folder=self.outputs_folder,
-            ssl_ckpt_run_id=self.ssl_checkpoint_run_id,
             encoder_params=create_from_matching_params(self, EncoderParams),
             pooling_params=create_from_matching_params(self, PoolingParams),
+            classifier_params=create_from_matching_params(self, ClassifierParams),
             optimizer_params=create_from_matching_params(self, OptimizerParams),
             outputs_handler=outputs_handler,
+            analyse_loss=self.analyse_loss,
         )
         outputs_handler.set_slides_dataset_for_plots_handlers(self.get_slides_dataset())
         return deepmil_module
 
 
 class SlidesPandaImageNetMILBenchmark(DeepSMILESlidesPandaBenchmark):
     def __init__(self, **kwargs: Any) -> None:
-        super().__init__(encoder_type=ImageNetEncoder_Resnet50.__name__, **kwargs)
+        super().__init__(encoder_type=Resnet50_NoPreproc.__name__, **kwargs)
 
 
 class SlidesPandaImageNetSimCLRMILBenchmark(DeepSMILESlidesPandaBenchmark):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(encoder_type=ImageNetSimCLREncoder.__name__, **kwargs)
 
 
 class SlidesPandaSSLMILBenchmark(DeepSMILESlidesPandaBenchmark):
     def __init__(self, **kwargs: Any) -> None:
+        # If no SSL checkpoint is provided, use the default one
+        self.ssl_checkpoint = self.ssl_checkpoint or CheckpointParser(innereye_ssl_checkpoint_binary)
         super().__init__(encoder_type=SSLEncoder.__name__, **kwargs)
 
 
 class SlidesPandaHistoSSLMILBenchmark(DeepSMILESlidesPandaBenchmark):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(encoder_type=HistoSSLEncoder.__name__, **kwargs)
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datamodules/base_module.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datamodules/base_module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
+import logging
 import torch
-import numpy as np
 from enum import Enum
 from pathlib import Path
-from typing import Any, Callable, Dict, Generic, Optional, Sequence, Tuple, TypeVar, Union
+from typing import Any, Callable, Dict, Generic, List, Optional, Sequence, Tuple, TypeVar, Union
 
-from monai.data.dataset import CacheDataset, Dataset, PersistentDataset
 from pytorch_lightning import LightningDataModule
-from torch.utils.data import DataLoader
+from pytorch_lightning.overrides.distributed import UnrepeatedDistributedSampler
+from torch.utils.data import DataLoader, DistributedSampler
+from health_cpath.preprocessing.loading import LoadingParams
 
 from health_ml.utils.bag_utils import BagDataset, multibag_collate
 from health_ml.utils.common_utils import _create_generator
 
-from health_cpath.utils.wsi_utils import image_collate
+from health_cpath.utils.wsi_utils import TilingParams, image_collate
 from health_cpath.models.transforms import LoadTilesBatchd
 from health_cpath.datasets.base_dataset import SlidesDataset, TilesDataset
 from health_cpath.utils.naming import ModelKey
 
-from monai.transforms.compose import Compose
-from monai.transforms.io.dictionary import LoadImaged
-from monai.apps.pathology.transforms import TileOnGridd
-from monai.data.image_reader import WSIReader
+from monai.data.dataset import CacheDataset, Dataset, PersistentDataset
+from monai.transforms import Compose
+
 
-_SlidesOrTilesDataset = TypeVar('_SlidesOrTilesDataset', SlidesDataset, TilesDataset)
+_SlidesOrTilesDataset = TypeVar("_SlidesOrTilesDataset", SlidesDataset, TilesDataset)
 
 
 class CacheMode(Enum):
     NONE = "none"
     MEMORY = "memory"
     DISK = "disk"
 
@@ -43,85 +43,117 @@
 class HistoDataModule(LightningDataModule, Generic[_SlidesOrTilesDataset]):
     """Base class to load a histopathology dataset as train, val, test sets"""
 
     def __init__(
         self,
         root_path: Path,
         batch_size: int = 1,
+        batch_size_inf: Optional[int] = None,
         max_bag_size: int = 0,
         max_bag_size_inf: int = 0,
         seed: Optional[int] = None,
         transforms_dict: Optional[Dict[ModelKey, Union[Callable, None]]] = None,
         crossval_count: int = 0,
         crossval_index: int = 0,
+        pl_replace_sampler_ddp: bool = True,
         dataloader_kwargs: Optional[Dict[str, Any]] = None,
+        dataframe_kwargs: Optional[Dict[str, Any]] = None,
+        class_weights: Optional[torch.Tensor] = None,
     ) -> None:
         """
         :param root_path: Root directory of the source dataset.
         :param batch_size: Number of slides to load per batch.
+        :param batch_size_inf: Number of slides to load per batch during inference. If None, use batch_size.
         :param max_bag_size: Upper bound on number of tiles in each loaded bag during training stage. If 0 (default),
         will return all samples in each bag. If > 0 , bags larger than `max_bag_size` will yield
-        random subsets of instances. For SlideDataModule, this parameter is used in TileOnGridd Transform to set the
-        tile_count used for tiling on the fly at training time.
+        random subsets of instances. For SlideDataModule, this parameter is used in Rand/GridPatchd Transform to set the
+        num_patches used for tiling on the fly at training time.
         :param max_bag_size_inf: Upper bound on number of tiles in each loaded bag during validation and test stages.
         If 0 (default), will return all samples in each bag. If > 0 , bags larger than `max_bag_size_inf` will yield
-        random subsets of instances. For SlideDataModule, this parameter is used in TileOnGridd Transform to set the
-        tile_count used for tiling on the fly at validation and test time.
+        random subsets of instances. For SlideDataModule, this parameter is used in Rand/GridPatchd Transform to set the
+        num_patches used for tiling on the fly at validation and test time.
         :param seed: pseudorandom number generator seed to use for shuffling instances and bags. Note that randomness in
         train/val/test splits is handled independently in `get_splits()`. (default: `None`)
         :param transforms_dict: A dictionary that contains transform, or a composition of transforms using
         `monai.transforms.Compose`, to apply to the source dataset at training, validation and testing time.
         By default (`None`).
         :param crossval_count: Number of folds to perform.
         :param crossval_index: Index of the cross validation split to be performed.
+        :param pl_replace_sampler_ddp: If True, replace the sampler with a DistributedSampler when using DDP.
         :param dataloader_kwargs: Additional keyword arguments for the training, validation, and test dataloaders.
+        :param dataframe_kwargs: Keyword arguments to pass to `pd.read_csv()` when loading the dataset CSV.
+        :param class_weights: Class weights to use for the dataset. If None, will compute them from the dataset.
         """
 
+        batch_size_inf = batch_size_inf or batch_size
         super().__init__()
 
         self.root_path = root_path
         self.transforms_dict = transforms_dict
-        self.batch_size = batch_size
-        self.max_bag_size = max_bag_size
-        self.max_bag_size_inf = max_bag_size_inf
+        self.batch_sizes = {ModelKey.TRAIN: batch_size, ModelKey.VAL: batch_size_inf, ModelKey.TEST: batch_size_inf}
+        self.bag_sizes = {ModelKey.TRAIN: max_bag_size, ModelKey.VAL: max_bag_size_inf, ModelKey.TEST: max_bag_size_inf}
         self.crossval_count = crossval_count
         self.crossval_index = crossval_index
+        self.pl_replace_sampler_ddp = pl_replace_sampler_ddp
         self.train_dataset: _SlidesOrTilesDataset
         self.val_dataset: _SlidesOrTilesDataset
         self.test_dataset: _SlidesOrTilesDataset
+        self.dataframe_kwargs = dataframe_kwargs or {}
         self.train_dataset, self.val_dataset, self.test_dataset = self.get_splits()
-        self.class_weights = self.train_dataset.get_class_weights()
+        self.class_weights = class_weights if class_weights is not None else self.train_dataset.get_class_weights()
         self.seed = seed
         self.dataloader_kwargs = dataloader_kwargs or {}
 
     def get_splits(self) -> Tuple[_SlidesOrTilesDataset, _SlidesOrTilesDataset, _SlidesOrTilesDataset]:
         """Create the training, validation, and test datasets"""
         raise NotImplementedError
 
+    def _get_dataloader(
+        self, dataset: _SlidesOrTilesDataset, stage: ModelKey, shuffle: bool, **dataloader_kwargs: Any
+    ) -> DataLoader:
+        raise NotImplementedError
+
+    def _get_ddp_sampler(self, dataset: Dataset, stage: ModelKey) -> Optional[DistributedSampler]:
+        is_distributed = torch.distributed.is_initialized() and torch.distributed.get_world_size() > 1
+        if is_distributed and not self.pl_replace_sampler_ddp:
+            assert self.seed is not None, "seed must be set when using distributed training for reproducibility"
+            if stage == ModelKey.TRAIN:
+                logging.info("pl_replace_sampler_ddp is False, setting DistributedSampler for training dataloader.")
+                return DistributedSampler(dataset, shuffle=True, seed=self.seed)
+            else:
+                logging.info(
+                    "pl_replace_sampler_ddp is False, setting UnrepeatedDistributedSampler for validation and "
+                    "test dataloaders. This will ensure that each process gets a unique set of samples. "
+                    "If you want to use DistributedSampler, set pl_replace_sampler_ddp to True."
+                )
+                return UnrepeatedDistributedSampler(dataset, shuffle=False, seed=self.seed)
+        return None
+
     def train_dataloader(self) -> DataLoader:
-        return self._get_dataloader(self.train_dataset,  # type: ignore
-                                    shuffle=True,
-                                    stage=ModelKey.TRAIN,
-                                    **self.dataloader_kwargs)
+        return self._get_dataloader(
+            self.train_dataset, shuffle=True, stage=ModelKey.TRAIN, **self.dataloader_kwargs  # type: ignore
+        )
 
     def val_dataloader(self) -> DataLoader:
-        return self._get_dataloader(self.val_dataset,  # type: ignore
-                                    shuffle=False,
-                                    stage=ModelKey.VAL,
-                                    **self.dataloader_kwargs)
+        return self._get_dataloader(
+            self.val_dataset, shuffle=False, stage=ModelKey.VAL, **self.dataloader_kwargs  # type: ignore
+        )
 
     def test_dataloader(self) -> DataLoader:
-        return self._get_dataloader(self.test_dataset,  # type: ignore
-                                    shuffle=False,
-                                    stage=ModelKey.TEST,
-                                    **self.dataloader_kwargs)
+        return self._get_dataloader(
+            self.test_dataset, shuffle=False, stage=ModelKey.TEST, **self.dataloader_kwargs  # type: ignore
+        )
 
 
 class TilesDataModule(HistoDataModule[TilesDataset]):
-    """Base class to load the tiles of a dataset as train, val, test sets"""
+    """Base class to load the tiles of a dataset as train, val, test sets. Note that tiles are always shuffled by
+    default. This means that we sample a random subset of tiles from each bag at each epoch. This is different from
+    slides shuffling that is switched on during training time only. This is done to avoid overfitting to the order of
+    the tiles in each bag.
+    """
 
     def __init__(
         self,
         cache_mode: CacheMode = CacheMode.NONE,
         precache_location: CacheLocation = CacheLocation.NONE,
         cache_dir: Optional[Path] = None,
         **kwargs: Any,
@@ -194,24 +226,19 @@
                 memory_location = None  # type: ignore
 
             with dataset_pickle_path.open("rb") as f:
                 return torch.load(f, map_location=memory_location)
 
         generator = _create_generator(self.seed)
 
-        if stage in [ModelKey.VAL, ModelKey.TEST]:
-            eff_max_bag_size = self.max_bag_size_inf
-        else:
-            eff_max_bag_size = self.max_bag_size
-
         bag_dataset = BagDataset(
             tiles_dataset,  # type: ignore
             bag_ids=tiles_dataset.slide_ids,
-            max_bag_size=eff_max_bag_size,
-            shuffle_samples=shuffle,
+            max_bag_size=self.bag_sizes[stage],
+            shuffle_samples=True,
             generator=generator,
         )
         if self.transforms_dict and self.transforms_dict[stage]:
             transform = self.transforms_dict[stage]
         else:
             transform = LoadTilesBatchd(tiles_dataset.IMAGE_COLUMN)
 
@@ -224,118 +251,85 @@
         if dataset_pickle_path:
             dataset_pickle_path.parent.mkdir(parents=True, exist_ok=True)
             with dataset_pickle_path.open("wb") as f:
                 torch.save(transformed_bag_dataset, f)
 
         return transformed_bag_dataset
 
-    def _get_dataloader(self, dataset: TilesDataset, stage: ModelKey, shuffle: bool,
-                        **dataloader_kwargs: Any) -> DataLoader:
+    def _get_dataloader(
+        self, dataset: TilesDataset, stage: ModelKey, shuffle: bool, **dataloader_kwargs: Any
+    ) -> DataLoader:
         transformed_bag_dataset = self._load_dataset(dataset, stage=stage, shuffle=shuffle)
         bag_dataset: BagDataset = transformed_bag_dataset.data  # type: ignore
         generator = bag_dataset.bag_sampler.generator
+        sampler = self._get_ddp_sampler(transformed_bag_dataset, stage)
         return DataLoader(
             transformed_bag_dataset,
-            batch_size=self.batch_size,
+            batch_size=self.batch_sizes[stage],
             collate_fn=multibag_collate,
-            shuffle=shuffle,
+            sampler=sampler,
+            # sampler option is mutually exclusive with shuffle
+            shuffle=shuffle if sampler is None else None,  # type: ignore
             generator=generator,
             **dataloader_kwargs,
         )
 
 
 class SlidesDataModule(HistoDataModule[SlidesDataset]):
     """
     Base class to load the slides of a dataset as train, val, test sets. The slide data module performs tiling on the
     fly by default. One can specify the tiling strategies (background removal, overlapping tiles, padding, ...) through
     the class parameters.
     """
 
     def __init__(
         self,
-        level: Optional[int] = 1,
-        tile_size: Optional[int] = 224,
-        step: Optional[int] = None,
-        random_offset: Optional[bool] = True,
-        pad_full: Optional[bool] = False,
-        background_val: Optional[int] = 255,
-        filter_mode: Optional[str] = "min",
+        loading_params: LoadingParams,
+        tiling_params: TilingParams,
         **kwargs: Any,
     ) -> None:
         """
-        :param level: the whole slide image level at which the image is extracted, defaults to 1
-        this param is passed to the LoadImaged monai transform that loads a WSI with cucim backend
-        :param tile_size: size of the square tile, defaults to 224
-        this param is passed to TileOnGridd monai transform for tiling on the fly.
-        :param step: step size to create overlapping tiles, defaults to None (same as tile_size)
-        Use a step < tile_size to create overlapping tiles, analogousely a step > tile_size will skip some chunks in
-        the wsi. This param is passed to TileOnGridd monai transform for tiling on the fly.
-        :param random_offset: randomize position of the grid, instead of starting from the top-left corner,
-        defaults to True. This param is passed to TileOnGridd monai transform for tiling on the fly.
-        :param pad_full: pad image to the size evenly divisible by tile_size, defaults to False
-        This param is passed to TileOnGridd monai transform for tiling on the fly.
-        :param background_val: the background constant to ignore background tiles (e.g. 255 for white background),
-        defaults to 255. This param is passed to TileOnGridd monai transform for tiling on the fly.
-        :param filter_mode: mode must be in ["min", "max", "random"]. If total number of tiles is greater than
-        tile_count, then sort by intensity sum, and take the smallest (for min), largest (for max) or random (for
-        random) subset, defaults to "min" (which assumes background is high value). This param is passed to TileOnGridd
-        monai transform for tiling on the fly.
+        :param tiling_params: the tiling on the fly parameters.
+        :param loading_params: the loading parameters.
+        :param kwargs: additional parameters to pass to the parent class HistoDataModule
         """
         super().__init__(**kwargs)
-        self.level = level
-        self.tile_size = tile_size
-        self.step = step
-        self.random_offset = random_offset
-        self.pad_full = pad_full
-        self.background_val = background_val
-        self.filter_mode = filter_mode
-        # TileOnGridd transform expects None to select all foreground tile so we hardcode max_bag_size and
-        # max_bag_size_inf to None if set to 0
-        self.max_bag_size = None if self.max_bag_size == 0 else self.max_bag_size  # type: ignore
-        self.max_bag_size_inf = None if self.max_bag_size_inf == 0 else self.max_bag_size_inf  # type: ignore
+        self.tiling_params = tiling_params
+        self.loading_params = loading_params
 
     def _load_dataset(self, slides_dataset: SlidesDataset, stage: ModelKey) -> Dataset:
-        base_transform = Compose(
-            [
-                LoadImaged(
-                    keys=slides_dataset.IMAGE_COLUMN,
-                    reader=WSIReader,
-                    backend="cuCIM",
-                    dtype=np.uint8,
-                    level=self.level,
-                    image_only=True,
-                ),
-                TileOnGridd(
-                    keys=slides_dataset.IMAGE_COLUMN,
-                    tile_count=self.max_bag_size if stage == ModelKey.TRAIN else self.max_bag_size_inf,
-                    tile_size=self.tile_size,
-                    step=self.step,
-                    random_offset=self.random_offset if stage == ModelKey.TRAIN else False,
-                    pad_full=self.pad_full,
-                    background_val=self.background_val,
-                    filter_mode=self.filter_mode,
-                    return_list_of_dicts=True,
-                ),
-            ]
-        )
+        base_transform = Compose(self.get_tiling_transforms(stage=stage))
         if self.transforms_dict and self.transforms_dict[stage]:
-
             transforms = Compose([base_transform, self.transforms_dict[stage]]).flatten()
         else:
             transforms = base_transform
         # The tiling transform is randomized. Make them deterministic. This call needs to be
         # done on the final Compose, not at the level of the individual randomized transforms.
         transforms.set_random_state(seed=self.seed)
         return Dataset(slides_dataset, transforms)
 
-    def _get_dataloader(self, dataset: SlidesDataset, stage: ModelKey, shuffle: bool,
-                        **dataloader_kwargs: Any) -> DataLoader:
+    def _get_dataloader(
+        self, dataset: SlidesDataset, stage: ModelKey, shuffle: bool, **dataloader_kwargs: Any
+    ) -> DataLoader:
         transformed_slides_dataset = self._load_dataset(dataset, stage)
         generator = _create_generator(self.seed)
+        sampler = self._get_ddp_sampler(transformed_slides_dataset, stage)
         return DataLoader(
             transformed_slides_dataset,
-            batch_size=self.batch_size,
+            batch_size=self.batch_sizes[stage],
             collate_fn=image_collate,
-            shuffle=shuffle,
+            sampler=sampler,
+            # sampler option is mutually exclusive with shuffle
+            shuffle=shuffle if not sampler else None,  # type: ignore
             generator=generator,
             **dataloader_kwargs,
         )
+
+    def get_tiling_transforms(self, stage: ModelKey) -> List[Callable]:
+        """Returns the list of transforms to apply to the dataset to perform tiling on the fly. The transforms are
+        applied in the order they are returned by this method. To add additional transforms, override this method."""
+        return [
+            self.loading_params.get_load_roid_transform(),
+            self.tiling_params.get_tiling_transform(bag_size=self.bag_sizes[stage], stage=stage),
+            self.tiling_params.get_extract_coordinates_transform(),
+            self.tiling_params.get_split_transform(),
+        ]
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datamodules/panda_module.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datamodules/panda_module.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,49 +8,57 @@
 
 from health_cpath.datamodules.base_module import SlidesDataModule, TilesDataModule
 from health_cpath.datasets.panda_dataset import PandaDataset
 from health_cpath.datasets.panda_tiles_dataset import PandaTilesDataset
 
 
 class PandaTilesDataModule(TilesDataModule):
-    """ PandaTilesDataModule is the child class of TilesDataModule specific to PANDA dataset
+    """PandaTilesDataModule is the child class of TilesDataModule specific to PANDA dataset
     Method get_splits() returns the train, val, test splits from the PANDA dataset
     """
 
     def get_splits(self) -> Tuple[PandaTilesDataset, PandaTilesDataset, PandaTilesDataset]:
         dataset = PandaTilesDataset(self.root_path)
-        splits = DatasetSplits.from_proportions(dataset.dataset_df.reset_index(),
-                                                proportion_train=.8,
-                                                proportion_test=.1,
-                                                proportion_val=.1,
-                                                subject_column=dataset.TILE_ID_COLUMN,
-                                                group_column=dataset.SLIDE_ID_COLUMN)
+        splits = DatasetSplits.from_proportions(
+            dataset.dataset_df.reset_index(),
+            proportion_train=0.8,
+            proportion_test=0.1,
+            proportion_val=0.1,
+            subject_column=dataset.TILE_ID_COLUMN,
+            group_column=dataset.SLIDE_ID_COLUMN,
+        )
 
         if self.crossval_count > 1:
             # Function get_k_fold_cross_validation_splits() will concatenate train and val splits
             splits = splits.get_k_fold_cross_validation_splits(self.crossval_count)[self.crossval_index]
 
-        return (PandaTilesDataset(self.root_path, dataset_df=splits.train),
-                PandaTilesDataset(self.root_path, dataset_df=splits.val),
-                PandaTilesDataset(self.root_path, dataset_df=splits.test))
+        return (
+            PandaTilesDataset(self.root_path, dataset_df=splits.train),
+            PandaTilesDataset(self.root_path, dataset_df=splits.val),
+            PandaTilesDataset(self.root_path, dataset_df=splits.test),
+        )
 
 
 class PandaSlidesDataModule(SlidesDataModule):
-    """ PandaSlidesDataModule is the child class of SlidesDataModule specific to PANDA dataset
+    """PandaSlidesDataModule is the child class of SlidesDataModule specific to PANDA dataset
     Method get_splits() returns the train, val, test splits from the PANDA dataset
     """
 
     def get_splits(self) -> Tuple[PandaDataset, PandaDataset, PandaDataset]:
         dataset = PandaDataset(self.root_path)
-        splits = DatasetSplits.from_proportions(dataset.dataset_df.reset_index(),
-                                                proportion_train=.8,
-                                                proportion_test=.1,
-                                                proportion_val=.1,
-                                                subject_column=dataset.SLIDE_ID_COLUMN)
+        splits = DatasetSplits.from_proportions(
+            dataset.dataset_df.reset_index(),
+            proportion_train=0.8,
+            proportion_test=0.1,
+            proportion_val=0.1,
+            subject_column=dataset.slide_id_column,
+        )
 
         if self.crossval_count > 1:
             # Function get_k_fold_cross_validation_splits() will concatenate train and val splits
             splits = splits.get_k_fold_cross_validation_splits(self.crossval_count)[self.crossval_index]
 
-        return (PandaDataset(self.root_path, dataset_df=splits.train),
-                PandaDataset(self.root_path, dataset_df=splits.val),
-                PandaDataset(self.root_path, dataset_df=splits.test))
+        return (
+            PandaDataset(self.root_path, dataset_df=splits.train),
+            PandaDataset(self.root_path, dataset_df=splits.val),
+            PandaDataset(self.root_path, dataset_df=splits.test),
+        )
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datamodules/panda_module_benchmark.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datamodules/panda_module_benchmark.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,26 +13,30 @@
 from health_ml.utils.split_dataset import DatasetSplits
 
 from health_cpath.datamodules.base_module import SlidesDataModule
 from health_cpath.datasets.panda_dataset import PandaDataset
 
 
 class PandaSlidesDataModuleBenchmark(SlidesDataModule):
-    """ PandaSlidesDataModuleBenchmark is the child class of SlidesDataModule specific to PANDA dataset
+    """PandaSlidesDataModuleBenchmark is the child class of SlidesDataModule specific to PANDA dataset
     Method get_splits() returns the train, val, test splits from the PANDA dataset
     """
 
     def get_splits(self) -> Tuple[PandaDataset, PandaDataset, PandaDataset]:
         dataset = PandaDataset(self.root_path)
-        splits = DatasetSplits.from_proportions(dataset.dataset_df.reset_index(),
-                                                proportion_train=0.8,
-                                                proportion_test=0.0,
-                                                proportion_val=0.2,
-                                                subject_column=dataset.SLIDE_ID_COLUMN)
+        splits = DatasetSplits.from_proportions(
+            dataset.dataset_df.reset_index(),
+            proportion_train=0.8,
+            proportion_test=0.0,
+            proportion_val=0.2,
+            subject_column=dataset.slide_id_column,
+        )
 
         if self.crossval_count > 1:
             # Function get_k_fold_cross_validation_splits() will concatenate train and val splits
             splits = splits.get_k_fold_cross_validation_splits(self.crossval_count)[self.crossval_index]
 
-        return (PandaDataset(self.root_path, dataset_df=splits.train),
-                PandaDataset(self.root_path, dataset_df=splits.val),
-                PandaDataset(self.root_path, dataset_df=splits.val))
+        return (
+            PandaDataset(self.root_path, dataset_df=splits.train),
+            PandaDataset(self.root_path, dataset_df=splits.val),
+            PandaDataset(self.root_path, dataset_df=splits.val),
+        )
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datamodules/tcga_crck_module.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datamodules/tcga_crck_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,30 +8,33 @@
 from health_ml.utils.split_dataset import DatasetSplits
 
 from health_cpath.datamodules.base_module import TilesDataModule
 from health_cpath.datasets.tcga_crck_tiles_dataset import TcgaCrck_TilesDataset
 
 
 class TcgaCrckTilesDataModule(TilesDataModule):
-    """ TcgaCrckTilesDataModule is the child class of TilesDataModule specific to TCGA-Crck dataset
-    """
+    """TcgaCrckTilesDataModule is the child class of TilesDataModule specific to TCGA-Crck dataset"""
 
     def get_splits(self) -> Tuple[TcgaCrck_TilesDataset, TcgaCrck_TilesDataset, TcgaCrck_TilesDataset]:
         """
         :return: the train, val, test splits from the TCGA-Crck dataset
         """
         trainval_dataset = TcgaCrck_TilesDataset(self.root_path, train=True)
-        splits = DatasetSplits.from_proportions(trainval_dataset.dataset_df.reset_index(),
-                                                proportion_train=0.8,
-                                                proportion_test=0.0,
-                                                proportion_val=0.2,
-                                                subject_column=trainval_dataset.TILE_ID_COLUMN,
-                                                group_column=trainval_dataset.SLIDE_ID_COLUMN,
-                                                random_seed=5)
+        splits = DatasetSplits.from_proportions(
+            trainval_dataset.dataset_df.reset_index(),
+            proportion_train=0.8,
+            proportion_test=0.0,
+            proportion_val=0.2,
+            subject_column=trainval_dataset.TILE_ID_COLUMN,
+            group_column=trainval_dataset.SLIDE_ID_COLUMN,
+            random_seed=5,
+        )
 
         if self.crossval_count > 1:
             # Function get_k_fold_cross_validation_splits() will concatenate train and val splits
             splits = splits.get_k_fold_cross_validation_splits(self.crossval_count)[self.crossval_index]
 
-        return (TcgaCrck_TilesDataset(self.root_path, dataset_df=splits.train),
-                TcgaCrck_TilesDataset(self.root_path, dataset_df=splits.val),
-                TcgaCrck_TilesDataset(self.root_path, train=False))
+        return (
+            TcgaCrck_TilesDataset(self.root_path, dataset_df=splits.train),
+            TcgaCrck_TilesDataset(self.root_path, dataset_df=splits.val),
+            TcgaCrck_TilesDataset(self.root_path, train=False),
+        )
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datasets/base_dataset.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datasets/base_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 import pandas as pd
 import torch
 from sklearn.utils.class_weight import compute_class_weight
 from torch.utils.data import Dataset
 
-from health_cpath.utils.naming import SlideKey
+from health_cpath.utils.naming import SlideKey, TileKey
 
 
 DEFAULT_TRAIN_SPLIT_LABEL = "train"  # Value used to indicate the training split in `SPLIT_COLUMN`
 DEFAULT_VAL_SPLIT_LABEL = "val"  # Value used to indicate the validation split in `SPLIT_COLUMN`
 DEFAULT_TEST_SPLIT_LABEL = "test"  # Value used to indicate the test split in `SPLIT_COLUMN`
 DEFAULT_LABEL_COLUMN = "label"  # Default column name for the label column
 
@@ -29,61 +29,67 @@
     :param IMAGE_COLUMN: CSV column name for relative path to image file.
     :param PATH_COLUMN: CSV column name for relative path to image file. Replicated to propagate the path to the batch.
     :param SPLIT_COLUMN: CSV column name for train/test split (optional).
     :param TILE_X_COLUMN: CSV column name for horizontal tile coordinate (optional).
     :param TILE_Y_COLUMN: CSV column name for vertical tile coordinate (optional).
     :param DEFAULT_CSV_FILENAME: Default name of the dataset CSV at the dataset rood directory.
     """
+
     TILE_ID_COLUMN: str = 'tile_id'
     SLIDE_ID_COLUMN: str = 'slide_id'
     IMAGE_COLUMN: str = 'image'
     PATH_COLUMN: str = 'image_path'
     SPLIT_COLUMN: Optional[str] = 'split'
     TILE_X_COLUMN: Optional[str] = 'tile_x'
     TILE_Y_COLUMN: Optional[str] = 'tile_y'
 
     DEFAULT_CSV_FILENAME: str = "dataset.csv"
 
-    def __init__(self,
-                 root: Union[str, Path],
-                 dataset_csv: Optional[Union[str, Path]] = None,
-                 dataset_df: Optional[pd.DataFrame] = None,
-                 train: Optional[bool] = None,
-                 validate_columns: bool = True,
-                 label_column: str = DEFAULT_LABEL_COLUMN,
-                 n_classes: int = 1) -> None:
+    def __init__(
+        self,
+        root: Union[str, Path],
+        dataset_csv: Optional[Union[str, Path]] = None,
+        dataset_df: Optional[pd.DataFrame] = None,
+        train: Optional[bool] = None,
+        validate_columns: bool = True,
+        label_column: str = DEFAULT_LABEL_COLUMN,
+        n_classes: int = 1,
+        dataframe_kwargs: Dict[str, Any] = {},
+    ) -> None:
         """
         :param root: Root directory of the dataset.
         :param dataset_csv: Full path to a dataset CSV file, containing at least
         `TILE_ID_COLUMN`, `SLIDE_ID_COLUMN`, and `IMAGE_COLUMN`. If omitted, the CSV will be read
         from `"{root}/{DEFAULT_CSV_FILENAME}"`.
         :param dataset_df: A potentially pre-processed dataframe in the same format as would be read
         from the dataset CSV file, e.g. after some filtering. If given, overrides `dataset_csv`.
         :param train: If `True`, loads only the training split (resp. `False` for test split). By
         default (`None`), loads the entire dataset as-is.
         :param validate_columns: Whether to call `validate_columns()` at the end of `__init__()`.
         `validate_columns()` checks that the loaded data frame for the dataset contains the expected column names
         for this class
         :param label_column: CSV column name for tile label. Defaults to `DEFAULT_LABEL_COLUMN="label"`.
         :param n_classes: Number of classes indexed in `label_column`. Default is 1 for binary classification.
+        :param dataframe_kwargs: Keyword arguments to pass to `pd.read_csv()` when loading the dataset CSV.
         """
         if self.SPLIT_COLUMN is None and train is not None:
             raise ValueError("Train/test split was specified but dataset has no split column")
 
         self.root_dir = Path(root)
         self.label_column = label_column
         self.n_classes = n_classes
 
         if dataset_df is not None:
             self.dataset_csv = None
         else:
             self.dataset_csv = dataset_csv or self.root_dir / self.DEFAULT_CSV_FILENAME
-            dataset_df = pd.read_csv(self.dataset_csv)
+            dataset_df = pd.read_csv(self.dataset_csv, **dataframe_kwargs)
 
-        dataset_df = dataset_df.set_index(self.TILE_ID_COLUMN)
+        if dataset_df.index.name != self.TILE_ID_COLUMN:
+            dataset_df = dataset_df.set_index(self.TILE_ID_COLUMN)
         if train is None:
             self.dataset_df = dataset_df
         else:
             split = DEFAULT_TRAIN_SPLIT_LABEL if train else DEFAULT_TEST_SPLIT_LABEL
             self.dataset_df = dataset_df[dataset_df[self.SPLIT_COLUMN] == split]
 
         if validate_columns:
@@ -91,32 +97,35 @@
 
     def validate_columns(self) -> None:
         """Check that loaded dataframe contains expected columns, raises `ValueError` otherwise.
 
         If the constructor is overloaded in a subclass, you can pass `validate_columns=False` and
         call `validate_columns()` after creating derived columns, for example.
         """
-        columns = [self.SLIDE_ID_COLUMN, self.IMAGE_COLUMN, self.label_column,
-                   self.SPLIT_COLUMN, self.TILE_X_COLUMN, self.TILE_Y_COLUMN]
+        columns = [
+            self.SLIDE_ID_COLUMN,
+            self.IMAGE_COLUMN,
+            self.label_column,
+            self.SPLIT_COLUMN,
+            self.TILE_X_COLUMN,
+            self.TILE_Y_COLUMN,
+        ]
         columns_not_found = []
         for column in columns:
             if column is not None and column not in self.dataset_df.columns:
                 columns_not_found.append(column)
         if len(columns_not_found) > 0:
             raise ValueError(f"Expected columns '{columns_not_found}' not found in the dataframe")
 
     def __len__(self) -> int:
         return self.dataset_df.shape[0]
 
     def __getitem__(self, index: int) -> Dict[str, Any]:
         tile_id = self.dataset_df.index[index]
-        sample = {
-            self.TILE_ID_COLUMN: tile_id,
-            **self.dataset_df.loc[tile_id].to_dict()
-        }
+        sample = {self.TILE_ID_COLUMN: tile_id, **self.dataset_df.loc[tile_id].to_dict()}
         sample[self.IMAGE_COLUMN] = str(self.root_dir / sample.pop(self.IMAGE_COLUMN))
         # we're replicating this column because we want to propagate the path to the batch
         sample[self.PATH_COLUMN] = sample[self.IMAGE_COLUMN]
         return sample
 
     @property
     def slide_ids(self) -> pd.Series:
@@ -127,115 +136,138 @@
 
     def get_class_weights(self) -> torch.Tensor:
         slide_labels = self.get_slide_labels()
         classes = np.unique(slide_labels)
         class_weights = compute_class_weight(class_weight='balanced', classes=classes, y=slide_labels)
         return torch.as_tensor(class_weights)
 
+    def copy_coordinates_columns(self) -> None:
+        """Copy columns "left" --> "tile_x" and "top" --> "tile_y" to be consistent with TilesDataset `TILE_X_COLUMN`
+        and `TILE_Y_COLUMN`."""
+
+        if TileKey.TILE_LEFT in self.dataset_df.columns:
+            self.dataset_df = self.dataset_df.assign(**{TilesDataset.TILE_X_COLUMN: self.dataset_df[TileKey.TILE_LEFT]})
+        if TileKey.TILE_TOP in self.dataset_df.columns:
+            self.dataset_df = self.dataset_df.assign(**{TilesDataset.TILE_Y_COLUMN: self.dataset_df[TileKey.TILE_TOP]})
+
+
+DEFAULT_DATASET_CSV = "dataset.csv"
+
 
 class SlidesDataset(Dataset):
     """Base class for datasets of WSIs, iterating dictionaries of image paths and metadata.
 
     The output dictionaries are indexed by `..utils.naming.SlideKey`.
-
-    :param SLIDE_ID_COLUMN: CSV column name for slide ID.
-    :param IMAGE_COLUMN: CSV column name for relative path to image file.
-    :param SPLIT_COLUMN: CSV column name for train/test split (optional).
-    :param DEFAULT_CSV_FILENAME: Default name of the dataset CSV at the dataset rood directory.
     """
-    SLIDE_ID_COLUMN: str = 'slide_id'
-    IMAGE_COLUMN: str = 'image'
-    MASK_COLUMN: Optional[str] = None
-    SPLIT_COLUMN: Optional[str] = None
 
-    METADATA_COLUMNS: Tuple[str, ...] = ()
-
-    DEFAULT_CSV_FILENAME: str = "dataset.csv"
-
-    def __init__(self,
-                 root: Union[str, Path],
-                 dataset_csv: Optional[Union[str, Path]] = None,
-                 dataset_df: Optional[pd.DataFrame] = None,
-                 train: Optional[bool] = None,
-                 validate_columns: bool = True,
-                 label_column: str = DEFAULT_LABEL_COLUMN,
-                 n_classes: int = 1) -> None:
+    def __init__(
+        self,
+        root: Union[str, Path],
+        dataset_csv: Optional[Union[str, Path]] = None,
+        dataset_df: Optional[pd.DataFrame] = None,
+        train: Optional[bool] = None,
+        validate_columns: bool = True,
+        label_column: str = DEFAULT_LABEL_COLUMN,
+        n_classes: int = 1,
+        dataframe_kwargs: Dict[str, Any] = {},
+        default_csv_filename: str = DEFAULT_DATASET_CSV,
+        slide_id_column: str = "slide_id",
+        image_column: str = "image",
+        mask_column: Optional[str] = None,
+        split_column: Optional[str] = None,
+        metadata_columns: Tuple[str, ...] = (),
+    ) -> None:
         """
         :param root: Root directory of the dataset.
         :param dataset_csv: Full path to a dataset CSV file, containing at least
-        `TILE_ID_COLUMN`, `SLIDE_ID_COLUMN`, and `IMAGE_COLUMN`. If omitted, the CSV will be read
-        from `"{root}/{DEFAULT_CSV_FILENAME}"`.
+            `slide_id_column` and `image_column`. If omitted, the CSV will be read
+            from `"{root}/{DEFAULT_CSV_FILENAME}"`.
         :param dataset_df: A potentially pre-processed dataframe in the same format as would be read
-        from the dataset CSV file, e.g. after some filtering. If given, overrides `dataset_csv`.
+            from the dataset CSV file, e.g. after some filtering. If given, overrides `dataset_csv`.
         :param train: If `True`, loads only the training split (resp. `False` for test split). By
-        default (`None`), loads the entire dataset as-is.
+            default (`None`), loads the entire dataset as-is.
         :param validate_columns: Whether to call `validate_columns()` at the end of `__init__()`.
-        `validate_columns()` checks that the loaded data frame for the dataset contains the expected column names
-        for this class
+            `validate_columns()` checks that the loaded data frame for the dataset contains the expected column names
+            for this class
         :param label_column: CSV column name for tile label. Default is `DEFAULT_LABEL_COLUMN="label"`.
         :param n_classes: Number of classes indexed in `label_column`. Default is 1 for binary classification.
+        :param dataframe_kwargs: Keyword arguments to pass to `pd.read_csv()` when loading the dataset CSV.
+        :param slide_id_column: CSV column name for slide ID. Default is `slide_id`.
+        :param image_column: CSV column name for relative path to image file. Default is `image`.
+        :param mask_column: CSV column name for relative path to mask file. Default is `None`.
+        :param split_column: CSV column name for train/test split. Default is `None`.
+        :param default_csv_filename: Default name of the dataset CSV at the dataset root directory.
         """
-        if self.SPLIT_COLUMN is None and train is not None:
-            raise ValueError("Train/test split was specified but dataset has no split column")
-
         self.root_dir = Path(root)
         self.label_column = label_column
         self.n_classes = n_classes
+        self.dataframe_kwargs = dataframe_kwargs
+        self.slide_id_column = slide_id_column
+        self.image_column = image_column
+        self.mask_column = mask_column
+        self.split_column = split_column
+        self.metadata_columns = metadata_columns
+        self.default_csv_filename = default_csv_filename
+        if self.split_column is None and train is not None:
+            raise ValueError("Train/test split was specified but dataset has no split column")
 
         if dataset_df is not None:
             self.dataset_csv = None
         else:
-            self.dataset_csv = dataset_csv or self.root_dir / self.DEFAULT_CSV_FILENAME
-            dataset_df = pd.read_csv(self.dataset_csv)
+            self.dataset_csv = dataset_csv or self.root_dir / self.default_csv_filename
+            dataset_df = pd.read_csv(self.dataset_csv, **self.dataframe_kwargs)
 
-        dataset_df = dataset_df.set_index(self.SLIDE_ID_COLUMN)
+        if dataset_df.index.name != self.slide_id_column:
+            dataset_df = dataset_df.set_index(self.slide_id_column)
         if train is None:
             self.dataset_df = dataset_df
         else:
             split = DEFAULT_TRAIN_SPLIT_LABEL if train else DEFAULT_TEST_SPLIT_LABEL
-            self.dataset_df = dataset_df[dataset_df[self.SPLIT_COLUMN] == split]
+            self.dataset_df = dataset_df[dataset_df[self.split_column] == split]
 
         if validate_columns:
             self.validate_columns()
 
     def validate_columns(self) -> None:
         """Check that loaded dataframe contains expected columns, raises `ValueError` otherwise.
 
         If the constructor is overloaded in a subclass, you can pass `validate_columns=False` and
         call `validate_columns()` after creating derived columns, for example.
         """
-        columns = [self.IMAGE_COLUMN, self.label_column, self.MASK_COLUMN,
-                   self.SPLIT_COLUMN] + list(self.METADATA_COLUMNS)
-        columns_not_found = []
-        for column in columns:
-            if column is not None and column not in self.dataset_df.columns:
-                columns_not_found.append(column)
+        mandatory_columns = {self.image_column, self.label_column, self.mask_column, self.split_column}
+        optional_columns = (
+            set(self.dataframe_kwargs["usecols"]) if "usecols" in self.dataframe_kwargs else set(self.metadata_columns)
+        )
+        columns = mandatory_columns.union(optional_columns)
+        # slide_id_column is used for indexing and is not in df.columns anymore
+        # None might be in columns if split_column is None
+        columns_not_found = columns - set(self.dataset_df.columns) - {None, self.slide_id_column}
         if len(columns_not_found) > 0:
             raise ValueError(f"Expected columns '{columns_not_found}' not found in the dataframe")
 
     def __len__(self) -> int:
         return self.dataset_df.shape[0]
 
     def __getitem__(self, index: int) -> Dict[SlideKey, Any]:
         slide_id = self.dataset_df.index[index]
         slide_row = self.dataset_df.loc[slide_id]
         sample = {SlideKey.SLIDE_ID: slide_id}
 
-        rel_image_path = slide_row[self.IMAGE_COLUMN]
+        rel_image_path = slide_row[self.image_column]
         sample[SlideKey.IMAGE] = str(self.root_dir / rel_image_path)
         # we're replicating this column because we want to propagate the path to the batch
         sample[SlideKey.IMAGE_PATH] = sample[SlideKey.IMAGE]
 
-        if self.MASK_COLUMN:
-            rel_mask_path = slide_row[self.MASK_COLUMN]
+        if self.mask_column:
+            rel_mask_path = slide_row[self.mask_column]
             sample[SlideKey.MASK] = str(self.root_dir / rel_mask_path)
             sample[SlideKey.MASK_PATH] = sample[SlideKey.MASK]
 
         sample[SlideKey.LABEL] = slide_row[self.label_column]
-        sample[SlideKey.METADATA] = {col: slide_row[col] for col in self.METADATA_COLUMNS}
+        sample[SlideKey.METADATA] = {col: slide_row[col] for col in self.metadata_columns}
         return sample
 
     @classmethod
     def has_mask(cls) -> bool:
         return cls.MASK_COLUMN is not None
 
     def get_slide_labels(self) -> pd.Series:
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datasets/dataset_return_index.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datasets/dataset_return_index.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datasets/default_paths.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datasets/default_paths.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datasets/panda_tiles_dataset.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datasets/panda_tiles_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Any, Callable, Optional, Tuple, Union
 
 import pandas as pd
 from torchvision.datasets.vision import VisionDataset
 
 from health_cpath.datasets.base_dataset import TilesDataset
 from health_cpath.models.transforms import load_pil_image
-from health_cpath.utils.naming import TileKey
 
 from health_cpath.datasets.dataset_return_index import DatasetWithReturnIndex
 
 
 class PandaTilesDataset(TilesDataset):
     """
     Dataset class for loading PANDA tiles.
@@ -24,89 +23,92 @@
     - `'slide_id'` (str): parent slide ID (`'image_id'` in the PANDA dataset)
     - `'tile_id'` (str)
     - `'image'` (`PIL.Image`): RGB tile
     - `'mask'` (str): path to mask PNG file
     - `'tile_x'`, `'tile_y'` (int): top-right tile coordinates
     - `'data_provider'`, `'slide_isup_grade'`, `'slide_gleason_score'` (str): parent slide metadata
     """
+
     SPLIT_COLUMN = None  # PANDA does not have an official train/test split
 
-    def __init__(self,
-                 root: Path,
-                 dataset_csv: Optional[Union[str, Path]] = None,
-                 dataset_df: Optional[pd.DataFrame] = None,
-                 occupancy_threshold: Optional[float] = None,
-                 random_subset_fraction: Optional[float] = None,
-                 label_column: str = "slide_isup_grade",
-                 n_classes: int = 6) -> None:
+    def __init__(
+        self,
+        root: Path,
+        dataset_csv: Optional[Union[str, Path]] = None,
+        dataset_df: Optional[pd.DataFrame] = None,
+        occupancy_threshold: Optional[float] = None,
+        random_subset_fraction: Optional[float] = None,
+        label_column: str = "slide_isup_grade",
+        n_classes: int = 6,
+    ) -> None:
         """
         :param root: Root directory of the dataset.
         :param dataset_csv: Full path to a dataset CSV file, containing at least
         `TILE_ID_COLUMN`, `SLIDE_ID_COLUMN`, and `IMAGE_COLUMN`. If omitted, the CSV will be read
         from `"{root}/{DEFAULT_CSV_FILENAME}"`.
         :param dataset_df: A potentially pre-processed dataframe in the same format as would be read
         from the dataset CSV file, e.g. after some filtering. If given, overrides `dataset_csv`.
         :occupancy_threshold: A value between 0-1 such that only tiles with occupancy > occupancy_threshold
         will be selected. If 0, all tiles are selected. If `None` (default), all tiles are selected.
         :random_subset_fraction: A value > 0 and <=1 such that this proportion of tiles will be randomly selected.
         If 1, all tiles are selected. If `None` (default), all tiles are selected.
         """
-        super().__init__(root=Path(root),
-                         dataset_csv=dataset_csv,
-                         dataset_df=dataset_df,
-                         train=None,
-                         validate_columns=False,
-                         label_column=label_column,
-                         n_classes=n_classes)
+        super().__init__(
+            root=Path(root),
+            dataset_csv=dataset_csv,
+            dataset_df=dataset_df,
+            train=None,
+            validate_columns=False,
+            label_column=label_column,
+            n_classes=n_classes,
+        )
 
         if occupancy_threshold is not None:
             if (occupancy_threshold < 0) or (occupancy_threshold > 1):
                 raise ValueError(f"Occupancy threshold value {occupancy_threshold} should be in range 0-1.")
-            dataset_df_filtered = self.dataset_df.loc[
-                self.dataset_df['occupancy'] > occupancy_threshold
-            ]
+            dataset_df_filtered = self.dataset_df.loc[self.dataset_df['occupancy'] > occupancy_threshold]
             self.dataset_df = dataset_df_filtered
 
         if random_subset_fraction is not None:
             if (random_subset_fraction <= 0) or (random_subset_fraction > 1):
                 raise ValueError(f"Random subset fraction value {random_subset_fraction} should be > 0 and < = 1.")
             df_length_random_subset_fraction = round(len(self.dataset_df) * random_subset_fraction)
             dataset_df_filtered = self.dataset_df.sample(n=df_length_random_subset_fraction)
             self.dataset_df = dataset_df_filtered
 
-        # Copy columns "left" --> "tile_x" and "top" --> "tile_y"
-        # to be consistent with TilesDataset `TILE_X_COLUMN` and `TILE_Y_COLUMN`
-        if TileKey.TILE_LEFT in self.dataset_df.columns:
-            self.dataset_df[TilesDataset.TILE_X_COLUMN] = self.dataset_df[TileKey.TILE_LEFT]
-        if TileKey.TILE_TOP in self.dataset_df.columns:
-            self.dataset_df[TilesDataset.TILE_Y_COLUMN] = self.dataset_df[TileKey.TILE_TOP]
+        self.copy_coordinates_columns()
         self.validate_columns()
 
 
 class PandaTilesDatasetReturnImageLabel(VisionDataset):
     """
     Any dataset used in SSL needs to return a tuple where the first element is the image and the second is a
     class label.
     """
+
     occupancy_threshold = 0
     random_subset_fraction = 1
 
-    def __init__(self,
-                 root: Path,
-                 dataset_csv: Optional[Union[str, Path]] = None,
-                 dataset_df: Optional[pd.DataFrame] = None,
-                 transform: Optional[Callable] = None,
-                 **kwargs: Any) -> None:
+    def __init__(
+        self,
+        root: Path,
+        dataset_csv: Optional[Union[str, Path]] = None,
+        dataset_df: Optional[pd.DataFrame] = None,
+        transform: Optional[Callable] = None,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(root=root, transform=transform)
 
-        self.base_dataset = PandaTilesDataset(root=root,
-                                              dataset_csv=dataset_csv,
-                                              dataset_df=dataset_df,
-                                              occupancy_threshold=self.occupancy_threshold,
-                                              random_subset_fraction=self.random_subset_fraction)
+        self.base_dataset = PandaTilesDataset(
+            root=root,
+            dataset_csv=dataset_csv,
+            dataset_df=dataset_df,
+            occupancy_threshold=self.occupancy_threshold,
+            random_subset_fraction=self.random_subset_fraction,
+        )
 
     def __getitem__(self, index: int) -> Tuple:  # type: ignore
         sample = self.base_dataset[index]
         # TODO change to a meaningful evaluation
         image = load_pil_image(sample[self.base_dataset.IMAGE_COLUMN])
         if self.transform:
             image = self.transform(image)
@@ -120,10 +122,11 @@
 
 class PandaTilesDatasetWithReturnIndex(DatasetWithReturnIndex, PandaTilesDatasetReturnImageLabel):
     """
     Any dataset used in SSL needs to inherit from DatasetWithReturnIndex as well as VisionData.
     This class is just a shorthand notation for this double inheritance. Please note that this class needs
     to override __getitem__(), this is why we need a separate PandaTilesDatasetReturnImageLabel.
     """
+
     @property
     def num_classes(self) -> int:
         return 2
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datasets/tcga_crck_tiles_dataset.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datasets/tcga_crck_tiles_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,52 +20,54 @@
 
     Iterating over this dataset returns a dictionary containing:
     - `'slide_id'` (str): parent slide ID
     - `'tile_id'` (str)
     - `'image'` (`PIL.Image`): RGB tile
     - `'label'` (str): MSS (0) vs MSIMUT (1)
     """
+
     TILE_X_COLUMN = TILE_Y_COLUMN = None  # no tile coordinates available
     # This dataset conforms to all other defaults in TilesDataset
 
 
 class TcgaCrck_TilesDatasetReturnImageLabel(VisionDataset):
     """
     Any dataset used in SSL needs to return a tuple where the first element is the image and the second is a
     class label.
     """
 
-    def __init__(self,
-                 root: Union[str, Path],
-                 dataset_csv: Optional[Union[str, Path]] = None,
-                 dataset_df: Optional[pd.DataFrame] = None,
-                 train: Optional[bool] = None,
-                 transform: Optional[Callable] = None,
-                 **kwargs: Any) -> None:
+    def __init__(
+        self,
+        root: Union[str, Path],
+        dataset_csv: Optional[Union[str, Path]] = None,
+        dataset_df: Optional[pd.DataFrame] = None,
+        train: Optional[bool] = None,
+        transform: Optional[Callable] = None,
+        **kwargs: Any
+    ) -> None:
         super().__init__(root=root, transform=transform)
-        self.base_dataset = TcgaCrck_TilesDataset(root=root,
-                                                  dataset_csv=dataset_csv,
-                                                  dataset_df=dataset_df,
-                                                  train=train)
+        self.base_dataset = TcgaCrck_TilesDataset(
+            root=root, dataset_csv=dataset_csv, dataset_df=dataset_df, train=train
+        )
 
     def __getitem__(self, index: int) -> Tuple:  # type: ignore
         sample = self.base_dataset[index]
         # TODO change to a meaningful evaluation
         image = load_pil_image(sample[self.base_dataset.IMAGE_COLUMN])
         if self.transform:
             image = self.transform(image)
         return image, sample[self.base_dataset.label_column]
 
     def __len__(self) -> int:
         return len(self.base_dataset)
 
 
-class TcgaCrck_TilesDatasetWithReturnIndex(DatasetWithReturnIndex,
-                                           TcgaCrck_TilesDatasetReturnImageLabel):
+class TcgaCrck_TilesDatasetWithReturnIndex(DatasetWithReturnIndex, TcgaCrck_TilesDatasetReturnImageLabel):
     """
     Any dataset used in SSL needs to inherit from DataClassBaseWithReturnIndex as well as VisionData.
     This class is just a shorthand notation for this double inheritance. Please note that this class needs
     to override __getitem__(), this is why we need a separate PandaTilesDatasetReturnImageLabel.
     """
+
     @property
     def num_classes(self) -> int:
         return 2
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/datasets/tcga_prad_dataset.py` & `hi-ml-cpath-0.3.0/src/health_cpath/datasets/panda_dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
-
+import pandas as pd
 from pathlib import Path
-from typing import Optional, Union
+from typing import Any, Dict, Union, Optional
+from health_cpath.datasets.base_dataset import SlidesDataset
 
-import pandas as pd
 
-from health_cpath.datasets.base_dataset import DEFAULT_LABEL_COLUMN, SlidesDataset
+class PandaColumns:
+    SLIDE_ID = 'image_id'
+    IMAGE = 'image'
+    MASK = 'mask'
+    METADATA = ('data_provider', 'isup_grade', 'gleason_score')
 
 
-class TcgaPradDataset(SlidesDataset):
-    """Dataset class for loading TCGA-PRAD slides.
+PANDA_CSV_FILENAME = "train.csv"
 
-    Iterating over this dataset returns a dictionary containing:
-    - `'slide_id'` (str)
-    - `'case_id'` (str)
-    - `'image_path'` (str): absolute slide image path
-    - `'label'` (int, 0 or 1): label for predicting positive or negative
-    """
-    IMAGE_COLUMN: str = 'image_path'
 
-    DEFAULT_CSV_FILENAME: str = "dataset.csv"
+class PandaDataset(SlidesDataset):
+    """Dataset class for loading files from the PANDA challenge dataset.
+
+    Iterating over this dataset returns a dictionary following the `SlideKey` schema plus meta-data
+    from the original dataset (`'data_provider'`, `'isup_grade'`, and `'gleason_score'`).
+
+    Ref.: https://www.kaggle.com/c/prostate-cancer-grade-assessment/overview
+    """
 
-    def __init__(self, root: Union[str, Path],
-                 dataset_csv: Optional[Union[str, Path]] = None,
-                 dataset_df: Optional[pd.DataFrame] = None,
-                 label_column: str = DEFAULT_LABEL_COLUMN) -> None:
-        """
-        :param root: Root directory of the dataset.
-        :param dataset_csv: Full path to a dataset CSV file. If omitted, the CSV will be read from
-        `"{root}/{DEFAULT_CSV_FILENAME}"`.
-        :param dataset_df: A potentially pre-processed dataframe in the same format as would be read
-        from the dataset CSV file, e.g. after some filtering. If given, overrides `dataset_csv`.
-        """
-        super().__init__(root, dataset_csv, dataset_df, validate_columns=False, label_column=label_column)
-        # Example of how to define a custom label column from existing columns:
-        self.dataset_df[self.label_column] = (self.dataset_df['label1']
-                                              | self.dataset_df['label2']).astype(int)  # noqa: W503
+    def __init__(
+        self,
+        root: Union[str, Path],
+        dataset_csv: Optional[Union[str, Path]] = None,
+        dataset_df: Optional[pd.DataFrame] = None,
+        label_column: str = "isup_grade",
+        n_classes: int = 6,
+        dataframe_kwargs: Dict[str, Any] = {},
+    ) -> None:
+        super().__init__(
+            root,
+            dataset_csv,
+            dataset_df,
+            validate_columns=False,
+            label_column=label_column,
+            n_classes=n_classes,
+            dataframe_kwargs=dataframe_kwargs,
+            slide_id_column=PandaColumns.SLIDE_ID,
+            image_column=PandaColumns.IMAGE,
+            mask_column=PandaColumns.MASK,
+            metadata_columns=PandaColumns.METADATA,
+            default_csv_filename=PANDA_CSV_FILENAME,
+        )
+        # PANDA CSV does not come with paths for image and mask files
+        slide_ids = self.dataset_df.index
+        self.dataset_df[self.image_column] = "train_images/" + slide_ids + ".tiff"
+        self.dataset_df[self.mask_column] = "train_label_masks/" + slide_ids + "_mask.tiff"
         self.validate_columns()
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/models/deepmil.py` & `hi-ml-cpath-0.3.0/src/health_cpath/models/deepmil.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,194 +1,325 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 import torch
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple
-from pytorch_lightning.utilities.rank_zero import rank_zero_warn
+from typing import Callable, Dict, List, Optional, Sequence, Tuple
 from pathlib import Path
-
 from pytorch_lightning import LightningModule
-from torch import Tensor, argmax, mode, nn, optim, round, set_grad_enabled
-from torchmetrics import AUROC, F1, Accuracy, ConfusionMatrix, Precision, Recall, CohenKappa  # type: ignore
-
+from torch import Tensor, argmax, mode, nn, optim, round
+from pytorch_lightning.utilities.rank_zero import rank_zero_warn
+from torchmetrics.classification import (
+    MulticlassAUROC,
+    MulticlassAccuracy,
+    MulticlassConfusionMatrix,
+    MulticlassCohenKappa,
+    MulticlassAveragePrecision,
+    BinaryConfusionMatrix,
+    BinaryAccuracy,
+    BinaryPrecision,
+    BinaryRecall,
+    BinaryF1Score,
+    BinaryCohenKappa,
+    BinaryAUROC,
+    BinarySpecificity,
+    BinaryAveragePrecision,
+)
 from health_ml.utils import log_on_epoch
 from health_ml.deep_learning_config import OptimizerParams
 from health_cpath.models.encoders import IdentityEncoder
-from health_cpath.utils.deepmil_utils import EncoderParams, PoolingParams
-
+from health_cpath.utils.deepmil_utils import ClassifierParams, EncoderParams, PoolingParams
 from health_cpath.datasets.base_dataset import TilesDataset
-from health_cpath.utils.naming import MetricsKey, ResultsKey, SlideKey, ModelKey, TileKey
-from health_cpath.utils.output_utils import (BatchResultsType, DeepMILOutputsHandler, EpochResultsType,
-                                             validate_class_names)
-
-RESULTS_COLS = [ResultsKey.SLIDE_ID, ResultsKey.TILE_ID, ResultsKey.IMAGE_PATH, ResultsKey.PROB,
-                ResultsKey.CLASS_PROBS, ResultsKey.PRED_LABEL, ResultsKey.TRUE_LABEL, ResultsKey.BAG_ATTN]
+from health_cpath.utils.naming import DeepMILSubmodules, MetricsKey, ResultsKey, SlideKey, ModelKey, TileKey
+from health_cpath.utils.output_utils import (
+    BatchResultsType,
+    DeepMILOutputsHandler,
+    EpochResultsType,
+    validate_class_names,
+    EXTRA_PREFIX,
+)
+
+
+RESULTS_COLS = [
+    ResultsKey.SLIDE_ID,
+    ResultsKey.TILE_ID,
+    ResultsKey.IMAGE_PATH,
+    ResultsKey.PROB,
+    ResultsKey.CLASS_PROBS,
+    ResultsKey.PRED_LABEL,
+    ResultsKey.TRUE_LABEL,
+    ResultsKey.BAG_ATTN,
+]
 
 
 def _format_cuda_memory_stats() -> str:
-    return (f"GPU {torch.cuda.current_device()} memory: "
-            f"{torch.cuda.memory_allocated() / 1024 ** 3:.2f} GB allocated, "
-            f"{torch.cuda.memory_reserved() / 1024 ** 3:.2f} GB reserved")
+    return (
+        f"GPU {torch.cuda.current_device()} memory: "
+        f"{torch.cuda.memory_allocated() / 1024 ** 3:.2f} GB allocated, "
+        f"{torch.cuda.memory_reserved() / 1024 ** 3:.2f} GB reserved"
+    )
 
 
-class BaseDeepMILModule(LightningModule):
+class DeepMILModule(LightningModule):
     """Base class for deep multiple-instance learning"""
 
-    def __init__(self,
-                 label_column: str,
-                 n_classes: int,
-                 class_weights: Optional[Tensor] = None,
-                 class_names: Optional[Sequence[str]] = None,
-                 dropout_rate: Optional[float] = None,
-                 verbose: bool = False,
-                 ssl_ckpt_run_id: Optional[str] = None,
-                 outputs_folder: Optional[Path] = None,
-                 encoder_params: EncoderParams = EncoderParams(),
-                 pooling_params: PoolingParams = PoolingParams(),
-                 optimizer_params: OptimizerParams = OptimizerParams(),
-                 outputs_handler: Optional[DeepMILOutputsHandler] = None) -> None:
+    def __init__(
+        self,
+        label_column: str,
+        n_classes: int,
+        class_weights: Optional[Tensor] = None,
+        class_names: Optional[Sequence[str]] = None,
+        encoder_params: EncoderParams = EncoderParams(),
+        pooling_params: PoolingParams = PoolingParams(),
+        classifier_params: ClassifierParams = ClassifierParams(),
+        optimizer_params: OptimizerParams = OptimizerParams(),
+        outputs_folder: Optional[Path] = None,
+        outputs_handler: Optional[DeepMILOutputsHandler] = None,
+        analyse_loss: Optional[bool] = False,
+        verbose: bool = False,
+    ) -> None:
         """
         :param label_column: Label key for input batch dictionary.
         :param n_classes: Number of output classes for MIL prediction. For binary classification, n_classes should be
          set to 1.
         :param class_weights: Tensor containing class weights (default=None).
         :param class_names: The names of the classes if available (default=None).
-        :param dropout_rate: Rate of pre-classifier dropout (0-1). `None` for no dropout (default).
-        :param verbose: if True statements about memory usage are output at each step.
-        :param ssl_ckpt_run_id: Optional parameter to provide the AML run id from where to download the checkpoint
-            if using `SSLEncoder`.
-        :param outputs_folder: Path to output folder where encoder checkpoint is downloaded.
         :param encoder_params: Encoder parameters that specify all encoder specific attributes.
         :param pooling_params: Pooling layer parameters that specify all encoder specific attributes.
+        :param classifier_params: Classifier parameters that specify all classifier specific attributes.
         :param optimizer_params: Optimizer parameters that specify all specific attributes to be used for oprimization.
+        :param outputs_folder: Path to output folder where encoder checkpoint is downloaded.
         :param outputs_handler: A configured :py:class:`DeepMILOutputsHandler` object to save outputs for the best
             validation epoch and test stage. If omitted (default), no outputs will be saved to disk (aside from usual
             metrics logging).
+        :param analyse_loss: If True, the loss is analysed per sample and analysed with LossAnalysisCallback.
+        :param verbose: if True statements about memory usage are output at each step.
         """
         super().__init__()
 
         # Dataset specific attributes
         self.label_column = label_column
         self.n_classes = n_classes
         self.class_weights = class_weights
         self.class_names = validate_class_names(class_names, self.n_classes)
 
-        self.dropout_rate = dropout_rate
         self.encoder_params = encoder_params
+        self.pooling_params = pooling_params
+        self.classifier_params = classifier_params
         self.optimizer_params = optimizer_params
 
         self.save_hyperparameters()
         self.verbose = verbose
         self.outputs_handler = outputs_handler
 
         # This flag can be switched on before invoking trainer.validate() to enable saving additional time/memory
-        # consuming validation outputs
-        self.run_extra_val_epoch = False
+        # consuming validation outputs via calling self.on_run_extra_validation_epoch()
+        self._on_extra_val_epoch = False
 
         # Model components
-        self.encoder = encoder_params.get_encoder(ssl_ckpt_run_id, outputs_folder)
-        self.aggregation_fn, self.num_pooling = pooling_params.get_pooling_layer(self.encoder.num_encoding)
-        self.classifier_fn = self.get_classifier()
+        self.encoder = encoder_params.get_encoder(outputs_folder)
+        self.projector = encoder_params.get_projection_layer(self.encoder.num_encoding)
+        # If projection is enabled, the number of encoding dimensions is the projection dimension otherwise it is the
+        # number of encoding dimensions of the encoder.
+        num_encoding = encoder_params.projection_dim if encoder_params.projection_dim > 0 else self.encoder.num_encoding
+        self.aggregation_fn, self.num_pooling = pooling_params.get_pooling_layer(num_encoding)
+        self.classifier_fn = classifier_params.get_classifier(self.num_pooling, self.n_classes)
         self.activation_fn = self.get_activation()
 
-        self.loss_fn = self.get_loss()
+        # Loss function
+        self.loss_fn = self.get_loss(reduction="mean")
+        self.loss_fn_no_reduction = self.get_loss(reduction="none")
+        self.analyse_loss = analyse_loss
 
         # Metrics Objects
         self.train_metrics = self.get_metrics()
         self.val_metrics = self.get_metrics()
         self.test_metrics = self.get_metrics()
 
-    def get_classifier(self) -> Callable:
-        classifier_layer = nn.Linear(in_features=self.num_pooling,
-                                     out_features=self.n_classes)
-        if self.dropout_rate is None:
-            return classifier_layer
-        elif 0 <= self.dropout_rate < 1:
-            return nn.Sequential(nn.Dropout(self.dropout_rate), classifier_layer)
-        else:
-            raise ValueError(f"Dropout rate should be in [0, 1), got {self.dropout_rate}")
+        self.reset_encoder_to_identity_if_caching()
+
+    def reset_encoder_to_identity_if_caching(self) -> None:
+        """If caching is enabled, the encoder is replaced with an identity encoder."""
+        if self.encoder_params.is_caching:
+            # Encoding is done in the datamodule, so here we provide instead a dummy
+            # no-op IdentityEncoder to be used inside the model
+            self.encoder = IdentityEncoder(input_dim=(self.encoder.num_encoding,))
+
+    @staticmethod
+    def copy_weights(
+        current_submodule: nn.Module, pretrained_submodule: nn.Module, submodule_name: DeepMILSubmodules
+    ) -> None:
+        """Copy weights from pretrained submodule to current submodule.
+
+        :param current_submodule: Submodule to copy weights to.
+        :param pretrained_submodule: Submodule to copy weights from.
+        :param submodule_name: Name of the submodule.
+        """
+
+        def _total_params(submodule: nn.Module) -> int:
+            return sum(p.numel() for p in submodule.parameters())
+
+        pre_total_params = _total_params(pretrained_submodule)
+        cur_total_params = _total_params(current_submodule)
+
+        if pre_total_params != cur_total_params:
+            raise ValueError(
+                f"Submodule {submodule_name} has different number of parameters "
+                f"({cur_total_params} vs {pre_total_params}) from pretrained model."
+            )
+
+        for param, pretrained_param in zip(
+            current_submodule.state_dict().values(), pretrained_submodule.state_dict().values()
+        ):
+            try:
+                param.data.copy_(pretrained_param.data)
+            except Exception as e:
+                raise ValueError(f"Failed to copy weights for {submodule_name} because of the following exception: {e}")
+
+    def transfer_weights(self, pretrained_checkpoint_path: Optional[Path]) -> None:
+        """Transfer weights from pretrained checkpoint if provided."""
+
+        if pretrained_checkpoint_path:
+            pretrained_model = self.load_from_checkpoint(checkpoint_path=str(pretrained_checkpoint_path))
+
+            if self.encoder_params.pretrained_encoder:
+                self.copy_weights(self.encoder, pretrained_model.encoder, DeepMILSubmodules.ENCODER)
+
+            if self.pooling_params.pretrained_pooling:
+                self.copy_weights(self.aggregation_fn, pretrained_model.aggregation_fn, DeepMILSubmodules.POOLING)
+
+            if self.classifier_params.pretrained_classifier:
+                if pretrained_model.n_classes != self.n_classes:
+                    raise ValueError(
+                        f"Number of classes in pretrained model {pretrained_model.n_classes} "
+                        f"does not match number of classes in current model {self.n_classes}."
+                    )
+                self.copy_weights(self.classifier_fn, pretrained_model.classifier_fn, DeepMILSubmodules.CLASSIFIER)
 
-    def get_loss(self) -> Callable:
+    def get_loss(self, reduction: str = "mean") -> Callable:
         if self.n_classes > 1:
             if self.class_weights is None:
-                return nn.CrossEntropyLoss()
+                return nn.CrossEntropyLoss(reduction=reduction)
             else:
                 class_weights = self.class_weights.float()
-                return nn.CrossEntropyLoss(weight=class_weights)
+                return nn.CrossEntropyLoss(weight=class_weights, reduction=reduction)
         else:
             pos_weight = None
             if self.class_weights is not None:
                 pos_weight = Tensor([self.class_weights[1] / (self.class_weights[0] + 1e-5)])
-            return nn.BCEWithLogitsLoss(pos_weight=pos_weight)
+            return nn.BCEWithLogitsLoss(pos_weight=pos_weight, reduction=reduction)
 
     def get_activation(self) -> Callable:
         if self.n_classes > 1:
             return nn.Softmax(dim=-1)
         else:
             return nn.Sigmoid()
 
     @staticmethod
     def get_bag_label(labels: Tensor) -> Tensor:
-        raise NotImplementedError
+        """Get bag label as the majority class of the bag's samples. For slides pipeline, we already have a single
+        label per bag so we just return that label. For tiles pipeline, we need to get the majority class as labels
+        are duplicated for each tile in the bag."""
+        if len(labels.shape) == 0:
+            return labels
+        bag_label = mode(labels).values
+        return bag_label.view(1)
 
     def get_metrics(self) -> nn.ModuleDict:
         if self.n_classes > 1:
-            return nn.ModuleDict({MetricsKey.ACC: Accuracy(num_classes=self.n_classes),
-                                  MetricsKey.ACC_MACRO: Accuracy(num_classes=self.n_classes, average='macro'),
-                                  MetricsKey.ACC_WEIGHTED: Accuracy(num_classes=self.n_classes, average='weighted'),
-                                  MetricsKey.AUROC: AUROC(num_classes=self.n_classes),
-                                  # Quadratic Weighted Kappa (QWK) used in PANDA challenge
-                                  # is calculated using Cohen's Kappa with quadratic weights
-                                  # https://www.kaggle.com/code/reighns/understanding-the-quadratic-weighted-kappa/
-                                  MetricsKey.COHENKAPPA: CohenKappa(num_classes=self.n_classes, weights='quadratic'),
-                                  MetricsKey.CONF_MATRIX: ConfusionMatrix(num_classes=self.n_classes)})
+            return nn.ModuleDict(
+                {
+                    MetricsKey.ACC: MulticlassAccuracy(num_classes=self.n_classes, average='micro'),
+                    MetricsKey.AUROC: MulticlassAUROC(num_classes=self.n_classes),
+                    MetricsKey.AVERAGE_PRECISION: MulticlassAveragePrecision(num_classes=self.n_classes),
+                    # Quadratic Weighted Kappa (QWK) used in PANDA challenge
+                    # is calculated using Cohen's Kappa with quadratic weights
+                    # https://www.kaggle.com/code/reighns/understanding-the-quadratic-weighted-kappa/
+                    MetricsKey.COHENKAPPA: MulticlassCohenKappa(num_classes=self.n_classes, weights='quadratic'),
+                    MetricsKey.CONF_MATRIX: MulticlassConfusionMatrix(num_classes=self.n_classes),
+                    # Metrics below are computed for multi-class case only
+                    MetricsKey.ACC_MACRO: MulticlassAccuracy(num_classes=self.n_classes, average='macro'),
+                    MetricsKey.ACC_WEIGHTED: MulticlassAccuracy(num_classes=self.n_classes, average='weighted'),
+                }
+            )
         else:
-            threshold = 0.5
-            return nn.ModuleDict({MetricsKey.ACC: Accuracy(threshold=threshold),
-                                  MetricsKey.AUROC: AUROC(num_classes=self.n_classes),
-                                  MetricsKey.PRECISION: Precision(threshold=threshold),
-                                  MetricsKey.RECALL: Recall(threshold=threshold),
-                                  MetricsKey.F1: F1(threshold=threshold),
-                                  MetricsKey.CONF_MATRIX: ConfusionMatrix(num_classes=2, threshold=threshold)})
+            return nn.ModuleDict(
+                {
+                    MetricsKey.ACC: BinaryAccuracy(),
+                    MetricsKey.AUROC: BinaryAUROC(),
+                    # Average precision is a measure of area under the PR curve
+                    MetricsKey.AVERAGE_PRECISION: BinaryAveragePrecision(),
+                    MetricsKey.COHENKAPPA: BinaryCohenKappa(weights='quadratic'),
+                    MetricsKey.CONF_MATRIX: BinaryConfusionMatrix(),
+                    # Metrics below are computed for binary case only
+                    MetricsKey.F1: BinaryF1Score(),
+                    MetricsKey.PRECISION: BinaryPrecision(),
+                    MetricsKey.RECALL: BinaryRecall(),
+                    MetricsKey.SPECIFICITY: BinarySpecificity(),
+                }
+            )
+
+    def get_extra_prefix(self) -> str:
+        """Get extra prefix for the metrics name to avoir overriding best validation metrics."""
+        return EXTRA_PREFIX if self._on_extra_val_epoch else ""
 
-    def log_metrics(self, stage: str) -> None:
-        valid_stages = [stage for stage in ModelKey]
+    def log_metrics(self, stage: str, prefix: str = '') -> None:
+        valid_stages = set([stage for stage in ModelKey])
         if stage not in valid_stages:
             raise Exception(f"Invalid stage. Chose one of {valid_stages}")
         for metric_name, metric_object in self.get_metrics_dict(stage).items():
             if metric_name == MetricsKey.CONF_MATRIX:
                 metric_value = metric_object.compute()
                 metric_value_n = metric_value / metric_value.sum(axis=1, keepdims=True)
                 for i in range(metric_value_n.shape[0]):
-                    log_on_epoch(self, f'{stage}/{self.class_names[i]}', metric_value_n[i, i])
+                    log_on_epoch(self, f'{prefix}{stage}/{self.class_names[i]}', metric_value_n[i, i])
             else:
-                log_on_epoch(self, f'{stage}/{metric_name}', metric_object)
+                log_on_epoch(self, f'{prefix}{stage}/{metric_name}', metric_object)
 
-    def forward(self, instances: Tensor) -> Tuple[Tensor, Tensor]:  # type: ignore
-        should_enable_encoder_grad = torch.is_grad_enabled() and self.encoder_params.is_finetune
-        with set_grad_enabled(should_enable_encoder_grad):
-            if self.encoder_params.encoding_chunk_size > 0:
-                embeddings = []
-                chunks = torch.split(instances, self.encoder_params.encoding_chunk_size)
-                for chunk in chunks:
-                    chunk_embeddings = self.encoder(chunk)
-                    embeddings.append(chunk_embeddings)
-                instance_features = torch.cat(embeddings)
-            else:
-                instance_features = self.encoder(instances)                # N X L x 1 x 1
+    def get_instance_features(self, instances: Tensor) -> Tensor:
+        if not self.encoder_params.tune_encoder:
+            self.encoder.eval()
+        if self.encoder_params.encoding_chunk_size > 0:
+            embeddings = []
+            chunks = torch.split(instances, self.encoder_params.encoding_chunk_size)
+            for chunk in chunks:
+                chunk_embeddings = self.encoder(chunk)
+                embeddings.append(chunk_embeddings)
+            instance_features = torch.cat(embeddings)
+        else:
+            instance_features = self.encoder(instances)  # N X L x 1 x 1
+        return instance_features
+
+    def get_attentions_and_bag_features(self, instance_features: Tensor) -> Tuple[Tensor, Tensor]:
+        if not self.pooling_params.tune_pooling:
+            self.aggregation_fn.eval()
         attentions, bag_features = self.aggregation_fn(instance_features)  # K x N | K x L
         bag_features = bag_features.view(1, -1)
+        return attentions, bag_features
+
+    def get_bag_logit(self, bag_features: Tensor) -> Tensor:
+        if not self.classifier_params.tune_classifier:
+            self.classifier_fn.eval()
         bag_logit = self.classifier_fn(bag_features)
+        return bag_logit
+
+    def forward(self, instances: Tensor) -> Tuple[Tensor, Tensor]:  # type: ignore
+        instance_features = self.get_instance_features(instances)
+        projected_features = self.projector(instance_features)
+        attentions, bag_features = self.get_attentions_and_bag_features(projected_features)
+        bag_logit = self.get_bag_logit(bag_features)
         return bag_logit, attentions
 
     def configure_optimizers(self) -> optim.Optimizer:
-        return optim.Adam(self.parameters(), lr=self.optimizer_params.l_rate,
-                          weight_decay=self.optimizer_params.weight_decay,
-                          betas=self.optimizer_params.adam_betas)
+        return optim.Adam(
+            filter(lambda p: p.requires_grad, self.parameters()),
+            lr=self.optimizer_params.l_rate,
+            weight_decay=self.optimizer_params.weight_decay,
+            betas=self.optimizer_params.adam_betas,
+        )
 
     def get_metrics_dict(self, stage: str) -> nn.ModuleDict:
         return getattr(self, f'{stage}_metrics')
 
     def compute_bag_labels_logits_and_attn_maps(self, batch: Dict) -> Tuple[Tensor, Tensor, List]:
         # The batch dict contains lists of tensors of different sizes, for all bags in the batch.
         # This means we can't stack them along a new axis without padding to the same length.
@@ -204,169 +335,145 @@
             logit, attn = self(images)
             bag_logits_list.append(logit.view(-1))
             bag_attn_list.append(attn)
         bag_logits = torch.stack(bag_logits_list)
         bag_labels = torch.stack(bag_labels_list).view(-1)
         return bag_logits, bag_labels, bag_attn_list
 
-    def update_results_with_data_specific_info(self, batch: Dict, results: Dict) -> None:
-        """Update training results with data specific info. This can be either tiles or slides related metadata."""
-        raise NotImplementedError
-
-    def _shared_step(self, batch: Dict, batch_idx: int, stage: str) -> BatchResultsType:
+    def update_results_with_metadata(self, batch: Dict, results: Dict) -> None:
+        """Update results with metadata. This can be either tiles or slides metadata including tiles coordinates."""
+        results.update({ResultsKey.SLIDE_ID: batch[SlideKey.SLIDE_ID], ResultsKey.TILE_ID: batch[TileKey.TILE_ID]})
+        # Add tiles coordinates if available
+        coordinates_keys = [TileKey.TILE_TOP, TileKey.TILE_BOTTOM, TileKey.TILE_RIGHT, TileKey.TILE_LEFT]
+        if all([key in batch for key in coordinates_keys]):
+            for key in coordinates_keys:
+                results[key] = batch[key]
+        elif TilesDataset.TILE_X_COLUMN in batch and TilesDataset.TILE_X_COLUMN in batch:
+            results[ResultsKey.TILE_LEFT] = batch[TilesDataset.TILE_X_COLUMN]
+            results[ResultsKey.TILE_TOP] = batch[TilesDataset.TILE_Y_COLUMN]
+        else:
+            rank_zero_warn(
+                message="Coordinates not found in batch. If this is not expected check your input tiles dataset."
+            )
 
-        bag_logits, bag_labels, bag_attn_list = self.compute_bag_labels_logits_and_attn_maps(batch)
+    def update_slides_selection(self, stage: str, batch: Dict, results: Dict) -> None:
+        if (
+            (stage == ModelKey.TEST or (stage == ModelKey.VAL and self._on_extra_val_epoch))
+            and self.outputs_handler
+            and self.outputs_handler.tiles_selector
+        ):
+            self.outputs_handler.tiles_selector.update_slides_selection(batch, results)
 
+    def _compute_loss(self, loss_fn: Callable, bag_logits: Tensor, bag_labels: Tensor) -> Tensor:
         if self.n_classes > 1:
-            loss = self.loss_fn(bag_logits, bag_labels.long())
+            return loss_fn(bag_logits, bag_labels.long())
         else:
-            loss = self.loss_fn(bag_logits.squeeze(1), bag_labels.float())
+            return loss_fn(bag_logits.squeeze(1), bag_labels.float())
+
+    def _shared_step(self, batch: Dict, batch_idx: int, stage: str) -> BatchResultsType:
+        bag_logits, bag_labels, bag_attn_list = self.compute_bag_labels_logits_and_attn_maps(batch)
+
+        loss = self._compute_loss(self.loss_fn, bag_logits, bag_labels)
 
         predicted_probs = self.activation_fn(bag_logits)
         if self.n_classes > 1:
             predicted_labels = argmax(predicted_probs, dim=1)
             probs_perclass = predicted_probs
         else:
-            predicted_labels = round(predicted_probs)
-            probs_perclass = Tensor([[1.0 - predicted_probs[i][0].item(), predicted_probs[i][0].item()]
-                                     for i in range(len(predicted_probs))])
+            predicted_labels = round(predicted_probs).int()
+            probs_perclass = Tensor(
+                [
+                    [1.0 - predicted_probs[i][0].item(), predicted_probs[i][0].item()]
+                    for i in range(len(predicted_probs))
+                ]
+            )
 
         loss = loss.view(-1, 1)
         predicted_labels = predicted_labels.view(-1, 1)
         batch_size = predicted_labels.shape[0]
 
         if self.n_classes == 1:
             predicted_probs = predicted_probs.squeeze(dim=1)
 
+        results = dict()
+
+        if self.analyse_loss and stage in [ModelKey.TRAIN, ModelKey.VAL]:
+            loss_per_sample = self._compute_loss(self.loss_fn_no_reduction, bag_logits, bag_labels)
+            results[ResultsKey.LOSS_PER_SAMPLE] = loss_per_sample.detach().cpu().numpy()
+
         bag_labels = bag_labels.view(-1, 1)
 
-        results = dict()
         for metric_object in self.get_metrics_dict(stage).values():
-            metric_object.update(predicted_probs, bag_labels.view(batch_size,).int())
-        results.update({ResultsKey.LOSS: loss,
-                        ResultsKey.PROB: predicted_probs,
-                        ResultsKey.CLASS_PROBS: probs_perclass,
-                        ResultsKey.PRED_LABEL: predicted_labels,
-                        ResultsKey.TRUE_LABEL: bag_labels,
-                        ResultsKey.BAG_ATTN: bag_attn_list
-                        })
-        self.update_results_with_data_specific_info(batch=batch, results=results)
-        if (
-            (stage == ModelKey.TEST or (stage == ModelKey.VAL and self.run_extra_val_epoch))
-            and self.outputs_handler
-            and self.outputs_handler.tiles_selector
-        ):
-            self.outputs_handler.tiles_selector.update_slides_selection(batch, results)
+            metric_object.update(
+                predicted_probs,
+                bag_labels.view(
+                    batch_size,
+                ).int(),
+            )
+        results.update(
+            {
+                ResultsKey.LOSS: loss,
+                ResultsKey.PROB: predicted_probs,
+                ResultsKey.CLASS_PROBS: probs_perclass,
+                ResultsKey.PRED_LABEL: predicted_labels,
+                ResultsKey.TRUE_LABEL: bag_labels.int(),
+                ResultsKey.BAG_ATTN: bag_attn_list,
+            }
+        )
+        self.update_results_with_metadata(batch=batch, results=results)
+        self.update_slides_selection(stage=stage, batch=batch, results=results)
         return results
 
-    def training_step(self, batch: Dict, batch_idx: int) -> Tensor:  # type: ignore
+    def training_step(self, batch: Dict, batch_idx: int) -> BatchResultsType:  # type: ignore
         train_result = self._shared_step(batch, batch_idx, ModelKey.TRAIN)
-        self.log('train/loss', train_result[ResultsKey.LOSS], on_epoch=True, on_step=True, logger=True,
-                 sync_dist=True)
+        self.log('train/loss', train_result[ResultsKey.LOSS], on_epoch=True, on_step=True, logger=True, sync_dist=True)
         if self.verbose:
             print(f"After loading images batch {batch_idx} -", _format_cuda_memory_stats())
-        return train_result[ResultsKey.LOSS]
+        results = {ResultsKey.LOSS: train_result[ResultsKey.LOSS]}
+        if self.analyse_loss:
+            results.update(
+                {
+                    ResultsKey.LOSS_PER_SAMPLE: train_result[ResultsKey.LOSS_PER_SAMPLE],
+                    ResultsKey.CLASS_PROBS: train_result[ResultsKey.CLASS_PROBS],
+                    ResultsKey.TILE_ID: train_result[ResultsKey.TILE_ID],
+                }
+            )
+        return results
 
     def validation_step(self, batch: Dict, batch_idx: int) -> BatchResultsType:  # type: ignore
         val_result = self._shared_step(batch, batch_idx, ModelKey.VAL)
-        self.log('val/loss', val_result[ResultsKey.LOSS], on_epoch=True, on_step=True, logger=True,
-                 sync_dist=True)
+        name = f'{self.get_extra_prefix()}val/loss'
+        self.log(name, val_result[ResultsKey.LOSS], on_epoch=True, on_step=True, logger=True, sync_dist=True)
         return val_result
 
     def test_step(self, batch: Dict, batch_idx: int) -> BatchResultsType:  # type: ignore
         test_result = self._shared_step(batch, batch_idx, ModelKey.TEST)
-        self.log('test/loss', test_result[ResultsKey.LOSS], on_epoch=True, on_step=True, logger=True,
-                 sync_dist=True)
+        self.log('test/loss', test_result[ResultsKey.LOSS], on_epoch=True, on_step=True, logger=True, sync_dist=True)
         return test_result
 
     def training_epoch_end(self, outputs: EpochResultsType) -> None:  # type: ignore
         self.log_metrics(ModelKey.TRAIN)
 
     def validation_epoch_end(self, epoch_results: EpochResultsType) -> None:  # type: ignore
-        self.log_metrics(ModelKey.VAL)
+        self.log_metrics(stage=ModelKey.VAL, prefix=self.get_extra_prefix())
         if self.outputs_handler:
-            if self.run_extra_val_epoch:
-                self.outputs_handler.val_plots_handler.plot_options = (
-                    self.outputs_handler.test_plots_handler.plot_options
-                )
             self.outputs_handler.save_validation_outputs(
                 epoch_results=epoch_results,
                 metrics_dict=self.get_metrics_dict(ModelKey.VAL),  # type: ignore
                 epoch=self.current_epoch,
                 is_global_rank_zero=self.global_rank == 0,
-                run_extra_val_epoch=self.run_extra_val_epoch
+                on_extra_val=self._on_extra_val_epoch,
             )
 
-            # Reset the top and bottom slides heaps
-            if self.outputs_handler.tiles_selector is not None:
-                self.outputs_handler.tiles_selector._clear_cached_slides_heaps()
-
     def test_epoch_end(self, epoch_results: EpochResultsType) -> None:  # type: ignore
         self.log_metrics(ModelKey.TEST)
         if self.outputs_handler:
             self.outputs_handler.save_test_outputs(
-                epoch_results=epoch_results,
-                is_global_rank_zero=self.global_rank == 0
+                epoch_results=epoch_results, is_global_rank_zero=self.global_rank == 0
             )
 
-
-class TilesDeepMILModule(BaseDeepMILModule):
-    """Base class for Tiles based deep multiple-instance learning."""
-
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs)
-        if self.encoder_params.is_caching:
-            # Encoding is done in the datamodule, so here we provide instead a dummy
-            # no-op IdentityEncoder to be used inside the model
-            self.encoder = IdentityEncoder(input_dim=(self.encoder.num_encoding,))
-
-    @staticmethod
-    def get_bag_label(labels: Tensor) -> Tensor:
-        # Get bag (batch) labels as majority vote
-        bag_label = mode(labels).values
-        return bag_label.view(1)
-
-    def update_results_with_data_specific_info(self, batch: Dict, results: Dict) -> None:
-        results.update({ResultsKey.SLIDE_ID: batch[TilesDataset.SLIDE_ID_COLUMN],
-                        ResultsKey.TILE_ID: batch[TilesDataset.TILE_ID_COLUMN],
-                        ResultsKey.IMAGE_PATH: batch[TilesDataset.PATH_COLUMN]})
-
-        if all(key in batch.keys() for key in [TileKey.TILE_TOP, TileKey.TILE_LEFT,
-                                               TileKey.TILE_RIGHT, TileKey.TILE_BOTTOM]):
-            results.update({ResultsKey.TILE_TOP: batch[TileKey.TILE_TOP],
-                            ResultsKey.TILE_LEFT: batch[TileKey.TILE_LEFT],
-                            ResultsKey.TILE_RIGHT: batch[TileKey.TILE_RIGHT],
-                            ResultsKey.TILE_BOTTOM: batch[TileKey.TILE_BOTTOM]})
-        # the condition below ensures compatibility with older tile datasets (without LEFT, TOP, RIGHT, BOTTOM)
-        elif (TilesDataset.TILE_X_COLUMN in batch.keys()) and (TilesDataset.TILE_Y_COLUMN in batch.keys()):
-            results.update({ResultsKey.TILE_LEFT: batch[TilesDataset.TILE_X_COLUMN],
-                           ResultsKey.TILE_TOP: batch[TilesDataset.TILE_Y_COLUMN]})
-        else:
-            rank_zero_warn(message="Coordinates not found in batch. If this is not expected check your"
-                           "input tiles dataset.")
-
-
-class SlidesDeepMILModule(BaseDeepMILModule):
-    """Base class for slides based deep multiple-instance learning."""
-
-    @staticmethod
-    def get_bag_label(labels: Tensor) -> Tensor:
-        # SlidesDataModule attributes a single label to a bag of tiles already no need to do majority voting
-        return labels
-
-    def update_results_with_data_specific_info(self, batch: Dict, results: Dict) -> None:
-        # WARNING: This is a dummy input until we figure out tiles coordinates retrieval in the next iteration.
-        bag_sizes = [tiles.shape[0] for tiles in batch[SlideKey.IMAGE]]
-        results.update(
-            {
-                ResultsKey.SLIDE_ID: [
-                    [slide_id] * bag_sizes[i] for i, slide_id in enumerate(batch[SlideKey.SLIDE_ID])
-                ],
-                ResultsKey.TILE_ID: [
-                    [f"{slide_id}_{tile_id}" for tile_id in range(bag_sizes[i])]
-                    for i, slide_id in enumerate(batch[SlideKey.SLIDE_ID])
-                ],
-                ResultsKey.IMAGE_PATH: [
-                    [img_path] * bag_sizes[i] for i, img_path in enumerate(batch[SlideKey.IMAGE_PATH])
-                ],
-            }
-        )
+    def on_run_extra_validation_epoch(self) -> None:
+        """Hook to be called at the beginning of an extra validation epoch to set validation plots options to the same
+        as the test plots options."""
+        self._on_extra_val_epoch = True
+        if self.outputs_handler:
+            self.outputs_handler.val_plots_handler.plot_options = self.outputs_handler.test_plots_handler.plot_options
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/preprocessing/create_panda_tiles_dataset.py` & `hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/create_panda_tiles_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 import shutil
 from pathlib import Path
 from argparse import ArgumentParser
 from typing import Tuple, Union, List
 
 import numpy as np
 from monai.data import Dataset
-from monai.data.image_reader import WSIReader
 from tqdm import tqdm
 from health_ml.utils.box_utils import Box
 
 from health_cpath.preprocessing import tiling
 from health_cpath.utils.naming import SlideKey, TileKey
-from health_cpath.datasets.panda_dataset import PandaDataset, LoadPandaROId
+from health_cpath.datasets.panda_dataset import PandaDataset
+from health_cpath.preprocessing.loading import LoadMaskROId, WSIBackend
 from health_cpath.preprocessing.create_tiles_dataset import get_tile_id, save_image, merge_dataset_csv_files
 
 CSV_COLUMNS = (
     'slide_id',
     'tile_id',
     'image',
     'mask',
@@ -38,30 +38,31 @@
     'slide_isup_grade',
     'slide_gleason_score',
     'num_discarded',
 )
 TMP_SUFFIX = "_tmp"
 
 
-def select_tile(mask_tile: np.ndarray, occupancy_threshold: float) \
-        -> Union[Tuple[bool, float], Tuple[np.ndarray, np.ndarray]]:
-    if occupancy_threshold < 0. or occupancy_threshold > 1.:
+def select_tile(
+    mask_tile: np.ndarray, occupancy_threshold: float
+) -> Union[Tuple[bool, float], Tuple[np.ndarray, np.ndarray]]:
+    if occupancy_threshold < 0.0 or occupancy_threshold > 1.0:
         raise ValueError("Tile occupancy threshold must be between 0 and 1")
     # mask_tile has shape (N, C, H, W)
     foreground_mask = mask_tile > 0
     occupancy = foreground_mask.mean(axis=(-2, -1))
     selected = occupancy >= occupancy_threshold  # if the threshold is 0, all tiles should be selected
     # selected has shape (N, 1)
     return selected[:, 0], occupancy[:, 0]
 
 
-def generate_tiles(sample: dict, tile_size: int, occupancy_threshold: float) \
-        -> Tuple[np.ndarray, np.ndarray, List[Box], np.ndarray, int]:
-    image_tiles, tile_locations = tiling.tile_array_2d(sample['image'], tile_size=tile_size,
-                                                       constant_values=255)
+def generate_tiles(
+    sample: dict, tile_size: int, occupancy_threshold: float
+) -> Tuple[np.ndarray, np.ndarray, List[Box], np.ndarray, int]:
+    image_tiles, tile_locations = tiling.tile_array_2d(sample['image'], tile_size=tile_size, constant_values=255)
     assert tile_locations.ndim == 2
     mask_tiles, _ = tiling.tile_array_2d(sample['mask'], tile_size=tile_size, constant_values=0)
 
     selected: np.ndarray
     occupancies: np.ndarray
     selected, occupancies = select_tile(mask_tiles, occupancy_threshold)  # type: ignore
     num_selected = selected.sum()
@@ -83,16 +84,15 @@
     tile_boxes = [Box(x, y, tile_size_scaled, tile_size_scaled) for x, y in abs_tile_locations]
 
     return image_tiles, mask_tiles, tile_boxes, occupancies, num_discarded
 
 
 # TODO refactor this to separate metadata identification from saving. We might want the metadata
 # even if the saving fails
-def save_tile(sample: dict, image_tile: np.ndarray, mask_tile: np.ndarray,
-              tile_box: Box, output_dir: Path) -> dict:
+def save_tile(sample: dict, image_tile: np.ndarray, mask_tile: np.ndarray, tile_box: Box, output_dir: Path) -> dict:
     slide_id = sample[SlideKey.SLIDE_ID]
     tile_id = get_tile_id(slide_id, tile_box)
     image_tile_filename = f"train_images/{tile_id}.png"
     mask_tile_filename = f"train_label_masks/{tile_id}_mask.png"
 
     save_image(image_tile, output_dir / image_tile_filename)
     save_image(mask_tile, output_dir / mask_tile_filename)
@@ -110,16 +110,24 @@
         'data_provider': slide_metadata['data_provider'],
         'slide_isup_grade': slide_metadata['isup_grade'],
         'slide_gleason_score': slide_metadata['gleason_score'],
     }
     return tile_metadata
 
 
-def process_slide(sample: dict, level: int, margin: int, tile_size: int, occupancy_threshold: int,
-                  output_dir: Path, tile_progress: bool = False, filter_slide: str = '') -> None:
+def process_slide(
+    sample: dict,
+    level: int,
+    margin: int,
+    tile_size: int,
+    occupancy_threshold: int,
+    output_dir: Path,
+    tile_progress: bool = False,
+    filter_slide: str = '',
+) -> None:
     slide_id = sample[SlideKey.SLIDE_ID]
     if filter_slide not in slide_id:
         return
     slide_dir: Path = output_dir / (slide_id + "/")
     print(f">>> Slide dir {slide_dir}")
     if slide_dir.exists():  # already processed slide - skip
         print(f">>> Skipping {slide_dir} - already processed")
@@ -134,32 +142,32 @@
         slide_dir.mkdir(parents=True)
 
         dataset_csv_path = slide_dir / "dataset.csv"
         dataset_csv_file = dataset_csv_path.open('w')
         dataset_csv_file.write(','.join(CSV_COLUMNS) + '\n')  # write CSV header
 
         print(f"Loading slide {slide_id} ...")
-        reader = WSIReader(backend="cucim")
-        loader = LoadPandaROId(reader, level=level, margin=margin)
+        loader = LoadMaskROId(backend=WSIBackend.CUCIM, level=level, margin=margin)
         try:
             sample = loader(sample)  # load 'image' and 'mask' from disk
             failed = False
         except RuntimeError as e:  # happens when masks are empty
             print(f'Error loading slide {slide_id}, maybe due to an empty mask:\n{e}')
             failed = True
 
         if failed:
             print(f'Error loading slide {slide_id}')
             dataset_csv_file.close()
             shutil.rmtree(slide_dir)
             return
 
         print(f"Tiling slide {slide_id} ...")
-        image_tiles, mask_tiles, tile_boxes, occupancies, num_discarded = \
-            generate_tiles(sample, tile_size, occupancy_threshold)
+        image_tiles, mask_tiles, tile_boxes, occupancies, num_discarded = generate_tiles(
+            sample, tile_size, occupancy_threshold
+        )
         n_tiles = image_tiles.shape[0]
 
         for i in tqdm(range(n_tiles), f"Tiles ({slide_id[:6]}…)", unit="img", disable=not tile_progress):
             tile_metadata = save_tile(
                 sample,
                 image_tiles[i],
                 mask_tiles[i],
@@ -173,33 +181,47 @@
             tile_metadata[TileKey.NUM_DISCARDED] = num_discarded
             dataset_row = ','.join(str(tile_metadata[column]) for column in CSV_COLUMNS)
             dataset_csv_file.write(dataset_row + '\n')
 
         dataset_csv_file.close()
 
 
-def main(panda_dir: Union[str, Path], root_output_dir: str, level: int, tile_size: int,
-         margin: int, occupancy_threshold: float, parallel: bool = False, overwrite: bool = False,
-         filter_slide: str = '') -> None:
-
+def main(
+    panda_dir: Union[str, Path],
+    root_output_dir: str,
+    level: int,
+    tile_size: int,
+    margin: int,
+    occupancy_threshold: float,
+    parallel: bool = False,
+    overwrite: bool = False,
+    filter_slide: str = '',
+) -> None:
     # Ignoring some types here because mypy is getting confused with the MONAI Dataset class
     # to select a subsample use keyword n_slides
     dataset = Dataset(PandaDataset(panda_dir))  # type: ignore
     output_dir = Path(root_output_dir)
 
     if overwrite and output_dir.exists():
         shutil.rmtree(output_dir)
     output_dir.mkdir(parents=True, exist_ok=not overwrite)
 
     print(f"Command: \"{' '.join(sys.argv)}\"")
     print(f"Creating dataset of level-{level} {tile_size}x{tile_size} PANDA tiles at: {output_dir}")
 
-    func = functools.partial(process_slide, level=level, margin=margin, tile_size=tile_size,
-                             occupancy_threshold=occupancy_threshold, output_dir=output_dir,
-                             tile_progress=not parallel, filter_slide=filter_slide)
+    func = functools.partial(
+        process_slide,
+        level=level,
+        margin=margin,
+        tile_size=tile_size,
+        occupancy_threshold=occupancy_threshold,
+        output_dir=output_dir,
+        tile_progress=not parallel,
+        filter_slide=filter_slide,
+    )
 
     if parallel:
         import multiprocessing
 
         pool = multiprocessing.Pool()
         map_func = pool.imap_unordered  # type: ignore
     else:
@@ -218,19 +240,15 @@
     parser = ArgumentParser()
     parser.add_argument(
         "--panda-dir",
         type=str,
         default="/tmp/datasets/PANDA",
         help="Folder with the PANDA dataset. For example, '/tmp/datasets/PANDA'",
     )
-    parser.add_argument(
-        "--output-dir",
-        type=str,
-        default="/datasetdrive/PANDA_20X_level_0_224"
-    )
+    parser.add_argument("--output-dir", type=str, default="/datasetdrive/PANDA_20X_level_0_224")
     parser.add_argument(
         "--level",
         type=int,
         default=0,
     )
     parser.add_argument(
         "--tile-size",
@@ -258,15 +276,15 @@
         action="store_true",
         default=True,
     )
     parser.add_argument(
         "--filter-slide",
         type=str,
         default="",  # filtering for "b896" gives 4 slides, good for debugging
-        help="Process only slides whose ID contain this substring. Useful for debugging"
+        help="Process only slides whose ID contain this substring. Useful for debugging",
     )
     args = parser.parse_args()
 
     main(
         panda_dir=args.panda_dir,
         root_output_dir=args.output_dir,
         level=args.level,
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/preprocessing/create_tiles_dataset.py` & `hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/create_tiles_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,34 +9,32 @@
 import warnings
 from pathlib import Path
 from typing import Any, Dict, Iterable, Optional, Tuple, Union
 
 import numpy as np
 import PIL
 from monai.data import Dataset
-from monai.data.image_reader import WSIReader
 from tqdm import tqdm
 from health_ml.utils.box_utils import Box
 
 from health_cpath.datasets.base_dataset import SlidesDataset
 from health_cpath.preprocessing import tiling
-from health_cpath.preprocessing.loading import LoadROId, segment_foreground
+from health_cpath.preprocessing.loading import LoadROId, WSIBackend, segment_foreground
 from health_cpath.utils.naming import SlideKey, TileKey
 
 
-def select_tiles(foreground_mask: np.ndarray, occupancy_threshold: float) \
-        -> Tuple[np.ndarray, np.ndarray]:
+def select_tiles(foreground_mask: np.ndarray, occupancy_threshold: float) -> Tuple[np.ndarray, np.ndarray]:
     """Exclude tiles that are mostly background based on estimated occupancy.
 
     :param foreground_mask: Boolean array of shape (*, H, W).
     :param occupancy_threshold: Tiles with lower occupancy (between 0 and 1) will be discarded.
     :return: A tuple containing which tiles were selected and the estimated occupancies. These will
     be boolean and float arrays of shape (*,), or scalars if `foreground_mask` is a single tile.
     """
-    if occupancy_threshold < 0. or occupancy_threshold > 1.:
+    if occupancy_threshold < 0.0 or occupancy_threshold > 1.0:
         raise ValueError("Tile occupancy threshold must be between 0 and 1")
     occupancy = foreground_mask.mean(axis=(-2, -1))
     return (occupancy > occupancy_threshold).squeeze(), occupancy.squeeze()  # type: ignore
 
 
 def get_tile_descriptor(tile_box: Box) -> str:
     """Format the box tile coordinates into a tile descriptor."""
@@ -55,42 +53,41 @@
     path.parent.mkdir(parents=True, exist_ok=True)
     array_hwc = np.moveaxis(array_chw, 0, -1).astype(np.uint8).squeeze()
     pil_image = PIL.Image.fromarray(array_hwc)
     pil_image.convert('RGB').save(path)
     return pil_image
 
 
-def generate_tiles(slide_image: np.ndarray, tile_size: int, foreground_threshold: float,
-                   occupancy_threshold: float) -> Tuple[np.ndarray, np.ndarray, np.ndarray, int]:
+def generate_tiles(
+    slide_image: np.ndarray, tile_size: int, foreground_threshold: float, occupancy_threshold: float
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray, int]:
     """Split the foreground of an input slide image into tiles.
 
     :param slide_image: The RGB image array in (C, H, W) format.
     :param tile_size: Lateral dimensions of each tile, in pixels.
     :param foreground_threshold: Luminance threshold (0 to 255) to determine tile occupancy.
     :param occupancy_threshold: Threshold (between 0 and 1) to determine empty tiles to discard.
     :return: A tuple containing the image tiles (N, C, H, W), tile coordinates (N, 2), occupancies
     (N,), and total number of discarded empty tiles.
     """
-    image_tiles, tile_locations = tiling.tile_array_2d(slide_image, tile_size=tile_size,
-                                                       constant_values=255)
+    image_tiles, tile_locations = tiling.tile_array_2d(slide_image, tile_size=tile_size, constant_values=255)
     foreground_mask, _ = segment_foreground(image_tiles, foreground_threshold)
 
     selected, occupancies = select_tiles(foreground_mask, occupancy_threshold)
     n_discarded = (~selected).sum()
     print(f"Percentage tiles discarded: {n_discarded / len(selected) * 100:.2f}")
 
     image_tiles = image_tiles[selected]
     tile_locations = tile_locations[selected]
     occupancies = occupancies[selected]
 
     return image_tiles, tile_locations, occupancies, n_discarded
 
 
-def get_tile_info(sample: Dict[SlideKey, Any], occupancy: float, tile_box: Box,
-                  rel_slide_dir: Path) -> dict:
+def get_tile_info(sample: Dict[SlideKey, Any], occupancy: float, tile_box: Box, rel_slide_dir: Path) -> dict:
     """Map slide information and tiling outputs into tile-specific information dictionary.
 
     :param sample: Slide dictionary.
     :param occupancy: Estimated tile foreground occuppancy.
     :param tile_box: Tile box coordinates.
     :param rel_slide_dir: Directory where tiles are saved, relative to dataset root.
     :return: Tile information dictionary.
@@ -105,22 +102,20 @@
         TileKey.IMAGE: rel_image_path,
         TileKey.LABEL: sample[SlideKey.LABEL],
         TileKey.TILE_LEFT.value: tile_box.x,
         TileKey.TILE_TOP.value: tile_box.y,
         TileKey.TILE_RIGHT.value: tile_box.x + tile_box.w,
         TileKey.TILE_BOTTOM.value: tile_box.y + tile_box.h,
         TileKey.OCCUPANCY: occupancy,
-        TileKey.SLIDE_METADATA: {key: value
-                                 for key, value in sample[SlideKey.METADATA].items()}
+        TileKey.SLIDE_METADATA: {key: value for key, value in sample[SlideKey.METADATA].items()},
     }
     return tile_info
 
 
-def format_csv_row(tile_info: Dict[TileKey, Any], keys_to_save: Iterable[TileKey],
-                   metadata_keys: Iterable[str]) -> str:
+def format_csv_row(tile_info: Dict[TileKey, Any], keys_to_save: Iterable[TileKey], metadata_keys: Iterable[str]) -> str:
     """Format tile information dictionary as a row to write to a dataset CSV tile.
 
     :param tile_info: Tile information dictionary.
     :param keys_to_save: Which main keys to include in the row, and in which order.
     :param metadata_keys: Likewise for metadata keys.
     :return: The formatted CSV row.
     """
@@ -130,33 +125,49 @@
     fields.extend(str(tile_slide_metadata[key]) for key in metadata_keys)
     fields = ['"' + value + '"' if ',' in value else value for value in fields]  # if field contains a , add extra " "
 
     dataset_row = ','.join(fields)
     return dataset_row
 
 
-def process_slide(sample: Dict[SlideKey, Any], level: int, margin: int, tile_size: int,
-                  foreground_threshold: Optional[float], occupancy_threshold: float, output_dir: Path,
-                  tile_progress: bool = False) -> None:
+def process_slide(
+    sample: Dict[SlideKey, Any],
+    level: int,
+    margin: int,
+    tile_size: int,
+    foreground_threshold: Optional[float],
+    occupancy_threshold: float,
+    output_dir: Path,
+    tile_progress: bool = False,
+) -> None:
     """Load and process a slide, saving tile images and information to a CSV file.
 
     :param sample: Slide information dictionary, returned by the input slide dataset.
     :param level: Magnification level at which to process the slide.
     :param margin: Margin around the foreground bounding box, in pixels at lowest resolution.
     :param tile_size: Lateral dimensions of each tile, in pixels.
     :param foreground_threshold: Luminance threshold (0 to 255) to determine tile occupancy.
     If `None` (default), an optimal threshold will be estimated automatically.
     :param occupancy_threshold: Threshold (between 0 and 1) to determine empty tiles to discard.
     :param output_dir: Root directory for the output dataset; outputs for a single slide will be
     saved inside `output_dir/slide_id/`.
     :param tile_progress: Whether to display a progress bar in the terminal.
     """
     slide_metadata: Dict[str, Any] = sample[SlideKey.METADATA]
-    keys_to_save = (TileKey.SLIDE_ID, TileKey.TILE_ID, TileKey.IMAGE, TileKey.LABEL,
-                    TileKey.TILE_LEFT, TileKey.TILE_TOP, TileKey.TILE_RIGHT, TileKey.TILE_BOTTOM, TileKey.OCCUPANCY)
+    keys_to_save = (
+        TileKey.SLIDE_ID,
+        TileKey.TILE_ID,
+        TileKey.IMAGE,
+        TileKey.LABEL,
+        TileKey.TILE_LEFT,
+        TileKey.TILE_TOP,
+        TileKey.TILE_RIGHT,
+        TileKey.TILE_BOTTOM,
+        TileKey.OCCUPANCY,
+    )
     metadata_keys = tuple(key for key in slide_metadata)
     csv_columns: Tuple[str, ...] = (*keys_to_save, *metadata_keys)
 
     slide_id: str = sample[SlideKey.SLIDE_ID]
     rel_slide_dir = Path(slide_id)
     slide_dir = output_dir / rel_slide_dir
     print(f">>> Slide dir {slide_dir}")
@@ -173,26 +184,27 @@
 
             n_failed_tiles = 0
             failed_tiles_csv_path = slide_dir / "failed_tiles.csv"
             failed_tiles_file = failed_tiles_csv_path.open('w')
             failed_tiles_file.write('tile_id' + '\n')
 
             print(f"Loading slide {slide_id} ...")
-            loader = LoadROId(WSIReader('cuCIM'), level=level, margin=margin,
-                              foreground_threshold=foreground_threshold)
+            loader = LoadROId(
+                backend=WSIBackend.CUCIM, level=level, margin=margin, foreground_threshold=foreground_threshold
+            )
             sample = loader(sample)  # load 'image' from disk
 
             print(f"Tiling slide {slide_id} ...")
-            image_tiles, rel_tile_locations, occupancies, _ = \
-                generate_tiles(sample[SlideKey.IMAGE], tile_size,
-                               sample[SlideKey.FOREGROUND_THRESHOLD],
-                               occupancy_threshold)
-
-            tile_locations = (sample[SlideKey.SCALE] * rel_tile_locations
-                              + sample[SlideKey.ORIGIN]).astype(int)  # noqa: W503
+            image_tiles, rel_tile_locations, occupancies, _ = generate_tiles(
+                sample[SlideKey.IMAGE], tile_size, sample[SlideKey.FOREGROUND_THRESHOLD], occupancy_threshold
+            )
+
+            tile_locations = (sample[SlideKey.SCALE] * rel_tile_locations + sample[SlideKey.ORIGIN]).astype(
+                int
+            )  # noqa: W503
             tile_size_scaled = int(tile_size * sample[SlideKey.SCALE])
             tile_boxes = [Box(x, y, tile_size_scaled, tile_size_scaled) for x, y in tile_locations]
 
             n_tiles = image_tiles.shape[0]
 
             print(f"Saving tiles for slide {slide_id} ...")
             for i in tqdm(range(n_tiles), f"Tiles ({slide_id[:6]}…)", unit="img", disable=not tile_progress):
@@ -202,16 +214,17 @@
                     dataset_row = format_csv_row(tile_info, keys_to_save, metadata_keys)
                     dataset_csv_file.write(dataset_row + '\n')
                 except Exception as e:
                     n_failed_tiles += 1
                     descriptor = get_tile_descriptor(tile_boxes[i])
                     failed_tiles_file.write(descriptor + '\n')
                     traceback.print_exc()
-                    warnings.warn(f"An error occurred while saving tile "
-                                  f"{get_tile_id(slide_id, tile_boxes[i])}: {e}")
+                    warnings.warn(
+                        f"An error occurred while saving tile " f"{get_tile_id(slide_id, tile_boxes[i])}: {e}"
+                    )
 
             dataset_csv_file.close()
             failed_tiles_file.close()
             if n_failed_tiles > 0:
                 # TODO what we want to do with slides that have some failed tiles?
                 print(f"{slide_id} is incomplete. {n_failed_tiles} tiles failed.")
             print(f"Finished processing slide {slide_id}")
@@ -230,56 +243,80 @@
     with full_csv.open('w') as full_csv_file:
         # full_csv_file.write(','.join(CSV_COLUMNS) + '\n')  # write CSV header
         first_file = True
         for slide_csv in tqdm(dataset_dir.glob("*/dataset.csv"), desc="Merging dataset.csv", unit='file'):
             print(f"Merging slide {slide_csv}")
             content = slide_csv.read_text()
             if not first_file:
-                content = content[content.index('\n') + 1:]  # discard header row for all but the first file
+                content = content[content.index('\n') + 1 :]  # discard header row for all but the first file
             full_csv_file.write(content)
             first_file = False
     return full_csv
 
 
-def main(slides_dataset: SlidesDataset, root_output_dir: Union[str, Path],
-         level: int, tile_size: int, margin: int, foreground_threshold: Optional[float],
-         occupancy_threshold: float, parallel: bool = False, overwrite: bool = False,
-         n_slides: Optional[int] = None) -> None:
+def main(
+    slides_dataset: SlidesDataset,
+    root_output_dir: Union[str, Path],
+    level: int,
+    tile_size: int,
+    margin: int,
+    foreground_threshold: Optional[float],
+    occupancy_threshold: float,
+    parallel: bool = False,
+    overwrite: bool = False,
+    n_slides: Optional[int] = 0,
+    only: Optional[str] = None,
+) -> None:
     """Process a slides dataset to produce a tiles dataset.
 
     :param slides_dataset: Input tiles dataset object.
     :param root_output_dir: The root directory of the output tiles dataset.
     :param level: Magnification level at which to process the slide.
     :param tile_size: Lateral dimensions of each tile, in pixels.
     :param margin: Margin around the foreground bounding box, in pixels at lowest resolution.
     :param foreground_threshold: Luminance threshold (0 to 255) to determine tile occupancy.
     If `None` (default), an optimal threshold will be estimated automatically.
     :param occupancy_threshold: Threshold (between 0 and 1) to determine empty tiles to discard.
     :param parallel: Whether slides should be processed in parallel with multiprocessing.
     :param overwrite: Whether to overwrite an existing output tiles dataset. If `True`, will delete
     and recreate `root_output_dir`, otherwise will resume by skipping already processed slides.
     :param n_slides: If given, limit the total number of slides for debugging.
+    :param only: Id of a single slide for debugging.
     """
 
     # Ignoring some types here because mypy is getting confused with the MONAI Dataset class
     # to select a subsample use keyword n_slides
-    dataset = Dataset(slides_dataset)[:n_slides]  # type: ignore
+    if only:
+        slides_dataset.dataset_df = slides_dataset.dataset_df.filter(items=[only], axis=0)
+    dataset = Dataset(slides_dataset)  # type: ignore
+
+    if n_slides > 0:  # type: ignore
+        dataset = dataset[:n_slides]
+
     output_dir = Path(root_output_dir)
 
-    print(f"Creating dataset of level-{level} {tile_size}x{tile_size} "
-          f"{slides_dataset.__class__.__name__} tiles at: {output_dir}")
+    print(
+        f"Creating dataset of level-{level} {tile_size}x{tile_size} "
+        f"{slides_dataset.__class__.__name__} tiles at: {output_dir}"
+    )
 
     if overwrite and output_dir.exists():
         shutil.rmtree(output_dir)
     output_dir.mkdir(parents=True, exist_ok=not overwrite)
 
-    func = functools.partial(process_slide, level=level, margin=margin, tile_size=tile_size,
-                             foreground_threshold=foreground_threshold,
-                             occupancy_threshold=occupancy_threshold, output_dir=output_dir,
-                             tile_progress=not parallel)
+    func = functools.partial(
+        process_slide,
+        level=level,
+        margin=margin,
+        tile_size=tile_size,
+        foreground_threshold=foreground_threshold,
+        occupancy_threshold=occupancy_threshold,
+        output_dir=output_dir,
+        tile_progress=not parallel,
+    )
 
     if parallel:
         import multiprocessing
 
         pool = multiprocessing.Pool()
         map_func = pool.imap_unordered  # type: ignore
     else:
@@ -294,17 +331,20 @@
     merge_dataset_csv_files(output_dir)
 
 
 if __name__ == '__main__':
     from health_cpath.datasets.tcga_prad_dataset import TcgaPradDataset
 
     # Example set up for an existing slides dataset:
-    main(slides_dataset=TcgaPradDataset("/tmp/datasets/TCGA-PRAD_20220712"),
-         root_output_dir="/tmp/datasets/TCGA-PRAD_10X_tiles_level1_224",
-         n_slides=5,
-         level=1,
-         tile_size=224,
-         margin=0,
-         foreground_threshold=None,
-         occupancy_threshold=0.05,
-         parallel=True,
-         overwrite=True)
+    main(
+        slides_dataset=TcgaPradDataset("/tmp/datasets/TCGA-PRAD_20220712"),
+        root_output_dir="/tmp/datasets/TCGA-PRAD_10X_tiles_level1_224",
+        n_slides=2,
+        only=None,
+        level=0,
+        tile_size=224,
+        margin=0,
+        foreground_threshold=None,
+        occupancy_threshold=0.05,
+        parallel=True,
+        overwrite=True,
+    )
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/preprocessing/tiling.py` & `hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/tiling.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 
 def get_1d_padding(length: int, tile_size: int) -> Tuple[int, int]:
     """Computes symmetric padding for `length` to be divisible by `tile_size`."""
     pad = (tile_size - length % tile_size) % tile_size
     return (pad // 2, pad - pad // 2)
 
 
-def pad_for_tiling_2d(array: np.ndarray, tile_size: int, channels_first: Optional[bool] = True,
-                      **pad_kwargs: Any) -> Tuple[np.ndarray, np.ndarray]:
+def pad_for_tiling_2d(
+    array: np.ndarray, tile_size: int, channels_first: Optional[bool] = True, **pad_kwargs: Any
+) -> Tuple[np.ndarray, np.ndarray]:
     """Symmetrically pads a 2D `array` such that both dimensions are divisible by `tile_size`.
 
     :param array: 2D image array.
     :param tile_size: Width/height of each tile in pixels.
     :param channels_first: Whether `array` is in CHW (`True`, default) or HWC (`False`) layout.
     :param pad_kwargs: Keyword arguments to be passed to `np.pad()` (e.g. `constant_values=0`).
     :return: A tuple containing:
@@ -36,16 +37,17 @@
     channels_axis = 0 if channels_first else 2
     padding.insert(channels_axis, (0, 0))  # zero padding on channels axis
     padded_array = np.pad(array, padding, **pad_kwargs)
     offset = (padding_w[0], padding_h[0])
     return padded_array, np.array(offset)
 
 
-def tile_array_2d(array: np.ndarray, tile_size: int, channels_first: Optional[bool] = True,
-                  **pad_kwargs: Any) -> Tuple[np.ndarray, np.ndarray]:
+def tile_array_2d(
+    array: np.ndarray, tile_size: int, channels_first: Optional[bool] = True, **pad_kwargs: Any
+) -> Tuple[np.ndarray, np.ndarray]:
     """Split an image array into square non-overlapping tiles.
 
     The array will be padded symmetrically if its dimensions are not exact multiples of `tile_size`.
 
     :param array: Image array.
     :param tile_size: Width/height of each tile in pixels.
     :param pad_kwargs: Keyword arguments to be passed to `np.pad()` (e.g. `constant_values=0`).
@@ -80,32 +82,34 @@
     coords_w = tile_size * np.arange(n_tiles_w) - offset_w
     # Shape: (n_tiles_h * n_tiles_w, 2)
     coords = np.stack(np.meshgrid(coords_w, coords_h), axis=-1).reshape(-1, 2)
 
     return tiles, coords
 
 
-def assemble_tiles_2d(tiles: np.ndarray, coords: np.ndarray, fill_value: Optional[float] = np.nan,
-                      channels_first: Optional[bool] = True) -> Tuple[np.ndarray, np.ndarray]:
+def assemble_tiles_2d(
+    tiles: np.ndarray, coords: np.ndarray, fill_value: Optional[float] = np.nan, channels_first: Optional[bool] = True
+) -> Tuple[np.ndarray, np.ndarray]:
     """Assembles a 2D array from sequences of tiles and coordinates.
 
     :param tiles: Stack of tiles with batch dimension first.
     :param coords: XY tile coordinates, assumed to be spaced by multiples of `tile_size` (shape: [N, 2]).
     :param tile_size: Size of each tile; must be >0.
     :param fill_value: Value to assign to empty elements (default: `NaN`).
     :param channels_first: Whether each tile is in CHW (`True`, default) or HWC (`False`) layout.
     :return: A tuple containing:
         - `array`: The reassembled 2D array with the smallest dimensions to contain all given tiles.
         - `offset`: The lowest XY coordinates.
         - `offset`: XY offset introduced by the assembly. Add this to tile coordinates to obtain
         indices for the assembled array.
     """
     if coords.shape[0] != tiles.shape[0]:
-        raise ValueError(f"Tile coordinates and values must have the same length, "
-                         f"got {coords.shape[0]} and {tiles.shape[0]}")
+        raise ValueError(
+            f"Tile coordinates and values must have the same length, " f"got {coords.shape[0]} and {tiles.shape[0]}"
+        )
 
     if channels_first:
         n_tiles, channels, tile_size, _ = tiles.shape
     else:
         n_tiles, tile_size, _, channels = tiles.shape
     tile_xs, tile_ys = coords.T
 
@@ -117,12 +121,12 @@
     array = np.full(output_shape, fill_value)
 
     offset = np.array([-x_min, -y_min])
     for idx in range(n_tiles):
         row = coords[idx, 1] + offset[1]
         col = coords[idx, 0] + offset[0]
         if channels_first:
-            array[:, row:row + tile_size, col:col + tile_size] = tiles[idx]
+            array[:, row : row + tile_size, col : col + tile_size] = tiles[idx]
         else:
-            array[row:row + tile_size, col:col + tile_size, :] = tiles[idx]
+            array[row : row + tile_size, col : col + tile_size, :] = tiles[idx]
 
     return array, offset
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/scripts/aggregate_metrics_crossvalidation.py` & `hi-ml-cpath-0.3.0/src/health_cpath/scripts/aggregate_metrics_crossvalidation.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 import pandas as pd
 from azureml.core import Run
 from azureml.core.run import _OfflineRun
 
 HIML_ROOT = Path(__file__).parent.parent.parent.parent.parent.absolute()
 health_ml_root = HIML_ROOT / "hi-ml" / "src"
 health_azure_root = HIML_ROOT / "hi-ml-azure" / "src"
-print(f"Inserting into sys path: {health_ml_root}")
-print(f"Inserting into sys path: {health_azure_root}")
 sys.path.insert(0, str(health_ml_root))
 sys.path.insert(0, str(health_azure_root))
 
 from health_ml.utils.common_utils import df_to_json  # noqa: E402
 from health_azure import aggregate_hyperdrive_metrics  # NOQA: E402
-from health_azure.utils import get_aml_run_from_run_id, get_metrics_for_childless_run  # NOQA: E402
+from health_azure.utils import get_aml_run_from_run_id, get_metrics_for_run  # NOQA: E402
 
 
 def print_metrics(metrics_list: List[str], metrics_df: pd.DataFrame) -> None:
     """
     Given a DataFrame of metric names and corresponding values, and a list of the names metrics we
     want to print, attempts to locate each metric in the table and prints some summary statistics for it.
 
@@ -53,21 +51,18 @@
     :return: A Pandas DataFrame containing metric names and corresponding values.
     """
     print(f"Getting metrics for run {run.id}")
     if isinstance(run, _OfflineRun):
         raise ValueError("Can't get metrics for an OfflineRun")
     if len(list(run.get_children())) > 0:
         metrics_df = aggregate_hyperdrive_metrics(
-            child_run_arg_name="crossval_index",
-            run=run,
-            keep_metrics=metrics_list)
+            child_run_arg_name="crossval_index", run=run, keep_metrics=metrics_list
+        )
     else:
-        metrics_df = get_metrics_for_childless_run(
-            run=run,
-            keep_metrics=metrics_list)
+        metrics_df = get_metrics_for_run(run=run, keep_metrics=metrics_list)
     print_metrics(metrics_list, metrics_df)
     return metrics_df
 
 
 def upload_regression_metrics_file_to_run(metrics_df: pd.DataFrame, run: Run) -> None:
     """
     For a given metrics DataFrame, creates a temporary local csv file and uploads its to the provided
@@ -85,18 +80,23 @@
     run.upload_file("outputs/regression_metrics.json", str(metrics_json_output))
     metrics_json_output.unlink()
 
 
 if __name__ == "__main__":
     parser = ArgumentParser()
     parser.add_argument("--run", type=str, default='', help="The run id to retrieve metrics from")
-    parser.add_argument("--metrics_list", type=str,
-                        help="A comma-separated list of metrics names to retrieve from the AML Run")
-    parser.add_argument("--upload_metrics_file", type=bool, default=True,
-                        help="If True, saves a json file of the metrics dataframe and uploads this to the AML Run")
+    parser.add_argument(
+        "--metrics_list", type=str, help="A comma-separated list of metrics names to retrieve from the AML Run"
+    )
+    parser.add_argument(
+        "--upload_metrics_file",
+        type=bool,
+        default=True,
+        help="If True, saves a json file of the metrics dataframe and uploads this to the AML Run",
+    )
     args = parser.parse_args(sys.argv[1:])
     run_id = args.run
     metrics_list = args.metrics_list.split(",")
 
     run = get_aml_run_from_run_id(run_id)
     print(f"Run: {run}. Run id: {run.id}")
     metrics_df = get_metrics_from_run(run, metrics_list)
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/scripts/generate_crossval_report.py` & `hi-ml-cpath-0.3.0/src/health_cpath/scripts/generate_crossval_report.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,255 +7,388 @@
 from typing import Dict, List, Optional
 
 import pandas as pd
 from matplotlib import pyplot as plt
 
 from health_azure.utils import get_aml_run_from_run_id, get_workspace
 from health_ml.utils.reports import HTMLReport
-from health_cpath.utils.analysis_plot_utils import (add_training_curves_legend, plot_confusion_matrices,
-                                                    plot_crossval_roc_and_pr_curves,
-                                                    plot_crossval_training_curves)
-from health_cpath.utils.output_utils import (AML_LEGACY_TEST_OUTPUTS_CSV, AML_TEST_OUTPUTS_CSV,
-                                             AML_VAL_OUTPUTS_CSV)
-from health_cpath.utils.report_utils import (collect_crossval_metrics, collect_crossval_outputs,
-                                             crossval_runs_have_val_and_test_outputs, get_best_epoch_metrics,
-                                             get_best_epochs, get_crossval_metrics_table, get_formatted_run_info,
-                                             collect_class_info)
+from health_cpath.utils.analysis_plot_utils import (
+    add_training_curves_legend,
+    plot_confusion_matrices,
+    plot_hyperdrive_roc_and_pr_curves,
+    plot_hyperdrive_training_curves,
+)
+from health_cpath.utils.output_utils import AML_LEGACY_TEST_OUTPUTS_CSV, AML_TEST_OUTPUTS_CSV, AML_VAL_OUTPUTS_CSV
+from health_cpath.utils.report_utils import (
+    collect_hyperdrive_metrics,
+    collect_hyperdrive_outputs,
+    child_runs_have_val_and_test_outputs,
+    get_best_epoch_metrics,
+    get_best_epochs,
+    get_child_runs_hyperparams,
+    get_hyperdrive_metrics_table,
+    get_formatted_run_info,
+    collect_class_info,
+    get_max_epochs,
+    download_hyperdrive_metrics_if_required,
+)
 from health_cpath.utils.naming import MetricsKey, ModelKey
 
 
-def generate_html_report(parent_run_id: str, output_dir: Path,
-                         workspace_config_path: Optional[Path] = None,
-                         include_test: bool = False, overwrite: bool = False) -> None:
+def generate_html_report(
+    parent_run_id: str,
+    output_dir: Path,
+    workspace_config_path: Optional[Path] = None,
+    include_test: bool = False,
+    overwrite: bool = False,
+    hyperdrive_arg_name: str = "crossval_index",
+    primary_metric: str = MetricsKey.AUROC,
+) -> None:
     """
-    Function to generate an HTML report of a cross validation AML run.
+    Function to generate an HTML report of a Hyperdrive AML run (e.g., cross validation, different random seeds, ...).
 
     :param run_id: The parent Hyperdrive run ID.
     :param output_dir: Directory where to download Azure ML data and save the report.
     :param workspace_config_path: Path to Azure ML workspace config.json file.
         If omitted, will try to load default workspace.
     :param include_test: Include test results in the generated report.
     :param overwrite: Forces (re)download of metrics and output files, even if they already exist locally.
+    :param hyperdrive_arg_name: Name of the Hyperdrive argument used for indexing the child runs.
+        Default `crossval_index`.
+    :param primary_metric: Name of the reference metric to optimise. Default `MetricsKey.AUROC`.
     """
     aml_workspace = get_workspace(workspace_config_path=workspace_config_path)
     parent_run = get_aml_run_from_run_id(parent_run_id, aml_workspace=aml_workspace)
     report_dir = output_dir / parent_run.display_name
     report_dir.mkdir(parents=True, exist_ok=True)
 
     report = HTMLReport(output_folder=report_dir)
 
     report.add_text(get_formatted_run_info(parent_run))
 
     report.add_heading("Azure ML metrics", level=2)
 
     # Download metrics from AML. Can take several seconds for each child run
-    metrics_df = collect_crossval_metrics(parent_run_id, report_dir, aml_workspace, overwrite=overwrite)
-    best_epochs = get_best_epochs(metrics_df, f'{ModelKey.VAL}/{MetricsKey.AUROC}', maximise=True)
+    metrics_json = download_hyperdrive_metrics_if_required(
+        parent_run_id, report_dir, aml_workspace, overwrite=overwrite, hyperdrive_arg_name=hyperdrive_arg_name
+    )
+
+    # Get metrics dataframe from the downloaded json file
+    metrics_df = collect_hyperdrive_metrics(metrics_json=metrics_json)
+
+    hyperparameters_children = get_child_runs_hyperparams(metrics_df)
+    max_epochs_dict = get_max_epochs(hyperparams_children=hyperparameters_children)
+    best_epochs = get_best_epochs(
+        metrics_df=metrics_df,
+        primary_metric=f'{ModelKey.VAL}/{primary_metric}',
+        max_epochs_dict=max_epochs_dict,
+        maximise=True,
+    )
 
     # Add training curves for loss and AUROC (train and val.)
-    render_training_curves(report, heading="Training curves", level=3,
-                           metrics_df=metrics_df, best_epochs=best_epochs, report_dir=report_dir)
+    render_training_curves(
+        report,
+        heading="Training curves",
+        level=3,
+        metrics_df=metrics_df,
+        best_epochs=best_epochs,
+        report_dir=report_dir,
+        primary_metric=primary_metric,
+    )
 
     # Get metrics list with class names
-    num_classes, class_names = collect_class_info(metrics_df=metrics_df)
+    num_classes, class_names = collect_class_info(hyperparams_children=hyperparameters_children)
 
-    base_metrics_list: List[str]
+    base_metrics_list: List[str] = [
+        MetricsKey.ACC,
+        MetricsKey.AUROC,
+        MetricsKey.AVERAGE_PRECISION,
+        MetricsKey.COHENKAPPA,
+    ]
     if num_classes > 1:
-        base_metrics_list = [MetricsKey.ACC, MetricsKey.AUROC]
+        base_metrics_list += [MetricsKey.ACC_MACRO, MetricsKey.ACC_WEIGHTED]
     else:
-        base_metrics_list = [MetricsKey.ACC, MetricsKey.AUROC, MetricsKey.PRECISION, MetricsKey.RECALL, MetricsKey.F1]
+        base_metrics_list += [MetricsKey.F1, MetricsKey.PRECISION, MetricsKey.RECALL, MetricsKey.SPECIFICITY]
 
     base_metrics_list += class_names
 
     # Add tables with relevant metrics (val. and test)
-    render_metrics_table(report, heading="Validation metrics (best epoch based on maximum validation AUROC)", level=3,
-                         metrics_df=metrics_df, best_epochs=best_epochs,
-                         base_metrics_list=base_metrics_list, metrics_prefix=f'{ModelKey.VAL}/')
+    render_metrics_table(
+        report,
+        heading=f"Validation metrics (best epoch based on maximum validation {primary_metric})",
+        level=3,
+        metrics_df=metrics_df,
+        best_epochs=best_epochs,
+        base_metrics_list=base_metrics_list,
+        metrics_prefix=f'{ModelKey.VAL}/',
+    )
 
     if include_test:
-        render_metrics_table(report, heading="Test metrics", level=3,
-                             metrics_df=metrics_df, best_epochs=None,
-                             base_metrics_list=base_metrics_list, metrics_prefix=f'{ModelKey.TEST}/')
-
-    has_val_and_test_outputs = crossval_runs_have_val_and_test_outputs(parent_run)
-
-    # Get output data frames
-    if has_val_and_test_outputs:
-        output_filename_val = AML_VAL_OUTPUTS_CSV
-        outputs_dfs_val = collect_crossval_outputs(parent_run_id=parent_run_id, download_dir=report_dir,
-                                                   aml_workspace=aml_workspace,
-                                                   output_filename=output_filename_val, overwrite=overwrite)
-        if include_test:
-            output_filename_test = AML_TEST_OUTPUTS_CSV if has_val_and_test_outputs else AML_LEGACY_TEST_OUTPUTS_CSV
-            outputs_dfs_test = collect_crossval_outputs(parent_run_id=parent_run_id, download_dir=report_dir,
-                                                        aml_workspace=aml_workspace,
-                                                        output_filename=output_filename_test, overwrite=overwrite)
-
-    if num_classes == 1:
-        # Currently ROC and PR curves rendered only for binary case
-        # TODO: Enable rendering of multi-class ROC and PR curves
-        report.add_heading("ROC and PR curves", level=2)
+        render_metrics_table(
+            report,
+            heading="Test metrics",
+            level=3,
+            metrics_df=metrics_df,
+            best_epochs=None,
+            base_metrics_list=base_metrics_list,
+            metrics_prefix=f'{ModelKey.TEST}/',
+        )
+
+    # Get output data frames if available
+    try:
+        has_val_and_test_outputs = child_runs_have_val_and_test_outputs(parent_run)
         if has_val_and_test_outputs:
-            # Add val. ROC and PR curves
-            render_roc_and_pr_curves(report=report, heading="Validation ROC and PR curves", level=3,
-                                     report_dir=report_dir,
-                                     outputs_dfs=outputs_dfs_val,
-                                     prefix=f'{ModelKey.VAL}_')
-        if include_test:
-            # Add test ROC and PR curves
-            render_roc_and_pr_curves(report=report, heading="Test ROC and PR curves", level=3,
-                                     report_dir=report_dir,
-                                     outputs_dfs=outputs_dfs_test,
-                                     prefix=f'{ModelKey.TEST}_')
-
-    # Add confusion matrices for each fold
-
-    report.add_heading("Confusion matrices", level=2)
-
-    if has_val_and_test_outputs:
-        # Add val. confusion matrices
-        render_confusion_matrices(report=report, heading="Validation confusion matrices", level=3,
-                                  class_names=class_names,
-                                  report_dir=report_dir, outputs_dfs=outputs_dfs_val,
-                                  prefix=f'{ModelKey.VAL}_')
+            output_filename_val = AML_VAL_OUTPUTS_CSV
+            outputs_dfs_val = collect_hyperdrive_outputs(
+                parent_run_id=parent_run_id,
+                download_dir=report_dir,
+                aml_workspace=aml_workspace,
+                output_filename=output_filename_val,
+                overwrite=overwrite,
+                hyperdrive_arg_name=hyperdrive_arg_name,
+            )
+            if include_test:
+                output_filename_test = AML_TEST_OUTPUTS_CSV if has_val_and_test_outputs else AML_LEGACY_TEST_OUTPUTS_CSV
+                outputs_dfs_test = collect_hyperdrive_outputs(
+                    parent_run_id=parent_run_id,
+                    download_dir=report_dir,
+                    aml_workspace=aml_workspace,
+                    output_filename=output_filename_test,
+                    overwrite=overwrite,
+                    hyperdrive_arg_name=hyperdrive_arg_name,
+                )
+
+        if num_classes == 1:
+            # Currently ROC and PR curves rendered only for binary case
+            # TODO: Enable rendering of multi-class ROC and PR curves
+            report.add_heading("ROC and PR curves", level=2)
+            if has_val_and_test_outputs:
+                # Add val. ROC and PR curves
+                render_roc_and_pr_curves(
+                    report=report,
+                    heading="Validation ROC and PR curves",
+                    level=3,
+                    report_dir=report_dir,
+                    outputs_dfs=outputs_dfs_val,
+                    prefix=f'{ModelKey.VAL}_',
+                )
+            if include_test:
+                # Add test ROC and PR curves
+                render_roc_and_pr_curves(
+                    report=report,
+                    heading="Test ROC and PR curves",
+                    level=3,
+                    report_dir=report_dir,
+                    outputs_dfs=outputs_dfs_test,
+                    prefix=f'{ModelKey.TEST}_',
+                )
 
-    if include_test:
-        # Add test confusion matrices
-        render_confusion_matrices(report=report, heading="Test confusion matrices", level=3,
-                                  class_names=class_names,
-                                  report_dir=report_dir, outputs_dfs=outputs_dfs_test,
-                                  prefix=f'{ModelKey.TEST}_')
+        # Add confusion matrices for each fold
+        report.add_heading("Confusion matrices", level=2)
+        if has_val_and_test_outputs:
+            # Add val. confusion matrices
+            render_confusion_matrices(
+                report=report,
+                heading="Validation confusion matrices",
+                level=3,
+                class_names=class_names,
+                report_dir=report_dir,
+                outputs_dfs=outputs_dfs_val,
+                prefix=f'{ModelKey.VAL}_',
+            )
+
+        if include_test:
+            # Add test confusion matrices
+            render_confusion_matrices(
+                report=report,
+                heading="Test confusion matrices",
+                level=3,
+                class_names=class_names,
+                report_dir=report_dir,
+                outputs_dfs=outputs_dfs_test,
+                prefix=f'{ModelKey.TEST}_',
+            )
+
+    except ValueError as e:
+        print(e)
+        print("Since all expected output files were not found, skipping ROC-PR curves and confusion matrices.")
 
     # TODO: Add qualitative model outputs
     # report.add_heading("Qualitative model outputs", level=2)
 
     print(f"Rendering report to: {report.report_path_html.resolve()}")
     report.render()
 
 
-def render_training_curves(report: HTMLReport, heading: str, level: int,
-                           metrics_df: pd.DataFrame, best_epochs: Optional[Dict[int, int]],
-                           report_dir: Path) -> None:
+def render_training_curves(
+    report: HTMLReport,
+    heading: str,
+    level: int,
+    metrics_df: pd.DataFrame,
+    best_epochs: Optional[Dict[int, int]],
+    report_dir: Path,
+    primary_metric: str = MetricsKey.AUROC,
+) -> None:
     """
     Function to render training curves for HTML reports.
 
     :param report: HTML report to perform the rendering.
     :param heading: Heading of the section.
     :param level: Level of HTML heading (e.g. sub-section, sub-sub-section) corresponding to HTML heading levels.
-    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_crossval_metrics()` and
+    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_hyperdrive_metrics()` and
         :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
-    :param best_epochs: Dictionary mapping each cross-validation index to its best epoch.
+    :param best_epochs: Dictionary mapping each hyperdrive child index to its best epoch.
     :param report_dir: Directory of the HTML report.
+    :param primary_metric: Primary metric name. Default is AUROC.
     """
     report.add_heading(heading, level=level)
-    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(8, 4))
-    plot_crossval_training_curves(metrics_df, train_metric=f'{ModelKey.TRAIN}/loss_epoch',
-                                  val_metric=f'{ModelKey.VAL}/loss_epoch',
-                                  ylabel="Loss", best_epochs=best_epochs, ax=ax1)
-    plot_crossval_training_curves(metrics_df, train_metric=f'{ModelKey.TRAIN}/{MetricsKey.AUROC}',
-                                  val_metric=f'{ModelKey.VAL}/{MetricsKey.AUROC}',
-                                  ylabel="AUROC", best_epochs=best_epochs, ax=ax2)
+    metrics = {"loss_epoch", MetricsKey.AUROC.value, primary_metric}
+    fig, axs = plt.subplots(1, len(metrics), figsize=(5 * len(metrics), 4))
+    for i, metric in enumerate(metrics):
+        plot_hyperdrive_training_curves(
+            metrics_df,
+            train_metric=f'{ModelKey.TRAIN}/{metric}',
+            val_metric=f'{ModelKey.VAL}/{metric}',
+            ylabel=metric,
+            best_epochs=best_epochs,
+            ax=axs[i],
+        )
     add_training_curves_legend(fig, include_best_epoch=True)
     training_curves_fig_path = report_dir / "training_curves.png"
     fig.savefig(training_curves_fig_path, bbox_inches='tight')
     report.add_images([training_curves_fig_path], base64_encode=True)
 
 
-def render_metrics_table(report: HTMLReport, heading: str, level: int,
-                         metrics_df: pd.DataFrame, best_epochs: Optional[Dict[int, int]],
-                         base_metrics_list: List[str], metrics_prefix: str) -> None:
+def render_metrics_table(
+    report: HTMLReport,
+    heading: str,
+    level: int,
+    metrics_df: pd.DataFrame,
+    best_epochs: Optional[Dict[int, int]],
+    base_metrics_list: List[str],
+    metrics_prefix: str,
+) -> None:
     """
     Function to render metrics table for HTML reports.
 
     :param report: HTML report to perform the rendering.
     :param heading: Heading of the section.
     :param level: Level of HTML heading (e.g. sub-section, sub-sub-section) corresponding to HTML heading levels.
-    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_crossval_metrics()` and
+    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_hyperdrive_metrics()` and
         :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
     :param base_metrics_list: List of metric names to include in the table.
-    :param best_epochs: Dictionary mapping each cross-validation index to its best epoch.
+    :param best_epochs: Dictionary mapping each hyperdrive child index to its best epoch.
     :param metrics_prefix: Prefix to add to the metrics names (e.g. `val`, `test`)
     """
     report.add_heading(heading, level=level)
     metrics_list = [metrics_prefix + metric for metric in base_metrics_list]
     if best_epochs:
         metrics_df = get_best_epoch_metrics(metrics_df, metrics_list, best_epochs)
-    metrics_table = get_crossval_metrics_table(metrics_df, metrics_list)
+    metrics_table = get_hyperdrive_metrics_table(metrics_df, metrics_list)
     report.add_tables([metrics_table])
 
 
-def render_roc_and_pr_curves(report: HTMLReport, heading: str, level: int, report_dir: Path,
-                             outputs_dfs: Dict[int, pd.DataFrame], prefix: str = '') -> None:
+def render_roc_and_pr_curves(
+    report: HTMLReport,
+    heading: str,
+    level: int,
+    report_dir: Path,
+    outputs_dfs: Dict[int, pd.DataFrame],
+    prefix: str = '',
+) -> None:
     """
     Function to render ROC and PR curves for HTML reports.
 
     :param report: HTML report to perform the rendering.
     :param heading: Heading of the section.
     :param level: Level of HTML heading (e.g. sub-section, sub-sub-section) corresponding to HTML heading levels.
     :param report_dir: Local directory where the report is stored.
-    :param outputs_dfs: A dictionary of dataframes with the sorted cross-validation indices as keys.
+    :param outputs_dfs: A dictionary of dataframes with the sorted hyperdrive child runs indices as keys.
     :param prefix: Prefix to add to the figures saved (e.g. `val`, `test`).
     """
     report.add_heading(heading, level=level)
-    fig = plot_crossval_roc_and_pr_curves(outputs_dfs, scores_column='prob_class1')
+    fig = plot_hyperdrive_roc_and_pr_curves(outputs_dfs, scores_column='prob_class1')
     roc_pr_curves_fig_path = report_dir / f"{prefix}roc_pr_curves.png"
     fig.savefig(roc_pr_curves_fig_path, bbox_inches='tight')
     report.add_images([roc_pr_curves_fig_path], base64_encode=True)
 
 
-def render_confusion_matrices(report: HTMLReport, heading: str, level: int, class_names: List[str],
-                              report_dir: Path, outputs_dfs: Dict[int, pd.DataFrame], prefix: str = '') -> None:
+def render_confusion_matrices(
+    report: HTMLReport,
+    heading: str,
+    level: int,
+    class_names: List[str],
+    report_dir: Path,
+    outputs_dfs: Dict[int, pd.DataFrame],
+    prefix: str = '',
+) -> None:
     """
     Function to render confusion matrices for HTML reports.
 
     :param report: HTML report to perform the rendering.
     :param heading: Heading of the section.
     :param level: Level of HTML heading (e.g. sub-section, sub-sub-section) corresponding to HTML heading levels.
     :param class_names: Names of classes.
     :param report_dir: Local directory where the report is stored.
-    :param outputs_dfs: A dictionary of dataframes with the sorted cross-validation indices as keys.
+    :param outputs_dfs: A dictionary of dataframes with the sorted hyperdrive child runs indices as keys.
     :param prefix: Prefix to add to the figures saved (e.g. `val`, `test`).
     """
     report.add_heading(heading, level=level)
-    fig = plot_confusion_matrices(crossval_dfs=outputs_dfs, class_names=class_names)
+    fig = plot_confusion_matrices(hyperdrive_dfs=outputs_dfs, class_names=class_names)
     confusion_matrices_fig_path = report_dir / f"{prefix}confusion_matrices.png"
     fig.savefig(confusion_matrices_fig_path, bbox_inches='tight')
     report.add_images([confusion_matrices_fig_path], base64_encode=True)
 
 
 if __name__ == "__main__":
     """
     Usage example from CLI:
-    python generate_crossval_report.py \
+    python generate_hyperdrive_report.py \
     --run_id <insert AML run ID here> \
     --output_dir outputs \
     --include_test
     """
 
     from argparse import ArgumentParser
 
     parser = ArgumentParser()
     parser.add_argument('--run_id', help="The parent Hyperdrive run ID.")
     parser.add_argument('--output_dir', help="Directory where to download Azure ML data and save the report.")
-    parser.add_argument('--workspace_config', help="Path to Azure ML workspace config.json file. "
-                                                   "If omitted, will try to load default workspace.")
-    parser.add_argument('--include_test', action='store_true', help="Opt-in flag to include test results "
-                                                                    "in the generated report.")
-    parser.add_argument('--overwrite', action='store_true', help="Forces (re)download of metrics and output files, "
-                                                                 "even if they already exist locally.")
+    parser.add_argument(
+        '--workspace_config',
+        help="Path to Azure ML workspace config.json file. If omitted, will try to load default workspace.",
+    )
+    parser.add_argument(
+        '--include_test', action='store_true', help="Opt-in flag to include test results in the generated report."
+    )
+    parser.add_argument(
+        '--overwrite',
+        action='store_true',
+        help="Forces (re)download of metrics and output files, even if they already exist locally.",
+    )
+    parser.add_argument(
+        "--hyper_arg_name",
+        default="crossval_index",
+        help="Name of the Hyperdrive argument used for indexing the child runs.",
+    )
+    parser.add_argument("--primary_metric", default=MetricsKey.AUROC, help="Name of the reference metric to optimise.")
     args = parser.parse_args()
 
     if args.output_dir is None:
         args.output_dir = Path.cwd() / "outputs"
     workspace_config = Path(args.workspace_config).resolve() if args.workspace_config else None
 
     print(f"Output dir: {Path(args.output_dir).resolve()}")
     if workspace_config is not None:
         if not workspace_config.is_file():
             raise ValueError(f"Specified workspace config file does not exist: {workspace_config}")
         print(f"Workspace config: {workspace_config}")
 
-    generate_html_report(parent_run_id=args.run_id,
-                         output_dir=Path(args.output_dir),
-                         workspace_config_path=workspace_config,
-                         include_test=args.include_test,
-                         overwrite=args.overwrite)
+    generate_html_report(
+        parent_run_id=args.run_id,
+        output_dir=Path(args.output_dir),
+        workspace_config_path=workspace_config,
+        include_test=args.include_test,
+        overwrite=args.overwrite,
+        hyperdrive_arg_name=args.hyper_arg_name,
+        primary_metric=args.primary_metric,
+    )
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/scripts/mount_azure_dataset.py` & `hi-ml-cpath-0.3.0/src/health_cpath/scripts/mount_azure_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 from pathlib import Path
 import sys
 import time
-from typing import Any
+from typing import Any, Optional
+from azureml.core import Workspace
 
 himl_histo_root_dir = Path(__file__).parent.parent.parent
 himl_root = himl_histo_root_dir.parent.parent
 himl_azure_package_root = himl_root / "hi-ml-azure" / "src"
 sys.path.insert(0, str(himl_azure_package_root))
 
 from health_azure import DatasetConfig  # noqa: E402
 from health_azure.utils import get_workspace  # noqa: E402
 
 
-def mount_dataset(dataset_id: str) -> Any:
-    ws = get_workspace()
-    target_folder = "/tmp/datasets/" + dataset_id
+def mount_dataset(dataset_id: str, tmp_root: str = "/tmp/datasets", aml_workspace: Optional[Workspace] = None) -> Any:
+    ws = get_workspace(aml_workspace)
+    target_folder = "/".join([tmp_root, dataset_id])
     dataset = DatasetConfig(name=dataset_id, target_folder=target_folder, use_mounting=True)
-    _, mount_ctx = dataset.to_input_dataset_local(ws)
+    _, mount_ctx = dataset.to_input_dataset_local(strictly_aml_v1=True, workspace=ws)
     assert mount_ctx is not None  # for mypy
     mount_ctx.start()
     return mount_ctx
 
 
 if __name__ == '__main__':
     import argparse
+
     parser = argparse.ArgumentParser()
     # Run this script as "python mount_azure_dataset.py --dataset_id TCGA-CRCk"
-    parser.add_argument('--dataset_id', type=str,
-                        help='Name of the Azure dataset e.g. PANDA or TCGA-CRCk')
+    parser.add_argument('--dataset_id', type=str, help='Name of the Azure dataset e.g. PANDA or TCGA-CRCk')
     args = parser.parse_args()
     # It is essential that the mount context is returned from the mounting function and referenced here.
     # If not, mounting will be stopped, and the files are no longer available.
     _ = mount_dataset(args.dataset_id)
     print("The mounted dataset will only be available while this script is running. Press Ctrl-C to terminate it.`")
     while True:
         time.sleep(60)
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/scripts/tcga_dataset_prep.py` & `hi-ml-cpath-0.3.0/src/health_cpath/scripts/tcga_dataset_prep.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,38 +4,40 @@
 #  -------------------------------------------------------------------------------------------
 from pathlib import Path
 
 import pandas as pd
 from health_cpath.datasets.default_paths import TCGA_CRCK_DATASET_ID
 
 from health_cpath.utils.tcga_utils import extract_fields
-from health_cpath.datasets.tcga_prad_dataset import TcgaPradDataset
+from health_cpath.datasets.tcga_prad_dataset import TCGA_PRAD_DATASET_FILE
 
 
 def check_dataset_csv_paths(dataset_dir: Path) -> None:
-    df = pd.read_csv(dataset_dir / TcgaPradDataset.DEFAULT_CSV_FILENAME)
+    df = pd.read_csv(dataset_dir / TCGA_PRAD_DATASET_FILE)
     for img_path in df.image:
         assert (dataset_dir / img_path).is_file()
 
 
 if __name__ == '__main__':
     # Script needs to be started in the parent folder of the dataset folder
     current_dir = Path.cwd()
     expected_datasetdir = TCGA_CRCK_DATASET_ID
-    if not (current_dir / expected_datasetdir).is_dir:
+    if not (current_dir / expected_datasetdir).is_dir():
         raise ValueError(f"The current folder must contain the actual dataset folder {expected_datasetdir}")
     dataset_dir = current_dir / expected_datasetdir
     expected_subdirs = ["CRC_DX_TEST", "CRC_DX_TRAIN"]
     if not all([(dataset_dir / subdir).is_dir() for subdir in expected_subdirs]):
         raise ValueError(f"The folder {expected_datasetdir} needs to have these subfolder: {expected_subdirs}")
-    image_paths = [str(image_path.relative_to(dataset_dir))
-                   for split_dir in dataset_dir.iterdir()
-                   for class_dir in split_dir.iterdir()
-                   for image_path in class_dir.iterdir()]
+    image_paths = [
+        str(image_path.relative_to(dataset_dir))
+        for split_dir in dataset_dir.iterdir()
+        for class_dir in split_dir.iterdir()
+        for image_path in class_dir.iterdir()
+    ]
 
     df = pd.DataFrame(image_paths, columns=['image'])
 
     # takes up to ~20 seconds
     df = df.apply(extract_fields, axis='columns', result_type='expand')
-    df.to_csv(dataset_dir / TcgaPradDataset.DEFAULT_CSV_FILENAME, index=False)
+    df.to_csv(dataset_dir / TCGA_PRAD_DATASET_FILE, index=False)
 
     check_dataset_csv_paths(dataset_dir)
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/analysis_plot_utils.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/analysis_plot_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,40 +116,40 @@
     :param title: plot title string
     """
     plt.figure()
     plt.hist(data, bins=50)
     plt.gca().set(title=title, xlabel='Values', ylabel='Frequency')
 
 
-def plot_roc_curve(labels: Sequence, scores: Sequence, label: str, ax: Axes) -> None:
+def plot_roc_curve(labels: Sequence, scores: Sequence, legend_label: str, ax: Axes) -> None:
     """Plot ROC curve for the given labels and scores, with AUROC in the line legend.
 
     :param labels: The true binary labels.
     :param scores: Scores predicted by the model.
-    :param label: An line identifier to be displayed in the legend.
+    :param legend_label: An line identifier to be displayed in the legend.
     :param ax: `Axes` object onto which to plot.
     """
     fpr, tpr, _ = roc_curve(labels, scores)
     auroc = auc(fpr, tpr)
-    label = f"{label} (AUROC: {auroc:.3f})"
-    ax.plot(fpr, tpr, label=label)
+    legend_label = f"{legend_label} (AUROC: {auroc:.3f})"
+    ax.plot(fpr, tpr, label=legend_label)
 
 
-def plot_pr_curve(labels: Sequence, scores: Sequence, label: str, ax: Axes) -> None:
-    """Plot precision-recall curve for the given labels and scores, with AUROC in the line legend.
+def plot_pr_curve(labels: Sequence, scores: Sequence, legend_label: str, ax: Axes) -> None:
+    """Plot precision-recall curve for the given labels and scores, with AUPR in the line legend.
 
     :param labels: The true binary labels.
     :param scores: Scores predicted by the model.
-    :param label: An line identifier to be displayed in the legend.
+    :param legend_label: A line identifier to be displayed in the legend.
     :param ax: `Axes` object onto which to plot.
     """
     precision, recall, _ = precision_recall_curve(labels, scores)
     aupr = auc(recall, precision)
-    label = f"{label} (AUPR: {aupr:.3f})"
-    ax.plot(recall, precision, label=label)
+    legend_label = f"{legend_label} (AUPR: {aupr:.3f})"
+    ax.plot(recall, precision, label=legend_label)
 
 
 def format_pr_or_roc_axes(plot_type: str, ax: Axes) -> None:
     """Format PR or ROC plot with appropriate axis labels, limits, and grid.
 
     :param plot_type: Either 'pr' or 'roc'.
     :param ax: `Axes` object to format.
@@ -159,153 +159,196 @@
     elif plot_type == 'roc':
         xlabel, ylabel = "False positive rate", "True positive rate"
     else:
         raise ValueError(f"Plot type must be either 'pr' or 'roc' (received '{plot_type}')")
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     ax.set_aspect(1)
-    ax.set_xlim(-.05, 1.05)
-    ax.set_ylim(-.05, 1.05)
+    ax.set_xlim(-0.05, 1.05)
+    ax.set_ylim(-0.05, 1.05)
     ax.grid(color='0.9')
 
 
-def _plot_crossval_roc_and_pr_curves(crossval_dfs: Dict[int, pd.DataFrame], roc_ax: Axes, pr_ax: Axes,
-                                     scores_column: str = ResultsKey.PROB) -> None:
-    """Plot ROC and precision-recall curves for multiple cross-validation runs onto provided axes.
+def _plot_hyperdrive_roc_and_pr_curves(
+    hyperdrive_dfs: Dict[int, pd.DataFrame], roc_ax: Axes, pr_ax: Axes, scores_column: str = ResultsKey.PROB
+) -> None:
+    """Plot ROC and precision-recall curves for multiple hyperdrive runs onto provided axes.
 
-    This is called by :py:func:`plot_crossval_roc_and_pr_curves()`, which additionally creates a figure and the axes.
+    This is called by :py:func:`plot_hyperdrive_roc_and_pr_curves()`, which additionally creates a figure and the axes.
 
-    :param crossval_dfs: Dictionary of dataframes with cross-validation indices as keys,
-        as returned by :py:func:`collect_crossval_outputs()`.
+    :param hyperdrive_dfs: Dictionary of dataframes with hyperdrive child runs indices as keys,
+        as returned by :py:func:`collect_hyperdrive_outputs()`.
     :param roc_ax: `Axes` object onto which to plot ROC curves.
     :param pr_ax: `Axes` object onto which to plot precision-recall curves.
     """
-    for k, tiles_df in crossval_dfs.items():
+    for k, tiles_df in hyperdrive_dfs.items():
         slides_groupby = tiles_df.groupby(ResultsKey.SLIDE_ID)
 
         tile_labels = slides_groupby[ResultsKey.TRUE_LABEL]
         # True slide label is guaranteed unique
         assert all(len(unique_slide_label) == 1 for unique_slide_label in tile_labels.unique())
         labels = tile_labels.first()
 
         tile_scores = slides_groupby[scores_column]
-        non_unique_slides = [slide_id for slide_id, unique_slide_score in tile_scores.unique().items()
-                             if len(unique_slide_score) > 1]
+        non_unique_slides = [
+            slide_id for slide_id, unique_slide_score in tile_scores.unique().items() if len(unique_slide_score) > 1
+        ]
         if non_unique_slides:
-            warnings.warn(f"Found {len(non_unique_slides)}/{len(slides_groupby)} non-unique slides in fold {k}: "
-                          f"{sorted(non_unique_slides)}")
+            warnings.warn(
+                f"Found {len(non_unique_slides)}/{len(slides_groupby)} non-unique slides in fold {k}: "
+                f"{sorted(non_unique_slides)}"
+            )
         # TODO: Re-enable assertion once we can guarantee uniqueness of slides during validation
         # assert len(non_unique_slides) == 0
         scores = tile_scores.first()
 
-        plot_roc_curve(labels, scores, label=f"Fold {k}", ax=roc_ax)
-        plot_pr_curve(labels, scores, label=f"Fold {k}", ax=pr_ax)
+        plot_roc_curve(labels, scores, legend_label=f"Child {k}", ax=roc_ax)
+        plot_pr_curve(labels, scores, legend_label=f"Child {k}", ax=pr_ax)
     legend_kwargs = dict(edgecolor='none', fontsize='small')
     roc_ax.legend(**legend_kwargs)
     pr_ax.legend(**legend_kwargs)
     format_pr_or_roc_axes('roc', roc_ax)
     format_pr_or_roc_axes('pr', pr_ax)
 
 
-def plot_crossval_roc_and_pr_curves(crossval_dfs: Dict[int, pd.DataFrame],
-                                    scores_column: str = ResultsKey.PROB) -> Figure:
-    """Plot ROC and precision-recall curves for multiple cross-validation runs.
+def plot_hyperdrive_roc_and_pr_curves(
+    hyperdrive_dfs: Dict[int, pd.DataFrame], scores_column: str = ResultsKey.PROB
+) -> Figure:
+    """Plot ROC and precision-recall curves for multiple hyperdrive child runs.
 
     This will create a new figure with two subplots (left: ROC, right: PR).
 
-    :param crossval_dfs: Dictionary of dataframes with cross-validation indices as keys,
-        as returned by :py:func:`collect_crossval_outputs()`.
+    :param hyperdrive_dfs: Dictionary of dataframes with hyperdrive child indices as keys,
+        as returned by :py:func:`collect_hyperdrive_outputs()`.
     :return: The created `Figure` object.
     """
     fig, axs = plt.subplots(1, 2, figsize=(8, 4))
-    _plot_crossval_roc_and_pr_curves(crossval_dfs, scores_column=scores_column, roc_ax=axs[0], pr_ax=axs[1])
+    _plot_hyperdrive_roc_and_pr_curves(hyperdrive_dfs, scores_column=scores_column, roc_ax=axs[0], pr_ax=axs[1])
     return fig
 
 
-def plot_crossval_training_curves(metrics_df: pd.DataFrame, train_metric: str, val_metric: str, ax: Axes,
-                                  best_epochs: Optional[Dict[int, int]] = None, ylabel: Optional[str] = None) -> None:
-    """Plot paired training and validation metrics for every training epoch of cross-validation runs.
+def plot_hyperdrive_training_curves(
+    metrics_df: pd.DataFrame,
+    train_metric: str,
+    val_metric: str,
+    ax: Axes,
+    best_epochs: Optional[Dict[int, int]] = None,
+    ylabel: Optional[str] = None,
+) -> None:
+    """Plot paired training and validation metrics for every training epoch of hyperdrive child runs.
 
-    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_crossval_metrics()` and
+    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_hyperdrive_metrics()` and
         :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
     :param train_metric: Name of the training metric to plot.
     :param val_metric: Name of the validation metric to plot.
     :param ax: `Axes` object onto which to plot.
     :param best_epochs: If provided, adds visual indicators of the best epoch for each run.
     :param ylabel: If provided, adds a label to the Y-axis.
     """
     for k in sorted(metrics_df.columns):
         train_values = metrics_df.loc[train_metric, k]
         val_values = metrics_df.loc[val_metric, k]
-        line, = ax.plot(train_values, **TRAIN_STYLE, label=f"Fold {k}")
-        color = line.get_color()
-        ax.plot(val_values, color=color, **VAL_STYLE)
+        if train_values is not None:
+            (line,) = ax.plot(train_values, **TRAIN_STYLE, label=f"Child {k}")
+            color = line.get_color()
+        if val_values is not None:
+            ax.plot(val_values, color=color, **VAL_STYLE)
         if best_epochs is not None:
             best_epoch = best_epochs[k]
-            ax.plot(best_epoch, train_values[best_epoch], color=color, zorder=1000, **BEST_TRAIN_MARKER_STYLE)
-            ax.plot(best_epoch, val_values[best_epoch], color=color, zorder=1000, **BEST_VAL_MARKER_STYLE)
-            ax.axvline(best_epoch, color=color, **BEST_EPOCH_LINE_STYLE)
+            if best_epoch is not None:
+                ax.plot(best_epoch, train_values[best_epoch], color=color, zorder=1000, **BEST_TRAIN_MARKER_STYLE)
+                ax.plot(best_epoch, val_values[best_epoch], color=color, zorder=1000, **BEST_VAL_MARKER_STYLE)
+                ax.axvline(best_epoch, color=color, **BEST_EPOCH_LINE_STYLE)
     ax.grid(color='0.9')
     ax.set_xlabel("Epoch")
     if ylabel:
         ax.set_ylabel(ylabel)
 
 
 def add_training_curves_legend(fig: Figure, include_best_epoch: bool = False) -> None:
-    """Add a legend to a training curves figure, indicating cross-validation indices and train/val.
+    """Add a legend to a training curves figure, indicating hyperdrive child indices and train/val.
 
     :param fig: `Figure` object onto which to add the legend.
     :param include_best_epoch: If `True`, adds legend items for the best epoch indicators from
-        :py:func:`plot_crossval_training_curves()`.
+        :py:func:`plot_hyperdrive_training_curves()`.
     """
-    legend_kwargs = dict(edgecolor='none', fontsize='small', borderpad=.2)
+    legend_kwargs = dict(edgecolor='none', fontsize='small', borderpad=0.2)
 
-    # Add primary legend for main lines (crossval folds)
+    # Add primary legend for main lines (hyperdrive runs)
     handles, labels = plt.gca().get_legend_handles_labels()
     by_label = dict(zip(labels, handles))
-    fig.legend(by_label.values(), by_label.keys(), **legend_kwargs, loc='lower center',
-               bbox_to_anchor=(0.5, -0.06), ncol=len(by_label))
+    fig.legend(
+        by_label.values(),
+        by_label.keys(),
+        **legend_kwargs,
+        loc='lower center',
+        bbox_to_anchor=(0.5, -0.06),
+        ncol=len(by_label),
+    )
 
     # Add secondary legend for line styles
-    legend_handles = [Line2D([], [], **TRAIN_STYLE, color='k', label="Training"),
-                      Line2D([], [], **VAL_STYLE, color='k', label="Validation")]
+    legend_handles = [
+        Line2D([], [], **TRAIN_STYLE, color='k', label="Training"),
+        Line2D([], [], **VAL_STYLE, color='k', label="Validation"),
+    ]
     if include_best_epoch:
-        legend_handles.append(Line2D([], [], **BEST_EPOCH_LINE_STYLE, **BEST_TRAIN_MARKER_STYLE,
-                                     color='k', label="Best epoch (train)"),)
-        legend_handles.append(Line2D([], [], **BEST_EPOCH_LINE_STYLE, **BEST_VAL_MARKER_STYLE,
-                                     color='k', label="Best epoch (val.)"),)
-    fig.legend(handles=legend_handles, **legend_kwargs, loc='lower center',
-               bbox_to_anchor=(0.5, -0.1), ncol=len(legend_handles))
+        legend_handles.append(
+            Line2D([], [], **BEST_EPOCH_LINE_STYLE, **BEST_TRAIN_MARKER_STYLE, color='k', label="Best epoch (train)"),
+        )
+        legend_handles.append(
+            Line2D([], [], **BEST_EPOCH_LINE_STYLE, **BEST_VAL_MARKER_STYLE, color='k', label="Best epoch (val.)"),
+        )
+    fig.legend(
+        handles=legend_handles,
+        **legend_kwargs,
+        loc='lower center',
+        bbox_to_anchor=(0.5, -0.1),
+        ncol=len(legend_handles),
+    )
 
 
-def plot_confusion_matrices(crossval_dfs: Dict[int, pd.DataFrame], class_names: List[str]) -> Figure:
+def plot_confusion_matrices(hyperdrive_dfs: Dict[int, pd.DataFrame], class_names: List[str]) -> Figure:
     """
     Plot normalized confusion matrices from HyperDrive child runs.
-    :param crossval_dfs: Dictionary of dataframes with cross-validation indices as keys,
-        as returned by :py:func:`collect_crossval_outputs()`.
+    :param hyperdrive_dfs: Dictionary of dataframes with hyperdrive indices as keys,
+        as returned by :py:func:`collect_hyperdrive_outputs()`.
     :param class_names: Names of classes.
     :return: The created `Figure` object.
     """
-    crossval_count = len(crossval_dfs)
-    fig, axs = plt.subplots(1, crossval_count, figsize=(crossval_count * 6, 5))
-    for k, tiles_df in crossval_dfs.items():
+    hyperdrive_count = len(hyperdrive_dfs)
+    fig, axs = plt.subplots(1, hyperdrive_count, figsize=(hyperdrive_count * 6, 5))
+    ax_index = 0
+    for k, tiles_df in hyperdrive_dfs.items():
         slides_groupby = tiles_df.groupby(ResultsKey.SLIDE_ID)
         tile_labels_true = slides_groupby[ResultsKey.TRUE_LABEL]
         # True slide label is guaranteed unique
         assert all(len(unique_slide_label) == 1 for unique_slide_label in tile_labels_true.unique())
         labels_true = tile_labels_true.first()
 
         tile_labels_pred = slides_groupby[ResultsKey.PRED_LABEL]
-        non_unique_slides = [slide_id for slide_id, unique_slide_label in tile_labels_pred.unique().items()
-                             if len(unique_slide_label) > 1]
+        non_unique_slides = [
+            slide_id
+            for slide_id, unique_slide_label in tile_labels_pred.unique().items()
+            if len(unique_slide_label) > 1
+        ]
         if non_unique_slides:
-            warnings.warn(f"Found {len(non_unique_slides)}/{len(slides_groupby)} non-unique slides in fold {k}: "
-                          f"{sorted(non_unique_slides)}")
+            warnings.warn(
+                f"Found {len(non_unique_slides)}/{len(slides_groupby)} non-unique slides in fold {k}: "
+                f"{sorted(non_unique_slides)}"
+            )
         labels_pred = tile_labels_pred.first()
 
         cf_matrix_n = confusion_matrix(y_true=labels_true, y_pred=labels_pred, normalize='true')
-        sns.heatmap(cf_matrix_n, annot=True, cmap='Blues', fmt=".2%", ax=axs[k],
-                    xticklabels=class_names, yticklabels=class_names)
-        axs[k].set_xlabel('Predicted')
-        axs[k].set_ylabel('True')
-        axs[k].set_title(f'Fold {k}')
+        sns.heatmap(
+            cf_matrix_n,
+            annot=True,
+            cmap='Blues',
+            fmt=".2%",
+            ax=axs[ax_index],
+            xticklabels=class_names,
+            yticklabels=class_names,
+        )
+        axs[ax_index].set_xlabel('Predicted')
+        axs[ax_index].set_ylabel('True')
+        axs[ax_index].set_title(f'Child {k}')
+        ax_index += 1
     return fig
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/download_utils.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/girder.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/girder.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,20 +27,26 @@
 from typing import Any, Dict, List, Optional, Sequence, Union
 
 import azureml
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 import matplotlib.pyplot as plt
-from girder_client import GirderClient
+from girder_client import GirderClient, HttpError
 from health_azure.logging import logging_to_stdout
 from health_azure.utils import get_aml_run_from_run_id
 
 from health_cpath.utils.naming import ResultsKey
-from health_cpath.utils.output_utils import AML_TEST_OUTPUTS_CSV
+from health_cpath.utils.output_utils import (
+    AML_OUTPUTS_DIR,
+    EXTRA_VAL_OUTPUTS_SUBDIR,
+    OUTPUTS_CSV_FILENAME,
+    TEST_OUTPUTS_SUBDIR,
+    VAL_OUTPUTS_SUBDIR,
+)
 
 
 TypeRectangleJSON = Dict[str, Union[str, float, Dict[str, str]]]
 TypePointJSON = Dict[str, Union[str, List[float], Dict[str, str]]]
 TypeAnnotationJSON = Dict[str, Union[str, List[Dict]]]
 
 # DSA coordinates are generally expressed using three dimensions
@@ -51,14 +57,15 @@
 class Color:
     """Container for RGBA color.
 
     All values are expected to be in :math:`[0, 255]`. Check the
     `documentation <https://github.com/girder/large_image/blob/master/girder_annotation/docs/annotations.rst#colors>`_
     for more information.
     """
+
     red: int
     green: int
     blue: int
     alpha: int
 
     def __post_init__(self) -> None:
         array = np.asarray(self)
@@ -79,26 +86,28 @@
 
 TRANSPARENT = Color(0, 0, 0, 0)
 
 
 @dataclass
 class Element:
     """Base class for annotations elements such as points or rectangles."""
+
     label: str
     fill_color: Color
     line_color: Color
 
     def as_json(self) -> Dict:
         """Return JSON representation suitable for the DSA."""
         raise NotImplementedError
 
 
 @dataclass
 class Coordinates:
     """Helper class to represent x and y coordinates."""
+
     x: float
     y: float
 
     def __post_init__(self) -> None:
         try:
             float(self.x)
             float(self.y)
@@ -112,14 +121,15 @@
 @dataclass
 class Rectangle(Element):
     """Container for rectangles in annotations.
 
     More information can be found in the
     `DSA documentation <https://github.com/girder/large_image/blob/master/girder_annotation/docs/annotations.rst#rectangle>`_.
     """  # noqa: E501
+
     left: float
     top: float
     right: float
     bottom: float
 
     def __post_init__(self) -> None:
         if self.left >= self.right:
@@ -156,14 +166,15 @@
 @dataclass
 class Point(Element):
     """Container for points in DSA annotations.
 
     More information can be found in the
     `DSA documentation <https://github.com/girder/large_image/blob/master/girder_annotation/docs/annotations.rst#point>`_.
     """  # noqa: E501
+
     center: Coordinates
 
     def __post_init__(self) -> None:
         if not isinstance(self.center, Coordinates):
             raise TypeError(f"Center must be an instance of Coordinates, not {type(self.center)}")
 
     def as_json(self) -> TypePointJSON:
@@ -178,15 +189,16 @@
 
 @dataclass
 class Annotation:
     """Container for DSA annotation.
 
     An example can be found in the
     `DSA documentation <https://github.com/girder/large_image/blob/master/girder_annotation/docs/annotations.rst#a-sample-annotation>`_.
-    """  # noqa: E501
+    """  # noqa: B950
+
     name: str
     elements: Sequence[Element]
     description: str = ""
 
     def __post_init__(self) -> None:
         if not self.name:
             # This is enforced by the JSON schema
@@ -206,14 +218,15 @@
     :param url: URL of a deployed instance of the `Digital Slide Archive <https://digitalslidearchive.github.io/>`_.
         For example: https://demo.kitware.com/histomicstk/. If not given, it must be defined in an environment
         variable ``DSA_URL``.
     :param api_key: Girder `API key <https://girder.readthedocs.io/en/latest/user-guide.html#api-keys>`_ to
         perform allowed operations. If not given, it must be defined in an environment
         variable ``DSA_API_KEY``.
     """
+
     URL_ENV_NAME = "DSA_URL"
     API_KEY_ENV_NAME = "DSA_API_KEY"
 
     def __init__(
         self,
         url: Optional[str] = None,
         api_key: Optional[str] = None,
@@ -259,31 +272,74 @@
         response = self.post(
             path="annotation",
             parameters={"itemId": item_id},
             json=annotation.as_json(),
         )
         return response
 
+    def make_api_call(self, api_path: str, parameters: Dict, result_field: str = "") -> Any:
+        """Issues a GET call to the DSA API on the given API path. If that raises a HttpError, a ValueError is raised
+        with more details.
+
+        :param api_path: The API path (for example, "resource/lookup")
+        :param parameters: A parameter dictionary with parameters for the API call.
+        :param result_field: If given, return only the specific item from the result dictionary.
+        :raises ValueError: If a HttpError is raised during the call.
+        :raises KeyError: If a specific field from the result was requested, but it was not found.
+        :return: The result of the API call, or only a given field thereof if `result_field` was provided.
+        """
+        try:
+            result = self.get(api_path, parameters=parameters)
+        except HttpError as ex:
+            raise ValueError(
+                f"API '{api_path}' does not exist or cannot be accessed. Please check "
+                f"the path and the access permissions of your API key. Exception: {ex}"
+            )
+        if result_field:
+            if result_field in result:
+                return result[result_field]
+            raise KeyError(f"Item '{result_field}' is not present in result: {result}")
+        return result
+
     def search_item(self, text: str, search_mode: str = "text") -> Item:
         """Search a file in the DSA collections and return its parent item.
 
         :param text: Text query.
         :param search_mode: Girder search mode. It ``'text'``, the full item ID will be matched.
             If ``'prefix'``, the file whose name starts with the value in ``text`` will be returned.
         :raises RuntimeError: If no items are found for the query or if more than one item is found.
         """
         parameters = dict(q=text, types="[\"item\"]", mode=search_mode)
-        result = self.get("/resource/search", parameters=parameters)
-        items_jsons = result["item"]
+        items_jsons = self.make_api_call("resource/search", parameters=parameters, result_field="item")
         if not items_jsons:
             raise RuntimeError(f"No items found for query \"{text}\"")
         elif len(items_jsons) > 1:
             raise RuntimeError(f"More than one item found for query \"{text}\":\n{items_jsons}")
         return Item(self, json=items_jsons[0])
 
+    def get_folder_id(self, folder_path: str) -> str:
+        """Retrieves the ID of a folder, when given a folder path.
+
+        :param folder_path: The path of the folder to retrieve (for example, "Coll1/folder2" for `folder2` in
+            collection `Coll1`)
+        :return: The ID of the folder in DSA.
+        """
+        parameters = dict(path=f"/collection/{folder_path.strip('/')}")
+        return self.make_api_call("resource/lookup", parameters=parameters, result_field="_id")
+
+    def get_items_in_folder(self, folder_id: str) -> List[Item]:
+        """Retrieves all items in the given folder.
+
+        :param folder_id: The ID of the folder to read from.
+        :return: A list of item JSON objects.
+        """
+        parameters = dict(type="folder", limit=5000)
+        result = self.make_api_call(f"resource/{folder_id}/items", parameters=parameters)
+        return [Item(self, json=item_json) for item_json in result]
+
 
 class Item:
     """Representation of an item in the Digital Slide Archive.
 
     :param dsa: Instance of :class:`DigitalSlideArchive`.
     :param id: ID of the item in the Digital Slide Archive.
     :param json: JSON representation of the Digital Slide Archive item.
@@ -302,14 +358,25 @@
 
         if id is None:
             id = json["_id"]  # type: ignore
         self.id = id
         self._json = json
 
     @property
+    def name(self) -> str:
+        """Gets the name of the item as stored in the "name" field in the JSON representation.
+        If the "name" field is not present, return an empty string.
+
+        :return: The "name" field of the JSON representation, or "" if that field is not present.
+        """
+        if self._json is None:
+            return ""
+        return self._json.get("name", "")
+
+    @property
     def url(self) -> str:
         return urljoin(self._dsa.url, f"/#item/{self.id}")
 
     def open(self) -> bool:
         return webbrowser.open(self.url)
 
     def add_annotation(self, annotation: Annotation) -> Dict:
@@ -330,46 +397,49 @@
     """
 
     def __init__(
         self,
         run_id: str,
         workspace_config_path: Optional[Path] = None,
         overwrite_csv: bool = False,
+        split: str = "test",
     ):
         logging.info("Getting run \"%s\"...", run_id)
         run = get_aml_run_from_run_id(run_id, workspace_config_path=workspace_config_path)
         experiment = run.experiment
         workspace = experiment.workspace
 
         self.run = run
         self.experiment = experiment
         self.workspace = workspace
         self.df = self.get_df(overwrite_csv)
         self.tile_size = None
+        self.split = split
 
     def get_df(self, overwrite_csv: bool) -> pd.DataFrame:
         """Download outputs CSV from Azure ML and read the data frame.
 
         The CSV is cached locally for future
 
         :param overwrite_csv: Force download of the output CSV even when it is found locally.
         """
-        csv_filename = AML_TEST_OUTPUTS_CSV
+        csv_filename = "/".join([AML_OUTPUTS_DIR, self.split, OUTPUTS_CSV_FILENAME])
         csv_stem = Path(csv_filename).stem
         csv_name = f"{csv_stem}-{self.workspace.name}-{self.run.id}.csv"
         cached_csv_path = Path(tempfile.gettempdir()) / csv_name
         if cached_csv_path.is_file() and not overwrite_csv:
-            logging.info("Found cached CSV file")
+            logging.info(f"Found cached CSV file {cached_csv_path}")
         else:
             logging.info("Downloading outputs CSV...")
             aml_exceptions = (
                 azureml.exceptions._azureml_exception.UserErrorException,
                 azureml._restclient.models.error_response.ErrorResponseException,
             )
             try:
+                logging.info(f"Downloading file {csv_filename}")
                 self.run.download_file(csv_filename, cached_csv_path)
             except aml_exceptions as e:
                 raise FileNotFoundError("Error downloading outputs file from run") from e
         logging.info("Reading CSV file: %s ...", cached_csv_path)
         return self._read_csv(cached_csv_path)
 
     def get_annotation_from_slide_data_frame(
@@ -438,23 +508,25 @@
     def upload(
         self,
         dsa: DigitalSlideArchive,
         dry_run: bool = False,
         max_slides: Optional[int] = None,
         id_filter: Optional[str] = "",
         search_mode: str = "full",
+        folder_path: str = "",
         **annotation_kwargs: Any,
     ) -> List[Dict]:
         """Create annotations from a data frame and upload them to DSA.
 
         :param dsa: Instance of :class:`DigitalSlideArchive` to which results will be uploaded.
         :param dry_run: Create annotations and show outputs, without uploading any data.
         :param max_slides: Maximum number of slides to upload, useful for debugging.
         :param id_filter: Filter to only process slides matching this string, according to ``search_mode``.
         :param search_mode: See :meth:`DigitalSlideArchive.search_item`.
+        :param folder_path: The path of the folder in DSA where results should be uploaded to.
         :param annotation_kwargs: Additional kwargs to :meth:`get_annotation_from_slide_data_frame`.
         """
         unique_slide_ids = sorted(self.df[ResultsKey.SLIDE_ID].unique())
 
         num_slides = len(unique_slide_ids)
         logging.info("Found outputs for %s slides", num_slides)
         if max_slides is not None:
@@ -462,22 +534,39 @@
             percentage = 100 * max_slides / num_slides
             logging.info("Using %s/%s slides (%s %% of total)", max_slides, num_slides, f"{percentage:.1f}")
             unique_slide_ids = unique_slide_ids[:max_slides]
 
         # I think "full" is more descriptive than "text" for our API
         search_mode = "text" if search_mode == "full" else search_mode
         progress = tqdm(unique_slide_ids)
+        annotation_name = f"{self.run.id} ({self.run.display_name})"
         responses = []
+        if folder_path:
+            folder_id = dsa.get_folder_id(folder_path)
+            items = dsa.get_items_in_folder(folder_id)
+            print(f"Found a total of {len(items)} items in folder {folder_path}")
+        else:
+            items = []
         for slide_id in progress:
             progress.set_description(slide_id)
             if id_filter not in slide_id:
                 continue
-            item = dsa.search_item(slide_id, search_mode=search_mode)
+            if folder_path:
+                matching_items = [item for item in items if slide_id in item.name]
+                if not matching_items:
+                    print(f"No items in DSA for slide ID {slide_id}")
+                    continue
+                elif len(matching_items) > 1:
+                    print(f"Multiple items in DSA for slide ID {slide_id}. Skipping this slide.")
+                    continue
+                item = matching_items[0]
+            else:
+                item = dsa.search_item(slide_id, search_mode=search_mode)
+
             tqdm.write(f"Processing slide {slide_id} - {item.url}")
-            annotation_name = self.run.id
             annotation = self.get_slide_annotation_from_df(
                 self.df,
                 slide_id,
                 annotation_name,
                 **annotation_kwargs,
             )
             if not dry_run:
@@ -533,50 +622,68 @@
     )
     parser.add_argument(
         "--login-only",
         action="store_true",
         help="Just log into the DSA and exit. Useful to ensure connection to the DSA from current host",
     )
     parser.add_argument(
-        "--rescale",
-        action="store_true",
-        help="Rescale attention values between 0 and 1 to maximize heatmaps contrast",
+        "--no-rescale",
+        action="store_false",
+        default=True,
+        help="Do not rescale attention values. By default, attention values are scaled such that the range "
+        "between min and max fills the colormap.",
     )
     parser.add_argument(
         "--colormap",
         type=str,
         choices=plt.colormaps(),
-        default="Greens",
+        default="Spectral_r",
         help="Matplotlib colormap used for the heatmaps",
     )
     parser.add_argument(
+        "--folder",
+        type=str,
+        default="",
+        help="The folder in DSA where uploads should go to. Use this if there are multiple slides with the same ID"
+        "in DSA. The folder name must contain the collection, like `Collection1/foo`",
+    )
+    parser.add_argument(
+        "--split",
+        type=str,
+        choices=[TEST_OUTPUTS_SUBDIR, EXTRA_VAL_OUTPUTS_SUBDIR, VAL_OUTPUTS_SUBDIR],
+        default=TEST_OUTPUTS_SUBDIR,
+        help="The results subfolder in the AzureML run where the results are downloaded from. Default: 'test'",
+    )
+    parser.add_argument(
         "--search-mode",
         type=str,
         choices=("full", "prefix"),
         default="full",
         help=(
             "If \"full\", the slide ID must match the DSA file name with or without extension."
             " If \"prefix\", all files whose name starts with the slide ID will be matched"
-        )
+        ),
     )
     args = parser.parse_args()
 
     logging_to_stdout()
     dsa = DigitalSlideArchive(args.dsa_url, args.dsa_key)
     if args.login_only:
         sys.exit(0)
     if args.run_id is None:
         raise ValueError("Please specify an Azure Machine Learning run ID")
     outputs = RunOutputs(
         run_id=args.run_id,
         workspace_config_path=args.workspace_config,
         overwrite_csv=args.overwrite_csv,
+        split=args.split,
     )
     outputs.upload(
         dsa,
         dry_run=args.dry_run,
         max_slides=args.max_slides,
         id_filter=args.id_filter,
         search_mode=args.search_mode,
         colormap_name=args.colormap,
-        rescale=args.rescale,
+        rescale=args.no_rescale,
+        folder_path=args.folder,
     )
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/layer_utils.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/layer_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from torchvision.transforms import Normalize
 
 
 def get_imagenet_preprocessing() -> nn.Module:
     return Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
 
 
-def setup_feature_extractor(pretrained_model: nn.Module,
-                            input_dim: Tuple[int, ...]) -> Tuple[nn.Module, int]:
+def setup_feature_extractor(pretrained_model: nn.Module, input_dim: Tuple[int, ...]) -> Tuple[nn.Module, int]:
     try:
         # Attempt to auto-detect final classification layer:
         num_features: int = pretrained_model.fc.in_features  # type: ignore
         pretrained_model.fc = nn.Flatten()
         feature_extractor = pretrained_model
     except AttributeError:
         # Otherwise fallback to sequence of child modules:
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/naming.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/naming.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,49 +46,65 @@
 
 class ResultsKey(str, Enum):
     SLIDE_ID = 'slide_id'
     TILE_ID = 'tile_id'
     FEATURES = 'features'
     IMAGE_PATH = 'image_path'
     LOSS = 'loss'
+    LOSS_PER_SAMPLE = 'loss_per_sample'
     PROB = 'prob'
     CLASS_PROBS = 'prob_class'
     PRED_LABEL = 'pred_label'
     TRUE_LABEL = 'true_label'
     BAG_ATTN = 'bag_attn'
     TILE_LEFT = 'left'
     TILE_TOP = 'top'
     TILE_RIGHT = 'right'
     TILE_BOTTOM = 'bottom'
+    ENTROPY = 'entropy'
 
 
 class MetricsKey(str, Enum):
     ACC = 'accuracy'
     ACC_MACRO = 'macro_accuracy'
     ACC_WEIGHTED = 'weighted_accuracy'
     CONF_MATRIX = 'confusion_matrix'
+    CONF_MATRIX_N = 'confusion_matrix_normalized'
     AUROC = 'auroc'
     PRECISION = 'precision'
     RECALL = 'recall'
     F1 = 'f1score'
     COHENKAPPA = 'cohenkappa'
+    AVERAGE_PRECISION = 'average_precision'
+    SPECIFICITY = 'specificity'
 
 
 class ModelKey(str, Enum):
     TRAIN = 'train'
     VAL = 'val'
     TEST = 'test'
 
 
 class AMLMetricsJsonKey(str, Enum):
     HYPERPARAMS = 'hyperparams'
     NAME = 'name'
     VALUE = 'value'
     N_CLASSES = 'n_classes'
     CLASS_NAMES = 'class_names'
+    MAX_EPOCHS = 'max_epochs'
 
 
 class PlotOption(Enum):
     TOP_BOTTOM_TILES = "top_bottom_tiles"
-    SLIDE_THUMBNAIL_HEATMAP = "slide_thumbnail_heatmap"
+    SLIDE_THUMBNAIL = "slide_thumbnail"
+    ATTENTION_HEATMAP = "attention_heatmap"
+    ATTENTION_HISTOGRAM = "attention_histogram"
     CONFUSION_MATRIX = "confusion_matrix"
     HISTOGRAM = "histogram"
+    PR_CURVE = "pr_curve"
+    ROC_CURVE = "roc_curve"
+
+
+class DeepMILSubmodules(str, Enum):
+    ENCODER = 'encoder'
+    POOLING = 'aggregation_fn'
+    CLASSIFIER = 'classifier_fn'
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/output_utils.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/output_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 #  -------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  -------------------------------------------------------------------------------------------
 
+from copy import deepcopy
 import shutil
 from itertools import chain
 from pathlib import Path
 from typing import Any, Collection, Dict, List, Mapping, Optional, Sequence, Tuple
 
 import numpy as np
 import pandas as pd
 import torch
 import logging
 
 from ruamel.yaml import YAML
-from torchmetrics import Accuracy
 from torchmetrics.metric import Metric
 
 from health_azure.utils import replace_directory
 from health_cpath.datasets.base_dataset import SlidesDataset
+from health_cpath.preprocessing.loading import LoadingParams
 from health_cpath.utils.plots_utils import DeepMILPlotsHandler, TilesSelector
 from health_cpath.utils.naming import MetricsKey, ModelKey, PlotOption, ResultsKey
 
 OUTPUTS_CSV_FILENAME = "test_output.csv"
 VAL_OUTPUTS_SUBDIR = "val"
 PREV_VAL_OUTPUTS_SUBDIR = "val_old"
 TEST_OUTPUTS_SUBDIR = "test"
+EXTRA_VAL_OUTPUTS_SUBDIR = "extra_val"
+EXTRA_PREFIX = "extra_"
 
 AML_OUTPUTS_DIR = "outputs"
 AML_LEGACY_TEST_OUTPUTS_CSV = "/".join([AML_OUTPUTS_DIR, OUTPUTS_CSV_FILENAME])
 AML_VAL_OUTPUTS_CSV = "/".join([AML_OUTPUTS_DIR, VAL_OUTPUTS_SUBDIR, OUTPUTS_CSV_FILENAME])
 AML_TEST_OUTPUTS_CSV = "/".join([AML_OUTPUTS_DIR, TEST_OUTPUTS_SUBDIR, OUTPUTS_CSV_FILENAME])
 
 BatchResultsType = Dict[ResultsKey, Any]
@@ -44,26 +47,35 @@
     :param n_classes: Number of classes. If `1` (binary), expects `len(class_names) == 2`.
     :return: Validated class names tuple with length `2` for binary classes (`n_classes == 1`), otherwise `n_classes`.
     """
     effective_n_classes = n_classes if n_classes > 1 else 2
     if class_names is None:
         class_names = [str(i) for i in range(effective_n_classes)]
     if len(class_names) != effective_n_classes:
-        raise ValueError(f"Mismatch in number of class names ({class_names}) and number"
-                         f"of classes ({effective_n_classes})")
+        raise ValueError(
+            f"Mismatch in number of class names ({class_names}) and number" f"of classes ({effective_n_classes})"
+        )
     return tuple(class_names)
 
 
 def validate_slide_datasets_for_plot_options(
     plot_options: Collection[PlotOption], slides_dataset: Optional[SlidesDataset]
 ) -> None:
-    if PlotOption.SLIDE_THUMBNAIL_HEATMAP in plot_options and not slides_dataset:
-        raise ValueError("You can not plot slide thumbnails and heatmaps without setting a slides_dataset. "
-                         "Please remove `PlotOption.SLIDE_THUMBNAIL_HEATMAP` from your plot options or provide "
-                         "a slide dataset.")
+    """Validate that the specified plot options are compatible with the specified slides dataset.
+
+    :param plot_options: Plot options to validate.
+    :param slides_dataset: Slides dataset to validate against.
+    """
+
+    def _validate_slide_plot_option(plot_option: PlotOption) -> None:
+        if plot_option in plot_options and not slides_dataset:
+            raise ValueError(f"Plot option {plot_option} requires a slides dataset")
+
+    _validate_slide_plot_option(PlotOption.SLIDE_THUMBNAIL)
+    _validate_slide_plot_option(PlotOption.ATTENTION_HEATMAP)
 
 
 def normalize_dict_for_df(dict_old: Dict[ResultsKey, Any]) -> Dict[str, Any]:
     # slide-level dictionaries are processed by making value dimensions uniform and converting to numpy arrays.
     # these steps are required to convert the dictionary to pandas dataframe.
     dict_new: Dict[str, Any] = dict()
     bag_size = len(dict_old[ResultsKey.SLIDE_ID])
@@ -109,28 +121,28 @@
     results: ResultsType = {}
     for key in epoch_results[0].keys():
         results[key] = []
         for batch_results in epoch_results:
             batch_elements = batch_results[key]
             if key == ResultsKey.LOSS:
                 batch_elements = [batch_elements]
-            batch_elements = [elem.cpu() if isinstance(elem, torch.Tensor) else elem
-                              for elem in batch_elements]
+            batch_elements = [elem.cpu() if isinstance(elem, torch.Tensor) else elem for elem in batch_elements]
             results[key].extend(batch_elements)
     return results
 
 
 def save_outputs_csv(results: ResultsType, outputs_dir: Path) -> None:
     logging.info("Saving outputs ...")
     # collate at slide level
     list_slide_dicts: List[Dict[ResultsKey, Any]] = []
     # any column can be used here, the assumption is that the first dimension is the N of slides
     for slide_idx in range(len(results[ResultsKey.SLIDE_ID])):
-        slide_dict = {key: results[key][slide_idx] for key in results
-                      if key not in [ResultsKey.FEATURES, ResultsKey.LOSS]}
+        slide_dict = {
+            key: results[key][slide_idx] for key in results if key not in [ResultsKey.FEATURES, ResultsKey.LOSS]
+        }
         list_slide_dicts.append(slide_dict)
 
     assert outputs_dir.is_dir(), f"No such dir: {outputs_dir}"
     logging.info(f"Metrics results will be output to {outputs_dir}")
     csv_filename = outputs_dir / OUTPUTS_CSV_FILENAME
 
     # Collect the list of dictionaries in a list of pandas dataframe and save
@@ -177,50 +189,58 @@
         :raises ValueError: If the primary metric name does not match the one saved on disk.
         """
         if self.best_metric_file_path.exists():
             contents = YAML().load(self.best_metric_file_path)
             self._best_metric_epoch = contents[self._BEST_EPOCH_KEY]
             self._best_metric_value = contents[self._BEST_VALUE_KEY]
             if contents[self._PRIMARY_METRIC_KEY] != self.primary_val_metric:
-                raise ValueError(f"Expected primary metric '{self.primary_val_metric}', but found "
-                                 f"'{contents[self._PRIMARY_METRIC_KEY]}' in {self.best_metric_file_path}")
+                raise ValueError(
+                    f"Expected primary metric '{self.primary_val_metric}', but found "
+                    f"'{contents[self._PRIMARY_METRIC_KEY]}' in {self.best_metric_file_path}"
+                )
         else:
             self._best_metric_epoch = 0
             self._best_metric_value = float('-inf') if self.maximise else float('inf')
 
     def _save_best_metric(self) -> None:
         """Save best metric epoch, value, and name to disk, to allow recovery (e.g. in case of pre-emption)."""
-        contents = {self._BEST_EPOCH_KEY: self._best_metric_epoch,
-                    self._BEST_VALUE_KEY: self._best_metric_value,
-                    self._PRIMARY_METRIC_KEY: self.primary_val_metric.value}
+        contents = {
+            self._BEST_EPOCH_KEY: self._best_metric_epoch,
+            self._BEST_VALUE_KEY: self._best_metric_value,
+            self._PRIMARY_METRIC_KEY: self.primary_val_metric.value,
+        }
         YAML().dump(contents, self.best_metric_file_path)
 
-    def should_save_validation_outputs(self, metrics_dict: Mapping[MetricsKey, Metric], epoch: int,
-                                       is_global_rank_zero: bool = True) -> bool:
+    def should_save_validation_outputs(
+        self,
+        metrics_dict: Mapping[MetricsKey, Metric],
+        epoch: int,
+        is_global_rank_zero: bool = True,
+        on_extra_val: bool = False,
+    ) -> bool:
         """Determine whether validation outputs should be saved given the current epoch's metrics.
 
         :param metrics_dict: Current epoch's metrics dictionary from
             :py:class:`~health_cpath.models.deepmil.DeepMILModule`.
         :param epoch: Current epoch number.
         :param is_global_rank_zero: Whether this is the global rank-0 process in distributed scenarios.
             Set to `True` (default) if running a single process.
+        :param on_extra_val: Whether this is an extra validation epoch (e.g. after training).
         :return: Whether this is the best validation epoch so far.
         """
+        if on_extra_val:
+            return False
         metric = metrics_dict[self.primary_val_metric]
         # If the metric hasn't been updated we don't want to save it
         if not metric._update_called:
             logging.warning("Encountered metric that hasn't been updated. Not saving.")
             return False
         # The metric needs to be computed on all ranks to allow synchronisation
         metric_value = float(metric.compute())
 
-        # It seems to be necessary to reset the Accuracy metric after computing, else some processes get stuck here
-        if isinstance(metric, Accuracy):
-            metric.reset()
-
         # Validation outputs and best metric should be saved only by the global rank-0 process
         if not is_global_rank_zero:
             return False
 
         if self.maximise:
             is_best = metric_value > self._best_metric_value
         else:
@@ -242,78 +262,103 @@
         # This is implemented as a method in case we want to add custom logic in the future
         return is_global_rank_zero
 
 
 class DeepMILOutputsHandler:
     """Class that manages writing validation and test outputs for DeepMIL models."""
 
-    def __init__(self, outputs_root: Path, n_classes: int, tile_size: int, level: int,
-                 class_names: Optional[Sequence[str]], primary_val_metric: MetricsKey,
-                 maximise: bool, val_plot_options: Collection[PlotOption],
-                 test_plot_options: Collection[PlotOption]) -> None:
+    def __init__(
+        self,
+        outputs_root: Path,
+        n_classes: int,
+        tile_size: int,
+        loading_params: LoadingParams,
+        class_names: Optional[Sequence[str]],
+        primary_val_metric: MetricsKey,
+        maximise: bool,
+        val_plot_options: Collection[PlotOption],
+        test_plot_options: Collection[PlotOption],
+        save_intermediate_outputs: bool = True,
+        stratify_plots_by: Optional[str] = None,
+    ) -> None:
         """
         :param outputs_root: Root directory where to save all produced outputs.
         :param n_classes: Number of MIL classes (set `n_classes=1` for binary).
         :param tile_size: The size of each tile.
-        :param level: The downsampling level (e.g. 0, 1, 2) of the tiles if available (default=1).
+        :param loading_params: Parameters for loading WSI to create plots. This paramter is passed to PlotsHandler.
         :param class_names: List of class names. For binary (`n_classes == 1`), expects `len(class_names) == 2`.
             If `None`, will return `('0', '1', ...)`.
         :param primary_val_metric: Name of the validation metric to track for saving best epoch outputs.
         :param maximise: Whether higher is better for `primary_val_metric`.
         :param val_plot_options: The desired plot options for validation time.
         :param test_plot_options: The desired plot options for test time.
+        :param save_intermediate_outputs: Whether to save intermediate outputs (e.g. after each epoch).
+        :param stratify_plots_by: Name of metadata field to stratify output plots (PR curve, ROC curve).
+        `None` by default (no stratification).
         """
         self.outputs_root = outputs_root
         self.n_classes = n_classes
-        self.tile_size = tile_size
-        self.level = level
         self.class_names = validate_class_names(class_names, self.n_classes)
-
-        self.outputs_policy = OutputsPolicy(outputs_root=outputs_root,
-                                            primary_val_metric=primary_val_metric,
-                                            maximise=maximise)
-
+        self.outputs_policy = OutputsPolicy(
+            outputs_root=outputs_root, primary_val_metric=primary_val_metric, maximise=maximise
+        )
+        self.save_intermediate_outputs = save_intermediate_outputs
         self.tiles_selector: Optional[TilesSelector] = None
-
         self.val_plots_handler = DeepMILPlotsHandler(
             plot_options=val_plot_options,
-            level=self.level,
-            tile_size=self.tile_size,
-            class_names=self.class_names
+            tile_size=tile_size,
+            class_names=self.class_names,
+            stage=ModelKey.VAL,
+            loading_params=deepcopy(loading_params),
+            stratify_plots_by=stratify_plots_by,
         )
         self.test_plots_handler = DeepMILPlotsHandler(
             plot_options=test_plot_options,
-            level=self.level,
-            tile_size=self.tile_size,
-            class_names=self.class_names
+            tile_size=tile_size,
+            class_names=self.class_names,
+            stage=ModelKey.TEST,
+            loading_params=deepcopy(loading_params),
+            stratify_plots_by=stratify_plots_by,
         )
 
     @property
     def validation_outputs_dir(self) -> Path:
         return self.outputs_root / VAL_OUTPUTS_SUBDIR
 
     @property
+    def extra_validation_outputs_dir(self) -> Path:
+        return self.outputs_root / EXTRA_VAL_OUTPUTS_SUBDIR
+
+    @property
     def previous_validation_outputs_dir(self) -> Path:
         return self.validation_outputs_dir.with_name(PREV_VAL_OUTPUTS_SUBDIR)
 
     @property
     def test_outputs_dir(self) -> Path:
         return self.outputs_root / TEST_OUTPUTS_SUBDIR
 
     def set_slides_dataset_for_plots_handlers(self, slides_dataset: Optional[SlidesDataset]) -> None:
         validate_slide_datasets_for_plot_options(self.test_plots_handler.plot_options, slides_dataset)
         validate_slide_datasets_for_plot_options(self.val_plots_handler.plot_options, slides_dataset)
         self.test_plots_handler.slides_dataset = slides_dataset
         self.val_plots_handler.slides_dataset = slides_dataset
 
+    def set_extra_slides_dataset_for_plots_handlers(self, extra_slides_dataset: Optional[SlidesDataset]) -> None:
+        self.test_plots_handler.extra_slides_dataset = extra_slides_dataset
+        self.val_plots_handler.extra_slides_dataset = extra_slides_dataset
+
+    def should_gather_tiles(self, plots_handler: DeepMILPlotsHandler) -> bool:
+        return PlotOption.TOP_BOTTOM_TILES in plots_handler.plot_options and self.tiles_selector is not None
+
     def _save_outputs(self, epoch_results: EpochResultsType, outputs_dir: Path, stage: ModelKey = ModelKey.VAL) -> None:
         """Trigger the rendering and saving of DeepMIL outputs and figures.
 
         :param epoch_results: Aggregated results from all epoch batches.
         :param outputs_dir: Specific directory into which outputs should be saved (different for validation and test).
+        :param stage: The stage of the model (e.g. `ModelKey.VAL` or `ModelKey.TEST`).
         """
         # outputs object consists of a list of dictionaries (of metadata and results, including encoded features)
         # It can be indexed as outputs[batch_idx][batch_key][bag_idx][tile_idx]
         # example of batch_key ResultsKey.SLIDE_ID_COL
         # for batch keys that contains multiple values for slides e.g. ResultsKey.BAG_ATTN_COL
         # outputs[batch_idx][batch_key][bag_idx][tile_idx]
         # contains the tile value
@@ -321,58 +366,69 @@
         results = collate_results_on_cpu(epoch_results)
         outputs_dir.mkdir(exist_ok=True, parents=True)
         save_outputs_csv(results, outputs_dir)
 
         plots_handler = self.val_plots_handler if stage == ModelKey.VAL else self.test_plots_handler
         plots_handler.save_plots(outputs_dir, self.tiles_selector, results)
 
-    def save_validation_outputs(self, epoch_results: EpochResultsType, metrics_dict: Mapping[MetricsKey, Metric],
-                                epoch: int, is_global_rank_zero: bool = True, run_extra_val_epoch: bool = False
-                                ) -> None:
+    def save_validation_outputs(
+        self,
+        epoch_results: EpochResultsType,
+        metrics_dict: Mapping[MetricsKey, Metric],
+        epoch: int,
+        is_global_rank_zero: bool = True,
+        on_extra_val: bool = False,
+    ) -> None:
         """Render and save validation epoch outputs, according to the configured :py:class:`OutputsPolicy`.
 
         :param epoch_results: Aggregated results from all epoch batches, as passed to :py:meth:`validation_epoch_end()`.
         :param metrics_dict: Current epoch's validation metrics dictionary from
             :py:class:`~health_cpath.models.deepmil.DeepMILModule`.
         :param is_global_rank_zero: Whether this is the global rank-0 process in distributed scenarios.
             Set to `True` (default) if running a single process.
         :param epoch: Current epoch number.
+        :param on_extra_val: Whether this is an extra validation epoch (e.g. after training).
         """
-        # All DDP processes must reach this point to allow synchronising epoch results
-        gathered_epoch_results = gather_results(epoch_results)
-        if PlotOption.TOP_BOTTOM_TILES in self.val_plots_handler.plot_options and self.tiles_selector:
-            self.tiles_selector.gather_selected_tiles_across_devices()
+        if self.save_intermediate_outputs or on_extra_val:
+            epoch_results = gather_results(epoch_results)
+
+            if self.should_gather_tiles(self.val_plots_handler):
+                self.tiles_selector.gather_selected_tiles_across_devices()  # type: ignore
 
         # Only global rank-0 process should actually render and save the outputs
-        # We also want to save the plots of the extra validation epoch
-        if (
-            self.outputs_policy.should_save_validation_outputs(metrics_dict, epoch, is_global_rank_zero)
-            or (run_extra_val_epoch and is_global_rank_zero)
+        if self.save_intermediate_outputs and self.outputs_policy.should_save_validation_outputs(
+            metrics_dict, epoch, is_global_rank_zero, on_extra_val
         ):
             # First move existing outputs to a temporary directory, to avoid mixing
             # outputs of different epochs in case writing fails halfway through
             if self.validation_outputs_dir.exists():
-                replace_directory(source=self.validation_outputs_dir,
-                                  target=self.previous_validation_outputs_dir)
+                replace_directory(source=self.validation_outputs_dir, target=self.previous_validation_outputs_dir)
 
-            self._save_outputs(gathered_epoch_results, self.validation_outputs_dir, ModelKey.VAL)
+            self._save_outputs(epoch_results, self.validation_outputs_dir, ModelKey.VAL)
 
             # Writing completed successfully; delete temporary back-up
             if self.previous_validation_outputs_dir.exists():
                 shutil.rmtree(self.previous_validation_outputs_dir, ignore_errors=True)
+        # We also want to save the plots of the extra validation epoch
+        elif on_extra_val and is_global_rank_zero:
+            self._save_outputs(epoch_results, self.extra_validation_outputs_dir, ModelKey.VAL)
+
+        # Reset the top and bottom slides heaps
+        if self.should_gather_tiles(self.val_plots_handler):
+            self.tiles_selector._clear_cached_slides_heaps()  # type: ignore
 
     def save_test_outputs(self, epoch_results: EpochResultsType, is_global_rank_zero: bool = True) -> None:
         """Render and save test epoch outputs.
 
         :param epoch_results: Aggregated results from all epoch batches, as passed to :py:meth:`test_epoch_end()`.
         :param metrics_dict: Test metrics dictionary from :py:class:`~health_cpath.models.deepmil.DeepMILModule`.
         :param is_global_rank_zero: Whether this is the global rank-0 process in distributed scenarios.
             Set to `True` (default) if running a single process.
         """
         # All DDP processes must reach this point to allow synchronising epoch results
         gathered_epoch_results = gather_results(epoch_results)
-        if PlotOption.TOP_BOTTOM_TILES in self.test_plots_handler.plot_options and self.tiles_selector:
-            self.tiles_selector.gather_selected_tiles_across_devices()
+        if self.should_gather_tiles(self.test_plots_handler):
+            self.tiles_selector.gather_selected_tiles_across_devices()  # type: ignore
 
         # Only global rank-0 process should actually render and save the outputs-
         if self.outputs_policy.should_save_test_outputs(is_global_rank_zero):
             self._save_outputs(gathered_epoch_results, self.test_outputs_dir, ModelKey.TEST)
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/report_utils.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/report_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 #  -------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  -------------------------------------------------------------------------------------------
 
 from pathlib import Path
-from typing import Dict, List, Sequence, Tuple
+from typing import Any, Dict, List, Sequence, Tuple
 
 import dateutil.parser
 import numpy as np
 import pandas as pd
 from azureml.core import Experiment, Run, Workspace
 
 from health_ml.utils.common_utils import df_to_json
-from health_azure.utils import (aggregate_hyperdrive_metrics, download_file_if_necessary, get_aml_run_from_run_id,
-                                get_tags_from_hyperdrive_run)
-from health_cpath.utils.output_utils import (AML_LEGACY_TEST_OUTPUTS_CSV, AML_TEST_OUTPUTS_CSV,
-                                             AML_VAL_OUTPUTS_CSV, validate_class_names)
+from health_azure.utils import (
+    aggregate_hyperdrive_metrics,
+    download_file_if_necessary,
+    get_aml_run_from_run_id,
+    get_tags_from_hyperdrive_run,
+)
+from health_cpath.utils.output_utils import (
+    AML_LEGACY_TEST_OUTPUTS_CSV,
+    AML_TEST_OUTPUTS_CSV,
+    AML_VAL_OUTPUTS_CSV,
+    validate_class_names,
+)
 from health_cpath.utils.naming import AMLMetricsJsonKey
 
 
 def run_has_val_and_test_outputs(run: Run) -> bool:
     """Checks whether the given run has both validation and test outputs files.
 
     :param parent_run: The run whose outputs to check.
@@ -30,172 +38,218 @@
     available_files: List[str] = run.get_file_names()
 
     if AML_VAL_OUTPUTS_CSV in available_files and AML_TEST_OUTPUTS_CSV in available_files:
         return True
     elif AML_LEGACY_TEST_OUTPUTS_CSV in available_files:
         return False
     else:
-        raise ValueError(f"Run {run.display_name} ({run.id}) does not have the expected files "
-                         f"({AML_LEGACY_TEST_OUTPUTS_CSV} or both {AML_VAL_OUTPUTS_CSV} and "
-                         f"{AML_TEST_OUTPUTS_CSV}): {available_files}")
+        raise ValueError(
+            f"Run {run.display_name} ({run.id}) does not have the expected files "
+            f"({AML_LEGACY_TEST_OUTPUTS_CSV} or both {AML_VAL_OUTPUTS_CSV} and "
+            f"{AML_TEST_OUTPUTS_CSV}): {available_files}"
+        )
 
 
-def crossval_runs_have_val_and_test_outputs(parent_run: Run) -> bool:
-    """Checks whether all child cross-validation runs have both validation and test outputs files.
+def child_runs_have_val_and_test_outputs(parent_run: Run) -> bool:
+    """Checks whether all child hyperdrive runs have both validation and test outputs files.
 
     :param parent_run: The parent Hyperdrive run.
     :raises ValueError: If any of the child runs does not have the expected output files, or if
         some of the child runs have both outputs and some have only test outputs.
     :return: `True` if all children have validation and test outputs, `False` if all children are
         legacy runs with only test outputs.
     """
     have_val_and_test_outputs = [run_has_val_and_test_outputs(child_run) for child_run in parent_run.get_children()]
     if all(have_val_and_test_outputs):
         return True
     elif not any(have_val_and_test_outputs):
         return False
     else:
-        raise ValueError(f"Parent run {parent_run.display_name} ({parent_run.id}) has mixed children with legacy "
-                         "test-only outputs and with both validation and test outputs")
+        raise ValueError(
+            f"Parent run {parent_run.display_name} ({parent_run.id}) has mixed children with legacy "
+            "test-only outputs and with both validation and test outputs"
+        )
 
 
-def collect_crossval_outputs(parent_run_id: str, download_dir: Path, aml_workspace: Workspace,
-                             crossval_arg_name: str = "crossval_index",
-                             output_filename: str = "test_output.csv",
-                             overwrite: bool = False) -> Dict[int, pd.DataFrame]:
-    """Fetch output CSV files from cross-validation runs as dataframes.
+def collect_hyperdrive_outputs(
+    parent_run_id: str,
+    download_dir: Path,
+    aml_workspace: Workspace,
+    hyperdrive_arg_name: str = "crossval_index",
+    output_filename: str = "test_output.csv",
+    overwrite: bool = False,
+) -> Dict[int, pd.DataFrame]:
+    """Fetch output CSV files from Hyperdrive child runs as dataframes.
 
     Will only download the CSV files if they do not already exist locally.
 
     :param parent_run_id: Azure ML run ID for the parent Hyperdrive run.
     :param download_dir: Base directory where to download the CSV files. A new sub-directory will
-        be created for each child run (e.g. `<download_dir>/<crossval index>/*.csv`).
+        be created for each child run (e.g. `<download_dir>/<hyperdrive_arg_name>/*.csv`).
     :param aml_workspace: Azure ML workspace in which the runs were executed.
-    :param crossval_arg_name: Name of the Hyperdrive argument used for indexing the child runs.
+    :param hyperdrive_arg_name: Name of the Hyperdrive argument used for indexing the child runs.
     :param output_filename: Filename of the output CSVs to download.
     :param overwrite: Whether to force the download even if each file already exists locally.
-    :return: A dictionary of dataframes with the sorted cross-validation indices as keys.
+    :return: A dictionary of dataframes with the sorted hyperdrive_arg_name indices as keys.
     """
     parent_run = get_aml_run_from_run_id(parent_run_id, aml_workspace)
 
     all_outputs_dfs = {}
     for child_run in parent_run.get_children():
-        child_run_index = get_tags_from_hyperdrive_run(child_run, crossval_arg_name)
+        child_run_index = get_tags_from_hyperdrive_run(child_run, hyperdrive_arg_name)
         if child_run_index is None:
-            raise ValueError(f"Child run expected to have the tag '{crossval_arg_name}'")
+            raise ValueError(f"Child run expected to have the tag '{hyperdrive_arg_name}'")
         child_dir = download_dir / str(child_run_index)
         try:
-            child_csv = download_file_if_necessary(child_run, output_filename, child_dir / output_filename,
-                                                   overwrite=overwrite)
+            child_csv = download_file_if_necessary(
+                child_run, output_filename, child_dir / output_filename, overwrite=overwrite
+            )
             all_outputs_dfs[child_run_index] = pd.read_csv(child_csv)
         except Exception as e:
             print(f"Failed to download {output_filename} for run {child_run.id}: {e}")
     return dict(sorted(all_outputs_dfs.items()))  # type: ignore
 
 
-def collect_crossval_metrics(parent_run_id: str, download_dir: Path, aml_workspace: Workspace,
-                             crossval_arg_name: str = "crossval_index",
-                             overwrite: bool = False) -> pd.DataFrame:
-    """Fetch metrics logged to Azure ML from cross-validation runs as a dataframe.
+def download_hyperdrive_metrics_if_required(
+    parent_run_id: str,
+    download_dir: Path,
+    aml_workspace: Workspace,
+    hyperdrive_arg_name: str = "crossval_index",
+    overwrite: bool = False,
+) -> Path:
+    """Fetch metrics logged to Azure ML from hyperdrive runs.
 
     Will only download the metrics if they do not already exist locally, as this can take several
     seconds for each child run.
 
     :param parent_run_id: Azure ML run ID for the parent Hyperdrive run.
     :param download_dir: Directory where to save the downloaded metrics as `aml_metrics.json`.
     :param aml_workspace: Azure ML workspace in which the runs were executed.
-    :param crossval_arg_name: Name of the Hyperdrive argument used for indexing the child runs.
+    :param hyperdrive_arg_name: Name of the Hyperdrive argument used for indexing the child runs.
     :param overwrite: Whether to force the download even if metrics are already saved locally.
-    :return: A dataframe in the format returned by :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
+    :return: The path of the downloaded json file.
     """
     metrics_json = download_dir / "aml_metrics.json"
     if not overwrite and metrics_json.is_file():
         print(f"AML metrics file already exists at {metrics_json}")
-        metrics_df = pd.read_json(metrics_json)
     else:
-        metrics_df = aggregate_hyperdrive_metrics(run_id=parent_run_id,
-                                                  child_run_arg_name=crossval_arg_name,
-                                                  aml_workspace=aml_workspace)
+        metrics_df = aggregate_hyperdrive_metrics(
+            run_id=parent_run_id, child_run_arg_name=hyperdrive_arg_name, aml_workspace=aml_workspace
+        )
         metrics_json.parent.mkdir(parents=True, exist_ok=True)
         print(f"Writing AML metrics file to {metrics_json}")
         df_to_json(metrics_df, metrics_json)
-    return metrics_df.sort_index(axis='columns')
+    return metrics_json
+
 
+def collect_hyperdrive_metrics(metrics_json: Path) -> pd.DataFrame:
+    """
+    Collect the hyperdrive metrics from the downloaded metrics json file in a dataframe.
+    :param metrics_json: Path of the downloaded metrics file `aml_metrics.json`.
+    :return: A dataframe in the format returned by :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
+    """
+    metrics_df = pd.read_json(metrics_json).sort_index(axis='columns')
+    return metrics_df
 
-def get_crossval_metrics_table(metrics_df: pd.DataFrame, metrics_list: Sequence[str]) -> pd.DataFrame:
-    """Format raw cross-validation metrics into a table with a summary "Mean ± Std" column.
+
+def get_hyperdrive_metrics_table(metrics_df: pd.DataFrame, metrics_list: Sequence[str]) -> pd.DataFrame:
+    """Format raw hyperdrive metrics into a table with a summary "Mean ± Std" column.
 
     Note that this function only supports scalar metrics. To format metrics that are logged
     throughout training, you should call :py:func:`get_best_epoch_metrics()` first.
 
-    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_crossval_metrics()` and
+    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_hyperdrive_metrics()` and
         :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
     :param metrics_list: The list of metrics to include in the table.
     :return: A dataframe with the values of the selected metrics formatted as strings, including a
         header and a summary column.
     """
-    header = ["Metric"] + [f"Split {k}" for k in metrics_df.columns] + ["Mean ± Std"]
+    header = ["Metric"] + [f"Child {k}" for k in metrics_df.columns] + ["Mean ± Std"]
     metrics_rows = []
     for metric in metrics_list:
         values: pd.Series = metrics_df.loc[metric]
         mean = values.mean()
         std = values.std()
-        row = [metric] + [f"{v:.3f}" for v in values] + [f"{mean:.3f} ± {std:.3f}"]
+        round_values: List[str] = [f"{v:.3f}" if v is not None else str(np.nan) for v in values]
+        agg_values: List[str] = [f"{mean:.3f} ± {std:.3f}"]
+        row = [metric] + round_values + agg_values
         metrics_rows.append(row)
     table = pd.DataFrame(metrics_rows, columns=header).set_index(header[0])
     return table
 
 
-def get_best_epochs(metrics_df: pd.DataFrame, primary_metric: str, maximise: bool = True) -> Dict[int, int]:
-    """Determine the best epoch for each cross-validation run based on a given metric.
+def get_best_epochs(
+    metrics_df: pd.DataFrame, primary_metric: str, max_epochs_dict: Dict[int, int], maximise: bool = True
+) -> Dict[int, Any]:
+    """Determine the best epoch for each hyperdrive child run based on a given metric.
 
     The returned epoch indices are relative to the logging frequency of the chosen metric, i.e.
     should not be mixed between pipeline stages that log metrics at different epoch intervals.
 
-    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_crossval_metrics()` and
+    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_hyperdrive_metrics()` and
         :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
     :param primary_metric: Name of the reference metric to optimise.
+    :max_epochs_dict: A dictionary of the maximum number of epochs in each cross-validation round.
     :param maximise: Whether the given metric should be maximised (minimised if `False`).
-    :return: Dictionary mapping each cross-validation index to its best epoch.
+    :return: Dictionary mapping each hyperdrive child index to its best epoch.
     """
-    best_fn = np.argmax if maximise else np.argmin
-    best_epochs = metrics_df.loc[primary_metric].apply(best_fn)
-    return best_epochs.to_dict()
-
-
-def get_best_epoch_metrics(metrics_df: pd.DataFrame, metrics_list: Sequence[str],
-                           best_epochs: Dict[int, int]) -> pd.DataFrame:
-    """Extract the values of the selected cross-validation metrics at the given best epochs.
+    best_epochs: Dict[int, Any] = {}
+    for child_index in metrics_df.columns:
+        primary_metric_list = metrics_df[child_index][primary_metric]
+        if primary_metric_list is not None:
+            # If extra validation epoch was logged (N+1), return only the first N elements
+            primary_metric_list = (
+                primary_metric_list[:-1]
+                if (len(primary_metric_list) == max_epochs_dict[child_index] + 1)
+                else primary_metric_list
+            )
+            best_epochs[child_index] = int(
+                np.argmax(primary_metric_list) if maximise else np.argmin(primary_metric_list)
+            )
+        else:
+            best_epochs[child_index] = None
+    return best_epochs
+
+
+def get_best_epoch_metrics(
+    metrics_df: pd.DataFrame, metrics_list: Sequence[str], best_epochs: Dict[int, Any]
+) -> pd.DataFrame:
+    """Extract the values of the selected hyperdrive metrics at the given best epochs.
 
     The `best_epoch` indices are relative to the logging frequency of the chosen primary metric,
     i.e. the metrics in `metrics_list` must have been logged at the same epoch intervals.
 
-    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_crossval_metrics()` and
+    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_hyperdrive_metrics()` and
         :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
     :param metrics_list: Names of the metrics to index by the best epoch indices provided. Their
         values in `metrics_df` should be lists.
-    :param best_epochs: Dictionary of cross-validation indices to best epochs, as returned by
+    :param best_epochs: Dictionary of hyperdrive child runs indices to best epochs, as returned by
         :py:func:`get_best_epochs()`.
     :return: Dataframe with the same columns as `metrics_df` and rows specified by `metrics_list`,
         containing only scalar values.
     """
-    best_metrics = [metrics_df.loc[metrics_list, k].apply(lambda values: values[epoch])
-                    for k, epoch in best_epochs.items()]
+    best_metrics = [
+        metrics_df.loc[metrics_list, k].apply(lambda values: values[epoch])
+        if epoch is not None
+        else metrics_df.loc[metrics_list, k]
+        for k, epoch in best_epochs.items()
+    ]
     best_metrics_df = pd.DataFrame(best_metrics).T
     return best_metrics_df
 
 
 def get_formatted_run_info(parent_run: Run) -> str:
-    """Format Azure ML cross-validation run information as HTML.
+    """Format Azure ML hyperdrive run information as HTML.
 
     Includes details of the parent and child runs, as well as submission information.
 
     :param parent_run: Parent Hyperdrive Azure ML run object.
     :return: Formatted HTML string.
     """
+
     def format_experiment(experiment: Experiment) -> str:
         return f"<a href={experiment.get_portal_url()}>{experiment.name}</a>"
 
     def format_run(run: Run) -> str:
         return f"<a href={run.get_portal_url()}>{run.display_name}</a> ({run.id}, {run.get_status()})"
 
     def format_submission_info(run: Run) -> str:
@@ -212,28 +266,50 @@
     html += "\n</ul>"
 
     html += f"\n<p>{format_submission_info(parent_run)}"
     html += f"\n<p>Command-line arguments: <code>{parent_run.get_tags()['commandline_args']}</code>"
     return html
 
 
-def collect_class_info(metrics_df: pd.DataFrame) -> Tuple[int, List[str]]:
+def get_child_runs_hyperparams(metrics_df: pd.DataFrame) -> Dict[int, Dict]:
     """
-    Get the class names from metrics dataframe
-    :param metrics_df: Metrics dataframe, as returned by :py:func:`collect_crossval_metrics()` and
+    Get the hyperparameters of each child run from the metrics dataframe.
+    :param: metrics_df: Metrics dataframe, as returned by :py:func:`collect_hyperdrive_metrics()` and
         :py:func:`~health_azure.aggregate_hyperdrive_metrics()`.
-    :return: Number of classes and list of class names
+    :return: A dictionary of hyperparameter dictionaries for the child runs.
     """
-    hyperparams = metrics_df[0][AMLMetricsJsonKey.HYPERPARAMS]
-    hyperparams_name = hyperparams[AMLMetricsJsonKey.NAME]
-    hyperparams_value = hyperparams[AMLMetricsJsonKey.VALUE]
-    num_classes_index = hyperparams_name.index(AMLMetricsJsonKey.N_CLASSES)
-    num_classes = int(hyperparams_value[num_classes_index])
-    class_names_index = hyperparams_name.index(AMLMetricsJsonKey.CLASS_NAMES)
-    class_names = hyperparams_value[class_names_index]
+    hyperparams_children = {}
+    for child_index in metrics_df.columns:
+        hyperparams = metrics_df[child_index][AMLMetricsJsonKey.HYPERPARAMS]
+        hyperparams_dict = dict(zip(hyperparams[AMLMetricsJsonKey.NAME], hyperparams[AMLMetricsJsonKey.VALUE]))
+        hyperparams_children[child_index] = hyperparams_dict
+    return hyperparams_children
+
+
+def collect_class_info(hyperparams_children: Dict[int, Dict]) -> Tuple[int, List[str]]:
+    """
+    Get the class names from the hyperparameters of child runs.
+    :param hyperparams_children: Dict of hyperparameter dicts, as returned by :py:func:`get_child_runs_hyperparams()`.
+    :return: Number of classes and list of class names.
+    """
+    hyperparams_single_run = list(hyperparams_children.values())[0]
+    num_classes = int(hyperparams_single_run[AMLMetricsJsonKey.N_CLASSES])
+    class_names = hyperparams_single_run[AMLMetricsJsonKey.CLASS_NAMES]
     if class_names == "None":
         class_names = None
     else:
         # Remove [,], and quotation marks from the string of class names
         class_names = [name.lstrip() for name in class_names[1:-1].replace("'", "").split(',')]
     class_names = validate_class_names(class_names=class_names, n_classes=num_classes)
     return (num_classes, list(class_names))
+
+
+def get_max_epochs(hyperparams_children: Dict[int, Dict]) -> Dict[int, int]:
+    """
+    Get the maximum number of epochs for each round from the metrics dataframe.
+    :param hyperparams_children: Dict of hyperparameter dicts, as returned by :py:func:`get_child_runs_hyperparams()`.
+    :return: Dictionary with the number of epochs in each hyperdrive run.
+    """
+    max_epochs_dict = {}
+    for child_index in hyperparams_children.keys():
+        max_epochs_dict[child_index] = int(hyperparams_children[child_index][AMLMetricsJsonKey.MAX_EPOCHS])
+    return max_epochs_dict
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/tcga_utils.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/tcga_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/tiles_selection_utils.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/tiles_selection_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,33 +36,37 @@
         self.id = id
         self.left = left
         self.top = top
 
 
 class SlideNode:
     """Data structure class for slide nodes used by `TopBottomTilesHandler` to store top and bottom slides by
-    probability score. """
+    probability score."""
 
-    def __init__(self, slide_id: str, prob_score: float, true_label: int, pred_label: int) -> None:
+    def __init__(
+        self, slide_id: str, gt_prob_score: float, pred_prob_score: float, true_label: int, pred_label: int
+    ) -> None:
         """
-        :param prob_score: The probability score assigned to the slide node. This scalar defines the order of the
-            slide_node among the nodes in the max/min heap.
+        :param gt_prob_score: The probability score assigned to ground truth label of slide node. This scalar defines
+            the order of the slide_node among the nodes in the max/min heap.
+        :param pred_prob_score: The probability score assigned to predicted label of slide node.
         :param slide_id: The slide id in the data cohort.
         :param true_label: The ground truth label of the slide node.
         :param pred_label: The label predicted by the model.
         """
         self.slide_id = slide_id
-        self.prob_score = prob_score
+        self.gt_prob_score = gt_prob_score
+        self.pred_prob_score = pred_prob_score
         self.true_label = true_label
         self.pred_label = pred_label
         self.top_tiles: List[TileNode] = []
         self.bottom_tiles: List[TileNode] = []
 
     def __lt__(self, other: "SlideNode") -> bool:
-        return self.prob_score < other.prob_score
+        return self.gt_prob_score < other.gt_prob_score
 
     def update_selected_tiles(self, tiles: Tensor, attn_scores: Tensor, num_top_tiles: int) -> None:
         """Update top and bottom k tiles values from a set of tiles and their assigned attention scores.
 
         :param tiles: A stack of tiles with shape (n_tiles, channels, height, width).
         :param attn_scores: A tensor of attention scores assigned by the deepmil model to tiles of shape (n_tiles, 1).
         :param num_top_tiles: The number of tiles to select as top and bottom tiles.
@@ -73,15 +77,15 @@
         self.top_tiles = [TileNode(data=tiles[i], attn=attn_scores[i].item()) for i in top_k_indices]
 
         _, bottom_k_indices = torch.topk(attn_scores, k=num_top_tiles, largest=False, sorted=True)
         self.bottom_tiles = [TileNode(data=tiles[i], attn=attn_scores[i].item()) for i in bottom_k_indices]
 
     def _shallow_copy(self) -> "SlideNode":
         """Returns a shallow copy of the current slide node contaning only the slide_id and its probability score."""
-        return SlideNode(self.slide_id, self.prob_score, self.true_label, self.pred_label)
+        return SlideNode(self.slide_id, self.gt_prob_score, self.pred_prob_score, self.true_label, self.pred_label)
 
 
 SlideOrTileKey = Union[SlideKey, TileKey]
 SlideDict = Dict[int, List[SlideNode]]
 TileDict = Dict[str, List[TileNode]]
 
 
@@ -102,56 +106,47 @@
             )
 
         self.n_classes = n_classes if n_classes > 1 else 2
         self.num_slides = num_slides
         self.num_tiles = num_tiles
         self.top_slides_heaps: SlideDict = self._initialise_slide_heaps()
         self.bottom_slides_heaps: SlideDict = self._initialise_slide_heaps()
-        self.report_cases_slide_ids = self.init_report_cases()
 
     def _initialise_slide_heaps(self) -> SlideDict:
         return {class_id: [] for class_id in range(self.n_classes)}
 
-    def init_report_cases(self) -> Dict[str, List[str]]:
-        """ Initializes the report cases dictionary to store slide_ids per case.
-        Possible cases are set such as class 0 is considered to be the negative class.
-
-        :return: A dictionary that maps TN/FP TP_{i}/FN_{i}, i={1,..., self.n_classes+1} cases to an empty list to be
-            filled with corresponding slide ids.
-        """
-        report_cases: Dict[str, List[str]] = {"TN": [], "FP": []}
-        report_cases.update({f"TP_{class_id}": [] for class_id in range(1, self.n_classes)})
-        report_cases.update({f"FN_{class_id}": [] for class_id in range(1, self.n_classes)})
-        return report_cases
-
     def _clear_cached_slides_heaps(self) -> None:
         self.top_slides_heaps = self._initialise_slide_heaps()
         self.bottom_slides_heaps = self._initialise_slide_heaps()
 
     def _reset_slides_heaps(self, new_top_slides_heaps: SlideDict, new_bottom_slides_heaps: SlideDict) -> None:
         self.top_slides_heaps = new_top_slides_heaps
         self.bottom_slides_heaps = new_bottom_slides_heaps
 
     def _update_label_slides(
-        self, class_slides_heap: List[SlideNode], tiles: Tensor, attn_scores: Tensor, slide_node: SlideNode,
+        self,
+        class_slides_heap: List[SlideNode],
+        tiles: Tensor,
+        attn_scores: Tensor,
+        slide_node: SlideNode,
     ) -> None:
         """Update the selected slides of a given class label on the fly by updating the content of class_slides_heap.
         First, we push a shallow slide_node into the slides_heaps[gt_label]. The order in slides_heaps[gt_label] is
-        defined by the slide_node.prob_score that is positive in top_slides_heaps nodes and negative in
+        defined by the slide_node.gt_prob_score that is positive in top_slides_heaps nodes and negative in
         bottom_slides_heaps nodes.
         Second, we check if we exceeded self.num_top_slides to be selected.
             If so, we update the slides_node top and bottom tiles only if it has been kept in the heap.
             Else, we haven't reached the heaps max_capacity so we save the top and bottom tiles.
 
         :param class_slides_heap: The class_slides_heap dict to be updated. Either self.top_slides_heaps or
             self.bottom_slides_heaps.
         :param tiles: Tiles of a given whole slide retrieved from the current validation or test batch.
             (n_tiles, channels, height, width)
         :param attn_scores: The tiles attention scores to determine top and bottom tiles. (n_tiles, )
-        :param slide_node: A shallow version of slide_node that contains only slide_id and its assigned prob_score.
+        :param slide_node: A shallow version of slide_node that contains only slide_id and additional metadata.
         """
         heapq.heappush(class_slides_heap, slide_node)
         if len(class_slides_heap) == self.num_slides + 1:
             old_slide_node = heapq.heappop(class_slides_heap)
             if old_slide_node.slide_id != slide_node.slide_id:
                 slide_node.update_selected_tiles(tiles, attn_scores, self.num_tiles)
         else:
@@ -166,41 +161,47 @@
         """
         if self.num_slides > 0:
             slide_ids = batch[SlideKey.SLIDE_ID]
             if isinstance(slide_ids[0], list):
                 slide_ids = [slide_id[0] for slide_id in slide_ids]  # to account for repetitions in tiles pipeline
             batch_size = len(batch[SlideKey.IMAGE])
             for i in range(batch_size):
-                label = results[ResultsKey.TRUE_LABEL][i].item()
-                probs_gt_label = results[ResultsKey.CLASS_PROBS][:, label][i].item()
+                gt_label = results[ResultsKey.TRUE_LABEL][i].item()
+                pred_label = results[ResultsKey.PRED_LABEL][i].item()
+                gt_prob_score = results[ResultsKey.CLASS_PROBS][:, gt_label][i].item()
+                pred_prob_score = results[ResultsKey.CLASS_PROBS][:, pred_label][i].item()
                 tiles = batch[SlideKey.IMAGE][i]
                 attn_scores = results[ResultsKey.BAG_ATTN][i].squeeze(0)
-                pred_label = results[ResultsKey.PRED_LABEL][i].item()
-                self._update_label_slides(
-                    class_slides_heap=self.top_slides_heaps[label],
-                    tiles=tiles,
-                    attn_scores=attn_scores,
-                    slide_node=SlideNode(
-                        slide_id=slide_ids[i],
-                        prob_score=probs_gt_label,
-                        true_label=label,
-                        pred_label=pred_label,
-                    ),
-                )
-                self._update_label_slides(
-                    class_slides_heap=self.bottom_slides_heaps[label],
-                    tiles=tiles,
-                    attn_scores=attn_scores,
-                    slide_node=SlideNode(
-                        slide_id=slide_ids[i],
-                        prob_score=-probs_gt_label,  # negative score for bottom slides to reverse order in max heap
-                        true_label=label,
-                        pred_label=pred_label,
-                    ),
-                )
+                if pred_label == gt_label:
+                    self._update_label_slides(
+                        class_slides_heap=self.top_slides_heaps[gt_label],
+                        tiles=tiles,
+                        attn_scores=attn_scores,
+                        slide_node=SlideNode(
+                            slide_id=slide_ids[i],
+                            gt_prob_score=gt_prob_score,
+                            pred_prob_score=pred_prob_score,
+                            true_label=gt_label,
+                            pred_label=pred_label,
+                        ),
+                    )
+                elif pred_label != gt_label:
+                    self._update_label_slides(
+                        class_slides_heap=self.bottom_slides_heaps[gt_label],
+                        tiles=tiles,
+                        attn_scores=attn_scores,
+                        slide_node=SlideNode(
+                            slide_id=slide_ids[i],
+                            # negative score for bottom slides to reverse order in max heap
+                            gt_prob_score=-gt_prob_score,
+                            pred_prob_score=pred_prob_score,
+                            true_label=gt_label,
+                            pred_label=pred_label,
+                        ),
+                    )
 
     def _shallow_copy_slides_heaps(self, slides_heaps: SlideDict) -> SlideDict:
         """Returns a shallow copy of slides heaps to be synchronised across devices.
 
         :param slides_heaps: The slides_heaps dict to be shallow copied. Either self.top_slides_heaps or
             self.bottom_slides_heaps.
         """
@@ -272,39 +273,41 @@
                     if slide_node.slide_id == new_slide_node.slide_id:
                         top_tiles[new_slide_node.slide_id] = slide_node.top_tiles
                         bottom_tiles[new_slide_node.slide_id] = slide_node.bottom_tiles
                         break
         return top_tiles, bottom_tiles
 
     def _update_shallow_slides_heaps_with_top_bottom_tiles(
-        self, slides_heaps: SlideDict, top_tiles: TileDict, bottom_tiles: TileDict,
+        self,
+        slides_heaps: SlideDict,
+        top_tiles: TileDict,
+        bottom_tiles: TileDict,
     ) -> None:
         """Update shallow version of slides heaps with top and bottom tiles gathered across devices.
 
         :param slides_heaps: The slides_heaps to update. Either self.top_slides_heaps or self.bottom_slides_heaps.
         :param top_tiles: Top tiles dictionary with slide_ids as keys.
         :param bottom_tiles: Bottom tiles dictionary with slide_ids as keys.
         """
         for class_id in range(self.n_classes):
             for slide_node in slides_heaps[class_id]:
                 slide_node.top_tiles = top_tiles[slide_node.slide_id]
                 slide_node.bottom_tiles = bottom_tiles[slide_node.slide_id]
 
     def gather_selected_tiles_across_devices(self) -> None:
         """Gathers top and bottom tiles across devices in ddp context. For each of top and bottom slides heaps:
-            1- make a shallow copy of top and bottom slides_heaps
-            2- gather best shallow slides across gpus
-            3- select top and bottom tiles available in each device
-            4- gather these tiles across devices
-            5- update the synchronized shallow slide nodes across devices with their top and bottom tiles
+        1- make a shallow copy of top and bottom slides_heaps
+        2- gather best shallow slides across gpus
+        3- select top and bottom tiles available in each device
+        4- gather these tiles across devices
+        5- update the synchronized shallow slide nodes across devices with their top and bottom tiles
         """
         if torch.distributed.is_initialized() and self.num_slides > 0:
             world_size = torch.distributed.get_world_size()
             if world_size > 1:
-
                 shallow_top_slides_heaps = self._shallow_copy_slides_heaps(slides_heaps=self.top_slides_heaps)
                 shallow_bottom_slides_heaps = self._shallow_copy_slides_heaps(slides_heaps=self.bottom_slides_heaps)
 
                 agg_top_slides_heaps = self._aggregate_shallow_slides_heaps(world_size, shallow_top_slides_heaps)
                 agg_bottom_slides_heaps = self._aggregate_shallow_slides_heaps(world_size, shallow_bottom_slides_heaps)
 
                 top_slides_top_tiles, top_slides_bottom_tiles = self._collect_tiles_for_selected_slides_on_device(
```

### Comparing `hi-ml-cpath-0.2.9/src/health_cpath/utils/viz_utils.py` & `hi-ml-cpath-0.3.0/src/health_cpath/utils/viz_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 
 import logging
 import sys
 import math
+import cv2
 import numpy as np
+import seaborn as sns
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 import matplotlib.collections as collection
 
 from math import ceil
 from pathlib import Path
 from typing import Sequence, List, Any, Dict, Optional, Union, Tuple
 
 from monai.data.dataset import Dataset
-from monai.data.image_reader import WSIReader
 from torch.utils.data import DataLoader
-
+from health_cpath.datasets.panda_dataset import PandaDataset
+from health_cpath.preprocessing.loading import LoadingParams, ROIType, WSIBackend
 from health_cpath.utils.naming import SlideKey
 from health_cpath.utils.naming import ResultsKey
 from health_cpath.utils.heatmap_utils import location_selected_tiles
 from health_cpath.utils.tiles_selection_utils import SlideNode
-from health_cpath.datasets.panda_dataset import PandaDataset, LoadPandaROId
 
 
-def load_image_dict(sample: dict, level: int, margin: int) -> Dict[SlideKey, Any]:
+def load_image_dict(sample: dict, loading_params: LoadingParams) -> Dict[SlideKey, Any]:
     """
     Load image from metadata dictionary
+
     :param sample: dict describing image metadata. Example:
         {'image_id': ['1ca999adbbc948e69783686e5b5414e4'],
         'image': ['/tmp/datasets/PANDA/train_images/1ca999adbbc948e69783686e5b5414e4.tiff'],
          'mask': ['/tmp/datasets/PANDA/train_label_masks/1ca999adbbc948e69783686e5b5414e4_mask.tiff'],
          'data_provider': ['karolinska'],
          'isup_grade': tensor([0]),
          'gleason_score': ['0+0']}
-    :param level: level of resolution to be loaded
-    :param margin: margin to be included
-    :return: a dict containing the image data and metadata
+    :param loading_params: LoadingParams object that contains the parameters to load the image.
     """
-    loader = LoadPandaROId(WSIReader("cuCIM"), level=level, margin=margin)
+    loader = loading_params.get_load_roid_transform()
     img = loader(sample)
     return img
 
 
 def plot_panda_data_sample(
     panda_dir: str, nsamples: int, ncols: int, level: int, margin: int, title_key: str = "data_provider"
 ) -> None:
@@ -63,24 +63,25 @@
     nrows = math.ceil(nsamples / ncols)
     fig, axes = plt.subplots(ncols=ncols, nrows=nrows, figsize=(9, 9))
 
     for dict_images, ax in zip(loader, axes.flat):
         slide_id = dict_images[SlideKey.SLIDE_ID]
         title = dict_images[SlideKey.METADATA][title_key]
         print(f">>> Slide {slide_id}")
-        img = load_image_dict(dict_images, level=level, margin=margin)
+        loading_params = LoadingParams(level=level, margin=margin, backend=WSIBackend.CUCIM, roi_type=ROIType.MASK)
+        img = load_image_dict(dict_images, loading_params)
         ax.imshow(img[SlideKey.IMAGE].transpose(1, 2, 0))
         ax.set_title(title)
     fig.tight_layout()
 
 
 def plot_scores_hist(
     results: Dict, prob_col: str = ResultsKey.CLASS_PROBS, gt_col: str = ResultsKey.TRUE_LABEL
 ) -> plt.Figure:
-    """Plot scores as a historgram.
+    """Plot scores as a histogram.
 
     :param results: List that contains slide_level dicts
     :param prob_col: column name that contains the scores
     :param gt_col: column name that contains the true label
     :return: matplotlib figure of the scores histogram by class
     """
     n_classes = len(results[prob_col][0])
@@ -91,14 +92,26 @@
     fig, ax = plt.subplots()
     ax.hist(scores_class, label=[str(i) for i in range(n_classes)], alpha=0.5)
     ax.set_xlabel("Predicted Score")
     ax.legend()
     return fig
 
 
+def _get_histo_plot_title(case: str, slide_node: SlideNode) -> str:
+    """Return the standard title for histopathology plots.
+
+    :param case: case id e.g., TP, FN, FP, TN
+    :param slide_node: SlideNode object that encapsulates the slide information
+    """
+    return (
+        f"{case}: {slide_node.slide_id} P={slide_node.pred_prob_score:.2f} \n Predicted label: {slide_node.pred_label} "
+        f"True label: {slide_node.true_label}"
+    )
+
+
 def plot_attention_tiles(
     case: str, slide_node: SlideNode, top: bool, num_columns: int, figsize: Tuple[int, int]
 ) -> Optional[plt.Figure]:
     """Plot top or bottom tiles figures along with their attention scores.
 
     :param case: The report case (e.g., TP, FN, ...)
     :param slide_node: The slide node for which we would like to plot attention tiles.
@@ -108,23 +121,20 @@
     :param figsize: The figure size of tiles attention plots, defaults to (10, 10)
     """
     tile_nodes = slide_node.top_tiles if top else slide_node.bottom_tiles
     num_rows = int(ceil(len(tile_nodes) / num_columns))
     if num_rows == 0:
         logging.warning(
             "The number of selected top and bottom tiles is too low, plotting will be skipped."
-            "Try debugging with a higher num_top_tiles and/or a higher number of batches.")
+            "Try debugging with a higher num_top_tiles and/or a higher number of batches."
+        )
         return None
 
     fig, axs = plt.subplots(nrows=num_rows, ncols=num_columns, figsize=figsize)
-    fig.suptitle(
-        f"{case}: {slide_node.slide_id} P={abs(slide_node.prob_score):.2f} \n Predicted label: {slide_node.pred_label} "
-        f"True label: {slide_node.true_label}"
-    )
-
+    fig.suptitle(_get_histo_plot_title(case, slide_node))
     for ax, tile_node in zip(axs.flat, tile_nodes):
         ax.imshow(np.transpose(tile_node.data.numpy(), (1, 2, 0)), clim=(0, 255), cmap="gray")
         ax.set_title("%.6f" % tile_node.attn)
 
     for ax in axs.flat:
         ax.set_axis_off()
     return fig
@@ -137,108 +147,165 @@
     :param slide_node: The slide node for which we would like to plot attention tiles.
     :param slide_image: Numpy array of the slide image (shape: [3, H, W]).
     :return: matplotlib figure of the slide thumbnail.
     """
     fig, ax = plt.subplots()
     slide_image = slide_image.transpose(1, 2, 0)
     ax.imshow(slide_image)
-    fig.suptitle(
-        f"{case}: {slide_node.slide_id} P={abs(slide_node.prob_score):.2f} \n Predicted label: {slide_node.pred_label} "
-        f"True label: {slide_node.true_label}"
-    )
+    fig.suptitle(_get_histo_plot_title(case, slide_node))
     ax.set_axis_off()
     original_size = fig.get_size_inches()
     fig.set_size_inches((original_size[0] * scale, original_size[1] * scale))
     return fig
 
 
 def plot_heatmap_overlay(
     case: str,
     slide_node: SlideNode,
-    slide_image: np.ndarray,
+    slide_dict: Dict[SlideKey, Any],
     results: Dict[ResultsKey, List[Any]],
-    location_bbox: List[int],
     tile_size: int = 224,
-    level: int = 1,
+    should_upscale_coords: bool = True,
+    extra_slide_dict: Optional[Dict[SlideKey, Any]] = None,
 ) -> plt.Figure:
     """Plots heatmap of selected tiles (e.g. tiles in a bag) overlay on the corresponding slide.
 
     :param case: The report case (e.g., TP, FN, ...)
     :param slide_node: The slide node that encapsulates the slide metadata.
-    :param slide_image: Numpy array of the slide image (shape: [3, H, W]).
+    :param slide_dict: Dictionary of the slide image (shape: [3, H, W]) containing the slide image and metadata: the
+        location of the bouding box of the slide and the scale factor to convert the heatmap coordinates to the slide
+        level.
     :param results: Dict containing ResultsKey keys (e.g. slide id) and values as lists of output slides.
     :param tile_size: Size of each tile. Default 224.
-    :param level: Magnification at which tiles are available (e.g. PANDA levels are 0 for original,
-    1 for 4x downsampled, 2 for 16x downsampled). Default 1.
-    :param location_bbox: Location of the bounding box of the slide.
+    :param should_upscale_coords: If True, upscales the heatmap coordinates to the slide level. Default True.
+    :param extra_slide_dict: An optional dictionary containing an extra slide image and metadata. Default None.
     :return: matplotlib figure of the heatmap of the given tiles on slide.
     """
-    fig, ax = plt.subplots()
-    fig.suptitle(
-        f"{case}: {slide_node.slide_id} P={abs(slide_node.prob_score):.2f} \n Predicted label: {slide_node.pred_label} "
-        f"True label: {slide_node.true_label}"
-    )
-    slide_image = slide_image.transpose(1, 2, 0)
-    ax.imshow(slide_image)
-    ax.set_xlim(0, slide_image.shape[1])
-    ax.set_ylim(slide_image.shape[0], 0)
-
-    coords_list = []
+    fig = plt.figure(constrained_layout=True)
+    gs = fig.add_gridspec(2 if not extra_slide_dict else 3, 1)
+    ax0 = fig.add_subplot(gs[0, 0])
+    ax1 = fig.add_subplot(gs[1, 0], sharex=ax0, sharey=ax0)
+    cax = ax1.inset_axes([1.02, 0, 0.03, 1], transform=ax1.transAxes)  # add colorbar axis
+    axes = [ax0, ax1]
+    if extra_slide_dict:
+        ax2 = fig.add_subplot(gs[2, 0], sharex=ax0, sharey=ax0)
+        axes.append(ax2)
+    fig.execute_constrained_layout()
+    fig.suptitle(_get_histo_plot_title(case, slide_node))
+
+    def _get_slide_image_from_slide_dict(slide_dict: Dict[SlideKey, Any]) -> np.ndarray:
+        slide_image = slide_dict[SlideKey.IMAGE]
+        assert isinstance(slide_image, np.ndarray), f"slide image must be a numpy array, got {type(slide_image)}"
+        return slide_image.transpose(1, 2, 0)
+
+    slide_image = _get_slide_image_from_slide_dict(slide_dict)
+
+    ax0.imshow(slide_image)
+    ax1.imshow(slide_image, alpha=0.5)
+    if extra_slide_dict:
+        extra_image = _get_slide_image_from_slide_dict(extra_slide_dict)
+        if extra_image.shape != slide_image.shape:
+            extra_image = cv2.resize(
+                extra_image, (slide_image.shape[1], slide_image.shape[0]), interpolation=cv2.INTER_AREA
+            )
+        ax2.imshow(extra_image)
+        ax2.tick_params('x', labelbottom=False)
+    for ax in axes:
+        ax.set_xlim(0, slide_image.shape[1])
+        ax.set_ylim(slide_image.shape[0], 0)
+    ax0.tick_params('x', labelbottom=False)
     slide_ids = [item[0] for item in results[ResultsKey.SLIDE_ID]]
     slide_idx = slide_ids.index(slide_node.slide_id)
     attentions = results[ResultsKey.BAG_ATTN][slide_idx]
 
-    # for each tile in the bag
-    for tile_idx in range(len(results[ResultsKey.IMAGE_PATH][slide_idx])):
-        tile_coords = np.transpose(
-            np.array(
-                [
-                    results[ResultsKey.TILE_LEFT][slide_idx][tile_idx].cpu().numpy(),
-                    results[ResultsKey.TILE_TOP][slide_idx][tile_idx].cpu().numpy(),
-                ]
-            )
-        )
-        coords_list.append(tile_coords)
-
-    coords = np.array(coords_list)
+    coords = np.transpose(
+        [results[ResultsKey.TILE_LEFT][slide_idx].cpu().numpy(), results[ResultsKey.TILE_TOP][slide_idx].cpu().numpy()]
+    )
     attentions = np.array(attentions.cpu()).reshape(-1)
 
-    sel_coords = location_selected_tiles(tile_coords=coords, location_bbox=location_bbox, level=level)
-    cmap = plt.cm.get_cmap("Reds")
+    sel_coords = location_selected_tiles(
+        tile_coords=coords,
+        location_bbox=slide_dict[SlideKey.ORIGIN],
+        scale_factor=slide_dict[SlideKey.SCALE],
+        should_upscale_coords=should_upscale_coords,
+    )
+    cmap = plt.cm.get_cmap("Spectral_r")  # _r reverse the color map so that the highest attention is red
 
     tile_xs, tile_ys = sel_coords.T
     rects = [patches.Rectangle(xy, tile_size, tile_size) for xy in zip(tile_xs, tile_ys)]
 
-    pc = collection.PatchCollection(rects, match_original=True, cmap=cmap, alpha=0.5, edgecolor="black")
+    # line width is set to 0 to avoid the black border around the tiles as the tiles are already colored
+    pc = collection.PatchCollection(rects, match_original=True, cmap=cmap, alpha=0.5, linewidth=0)
     pc.set_array(np.array(attentions))
-    pc.set_clim([0, 1])
-    ax.add_collection(pc)
-    plt.colorbar(pc, ax=ax)
+    ax1.add_collection(pc)
+    cb = plt.colorbar(pc, cax=cax)  # add colorbar to the right of the plot (cax)
+    mean_loc = attentions.mean()  # add a horizontal line at the mean attention value
+    cb.ax.hlines(mean_loc, attentions.min(), attentions.max(), color="k", linewidth=2)
+    return fig
+
+
+def plot_attention_histogram(case: str, slide_node: SlideNode, results: Dict[ResultsKey, List[Any]]) -> plt.Figure:
+    """Plots a histogram of the attention values of the tiles in a bag.
+
+    :param case: The report case (e.g., TP, FN, ...)
+    :param slide_node: The slide node that encapsulates the slide metadata.
+    :param results: Dict containing ResultsKey keys (e.g. slide id) and values as lists of output slides.
+    :return: matplotlib figure of the histogram of the attention values of the tiles in a bag.
+    """
+    slide_ids = [item[0] for item in results[ResultsKey.SLIDE_ID]]
+    slide_idx = slide_ids.index(slide_node.slide_id)
+    attentions = results[ResultsKey.BAG_ATTN][slide_idx]
+    fig, ax = plt.subplots()
+    ax = sns.distplot(attentions.cpu().numpy().reshape(-1), kde=False)
+    ax.set_xlabel("Attention scores")
+    fig.suptitle(_get_histo_plot_title(case, slide_node))
     return fig
 
 
 def plot_normalized_confusion_matrix(cm: np.ndarray, class_names: Sequence[str]) -> plt.Figure:
     """Plots a normalized confusion matrix and returns the figure.
-    param cm: Normalized confusion matrix to be plotted.
-    param class_names: List of class names.
-    """
-    import seaborn as sns
 
+    :param cm: Normalized confusion matrix to be plotted.
+    :param class_names: List of class names.
+    """
     fig, ax = plt.subplots()
     ax = sns.heatmap(cm, annot=True, cmap="Blues", fmt=".2%")
     ax.set_xlabel("Predicted")
     ax.set_ylabel("True")
     ax.xaxis.set_ticklabels(class_names)
     ax.yaxis.set_ticklabels(class_names)
     return fig
 
 
+def plot_normalized_and_non_normalized_confusion_matrices(
+    cm: np.ndarray,
+    cm_n: np.ndarray,
+    class_names: Sequence[str],
+) -> plt.Figure:
+    """Plots a normalized and non-normalized confusion matrix and returns the figure.
+
+    :param cm: Non normalized confusion matrix to be plotted.
+    :param cm_n: Normalized confusion matrix to be plotted.
+    :param class_names: List of class names.
+    """
+    fig, axes = plt.subplots(1, 2, figsize=(15, 5))
+    axes[0] = sns.heatmap(cm, annot=True, cmap="Blues", fmt="d", ax=axes[0])
+    axes[1] = sns.heatmap(cm_n, annot=True, cmap="Blues", fmt=".2%", ax=axes[1])
+    for ax in axes:
+        ax.set_xlabel("Predicted")
+        ax.set_ylabel("True")
+        ax.xaxis.set_ticklabels(class_names)
+        ax.yaxis.set_ticklabels(class_names)
+    return fig
+
+
 def resize_and_save(width_inch: int, height_inch: int, filename: Union[Path, str], dpi: int = 150) -> None:
     """
     Resizes the present figure to the given (width, height) in inches, and saves it to the given filename.
+
     :param width_inch: The width of the figure in inches.
     :param height_inch: The height of the figure in inches.
     :param filename: The filename to save to.
     :param dpi: Image resolution in dots per inch
     """
     fig = plt.gcf()
     fig.set_size_inches(width_inch, height_inch)
```

### Comparing `hi-ml-cpath-0.2.9/src/hi_ml_cpath.egg-info/PKG-INFO` & `hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-cpath
-Version: 0.2.9
+Version: 0.3.0
 Summary: Microsoft Health Futures package for deep learning on histopathology images
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Keywords: Health Futures,Health Intelligence,Computational Pathology,AzureML
 Platform: UNKNOWN
```

### Comparing `hi-ml-cpath-0.2.9/src/hi_ml_cpath.egg-info/SOURCES.txt` & `hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,30 +18,39 @@
 src/health_cpath/datasets/tcga_prad_dataset.py
 src/health_cpath/models/deepmil.py
 src/health_cpath/models/encoders.py
 src/health_cpath/models/transforms.py
 src/health_cpath/preprocessing/create_panda_tiles_dataset.py
 src/health_cpath/preprocessing/create_tiles_dataset.py
 src/health_cpath/preprocessing/loading.py
+src/health_cpath/preprocessing/tiff_conversion.py
 src/health_cpath/preprocessing/tiling.py
 src/health_cpath/scripts/aggregate_metrics_crossvalidation.py
+src/health_cpath/scripts/create_montage.py
+src/health_cpath/scripts/generate_checkpoint_url.py
 src/health_cpath/scripts/generate_crossval_report.py
 src/health_cpath/scripts/mount_azure_dataset.py
 src/health_cpath/scripts/tcga_dataset_prep.py
+src/health_cpath/utils/__init__.py
 src/health_cpath/utils/analysis_plot_utils.py
+src/health_cpath/utils/callbacks.py
 src/health_cpath/utils/deepmil_utils.py
 src/health_cpath/utils/download_utils.py
 src/health_cpath/utils/girder.py
 src/health_cpath/utils/heatmap_utils.py
 src/health_cpath/utils/layer_utils.py
+src/health_cpath/utils/montage.py
+src/health_cpath/utils/montage_config.py
 src/health_cpath/utils/naming.py
 src/health_cpath/utils/output_utils.py
+src/health_cpath/utils/package_setup.py
 src/health_cpath/utils/plots_utils.py
 src/health_cpath/utils/report_utils.py
 src/health_cpath/utils/tcga_utils.py
+src/health_cpath/utils/tiff_conversion_config.py
 src/health_cpath/utils/tiles_selection_utils.py
 src/health_cpath/utils/viz_utils.py
 src/health_cpath/utils/wsi_utils.py
 src/hi_ml_cpath.egg-info/PKG-INFO
 src/hi_ml_cpath.egg-info/SOURCES.txt
 src/hi_ml_cpath.egg-info/dependency_links.txt
 src/hi_ml_cpath.egg-info/requires.txt
```

