# Comparing `tmp/lightwood-23.4.3.0.tar.gz` & `tmp/lightwood-23.5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lightwood-23.4.3.0.tar", last modified: Wed Apr 19 01:28:40 2023, max compression
+gzip compressed data, was "lightwood-23.5.1.0.tar", last modified: Sun May  7 10:11:05 2023, max compression
```

## Comparing `lightwood-23.4.3.0.tar` & `lightwood-23.5.1.0.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/explain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/acc_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/conf_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/pyod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/analysis/nc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/analysis/nn_conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nn_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nn_conf/temp_scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/api/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    50128 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/json_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/data/encoded_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/data/timeseries_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/data/timeseries_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/array/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/array/ts_cat_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/array/ts_num_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/audio/mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/multihot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/onehot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/datetime/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/identity/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/image/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/image/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/image/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/image/helpers/img_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/image/img_2_vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/numeric/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/numeric/ts_numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/text/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/text/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/helpers/pretrained_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/short.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/best_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/mode_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/ts_stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/weighted_mean_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/ets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/ar_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/default_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/qclassic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/residual_net.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/lightgbm_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/neural.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/neural_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/qclassic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/sktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-04-19 01:28:39.000000 lightwood-23.4.3.0/lightwood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 01:28:39.000000 lightwood-23.4.3.0/lightwood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-19 01:28:39.000000 lightwood-23.4.3.0/lightwood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 01:28:39.000000 lightwood-23.4.3.0/lightwood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-05-07 10:10:52.000000 lightwood-23.5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 10:10:52.000000 lightwood-23.5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-05-07 10:10:52.000000 lightwood-23.5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.380733 lightwood-23.5.1.0/lightwood/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/analysis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/acc_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/conf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/pyod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/analysis/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/analysis/nn_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nn_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nn_conf/temp_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50128 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/json_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/data/encoded_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/data/timeseries_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/data/timeseries_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/array/ts_cat_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/array/ts_num_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/audio/mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/multihot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/onehot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/datetime/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/identity/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/image/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/image/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/image/helpers/img_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/image/img_2_vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/numeric/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/numeric/ts_numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/text/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.392734 lightwood-23.5.1.0/lightwood/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/best_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/mode_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/ts_stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/weighted_mean_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.392734 lightwood-23.5.1.0/lightwood/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/lightwood/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/ets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/lightwood/mixer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/ar_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/default_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/qclassic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/residual_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/lightgbm_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/neural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/neural_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/qclassic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/sktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lightwood-23.4.3.0/PKG-INFO` & `lightwood-23.5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.4.3.0
+Version: 23.5.1.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -125,15 +125,15 @@
         pip3 install lightwood
         ```
         >Note: depending on your environment, you might have to use pip instead of pip3 in the above command.
         
         However, we recommend creating a python virtual environment.
         
         #### Setting up a dev environment
-        - Python version should be in the range >=3.7, < 3.10
+        - Python version should be in the range >=3.8, < 3.11
         - Clone lightwood
         - `cd lightwood && pip install -r requirements.txt && pip install -r requirements_image.txt`
         - Add it to your python path (e.g. by adding `export PYTHONPATH='/where/you/cloned/lightwood':$PYTHONPATH` as a newline at the end of your `~/.bashrc` file)
         - Check that the `unittest`s are passing by going into the directory where you cloned lightwood and running: `python -m unittest discover tests` 
         
         > If `python` default to python2.x on your environment use `python3` and `pip3` instead
         
@@ -214,17 +214,17 @@
         * [Lightwood License](https://github.com/mindsdb/lightwood/blob/master/LICENSE)
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: extra_ts
+Provides-Extra: image
 Provides-Extra: quantum
-Provides-Extra: audio
 Provides-Extra: extra
-Provides-Extra: image
+Provides-Extra: audio
+Provides-Extra: extra_ts
 Provides-Extra: xai
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.4.3.0/README.md` & `lightwood-23.5.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 pip3 install lightwood
 ```
 >Note: depending on your environment, you might have to use pip instead of pip3 in the above command.
 
 However, we recommend creating a python virtual environment.
 
 #### Setting up a dev environment
