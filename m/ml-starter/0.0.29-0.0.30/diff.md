# Comparing `tmp/ml-starter-0.0.29.tar.gz` & `tmp/ml-starter-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.29.tar", last modified: Sun May  7 15:14:26 2023, max compression
+gzip compressed data, was "ml-starter-0.0.30.tar", last modified: Sun May  7 16:08:04 2023, max compression
```

## Comparing `ml-starter-0.0.29.tar` & `ml-starter-0.0.30.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.922432 ml-starter-0.0.29/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 15:14:09.000000 ml-starter-0.0.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 15:14:09.000000 ml-starter-0.0.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 15:14:26.922432 ml-starter-0.0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-07 15:14:09.000000 ml-starter-0.0.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32994 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.918432 ml-starter-0.0.29/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.918432 ml-starter-0.0.29/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.922432 ml-starter-0.0.29/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.922432 ml-starter-0.0.29/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-07 15:14:09.000000 ml-starter-0.0.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 15:14:09.000000 ml-starter-0.0.29/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-07 15:14:09.000000 ml-starter-0.0.29/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 15:14:09.000000 ml-starter-0.0.29/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 15:14:26.922432 ml-starter-0.0.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-07 15:14:09.000000 ml-starter-0.0.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.549317 ml-starter-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 16:07:51.000000 ml-starter-0.0.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 16:07:51.000000 ml-starter-0.0.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 16:08:04.549317 ml-starter-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-07 16:07:51.000000 ml-starter-0.0.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.533316 ml-starter-0.0.30/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.533316 ml-starter-0.0.30/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.533316 ml-starter-0.0.30/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.533316 ml-starter-0.0.30/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33142 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.537317 ml-starter-0.0.30/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.537317 ml-starter-0.0.30/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.537317 ml-starter-0.0.30/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.545317 ml-starter-0.0.30/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.545317 ml-starter-0.0.30/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.545317 ml-starter-0.0.30/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.545317 ml-starter-0.0.30/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.549317 ml-starter-0.0.30/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.549317 ml-starter-0.0.30/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.549317 ml-starter-0.0.30/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-07 16:07:51.000000 ml-starter-0.0.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 16:07:51.000000 ml-starter-0.0.30/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-07 16:07:51.000000 ml-starter-0.0.30/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 16:07:51.000000 ml-starter-0.0.30/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 16:08:04.553317 ml-starter-0.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-07 16:07:51.000000 ml-starter-0.0.30/setup.py
```

### Comparing `ml-starter-0.0.29/LICENSE` & `ml-starter-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/PKG-INFO` & `ml-starter-0.0.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.29
+Version: 0.0.30
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.29/README.md` & `ml-starter-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/api.py` & `ml-starter-0.0.30/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/core/config.py` & `ml-starter-0.0.30/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/core/env.py` & `ml-starter-0.0.30/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/core/registry.py` & `ml-starter-0.0.30/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/core/state.py` & `ml-starter-0.0.30/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/launchers/base.py` & `ml-starter-0.0.30/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/launchers/ddp.py` & `ml-starter-0.0.30/ml/launchers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/launchers/slurm.py` & `ml-starter-0.0.30/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/launchers/torchrun.py` & `ml-starter-0.0.30/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/loggers/base.py` & `ml-starter-0.0.30/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/loggers/meter.py` & `ml-starter-0.0.30/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/loggers/multi.py` & `ml-starter-0.0.30/ml/loggers/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 import math
 import re
+import warnings
 from collections import defaultdict
 from typing import Any, Callable, Iterator, Sequence, TypeVar
 
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional as V
 from PIL import Image, ImageDraw, ImageFont
@@ -195,14 +196,17 @@
             pass
         elif audio.shape[1] in VALID_AUDIO_CHANNEL_COUNTS:
             audio = audio.permute(1, 0)
         else:
             raise ValueError(f"Invalid channel count{'' if log_key is None else f' for {log_key}'}: {audio.shape}")
     else:
         raise ValueError(f"Invalid audio shape{'' if log_key is None else f' for {log_key}'}: {audio.shape}")
