# Comparing `tmp/ml-starter-0.0.28.tar.gz` & `tmp/ml-starter-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.28.tar", last modified: Fri May  5 13:05:23 2023, max compression
+gzip compressed data, was "ml-starter-0.0.29.tar", last modified: Sun May  7 15:14:26 2023, max compression
```

## Comparing `ml-starter-0.0.28.tar` & `ml-starter-0.0.29.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.746111 ml-starter-0.0.28/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 13:05:07.000000 ml-starter-0.0.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 13:05:07.000000 ml-starter-0.0.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-05 13:05:23.746111 ml-starter-0.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-05 13:05:07.000000 ml-starter-0.0.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32994 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.742111 ml-starter-0.0.28/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.742111 ml-starter-0.0.28/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.746111 ml-starter-0.0.28/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-05 13:05:07.000000 ml-starter-0.0.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 13:05:07.000000 ml-starter-0.0.28/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 13:05:07.000000 ml-starter-0.0.28/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 13:05:07.000000 ml-starter-0.0.28/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 13:05:23.746111 ml-starter-0.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-05 13:05:07.000000 ml-starter-0.0.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.922432 ml-starter-0.0.29/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 15:14:09.000000 ml-starter-0.0.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 15:14:09.000000 ml-starter-0.0.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 15:14:26.922432 ml-starter-0.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-07 15:14:09.000000 ml-starter-0.0.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32994 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.906432 ml-starter-0.0.29/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.910431 ml-starter-0.0.29/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.914432 ml-starter-0.0.29/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.918432 ml-starter-0.0.29/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.918432 ml-starter-0.0.29/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.922432 ml-starter-0.0.29/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-07 15:14:09.000000 ml-starter-0.0.29/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:14:26.922432 ml-starter-0.0.29/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-07 15:14:26.000000 ml-starter-0.0.29/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-07 15:14:09.000000 ml-starter-0.0.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 15:14:09.000000 ml-starter-0.0.29/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-07 15:14:09.000000 ml-starter-0.0.29/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 15:14:09.000000 ml-starter-0.0.29/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 15:14:26.922432 ml-starter-0.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-07 15:14:09.000000 ml-starter-0.0.29/setup.py
```

### Comparing `ml-starter-0.0.28/LICENSE` & `ml-starter-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/PKG-INFO` & `ml-starter-0.0.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.28
+Version: 0.0.29
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.28/README.md` & `ml-starter-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/api.py` & `ml-starter-0.0.29/ml/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,18 @@
     "InitializationType",
     "instantiate_config",
     "is_debugging",
     "is_distributed",
     "is_master",
     "LearnedPositionalEmbeddings",
     "load_model_and_task",
+    "LoRAConv1D",
+    "LoRAConv2D",
+    "LoRAEmbedding",
+    "LoRALinear",
     "Loss",
     "meta_to_empty_func",
     "MultiIterDataset",
     "NormType",
     "open_atomic",
     "Output",
     "pad_all",
@@ -170,14 +174,15 @@
     LearnedPositionalEmbeddings,
     RotaryEmbeddings,
     SinusoidalEmbeddings,
     cast_embedding_kind,
     get_positional_embeddings,
 )
 from ml.models.init import InitializationType, cast_init_type, init_
