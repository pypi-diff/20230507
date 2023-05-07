# Comparing `tmp/tensorcircuit-nightly-0.9.0.dev20230505.tar.gz` & `tmp/tensorcircuit-nightly-0.9.0.dev20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.0.dev20230505.tar", last modified: Fri May  5 12:43:34 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.0.dev20230506.tar", last modified: Sat May  6 12:38:06 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.0.dev20230505.tar` & `tensorcircuit-nightly-0.9.0.dev20230506.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.129597 tensorcircuit-nightly-0.9.0.dev20230505/
--rw-r--r--   0 runner    (1001) docker     (122)    23650 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-05-05 12:43:34.129597 tensorcircuit-nightly-0.9.0.dev20230505/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.109597 tensorcircuit-nightly-0.9.0.dev20230505/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.117597 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27390 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 12:43:34.133597 tensorcircuit-nightly-0.9.0.dev20230505/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-05 12:43:27.000000 tensorcircuit-nightly-0.9.0.dev20230505/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.117597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-05-05 12:43:27.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.121597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.121597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.121597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.125597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.125597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.125597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.125597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.125597 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-05-05 12:43:33.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-05-05 12:43:33.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 12:43:33.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-05 12:43:33.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-05 12:43:33.000000 tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:43:34.129597 tensorcircuit-nightly-0.9.0.dev20230505/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-05 12:16:16.000000 tensorcircuit-nightly-0.9.0.dev20230505/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.422043 tensorcircuit-nightly-0.9.0.dev20230506/
+-rw-r--r--   0 runner    (1001) docker     (122)    23737 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20508 2023-05-06 12:38:06.422043 tensorcircuit-nightly-0.9.0.dev20230506/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18206 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.406043 tensorcircuit-nightly-0.9.0.dev20230506/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.410043 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6397 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8695 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-06 12:38:06.422043 tensorcircuit-nightly-0.9.0.dev20230506/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-06 12:38:00.000000 tensorcircuit-nightly-0.9.0.dev20230506/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.414043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-05-06 12:38:00.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.414043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.414043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.414043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17674 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7791 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.414043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.418043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.418043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.418043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.418043 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20508 2023-05-06 12:38:06.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-05-06 12:38:06.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 12:38:06.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-06 12:38:06.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-06 12:38:06.000000 tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 12:38:06.422043 tensorcircuit-nightly-0.9.0.dev20230506/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-06 12:15:16.000000 tensorcircuit-nightly-0.9.0.dev20230506/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/CHANGELOG.md` & `tensorcircuit-nightly-0.9.0.dev20230506/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Change Log
 
 ## Unreleased
 
+### Changed
+
+- Add compiler and cloud namespace to the global tensorcircuit namespace
+
 ## 0.9.0
 
 ### Added
 
 - Cloud module for Tencent QCloud is now merged into the master branch and ready to release
 
 - Add `tc.about()` to print related software versions and configs
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/HISTORY.md` & `tensorcircuit-nightly-0.9.0.dev20230506/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/LICENSE` & `tensorcircuit-nightly-0.9.0.dev20230506/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/PKG-INFO` & `tensorcircuit-nightly-0.9.0.dev20230506/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.0.dev20230505
+Version: 0.9.0.dev20230506
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -33,17 +33,17 @@
           <a href="./LICENSE">
             <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
           </a>
         </p>
         
         <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
         
-        TensorCircuit is the next generation of quantum circuit simulators with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
+        TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
         
-        TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms.
+        TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
         
         ## Getting Started
         
         Please begin with [Quick Start](/docs/source/quickstart.rst).
         
         For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
         
@@ -94,15 +94,15 @@
         
         We recommend you install this package with tensorflow also installed as:
         
         ```python
         pip install tensorcircuit[tensorflow]
         ```
         
-        Other optional dependencies include `[torch]`, `[jax]` and `[qiskit]`.
+        Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
         
         For the nightly build of tensorcircuit with new features, try:
         
         ```python
         pip uninstall tensorcircuit
         pip install tensorcircuit-nightly
         ```
@@ -198,30 +198,40 @@
         <!-- ALL-CONTRIBUTORS-LIST:END -->
         
         ## Research and Applications
         
         ### DQAS
         
         For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
-        Reference paper: https://arxiv.org/pdf/2010.08561.pdf (published in QST).
+        Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
         
         ### VQNHE
         
         For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