+    if audio.max() > 1.0:
+        warnings.warn("Audio is outside the range [-1, 1]; clipping")
+        audio = audio / audio.max()
     return audio
 
 
 def standardize_video(video: Tensor, *, log_key: str | None = None, normalize: bool = True) -> Tensor:
     """Converts an arbitrary video to shape (T, C, H, W).
 
     Args:
```

### Comparing `ml-starter-0.0.29/ml/loggers/stdout.py` & `ml-starter-0.0.30/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/loggers/tensorboard.py` & `ml-starter-0.0.30/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/lr_schedulers/base.py` & `ml-starter-0.0.30/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.30/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.30/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/lr_schedulers/linear.py` & `ml-starter-0.0.30/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.30/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.30/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/models/activations.py` & `ml-starter-0.0.30/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/models/base.py` & `ml-starter-0.0.30/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/models/embeddings.py` & `ml-starter-0.0.30/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/models/init.py` & `ml-starter-0.0.30/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/models/lora.py` & `ml-starter-0.0.30/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/models/norms.py` & `ml-starter-0.0.30/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/optimizers/adam.py` & `ml-starter-0.0.30/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/optimizers/adamw.py` & `ml-starter-0.0.30/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/optimizers/adan.py` & `ml-starter-0.0.30/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/optimizers/base.py` & `ml-starter-0.0.30/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/optimizers/sgd.py` & `ml-starter-0.0.30/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/optimizers/shampoo.py` & `ml-starter-0.0.30/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/scripts/cli.py` & `ml-starter-0.0.30/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/scripts/stage.py` & `ml-starter-0.0.30/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/scripts/train.py` & `ml-starter-0.0.30/ml/scripts/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,13 +55,13 @@
             stats: dict[str, str] = {
                 "Start Time": format_datetime(start_time),
                 "End Time": format_datetime(end_time),
                 "Duration": format_timedelta(delta),
             }
             if trainer is not None:
                 stats["Experiment Directory"] = str(trainer.exp_dir)
-            stats_str = "".join(f"\n ↪ {colorize(k, 'cyan')}: {colorize(v, 'cyan')}" for k, v in stats.items())
-            logger.info("Finished training. Stats:\n%s", stats_str)
+            stats_str = "".join(f"\n ↪ {colorize(k, 'magenta')}: {colorize(v, 'cyan')}" for k, v in stats.items())
+            logger.info("Finished training. Stats:%s", stats_str)
 
     # Runs the training loop.
     with log_info_wrapper():
         trainer.train(model, task, optimizer, lr_scheduler)
```

### Comparing `ml-starter-0.0.29/ml/tasks/base.py` & `ml-starter-0.0.30/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.30/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.30/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/collate.py` & `ml-starter-0.0.30/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.30/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.30/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.30/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.30/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.30/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/utils.py` & `ml-starter-0.0.30/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.30/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/environments/base.py` & `ml-starter-0.0.30/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/environments/utils.py` & `ml-starter-0.0.30/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/environments/worker.py` & `ml-starter-0.0.30/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/losses/reduce.py` & `ml-starter-0.0.30/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/rl/base.py` & `ml-starter-0.0.30/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/rl/replay.py` & `ml-starter-0.0.30/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/tasks/sl/base.py` & `ml-starter-0.0.30/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/base.py` & `ml-starter-0.0.30/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.30/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.30/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.30/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.30/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.30/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.30/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.30/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.30/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/rl.py` & `ml-starter-0.0.30/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/sl.py` & `ml-starter-0.0.30/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/trainers/vanilla.py` & `ml-starter-0.0.30/ml/trainers/vanilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                 state.num_test_steps += 1
 
     def _init_environment(self) -> None:
         root_logger = logging.getLogger()
         for handler in root_logger.handlers:
             if isinstance(handler, logging.FileHandler) and Path(handler.baseFilename).name == "main.log":
                 root_logger.removeHandler(handler)
-        root_logger.addHandler(logging.FileHandler("main.log"))
+        root_logger.addHandler(logging.FileHandler(str((self.log_dir / "main.log").resolve())))
 
         # Sets up environment.
         if self.config.deterministic:
             torch.use_deterministic_algorithms(True)
         if self.config.use_tf32 and torch.cuda.is_available():
             torch.backends.cuda.matmul.allow_tf32 = True
```

### Comparing `ml-starter-0.0.29/ml/utils/argparse.py` & `ml-starter-0.0.30/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/atomic.py` & `ml-starter-0.0.30/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/augmentation.py` & `ml-starter-0.0.30/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/caching.py` & `ml-starter-0.0.30/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/call_train.py` & `ml-starter-0.0.30/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/cli.py` & `ml-starter-0.0.30/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/colors.py` & `ml-starter-0.0.30/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/data.py` & `ml-starter-0.0.30/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/datetime.py` & `ml-starter-0.0.30/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/device/auto.py` & `ml-starter-0.0.30/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/device/base.py` & `ml-starter-0.0.30/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/device/cpu.py` & `ml-starter-0.0.30/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/device/gpu.py` & `ml-starter-0.0.30/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/device/metal.py` & `ml-starter-0.0.30/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/distributed.py` & `ml-starter-0.0.30/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/image.py` & `ml-starter-0.0.30/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/io.py` & `ml-starter-0.0.30/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/large_models.py` & `ml-starter-0.0.30/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/logging.py` & `ml-starter-0.0.30/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/meter.py` & `ml-starter-0.0.30/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/staging.py` & `ml-starter-0.0.30/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/timer.py` & `ml-starter-0.0.30/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/torch_distributed.py` & `ml-starter-0.0.30/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml/utils/video.py` & `ml-starter-0.0.30/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.30/ml_starter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.29
+Version: 0.0.30
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.29/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.30/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/pyproject.toml` & `ml-starter-0.0.30/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.29/setup.py` & `ml-starter-0.0.30/setup.py`

 * *Files identical despite different names*