-- Python version should be in the range >=3.7, < 3.10
+- Python version should be in the range >=3.8, < 3.11
 - Clone lightwood
 - `cd lightwood && pip install -r requirements.txt && pip install -r requirements_image.txt`
 - Add it to your python path (e.g. by adding `export PYTHONPATH='/where/you/cloned/lightwood':$PYTHONPATH` as a newline at the end of your `~/.bashrc` file)
 - Check that the `unittest`s are passing by going into the directory where you cloned lightwood and running: `python -m unittest discover tests` 
 
 > If `python` default to python2.x on your environment use `python3` and `pip3` instead
```

### Comparing `lightwood-23.4.3.0/lightwood/analysis/__init__.py` & `lightwood-23.5.1.0/lightwood/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/analyze.py` & `lightwood-23.5.1.0/lightwood/analysis/analyze.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/base.py` & `lightwood-23.5.1.0/lightwood/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/explain.py` & `lightwood-23.5.1.0/lightwood/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/helpers/acc_stats.py` & `lightwood-23.5.1.0/lightwood/analysis/helpers/acc_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/helpers/conf_stats.py` & `lightwood-23.5.1.0/lightwood/analysis/helpers/conf_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/helpers/feature_importance.py` & `lightwood-23.5.1.0/lightwood/analysis/helpers/feature_importance.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/helpers/pyod.py` & `lightwood-23.5.1.0/lightwood/analysis/helpers/pyod.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/helpers/shap.py` & `lightwood-23.5.1.0/lightwood/analysis/helpers/shap.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/nc/base.py` & `lightwood-23.5.1.0/lightwood/analysis/nc/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/nc/calibrate.py` & `lightwood-23.5.1.0/lightwood/analysis/nc/calibrate.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/nc/icp.py` & `lightwood-23.5.1.0/lightwood/analysis/nc/icp.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/nc/metrics.py` & `lightwood-23.5.1.0/lightwood/analysis/nc/metrics.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/nc/nc.py` & `lightwood-23.5.1.0/lightwood/analysis/nc/nc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/nc/norm.py` & `lightwood-23.5.1.0/lightwood/analysis/nc/norm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/nc/util.py` & `lightwood-23.5.1.0/lightwood/analysis/nc/util.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/analysis/nn_conf/temp_scale.py` & `lightwood-23.5.1.0/lightwood/analysis/nn_conf/temp_scale.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/api/__init__.py` & `lightwood-23.5.1.0/lightwood/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/api/high_level.py` & `lightwood-23.5.1.0/lightwood/api/high_level.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/api/json_ai.py` & `lightwood-23.5.1.0/lightwood/api/json_ai.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/api/predictor.py` & `lightwood-23.5.1.0/lightwood/api/predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 # Interface that must be respected by predictor objects generated from JSON ML and/or compatible with Mindsdb
 class PredictorInterface:
     """
     Abstraction of a Lightwood predictor. The ``PredictorInterface`` encompasses how Lightwood interacts with the full ML pipeline. Internally,
 
     The ``PredictorInterface`` class must have several expected functions:
-    
+
     - ``analyze_data``: Peform a statistical analysis on the unprocessed data; this helps inform downstream encoders and mixers on how to treat the data types.
     - ``preprocess``: Apply cleaning functions to each of the columns within the dataset to prepare them for featurization
     - ``split``: Split the input dataset into a train/dev/test set according to your splitter function
     - ``prepare``: Create and, if necessary, train your encoders to create feature representations from each column of your data.
     - ``featurize``: For input, pre-processed data, create feature vectors
     - ``fit``: Train your mixer models to yield predictions from featurized data
     - ``analyze_ensemble``: Evaluate the quality of fit for your mixer models
     - ``adjust``: Incorporate new data to update pre-existing model(s).
 
     For simplification, we offer an end-to-end approach that allows you to input raw data and follow every step of the process until you reach a trained predictor with the ``learn`` function:
 
         - ``learn``: An end-to-end technique specifying how to pre-process, featurize, and train the model(s) of interest. The expected input is raw, untrained data. No explicit output is provided, but the Predictor object will "host" the trained model thus.
-    
+
     You can also use the predictor to now estimate new data:
 
     - ``predict``: Deploys the chosen best model, and evaluates the given data to provide target estimates.
     - ``save``: Saves the Predictor object for further use.
 
     The ``PredictorInterface`` is created via J{ai}son's custom code creation. A problem inherits from this class with pre-populated routines to fill out expected results, given the nature of each problem type.
     """ # noqa