-        Reference paper: https://arxiv.org/pdf/2106.05105.pdf (published in PRL) and https://arxiv.org/pdf/2112.10380.pdf.
+        Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
         
         ### VQEX - MBL
         
         For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
-        Reference paper: https://arxiv.org/pdf/2111.13719.pdf (published in PRB).
+        Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
         
         ### Stark - DTC
         
         For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
-        Reference paper: https://arxiv.org/pdf/2208.02866.pdf (published in PRL).
+        Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
+        
+        ### EMQAOA-DARBO
+        
+        For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        Reference paper: https://arxiv.org/abs/2303.14877.
+        
+        ### TenCirChem
+        
+        [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+        Reference paper: https://arxiv.org/abs/2303.10825.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: jax
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/README.md` & `tensorcircuit-nightly-0.9.0.dev20230506/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
   <a href="./LICENSE">
     <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
   </a>
 </p>
 
 <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
 
-TensorCircuit is the next generation of quantum circuit simulators with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
+TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
 
-TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms.
+TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
 
 ## Getting Started
 
 Please begin with [Quick Start](/docs/source/quickstart.rst).
 
 For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
 
@@ -86,15 +86,15 @@
 
 We recommend you install this package with tensorflow also installed as:
 
 ```python
 pip install tensorcircuit[tensorflow]
 ```
 
-Other optional dependencies include `[torch]`, `[jax]` and `[qiskit]`.
+Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
 
 For the nightly build of tensorcircuit with new features, try:
 
 ```python
 pip uninstall tensorcircuit
 pip install tensorcircuit-nightly
 ```
@@ -190,23 +190,33 @@
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 ## Research and Applications
 
 ### DQAS
 
 For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
-Reference paper: https://arxiv.org/pdf/2010.08561.pdf (published in QST).
+Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
 
 ### VQNHE
 
 For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
-Reference paper: https://arxiv.org/pdf/2106.05105.pdf (published in PRL) and https://arxiv.org/pdf/2112.10380.pdf.
+Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
 
 ### VQEX - MBL
 
 For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
-Reference paper: https://arxiv.org/pdf/2111.13719.pdf (published in PRB).
+Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
 
 ### Stark - DTC
 
 For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
-Reference paper: https://arxiv.org/pdf/2208.02866.pdf (published in PRL).
+Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
+
+### EMQAOA-DARBO
+
+For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+Reference paper: https://arxiv.org/abs/2303.14877.
+
+### TenCirChem
+
+[TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+Reference paper: https://arxiv.org/abs/2303.10825.
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/README_cn.md` & `tensorcircuit-nightly-0.9.0.dev20230506/README_cn.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,20 @@
   <a href="./LICENSE">
     <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
   </a>
 </p>
 
 <p align="center"> <a href="README.md">English</a> |  简体中文 </p>
 
-TensorCircuit 是下一代量子电路模拟器，支持自动微分、即时编译、硬件加速和向量并行化。
+TensorCircuit 是下一代量子软件框架，支持自动微分、即时编译、硬件加速和向量并行化。
 
 TensorCircuit 建立在现代机器学习框架之上，并且与机器学习后端无关。 它特别适用于量子经典混合范式和变分量子算法的高效模拟。
 
+TensorCircuit 现在支持真实量子硬件连接和实验，并提供优雅的 CPU/GPU/QPU 混合部署方案（v0.9+）。
+
 ## 入门
 
 请从 [快速上手](/docs/source/quickstart.rst) 和 [Jupyter 教程](/docs/source/tutorials) 开始。
 
 有关更多信息和介绍，请参阅有用的 [示例脚本](/examples) 和 [完整文档](https://tensorcircuit.readthedocs.io/zh/latest/)。 [测试](/tests) 中的 API docstring 和测试用例也提供了丰富的信息。
 
 以下是一些最简易的演示。
@@ -82,15 +84,15 @@
 
 我们推荐安装时同时安装 TensorFlow，这可以通过以下安装可选项实现：
 
 ```python
 pip install tensorcircuit[tensorflow]
 ```
 
-其他安装选项包括： `[torch]`, `[jax]` and `[qiskit]`。
+其他安装选项包括： `[torch]`, `[jax]`, `[qiskit]` 和 `[cloud]`。
 
 此外我们有每日发布的最新版本 pip package，可以尝鲜开发的最新功能，请通过以下方式安装:
 
 ```python
 pip uninstall tensorcircuit
 pip install tensorcircuit-nightly
 ```
@@ -134,23 +136,33 @@
 我们欢迎大家提出 [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PR](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), 和 [讨论](https://github.com/tencent-quantum-lab/tensorcircuit/discussions)，这些都托管在 GitHub 上。
 
 ## 研究和应用
 
 ### DQAS
 
 可微量子架构搜索的应用见 [应用](/tensorcircuit/applications)。
-参考论文：https://arxiv.org/pdf/2010.08561.pdf (QST)。
+参考论文：https://arxiv.org/abs/2010.08561 (QST)。
 
 ### VQNHE
 
 关于变分量子神经混合本征求解器的应用，请参见 [应用](tensorcircuit/applications)。
-参考论文：https://arxiv.org/pdf/2106.05105.pdf (PRL) 和 https://arxiv.org/pdf/2112.10380.pdf 。
+参考论文：https://arxiv.org/abs/2106.05105 (PRL) 和 https://arxiv.org/abs/2112.10380 。
 
 ### VQEX - MBL
 
 VQEX 在 MBL 相位识别上的应用见 [教程](/docs/source/tutorials/vqex_mbl.ipynb)。
-参考论文: https://arxiv.org/pdf/2111.13719.pdf (PRB)。
+参考论文: https://arxiv.org/abs/2111.13719 (PRB)。
 
 ### Stark - DTC
 
 数值验证 Stark 多体局域化稳定的离散时间晶体，类似的 Floquet 系统模拟请参考 [例子](/examples/timeevolution_trotter.py).
-参考论文: https://arxiv.org/pdf/2208.02866.pdf (PRL).
+参考论文: https://arxiv.org/abs/2208.02866 (PRL).
+
+### EMQAOA-DARBO
+
+数值模拟和带错误消除的真实量子硬件实验验证 QAOA 优化的代码请参考 [项目](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+参考论文: https://arxiv.org/abs/2303.14877.
+
+### TenCirChem
+
+[TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) 是高效的，专注于处理和计算分子性质的量子计算软件。其基于 TensorCircuit 并为量子化学任务进行了专门的优化。
+参考论文: https://arxiv.org/abs/2303.10825.
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/conf.py` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     "sphinx_copybutton",
     "nbsphinx",
     "toctree_filter",
     "sphinx.ext.napoleon",
     "myst_parser",
 ]
 
+nbsphinx_allow_errors = True
+
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/index.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -8,39 +8,43 @@
 
 * It is built for human beings. 👽
 
 * It is designed for speed, flexibility and elegance. 🚀
 
 * It is empowered by advanced tensor network simulator engine. 🔋
 
+* It is ready for quantum hardware access with CPU/GPU/QPU hybrid deployment solutions. 🖥
+
 * It is implemented with industry-standard machine learning frameworks: TensorFlow, JAX, and PyTorch. 🤖
 
 * It is compatible with machine learning engineering paradigms: automatic differentiation, just-in-time compilation, vectorized parallelism and GPU acceleration. 🛠
 
+
 Links
 ----------
 
 TensorCircuit is created and maintained by `Shi-Xin Zhang <https://github.com/refraction-ray>`_ and this version of the software is released by `Tencent Quantum Lab <https://quantum.tencent.com/>`_.
 The current core authors of TensorCircuit are `Shi-Xin Zhang <https://github.com/refraction-ray>`_ and `Yu-Qin Chen <https://github.com/yutuer21>`_.
 We also thank `contributions <https://github.com/tencent-quantum-lab/tensorcircuit/graphs/contributors>`_ from the lab and the open source community.
 
 * Source code: https://github.com/tencent-quantum-lab/tensorcircuit
 
-* Software Whitepaper in Quantum: https://quantum-journal.org/papers/q-2023-02-02-912/
-
 * Documentation: https://tensorcircuit.readthedocs.io 
 
+* Software Whitepaper published in Quantum: https://quantum-journal.org/papers/q-2023-02-02-912/
+
 * Issue Tracker: https://github.com/tencent-quantum-lab/tensorcircuit/issues
 
 * Forum: https://github.com/tencent-quantum-lab/tensorcircuit/discussions
 
 * PyPI page: https://pypi.org/project/tensorcircuit
 
 * DockerHub page: https://hub.docker.com/repository/docker/tensorcircuit/tensorcircuit
 
+If you have any further questions or collaboration ideas in terms of TensorCircuit, please send email to shixinzhang#tencent.com.
 
 
 Reference Documentation
 ----------------------------
 
 The following documentation sections briefly introduce TensorCircuit to the users and developpers.
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/infras.rst`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 - :py:mod:`tensorcircuit.densitymatrix`: Referenced and highly efficient implementation of ``tc.DMCircuit`` class, with similar set API of ``tc.Circuit`` while simulating the noise in the full form of the density matrix.
 
 - :py:mod:`tensorcircuit.noisemodel`: The global noise configuration and circuit noisy method APIs
 
 **ML Interfaces Related Modules:**
 
-- :py:mod:`tensorcircuit.interfaces`: Provide interfaces when quantum simulation backend is different from neural libraries. Currently include PyTorch and scipy optimizer interfaces.
+- :py:mod:`tensorcircuit.interfaces`: Provide interfaces when quantum simulation backend is different from neural libraries. Currently include PyTorch, TensorFlow, NumPy and SciPy optimizer interfaces.
 
 - :py:mod:`tensorcircuit.keras`: Provide TensorFlow Keras layers, as well as wrappers of jitted function, save/load from tf side.
 
 - :py:mod:`tensorcircuit.torchnn`: Provide PyTorch nn Modules.
 
 **MPS and MPO Utiliy Modules:**
 
@@ -58,15 +58,21 @@
 
 - :py:mod:`tensorcircuit.vis`: Visualization code for circuit drawing.
 
 - :py:mod:`tensorcircuit.translation`: Translate circuit object to circuit object in other quantum packages.
 
 **Processing and error mitigation on sample results:**
 
-- :py:mod:`tensorcircuit.results`: Provide tools to process count dict and to apply error mitigation
+- :py:mod:`tensorcircuit.results`: Provide tools to process count dict and to apply error mitigation.
+
+**Cloud quantum hardware access module:**
+
+- :py:mod:`tensorcircuit.cloud`: Provide quantum cloud SDK that can access and program the real quantum hardware.
+
+- :py:mod:`tensorcircuit.compiler`: Provide compiler chains to compile and transform quantum circuits.
 
 **Shortcuts and Templates for Circuit Manipulation:**
 
 - :py:mod:`tensorcircuit.templates`: provide handy shortcuts functions for expectation or circuit building patterns.
 
 **Applications:**
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/modules.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     ./api/about.rst
     ./api/abstractcircuit.rst
     ./api/applications.rst
     ./api/backends.rst
     ./api/basecircuit.rst
     ./api/channels.rst
     ./api/circuit.rst
+    ./api/cloud.rst
     ./api/compiler.rst
     ./api/cons.rst
     ./api/densitymatrix.rst
     ./api/experimental.rst
     ./api/gates.rst
     ./api/interfaces.rst
     ./api/keras.rst
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/quickstart.rst`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 `Jax <https://github.com/google/jax#pip-installation-gpu-cuda>`_, 
 or `PyTorch <https://pytorch.org/get-started/locally/>`_.
 
 Docker is also recommended (especially Linux + Nvidia GPU setup): 
 
 ``sudo docker run -it --network host --gpus all tensorcircuit/tensorcircuit``.
 
+For more details on docker setup, please refer to `docker readme <https://github.com/tencent-quantum-lab/tensorcircuit/tree/master/docker>`_.
+
 - For Windows, due to the lack of support for Jax, we recommend to use docker or WSL, please refer to `TC via windows docker <contribs/development_windows.html>`_ or `TC via WSL <contribs/development_wsl2.html>`_.
 
 - For Mac with M series chips (arm architecture), please refer to `TC on Mac M series <contribs/development_MacARM.html>`_.
 
 Overall, the installation of TensorCircuit is simple, since it is purely in Python and hence very portable. 
 As long as the users can take care of the installation of ML frameworks on the corresponding system, TensorCircuit will work as expected.
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.0.dev20230506/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/setup.py` & `tensorcircuit-nightly-0.9.0.dev20230506/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.0.dev20230505"
+__version__ = "0.9.0.dev20230506"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
 
@@ -34,14 +34,16 @@
 from .gates import num_to_tensor, array_to_tensor
 from .vis import qir2tex, render_pdf
 from . import interfaces
 from . import templates
 from . import results
 from . import quantum
 from .quantum import QuOperator, QuVector, QuAdjointVector, QuScalar
+from . import compiler
+from . import cloud
 
 try:
     from . import keras
     from .keras import QuantumLayer as KerasLayer
 except ModuleNotFoundError:
     pass  # in case tf is not installed
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/apis.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 default_provider = Provider.from_name("tencent")
 avail_providers = ["tencent", "local"]
 
 
 def list_providers() -> List[Provider]:
     """
-    list all providers that tensorcircuit supports
+    list all cloud providers that tensorcircuit supports
 
     :return: _description_
     :rtype: List[Provider]
     """
     return [get_provider(s) for s in avail_providers]
 
 
@@ -81,15 +81,15 @@
 
 def set_device(
     provider: Optional[Union[str, Provider]] = None,
     device: Optional[Union[str, Device]] = None,
     set_global: bool = True,
 ) -> Device:
     """
-    _summary_
+    set the default device
 
     :param provider: provider of the device, defaults to None
     :type provider: Optional[Union[str, Provider]], optional
     :param device: the device, defaults to None
     :type device: Optional[Union[str, Device]], optional
     :param set_global: whether set, defaults to True,
         if False, equivalent to ``get_device``, defaults to True
@@ -409,14 +409,18 @@
     device: Optional[Union[str, Device]] = None,
     token: Optional[str] = None,
     **task_kws: Any,
 ) -> List[Task]:
     """
     submit task to the cloud platform, batch submission default enabled
 
+    .. seealso::
+
+        :py:meth:`tensorcircuit.cloud.tencent.submit_task`
+
     :param provider: _description_, defaults to None
     :type provider: Optional[Union[str, Provider]], optional
     :param device: _description_, defaults to None
     :type device: Optional[Union[str, Device]], optional
     :param token: _description_, defaults to None
     :type token: Optional[str], optional
     :param task_kws: all necessary keywords arguments for task submission,
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cloud/wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 logger = logging.getLogger(__name__)
 Tensor = Any
 
 
 def batch_submit_template(device: str) -> Callable[..., List[counts.ct]]:
-    # TODO(@refraction-ray): fixed when batch submission really works
+    # TODO(@refraction-ray): adpative batch
     def run(cs: Union[Circuit, Sequence[Circuit]], shots: int) -> List[counts.ct]:
         """
         batch circuit running alternative
         """
         single = False
         if not is_sequence(cs):
             cs = [cs]  # type: ignore
@@ -50,16 +50,21 @@
     x: Optional[Sequence[int]] = None,
     y: Optional[Sequence[int]] = None,
     z: Optional[Sequence[int]] = None,
     shots: int = 1024,
     device: Optional[Device] = None,
     **kws: Any,
 ) -> float:
-    # deprecated
-    # TODO(@refraction-ray): integrated error mitigation
+    """
+    Deprecated, please use :py:meth:`tensorcircuit.cloud.wrapper.batch_expectation_ps`.
+    """
+    logger.warning(
+        "This method is deprecated and not maintained, \
+        please use `tensorcircuit.cloud.wrapper.batch_expectation_ps` instead"
+    )
     c1 = Circuit.from_qir(c.to_qir())
     if x is None:
         x = []
     if y is None:
         y = []
     if z is None:
         z = []
@@ -79,22 +84,58 @@
     c: Circuit,
     pss: List[List[int]],
     device: Any = None,
     ws: Optional[List[float]] = None,
     shots: int = 8192,
     with_rem: bool = True,
 ) -> Union[Any, List[Any]]:
+    """
+    Unified interface to compute the Pauli string expectation lists or sums via simulation or on real qpu.
+    Error mitigation, circuit compilation and Pauli string grouping are all built-in.
+
+    One line access to unlock the whole power or real quantum hardware on quantum cloud.
+
+    :Example:
+
+    .. code-block:: python
+
+        c = tc.Circuit(2)
+        c.h(0)
+        c.x(1)
+        tc.cloud.wrapper.batch_expectation_ps(c, [[1, 0], [0, 3]], device=None)
+        # array([ 0.99999994, -0.99999994], dtype=float32)
+        tc.cloud.wrapper.batch_expectation_ps(c, [[1, 0], [0, 3]], device="tencent::9gmon")
+        # array([ 1.03093477, -1.11715944])
+
+    :param c: The target circuit to compute expectation
+    :type c: Circuit
+    :param pss: List of Pauli string list, eg. [[0, 1, 0], [2, 3, 3]] represents [X1, Y0Z1Z2].
+    :type pss: List[List[int]]
+    :param device: The device str or object for quantum cloud module,
+        defaults to None, None is for analytical exact simulation
+    :type device: Any, optional
+    :param ws: List of float to indicate the final return is the weighted sum of Pauli string expectations,
+        e.g. [2., -0.3] represents the final results is 2* ``pss`` [0]-0.3* ``pss`` [1]
+        defaults to None, None indicate the list of expectations for ``pss`` are all returned
+    :type ws: Optional[List[float]], optional
+    :param shots: measurement shots for each expectation estimation, defaults to 8192
+    :type shots: int, optional
+    :param with_rem: whether enable readout error mitigation for the result, defaults to True
+    :type with_rem: bool, optional
+    :return: List of Pauli string expectation or a weighted sum float for Pauli strings, depending on ``ws``
+    :rtype: Union[Any, List[Any]]
+    """
     if device is None:
         results = []
         for ps in pss:
             results.append(c.expectation_ps(**ps2xyz(ps)))  # type: ignore
         if ws is None:
-            return backend.stack(results)
+            return backend.real(backend.stack(results))
         else:
-            return backend.sum([w * r for w, r in zip(ws, results)])
+            return backend.real(backend.sum([w * r for w, r in zip(ws, results)]))
     cs = []
     infos = []
     exps = []
     if isinstance(device, str):
         device = get_device(device)
     for ps in pss:
         # TODO(@refraction-ray): Pauli string grouping
@@ -109,14 +150,15 @@
                 exp.append(j)
             elif i == 3:
                 exp.append(j)
         c1, info = qiskit_compile(
             c1,
             compiled_options={
                 "basis_gates": device.native_gates(),
+                # whether + "cx" here?
                 "optimization_level": 3,
                 "coupling_map": device.topology(),
             },
         )
         cs.append(c1)
         infos.append(info)
         exps.append(exp)
@@ -176,10 +218,10 @@
             for i in range(len(raw_counts))
         ]
     else:
         results = [
             counts.expectation(raw_counts[i], exps[i]) for i in range(len(raw_counts))
         ]
     if ws is not None:
-        sumr = sum([w * r for w, r in zip(ws, results)])
+        sumr = backend.sum([w * r for w, r in zip(ws, results)])
         return sumr
-    return results
+    return backend.stack(results)
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.0.dev20230505
+Version: 0.9.0.dev20230506
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -33,17 +33,17 @@
           <a href="./LICENSE">
             <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
           </a>
         </p>
         
         <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
         
-        TensorCircuit is the next generation of quantum circuit simulators with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
+        TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
         
-        TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms.
+        TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
         
         ## Getting Started
         
         Please begin with [Quick Start](/docs/source/quickstart.rst).
         
         For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
         
@@ -94,15 +94,15 @@
         
         We recommend you install this package with tensorflow also installed as:
         
         ```python
         pip install tensorcircuit[tensorflow]
         ```
         
-        Other optional dependencies include `[torch]`, `[jax]` and `[qiskit]`.
+        Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
         
         For the nightly build of tensorcircuit with new features, try:
         
         ```python
         pip uninstall tensorcircuit
         pip install tensorcircuit-nightly
         ```
@@ -198,30 +198,40 @@
         <!-- ALL-CONTRIBUTORS-LIST:END -->
         
         ## Research and Applications
         
         ### DQAS
         
         For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
-        Reference paper: https://arxiv.org/pdf/2010.08561.pdf (published in QST).
+        Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
         
         ### VQNHE
         
         For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
-        Reference paper: https://arxiv.org/pdf/2106.05105.pdf (published in PRL) and https://arxiv.org/pdf/2112.10380.pdf.
+        Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
         
         ### VQEX - MBL
         
         For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
-        Reference paper: https://arxiv.org/pdf/2111.13719.pdf (published in PRB).
+        Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
         
         ### Stark - DTC
         
         For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
-        Reference paper: https://arxiv.org/pdf/2208.02866.pdf (published in PRL).
+        Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
+        
+        ### EMQAOA-DARBO
+        
+        For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        Reference paper: https://arxiv.org/abs/2303.14877.
+        
+        ### TenCirChem
+        
+        [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+        Reference paper: https://arxiv.org/abs/2303.10825.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: jax
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.0.dev20230506/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/conftest.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_backends.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_channels.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_gates.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_keras.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_results.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_templates.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230505/tests/test_van.py` & `tensorcircuit-nightly-0.9.0.dev20230506/tests/test_van.py`

 * *Files identical despite different names*

