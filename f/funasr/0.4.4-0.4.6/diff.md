# Comparing `tmp/funasr-0.4.4.tar.gz` & `tmp/funasr-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.4.4.tar", last modified: Thu Apr 27 09:39:42 2023, max compression
+gzip compressed data, was "funasr-0.4.6.tar", last modified: Sun May  7 16:15:07 2023, max compression
```

## Comparing `funasr-0.4.4.tar` & `funasr-0.4.6.tar`

### file list

```diff
@@ -1,413 +1,422 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.585833 funasr-0.4.4/
--rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.4.4/LICENSE
--rw-r--r--   0 zhifu      (502) staff       (20)     8336 2023-04-27 09:39:42.585606 funasr-0.4.4/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7294 2023-04-27 08:40:56.000000 funasr-0.4.4/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.443849 funasr-0.4.4/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.467052 funasr-0.4.4/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21327 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11203 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    37755 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25868 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/bin/asr_inference_paraformer_streaming.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19242 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_paraformer_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32974 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_paraformer_vad_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25051 2023-04-25 05:58:46.000000 funasr-0.4.4/funasr/bin/asr_inference_rnnt.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_uniasr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23931 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/bin/asr_inference_uniasr_vad.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1006 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/asr_train_paraformer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_train_transducer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/asr_train_uniasr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5309 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/bin/diar_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/eend_ola_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-02-11 09:29:33.000000 funasr-0.4.4/funasr/bin/lm_calc_perplexity.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/lm_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-02-11 09:29:33.000000 funasr-0.4.4/funasr/bin/lm_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/modelscope_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/bin/punc_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/punctuation_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11121 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/punctuation_infer_vadrealtime.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/sond_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/sv_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.4.4/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13304 2023-04-25 07:21:40.000000 funasr-0.4.4/funasr/bin/tp_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/tp_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20030 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/vad_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/vad_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11752 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/vad_inference_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.471933 funasr-0.4.4/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/datasets/iterable_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/iterable_dataset_modelscope.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.474213 funasr-0.4.4/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.476467 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8055 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.484380 funasr-0.4.4/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1201 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2318 2023-04-27 08:40:56.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.4.4/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.484829 funasr-0.4.4/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10833 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.504385 funasr-0.4.4/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5091 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.505202 funasr-0.4.4/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.4.4/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.506319 funasr-0.4.4/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.507695 funasr-0.4.4/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.4.4/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.508123 funasr-0.4.4/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.4.4/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.509454 funasr-0.4.4/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.509724 funasr-0.4.4/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.511144 funasr-0.4.4/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3479 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.512455 funasr-0.4.4/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.515723 funasr-0.4.4/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.516370 funasr-0.4.4/funasr/lm/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/lm/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/lm/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/lm/seq_rnn_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/lm/transformer_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.516687 funasr-0.4.4/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2804 2023-03-02 10:32:58.000000 funasr-0.4.4/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.517918 funasr-0.4.4/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.525592 funasr-0.4.4/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.4.4/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.527568 funasr-0.4.4/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7917 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    28528 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    74013 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34815 2023-04-27 08:40:56.000000 funasr-0.4.4/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.531905 funasr-0.4.4/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43611 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.533196 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    54425 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.535636 funasr-0.4.4/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8895 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-02-23 03:32:15.000000 funasr-0.4.4/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.536068 funasr-0.4.4/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.536466 funasr-0.4.4/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3546 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.537483 funasr-0.4.4/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.537815 funasr-0.4.4/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35684 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.538699 funasr-0.4.4/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/preencoder/sinc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.539518 funasr-0.4.4/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.544641 funasr-0.4.4/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    36791 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.546829 funasr-0.4.4/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/beam_search/beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.548818 funasr-0.4.4/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.4.4/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.549496 funasr-0.4.4/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.550891 funasr-0.4.4/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.4.4/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22114 2023-04-25 05:58:46.000000 funasr-0.4.4/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3649 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.552209 funasr-0.4.4/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.553080 funasr-0.4.4/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.554434 funasr-0.4.4/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.555370 funasr-0.4.4/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.555678 funasr-0.4.4/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.555856 funasr-0.4.4/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.556472 funasr-0.4.4/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.4.4/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.557013 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.558512 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.560286 funasr-0.4.4/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      617 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo.py
--rw-r--r--   0 zhifu      (502) staff       (20)      740 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      932 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      383 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      969 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.561196 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8145 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12279 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.563088 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29270 2023-04-25 07:21:40.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9851 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1393 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.565390 funasr-0.4.4/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.566475 funasr-0.4.4/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.570153 funasr-0.4.4/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73890 2023-04-23 09:14:57.000000 funasr-0.4.4/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    60627 2023-04-23 09:14:57.000000 funasr-0.4.4/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.572918 funasr-0.4.4/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.575595 funasr-0.4.4/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3815 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.578633 funasr-0.4.4/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/train/abs_espnet_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.4.4/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    36453 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.585131 funasr-0.4.4/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.4.4/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7735 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13178 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-04-27 09:38:41.000000 funasr-0.4.4/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.444817 funasr-0.4.4/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8336 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    12988 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      838 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-04-27 09:39:42.585881 funasr-0.4.4/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4573 2023-04-25 05:58:46.000000 funasr-0.4.4/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.274291 funasr-0.4.6/
+-rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.4.6/LICENSE
+-rw-r--r--   0 zhifu      (502) staff       (20)     8180 2023-05-07 16:15:07.274079 funasr-0.4.6/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7158 2023-05-07 09:22:42.000000 funasr-0.4.6/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.154762 funasr-0.4.6/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.169813 funasr-0.4.6/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21327 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/asr_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11203 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/asr_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/asr_inference_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    37897 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/bin/asr_inference_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26705 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/bin/asr_inference_paraformer_streaming.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19242 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/asr_inference_paraformer_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32974 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/asr_inference_paraformer_vad_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25051 2023-04-25 05:58:46.000000 funasr-0.4.6/funasr/bin/asr_inference_rnnt.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/asr_inference_uniasr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23931 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/bin/asr_inference_uniasr_vad.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1006 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/bin/asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/bin/asr_train_paraformer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/asr_train_transducer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/bin/asr_train_uniasr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5382 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-03-10 07:21:13.000000 funasr-0.4.6/funasr/bin/diar_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/eend_ola_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-02-11 09:29:33.000000 funasr-0.4.6/funasr/bin/lm_calc_perplexity.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/lm_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-02-11 09:29:33.000000 funasr-0.4.6/funasr/bin/lm_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/bin/modelscope_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-03-10 07:21:13.000000 funasr-0.4.6/funasr/bin/punc_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/punctuation_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11121 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/punctuation_infer_vadrealtime.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/sond_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/sv_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.4.6/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13304 2023-04-25 07:21:40.000000 funasr-0.4.6/funasr/bin/tp_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/tp_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19910 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/bin/vad_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/bin/vad_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11688 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/bin/vad_inference_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.172453 funasr-0.4.6/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.4.6/funasr/datasets/iterable_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/iterable_dataset_modelscope.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.173760 funasr-0.4.6/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.174970 funasr-0.4.6/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9294 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.176891 funasr-0.4.6/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2583 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.4.6/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.177382 funasr-0.4.6/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.6/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10833 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.178478 funasr-0.4.6/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.179211 funasr-0.4.6/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.6/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.4.6/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.4.6/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.180413 funasr-0.4.6/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.6/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.4.6/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.4.6/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.182130 funasr-0.4.6/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.6/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.4.6/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.4.6/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.4.6/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.182637 funasr-0.4.6/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.6/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.4.6/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.184340 funasr-0.4.6/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-05-05 07:04:25.000000 funasr-0.4.6/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.184689 funasr-0.4.6/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.6/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.4.6/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.186514 funasr-0.4.6/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3479 2023-03-29 08:06:18.000000 funasr-0.4.6/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.187751 funasr-0.4.6/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.191006 funasr-0.4.6/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.4.6/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.191884 funasr-0.4.6/funasr/lm/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/lm/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/lm/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/lm/seq_rnn_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/lm/transformer_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.192249 funasr-0.4.6/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2804 2023-03-02 10:32:58.000000 funasr-0.4.6/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.193945 funasr-0.4.6/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.201411 funasr-0.4.6/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.4.6/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.203940 funasr-0.4.6/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7917 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    28528 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    74013 2023-04-27 09:38:10.000000 funasr-0.4.6/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34815 2023-04-27 08:40:56.000000 funasr-0.4.6/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.208776 funasr-0.4.6/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43611 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.4.6/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.4.6/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.4.6/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-02-16 09:30:51.000000 funasr-0.4.6/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.211100 funasr-0.4.6/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.4.6/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.4.6/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.4.6/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    54458 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.214739 funasr-0.4.6/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8895 2023-02-16 09:30:51.000000 funasr-0.4.6/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-02-23 03:32:15.000000 funasr-0.4.6/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.215384 funasr-0.4.6/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.215800 funasr-0.4.6/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3546 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.216519 funasr-0.4.6/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.216858 funasr-0.4.6/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35684 2023-04-27 09:38:10.000000 funasr-0.4.6/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.218044 funasr-0.4.6/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/preencoder/sinc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.218785 funasr-0.4.6/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.224897 funasr-0.4.6/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    36791 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.226106 funasr-0.4.6/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/beam_search/beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.228297 funasr-0.4.6/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.4.6/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.229388 funasr-0.4.6/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.4.6/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.4.6/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.231011 funasr-0.4.6/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.4.6/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.4.6/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22114 2023-04-25 05:58:46.000000 funasr-0.4.6/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3649 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.233148 funasr-0.4.6/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.234386 funasr-0.4.6/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.235619 funasr-0.4.6/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.236604 funasr-0.4.6/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.236822 funasr-0.4.6/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.6/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.236985 funasr-0.4.6/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.6/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.237661 funasr-0.4.6/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.4.6/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.238335 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.240432 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.242334 funasr-0.4.6/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      617 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/demo.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      740 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      932 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      383 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      969 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.243258 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8145 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12279 2023-05-05 07:04:25.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.245610 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9851 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1393 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.247854 funasr-0.4.6/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.249145 funasr-0.4.6/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.252648 funasr-0.4.6/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    74081 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    60767 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.256084 funasr-0.4.6/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.259690 funasr-0.4.6/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.262838 funasr-0.4.6/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/train/abs_espnet_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.4.6/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    37188 2023-05-07 09:22:42.000000 funasr-0.4.6/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.271368 funasr-0.4.6/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.4.6/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.4.6/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.4.6/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.4.6/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.4.6/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7735 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13178 2023-04-12 07:23:40.000000 funasr-0.4.6/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.4.6/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.4.6/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-05-07 16:14:29.000000 funasr-0.4.6/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.155667 funasr-0.4.6/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8180 2023-05-07 16:15:07.000000 funasr-0.4.6/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    13306 2023-05-07 16:15:07.000000 funasr-0.4.6/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-07 16:15:07.000000 funasr-0.4.6/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      838 2023-05-07 16:15:07.000000 funasr-0.4.6/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-05-07 16:15:07.000000 funasr-0.4.6/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-07 16:15:07.274350 funasr-0.4.6/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4573 2023-04-25 05:58:46.000000 funasr-0.4.6/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-07 16:15:07.273666 funasr-0.4.6/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    25268 2023-04-17 03:36:48.000000 funasr-0.4.6/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.4.6/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.4.6/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.4.6/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.4.6/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.4.6/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.4.4/LICENSE` & `funasr-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/PKG-INFO` & `funasr-0.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.4.4
+Version: 0.4.6
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -37,30 +36,30 @@
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
-| [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
+| [**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
+| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
 We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
-- We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
+- We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - Compared to [Espnet](https://github.com/espnet/espnet) framework, the training speed of large-scale datasets in FunASR is much faster owning to the optimized dataloader.
 
 ## Installation
 
 Install from pip
@@ -84,20 +83,16 @@
 
 ```shell
 pip install -U modelscope
 # For the users in China, you could install with the command:
 # pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
-For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation.html)
+For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
 
-[//]: # ()
-[//]: # (## Usage)
-
-[//]: # (For users who are new to FunASR and ModelScope, please refer to FunASR Docs&#40;[CN]&#40;https://alibaba-damo-academy.github.io/FunASR/cn/index.html&#41; / [EN]&#40;https://alibaba-damo-academy.github.io/FunASR/en/index.html&#41;&#41;)
 
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
 
@@ -140,9 +135,7 @@
 @inproceedings{Shi2023AchievingTP,
   title={Achieving Timestamp Prediction While Recognizing with Non-Autoregressive End-to-End ASR Model},
   author={Xian Shi and Yanni Chen and Shiliang Zhang and Zhijie Yan},
   booktitle={arXiv preprint arXiv:2301.12343}
   year={2023}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.4.4 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.4.6 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
-License Platform: UNKNOWN Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
-Research Classifier: Operating System :: POSIX :: Linux Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown Provides-Extra: train Provides-Extra:
-recipe Provides-Extra: all Provides-Extra: test Provides-Extra: doc License-
-File: LICENSE [//]: # (
+License Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
+System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
+Provides-Extra: train Provides-Extra: recipe Provides-Extra: all Provides-
+Extra: test Provides-Extra: doc License-File: LICENSE [//]: # (
 [docs/images/funasr_logo.jpg]
 ) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
-[**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/
+[**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
-Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
+Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
 modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
 (https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
 meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
 Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
 announce that the M2MeT2.0 challenge will be held in the near future. The
 baseline system is conducted on FunASR and is provided as a receipe of
 AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
@@ -43,41 +42,40 @@
 (https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
 notes For the release notes, please ref to [news](https://github.com/alibaba-
 damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
 recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
 Restoration, Language Models, Speaker Verification and Speaker diarization. -
 We have released large number of academic and industrial pretrained models on
 [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition) - The pretrained model [Paraformer-large](https://
-www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
-vocab8404-pytorch/summary) obtains the best performance on many tasks in
-[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
-supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
-(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
-Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
-speed of large-scale datasets in FunASR is much faster owning to the optimized
-dataloader. ## Installation Install from pip ```shell pip install -U funasr #
-For the users in China, you could install with the command: # pip install -
-U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
-source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
-pip install -e ./ # For the users in China, you could install with the command:
-# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
-want to use the pretrained models in ModelScope, you should install the
-modelscope: ```shell pip install -U modelscope # For the users in China, you
-could install with the command: # pip install -U modelscope -f https://
-modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
-[installation](https://alibaba-damo-academy.github.io/FunASR/en/
-installation.html) [//]: # () [//]: # (## Usage) [//]: # (For users who are new
-to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-
-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-
-academy.github.io/FunASR/en/index.html))) ## Contact If you have any questions
-about FunASR, please contact us by - email: [funasr@list.alibaba-inc.com]
-(funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:--------
----------------------------------------------:| |
+recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/
+FunASR/blob/main/docs/model_zoo/modelscope_models.md) - The pretrained model
+[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
+large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
+performance on many tasks in [SpeechIO leaderboard](https://github.com/
+SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
+pretrained models from [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
+github.com/espnet/espnet) framework, the training speed of large-scale datasets
+in FunASR is much faster owning to the optimized dataloader. ## Installation
+Install from pip ```shell pip install -U funasr # For the users in China, you
+could install with the command: # pip install -U funasr -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
+clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
+For the users in China, you could install with the command: # pip install -e ./
+-i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
+pretrained models in ModelScope, you should install the modelscope: ```shell
+pip install -U modelscope # For the users in China, you could install with the
+command: # pip install -U modelscope -f https://modelscope.oss-cn-
+beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
+simple ``` For more details, please ref to [installation](https://alibaba-damo-
+academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
+have any questions about FunASR, please contact us by - email:
+[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
+Wechat group | |:---:|:-----------------------------------------------------:
+| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.4.4/README.md` & `funasr-0.4.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
-| [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
+| [**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
+| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
 We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
-- We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
+- We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - Compared to [Espnet](https://github.com/espnet/espnet) framework, the training speed of large-scale datasets in FunASR is much faster owning to the optimized dataloader.
 
 ## Installation
 
 Install from pip
@@ -56,20 +56,16 @@
 
 ```shell
 pip install -U modelscope
 # For the users in China, you could install with the command:
 # pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
-For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation.html)
+For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
 
-[//]: # ()
-[//]: # (## Usage)
-
-[//]: # (For users who are new to FunASR and ModelScope, please refer to FunASR Docs&#40;[CN]&#40;https://alibaba-damo-academy.github.io/FunASR/cn/index.html&#41; / [EN]&#40;https://alibaba-damo-academy.github.io/FunASR/en/index.html&#41;&#41;)
 
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
```

#### html2text {}

```diff
@@ -9,19 +9,19 @@
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
-[**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/
+[**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
-Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
+Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
 modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
 (https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
 meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
 Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
 announce that the M2MeT2.0 challenge will be held in the near future. The
 baseline system is conducted on FunASR and is provided as a receipe of
 AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
@@ -29,41 +29,40 @@
 (https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
 notes For the release notes, please ref to [news](https://github.com/alibaba-
 damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
 recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
 Restoration, Language Models, Speaker Verification and Speaker diarization. -
 We have released large number of academic and industrial pretrained models on
 [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition) - The pretrained model [Paraformer-large](https://
-www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
-vocab8404-pytorch/summary) obtains the best performance on many tasks in
-[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
-supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
-(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
-Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
-speed of large-scale datasets in FunASR is much faster owning to the optimized
-dataloader. ## Installation Install from pip ```shell pip install -U funasr #
-For the users in China, you could install with the command: # pip install -
-U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
-source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
-pip install -e ./ # For the users in China, you could install with the command:
-# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
-want to use the pretrained models in ModelScope, you should install the
-modelscope: ```shell pip install -U modelscope # For the users in China, you
-could install with the command: # pip install -U modelscope -f https://
-modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
-[installation](https://alibaba-damo-academy.github.io/FunASR/en/
-installation.html) [//]: # () [//]: # (## Usage) [//]: # (For users who are new
-to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-
-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-
-academy.github.io/FunASR/en/index.html))) ## Contact If you have any questions
-about FunASR, please contact us by - email: [funasr@list.alibaba-inc.com]
-(funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:--------
----------------------------------------------:| |
+recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/
+FunASR/blob/main/docs/model_zoo/modelscope_models.md) - The pretrained model
+[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
+large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
+performance on many tasks in [SpeechIO leaderboard](https://github.com/
+SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
+pretrained models from [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
+github.com/espnet/espnet) framework, the training speed of large-scale datasets
+in FunASR is much faster owning to the optimized dataloader. ## Installation
+Install from pip ```shell pip install -U funasr # For the users in China, you
+could install with the command: # pip install -U funasr -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
+clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
+For the users in China, you could install with the command: # pip install -e ./
+-i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
+pretrained models in ModelScope, you should install the modelscope: ```shell
+pip install -U modelscope # For the users in China, you could install with the
+command: # pip install -U modelscope -f https://modelscope.oss-cn-
+beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
+simple ``` For more details, please ref to [installation](https://alibaba-damo-
+academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
+have any questions about FunASR, please contact us by - email:
+[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
+Wechat group | |:---:|:-----------------------------------------------------:
+| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.4.4/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.4.6/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_inference.py` & `funasr-0.4.6/funasr/bin/asr_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_launch.py` & `funasr-0.4.6/funasr/bin/asr_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_mfcca.py` & `funasr-0.4.6/funasr/bin/asr_inference_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_paraformer.py` & `funasr-0.4.6/funasr/bin/asr_inference_paraformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
+from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
 from funasr.utils.timestamp_tools import ts_prediction_lfr6_standard
 from funasr.bin.tp_inference import SpeechText2Timestamp
 
 
 class Speech2Text:
     """Speech2Text class
@@ -232,15 +233,15 @@
 
         predictor_outs = self.asr_model.calc_predictor(enc, enc_len)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
                                                                         predictor_outs[2], predictor_outs[3]
         pre_token_length = pre_token_length.round().long()
         if torch.max(pre_token_length) < 1:
             return []
-        if not isinstance(self.asr_model, ContextualParaformer):
+        if not isinstance(self.asr_model, ContextualParaformer) and not isinstance(self.asr_model, NeatContextualParaformer):
             if self.hotword_list:
                 logging.warning("Hotword is given but asr model is not a ContextualParaformer.")
             decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length)
             decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
         else:
             decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length, hw_list=self.hotword_list)
             decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
```

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_paraformer_streaming.py` & `funasr-0.4.6/funasr/bin/asr_inference_paraformer_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Union
 from typing import Dict
 from typing import Any
 from typing import List
 
 import numpy as np
 import torch
+import torchaudio
 from typeguard import check_argument_types
 
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
 from funasr.modules.beam_search.beam_search import Hypothesis
 from funasr.modules.scorers.ctc import CTCPrefixScorer
 from funasr.modules.scorers.length_bonus import LengthBonus
@@ -200,17 +201,20 @@
                 text, token, token_int, hyp
 
         """
         assert check_argument_types()
         results = []
         cache_en = cache["encoder"]
         if speech.shape[1] < 16 * 60 and cache_en["is_final"]:
+            if cache_en["start_idx"] == 0:
+                return []
             cache_en["tail_chunk"] = True
             feats = cache_en["feats"]
             feats_len = torch.tensor([feats.shape[1]])
+            self.asr_model.frontend = None
             results = self.infer(feats, feats_len, cache)
             return results
         else:
             if self.frontend is not None:
                 feats, feats_len = self.frontend.forward(speech, speech_lengths, cache_en["is_final"])
                 feats = to_device(feats, device=self.device)
                 feats_len = feats_len.int()
@@ -231,15 +235,15 @@
 
                         # last chunk
                         cache_en["last_chunk"] = True
                         feats_chunk2 = feats[:, -(feats.shape[1] + cache_en["chunk_size"][2] - cache_en["chunk_size"][1]):, :]
                         feats_len = torch.tensor([feats_chunk2.shape[1]])
                         results_chunk2 = self.infer(feats_chunk2, feats_len, cache)
 
-                        return ["".join(results_chunk1 + results_chunk2)]
+                        return [" ".join(results_chunk1 + results_chunk2)]
 
                 results = self.infer(feats, feats_len, cache)
 
         return results
 
     @torch.no_grad()
     def infer(self, feats: Union[torch.Tensor], feats_len: Union[torch.Tensor], cache: List = None):
@@ -291,20 +295,17 @@
                     token_int = hyp.yseq[1:last_pos].tolist()
 
                 # remove blank symbol id, which is assumed to be 0
                 token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
 
                 # Change integer-ids to tokens
                 token = self.converter.ids2tokens(token_int)
+                token = " ".join(token)
 
-                if self.tokenizer is not None:
-                    text = self.tokenizer.tokens2text(token)
-                else:
-                    text = None
-                results.append(text)
+                results.append(token)
 
         # assert check_return_type(results)
         return results
 
 
 def inference(
         maxlenratio: float,
@@ -511,14 +512,16 @@
             **kwargs,
     ):
 
         # 3. Build data-iterator
         if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "bytes":
             raw_inputs = _load_bytes(data_path_and_name_and_type[0])
             raw_inputs = torch.tensor(raw_inputs)
+        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "sound":
+            raw_inputs = torchaudio.load(data_path_and_name_and_type[0])[0][0]
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, np.ndarray):
                 raw_inputs = torch.tensor(raw_inputs)
         is_final = False
         cache = {}
         chunk_size = [5, 10, 5]
         if param_dict is not None and "cache" in param_dict:
@@ -527,21 +530,40 @@
             is_final = param_dict["is_final"]
         if param_dict is not None and "chunk_size" in param_dict:
             chunk_size = param_dict["chunk_size"]
 
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         raw_inputs = torch.unsqueeze(raw_inputs, axis=0)
-        input_lens = torch.tensor([raw_inputs.shape[1]])
         asr_result_list = []
-
         cache = _prepare_cache(cache, chunk_size=chunk_size, batch_size=1)
-        cache["encoder"]["is_final"] = is_final
-        asr_result = speech2text(cache, raw_inputs, input_lens)
-        item = {'key': "utt", 'value': asr_result}
+        item = {}
+        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "sound":
+            sample_offset = 0
+            speech_length = raw_inputs.shape[1]
+            stride_size =  chunk_size[1] * 960
+            cache = _prepare_cache(cache, chunk_size=chunk_size, batch_size=1)
+            final_result = ""
+            for sample_offset in range(0, speech_length, min(stride_size, speech_length - sample_offset)):
+                if sample_offset + stride_size >= speech_length - 1:
+                    stride_size = speech_length - sample_offset
+                    cache["encoder"]["is_final"] = True
+                else:
+                    cache["encoder"]["is_final"] = False
+                input_lens = torch.tensor([stride_size])
+                asr_result = speech2text(cache, raw_inputs[:, sample_offset: sample_offset + stride_size], input_lens)
+                if len(asr_result) != 0: 
+                    final_result += " ".join(asr_result) + " "
+            item = {'key': "utt", 'value': [final_result.strip()]}
+        else:
+            input_lens = torch.tensor([raw_inputs.shape[1]])
+            cache["encoder"]["is_final"] = is_final
+            asr_result = speech2text(cache, raw_inputs, input_lens)
+            item = {'key': "utt", 'value': asr_result}
+
         asr_result_list.append(item)
         if is_final:
             cache = _cache_reset(cache, chunk_size=chunk_size, batch_size=1)
         return asr_result_list
 
     return _forward
 
@@ -721,16 +743,7 @@
     kwargs['param_dict'] = param_dict
     inference(**kwargs)
 
 
 if __name__ == "__main__":
     main()
 
-    # from modelscope.pipelines import pipeline
-    # from modelscope.utils.constant import Tasks
-    #
-    # inference_16k_pipline = pipeline(
-    #     task=Tasks.auto_speech_recognition,
-    #     model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch')
-    #
-    # rec_result = inference_16k_pipline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
-    # print(rec_result)
```

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_paraformer_vad.py` & `funasr-0.4.6/funasr/bin/asr_inference_paraformer_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_paraformer_vad_punc.py` & `funasr-0.4.6/funasr/bin/asr_inference_paraformer_vad_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_rnnt.py` & `funasr-0.4.6/funasr/bin/asr_inference_rnnt.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_uniasr.py` & `funasr-0.4.6/funasr/bin/asr_inference_uniasr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_inference_uniasr_vad.py` & `funasr-0.4.6/funasr/bin/asr_inference_uniasr_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_train.py` & `funasr-0.4.6/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_train_paraformer.py` & `funasr-0.4.6/funasr/bin/asr_train_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_train_transducer.py` & `funasr-0.4.6/funasr/bin/asr_train_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/asr_train_uniasr.py` & `funasr-0.4.6/funasr/bin/asr_train_uniasr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/build_trainer.py` & `funasr-0.4.6/funasr/bin/build_trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,16 @@
     # overwrite parameters
     with open(config) as f:
         configs = yaml.safe_load(f)
     with open(finetune_config) as f:
         finetune_configs = yaml.safe_load(f)
         # set data_types
         if dataset_type == "large":
-            finetune_configs["dataset_conf"]["data_types"] = "sound,text"
+            if 'data_types' not in finetune_configs['dataset_conf']:
+                finetune_configs["dataset_conf"]["data_types"] = "sound,text"
     finetune_configs = update_dct(configs, finetune_configs)
     for key, value in finetune_configs.items():
         if hasattr(args, key):
             setattr(args, key, value)
 
     # prepare data
     args.dataset_type = dataset_type
```

### Comparing `funasr-0.4.4/funasr/bin/data2vec_train.py` & `funasr-0.4.6/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/diar_inference_launch.py` & `funasr-0.4.6/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/diar_train.py` & `funasr-0.4.6/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/eend_ola_inference.py` & `funasr-0.4.6/funasr/bin/eend_ola_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/lm_calc_perplexity.py` & `funasr-0.4.6/funasr/bin/lm_calc_perplexity.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/lm_inference.py` & `funasr-0.4.6/funasr/bin/lm_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/lm_inference_launch.py` & `funasr-0.4.6/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/lm_train.py` & `funasr-0.4.6/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/modelscope_infer.py` & `funasr-0.4.6/funasr/bin/modelscope_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/punc_inference_launch.py` & `funasr-0.4.6/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/punc_train.py` & `funasr-0.4.6/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/punctuation_infer.py` & `funasr-0.4.6/funasr/bin/punctuation_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/punctuation_infer_vadrealtime.py` & `funasr-0.4.6/funasr/bin/punctuation_infer_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/sond_inference.py` & `funasr-0.4.6/funasr/bin/sond_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/sv_inference.py` & `funasr-0.4.6/funasr/bin/sv_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/sv_inference_launch.py` & `funasr-0.4.6/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/tokenize_text.py` & `funasr-0.4.6/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/tp_inference.py` & `funasr-0.4.6/funasr/bin/tp_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/tp_inference_launch.py` & `funasr-0.4.6/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/vad_inference.py` & `funasr-0.4.6/funasr/bin/vad_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,14 @@
             _, results = speech2vadsegment(**batch)
             for i, _ in enumerate(keys):
                 if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
                     results[i] = json.dumps(results[i])
                 item = {'key': keys[i], 'value': results[i]}
                 vad_results.append(item)
                 if writer is not None:
-                    results[i] = json.loads(results[i])
                     ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
         return vad_results
 
     return _forward
 
 def inference_modelscope_online(
@@ -462,15 +461,14 @@
                 for i, _ in enumerate(keys):
                     if results[i]:
                         if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
                             results[i] = json.dumps(results[i])
                         item = {'key': keys[i], 'value': results[i]}
                         vad_results.append(item)
                         if writer is not None:
-                            results[i] = json.loads(results[i])
                             ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
         return vad_results
 
     return _forward
 
 def get_parser():
```

### Comparing `funasr-0.4.4/funasr/bin/vad_inference_launch.py` & `funasr-0.4.6/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/bin/vad_inference_online.py` & `funasr-0.4.6/funasr/bin/vad_inference_online.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,14 @@
                 for i, _ in enumerate(keys):
                     if results[i]:
                         if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
                             results[i] = json.dumps(results[i])
                         item = {'key': keys[i], 'value': results[i]}
                         vad_results.append(item)
                         if writer is not None:
-                            results[i] = json.loads(results[i])
                             ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
         return vad_results
 
     return _forward
```

### Comparing `funasr-0.4.4/funasr/datasets/collate_fn.py` & `funasr-0.4.6/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/dataset.py` & `funasr-0.4.6/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/iterable_dataset.py` & `funasr-0.4.6/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/iterable_dataset_modelscope.py` & `funasr-0.4.6/funasr/datasets/iterable_dataset_modelscope.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.4.6/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.4.6/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.4.6/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/large_datasets/dataset.py` & `funasr-0.4.6/funasr/datasets/large_datasets/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 "The item number of data, data_names, data_types must be the same "
 
             reader_list = []
             for data_file, data_type in zip(data_file_list, data_type_list):
                 if data_type == "kaldi_ark":
                     ark_reader = ReadHelper('ark:{}'.format(data_file))
                     reader_list.append(ark_reader)
-                elif data_type == "text" or data_type == "sound":
+                elif data_type == "text" or data_type == "sound" or data_type == 'text_hotword':
                     text_reader = open(data_file, "r")
                     reader_list.append(text_reader)
                 elif data_type == "none":
                     continue
                 else:
                     raise TypeError("Data type {} is not supported".format(data_type))
 
@@ -127,14 +127,21 @@
                                 sampling_rate = self.frontend_conf["fs"] 
                         waveform = waveform.numpy()
                         mat = waveform[0]
                         sample_dict[data_name] = mat
                         sample_dict["sampling_rate"] = sampling_rate
                         if data_name == "speech":
                             sample_dict["key"] = key
+                    elif data_type == "text_hotword":
+                        text = item
+                        segs = text.strip().split()
+                        sample_dict[data_name] = segs[1:]
+                        if "key" not in sample_dict:
+                            sample_dict["key"] = segs[0]
+                        sample_dict['hw_tag'] = 1
                     else:
                         text = item
                         segs = text.strip().split()
                         sample_dict[data_name] = segs[1:]
                         if "key" not in sample_dict:
                             sample_dict["key"] = segs[0]
                 yield sample_dict
@@ -163,22 +170,46 @@
             frontend_conf,
             mode="train",
             batch_mode="padding"):
     scp_lists = read_lists(data_list_file)
     shuffle = conf.get('shuffle', True)
     data_names = conf.get("data_names", "speech,text")
     data_types = conf.get("data_types", "kaldi_ark,text")
-    dataset = AudioDataset(scp_lists, data_names, data_types, frontend_conf=frontend_conf, shuffle=shuffle, mode=mode)
+
+    pre_hwfile = conf.get("pre_hwlist", None)
+    pre_prob = conf.get("pre_prob", 0)  # unused yet
+
+    hw_config = {"sample_rate": conf.get("sample_rate", 0.6),
+                 "double_rate": conf.get("double_rate", 0.1),
+                 "hotword_min_length": conf.get("hotword_min_length", 2),
+                 "hotword_max_length": conf.get("hotword_max_length", 8),
+                 "pre_prob": conf.get("pre_prob", 0.0)}
+
+    if pre_hwfile is not None:
+        pre_hwlist = []
+        with open(pre_hwfile, 'r') as fin:
+            for line in fin.readlines():
+                pre_hwlist.append(line.strip())
+    else:
+        pre_hwlist = None
+
+    dataset = AudioDataset(scp_lists, 
+                           data_names, 
+                           data_types, 
+                           frontend_conf=frontend_conf, 
+                           shuffle=shuffle, 
+                           mode=mode, 
+                           )
 
     filter_conf = conf.get('filter_conf', {})
     filter_fn = partial(filter, **filter_conf)
     dataset = FilterIterDataPipe(dataset, fn=filter_fn)
 
     if "text" in data_names:
-        vocab = {'vocab': dict, 'seg_dict': seg_dict, 'punc_dict': punc_dict, 'bpe_tokenizer': bpe_tokenizer}
+        vocab = {'vocab': dict, 'seg_dict': seg_dict, 'punc_dict': punc_dict, 'bpe_tokenizer': bpe_tokenizer, 'hw_config': hw_config}
         tokenize_fn = partial(tokenize, **vocab)
         dataset = MapperIterDataPipe(dataset, fn=tokenize_fn)
 
     if shuffle:
         buffer_conf = conf.get('shuffle_conf', {})
         buffer_size = buffer_conf['shuffle_size']
         sort_size = buffer_conf['sort_size']
```

### Comparing `funasr-0.4.4/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.4.6/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.4.6/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.4.6/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.4.6/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 import re
 import numpy as np
+from funasr.datasets.large_datasets.utils.hotword_utils import sample_hotword
 
 def forward_segment(text, seg_dict):
     word_list = []
     i = 0
     while i < len(text):
         longest_word = text[i]
         for j in range(i + 1, len(text) + 1):
@@ -34,29 +35,34 @@
                 out_txt += "<unk>" + " "
     return out_txt.strip().split()
 
 def tokenize(data,
              vocab=None,
              seg_dict=None,
              punc_dict=None,
-             bpe_tokenizer=None):
+             bpe_tokenizer=None,
+             hw_config=None):
     assert "text" in data
     assert isinstance(vocab, dict)
     text = data["text"]
     token = []
     vad = -2
 
     if bpe_tokenizer is not None:
         text = bpe_tokenizer.text2tokens("".join(text))
 
     if seg_dict is not None:
         assert isinstance(seg_dict, dict)
         text = seg_tokenize(text, seg_dict)
 
     length = len(text)
+    if 'hw_tag' in data:
+        hotword_indxs = sample_hotword(length, **hw_config)
+        data['hotword_indxs'] = hotword_indxs
+        del data['hw_tag']
     for i in range(length):
         x = text[i]
         if i == length-1 and "punc" in data and x.startswith("vad:"):
             vad = x[4:]
             if len(vad) == 0:
                 vad = -1
             else:
```

### Comparing `funasr-0.4.4/funasr/datasets/ms_dataset.py` & `funasr-0.4.6/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/datasets/preprocessor.py` & `funasr-0.4.6/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/export_model.py` & `funasr-0.4.6/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/CT_Transformer.py` & `funasr-0.4.6/funasr/export/models/CT_Transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         # mask = self._target_mask(input)
         h, _ = self.encoder(x, text_lengths)
         y = self.decoder(h)
         return y
 
     def get_dummy_inputs(self):
         length = 120
-        text_indexes = torch.randint(0, self.embed.num_embeddings, (2, length))
+        text_indexes = torch.randint(0, self.embed.num_embeddings, (2, length)).type(torch.int32)
         text_lengths = torch.tensor([length-20, length], dtype=torch.int32)
         return (text_indexes, text_lengths)
 
     def get_input_names(self):
         return ['inputs', 'text_lengths']
 
     def get_output_names(self):
@@ -126,15 +126,15 @@
         return y
 
     def with_vad(self):
         return True
 
     def get_dummy_inputs(self):
         length = 120
-        text_indexes = torch.randint(0, self.embed.num_embeddings, (1, length))
+        text_indexes = torch.randint(0, self.embed.num_embeddings, (1, length)).type(torch.int32)
         text_lengths = torch.tensor([length], dtype=torch.int32)
         vad_mask = torch.ones(length, length, dtype=torch.float32)[None, None, :, :]
         sub_masks = torch.ones(length, length, dtype=torch.float32)
         sub_masks = torch.tril(sub_masks).type(torch.float32)
         return (text_indexes, text_lengths, vad_mask, sub_masks[None, None, :, :])
 
     def get_input_names(self):
```

### Comparing `funasr-0.4.4/funasr/export/models/__init__.py` & `funasr-0.4.6/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.4.6/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.4.6/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.4.6/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/e2e_vad.py` & `funasr-0.4.6/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.4.6/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.4.6/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.4.6/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/modules/decoder_layer.py` & `funasr-0.4.6/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/modules/encoder_layer.py` & `funasr-0.4.6/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/modules/feedforward.py` & `funasr-0.4.6/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/modules/multihead_att.py` & `funasr-0.4.6/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/models/predictor/cif.py` & `funasr-0.4.6/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/test/test_onnx.py` & `funasr-0.4.6/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/test/test_onnx_punc.py` & `funasr-0.4.6/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.4.6/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/test/test_onnx_vad.py` & `funasr-0.4.6/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/export/utils/torch_function.py` & `funasr-0.4.6/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/fileio/datadir_writer.py` & `funasr-0.4.6/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/fileio/npy_scp.py` & `funasr-0.4.6/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/fileio/rand_gen_dataset.py` & `funasr-0.4.6/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/fileio/read_text.py` & `funasr-0.4.6/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/fileio/sound_scp.py` & `funasr-0.4.6/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/iterators/chunk_iter_factory.py` & `funasr-0.4.6/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/iterators/multiple_iter_factory.py` & `funasr-0.4.6/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/iterators/sequence_iter_factory.py` & `funasr-0.4.6/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/complex_utils.py` & `funasr-0.4.6/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/global_mvn.py` & `funasr-0.4.6/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/label_aggregation.py` & `funasr-0.4.6/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/log_mel.py` & `funasr-0.4.6/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/mask_along_axis.py` & `funasr-0.4.6/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/sinc_conv.py` & `funasr-0.4.6/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/stft.py` & `funasr-0.4.6/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/time_warp.py` & `funasr-0.4.6/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/layers/utterance_mvn.py` & `funasr-0.4.6/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/lm/abs_model.py` & `funasr-0.4.6/funasr/lm/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/lm/seq_rnn_lm.py` & `funasr-0.4.6/funasr/lm/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/lm/transformer_lm.py` & `funasr-0.4.6/funasr/lm/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/losses/label_smoothing_loss.py` & `funasr-0.4.6/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/main_funcs/average_nbest_models.py` & `funasr-0.4.6/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.4.6/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/main_funcs/collect_stats.py` & `funasr-0.4.6/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/main_funcs/pack_funcs.py` & `funasr-0.4.6/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/ctc.py` & `funasr-0.4.6/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/data2vec.py` & `funasr-0.4.6/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/decoder/contextual_decoder.py` & `funasr-0.4.6/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/decoder/rnn_decoder.py` & `funasr-0.4.6/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.4.6/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/decoder/sanm_decoder.py` & `funasr-0.4.6/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/decoder/sv_decoder.py` & `funasr-0.4.6/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/decoder/transformer_decoder.py` & `funasr-0.4.6/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_asr.py` & `funasr-0.4.6/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_asr_common.py` & `funasr-0.4.6/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_asr_mfcca.py` & `funasr-0.4.6/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_asr_paraformer.py` & `funasr-0.4.6/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_asr_transducer.py` & `funasr-0.4.6/funasr/models/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.4.6/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_diar_sond.py` & `funasr-0.4.6/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_sv.py` & `funasr-0.4.6/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_tp.py` & `funasr-0.4.6/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_uni_asr.py` & `funasr-0.4.6/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/e2e_vad.py` & `funasr-0.4.6/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/conformer_encoder.py` & `funasr-0.4.6/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.4.6/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.4.6/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.4.6/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.4.6/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.4.6/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.4.6/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.4.6/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.4.6/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.4.6/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.4.6/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/rnn_encoder.py` & `funasr-0.4.6/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/encoder/sanm_encoder.py` & `funasr-0.4.6/funasr/models/encoder/sanm_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
                       ):
         xs_pad *= self.output_size() ** 0.5
         if self.embed is None:
             xs_pad = xs_pad
         else:
             xs_pad = self.embed(xs_pad, cache)
         if cache["tail_chunk"]:
-            xs_pad = cache["feats"]
+            xs_pad = to_device(cache["feats"], device=xs_pad.device)
         else:
             xs_pad = self._add_overlap_chunk(xs_pad, cache)
         encoder_outs = self.encoders0(xs_pad, None, None, None, None)
         xs_pad, masks = encoder_outs[0], encoder_outs[1]
         intermediate_outs = []
         if len(self.interctc_layer_idx) == 0:
             encoder_outs = self.encoders(xs_pad, None, None, None, None)
```

### Comparing `funasr-0.4.4/funasr/models/encoder/transformer_encoder.py` & `funasr-0.4.6/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/frontend/default.py` & `funasr-0.4.6/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.4.6/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/frontend/fused.py` & `funasr-0.4.6/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/frontend/s3prl.py` & `funasr-0.4.6/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/frontend/wav_frontend.py` & `funasr-0.4.6/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.4.6/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/frontend/windowing.py` & `funasr-0.4.6/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/joint_net/joint_network.py` & `funasr-0.4.6/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/pooling/statistic_pooling.py` & `funasr-0.4.6/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.4.6/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/predictor/cif.py` & `funasr-0.4.6/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/preencoder/linear.py` & `funasr-0.4.6/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/preencoder/sinc.py` & `funasr-0.4.6/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/specaug/specaug.py` & `funasr-0.4.6/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/target_delay_transformer.py` & `funasr-0.4.6/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/models/vad_realtime_transformer.py` & `funasr-0.4.6/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/add_sos_eos.py` & `funasr-0.4.6/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/attention.py` & `funasr-0.4.6/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.4.6/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.4.6/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/beam_search/beam_search.py` & `funasr-0.4.6/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.4.6/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/data2vec/data_utils.py` & `funasr-0.4.6/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/data2vec/ema_module.py` & `funasr-0.4.6/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.4.6/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/data2vec/quant_noise.py` & `funasr-0.4.6/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/data2vec/utils.py` & `funasr-0.4.6/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.4.6/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/dynamic_conv.py` & `funasr-0.4.6/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/dynamic_conv2d.py` & `funasr-0.4.6/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/e2e_asr_common.py` & `funasr-0.4.6/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/eend_ola/encoder.py` & `funasr-0.4.6/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.4.6/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/embedding.py` & `funasr-0.4.6/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/frontends/beamformer.py` & `funasr-0.4.6/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.4.6/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.4.6/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/frontends/feature_transform.py` & `funasr-0.4.6/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/frontends/frontend.py` & `funasr-0.4.6/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/frontends/mask_estimator.py` & `funasr-0.4.6/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/layer_norm.py` & `funasr-0.4.6/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/lightconv.py` & `funasr-0.4.6/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/lightconv2d.py` & `funasr-0.4.6/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/mask.py` & `funasr-0.4.6/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/multi_layer_conv.py` & `funasr-0.4.6/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/nets_utils.py` & `funasr-0.4.6/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/positionwise_feed_forward.py` & `funasr-0.4.6/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/repeat.py` & `funasr-0.4.6/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/rnn/argument.py` & `funasr-0.4.6/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/rnn/attentions.py` & `funasr-0.4.6/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/rnn/decoders.py` & `funasr-0.4.6/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/rnn/encoders.py` & `funasr-0.4.6/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/scorers/ctc.py` & `funasr-0.4.6/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.4.6/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/scorers/length_bonus.py` & `funasr-0.4.6/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/scorers/scorer_interface.py` & `funasr-0.4.6/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.4.6/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.4.6/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/streaming_utils/utils.py` & `funasr-0.4.6/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/subsampling.py` & `funasr-0.4.6/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/modules/subsampling_without_posenc.py` & `funasr-0.4.6/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/optimizers/fairseq_adam.py` & `funasr-0.4.6/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/optimizers/sgd.py` & `funasr-0.4.6/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/libtorch/demo.py` & `funasr-0.4.6/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.4.6/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/libtorch/setup.py` & `funasr-0.4.6/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/demo.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,18 +225,19 @@
 
         self.output_data_buf = []
         self.output_data_buf_offset = 0
         self.frame_probs = []
         self.max_end_sil_frame_cnt_thresh = self.vad_opts.max_end_silence_time - self.vad_opts.speech_to_sil_time_thres
         self.speech_noise_thres = self.vad_opts.speech_noise_thres
         self.scores = None
+        self.idx_pre_chunk = 0
         self.max_time_out = False
         self.decibel = []
-        self.data_buf = None
-        self.data_buf_all = None
+        self.data_buf_size = 0
+        self.data_buf_all_size = 0
         self.waveform = None
         self.ResetDetection()
 
     def AllResetDetection(self):
         self.is_final = False
         self.data_buf_start_frame = 0
         self.frm_cnt = 0
@@ -255,18 +256,19 @@
 
         self.output_data_buf = []
         self.output_data_buf_offset = 0
         self.frame_probs = []
         self.max_end_sil_frame_cnt_thresh = self.vad_opts.max_end_silence_time - self.vad_opts.speech_to_sil_time_thres
         self.speech_noise_thres = self.vad_opts.speech_noise_thres
         self.scores = None
+        self.idx_pre_chunk = 0
         self.max_time_out = False
         self.decibel = []
-        self.data_buf = None
-        self.data_buf_all = None
+        self.data_buf_size = 0
+        self.data_buf_all_size = 0
         self.waveform = None
         self.ResetDetection()
 
     def ResetDetection(self):
         self.continous_silence_frame_count = 0
         self.latest_confirmed_speech_frame = 0
         self.lastest_confirmed_silence_frame = -1
@@ -276,51 +278,48 @@
         self.windows_detector.Reset()
         self.sil_frame = 0
         self.frame_probs = []
 
     def ComputeDecibel(self) -> None:
         frame_sample_length = int(self.vad_opts.frame_length_ms * self.vad_opts.sample_rate / 1000)
         frame_shift_length = int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000)
-        if self.data_buf_all is None:
-            self.data_buf_all = self.waveform[0]  # self.data_buf is pointed to self.waveform[0]
-            self.data_buf = self.data_buf_all
+        if self.data_buf_all_size == 0:
+            self.data_buf_all_size = len(self.waveform[0])
+            self.data_buf_size = self.data_buf_all_size
         else:
-            self.data_buf_all = np.concatenate((self.data_buf_all, self.waveform[0]))
+            self.data_buf_all_size += len(self.waveform[0])
         for offset in range(0, self.waveform.shape[1] - frame_sample_length + 1, frame_shift_length):
             self.decibel.append(
                 10 * math.log10(np.square((self.waveform[0][offset: offset + frame_sample_length])).sum() + \
                                 0.000001))
 
     def ComputeScores(self, scores: np.ndarray) -> None:
         # scores = self.encoder(feats, in_cache)  # return B * T * D
         self.vad_opts.nn_eval_block_size = scores.shape[1]
         self.frm_cnt += scores.shape[1]  # count total frames
-        if self.scores is None:
-            self.scores = scores  # the first calculation
-        else:
-            self.scores = np.concatenate((self.scores, scores), axis=1)
+        self.scores=scores
 
     def PopDataBufTillFrame(self, frame_idx: int) -> None:  # need check again
         while self.data_buf_start_frame < frame_idx:
-            if len(self.data_buf) >= int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):
+            if self.data_buf_size >= int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):
                 self.data_buf_start_frame += 1
-                self.data_buf = self.data_buf_all[self.data_buf_start_frame * int(
-                    self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):]
+                self.data_buf_size = self.data_buf_all_size-self.data_buf_start_frame * int(
+                    self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000)
 
     def PopDataToOutputBuf(self, start_frm: int, frm_cnt: int, first_frm_is_start_point: bool,
                            last_frm_is_end_point: bool, end_point_is_sent_end: bool) -> None:
         self.PopDataBufTillFrame(start_frm)
         expected_sample_number = int(frm_cnt * self.vad_opts.sample_rate * self.vad_opts.frame_in_ms / 1000)
         if last_frm_is_end_point:
             extra_sample = max(0, int(self.vad_opts.frame_length_ms * self.vad_opts.sample_rate / 1000 - \
                                       self.vad_opts.sample_rate * self.vad_opts.frame_in_ms / 1000))
             expected_sample_number += int(extra_sample)
         if end_point_is_sent_end:
-            expected_sample_number = max(expected_sample_number, len(self.data_buf))
-        if len(self.data_buf) < expected_sample_number:
+            expected_sample_number = max(expected_sample_number, self.data_buf_size)
+        if self.data_buf_size < expected_sample_number:
             print('error in calling pop data_buf\n')
 
         if len(self.output_data_buf) == 0 or first_frm_is_start_point:
             self.output_data_buf.append(E2EVadSpeechBufWithDoa())
             self.output_data_buf[-1].Reset()
             self.output_data_buf[-1].start_ms = start_frm * self.vad_opts.frame_in_ms
             self.output_data_buf[-1].end_ms = self.output_data_buf[-1].start_ms
@@ -330,18 +329,18 @@
             print('warning\n')
         out_pos = len(cur_seg.buffer)  # cur_seg.buff现在没做任何操作
         data_to_pop = 0
         if end_point_is_sent_end:
             data_to_pop = expected_sample_number
         else:
             data_to_pop = int(frm_cnt * self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000)
-        if data_to_pop > len(self.data_buf):
-            print('VAD data_to_pop is bigger than self.data_buf.size()!!!\n')
-            data_to_pop = len(self.data_buf)
-            expected_sample_number = len(self.data_buf)
+        if data_to_pop > self.data_buf_size:
+            print('VAD data_to_pop is bigger than self.data_buf_size!!!\n')
+            data_to_pop = self.data_buf_size
+            expected_sample_number = self.data_buf_size
 
         cur_seg.doa = 0
         for sample_cpy_out in range(0, data_to_pop):
             # cur_seg.buffer[out_pos ++] = data_buf_.back();
             out_pos += 1
         for sample_cpy_out in range(data_to_pop, expected_sample_number):
             # cur_seg.buffer[out_pos++] = data_buf_.back()
@@ -416,15 +415,15 @@
             return frame_state
 
         sum_score = 0.0
         noise_prob = 0.0
         assert len(self.sil_pdf_ids) == self.vad_opts.silence_pdf_num
         if len(self.sil_pdf_ids) > 0:
             assert len(self.scores) == 1  # 只支持batch_size = 1的测试
-            sil_pdf_scores = [self.scores[0][t][sil_pdf_id] for sil_pdf_id in self.sil_pdf_ids]
+            sil_pdf_scores = [self.scores[0][t - self.idx_pre_chunk][sil_pdf_id] for sil_pdf_id in self.sil_pdf_ids]
             sum_score = sum(sil_pdf_scores)
             noise_prob = math.log(sum_score) * self.vad_opts.speech_2_noise_ratio
             total_score = 1.0
             sum_score = total_score - sum_score
         speech_prob = math.log(sum_score)
         if self.vad_opts.output_frame_probs:
             frame_prob = E2EVadFrameProb()
@@ -498,15 +497,15 @@
     def DetectCommonFrames(self) -> int:
         if self.vad_state_machine == VadStateMachine.kVadInStateEndPointDetected:
             return 0
         for i in range(self.vad_opts.nn_eval_block_size - 1, -1, -1):
             frame_state = FrameState.kFrameStateInvalid
             frame_state = self.GetFrameState(self.frm_cnt - 1 - i)
             self.DetectOneFrame(frame_state, self.frm_cnt - 1 - i, False)
-
+        self.idx_pre_chunk += self.scores.shape[1]
         return 0
 
     def DetectLastFrames(self) -> int:
         if self.vad_state_machine == VadStateMachine.kVadInStateEndPointDetected:
             return 0
         for i in range(self.vad_opts.nn_eval_block_size - 1, -1, -1):
             frame_state = FrameState.kFrameStateInvalid
```

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.4.6/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/samplers/build_batch_sampler.py` & `funasr-0.4.6/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/samplers/folded_batch_sampler.py` & `funasr-0.4.6/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/samplers/length_batch_sampler.py` & `funasr-0.4.6/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.4.6/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.4.6/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.4.6/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/schedulers/abs_scheduler.py` & `funasr-0.4.6/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/schedulers/noam_lr.py` & `funasr-0.4.6/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.4.6/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/schedulers/warmup_lr.py` & `funasr-0.4.6/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/tasks/abs_task.py` & `funasr-0.4.6/funasr/tasks/abs_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,14 +545,20 @@
         group.add_argument(
             "--accum_grad",
             type=int,
             default=1,
             help="The number of gradient accumulation",
         )
         group.add_argument(
+            "--bias_grad_times",
+            type=float,
+            default=1.0,
+            help="To scale the gradient of contextual related params",
+        )
+        group.add_argument(
             "--no_forward_run",
             type=str2bool,
             default=False,
             help="Just only iterating data loading without "
                  "model forwarding and training",
         )
         group.add_argument(
```

### Comparing `funasr-0.4.4/funasr/tasks/asr.py` & `funasr-0.4.6/funasr/tasks/asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.models.decoder.transformer_decoder import TransformerDecoder
 from funasr.models.decoder.contextual_decoder import ContextualParaformerDecoder
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.models.e2e_asr import ESPnetASRModel
 from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
+from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_asr_mfcca import MFCCA
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
@@ -124,14 +125,15 @@
         asr=ESPnetASRModel,
         uniasr=UniASR,
         paraformer=Paraformer,
         paraformer_online=ParaformerOnline,
         paraformer_bert=ParaformerBert,
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
+        neatcontextual_paraformer=NeatContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
     ),
     type_check=AbsESPnetModel,
     default="asr",
 )
 preencoder_choices = ClassChoices(
@@ -1643,15 +1645,14 @@
         if args.normalize is not None:
             normalize_class = normalize_choices.get_class(args.normalize)
             normalize = normalize_class(**args.normalize_conf)
         else:
             normalize = None
 
         # 4. Encoder
-
         if getattr(args, "encoder", None) is not None:
             encoder_class = encoder_choices.get_class(args.encoder)
             encoder = encoder_class(input_size, **args.encoder_conf)
         else:
             encoder = Encoder(input_size, **args.encoder_conf)
         encoder_output_size = encoder.output_size()
```

### Comparing `funasr-0.4.4/funasr/tasks/data2vec.py` & `funasr-0.4.6/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/tasks/diar.py` & `funasr-0.4.6/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/tasks/lm.py` & `funasr-0.4.6/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/tasks/punctuation.py` & `funasr-0.4.6/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/tasks/sv.py` & `funasr-0.4.6/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/tasks/vad.py` & `funasr-0.4.6/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/text/build_tokenizer.py` & `funasr-0.4.6/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/text/char_tokenizer.py` & `funasr-0.4.6/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/text/cleaner.py` & `funasr-0.4.6/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/text/korean_cleaner.py` & `funasr-0.4.6/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/text/phoneme_tokenizer.py` & `funasr-0.4.6/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.4.6/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/text/token_id_converter.py` & `funasr-0.4.6/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/text/word_tokenizer.py` & `funasr-0.4.6/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.4.6/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/torch_utils/device_funcs.py` & `funasr-0.4.6/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/torch_utils/forward_adaptor.py` & `funasr-0.4.6/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/torch_utils/initialize.py` & `funasr-0.4.6/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.4.6/funasr/torch_utils/load_pretrained_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,10 +116,10 @@
             if k.startswith(src_key)
         }
 
     dst_state = obj.state_dict()
     if ignore_init_mismatch:
         src_state = filter_state_dict(dst_state, src_state)
 
-    logging.info("Loaded src_state keys: {}".format(src_state.keys()))
+    # logging.info("Loaded src_state keys: {}".format(src_state.keys()))
     dst_state.update(src_state)
     obj.load_state_dict(dst_state)
```

### Comparing `funasr-0.4.4/funasr/torch_utils/model_summary.py` & `funasr-0.4.6/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/torch_utils/recursive_op.py` & `funasr-0.4.6/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/train/abs_espnet_model.py` & `funasr-0.4.6/funasr/train/abs_espnet_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/train/abs_model.py` & `funasr-0.4.6/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/train/class_choices.py` & `funasr-0.4.6/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/train/distributed_utils.py` & `funasr-0.4.6/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/train/reporter.py` & `funasr-0.4.6/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/train/trainer.py` & `funasr-0.4.6/funasr/train/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     best_model_criterion: Sequence[Sequence[str]]
     val_scheduler_criterion: Sequence[str]
     unused_parameters: bool
     wandb_model_log_interval: int
     use_pai: bool
     oss_bucket: Union[oss2.Bucket, None]
     batch_interval: int
+    bias_grad_times: float
 
 class Trainer:
     """Trainer having a optimizer.
 
     If you'd like to use multiple optimizers, then inherit this class
     and override the methods if necessary - at least "train_one_epoch()"
 
@@ -542,16 +543,19 @@
         accum_grad = options.accum_grad
         grad_clip = options.grad_clip
         grad_clip_type = options.grad_clip_type
         log_interval = options.log_interval
         no_forward_run = options.no_forward_run
         ngpu = options.ngpu
         use_wandb = options.use_wandb
+        bias_grad_times = options.bias_grad_times
         distributed = distributed_option.distributed
 
+        if bias_grad_times != 1.0:
+            logging.warning("Using bias_grad_times: {} for gradient scaling".format(bias_grad_times))
         if log_interval is None:
             try:
                 log_interval = max(len(iterator) // 20, 10)
             except TypeError:
                 log_interval = 100
 
         model.train()
@@ -686,14 +690,24 @@
                         model,
                         reporter.get_total_count(),
                         duration=100,
                         eta=1.0,
                         scale_factor=0.55,
                     )
 
+                # for contextual training
+                if bias_grad_times != 1.0:
+                    # contextual related parameter names
+                    cr_pnames = ["bias_encoder", "bias_embed", "decoder.bias_decoder", "decoder.bias_output"]
+                    for name, param in model.named_parameters():
+                        for cr_pname in cr_pnames:
+                            if cr_pname in name:
+                                param.grad *= bias_grad_times
+                                continue
+
                 # compute the gradient norm to check if it is normal or not
                 grad_norm = torch.nn.utils.clip_grad_norm_(
                     model.parameters(),
                     max_norm=grad_clip,
                     norm_type=grad_clip_type,
                 )
                 # PyTorch<=1.4, clip_grad_norm_ returns float value
```

### Comparing `funasr-0.4.4/funasr/utils/asr_env_checking.py` & `funasr-0.4.6/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/asr_utils.py` & `funasr-0.4.6/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/build_dataclass.py` & `funasr-0.4.6/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/cli_utils.py` & `funasr-0.4.6/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/compute_eer.py` & `funasr-0.4.6/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/compute_min_dcf.py` & `funasr-0.4.6/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/compute_wer.py` & `funasr-0.4.6/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/config_argparse.py` & `funasr-0.4.6/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/get_default_kwargs.py` & `funasr-0.4.6/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/griffin_lim.py` & `funasr-0.4.6/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/job_runner.py` & `funasr-0.4.6/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/misc.py` & `funasr-0.4.6/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/modelscope_param.py` & `funasr-0.4.6/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/nested_dict_action.py` & `funasr-0.4.6/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/postprocess_utils.py` & `funasr-0.4.6/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/sized_dict.py` & `funasr-0.4.6/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/timestamp_tools.py` & `funasr-0.4.6/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/types.py` & `funasr-0.4.6/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr/utils/wav_utils.py` & `funasr-0.4.6/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/funasr.egg-info/PKG-INFO` & `funasr-0.4.6/funasr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.4.4
+Version: 0.4.6
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -37,30 +36,30 @@
 
 <strong>FunASR</strong> hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
 [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-new) 
 | [**Highlights**](#highlights)
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
-| [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
+| [**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
-| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
+| [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
 We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
-- We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
+- We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - Compared to [Espnet](https://github.com/espnet/espnet) framework, the training speed of large-scale datasets in FunASR is much faster owning to the optimized dataloader.
 
 ## Installation
 
 Install from pip
@@ -84,20 +83,16 @@
 
 ```shell
 pip install -U modelscope
 # For the users in China, you could install with the command:
 # pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
-For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation.html)
+For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/installation.html)
 
-[//]: # ()
-[//]: # (## Usage)
-
-[//]: # (For users who are new to FunASR and ModelScope, please refer to FunASR Docs&#40;[CN]&#40;https://alibaba-damo-academy.github.io/FunASR/cn/index.html&#41; / [EN]&#40;https://alibaba-damo-academy.github.io/FunASR/en/index.html&#41;&#41;)
 
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
 
@@ -140,9 +135,7 @@
 @inproceedings{Shi2023AchievingTP,
   title={Achieving Timestamp Prediction While Recognizing with Non-Autoregressive End-to-End ASR Model},
   author={Xian Shi and Yanni Chen and Shiliang Zhang and Zhijie Yan},
   booktitle={arXiv preprint arXiv:2301.12343}
   year={2023}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.4.4 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.4.6 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
-License Platform: UNKNOWN Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
-Research Classifier: Operating System :: POSIX :: Linux Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown Provides-Extra: train Provides-Extra:
-recipe Provides-Extra: all Provides-Extra: test Provides-Extra: doc License-
-File: LICENSE [//]: # (
+License Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
+System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
+Provides-Extra: train Provides-Extra: recipe Provides-Extra: all Provides-
+Extra: test Provides-Extra: doc License-File: LICENSE [//]: # (
 [docs/images/funasr_logo.jpg]
 ) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
 developers can conduct research and production of speech recognition models
 more conveniently, and promote the development of speech recognition ecology.
 ASR for Funï¼ [**News**](https://github.com/alibaba-damo-academy/FunASR#whats-
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
-[**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/
+[**Tutorial_CN**](https://github.com/alibaba-damo-academy/FunASR/
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
-Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
+Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
 modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
 (https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
 meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
 Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
 announce that the M2MeT2.0 challenge will be held in the near future. The
 baseline system is conducted on FunASR and is provided as a receipe of
 AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
@@ -43,41 +42,40 @@
 (https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
 notes For the release notes, please ref to [news](https://github.com/alibaba-
 damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
 recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
 Restoration, Language Models, Speaker Verification and Speaker diarization. -
 We have released large number of academic and industrial pretrained models on
 [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition) - The pretrained model [Paraformer-large](https://
-www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
-vocab8404-pytorch/summary) obtains the best performance on many tasks in
-[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
-supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
-(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
-Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
-speed of large-scale datasets in FunASR is much faster owning to the optimized
-dataloader. ## Installation Install from pip ```shell pip install -U funasr #
-For the users in China, you could install with the command: # pip install -
-U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
-source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
-pip install -e ./ # For the users in China, you could install with the command:
-# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
-want to use the pretrained models in ModelScope, you should install the
-modelscope: ```shell pip install -U modelscope # For the users in China, you
-could install with the command: # pip install -U modelscope -f https://
-modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
-[installation](https://alibaba-damo-academy.github.io/FunASR/en/
-installation.html) [//]: # () [//]: # (## Usage) [//]: # (For users who are new
-to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-
-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-
-academy.github.io/FunASR/en/index.html))) ## Contact If you have any questions
-about FunASR, please contact us by - email: [funasr@list.alibaba-inc.com]
-(funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:--------
----------------------------------------------:| |
+recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/
+FunASR/blob/main/docs/model_zoo/modelscope_models.md) - The pretrained model
+[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
+large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
+performance on many tasks in [SpeechIO leaderboard](https://github.com/
+SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
+pretrained models from [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
+github.com/espnet/espnet) framework, the training speed of large-scale datasets
+in FunASR is much faster owning to the optimized dataloader. ## Installation
+Install from pip ```shell pip install -U funasr # For the users in China, you
+could install with the command: # pip install -U funasr -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
+clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
+For the users in China, you could install with the command: # pip install -e ./
+-i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
+pretrained models in ModelScope, you should install the modelscope: ```shell
+pip install -U modelscope # For the users in China, you could install with the
+command: # pip install -U modelscope -f https://modelscope.oss-cn-
+beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
+simple ``` For more details, please ref to [installation](https://alibaba-damo-
+academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
+have any questions about FunASR, please contact us by - email:
+[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
+Wechat group | |:---:|:-----------------------------------------------------:
+| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.4.4/funasr.egg-info/SOURCES.txt` & `funasr-0.4.6/funasr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 funasr/datasets/large_datasets/datapipes/__init__.py
 funasr/datasets/large_datasets/datapipes/batch.py
 funasr/datasets/large_datasets/datapipes/filter.py
 funasr/datasets/large_datasets/datapipes/map.py
 funasr/datasets/large_datasets/utils/__init__.py
 funasr/datasets/large_datasets/utils/clipping.py
 funasr/datasets/large_datasets/utils/filter.py
+funasr/datasets/large_datasets/utils/hotword_utils.py
 funasr/datasets/large_datasets/utils/low_frame_rate.py
 funasr/datasets/large_datasets/utils/padding.py
 funasr/datasets/large_datasets/utils/tokenize.py
 funasr/export/__init__.py
 funasr/export/export_model.py
 funasr/export/models/CT_Transformer.py
 funasr/export/models/__init__.py
@@ -130,14 +131,15 @@
 funasr/main_funcs/collect_stats.py
 funasr/main_funcs/pack_funcs.py
 funasr/models/__init__.py
 funasr/models/ctc.py
 funasr/models/data2vec.py
 funasr/models/e2e_asr.py
 funasr/models/e2e_asr_common.py
+funasr/models/e2e_asr_contextual_paraformer.py
 funasr/models/e2e_asr_mfcca.py
 funasr/models/e2e_asr_paraformer.py
 funasr/models/e2e_asr_transducer.py
 funasr/models/e2e_diar_eend_ola.py
 funasr/models/e2e_diar_sond.py
 funasr/models/e2e_sv.py
 funasr/models/e2e_tp.py
@@ -347,8 +349,14 @@
 funasr/utils/modelscope_param.py
 funasr/utils/nested_dict_action.py
 funasr/utils/postprocess_utils.py
 funasr/utils/sized_dict.py
 funasr/utils/timestamp_tools.py
 funasr/utils/types.py
 funasr/utils/wav_utils.py
-funasr/utils/yaml_no_alias_safe_dump.py
+funasr/utils/yaml_no_alias_safe_dump.py
+tests/test_asr_inference_pipeline.py
+tests/test_asr_vad_punc_inference_pipeline.py
+tests/test_lm_pipeline.py
+tests/test_punctuation_pipeline.py
+tests/test_sv_inference_pipeline.py
+tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.4.4/funasr.egg-info/requires.txt` & `funasr-0.4.6/funasr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.4.4/setup.py` & `funasr-0.4.6/setup.py`

 * *Files identical despite different names*