@@ -81,15 +81,15 @@
 
         :returns: For each dataset provided in ``split_data``, the encoded representations of the data.
         """ # noqa
         pass
 
     def fit(self, enc_data: Dict[str, pd.DataFrame]) -> None:
         """
-        Fits "mixer" models to train predictors on the featurized data. Instantiates a set of trained mixers and an ensemble of them. 
+        Fits "mixer" models to train predictors on the featurized data. Instantiates a set of trained mixers and an ensemble of them.
 
         :param enc_data: Pre-processed and featurized data, split into the relevant train/test splits. Keys expected are "train", "dev", and "test"
         """  # noqa
         pass
 
     def analyze_ensemble(self, enc_data: Dict[str, pd.DataFrame]) -> None:
         """
@@ -99,28 +99,28 @@
         """
         pass
 
     def learn(self, data: pd.DataFrame) -> None:
         """
         Trains the attribute model starting from raw data. Raw data is pre-processed and cleaned accordingly. As data is assigned a particular type (ex: numerical, categorical, etc.), the respective feature encoder will convert it into a representation useable for training ML models. Of all ML models requested, these models are compiled and fit on the training data.
 
-        This step amalgates ``preprocess`` -> ``featurize`` -> ``fit`` with the necessary splitting + analyze_data that occurs. 
+        This step amalgates ``preprocess`` -> ``featurize`` -> ``fit`` with the necessary splitting + analyze_data that occurs.
 
         :param data: (Unprocessed) Data used in training the model(s).
 
         :returns: Nothing; instantiates with best fit model from ensemble.
         """  # noqa
         pass
 
     def adjust(self, new_data: pd.DataFrame, old_data: Optional[pd.DataFrame] = None, adjust_args: Optional[dict] = None
                ) -> None:
         """
         Adjusts a previously trained model on new data. Adopts the same process as ``learn`` but with the exception that the `adjust` function expects the best model to have been already trained.
 
-        .. warning:: This is experimental and subject to change. 
+        .. warning:: This is experimental and subject to change.
         :param new_data: New data used to adjust a previously trained model.
         :param old_data: In some situations, the old data is still required to train a model (i.e. Regression mixer) to ensure the new data doesn't entirely override it.
         :param adjust_args: Optional dictionary with parameters to customize the finetuning process.
 
         :returns: Adjusts best-fit model in-place, doesn't return anything.
         """  # noqa
         pass
@@ -135,14 +135,29 @@
         :returns: A dataframe of predictions of the same length of input.
         """  # noqa
         pass
 
     def save(self, file_path: str) -> None:
         """
         With a provided file path, saves the Predictor instance for later use.
+        :param file_path: Location to store your Predictor Instance.
+        :returns: Saves Predictor instance.
+        """
+        with open(file_path, "wb") as fp:
+            dill.dump(self, fp)
+
+    def export(self, file_path: str, json_ai_code: str) -> None:
+        """
+        Exports both the predictor object and its code to a single binary file for later usage.
 
         :param file_path: Location to store your Predictor Instance.
+        :param json_ai_code: The code generated by the user's specification.
 
         :returns: Saves Predictor instance.
         """
+
+        predictor_dict = {}
+        predictor_dict['predictor'] = self
+        predictor_dict['code'] = json_ai_code
+
         with open(file_path, "wb") as fp:
-            dill.dump(self, fp)
+            dill.dump(predictor_dict, fp)
```

### Comparing `lightwood-23.4.3.0/lightwood/api/types.py` & `lightwood-23.5.1.0/lightwood/api/types.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/data/encoded_ds.py` & `lightwood-23.5.1.0/lightwood/data/encoded_ds.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/data/timeseries_analyzer.py` & `lightwood-23.5.1.0/lightwood/data/timeseries_analyzer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/data/timeseries_transform.py` & `lightwood-23.5.1.0/lightwood/data/timeseries_transform.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/__init__.py` & `lightwood-23.5.1.0/lightwood/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/array/array.py` & `lightwood-23.5.1.0/lightwood/encoder/array/array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/array/ts_cat_array.py` & `lightwood-23.5.1.0/lightwood/encoder/array/ts_cat_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/array/ts_num_array.py` & `lightwood-23.5.1.0/lightwood/encoder/array/ts_num_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/audio/mfcc.py` & `lightwood-23.5.1.0/lightwood/encoder/audio/mfcc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/base.py` & `lightwood-23.5.1.0/lightwood/encoder/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/categorical/autoencoder.py` & `lightwood-23.5.1.0/lightwood/encoder/categorical/autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/categorical/binary.py` & `lightwood-23.5.1.0/lightwood/encoder/categorical/binary.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/categorical/gym.py` & `lightwood-23.5.1.0/lightwood/encoder/categorical/gym.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/categorical/multihot.py` & `lightwood-23.5.1.0/lightwood/encoder/categorical/multihot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/categorical/onehot.py` & `lightwood-23.5.1.0/lightwood/encoder/categorical/onehot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/datetime/datetime.py` & `lightwood-23.5.1.0/lightwood/encoder/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/datetime/datetime_sin_normalizer.py` & `lightwood-23.5.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/helpers.py` & `lightwood-23.5.1.0/lightwood/encoder/helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/identity/identity.py` & `lightwood-23.5.1.0/lightwood/encoder/identity/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/image/helpers/img_to_vec.py` & `lightwood-23.5.1.0/lightwood/encoder/image/helpers/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/image/img_2_vec.py` & `lightwood-23.5.1.0/lightwood/encoder/image/img_2_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/numeric/numeric.py` & `lightwood-23.5.1.0/lightwood/encoder/numeric/numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/numeric/ts_numeric.py` & `lightwood-23.5.1.0/lightwood/encoder/numeric/ts_numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/text/helpers/pretrained_helpers.py` & `lightwood-23.5.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/text/helpers/rnn_helpers.py` & `lightwood-23.5.1.0/lightwood/encoder/text/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/text/pretrained.py` & `lightwood-23.5.1.0/lightwood/encoder/text/pretrained.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/text/rnn.py` & `lightwood-23.5.1.0/lightwood/encoder/text/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/text/short.py` & `lightwood-23.5.1.0/lightwood/encoder/text/short.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/text/tfidf.py` & `lightwood-23.5.1.0/lightwood/encoder/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/text/vocab.py` & `lightwood-23.5.1.0/lightwood/encoder/text/vocab.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/common.py` & `lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/rnn_helpers.py` & `lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/transformer_helpers.py` & `lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/time_series/rnn.py` & `lightwood-23.5.1.0/lightwood/encoder/time_series/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/encoder/time_series/ts.py` & `lightwood-23.5.1.0/lightwood/encoder/time_series/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/ensemble/__init__.py` & `lightwood-23.5.1.0/lightwood/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/ensemble/base.py` & `lightwood-23.5.1.0/lightwood/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/ensemble/best_of.py` & `lightwood-23.5.1.0/lightwood/ensemble/best_of.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/ensemble/mean_ensemble.py` & `lightwood-23.5.1.0/lightwood/ensemble/mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/ensemble/mode_ensemble.py` & `lightwood-23.5.1.0/lightwood/ensemble/mode_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/ensemble/stacked_ensemble.py` & `lightwood-23.5.1.0/lightwood/ensemble/stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/ensemble/ts_stacked_ensemble.py` & `lightwood-23.5.1.0/lightwood/ensemble/ts_stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/ensemble/weighted_mean_ensemble.py` & `lightwood-23.5.1.0/lightwood/ensemble/weighted_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/__init__.py` & `lightwood-23.5.1.0/lightwood/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/device.py` & `lightwood-23.5.1.0/lightwood/helpers/device.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/general.py` & `lightwood-23.5.1.0/lightwood/helpers/general.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/io.py` & `lightwood-23.5.1.0/lightwood/helpers/io.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/log.py` & `lightwood-23.5.1.0/lightwood/helpers/log.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/parallelism.py` & `lightwood-23.5.1.0/lightwood/helpers/parallelism.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/templating.py` & `lightwood-23.5.1.0/lightwood/helpers/templating.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/text.py` & `lightwood-23.5.1.0/lightwood/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/torch.py` & `lightwood-23.5.1.0/lightwood/helpers/torch.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/helpers/ts.py` & `lightwood-23.5.1.0/lightwood/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/__init__.py` & `lightwood-23.5.1.0/lightwood/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/arima.py` & `lightwood-23.5.1.0/lightwood/mixer/arima.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/base.py` & `lightwood-23.5.1.0/lightwood/mixer/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/ets.py` & `lightwood-23.5.1.0/lightwood/mixer/ets.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/gluonts.py` & `lightwood-23.5.1.0/lightwood/mixer/gluonts.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,16 +237,16 @@
 
         ds = PandasDataset.from_long_dataframe(
             df,
             target=self.target,
             item_id=gby,
             freq=freq,
             timestamp=oby_col_name,
-            feat_static_real=self.static_features_real if self.static_features_real else None,
-            feat_static_cat=self.static_features_cat if self.static_features_cat else None,
+            feat_static_real=self.static_features_real if self.static_features_real else [],
+            feat_static_cat=self.static_features_cat if self.static_features_cat else [],
         )
         return ds
 
 
 class EarlyStop(TrainingHistory):
     def __init__(self, patience=3):
         super().__init__()
