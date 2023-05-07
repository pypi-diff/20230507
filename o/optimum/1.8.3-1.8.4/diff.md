# Comparing `tmp/optimum-1.8.3.tar.gz` & `tmp/optimum-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-1.8.3.tar", last modified: Fri Apr 28 16:34:11 2023, max compression
+gzip compressed data, was "optimum-1.8.4.tar", last modified: Sun May  7 20:52:25 2023, max compression
```

## Comparing `optimum-1.8.3.tar` & `optimum-1.8.4.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.363056 optimum-1.8.3/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-04-28 16:15:05.000000 optimum-1.8.3/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-04-28 16:15:05.000000 optimum-1.8.3/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    11475 2023-04-28 16:34:11.363056 optimum-1.8.3/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9876 2023-04-28 16:21:41.000000 optimum-1.8.3/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.333056 optimum-1.8.3/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.333056 optimum-1.8.3/optimum/bettertransformer/
--rw-r--r--   0 ella      (1000) ella      (1000)      707 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/bettertransformer/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.333056 optimum-1.8.3/optimum/bettertransformer/models/
--rw-r--r--   0 ella      (1000) ella      (1000)     8420 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/bettertransformer/models/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    21474 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/bettertransformer/models/attention.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8092 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/bettertransformer/models/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    12222 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/bettertransformer/models/decoder_models.py
--rw-r--r--   0 ella      (1000) ella      (1000)    60023 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/bettertransformer/models/encoder_models.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17127 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/bettertransformer/transformation.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.333056 optimum-1.8.3/optimum/commands/
--rw-r--r--   0 ella      (1000) ella      (1000)      952 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5872 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2475 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/env.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.333056 optimum-1.8.3/optimum/commands/export/
--rw-r--r--   0 ella      (1000) ella      (1000)      716 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/export/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1340 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/export/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8554 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/export/onnx.py
--rw-r--r--   0 ella      (1000) ella      (1000)     9016 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/export/tflite.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.333056 optimum-1.8.3/optimum/commands/onnxruntime/
--rw-r--r--   0 ella      (1000) ella      (1000)      759 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/onnxruntime/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1374 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/onnxruntime/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3885 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/onnxruntime/optimize.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4011 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/onnxruntime/quantize.py
--rw-r--r--   0 ella      (1000) ella      (1000)     6871 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/optimum_cli.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.343056 optimum-1.8.3/optimum/commands/register/
--rw-r--r--   0 ella      (1000) ella      (1000)      621 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/commands/register/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17957 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/configuration_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1454 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/conftest.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.343056 optimum-1.8.3/optimum/exporters/
--rw-r--r--   0 ella      (1000) ella      (1000)      688 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)      707 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)      903 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/error_utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.343056 optimum-1.8.3/optimum/exporters/onnx/
--rw-r--r--   0 ella      (1000) ella      (1000)     1918 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/onnx/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17290 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/exporters/onnx/__main__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    44198 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/onnx/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    16221 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/onnx/config.py
--rw-r--r--   0 ella      (1000) ella      (1000)      865 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/onnx/constants.py
--rw-r--r--   0 ella      (1000) ella      (1000)    31628 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/onnx/convert.py
--rw-r--r--   0 ella      (1000) ella      (1000)    37124 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/exporters/onnx/model_configs.py
--rw-r--r--   0 ella      (1000) ella      (1000)     7326 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/onnx/model_patcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)     9950 2023-04-28 16:21:49.000000 optimum-1.8.3/optimum/exporters/onnx/utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    60556 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/exporters/tasks.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.343056 optimum-1.8.3/optimum/exporters/tflite/
--rw-r--r--   0 ella      (1000) ella      (1000)     1209 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/tflite/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5256 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/tflite/__main__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15507 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/tflite/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1397 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/tflite/config.py
--rw-r--r--   0 ella      (1000) ella      (1000)    16963 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/tflite/convert.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3588 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/exporters/tflite/model_configs.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.343056 optimum-1.8.3/optimum/fx/
--rw-r--r--   0 ella      (1000) ella      (1000)      672 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/fx/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.343056 optimum-1.8.3/optimum/fx/optimization/
--rw-r--r--   0 ella      (1000) ella      (1000)      866 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/fx/optimization/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    32725 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/fx/optimization/transformations.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.343056 optimum-1.8.3/optimum/fx/quantization/
--rw-r--r--   0 ella      (1000) ella      (1000)      675 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/fx/quantization/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13591 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/fx/quantization/functions.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1450 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/fx/utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15117 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/modeling_base.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.343056 optimum-1.8.3/optimum/onnx/
--rw-r--r--   0 ella      (1000) ella      (1000)     1276 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnx/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3830 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnx/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    11198 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/onnx/graph_transformations.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4316 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnx/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13025 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnx/transformations_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3307 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnx/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.353056 optimum-1.8.3/optimum/onnxruntime/
--rw-r--r--   0 ella      (1000) ella      (1000)     4279 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    32544 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/onnxruntime/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    45434 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/onnxruntime/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      901 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/constants.py
--rw-r--r--   0 ella      (1000) ella      (1000)      955 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/graph.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.353056 optimum-1.8.3/optimum/onnxruntime/io_binding/
--rw-r--r--   0 ella      (1000) ella      (1000)      675 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/io_binding/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     7767 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/io_binding/io_binding_helper.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3915 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/model.py
--rw-r--r--   0 ella      (1000) ella      (1000)    30965 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/modeling_decoder.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17940 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    83591 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/modeling_ort.py
--rw-r--r--   0 ella      (1000) ella      (1000)    58316 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15083 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/optimization.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.353056 optimum-1.8.3/optimum/onnxruntime/preprocessors/
--rw-r--r--   0 ella      (1000) ella      (1000)      686 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/preprocessors/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.353056 optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/
--rw-r--r--   0 ella      (1000) ella      (1000)      760 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3048 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/excluders.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1377 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/fully_connected.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1415 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/gelu.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1580 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/layernorm.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2350 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/preprocessors/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    23448 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/onnxruntime/quantization.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.353056 optimum-1.8.3/optimum/onnxruntime/runs/
--rw-r--r--   0 ella      (1000) ella      (1000)     8001 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/runs/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4070 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/runs/calibrator.py
--rw-r--r--   0 ella      (1000) ella      (1000)      625 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/runs/utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    88945 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    38387 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17122 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1362 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/onnxruntime/training_args_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    11746 2023-04-28 16:21:41.000000 optimum-1.8.3/optimum/onnxruntime/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.353056 optimum-1.8.3/optimum/pipelines/
--rw-r--r--   0 ella      (1000) ella      (1000)      770 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/pipelines/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.353056 optimum-1.8.3/optimum/pipelines/diffusers/
--rw-r--r--   0 ella      (1000) ella      (1000)    11266 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2211 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/pipelines/diffusers/pipeline_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13522 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/pipelines/pipelines_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)      948 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/quantization_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10268 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/runs_base.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.363056 optimum-1.8.3/optimum/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)     1989 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)      845 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/constant.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2001 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/doc.py
--rw-r--r--   0 ella      (1000) ella      (1000)      953 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/dummy_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3747 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/file_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     6181 2023-04-28 16:21:49.000000 optimum-1.8.3/optimum/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    23612 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/input_generators.py
--rw-r--r--   0 ella      (1000) ella      (1000)     7836 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/logging.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1295 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/modeling_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     9323 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/normalized_config.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.363056 optimum-1.8.3/optimum/utils/preprocessing/
--rw-r--r--   0 ella      (1000) ella      (1000)      977 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/preprocessing/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10271 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/preprocessing/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4263 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/preprocessing/image_classification.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3995 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/preprocessing/question_answering.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2169 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/preprocessing/task_processors_manager.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4436 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/preprocessing/text_classification.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3940 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/preprocessing/token_classification.py
--rw-r--r--   0 ella      (1000) ella      (1000)    11609 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/runs.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2364 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/save_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5762 2023-04-28 16:15:05.000000 optimum-1.8.3/optimum/utils/testing_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      639 2023-04-28 16:22:54.000000 optimum-1.8.3/optimum/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-28 16:34:11.333056 optimum-1.8.3/optimum.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    11475 2023-04-28 16:34:10.000000 optimum-1.8.3/optimum.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     4271 2023-04-28 16:34:11.000000 optimum-1.8.3/optimum.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-04-28 16:34:10.000000 optimum-1.8.3/optimum.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-04-28 16:34:11.000000 optimum-1.8.3/optimum.egg-info/entry_points.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-04-28 16:34:10.000000 optimum-1.8.3/optimum.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)     1041 2023-04-28 16:34:11.000000 optimum-1.8.3/optimum.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-04-28 16:34:11.000000 optimum-1.8.3/optimum.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)     1212 2023-04-28 16:15:05.000000 optimum-1.8.3/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      423 2023-04-28 16:34:11.363056 optimum-1.8.3/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     3511 2023-04-28 16:21:41.000000 optimum-1.8.3/setup.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-05-07 20:38:30.000000 optimum-1.8.4/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-05-07 20:38:30.000000 optimum-1.8.4/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    11475 2023-05-07 20:52:25.015384 optimum-1.8.4/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     9876 2023-05-07 20:39:37.000000 optimum-1.8.4/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.965384 optimum-1.8.4/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.975384 optimum-1.8.4/optimum/bettertransformer/
+-rw-r--r--   0 ella      (1000) ella      (1000)      707 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/bettertransformer/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.975384 optimum-1.8.4/optimum/bettertransformer/models/
+-rw-r--r--   0 ella      (1000) ella      (1000)     8420 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/bettertransformer/models/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    21474 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/bettertransformer/models/attention.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     8092 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/bettertransformer/models/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    12222 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/bettertransformer/models/decoder_models.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    60023 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/bettertransformer/models/encoder_models.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17127 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/bettertransformer/transformation.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.975384 optimum-1.8.4/optimum/commands/
+-rw-r--r--   0 ella      (1000) ella      (1000)      952 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     5872 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2475 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/env.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.975384 optimum-1.8.4/optimum/commands/export/
+-rw-r--r--   0 ella      (1000) ella      (1000)      716 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/export/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1340 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/export/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     8554 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/commands/export/onnx.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9016 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/export/tflite.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.975384 optimum-1.8.4/optimum/commands/onnxruntime/
+-rw-r--r--   0 ella      (1000) ella      (1000)      759 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/onnxruntime/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1374 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/onnxruntime/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3885 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/onnxruntime/optimize.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4011 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/onnxruntime/quantize.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6871 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/optimum_cli.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.975384 optimum-1.8.4/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      621 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/commands/register/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17957 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/configuration_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1454 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/conftest.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.985384 optimum-1.8.4/optimum/exporters/
+-rw-r--r--   0 ella      (1000) ella      (1000)      688 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      707 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      903 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/exporters/error_utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.985384 optimum-1.8.4/optimum/exporters/onnx/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1918 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/onnx/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17290 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/exporters/onnx/__main__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    44198 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/exporters/onnx/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    16221 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/onnx/config.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      865 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/onnx/constants.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    31628 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/exporters/onnx/convert.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    37124 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/exporters/onnx/model_configs.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     7326 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/onnx/model_patcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9950 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/onnx/utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    60556 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/exporters/tasks.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.995384 optimum-1.8.4/optimum/exporters/tflite/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1209 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/tflite/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     5256 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/tflite/__main__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15507 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/exporters/tflite/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1397 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/tflite/config.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    16963 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/tflite/convert.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3588 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/exporters/tflite/model_configs.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.995384 optimum-1.8.4/optimum/fx/
+-rw-r--r--   0 ella      (1000) ella      (1000)      672 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/fx/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.995384 optimum-1.8.4/optimum/fx/optimization/
+-rw-r--r--   0 ella      (1000) ella      (1000)      866 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/fx/optimization/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    32725 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/fx/optimization/transformations.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.995384 optimum-1.8.4/optimum/fx/quantization/
+-rw-r--r--   0 ella      (1000) ella      (1000)      675 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/fx/quantization/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13591 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/fx/quantization/functions.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1450 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/fx/utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15117 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/modeling_base.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.995384 optimum-1.8.4/optimum/onnx/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1276 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnx/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3830 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnx/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    11198 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/onnx/graph_transformations.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4316 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnx/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13025 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnx/transformations_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3307 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnx/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/onnxruntime/
+-rw-r--r--   0 ella      (1000) ella      (1000)     4279 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    32544 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/onnxruntime/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    45434 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/onnxruntime/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      901 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/constants.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      955 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/graph.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/onnxruntime/io_binding/
+-rw-r--r--   0 ella      (1000) ella      (1000)      675 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/io_binding/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     7767 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/io_binding/io_binding_helper.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3915 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/model.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    30965 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17940 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    83591 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/modeling_ort.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    58316 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15083 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/optimization.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/onnxruntime/preprocessors/
+-rw-r--r--   0 ella      (1000) ella      (1000)      686 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/preprocessors/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/
+-rw-r--r--   0 ella      (1000) ella      (1000)      760 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3048 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/excluders.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1377 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/fully_connected.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1415 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/gelu.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1580 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/layernorm.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2350 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/preprocessors/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    23448 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/onnxruntime/quantization.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/onnxruntime/runs/
+-rw-r--r--   0 ella      (1000) ella      (1000)     8001 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/runs/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4070 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/runs/calibrator.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      625 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/runs/utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    88945 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    38387 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17122 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1362 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/onnxruntime/training_args_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    11746 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/onnxruntime/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/pipelines/
+-rw-r--r--   0 ella      (1000) ella      (1000)      770 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/pipelines/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/pipelines/diffusers/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11266 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2211 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/pipelines/diffusers/pipeline_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13522 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/pipelines/pipelines_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      948 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/quantization_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10268 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/runs_base.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1989 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      845 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2001 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/doc.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      953 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/dummy_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3747 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/file_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6181 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    23612 2023-05-07 20:39:37.000000 optimum-1.8.4/optimum/utils/input_generators.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     7836 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/logging.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1295 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/modeling_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9323 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/normalized_config.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:25.005384 optimum-1.8.4/optimum/utils/preprocessing/
+-rw-r--r--   0 ella      (1000) ella      (1000)      977 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/preprocessing/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10271 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/preprocessing/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4263 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/preprocessing/image_classification.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3995 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/preprocessing/question_answering.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2169 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/preprocessing/task_processors_manager.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4436 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/preprocessing/text_classification.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3940 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/preprocessing/token_classification.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    11609 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/runs.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2364 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/save_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     5762 2023-05-07 20:38:30.000000 optimum-1.8.4/optimum/utils/testing_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      639 2023-05-07 20:42:31.000000 optimum-1.8.4/optimum/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-05-07 20:52:24.965384 optimum-1.8.4/optimum.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11475 2023-05-07 20:52:24.000000 optimum-1.8.4/optimum.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     4271 2023-05-07 20:52:24.000000 optimum-1.8.4/optimum.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-05-07 20:52:24.000000 optimum-1.8.4/optimum.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-05-07 20:52:24.000000 optimum-1.8.4/optimum.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-05-07 20:52:13.000000 optimum-1.8.4/optimum.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)     1069 2023-05-07 20:52:24.000000 optimum-1.8.4/optimum.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-05-07 20:52:24.000000 optimum-1.8.4/optimum.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1212 2023-05-07 20:38:30.000000 optimum-1.8.4/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      423 2023-05-07 20:52:25.015384 optimum-1.8.4/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     3539 2023-05-07 20:40:22.000000 optimum-1.8.4/setup.py
```

### Comparing `optimum-1.8.3/LICENSE` & `optimum-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/MANIFEST.in` & `optimum-1.8.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/PKG-INFO` & `optimum-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.8.3
+Version: 1.8.4
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-1.8.3/README.md` & `optimum-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/bettertransformer/__init__.py` & `optimum-1.8.4/optimum/bettertransformer/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/bettertransformer/models/__init__.py` & `optimum-1.8.4/optimum/bettertransformer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/bettertransformer/models/attention.py` & `optimum-1.8.4/optimum/bettertransformer/models/attention.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/bettertransformer/models/base.py` & `optimum-1.8.4/optimum/bettertransformer/models/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/bettertransformer/models/decoder_models.py` & `optimum-1.8.4/optimum/bettertransformer/models/decoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/bettertransformer/models/encoder_models.py` & `optimum-1.8.4/optimum/bettertransformer/models/encoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/bettertransformer/transformation.py` & `optimum-1.8.4/optimum/bettertransformer/transformation.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/__init__.py` & `optimum-1.8.4/optimum/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/base.py` & `optimum-1.8.4/optimum/commands/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/env.py` & `optimum-1.8.4/optimum/commands/env.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/export/__init__.py` & `optimum-1.8.4/optimum/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/export/base.py` & `optimum-1.8.4/optimum/commands/export/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/export/onnx.py` & `optimum-1.8.4/optimum/commands/export/onnx.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/export/tflite.py` & `optimum-1.8.4/optimum/commands/export/tflite.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/onnxruntime/__init__.py` & `optimum-1.8.4/optimum/commands/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/onnxruntime/base.py` & `optimum-1.8.4/optimum/commands/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/onnxruntime/optimize.py` & `optimum-1.8.4/optimum/commands/onnxruntime/optimize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/onnxruntime/quantize.py` & `optimum-1.8.4/optimum/commands/onnxruntime/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/optimum_cli.py` & `optimum-1.8.4/optimum/commands/optimum_cli.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/commands/register/__init__.py` & `optimum-1.8.4/optimum/commands/register/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/configuration_utils.py` & `optimum-1.8.4/optimum/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/conftest.py` & `optimum-1.8.4/optimum/conftest.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/__init__.py` & `optimum-1.8.4/optimum/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/base.py` & `optimum-1.8.4/optimum/exporters/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/error_utils.py` & `optimum-1.8.4/optimum/exporters/error_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/__init__.py` & `optimum-1.8.4/optimum/exporters/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/__main__.py` & `optimum-1.8.4/optimum/exporters/onnx/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/base.py` & `optimum-1.8.4/optimum/exporters/onnx/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/config.py` & `optimum-1.8.4/optimum/exporters/onnx/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/constants.py` & `optimum-1.8.4/optimum/exporters/onnx/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/convert.py` & `optimum-1.8.4/optimum/exporters/onnx/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/model_configs.py` & `optimum-1.8.4/optimum/exporters/onnx/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/model_patcher.py` & `optimum-1.8.4/optimum/exporters/onnx/model_patcher.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/onnx/utils.py` & `optimum-1.8.4/optimum/exporters/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/tasks.py` & `optimum-1.8.4/optimum/exporters/tasks.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/tflite/__init__.py` & `optimum-1.8.4/optimum/exporters/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/tflite/__main__.py` & `optimum-1.8.4/optimum/exporters/tflite/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/tflite/base.py` & `optimum-1.8.4/optimum/exporters/tflite/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/tflite/config.py` & `optimum-1.8.4/optimum/exporters/tflite/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/tflite/convert.py` & `optimum-1.8.4/optimum/exporters/tflite/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/exporters/tflite/model_configs.py` & `optimum-1.8.4/optimum/exporters/tflite/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/fx/__init__.py` & `optimum-1.8.4/optimum/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/fx/optimization/__init__.py` & `optimum-1.8.4/optimum/fx/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/fx/optimization/transformations.py` & `optimum-1.8.4/optimum/fx/optimization/transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/fx/quantization/__init__.py` & `optimum-1.8.4/optimum/fx/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/fx/quantization/functions.py` & `optimum-1.8.4/optimum/fx/quantization/functions.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/fx/utils.py` & `optimum-1.8.4/optimum/fx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/modeling_base.py` & `optimum-1.8.4/optimum/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnx/__init__.py` & `optimum-1.8.4/optimum/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnx/configuration.py` & `optimum-1.8.4/optimum/onnx/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnx/graph_transformations.py` & `optimum-1.8.4/optimum/onnx/graph_transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnx/modeling_seq2seq.py` & `optimum-1.8.4/optimum/onnx/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnx/transformations_utils.py` & `optimum-1.8.4/optimum/onnx/transformations_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnx/utils.py` & `optimum-1.8.4/optimum/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/__init__.py` & `optimum-1.8.4/optimum/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/base.py` & `optimum-1.8.4/optimum/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/configuration.py` & `optimum-1.8.4/optimum/onnxruntime/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/constants.py` & `optimum-1.8.4/optimum/onnxruntime/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/graph.py` & `optimum-1.8.4/optimum/onnxruntime/graph.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/io_binding/__init__.py` & `optimum-1.8.4/optimum/onnxruntime/io_binding/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/io_binding/io_binding_helper.py` & `optimum-1.8.4/optimum/onnxruntime/io_binding/io_binding_helper.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/model.py` & `optimum-1.8.4/optimum/onnxruntime/model.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/modeling_decoder.py` & `optimum-1.8.4/optimum/onnxruntime/modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/modeling_diffusion.py` & `optimum-1.8.4/optimum/onnxruntime/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/modeling_ort.py` & `optimum-1.8.4/optimum/onnxruntime/modeling_ort.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/modeling_seq2seq.py` & `optimum-1.8.4/optimum/onnxruntime/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/optimization.py` & `optimum-1.8.4/optimum/onnxruntime/optimization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/preprocessors/__init__.py` & `optimum-1.8.4/optimum/onnxruntime/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/__init__.py` & `optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/excluders.py` & `optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/excluders.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/fully_connected.py` & `optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/fully_connected.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/gelu.py` & `optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/gelu.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/preprocessors/passes/layernorm.py` & `optimum-1.8.4/optimum/onnxruntime/preprocessors/passes/layernorm.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/preprocessors/quantization.py` & `optimum-1.8.4/optimum/onnxruntime/preprocessors/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/quantization.py` & `optimum-1.8.4/optimum/onnxruntime/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/runs/__init__.py` & `optimum-1.8.4/optimum/onnxruntime/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/runs/calibrator.py` & `optimum-1.8.4/optimum/onnxruntime/runs/calibrator.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/runs/utils.py` & `optimum-1.8.4/optimum/onnxruntime/runs/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/trainer.py` & `optimum-1.8.4/optimum/onnxruntime/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/trainer_seq2seq.py` & `optimum-1.8.4/optimum/onnxruntime/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/training_args.py` & `optimum-1.8.4/optimum/onnxruntime/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/training_args_seq2seq.py` & `optimum-1.8.4/optimum/onnxruntime/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/onnxruntime/utils.py` & `optimum-1.8.4/optimum/onnxruntime/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/pipelines/__init__.py` & `optimum-1.8.4/optimum/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/pipelines/diffusers/pipeline_stable_diffusion.py` & `optimum-1.8.4/optimum/pipelines/diffusers/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/pipelines/diffusers/pipeline_utils.py` & `optimum-1.8.4/optimum/pipelines/diffusers/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/pipelines/pipelines_base.py` & `optimum-1.8.4/optimum/pipelines/pipelines_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/quantization_base.py` & `optimum-1.8.4/optimum/quantization_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/runs_base.py` & `optimum-1.8.4/optimum/runs_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/__init__.py` & `optimum-1.8.4/optimum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/constant.py` & `optimum-1.8.4/optimum/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/doc.py` & `optimum-1.8.4/optimum/utils/doc.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/dummy_diffusers_objects.py` & `optimum-1.8.4/optimum/utils/dummy_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/file_utils.py` & `optimum-1.8.4/optimum/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/import_utils.py` & `optimum-1.8.4/optimum/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/input_generators.py` & `optimum-1.8.4/optimum/utils/input_generators.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/logging.py` & `optimum-1.8.4/optimum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/modeling_utils.py` & `optimum-1.8.4/optimum/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/normalized_config.py` & `optimum-1.8.4/optimum/utils/normalized_config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/preprocessing/__init__.py` & `optimum-1.8.4/optimum/utils/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/preprocessing/base.py` & `optimum-1.8.4/optimum/utils/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/preprocessing/image_classification.py` & `optimum-1.8.4/optimum/utils/preprocessing/image_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/preprocessing/question_answering.py` & `optimum-1.8.4/optimum/utils/preprocessing/question_answering.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/preprocessing/task_processors_manager.py` & `optimum-1.8.4/optimum/utils/preprocessing/task_processors_manager.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/preprocessing/text_classification.py` & `optimum-1.8.4/optimum/utils/preprocessing/text_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/preprocessing/token_classification.py` & `optimum-1.8.4/optimum/utils/preprocessing/token_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/runs.py` & `optimum-1.8.4/optimum/utils/runs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/save_utils.py` & `optimum-1.8.4/optimum/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/utils/testing_utils.py` & `optimum-1.8.4/optimum/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum/version.py` & `optimum-1.8.4/optimum/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.8.3"
+__version__ = "1.8.4"
```

### Comparing `optimum-1.8.3/optimum.egg-info/PKG-INFO` & `optimum-1.8.4/optimum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.8.3
+Version: 1.8.4
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-1.8.3/optimum.egg-info/SOURCES.txt` & `optimum-1.8.4/optimum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/optimum.egg-info/requires.txt` & `optimum-1.8.4/optimum.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 sacremoses
 diffusers
 torchaudio
 black~=23.1
 ruff>=0.0.241
 
 [exporters]