+from ml.models.lora import LoRAConv1D, LoRAConv2D, LoRAEmbedding, LoRALinear
 from ml.models.norms import (
     NormType,
     cast_norm_type,
     get_norm_1d,
     get_norm_2d,
     get_norm_3d,
     get_norm_linear,
```

### Comparing `ml-starter-0.0.28/ml/core/config.py` & `ml-starter-0.0.29/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/core/env.py` & `ml-starter-0.0.29/ml/core/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,10 +145,14 @@
 DisableMetal = _BoolEnvVar("DISABLE_METAL", default=False)
 is_metal_disabled = DisableMetal.get
 
 # Disables using the GPU.
 DisableGPU = _BoolEnvVar("DISABLE_GPU", default=False)
 is_gpu_disabled = DisableGPU.get
 
+# Disables Tensorboard subprocess.
+DisableTensorboard = _BoolEnvVar("DISABLE_TENSORBOARD", default=False)
+is_tensorboard_disabled = DisableTensorboard.get
+
 # Show full error message when trying to import a file.
 ShowFullImportError = _BoolEnvVar("SHOW_FULL_IMPORT_ERROR", default=False)
 should_show_full_import_error = ShowFullImportError.get
```

### Comparing `ml-starter-0.0.28/ml/core/registry.py` & `ml-starter-0.0.29/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/core/state.py` & `ml-starter-0.0.29/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/launchers/base.py` & `ml-starter-0.0.29/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/launchers/ddp.py` & `ml-starter-0.0.29/ml/launchers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/launchers/slurm.py` & `ml-starter-0.0.29/ml/launchers/slurm.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,17 @@
 export MASTER_PORT={master_port}
 
 # Set some debugging flags.
 export TORCH_DISTRIBUTED_DEBUG=DETAIL
 export TORCH_SHOW_CPP_STACKTRACES=1
 export NCCL_DEBUG=1
 
+# Disables Tensorboard subprocess.
+export DISABLE_TENSORBOARD=1
+
 echo "***"
 echo "Job ID: ${{SLURM_JOBID}}"
 echo "***"
 echo ""
 
 # Runs the training command.
 srun \\
```

### Comparing `ml-starter-0.0.28/ml/launchers/torchrun.py` & `ml-starter-0.0.29/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/loggers/base.py` & `ml-starter-0.0.29/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/loggers/meter.py` & `ml-starter-0.0.29/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/loggers/multi.py` & `ml-starter-0.0.29/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/loggers/stdout.py` & `ml-starter-0.0.29/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/loggers/tensorboard.py` & `ml-starter-0.0.29/ml/loggers/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import torch
 from omegaconf import MISSING, DictConfig, OmegaConf
 from torch import Tensor
 from torch.utils.tensorboard import SummaryWriter
 
 from ml.core.config import conf_field
+from ml.core.env import is_tensorboard_disabled
 from ml.core.registry import register_logger
 from ml.core.state import Phase, State
 from ml.loggers.base import BaseLogger, BaseLoggerConfig
 from ml.loggers.multi import TARGET_FPS, TARGET_SAMPLE_RATE
 from ml.utils.distributed import is_distributed, is_master
 from ml.utils.networking import get_unused_port
 
@@ -148,15 +149,15 @@
             port, use_localhost = get_unused_port(), False
 
         def make_localhost(s: str) -> str:
             if use_localhost:
                 s = re.sub(rf"://(.+?):{port}", f"://localhost:{port}", s)
             return s
 
-        if not self.config.start_in_subprocess or is_distributed():
+        if not self.config.start_in_subprocess or is_tensorboard_disabled():
             tensorboard_command_strs = [
                 "tensorboard serve \\",
                 f"  --logdir {self.tensorboard_log_directory} \\",
                 "  --bind_all \\",
                 f"  --port {port} \\",
                 "  --reload_interval 15",
             ]
```

### Comparing `ml-starter-0.0.28/ml/lr_schedulers/base.py` & `ml-starter-0.0.29/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.29/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.29/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/lr_schedulers/linear.py` & `ml-starter-0.0.29/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.29/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.29/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/models/activations.py` & `ml-starter-0.0.29/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/models/base.py` & `ml-starter-0.0.29/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/models/embeddings.py` & `ml-starter-0.0.29/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/models/init.py` & `ml-starter-0.0.29/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/models/norms.py` & `ml-starter-0.0.29/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/optimizers/adam.py` & `ml-starter-0.0.29/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/optimizers/adamw.py` & `ml-starter-0.0.29/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/optimizers/adan.py` & `ml-starter-0.0.29/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/optimizers/base.py` & `ml-starter-0.0.29/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/optimizers/sgd.py` & `ml-starter-0.0.29/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/optimizers/shampoo.py` & `ml-starter-0.0.29/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/scripts/cli.py` & `ml-starter-0.0.29/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/scripts/stage.py` & `ml-starter-0.0.29/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/base.py` & `ml-starter-0.0.29/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.29/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.29/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/collate.py` & `ml-starter-0.0.29/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.29/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.29/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.29/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.29/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.29/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/utils.py` & `ml-starter-0.0.29/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.29/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/environments/base.py` & `ml-starter-0.0.29/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/environments/utils.py` & `ml-starter-0.0.29/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/environments/worker.py` & `ml-starter-0.0.29/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/losses/reduce.py` & `ml-starter-0.0.29/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/rl/base.py` & `ml-starter-0.0.29/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/rl/replay.py` & `ml-starter-0.0.29/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/tasks/sl/base.py` & `ml-starter-0.0.29/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/base.py` & `ml-starter-0.0.29/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.29/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.29/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.29/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.29/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.29/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.29/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.29/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.29/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/rl.py` & `ml-starter-0.0.29/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/trainers/sl.py` & `ml-starter-0.0.29/ml/trainers/sl.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class EpochDoneException(Exception):
     """Raised when an epoch is done."""
 
 
 @dataclass
 class ValidationConfig:
     valid_every_n_steps: int | None = conf_field(100, help="Number of training steps to run per test step")
-    num_init_valid_steps: int | None = conf_field(2, help="Number of initial validation steps")
+    num_init_valid_steps: int | None = conf_field(1, help="Number of initial validation steps")
 
 
 @dataclass
 class SupervisedLearningTrainerConfig(VanillaTrainerConfig):
     validation: ValidationConfig = conf_field(ValidationConfig())
     batches_per_step: int = conf_field(1, help="Batches per training step, to simulate larger effective batch sizes")
 
@@ -205,11 +205,11 @@
                 "Finished training after %d epochs, %d steps, %d samples",
                 state.num_epochs,
                 state.num_steps,
                 state.num_samples,
             )
 
         except Exception:
-            logger.exception("Caught exception during training loop")
+            logger.exception("Caught exception during training loop for %s", self.config_path)
 
         finally:
             self.on_training_end(state, task, model, optim, lr_sched)
```

### Comparing `ml-starter-0.0.28/ml/trainers/vanilla.py` & `ml-starter-0.0.29/ml/trainers/vanilla.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This trainer expects the task to handle all the relevant movement of data and
 models to their associated devices.
 """
 
 import logging
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Callable, Generic, Iterator, TypeVar, cast
 
 import torch
 from omegaconf import II
 from torch import Tensor, nn
 from torch.optim import Optimizer
 
@@ -200,14 +201,20 @@
                 task.log_loss_dict(loss_dict, state)
             with self.step_context("write_logs"):
                 self.write_logs(task, model, state)
             with self.step_context("update_state"):
                 state.num_test_steps += 1
 
     def _init_environment(self) -> None:
+        root_logger = logging.getLogger()
+        for handler in root_logger.handlers:
+            if isinstance(handler, logging.FileHandler) and Path(handler.baseFilename).name == "main.log":
+                root_logger.removeHandler(handler)
+        root_logger.addHandler(logging.FileHandler("main.log"))
+
         # Sets up environment.
         if self.config.deterministic:
             torch.use_deterministic_algorithms(True)
         if self.config.use_tf32 and torch.cuda.is_available():
             torch.backends.cuda.matmul.allow_tf32 = True
 
         # Saves the config at the start of training.
```

### Comparing `ml-starter-0.0.28/ml/utils/argparse.py` & `ml-starter-0.0.29/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/atomic.py` & `ml-starter-0.0.29/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/augmentation.py` & `ml-starter-0.0.29/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/caching.py` & `ml-starter-0.0.29/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/call_train.py` & `ml-starter-0.0.29/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/cli.py` & `ml-starter-0.0.29/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/colors.py` & `ml-starter-0.0.29/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/data.py` & `ml-starter-0.0.29/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/device/auto.py` & `ml-starter-0.0.29/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/device/base.py` & `ml-starter-0.0.29/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/device/cpu.py` & `ml-starter-0.0.29/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/device/gpu.py` & `ml-starter-0.0.29/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/device/metal.py` & `ml-starter-0.0.29/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/distributed.py` & `ml-starter-0.0.29/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/image.py` & `ml-starter-0.0.29/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/io.py` & `ml-starter-0.0.29/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/large_models.py` & `ml-starter-0.0.29/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/logging.py` & `ml-starter-0.0.29/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/meter.py` & `ml-starter-0.0.29/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/staging.py` & `ml-starter-0.0.29/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/timer.py` & `ml-starter-0.0.29/ml/utils/timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 import threading
 import time
 import warnings
 from threading import Thread
 from typing import Any, Callable, TypeVar
 
 from ml.utils.colors import colorize
+from ml.utils.distributed import is_master
 
 timer_logger: logging.Logger = logging.getLogger(__name__)
 
 TimeoutFunc = TypeVar("TimeoutFunc", bound=Callable[..., Any])
 
 
 @functools.lru_cache
 def allow_spinners() -> bool:
     return (
         "PYTEST_CURRENT_TEST" not in os.environ
         and "pytest" not in sys.modules
         and sys.stdout.isatty()
         and os.environ.get("TERM") != "dumb"
+        and is_master()
     )
 
 
 class Spinner:
     def __init__(self, text: str | None = None) -> None:
         self._text = "" if text is None else text
         self._spinner_stop = False
```

### Comparing `ml-starter-0.0.28/ml/utils/torch_distributed.py` & `ml-starter-0.0.29/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml/utils/video.py` & `ml-starter-0.0.29/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.29/ml_starter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.28
+Version: 0.0.29
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.28/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.29/ml_starter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 ml/lr_schedulers/scripts/__init__.py
 ml/lr_schedulers/scripts/plot.py
 ml/models/__init__.py
 ml/models/activations.py
 ml/models/base.py
 ml/models/embeddings.py
 ml/models/init.py
+ml/models/lora.py
 ml/models/norms.py
 ml/optimizers/__init__.py
 ml/optimizers/adam.py
 ml/optimizers/adamw.py
 ml/optimizers/adan.py
 ml/optimizers/base.py
 ml/optimizers/sgd.py
```

### Comparing `ml-starter-0.0.28/pyproject.toml` & `ml-starter-0.0.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.28/setup.py` & `ml-starter-0.0.29/setup.py`

 * *Files identical despite different names*