```

### Comparing `lightwood-23.4.3.0/lightwood/mixer/helpers/ar_net.py` & `lightwood-23.5.1.0/lightwood/mixer/helpers/ar_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/helpers/default_net.py` & `lightwood-23.5.1.0/lightwood/mixer/helpers/default_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/helpers/qclassic_net.py` & `lightwood-23.5.1.0/lightwood/mixer/helpers/qclassic_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/helpers/ranger.py` & `lightwood-23.5.1.0/lightwood/mixer/helpers/ranger.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/helpers/residual_net.py` & `lightwood-23.5.1.0/lightwood/mixer/helpers/residual_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py` & `lightwood-23.5.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/helpers/ts.py` & `lightwood-23.5.1.0/lightwood/mixer/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/lightgbm.py` & `lightwood-23.5.1.0/lightwood/mixer/lightgbm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/lightgbm_array.py` & `lightwood-23.5.1.0/lightwood/mixer/lightgbm_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/neural.py` & `lightwood-23.5.1.0/lightwood/mixer/neural.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/neural_ts.py` & `lightwood-23.5.1.0/lightwood/mixer/neural_ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/nhits.py` & `lightwood-23.5.1.0/lightwood/mixer/nhits.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Union, Optional
 from copy import deepcopy
 
 import numpy as np
 import pandas as pd
-from hyperopt import hp
-import neuralforecast as nf
-from neuralforecast.models.mqnhits.mqnhits import MQNHITS
+from neuralforecast import NeuralForecast
+from neuralforecast.models.nhits import NHITS
+from neuralforecast.losses.pytorch import MQLoss
 
 from lightwood.helpers.log import log
 from lightwood.mixer.base import BaseMixer
 from lightwood.api.types import PredictionArguments
 from lightwood.data.encoded_ds import EncodedDs, ConcatedEncodedDs
 
 
@@ -25,35 +25,41 @@
             self,
             stop_after: float,
             target: str,
             horizon: int,
             window: int,
             dtype_dict: Dict,
             ts_analysis: Dict,
-            pretrained: bool = False
+            pretrained: bool = False,
+            train_args: Optional[Dict] = None,
     ):
         """
-        Wrapper around a MQN-HITS deep learning model.
+        Wrapper around an N-HITS deep learning model.
         
         :param stop_after: time budget in seconds.
         :param target: column to forecast.
         :param horizon: length of forecasted horizon.
         :param window: length of input data.
         :param ts_analysis: dictionary with miscellaneous time series info, as generated by 'lightwood.data.timeseries_analyzer'.
+        :param train_args: arguments to steer the training process. 
+            - `trainer_args`: all arguments for the PyTorchLightning trainer.
+            - `conf_level`: level passed into MQLoss. Directly impacts prediction bounds. 
         """  # noqa
         super().__init__(stop_after)
         self.stable = False
         self.prepared = False
         self.supports_proba = False
         self.target = target
         self.window = window
         self.horizon = horizon
         self.dtype_dict = dtype_dict
         self.ts_analysis = ts_analysis
         self.grouped_by = ['__default'] if not ts_analysis['tss'].group_by else ts_analysis['tss'].group_by