-onnx
+onnx<1.14.0
 onnxruntime
 timm
 
 [exporters-gpu]
-onnx
+onnx<1.14.0
 onnxruntime-gpu
 timm
 
 [exporters-tf]
 tensorflow<2.11,>=2.4
 tf2onnx
 onnx
@@ -65,22 +65,22 @@
 [neuronx]
 optimum-neuron[neuronx]
 
 [nncf]
 optimum-intel[nncf]
 
 [onnxruntime]
-onnx
+onnx<1.14.0
 onnxruntime>=1.9.0
 datasets>=1.2.1
 evaluate
 protobuf>=3.20.1
 
 [onnxruntime-gpu]
-onnx
+onnx<1.14.0
 onnxruntime-gpu>=1.9.0
 datasets>=1.2.1
 evaluate
 protobuf>=3.20.1
 
 [openvino]
 optimum-intel[openvino]
```

### Comparing `optimum-1.8.3/pyproject.toml` & `optimum-1.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-1.8.3/setup.py` & `optimum-1.8.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,29 +37,29 @@
 
 QUALITY_REQUIRE = ["black~=23.1", "ruff>=0.0.241"]
 
 BENCHMARK_REQUIRE = ["optuna", "tqdm", "scikit-learn", "seqeval", "torchvision", "evaluate>=0.2.0"]
 
 EXTRAS_REQUIRE = {
     "onnxruntime": [
-        "onnx",
+        "onnx<1.14.0",
         "onnxruntime>=1.9.0",
         "datasets>=1.2.1",
         "evaluate",
         "protobuf>=3.20.1",
     ],
     "onnxruntime-gpu": [
-        "onnx",
+        "onnx<1.14.0",
         "onnxruntime-gpu>=1.9.0",
         "datasets>=1.2.1",
         "evaluate",
         "protobuf>=3.20.1",
     ],
-    "exporters": ["onnx", "onnxruntime", "timm"],
-    "exporters-gpu": ["onnx", "onnxruntime-gpu", "timm"],
+    "exporters": ["onnx<1.14.0", "onnxruntime", "timm"],
+    "exporters-gpu": ["onnx<1.14.0", "onnxruntime-gpu", "timm"],
     "exporters-tf": ["tensorflow>=2.4,<2.11", "tf2onnx", "onnx", "onnxruntime", "timm", "h5py", "numpy<1.24.0"],
     "intel": "optimum-intel",
     "openvino": "optimum-intel[openvino]",
     "nncf": "optimum-intel[nncf]",
     "neural-compressor": "optimum-intel[neural-compressor]",
     "graphcore": "optimum-graphcore",
     "habana": "optimum-habana",
```