+        self.train_args = train_args.get('trainer_args', {}) if train_args else {}
+        self.conf_level = self.train_args.pop('conf_level', 90)
 
         self.pretrained = pretrained
         self.base_url = 'https://nixtla-public.s3.amazonaws.com/transfer/pretrained_models/'
         self.freq_to_model = {
             'Y': 'yearly',
             'Q': 'monthly',
             'M': 'monthly',
@@ -84,26 +90,25 @@
         gby = self.ts_analysis["tss"].group_by if self.ts_analysis["tss"].group_by else []
         df = deepcopy(cat_ds.data_frame)
         Y_df = self._make_initial_df(df)
         if gby:
             n_time = df[gby].value_counts().min()
         else:
             n_time = len(df[f'__mdb_original_{oby_col}'].unique())
-        n_ts_val = max(int(.1 * n_time), self.horizon)  # at least self.horizon to validate&test on
-        n_ts_test = max(int(.1 * n_time), self.horizon)
+        n_ts_val = max(int(.1 * n_time), self.horizon)  # at least self.horizon to validate on
 
         # train the model
         n_time_out = self.horizon
         if self.pretrained:
             # TODO: let user specify finetuning
             self.model_name = self.model_names.get(self.freq_to_model[self.ts_analysis['sample_freqs']['__default']],
                                                    None)
             self.model_name = self.model_names['hourly'] if self.model_name is None else self.model_name
             ckpt_url = self.base_url + self.model_name
-            self.model = MQNHITS.load_from_checkpoint(ckpt_url)
+            self.model = NHITS.load_from_checkpoint(ckpt_url)
 
             if not self.window < self.model.hparams.n_time_in:
                 log.info(f'NOTE: Provided window ({self.window}) is smaller than specified model input length ({self.model.hparams.n_time_in}). Will train a new model from scratch.')  # noqa
                 self.pretrained = False
             if self.horizon > self.model.hparams.n_time_out:
                 log.info(f'NOTE: Horizon ({self.horizon}) is bigger than that of the pretrained model ({self.model.hparams.n_time_out}). Will train a new model from scratch.')  # noqa
                 self.pretrained = False
@@ -111,45 +116,21 @@
                 log.info(f'Successfully loaded pretrained N-HITS forecasting model ({self.model_name})')
 
         if not self.pretrained:
             if self.window + self.horizon > n_time:
                 new_window = max(1, n_time - self.horizon - 1)
                 self.window = new_window
                 log.info(f'Window {self.window} is too long for data provided (group: {df[gby].value_counts()[::-1].index[0]}), reducing window to {new_window}.')  # noqa
-            self.model = nf.auto.MQNHITS(horizon=n_time_out)
-            self.model.space['max_steps'] = hp.choice('max_steps', [1e4])
-            self.model.space['max_epochs'] = hp.choice('max_epochs', [50])
-            self.model.space['n_time_in'] = hp.choice('n_time_in', [self.window])
-            self.model.space['n_time_out'] = hp.choice('n_time_out', [self.horizon])
-            self.model.space['n_x_hidden'] = hp.choice('n_x_hidden', [0])
-            self.model.space['n_s_hidden'] = hp.choice('n_s_hidden', [0])
-            self.model.space['complete_windows'] = hp.choice('complete_windows', [False])
-            self.model.space['frequency'] = hp.choice('frequency', [self.ts_analysis['sample_freqs']['__default']])
-            self.model.space['random_seed'] = hp.choice('random_seed', [42])
-            self.model.fit(Y_df=Y_df,
-                           X_df=None,       # Exogenous variables
-                           S_df=None,       # Static variables
-                           hyperopt_steps=5,
-                           n_ts_val=n_ts_val,
-                           n_ts_test=n_ts_test,
-                           results_dir='./results/autonhits',
-                           save_trials=False,
-                           loss_function_val=nf.losses.numpy.mqloss,
-                           loss_functions_test={'MQ': nf.losses.numpy.mqloss},
-                           return_test_forecast=False,
-                           verbose=False)
+            model = NHITS(h=n_time_out, input_size=self.window, **self.train_args, loss=MQLoss(level=[self.conf_level]))
+            self.model = NeuralForecast(models=[model], freq=self.ts_analysis['sample_freqs']['__default'])
+            self.model.fit(df=Y_df, val_size=n_ts_val)
             log.info('Successfully trained N-HITS forecasting model.')
 
     def partial_fit(self, train_data: EncodedDs, dev_data: EncodedDs, args: Optional[dict] = None) -> None:
-        """
-        Due to how lightwood implements the `update` procedure, expected inputs for this method are:
-        
-        :param dev_data: original `test` split (used to validate and select model if ensemble is `BestOf`).
-        :param train_data: concatenated original `train` and `dev` splits.
-        """  # noqa
+        # TODO: reimplement this with automatic novel-row differential
         self.hyperparam_search = False
         self.fit(dev_data, train_data)
         self.prepared = True
 
     def __call__(self, ds: Union[EncodedDs, ConcatedEncodedDs],
                  args: PredictionArguments = PredictionArguments()) -> pd.DataFrame:
         """
@@ -167,23 +148,23 @@
                            index=np.arange(length),
                            columns=['prediction', 'lower', 'upper'],
                            dtype=object)
 
         input_df = self._make_initial_df(deepcopy(ds.data_frame))
         ydf['index'] = input_df['index']
 
-        pred_cols = ['y_5', 'y_50', 'y_95']
+        pred_cols = [f'NHITS-lo-{self.conf_level}', 'NHITS-median', f'NHITS-hi-{self.conf_level}']
         target_cols = ['lower', 'prediction', 'upper']
         for target_col in target_cols:
             ydf[target_col] = [[0 for _ in range(self.horizon)] for _ in range(len(ydf))]  # zero-filled arrays
 
         group_ends = []
         for group in input_df['unique_id'].unique():
             group_ends.append(input_df[input_df['unique_id'] == group]['index'].iloc[-1])
-        fcst = self.model.forecast(Y_df=input_df)
+        fcst = self.model.predict(futr_df=input_df).reset_index()
 
         for gidx, group in zip(group_ends, input_df['unique_id'].unique()):
             for pred_col, target_col in zip(pred_cols, target_cols):
                 group_preds = fcst[fcst['unique_id'] == group][pred_col].tolist()[:self.horizon]
                 idx = ydf[ydf['index'] == gidx].index[0]
                 ydf.at[idx, target_col] = group_preds
```

### Comparing `lightwood-23.4.3.0/lightwood/mixer/prophet.py` & `lightwood-23.5.1.0/lightwood/mixer/prophet.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/qclassic.py` & `lightwood-23.5.1.0/lightwood/mixer/qclassic.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/random_forest.py` & `lightwood-23.5.1.0/lightwood/mixer/random_forest.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/regression.py` & `lightwood-23.5.1.0/lightwood/mixer/regression.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/sktime.py` & `lightwood-23.5.1.0/lightwood/mixer/sktime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/tabtransformer.py` & `lightwood-23.5.1.0/lightwood/mixer/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/unit.py` & `lightwood-23.5.1.0/lightwood/mixer/unit.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood/mixer/xgboost.py` & `lightwood-23.5.1.0/lightwood/mixer/xgboost.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.4.3.0/lightwood.egg-info/PKG-INFO` & `lightwood-23.5.1.0/lightwood.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.4.3.0
+Version: 23.5.1.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -125,15 +125,15 @@
         pip3 install lightwood
         ```
         >Note: depending on your environment, you might have to use pip instead of pip3 in the above command.
         
         However, we recommend creating a python virtual environment.
         
         #### Setting up a dev environment
-        - Python version should be in the range >=3.7, < 3.10
+        - Python version should be in the range >=3.8, < 3.11
         - Clone lightwood
         - `cd lightwood && pip install -r requirements.txt && pip install -r requirements_image.txt`
         - Add it to your python path (e.g. by adding `export PYTHONPATH='/where/you/cloned/lightwood':$PYTHONPATH` as a newline at the end of your `~/.bashrc` file)
         - Check that the `unittest`s are passing by going into the directory where you cloned lightwood and running: `python -m unittest discover tests` 
         
         > If `python` default to python2.x on your environment use `python3` and `pip3` instead
         
@@ -214,17 +214,17 @@
         * [Lightwood License](https://github.com/mindsdb/lightwood/blob/master/LICENSE)
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: extra_ts
+Provides-Extra: image
 Provides-Extra: quantum
-Provides-Extra: audio
 Provides-Extra: extra
-Provides-Extra: image
+Provides-Extra: audio
+Provides-Extra: extra_ts
 Provides-Extra: xai
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.4.3.0/lightwood.egg-info/SOURCES.txt` & `lightwood-23.5.1.0/lightwood.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 lightwood/__about__.py
 lightwood/__init__.py
```

### Comparing `lightwood-23.4.3.0/lightwood.egg-info/requires.txt` & `lightwood-23.5.1.0/lightwood.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dataprep_ml==0.0.8
 mindsdb-evaluator>=0.0.7
 numpy
 nltk<3.6,>=3
 python-dateutil>=2.8.1
 pandas<1.5.0,>=1.1.5
 schema>=0.6.8
-torch<1.14.0,>=1.13.0
+torch<2.1,>=2.0.0
 requests>=2.0.0
 transformers
 optuna<2.10.0,>=2.8.0
 scipy>=1.5.4
 psutil>=5.7.0
 setuptools>=21.2.1
 wheel>=0.32.2
@@ -30,44 +30,42 @@
 xgboost<=1.8.0,>=1.6.0
 tab-transformer-pytorch>=0.2.1
 typing-inspect
 six
 regex
 
 [all_extras]
-gluonts<0.12.0,>=0.11.0
-neuralforecast==0.1.0
+pystan==2.19.1.1
+neuralforecast==1.5.0
+shap>=0.40.0
 qiskit==0.31.0
+torchvision<0.11.0,>=0.10.0
 pillow>8.3.1
-prophet==1.1
+librosa==0.8.1
+suod
+mxnet<2.0.0,>=1.6.0
 lightgbm<=3.3.3,>=3.3.0
-pytorch-lightning<1.7.0,>=1.6.0
+gluonts<0.12.0,>=0.11.0
+prophet==1.1
 autopep8>=1.5.7
-mxnet<2.0.0,>=1.6.0
 pyod==1.0.4
-suod
-torchvision<0.11.0,>=0.10.0
-pystan==2.19.1.1
-librosa==0.8.1
-shap>=0.40.0
 
 [audio]
 librosa==0.8.1
 
 [dev]
 autopep8>=1.5.7
 
 [extra]
 lightgbm<=3.3.3,>=3.3.0
 
 [extra_ts]
 pystan==2.19.1.1
 prophet==1.1
-neuralforecast==0.1.0
-pytorch-lightning<1.7.0,>=1.6.0
+neuralforecast==1.5.0
 mxnet<2.0.0,>=1.6.0
 gluonts<0.12.0,>=0.11.0
 
 [image]
 torchvision<0.11.0,>=0.10.0
 pillow>8.3.1
```

### Comparing `lightwood-23.4.3.0/requirements.txt` & `lightwood-23.5.1.0/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dataprep_ml ==0.0.8
 mindsdb-evaluator >=0.0.7
 numpy
 nltk >=3,<3.6
 python-dateutil >=2.8.1
 pandas >=1.1.5, <1.5.0
 schema >=0.6.8
-torch >=1.13.0, <1.14.0
+torch >=2.0.0, <2.1
 requests >=2.0.0
 transformers
 optuna >=2.8.0,<2.10.0
 scipy >=1.5.4
 psutil >=5.7.0
 setuptools >=21.2.1
 wheel >=0.32.2
```

### Comparing `lightwood-23.4.3.0/setup.py` & `lightwood-23.5.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,9 +58,9 @@
     install_requires=requirements,
     extras_require=extra_requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.8"
 )
```

