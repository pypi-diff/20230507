# Comparing `tmp/deepdoctection-0.22.tar.gz` & `tmp/deepdoctection-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdoctection-0.22.tar", last modified: Thu Mar 23 15:44:52 2023, max compression
+gzip compressed data, was "deepdoctection-0.23.tar", last modified: Sun May  7 17:40:46 2023, max compression
```

## Comparing `deepdoctection-0.22.tar` & `deepdoctection-0.23.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.498546 deepdoctection-0.22/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2022-06-16 05:58:47.000000 deepdoctection-0.22/LICENSE
--rw-rw-r--   0 janis     (1000) janis     (1000)    10337 2023-03-23 15:44:52.498546 deepdoctection-0.22/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     9613 2023-03-06 09:49:05.000000 deepdoctection-0.22/README.md
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.482546 deepdoctection-0.22/deepdoctection/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11794 2023-03-23 15:43:14.000000 deepdoctection-0.22/deepdoctection/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.482546 deepdoctection-0.22/deepdoctection/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      727 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11612 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/analyzer/dd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1762 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/analyzer/tools.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.482546 deepdoctection-0.22/deepdoctection/configs/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/configs/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1032 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/configs/conf_dd_one.yaml
--rw-rw-r--   0 janis     (1000) janis     (1000)       35 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/configs/conf_tesseract.yaml
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.482546 deepdoctection-0.22/deepdoctection/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6807 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/dataflow/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8413 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/dataflow/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6736 2023-02-23 18:53:18.000000 deepdoctection-0.22/deepdoctection/dataflow/custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20342 2023-03-23 15:29:43.000000 deepdoctection-0.22/deepdoctection/dataflow/custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15649 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/dataflow/parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/dataflow/serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9604 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/dataflow/stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19092 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datapoint/annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23301 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/datapoint/box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6824 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/datapoint/convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    24922 2023-03-23 15:29:43.000000 deepdoctection-0.22/deepdoctection/datapoint/image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    28073 2023-03-23 15:29:43.000000 deepdoctection-0.22/deepdoctection/datapoint/view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7391 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/datasets/adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18887 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/datasets/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4105 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/dataflow_builder.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19410 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/info.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/datasets/instances/doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-03-10 13:44:58.000000 deepdoctection-0.22/deepdoctection/datasets/instances/fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/instances/funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6491 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/instances/iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/instances/layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-02-20 09:20:02.000000 deepdoctection-0.22/deepdoctection/datasets/instances/publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11948 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/datasets/instances/pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8509 2023-03-23 15:29:43.000000 deepdoctection-0.22/deepdoctection/datasets/instances/pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/instances/rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/instances/xfund.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/datasets/instances/xsl/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/datasets/instances/xsl/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
--rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3326 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/datasets/save.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2022-06-30 08:30:21.000000 deepdoctection-0.22/deepdoctection/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19509 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/eval/accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4804 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/eval/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/eval/cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    16253 2023-02-23 18:53:18.000000 deepdoctection-0.22/deepdoctection/eval/eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/eval/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9101 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/eval/tedsmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5713 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/eval/tp_eval_callback.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1140 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11828 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10106 2023-02-13 09:06:49.000000 deepdoctection-0.22/deepdoctection/extern/d2detect.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7535 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9266 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/extern/hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    39080 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    42645 2023-03-10 14:26:38.000000 deepdoctection-0.22/deepdoctection/extern/model.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/pdftext.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/extern/pt/
--rw-rw-r--   0 janis     (1000) janis     (1000)      699 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/extern/pt/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2022-06-22 06:44:07.000000 deepdoctection-0.22/deepdoctection/extern/pt/ptutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12369 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4996 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/texocr.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/extern/tp/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/extern/tp/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2022-06-22 06:44:07.000000 deepdoctection-0.22/deepdoctection/extern/tp/tfutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpcompat.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3664 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/common.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.486546 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/config/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/config/config.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.490546 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9362 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13545 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11006 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17743 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4597 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4215 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/predict.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/preproc.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.490546 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-02-13 13:44:17.000000 deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6662 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/extern/tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.490546 deepdoctection-0.22/deepdoctection/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1390 2023-02-13 13:44:17.000000 deepdoctection-0.22/deepdoctection/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14674 2023-02-20 09:20:02.000000 deepdoctection-0.22/deepdoctection/mapper/cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6055 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/mapper/cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6463 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/mapper/d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5593 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/mapper/hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    33982 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/mapper/laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7775 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/mapper/maputils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7912 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/mapper/match.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-03-23 15:29:43.000000 deepdoctection-0.22/deepdoctection/mapper/misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2022-09-21 17:02:22.000000 deepdoctection-0.22/deepdoctection/mapper/pascalstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6876 2022-09-27 06:19:11.000000 deepdoctection-0.22/deepdoctection/mapper/prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23607 2023-03-23 15:29:43.000000 deepdoctection-0.22/deepdoctection/mapper/pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4687 2023-02-20 09:20:02.000000 deepdoctection-0.22/deepdoctection/mapper/tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8808 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/mapper/xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.490546 deepdoctection-0.22/deepdoctection/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1100 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13801 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/pipe/anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13221 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/pipe/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10805 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/pipe/cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11801 2023-02-13 13:44:17.000000 deepdoctection-0.22/deepdoctection/pipe/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6312 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/pipe/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8298 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/pipe/doctectionpipe.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6091 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/pipe/language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4589 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/pipe/layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/pipe/lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    21725 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/pipe/refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      902 2022-08-12 12:59:53.000000 deepdoctection-0.22/deepdoctection/pipe/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    45813 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/pipe/segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    26382 2023-01-30 19:58:28.000000 deepdoctection-0.22/deepdoctection/pipe/text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3138 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/pipe/transform.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.490546 deepdoctection-0.22/deepdoctection/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15612 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/train/d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10538 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/train/hf_detr_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19404 2023-02-03 14:03:14.000000 deepdoctection-0.22/deepdoctection/train/hf_layoutlm_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12968 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/train/tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.490546 deepdoctection-0.22/deepdoctection/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)     2238 2022-09-27 06:16:10.000000 deepdoctection-0.22/deepdoctection/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4612 2023-01-05 12:44:38.000000 deepdoctection-0.22/deepdoctection/utils/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3998 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/utils/context.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2022-09-12 13:32:10.000000 deepdoctection-0.22/deepdoctection/utils/detection_types.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3441 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/utils/develop.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17992 2023-02-23 18:53:12.000000 deepdoctection-0.22/deepdoctection/utils/file_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7626 2022-09-27 06:19:11.000000 deepdoctection-0.22/deepdoctection/utils/fs.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2022-06-16 05:58:47.000000 deepdoctection-0.22/deepdoctection/utils/identifier.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8627 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/utils/logger.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/utils/metacfg.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7564 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/utils/pdf_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11954 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/utils/settings.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1923 2023-01-27 07:53:16.000000 deepdoctection-0.22/deepdoctection/utils/systools.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1813 2022-09-12 13:32:10.000000 deepdoctection-0.22/deepdoctection/utils/tqdm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8247 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/utils/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2022-09-27 06:19:11.000000 deepdoctection-0.22/deepdoctection/utils/utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9216 2023-02-09 09:34:37.000000 deepdoctection-0.22/deepdoctection/utils/viz.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.482546 deepdoctection-0.22/deepdoctection.egg-info/
--rw-rw-r--   0 janis     (1000) janis     (1000)    10337 2023-03-23 15:44:52.000000 deepdoctection-0.22/deepdoctection.egg-info/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     7913 2023-03-23 15:44:52.000000 deepdoctection-0.22/deepdoctection.egg-info/SOURCES.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)        1 2023-03-23 15:44:52.000000 deepdoctection-0.22/deepdoctection.egg-info/dependency_links.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2175 2023-03-23 15:44:52.000000 deepdoctection-0.22/deepdoctection.egg-info/requires.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)       30 2023-03-23 15:44:52.000000 deepdoctection-0.22/deepdoctection.egg-info/top_level.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2346 2023-03-23 15:44:52.498546 deepdoctection-0.22/setup.cfg
--rw-rw-r--   0 janis     (1000) janis     (1000)     6249 2023-03-23 15:44:15.000000 deepdoctection-0.22/setup.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.494546 deepdoctection-0.22/tests/
--rw-rw-r--   0 janis     (1000) janis     (1000)      725 2022-09-18 14:33:32.000000 deepdoctection-0.22/tests/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.494546 deepdoctection-0.22/tests/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5142 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/analyzer/test_dd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17378 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    64681 2022-11-28 15:25:21.000000 deepdoctection-0.22/tests/data.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.494546 deepdoctection-0.22/tests/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/dataflow/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4337 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/dataflow/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/dataflow/test_custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/dataflow/test_custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/dataflow/test_parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/dataflow/test_stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.494546 deepdoctection-0.22/tests/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2022-09-06 06:55:23.000000 deepdoctection-0.22/tests/datapoint/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4860 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/datapoint/test_annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/datapoint/test_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/datapoint/test_convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11831 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/datapoint/test_image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3375 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/datapoint/test_view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.494546 deepdoctection-0.22/tests/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/datasets/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.494546 deepdoctection-0.22/tests/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      974 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/datasets/instances/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2022-11-03 14:05:55.000000 deepdoctection-0.22/tests/datasets/instances/test_doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/datasets/instances/test_fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2091 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/datasets/instances/test_funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1263 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/datasets/instances/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/datasets/instances/test_layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/datasets/instances/test_publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1921 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/datasets/instances/test_pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/datasets/instances/test_pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/datasets/instances/test_rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2704 2022-06-29 12:05:00.000000 deepdoctection-0.22/tests/datasets/test_adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/datasets/test_info.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/datasets/test_registry.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.494546 deepdoctection-0.22/tests/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/eval/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/eval/test_accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3803 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/eval/test_cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2952 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/eval/test_eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/eval/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1253 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/eval/test_tedsmetric.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.494546 deepdoctection-0.22/tests/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/extern/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/extern/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1652 2022-11-03 14:06:59.000000 deepdoctection-0.22/tests/extern/test_deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2860 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/extern/test_doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2142 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/extern/test_fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3781 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/extern/test_hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19460 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/extern/test_hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2066 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/extern/test_pdftext.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/extern/test_tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1734 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/extern/test_texocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4372 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/extern/test_tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.498546 deepdoctection-0.22/tests/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/mapper/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    81693 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/mapper/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10530 2023-03-10 14:33:06.000000 deepdoctection-0.22/tests/mapper/test_cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/mapper/test_cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1907 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/mapper/test_d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2050 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/mapper/test_hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2382 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/mapper/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5504 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/mapper/test_laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/mapper/test_misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2867 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/mapper/test_prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-03-10 14:21:40.000000 deepdoctection-0.22/tests/mapper/test_pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/mapper/test_tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/mapper/test_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/mapper/test_xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.498546 deepdoctection-0.22/tests/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6290 2022-10-24 07:01:39.000000 deepdoctection-0.22/tests/pipe/test_anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4498 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/pipe/test_cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3449 2023-02-13 13:44:17.000000 deepdoctection-0.22/tests/pipe/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3049 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/pipe/test_language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2022-10-24 07:01:39.000000 deepdoctection-0.22/tests/pipe/test_layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4604 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/pipe/test_lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9676 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/pipe/test_refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-02-13 13:44:17.000000 deepdoctection-0.22/tests/pipe/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14433 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests/pipe/test_segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9811 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/pipe/test_text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2022-11-03 14:06:59.000000 deepdoctection-0.22/tests/pipe/test_transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/test_utils.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.498546 deepdoctection-0.22/tests/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-01-27 07:53:16.000000 deepdoctection-0.22/tests/train/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2022-09-29 09:12:15.000000 deepdoctection-0.22/tests/train/test_d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3540 2022-10-12 13:27:51.000000 deepdoctection-0.22/tests/train/test_tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-03-23 15:44:52.498546 deepdoctection-0.22/tests_d2/
--rw-rw-r--   0 janis     (1000) janis     (1000)      761 2022-06-16 05:58:47.000000 deepdoctection-0.22/tests_d2/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1580 2022-09-21 17:02:23.000000 deepdoctection-0.22/tests_d2/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3226 2023-02-09 09:34:37.000000 deepdoctection-0.22/tests_d2/test_d2detect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.479299 deepdoctection-0.23/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2022-06-16 05:58:47.000000 deepdoctection-0.23/LICENSE
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10493 2023-05-07 17:40:46.479299 deepdoctection-0.23/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9769 2023-05-07 15:01:33.000000 deepdoctection-0.23/README.md
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11864 2023-05-07 17:39:00.000000 deepdoctection-0.23/deepdoctection/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11612 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/analyzer/dd.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/configs/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/configs/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1032 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/configs/conf_dd_one.yaml
+-rw-rw-r--   0 janis     (1000) janis     (1000)       35 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/configs/conf_tesseract.yaml
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6806 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/dataflow/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10039 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/dataflow/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6736 2023-02-23 18:53:18.000000 deepdoctection-0.23/deepdoctection/dataflow/custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20342 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/dataflow/custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15599 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/dataflow/parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/dataflow/serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9604 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/dataflow/stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19092 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datapoint/annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23301 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/datapoint/box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6824 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/datapoint/convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    27037 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/datapoint/image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    28742 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/datapoint/view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7391 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/datasets/adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18887 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/datasets/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4105 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/dataflow_builder.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19410 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/info.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/datasets/instances/doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/datasets/instances/fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6491 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-02-20 09:20:02.000000 deepdoctection-0.23/deepdoctection/datasets/instances/publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11948 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/datasets/instances/pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8509 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/datasets/instances/pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/instances/xfund.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/datasets/instances/xsl/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/datasets/instances/xsl/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3326 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/datasets/save.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2022-06-30 08:30:21.000000 deepdoctection-0.23/deepdoctection/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19509 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/eval/accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4804 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/eval/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/eval/cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    16253 2023-02-23 18:53:18.000000 deepdoctection-0.23/deepdoctection/eval/eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/eval/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9069 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/eval/tedsmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5713 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/eval/tp_eval_callback.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1140 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11828 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11010 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/extern/d2detect.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12381 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/extern/doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9319 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/extern/hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    39080 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    46200 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/extern/model.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/pdftext.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/pt/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      699 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/pt/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2022-06-22 06:44:07.000000 deepdoctection-0.23/deepdoctection/extern/pt/ptutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12369 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5654 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/extern/texocr.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2022-06-22 06:44:07.000000 deepdoctection-0.23/deepdoctection/extern/tp/tfutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpcompat.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3664 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/common.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/config/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/config/config.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9362 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13545 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11006 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17743 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4597 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4215 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/predict.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/preproc.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.467299 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-02-13 13:44:17.000000 deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7525 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/extern/tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/deepdoctection/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1390 2023-02-13 13:44:17.000000 deepdoctection-0.23/deepdoctection/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14674 2023-02-20 09:20:02.000000 deepdoctection-0.23/deepdoctection/mapper/cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6055 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6866 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/mapper/d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5593 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/mapper/hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    33982 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7775 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/maputils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7912 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/match.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/mapper/misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2022-09-21 17:02:22.000000 deepdoctection-0.23/deepdoctection/mapper/pascalstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6876 2022-09-27 06:19:11.000000 deepdoctection-0.23/deepdoctection/mapper/prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23607 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/mapper/pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5090 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/mapper/tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8808 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/mapper/xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/deepdoctection/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1100 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13801 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/pipe/anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13221 2023-04-11 09:55:32.000000 deepdoctection-0.23/deepdoctection/pipe/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10805 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/pipe/cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14447 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9425 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8816 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/doctectionpipe.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6075 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4589 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/pipe/layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/pipe/lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22256 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      902 2022-08-12 12:59:53.000000 deepdoctection-0.23/deepdoctection/pipe/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    47806 2023-05-07 17:37:06.000000 deepdoctection-0.23/deepdoctection/pipe/segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    29038 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/pipe/text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3138 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/pipe/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-05-07 15:01:33.000000 deepdoctection-0.23/deepdoctection/py.typed
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/deepdoctection/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15612 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/train/d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10538 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/train/hf_detr_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19404 2023-02-03 14:03:14.000000 deepdoctection-0.23/deepdoctection/train/hf_layoutlm_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12968 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/train/tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/deepdoctection/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2238 2022-09-27 06:16:10.000000 deepdoctection-0.23/deepdoctection/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4612 2023-01-05 12:44:38.000000 deepdoctection-0.23/deepdoctection/utils/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3998 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/context.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2022-09-12 13:32:10.000000 deepdoctection-0.23/deepdoctection/utils/detection_types.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3441 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/develop.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17992 2023-02-23 18:53:12.000000 deepdoctection-0.23/deepdoctection/utils/file_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7626 2022-09-27 06:19:11.000000 deepdoctection-0.23/deepdoctection/utils/fs.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2022-06-16 05:58:47.000000 deepdoctection-0.23/deepdoctection/utils/identifier.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8627 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/logger.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/metacfg.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7564 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/pdf_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11954 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/utils/settings.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1923 2023-01-27 07:53:16.000000 deepdoctection-0.23/deepdoctection/utils/systools.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1813 2022-09-12 13:32:10.000000 deepdoctection-0.23/deepdoctection/utils/tqdm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8247 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/utils/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2022-09-27 06:19:11.000000 deepdoctection-0.23/deepdoctection/utils/utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9216 2023-02-09 09:34:37.000000 deepdoctection-0.23/deepdoctection/utils/viz.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.463299 deepdoctection-0.23/deepdoctection.egg-info/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10493 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7904 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/SOURCES.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)        1 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/dependency_links.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/requires.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)       30 2023-05-07 17:40:46.000000 deepdoctection-0.23/deepdoctection.egg-info/top_level.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2346 2023-05-07 17:40:46.479299 deepdoctection-0.23/setup.cfg
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6406 2023-05-07 17:40:38.000000 deepdoctection-0.23/setup.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/tests/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      725 2022-09-18 14:33:32.000000 deepdoctection-0.23/tests/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/tests/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5142 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/analyzer/test_dd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17378 2023-05-03 16:43:31.000000 deepdoctection-0.23/tests/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    64681 2022-11-28 15:25:21.000000 deepdoctection-0.23/tests/data.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.471299 deepdoctection-0.23/tests/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/dataflow/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/dataflow/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/dataflow/test_custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/dataflow/test_custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/dataflow/test_parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/dataflow/test_stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2022-09-06 06:55:23.000000 deepdoctection-0.23/tests/datapoint/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4860 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/datapoint/test_annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/datapoint/test_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/datapoint/test_convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12141 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/datapoint/test_image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3670 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/datapoint/test_view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/datasets/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      974 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/datasets/instances/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2022-11-03 14:05:55.000000 deepdoctection-0.23/tests/datasets/instances/test_doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/datasets/instances/test_fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2091 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/datasets/instances/test_funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1263 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/datasets/instances/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/datasets/instances/test_layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/datasets/instances/test_publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1921 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/datasets/instances/test_pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/datasets/instances/test_pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/datasets/instances/test_rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2704 2022-06-29 12:05:00.000000 deepdoctection-0.23/tests/datasets/test_adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/datasets/test_info.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/datasets/test_registry.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/eval/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/eval/test_accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3803 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/eval/test_cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2952 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/eval/test_eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/eval/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1253 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/eval/test_tedsmetric.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/extern/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/extern/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1652 2022-11-03 14:06:59.000000 deepdoctection-0.23/tests/extern/test_deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4973 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/extern/test_doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2142 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/extern/test_fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3781 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/extern/test_hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19460 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/extern/test_hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2066 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/extern/test_pdftext.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/extern/test_tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1734 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/extern/test_texocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4372 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/extern/test_tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    81693 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/mapper/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10530 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/mapper/test_cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/mapper/test_cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1907 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/mapper/test_d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2050 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/mapper/test_hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2382 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/mapper/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5504 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/test_laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/test_misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2867 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/mapper/test_prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/mapper/test_pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/mapper/test_tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/test_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/mapper/test_xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6290 2022-10-24 07:01:39.000000 deepdoctection-0.23/tests/pipe/test_anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4498 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/pipe/test_cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3449 2023-02-13 13:44:17.000000 deepdoctection-0.23/tests/pipe/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3049 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/pipe/test_language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2022-10-24 07:01:39.000000 deepdoctection-0.23/tests/pipe/test_layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4604 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/pipe/test_lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9676 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/pipe/test_refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-05-07 15:01:33.000000 deepdoctection-0.23/tests/pipe/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14433 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests/pipe/test_segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9811 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/pipe/test_text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2022-11-03 14:06:59.000000 deepdoctection-0.23/tests/pipe/test_transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/test_utils.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.475299 deepdoctection-0.23/tests/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-01-27 07:53:16.000000 deepdoctection-0.23/tests/train/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2022-09-29 09:12:15.000000 deepdoctection-0.23/tests/train/test_d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3540 2022-10-12 13:27:51.000000 deepdoctection-0.23/tests/train/test_tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-05-07 17:40:46.479299 deepdoctection-0.23/tests_d2/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      761 2022-06-16 05:58:47.000000 deepdoctection-0.23/tests_d2/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1580 2022-09-21 17:02:23.000000 deepdoctection-0.23/tests_d2/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3226 2023-02-09 09:34:37.000000 deepdoctection-0.23/tests_d2/test_d2detect.py
```

### Comparing `deepdoctection-0.22/LICENSE` & `deepdoctection-0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/PKG-INFO` & `deepdoctection-0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.22
+Version: 0.23
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -49,19 +49,20 @@
 
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
- - Deskewing and rotating images with jdeskew. 
+ - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
    provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!) 
- - [**new!**] Table detection and table structure recognition with 
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). Check the notebook repo or 
+   the documentation on how to train a model on your custom task or how to setup a pipeline.
+ - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
@@ -140,22 +141,22 @@
 as possible. However, we are aware that there are still many areas where significant improvements can be made in terms 
 of clarity, grammar and correctness. We look forward to every hint and comment that increases the quality of the 
 documentation.
 
 
 ## Requirements
 
-![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.jpg)
+![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
 - Python >= 3.8
-- PyTorch >= 1.8 **or** Tensorflow >= 2.8 and CUDA. If you want to run the models provided by Tensorpack a GPU is
+- PyTorch >= 1.8 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
   required. You can run on PyTorch with a CPU only.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
```

### Comparing `deepdoctection-0.22/README.md` & `deepdoctection-0.23/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,20 @@
 
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
- - Deskewing and rotating images with jdeskew. 
+ - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
    provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!) 
- - [**new!**] Table detection and table structure recognition with 
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). Check the notebook repo or 
+   the documentation on how to train a model on your custom task or how to setup a pipeline.
+ - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
@@ -117,22 +118,22 @@
 as possible. However, we are aware that there are still many areas where significant improvements can be made in terms 
 of clarity, grammar and correctness. We look forward to every hint and comment that increases the quality of the 
 documentation.
 
 
 ## Requirements
 
-![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.jpg)
+![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
 - Python >= 3.8
-- PyTorch >= 1.8 **or** Tensorflow >= 2.8 and CUDA. If you want to run the models provided by Tensorpack a GPU is
+- PyTorch >= 1.8 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
   required. You can run on PyTorch with a CPU only.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
```

### Comparing `deepdoctection-0.22/deepdoctection/__init__.py` & `deepdoctection-0.23/deepdoctection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from typing import TYPE_CHECKING
 
 from packaging import version
 
 from .utils.file_utils import _LazyModule, get_tf_version, pytorch_available, tf_available
 from .utils.logger import logger
 
-__version__ = 0.22
+__version__ = 0.23
 
 _IMPORT_STRUCTURE = {
-    "analyzer": ["get_dd_analyzer", "build_analyzer", "load_page", "load_document"],
+    "analyzer": ["get_dd_analyzer", "build_analyzer"],
     "configs": [],
     "dataflow": [
         "DataFlowTerminated",
         "DataFlowResetStateNotCalled",
         "DataFlowReentrantGuard",
         "DataFlow",
         "RNGDataFlow",
@@ -29,14 +29,15 @@
         "TestDataSpeed",
         "FlattenData",
         "MapData",
         "MapDataComponent",
         "RepeatedData",
         "ConcatData",
         "JoinData",
+        "BatchData",
         "CacheData",
         "CustomDataFromList",
         "CustomDataFromIterable",
         "SerializerJsonlines",
         "SerializerTabsepFiles",
         "SerializerFiles",
         "CocoParser",
@@ -154,14 +155,15 @@
         "DoctrTextlineDetector",
         "DoctrTextRecognizer",
         "FasttextLangDetector",
         "HFDetrDerivedDetector",
         "HFLayoutLmTokenClassifierBase",
         "HFLayoutLmTokenClassifier",
         "HFLayoutLmv2TokenClassifier",
+        "HFLayoutLmv3TokenClassifier",
         "HFLayoutLmSequenceClassifier",
         "HFLayoutLmv2SequenceClassifier",
         "HFLayoutLmv3SequenceClassifier",
         "ModelProfile",
         "ModelCatalog",
         "print_model_infos",
         "ModelDownloadManager",
@@ -242,14 +244,15 @@
         "get_tokenizer_from_architecture",
         "LMTokenClassifierService",
         "LMSequenceClassifierService",
         "TableSegmentationRefinementService",
         "generate_html_string",
         "pipeline_component_registry",
         "TableSegmentationService",
+        "PubtablesSegmentationService",
         "SegmentationResult",
         "TextExtractionService",
         "TextOrderService",
         "SimpleTransformPipelineComponent",
     ],
     "train": [
         "D2Trainer",
```

### Comparing `deepdoctection-0.22/deepdoctection/analyzer/__init__.py` & `deepdoctection-0.23/deepdoctection/configs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""
-Package for pre-built pipelines
-"""
-
-from .dd import *
-from .tools import *
```

### Comparing `deepdoctection-0.22/deepdoctection/analyzer/dd.py` & `deepdoctection-0.23/deepdoctection/analyzer/dd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/configs/__init__.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/xsl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/configs/conf_dd_one.yaml` & `deepdoctection-0.23/deepdoctection/configs/conf_dd_one.yaml`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/dataflow/__init__.py` & `deepdoctection-0.23/deepdoctection/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/dataflow/base.py` & `deepdoctection-0.23/deepdoctection/dataflow/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def __iter__(self) -> Iterator[Any]:
         """
         * A dataflow is an iterable. The `__iter__` method should yield a list or dict each time.
           Note that dict is **partially** supported at the moment: certain dataflow does not support dict.
         * The `__iter__` method can be either finite (will stop iteration) or infinite
           (will not stop iteration). For a finite dataflow, `__iter__` can be called
           again immediately after the previous call returned.
-        * For many dataflow, the `__iter__` method is non-reentrant, which means for an dataflow
+        * For many dataflow, the `__iter__` method is non-reentrant, which means for a dataflow
           instance ``df``, `df.__iter__` cannot be called before the previous
           `df.__iter__` call has finished (iteration has stopped).
           When a dataflow is non-reentrant, `df.__iter__` should throw an exception if
           called before the previous call has finished.
           For such non-reentrant dataflows, if you need to use the same dataflow in two places,
           you need to create two dataflow instances.
         Yields:
```

### Comparing `deepdoctection-0.22/deepdoctection/dataflow/common.py` & `deepdoctection-0.23/deepdoctection/dataflow/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -231,20 +231,18 @@
         joined: {"a":c1, "b":c2, "c":c3}
 
     `JoinData` will stop once the first Dataflow throws a StopIteration
     """
 
     def __init__(self, df_lists: List[DataFlow]) -> None:
         """
-        Args:
-            df_lists (list): a list of DataFlow.
-                When these dataflows have different sizes, JoinData will stop when any
-                of them is exhausted.
-                The list could contain the same DataFlow instance more than once,
-                but note that in that case `__iter__` will then also be called many times.
+        :param df_lists: a list of DataFlow. When these dataflows have different sizes, JoinData will stop when any
+                        of them is exhausted.
+                        The list could contain the same DataFlow instance more than once,
+                        but note that in that case `__iter__` will then also be called many times.
         """
         self.df_lists = df_lists
 
     def reset_state(self) -> None:
         for df in set(self.df_lists):
             df.reset_state()
 
@@ -265,7 +263,50 @@
                 else:
                     dp = {}
                     for x in all_dps:
                         dp.update(x)
                 yield dp
         except StopIteration:  # some of them are exhausted
             pass
+
+
+class BatchData(ProxyDataFlow):
+    """
+    Stack datapoints into batches. It produces datapoints of the same number of components as `df`, but
+    each datapoint is now a list of datapoints.
+    """
+
+    def __init__(self, df: DataFlow, batch_size: int, remainder: bool = False) -> None:
+        """
+        :param df: A dataflow
+        :param batch_size: batch size
+        :param remainder: When the remaining datapoints in ``df`` is not enough to form a batch, whether or not to
+                          also produce the remaining data as a smaller batch.
+                          If set to `False`, all produced datapoints are guaranteed to have the same batch size.
+                          If set to `True`, `len(ds)` must be accurate.
+        """
+        super().__init__(df)
+        if not remainder:
+            if batch_size > len(df):
+                raise ValueError("Dataflow must be larger than batch_size")
+        self.batch_size = int(batch_size)
+        if self.batch_size <= 0:
+            raise ValueError("batch_size must be a positive integer")
+        self.remainder = remainder
+
+    def __len__(self) -> int:
+        df_size = len(self.df)
+        div = df_size // self.batch_size
+        rem = df_size % self.batch_size
+        if rem == 0:
+            return div
+        return div + int(self.remainder)
+
+    def __iter__(self) -> Iterator[Any]:
+        holder = []
+        for data in self.df:
+            holder.append(data)
+            if len(holder) == self.batch_size:
+                yield holder
+                holder = []
+        if self.remainder and len(holder) > 0:
+            yield holder
```

### Comparing `deepdoctection-0.22/deepdoctection/dataflow/custom.py` & `deepdoctection-0.23/deepdoctection/dataflow/custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/dataflow/custom_serialize.py` & `deepdoctection-0.23/deepdoctection/dataflow/custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/dataflow/parallel_map.py` & `deepdoctection-0.23/deepdoctection/dataflow/parallel_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             self.map_func = map_func
             self.pipename = pipename
             self.hwm = hwm
 
         @no_type_check
         def run(self):
             enable_death_signal(_warn=self.identity == b"0")
-            ctx = zmq.Context()  # pylint: disable=E0110
+            ctx = zmq.Context()
             socket = ctx.socket(zmq.REP)
             socket.setsockopt(zmq.IDENTITY, self.identity)
             socket.set_hwm(self.hwm)
             socket.connect(self.pipename)
 
             while True:
                 dp = PickleSerializer.loads(socket.recv(copy=False))
@@ -406,15 +406,15 @@
         return MultiProcessMapData._Worker(idx, self.map_func, pipename, hwm)
 
     def reset_state(self) -> None:
         _MultiProcessZMQDataFlow.reset_state(self)
         _ParallelMapData.reset_state(self)
         self._guard = DataFlowReentrantGuard()
 
-        self.context = zmq.Context()  # type: ignore  # pylint: disable=E0110
+        self.context = zmq.Context()  # type: ignore
         self.socket = self.context.socket(zmq.DEALER)  # type: ignore
         self.socket.set_hwm(self._buffer_size * 2)  # type: ignore
         pipename = _get_pipe_name("dataflow-map")
         _bind_guard(self.socket, pipename)
 
         self._proc_ids = [f"{k}".encode("utf-8") for k in range(self.num_proc)]
         worker_hwm = int(self._buffer_size * 2 // self.num_proc)
```

### Comparing `deepdoctection-0.22/deepdoctection/dataflow/serialize.py` & `deepdoctection-0.23/deepdoctection/dataflow/serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/dataflow/stats.py` & `deepdoctection-0.23/deepdoctection/dataflow/stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datapoint/__init__.py` & `deepdoctection-0.23/deepdoctection/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datapoint/annotation.py` & `deepdoctection-0.23/deepdoctection/datapoint/annotation.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datapoint/box.py` & `deepdoctection-0.23/deepdoctection/datapoint/box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datapoint/convert.py` & `deepdoctection-0.23/deepdoctection/datapoint/convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datapoint/image.py` & `deepdoctection-0.23/deepdoctection/datapoint/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Dataclass Image
 """
-
+import json
 from dataclasses import dataclass, field
+from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union, no_type_check
 
 import numpy as np
 from numpy import uint8
 
-from ..utils.detection_types import ImageType
+from ..utils.detection_types import ImageType, JsonDict, Pathlike
 from ..utils.identifier import get_uuid, is_uuid_like
 from ..utils.settings import ObjectTypes, get_type
 from .annotation import Annotation, BoundingBox, ImageAnnotation, SummaryAnnotation
 from .box import crop_box_from_image, global_to_local_coords, intersection_box
 from .convert import as_dict, convert_b64_to_np_array, convert_np_array_to_b64, convert_pdf_bytes_to_np_array_v2
 
 
@@ -530,14 +531,27 @@
                 if image_dict:
                     image_ann.image = cls.from_dict(**image_dict)
             image.dump(image_ann)
         if summary_dict := kwargs.get("_summary", kwargs.get("summary")):
             image.summary = SummaryAnnotation.from_dict(**summary_dict)
         return image
 
+    @classmethod
+    @no_type_check
+    def from_file(cls, file_path: str) -> "Image":
+        """
+        Create `Image` instance from .json file.
+
+        :param file_path: file_path
+        :return: Initialized image
+        """
+        with open(file_path, "r", encoding="UTF-8") as file:
+            image = Image.from_dict(**json.load(file))
+        return image
+
     @staticmethod
     def get_state_attributes() -> List[str]:
         """
         Returns the list of attributes that define the `state_id` of an image.
 
         :return: List of attributes
         """
@@ -573,7 +587,48 @@
                     else:
                         container_ids.append(str(element))
             elif isinstance(attr, np.ndarray):
                 container_ids.append(convert_np_array_to_b64(attr))
             else:
                 container_ids.append(str(attr))
         return get_uuid(self.image_id, *container_ids)
+
+    def save(
+        self,
+        image_to_json: bool = True,
+        highest_hierarchy_only: bool = False,
+        path: Optional[Pathlike] = None,
+        dry: bool = False,
+    ) -> Optional[JsonDict]:
+        """
+        Export image as dictionary. As numpy array cannot be serialized `image` values will be converted into
+        base64 encodings.
+        :param image_to_json: If True will save the image as b64 encoded string in output
+        :param highest_hierarchy_only: If True it will remove all image attributes of ImageAnnotations
+        :param path: Path to save the .json file to. If `None` results will be saved in the folder of the original
+                     document.
+        :param dry: Will run dry, i.e. without saving anything but returning the dict
+
+        :return: optional dict
+        """
+        if isinstance(path, str):
+            path = Path(path)
+        elif path is None:
+            path = Path(self.location)
+        if path.is_dir():
+            path = path / self.image_id
+        suffix = path.suffix
+        if suffix:
+            path_json = path.as_posix().replace(suffix, ".json")
+        else:
+            path_json = path.as_posix() + ".json"
+        if highest_hierarchy_only:
+            self.remove_image_from_lower_hierachy()
+        export_dict = self.as_dict()
+        export_dict["location"] = str(export_dict["location"])
+        if image_to_json and self.image is not None:
+            export_dict["_image"] = convert_np_array_to_b64(self.image)
+        if dry:
+            return export_dict
+        with open(path_json, "w", encoding="UTF-8") as file:
+            json.dump(export_dict, file, indent=2)
+        return None
```

### Comparing `deepdoctection-0.22/deepdoctection/datapoint/view.py` & `deepdoctection-0.23/deepdoctection/datapoint/view.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,30 +16,27 @@
 # limitations under the License.
 
 """
 Subclasses for ImageAnnotation and Image objects with various properties. These classes
 simplify consumption
 """
 
-import json
 from copy import copy
 from itertools import chain
-from pathlib import Path
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Type, Union, no_type_check
 
 import cv2
 import numpy as np
 
 from ..utils.detection_types import ImageType, JsonDict, Pathlike
 from ..utils.logger import logger
 from ..utils.settings import CellType, LayoutType, ObjectTypes, PageType, Relationships, TableType, WordType, get_type
 from ..utils.viz import draw_boxes, interactive_imshow
 from .annotation import ContainerAnnotation, ImageAnnotation, SummaryAnnotation, ann_from_dict
 from .box import BoundingBox
-from .convert import convert_np_array_to_b64
 from .image import Image
 
 
 class ImageAnnotationBaseView(ImageAnnotation):
     """
     Consumption class for having easier access to categories added to an ImageAnnotation.
 
@@ -276,14 +273,25 @@
     LayoutType.cell: Cell,
     CellType.projected_row_header: Cell,
     CellType.spanning: Cell,
     CellType.row_header: Cell,
     CellType.column_header: Cell,
 }
 
+IMAGE_DEFAULTS: Dict[str, Union[LayoutType, Sequence[ObjectTypes]]] = {
+    "text_container": LayoutType.word,
+    "top_level_text_block_names": [
+        LayoutType.table,
+        LayoutType.text,
+        LayoutType.title,
+        LayoutType.figure,
+        LayoutType.list,
+    ],
+}
+
 
 @no_type_check
 def ann_obj_view_factory(annotation: ImageAnnotation, text_container: ObjectTypes) -> ImageAnnotationBaseView:
     """
     Create an `ImageAnnotationBaseView` sub class given the mapping `IMAGE_ANNOTATION_TO_LAYOUTS` .
 
     :param annotation: The annotation to transform. Note, that we do not use the input annotation as base class
@@ -411,16 +419,16 @@
         """
         return self.get_annotation(category_names=LayoutType.table)
 
     @classmethod
     def from_image(
         cls,
         image_orig: Image,
-        text_container: ObjectTypes,
-        top_level_text_block_names: List[ObjectTypes],
+        text_container: Optional[ObjectTypes] = None,
+        top_level_text_block_names: Optional[List[ObjectTypes]] = None,
         text_block_names: Optional[List[ObjectTypes]] = None,
         base_page: Optional["Page"] = None,
     ) -> "Page":
         """
         Factory function for generating a `Page` instance from `image_orig` .
 
         :param image_orig: `Image` instance to convert
@@ -429,14 +437,21 @@
         :param text_block_names: name of image annotation that have a relation with text containers (or which might be
                                  text containers themselves). This is only necessary, when residual text_container (e.g.
                                  words that have not been assigned to any text block) should be displayed in `page.text`
         :param base_page: For top level objects that are images themselves, pass the page that encloses all objects.
                           In doubt, do not populate this value.
         :return:
         """
+
+        if text_container is None:
+            text_container = IMAGE_DEFAULTS["text_container"]  # type: ignore
+
+        if top_level_text_block_names is None:
+            top_level_text_block_names = IMAGE_DEFAULTS["top_level_text_block_names"]  # type: ignore
+
         img_kwargs = image_orig.as_dict()
         page = cls(
             img_kwargs.get("file_name"), img_kwargs.get("location"), img_kwargs.get("external_id")  # type: ignore
         )
         page.image_orig = image_orig
         page.page_number = image_orig.page_number
         page.document_id = image_orig.document_id
@@ -461,17 +476,17 @@
                     layout_ann.image = cls.from_image(
                         image, text_container, top_level_text_block_names, text_block_names, page
                     )
             layout_ann.base_page = base_page if base_page is not None else page
             page.dump(layout_ann)
         if summary_dict := img_kwargs.get("_summary"):
             page.summary = SummaryAnnotation.from_dict(**summary_dict)
-        page.top_level_text_block_names = top_level_text_block_names
+        page.top_level_text_block_names = top_level_text_block_names  # type: ignore
         page.text_block_names = text_block_names
-        page.text_container = text_container
+        page.text_container = text_container  # type: ignore
         return page
 
     def _order(self, block: str) -> List[ImageAnnotationBaseView]:
         blocks_with_order = [layout for layout in getattr(self, block) if layout.reading_order is not None]
         if self.residual_words:
             blocks_with_order.extend(self.residual_words)
         blocks_with_order.sort(key=lambda x: x.reading_order)
@@ -483,15 +498,15 @@
         Get text of all layouts.
         """
         text: str = ""
         block_name = "layouts" if self.layouts else "words"
         block_with_order = self._order(block_name)
         linebreak = "\n" if block_name == "layouts" else " "
         for block in block_with_order:
-            block_attr = "text" if block.category_name != LayoutType.word else "characters"
+            block_attr = "text" if not isinstance(block, Word) else "characters"
             text += f"{linebreak}{getattr(block, block_attr)}"
         return text
 
     @property
     def chunks(self) -> List[Tuple[str, str, str, str, str, str]]:
         """
         :return: Returns a "chunk" of a layout element or a table as 6-tuple containing
@@ -577,15 +592,21 @@
 
         if show_tables:
             for table in self.tables:
                 box_stack.append(table.bbox)
                 category_names_list.append(LayoutType.table)
                 if show_cells:
                     for cell in table.cells:
-                        if cell.category_name != LayoutType.cell:
+                        if cell.category_name in {
+                            LayoutType.cell,
+                            CellType.projected_row_header,
+                            CellType.spanning,
+                            CellType.row_header,
+                            CellType.column_header,
+                        }:
                             cells_found = True
                             box_stack.append(cell.bbox)
                             category_names_list.append(None)
                 if show_table_structure:
                     rows = table.rows
                     cols = table.columns
                     for row in rows:
@@ -593,15 +614,15 @@
                         category_names_list.append(None)
                     for col in cols:
                         box_stack.append(col.bbox)
                         category_names_list.append(None)
 
         if show_cells and not cells_found:
             for ann in self.annotations:
-                if isinstance(ann, Cell):
+                if isinstance(ann, Cell) and ann.active:
                     box_stack.append(ann.bbox)
                     category_names_list.append(None)
 
         if show_words:
             all_words = []
             for layout in self.layouts:
                 all_words.extend(layout.words)
@@ -649,31 +670,28 @@
         highest_hierarchy_only: bool = False,
         path: Optional[Pathlike] = None,
         dry: bool = False,
     ) -> Optional[JsonDict]:
         """
         Export image as dictionary. As numpy array cannot be serialized `image` values will be converted into
         base64 encodings.
-        :param image_to_json: If True will save the image as b64 encoded string in output
+        :param image_to_json: If `True` will save the image as b64 encoded string in output
         :param highest_hierarchy_only: If True it will remove all image attributes of ImageAnnotations
-        :param path: Path to save the .json file to
+        :param path: Path to save the .json file to. If `None` results will be saved in the folder of the original
+                     document.
         :param dry: Will run dry, i.e. without saving anything but returning the dict
 
         :return: optional dict
         """
-        if isinstance(path, str):
-            path = Path(path)
-        elif path is None:
-            path = Path(self.image_orig.location)
-        suffix = path.suffix
-        path_json = path.as_posix().replace(suffix, ".json")
-        if highest_hierarchy_only:
-            self.image_orig.remove_image_from_lower_hierachy()
-        export_dict = self.image_orig.as_dict()
-        export_dict["location"] = str(export_dict["location"])
-        if image_to_json and self.image_orig.image is not None:
-            export_dict["_image"] = convert_np_array_to_b64(self.image_orig.image)
-        if dry:
-            return export_dict
-        with open(path_json, "w", encoding="UTF-8") as file:
-            json.dump(export_dict, file)
-        return None
+        return self.image_orig.save(image_to_json, highest_hierarchy_only, path, dry)
+
+    @classmethod
+    @no_type_check
+    def from_file(
+        cls,
+        file_path: str,
+        text_container: Optional[ObjectTypes] = None,
+        top_level_text_block_names: Optional[List[ObjectTypes]] = None,
+        text_block_names: Optional[List[ObjectTypes]] = None,
+    ) -> "Page":
+        image = Image.from_file(file_path)
+        return cls.from_image(image, text_container, top_level_text_block_names, text_block_names)
```

### Comparing `deepdoctection-0.22/deepdoctection/datasets/__init__.py` & `deepdoctection-0.23/deepdoctection/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/adapter.py` & `deepdoctection-0.23/deepdoctection/datasets/adapter.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/base.py` & `deepdoctection-0.23/deepdoctection/datasets/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/dataflow_builder.py` & `deepdoctection-0.23/deepdoctection/datasets/dataflow_builder.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/info.py` & `deepdoctection-0.23/deepdoctection/datasets/info.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/__init__.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/doclaynet.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/fintabnet.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/funsd.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/funsd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/iiitar13k.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/layouttest.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/publaynet.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/pubtables1m.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/pubtables1m.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/pubtabnet.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/rvlcdip.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/xfund.py` & `deepdoctection-0.23/deepdoctection/datasets/instances/xfund.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/xsl/__init__.py` & `deepdoctection-0.23/tests/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/instances/xsl/pascal_voc.xsl` & `deepdoctection-0.23/deepdoctection/datasets/instances/xsl/pascal_voc.xsl`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/registry.py` & `deepdoctection-0.23/deepdoctection/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/datasets/save.py` & `deepdoctection-0.23/deepdoctection/datasets/save.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/eval/__init__.py` & `deepdoctection-0.23/deepdoctection/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/eval/accmetric.py` & `deepdoctection-0.23/deepdoctection/eval/accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/eval/base.py` & `deepdoctection-0.23/deepdoctection/eval/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/eval/cocometric.py` & `deepdoctection-0.23/deepdoctection/eval/cocometric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/eval/eval.py` & `deepdoctection-0.23/deepdoctection/eval/eval.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/eval/registry.py` & `deepdoctection-0.23/deepdoctection/eval/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/eval/tedsmetric.py` & `deepdoctection-0.23/deepdoctection/eval/tedsmetric.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,44 +207,44 @@
 @metric_registry.register("teds")
 class TedsMetric(MetricBase):
     """
     Metric induced by `teds`
     """
 
     metric = teds_metric  # type: ignore
-    mapper = Page.from_image  # type: ignore
+    mapper = Page.from_image
     structure_only = False
 
     @classmethod
     def dump(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> Tuple[List[str], List[str]]:
 
         dataflow_gt.reset_state()
         dataflow_predictions.reset_state()
 
         # gt and predictions are not necessarily in same order. Will need to reorder
         gt_dict = defaultdict(list)
         pred_dict = defaultdict(list)
         for dp_gt, dp_pred in zip(dataflow_gt, dataflow_predictions):
-            page_gt = cls.mapper(dp_gt, LayoutType.word, [LayoutType.table])  # type: ignore
+            page_gt = cls.mapper(dp_gt, LayoutType.word, [LayoutType.table])
             for table in page_gt.tables:
                 gt_dict[page_gt.image_id].append(table.html)
 
-            page_pred = cls.mapper(dp_pred, LayoutType.word, [LayoutType.table])  # type: ignore
+            page_pred = cls.mapper(dp_pred, LayoutType.word, [LayoutType.table])
             for table in page_pred.tables:
                 pred_dict[page_pred.image_id].append(table.html)
 
         gt_list = []
         pred_list = []
         for sample in gt_dict:
             gt_list.extend(gt_dict[sample])
             pred_list.extend(pred_dict[sample])
 
-        return gt_list, pred_list
+        return gt_list, pred_list  # type: ignore
 
     @classmethod
     def get_distance(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> List[JsonDict]:
         html_gt_list, html_pr_list = cls.dump(dataflow_gt, dataflow_predictions, categories)
```

### Comparing `deepdoctection-0.22/deepdoctection/eval/tp_eval_callback.py` & `deepdoctection-0.23/deepdoctection/eval/tp_eval_callback.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/__init__.py` & `deepdoctection-0.23/deepdoctection/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/base.py` & `deepdoctection-0.23/deepdoctection/extern/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/d2detect.py` & `deepdoctection-0.23/deepdoctection/extern/d2detect.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """
 D2 GeneralizedRCNN model as predictor for deepdoctection pipeline
 """
 
 from copy import copy
 from pathlib import Path
-from typing import Dict, List, Literal, Mapping, Optional
+from typing import Dict, List, Literal, Mapping, Optional, Sequence
 
 from ..utils.detection_types import ImageType, Requirement
 from ..utils.file_utils import (
     detectron2_available,
     get_detectron2_requirement,
     get_pytorch_requirement,
     pytorch_available,
@@ -128,14 +128,15 @@
     def __init__(
         self,
         path_yaml: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         config_overwrite: Optional[List[str]] = None,
         device: Optional[Literal["cpu", "cuda"]] = None,
+        filter_categories: Optional[Sequence[TypeOrStr]] = None,
     ):
         """
         Set up the predictor.
 
         The configuration of the model uses the full stack of build model tools of D2. For more information
         please check <https://detectron2.readthedocs.io/en/latest/tutorials/models.html#build-models-from-yacs-config>.
 
@@ -144,14 +145,16 @@
         :param path_weights: The path to the model checkpoint.
         :param categories: A dict with key (indices) and values (category names). Index 0 must be reserved for a
                            dummy 'BG' category. Note, that this convention is different from the builtin D2 framework,
                            where models in the model zoo are trained with 'BG' class having the highest index.
         :param config_overwrite:  Overwrite some hyperparameters defined by the yaml file with some new values. E.g.
                                  ["OUTPUT.FRCNN_NMS_THRESH=0.3","OUTPUT.RESULT_SCORE_THRESH=0.6"].
         :param device: "cpu" or "cuda". If not specified will auto select depending on what is available
+        :param filter_categories: The model might return objects that are not supposed to be predicted and that should
+                                  be filtered. Pass a list of category names that must not be returned
         """
 
         self.name = "_".join(Path(path_weights).parts[-3:])
         self._categories_d2 = self._map_to_d2_categories(copy(categories))
         if config_overwrite is None:
             config_overwrite = []
         self.path_weights = path_weights
@@ -163,14 +166,17 @@
         self.path_yaml = path_yaml
         self.categories = copy(categories)  # type: ignore
         self.config_overwrite = config_overwrite
         if device is not None:
             self.device = device
         else:
             self.device = set_torch_auto_device()
+        if filter_categories:
+            filter_categories = [get_type(cat) for cat in filter_categories]
+        self.filter_categories = filter_categories
         self.cfg = self._set_config(path_yaml, d2_conf_list, device)
         self.d2_predictor = D2FrcnnDetector.set_model(self.cfg)
         self._instantiate_d2_predictor()
 
     @staticmethod
     def _set_config(
         path_yaml: str, d2_conf_list: List[str], device: Optional[Literal["cpu", "cuda"]] = None
@@ -215,29 +221,42 @@
         )
         return self._map_category_names(detection_results)
 
     def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
         """
         Populating category names to detection results
 
-        :param detection_results: list of detection results
+        :param detection_results: list of detection results. Will also filter categories
         :return: List of detection results with attribute class_name populated
         """
+        filtered_detection_result: List[DetectionResult] = []
         for result in detection_results:
             result.class_name = self._categories_d2[str(result.class_id)]
             if isinstance(result.class_id, int):
                 result.class_id += 1
-        return detection_results
+            if self.filter_categories:
+                if result.class_name not in self.filter_categories:
+                    filtered_detection_result.append(result)
+            else:
+                filtered_detection_result.append(result)
+        return filtered_detection_result
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_pytorch_requirement(), get_detectron2_requirement()]
 
     @classmethod
     def _map_to_d2_categories(cls, categories: Mapping[str, TypeOrStr]) -> Dict[str, ObjectTypes]:
         return {str(int(k) - 1): get_type(v) for k, v in categories.items()}
 
     def clone(self) -> PredictorBase:
-        return self.__class__(self.path_yaml, self.path_weights, self.categories, self.config_overwrite, self.device)
+        return self.__class__(
+            self.path_yaml,
+            self.path_weights,
+            self.categories,
+            self.config_overwrite,
+            self.device,
+            self.filter_categories,
+        )
 
     def possible_categories(self) -> List[ObjectTypes]:
         return list(self.categories.values())
```

### Comparing `deepdoctection-0.22/deepdoctection/extern/deskew.py` & `deepdoctection-0.23/deepdoctection/extern/deskew.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/fastlang.py` & `deepdoctection-0.23/deepdoctection/extern/fastlang.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/hfdetr.py` & `deepdoctection-0.23/deepdoctection/extern/hfdetr.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     feature_extractor: "DetrFeatureExtractor",
     device: Literal["cpu", "cuda"],
     threshold: float,
     nms_threshold: float,
 ) -> List[DetectionResult]:
     """
     Calling predictor. Before doing that, tensors must be transferred to the device where the model is loaded. After
-    prediction it will present prediction in DetectionResult format-
+    running prediction it will present prediction in DetectionResult format-
 
     :param np_img: image as numpy array
     :param predictor: TableTransformerForObjectDetection
     :param feature_extractor: feature extractor
     :param device: device where the model is loaded
     :param threshold: Will filter all predictions with confidence score less threshold
     :param nms_threshold: Threshold to perform NMS on prediction outputs. (Note, that NMS does not belong to canonical
@@ -140,14 +140,15 @@
         """
         self.name = "Detr"
         self.categories = {idx: get_type(cat) for idx, cat in categories.items()}
         self.path_config = path_config_json
         self.path_weights = path_weights
         self.path_feature_extractor_config = path_feature_extractor_config_json
         self.config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=self.path_config)
+        self.config.use_timm_backbone = True
         self.config.threshold = 0.1
         self.config.nms_threshold = 0.05
         self.hf_detr_predictor = self.set_model(path_weights)
         self.feature_extractor = self.set_pre_processor()
 
         if device is not None:
             self.device = device
```

### Comparing `deepdoctection-0.22/deepdoctection/extern/hflayoutlm.py` & `deepdoctection-0.23/deepdoctection/extern/hflayoutlm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/model.py` & `deepdoctection-0.23/deepdoctection/extern/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     config: Optional[str] = field(default=None)
     preprocessor_config: Optional[str] = field(default=None)
     hf_repo_id: Optional[str] = field(default=None)
     hf_model_name: Optional[str] = field(default=None)
     hf_config_file: Optional[List[str]] = field(default=None)
     urls: Optional[List[str]] = field(default=None)
     categories: Optional[Dict[str, ObjectTypes]] = field(default=None)
+    dl_library: Optional[str] = field(default=None)
     model_wrapper: Optional[str] = field(default=None)
 
     def as_dict(self) -> Dict[str, Any]:
         """
         returns a dict of the dataclass
         """
         return asdict(self)
@@ -100,61 +101,66 @@
             categories={
                 "1": LayoutType.text,
                 "2": LayoutType.title,
                 "3": LayoutType.list,
                 "4": LayoutType.table,
                 "5": LayoutType.figure,
             },
+            dl_library="TF",
             model_wrapper="TPFrcnnDetector",
         ),
         "cell/model-1800000_inf_only.data-00000-of-00001": ModelProfile(
             name="cell/model-1800000_inf_only.data-00000-of-00001",
             description="Tensorpack cell detection model for inference purposes trained on Pubtabnet",
             config="dd/tp/conf_frcnn_cell.yaml",
             size=[274503056, 8056],
             tp_model=True,
             hf_repo_id="deepdoctection/tp_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
             hf_model_name="model-1800000_inf_only",
             hf_config_file=["conf_frcnn_cell.yaml"],
             categories={"1": LayoutType.cell},
+            dl_library="TF",
             model_wrapper="TPFrcnnDetector",
         ),
         "item/model-1620000_inf_only.data-00000-of-00001": ModelProfile(
             name="item/model-1620000_inf_only.data-00000-of-00001",
             description="Tensorpack row/column detection model for inference purposes trained on Pubtabnet",
             config="dd/tp/conf_frcnn_rows.yaml",
             size=[274515344, 7904],
             tp_model=True,
             hf_repo_id="deepdoctection/tp_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
             hf_model_name="model-1620000_inf_only",
             hf_config_file=["conf_frcnn_rows.yaml"],
             categories={"1": LayoutType.row, "2": LayoutType.column},
+            dl_library="TF",
             model_wrapper="TPFrcnnDetector",
         ),
         "item/model-1620000.data-00000-of-00001": ModelProfile(
             name="item/model-1620000.data-00000-of-00001",
             description="Tensorpack row/column detection model trained on Pubtabnet",
             config="dd/tp/conf_frcnn_rows.yaml",
             size=[823546048, 25787],
             tp_model=True,
             hf_repo_id="deepdoctection/tp_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc",
             hf_model_name="model-1620000",
             hf_config_file=["conf_frcnn_rows.yaml"],
             categories={"1": LayoutType.row, "2": LayoutType.column},
+            dl_library="TF",
             model_wrapper="TPFrcnnDetector",
         ),
         "layout/model-800000.data-00000-of-00001": ModelProfile(
             name="layout/model-800000.data-00000-of-00001",
             description="Tensorpack layout detection model trained on Publaynet",
             config="dd/tp/conf_frcnn_layout.yaml",
             size=[823656748, 25796],
             tp_model=True,
             hf_repo_id="deepdoctection/tp_casc_rcnn_X_32xd4_50_FPN_GN_2FC_publaynet",
             hf_model_name="model-800000",
             hf_config_file=["conf_frcnn_layout.yaml"],
+            dl_library="TF",
             categories={
                 "1": LayoutType.text,
                 "2": LayoutType.title,
                 "3": LayoutType.list,
                 "4": LayoutType.table,
                 "5": LayoutType.figure,
             },
@@ -166,14 +172,15 @@
             config="dd/tp/conf_frcnn_cell.yaml",
             size=[823509160, 25905],
             tp_model=True,
             hf_repo_id="deepdoctection/tp_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c",
             hf_model_name="model-1800000",
             hf_config_file=["conf_frcnn_cell.yaml"],
             categories={"1": LayoutType.cell},
+            dl_library="TF",
             model_wrapper="TPFrcnnDetector",
         ),
         "layout/d2_model-800000-layout.pkl": ModelProfile(
             name="layout/d2_model-800000-layout.pkl",
             description="Detectron2 layout detection model trained on Publaynet",
             config="dd/d2/layout/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274568239],
@@ -184,14 +191,15 @@
             categories={
                 "1": LayoutType.text,
                 "2": LayoutType.title,
                 "3": LayoutType.list,
                 "4": LayoutType.table,
                 "5": LayoutType.figure,
             },
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "layout/d2_model_0829999_layout_inf_only.pt": ModelProfile(
             name="layout/d2_model_0829999_layout_inf_only.pt",
             description="Detectron2 layout detection model trained on Publaynet",
             config="dd/d2/layout/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274632215],
@@ -202,14 +210,15 @@
             categories={
                 "1": LayoutType.text,
                 "2": LayoutType.title,
                 "3": LayoutType.list,
                 "4": LayoutType.table,
                 "5": LayoutType.figure,
             },
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "layout/d2_model_0829999_layout.pth": ModelProfile(
             name="layout/d2_model_0829999_layout.pth",
             description="Detectron2 layout detection model trained on Publaynet. Checkpoint for resuming training",
             config="dd/d2/layout/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[548377327],
@@ -220,86 +229,93 @@
             categories={
                 "1": LayoutType.text,
                 "2": LayoutType.title,
                 "3": LayoutType.list,
                 "4": LayoutType.table,
                 "5": LayoutType.figure,
             },
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "cell/d2_model-1800000-cell.pkl": ModelProfile(
             name="cell/d2_model-1800000-cell.pkl",
             description="Detectron2 cell detection inference only model trained on Pubtabnet",
             config="dd/d2/cell/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274519039],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
             hf_model_name="d2_model-1800000-cell.pkl",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.cell},
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "cell/d2_model_1849999_cell_inf_only.pt": ModelProfile(
             name="cell/d2_model_1849999_cell_inf_only.pt",
             description="Detectron2 cell detection inference only model trained on Pubtabnet",
             config="dd/d2/cell/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274583063],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
             hf_model_name="d2_model_1849999_cell_inf_only.pt",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.cell},
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "cell/d2_model_1849999_cell.pth": ModelProfile(
             name="cell/d2_model_1849999_cell.pth",
             description="Detectron2 cell detection inference only model trained on Pubtabnet",
             config="dd/d2/cell/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[548279023],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
             hf_model_name="cell/d2_model_1849999_cell.pth",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.cell},
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "item/d2_model-1620000-item.pkl": ModelProfile(
             name="item/d2_model-1620000-item.pkl",
             description="Detectron2 item detection inference only model trained on Pubtabnet",
             config="dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274531339],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
             hf_model_name="d2_model-1620000-item.pkl",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.row, "2": LayoutType.column},
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "item/d2_model_1639999_item.pth": ModelProfile(
             name="item/d2_model_1639999_item.pth",
             description="Detectron2 item detection model trained on Pubtabnet",
             config="dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[548303599],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
             hf_model_name="d2_model_1639999_item.pth",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.row, "2": LayoutType.column},
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "item/d2_model_1639999_item_inf_only.pt": ModelProfile(
             name="item/d2_model_1639999_item_inf_only.pt",
             description="Detectron2 item detection model inference only trained on Pubtabnet",
             config="dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274595351],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
             hf_model_name="d2_model_1639999_item_inf_only.pt",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.row, "2": LayoutType.column},
+            dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
         "microsoft/layoutlm-base-uncased/pytorch_model.bin": ModelProfile(
             name="microsoft/layoutlm-base-uncased/pytorch_model.bin",
             description="LayoutLM is a simple but effective pre-training method of text and layout for document image"
             " understanding and information extraction tasks, such as form understanding and receipt"
             " understanding. LayoutLM archived the SOTA results on multiple datasets. This model does not"
@@ -307,28 +323,30 @@
             "on 11M documents for 2 epochs.  Configuration: 12-layer, 768-hidden, 12-heads, 113M parameters",
             size=[453093832],
             tp_model=False,
             config="microsoft/layoutlm-base-uncased/config.json",
             hf_repo_id="microsoft/layoutlm-base-uncased",
             hf_model_name="pytorch_model.bin",
             hf_config_file=["config.json"],
+            dl_library="PT",
         ),
         "microsoft/layoutlm-large-uncased/pytorch_model.bin": ModelProfile(
             name="microsoft/layoutlm-large-uncased/pytorch_model.bin",
             description="LayoutLM is a simple but effective pre-training method of text and layout for document image"
             " understanding and information extraction tasks, such as form understanding and receipt"
             " understanding. LayoutLM archived the SOTA results on multiple datasets. This model does not"
             "contain any head and has to be fine tuned on a downstream task. This is model has been trained"
             " on 11M documents for 2 epochs.  Configuration: 24-layer, 1024-hidden, 16-heads, 343M parameters",
             size=[1361845448],
             tp_model=False,
             config="microsoft/layoutlm-large-uncased/config.json",
             hf_repo_id="microsoft/layoutlm-large-uncased",
             hf_model_name="pytorch_model.bin",
             hf_config_file=["config.json"],
+            dl_library="PT",
         ),
         "microsoft/layoutlmv2-base-uncased/pytorch_model.bin": ModelProfile(
             name="microsoft/layoutlmv2-base-uncased/pytorch_model.bin",
             description="LayoutLMv2 is an improved version of LayoutLM with new pre-training tasks to model the"
             " interaction among text, layout, and image in a single multi-modal framework. It outperforms"
             " strong baselines and achieves new state-of-the-art results on a wide variety of downstream"
             " visually-rich document understanding tasks, including , including FUNSD (0.7895 → 0.8420),"
@@ -336,14 +354,15 @@
             " (0.9443 → 0.9564), and DocVQA (0.7295 → 0.8672). The license is cc-by-nc-sa-4.0",
             size=[802243295],
             tp_model=False,
             config="microsoft/layoutlmv2-base-uncased/config.json",
             hf_repo_id="microsoft/layoutlmv2-base-uncased",
             hf_model_name="pytorch_model.bin",
             hf_config_file=["config.json"],
+            dl_library="PT",
         ),
         "microsoft/layoutxlm-base/pytorch_model.bin": ModelProfile(
             name="microsoft/layoutxlm-base/pytorch_model.bin",
             description="Multimodal pre-training with text, layout, and image has achieved SOTA performance for "
             "visually-rich document understanding tasks recently, which demonstrates the great potential"
             " for joint learning across different modalities. In this paper, we present LayoutXLM, a"
             " multimodal pre-trained model for multilingual document understanding, which aims to bridge"
@@ -355,14 +374,15 @@
             " SOTA cross-lingual pre-trained models on the XFUN dataset. The license is cc-by-nc-sa-4.0",
             size=[1476537178],
             tp_model=False,
             config="microsoft/layoutxlm-base/config.json",
             hf_repo_id="microsoft/layoutxlm-base",
             hf_model_name="pytorch_model.bin",
             hf_config_file=["config.json"],
+            dl_library="PT",
         ),
         "microsoft/layoutlmv3-base/pytorch_model.bin": ModelProfile(
             name="microsoft/layoutlmv3-base/pytorch_model.bin",
             description="LayoutLMv3 is a pre-trained multimodal Transformer for Document AI with unified text and"
             " image masking. The simple unified architecture and training objectives make LayoutLMv3 a"
             " general-purpose pre-trained model. For example, LayoutLMv3 can be fine-tuned for both"
             " text-centric tasks, including form understanding, receipt understanding, and document"
@@ -370,28 +390,30 @@
             " and document layout analysis. The license is cc-by-nc-sa-4.0",
             size=[501380823],
             tp_model=False,
             config="microsoft/layoutlmv3-base/config.json",
             hf_repo_id="microsoft/layoutlmv3-base",
             hf_model_name="pytorch_model.bin",
             hf_config_file=["config.json"],
+            dl_library="PT",
         ),
         "microsoft/table-transformer-detection/pytorch_model.bin": ModelProfile(
             name="microsoft/table-transformer-detection/pytorch_model.bin",
             description="Table Transformer (DETR) model trained on PubTables1M. It was introduced in the paper "
             "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents by Smock et "
             "al. This model is devoted to table detection",
             size=[115393245],
             tp_model=False,
             config="microsoft/table-transformer-detection/config.json",
             preprocessor_config="microsoft/table-transformer-detection/preprocessor_config.json",
             hf_repo_id="microsoft/table-transformer-detection",
             hf_model_name="pytorch_model.bin",
             hf_config_file=["config.json", "preprocessor_config.json"],
             categories={"1": LayoutType.table},
+            dl_library="PT",
             model_wrapper="HFDetrDerivedDetector",
         ),
         "microsoft/table-transformer-structure-recognition/pytorch_model.bin": ModelProfile(
             name="microsoft/table-transformer-structure-recognition/pytorch_model.bin",
             description="Table Transformer (DETR) model trained on PubTables1M. It was introduced in the paper "
             "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents by Smock et "
             "al. This model is devoted to table structure recognition and assumes to receive a cropped"
@@ -407,16 +429,61 @@
                 "1": LayoutType.table,
                 "2": LayoutType.column,
                 "3": LayoutType.row,
                 "4": CellType.column_header,
                 "5": CellType.projected_row_header,
                 "6": CellType.spanning,
             },
+            dl_library="PT",
             model_wrapper="HFDetrDerivedDetector",
         ),
+        "doctr/db_resnet50/pt/db_resnet50-ac60cadc.pt": ModelProfile(
+            name="doctr/db_resnet50/pt/db_resnet50-ac60cadc.pt",
+            description="Doctr implementation of DBNet from “Real-time Scene Text Detection with Differentiable "
+            "Binarization”. For more information please check "
+            "https://mindee.github.io/doctr/using_doctr/using_models.html#. This is the Pytorch artefact.",
+            size=[101971449],
+            urls=["https://doctr-static.mindee.com/models?id=v0.3.1/db_resnet50-ac60cadc.pt&src=0"],
+            categories={"1": LayoutType.word},
+            dl_library="PT",
+            model_wrapper="DoctrTextlineDetector",
+        ),
+        "doctr/db_resnet50/tf/db_resnet50-adcafc63.zip": ModelProfile(
+            name="doctr/db_resnet50/tf/db_resnet50-adcafc63.zip",
+            description="Doctr implementation of DBNet from “Real-time Scene Text Detection with Differentiable "
+            "Binarization”. For more information please check "
+            "https://mindee.github.io/doctr/using_doctr/using_models.html#. This is the Tensorflow artefact.",
+            size=[94178964],
+            urls=["https://doctr-static.mindee.com/models?id=v0.2.0/db_resnet50-adcafc63.zip&src=0"],
+            categories={"1": LayoutType.word},
+            dl_library="TF",
+            model_wrapper="DoctrTextlineDetector",
+        ),
+        "doctr/crnn_vgg16_bn/pt/crnn_vgg16_bn-9762b0b0.pt": ModelProfile(
+            name="doctr/crnn_vgg16_bn/pt/crnn_vgg16_bn-9762b0b0.pt",
+            description="Doctr implementation of CRNN from “An End-to-End Trainable Neural Network for Image-based "
+            "Sequence Recognition and Its Application to Scene Text Recognition”. For more information "
+            "please check https://mindee.github.io/doctr/using_doctr/using_models.html#. This is the Pytorch "
+            "artefact.",
+            size=[63286381],
+            urls=["https://doctr-static.mindee.com/models?id=v0.3.1/crnn_vgg16_bn-9762b0b0.pt&src=0"],
+            dl_library="PT",
+            model_wrapper="DoctrTextRecognizer",
+        ),
+        "doctr/crnn_vgg16_bn/tf/crnn_vgg16_bn-76b7f2c6.zip": ModelProfile(
+            name="doctr/crnn_vgg16_bn/tf/crnn_vgg16_bn-76b7f2c6.zip",
+            description="Doctr implementation of CRNN from “An End-to-End Trainable Neural Network for Image-based "
+            "Sequence Recognition and Its Application to Scene Text Recognition”. For more information "
+            "please check https://mindee.github.io/doctr/using_doctr/using_models.html#. This is the Tensorflow "
+            "artefact.",
+            size=[58758994],
+            urls=["https://doctr-static.mindee.com/models?id=v0.3.0/crnn_vgg16_bn-76b7f2c6.zip&src=0"],
+            dl_library="TF",
+            model_wrapper="DoctrTextRecognizer",
+        ),
         "fasttext/lid.176.bin": ModelProfile(
             name="fasttext/lid.176.bin",
             description="Fasttext language detection model",
             size=[131266198],
             urls=["https://dl.fbaipublicfiles.com/fasttext/supervised-models/lid.176.bin"],
             categories={
                 "__label__en": Languages.english,
@@ -784,15 +851,15 @@
             else:
                 model_name = profile.hf_model_name
                 if model_name is None:
                     # second try. Check if a url is provided
                     if profile.urls is None:
                         raise ValueError("hf_model_name and urls cannot be both None")
                     for url in profile.urls:
-                        file_names.append(url.split("/")[-1])
+                        file_names.append(url.split("/")[-1].split("&")[0])
                 else:
                     file_names.append(model_name)
             if profile.hf_repo_id:
                 ModelDownloadManager.load_model_from_hf_hub(profile, absolute_path_weights, file_names)
                 absolute_path_configs = ModelCatalog.get_full_path_configs(name)
                 ModelDownloadManager.load_configs_from_hf_hub(profile, absolute_path_configs)
             else:
```

### Comparing `deepdoctection-0.22/deepdoctection/extern/pdftext.py` & `deepdoctection-0.23/deepdoctection/extern/pdftext.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/pt/__init__.py` & `deepdoctection-0.23/deepdoctection/extern/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/pt/ptutils.py` & `deepdoctection-0.23/deepdoctection/extern/pt/ptutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tessocr.py` & `deepdoctection-0.23/deepdoctection/extern/tessocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/texocr.py` & `deepdoctection-0.23/deepdoctection/extern/texocr.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 AWS Textract OCR engine for text extraction
 """
 
+import sys
+import traceback
 from typing import List
 
 from ..datapoint.convert import convert_np_array_to_b64_b
 from ..utils.detection_types import ImageType, JsonDict, Requirement
-from ..utils.file_utils import boto3_available, get_aws_requirement, get_boto3_requirement
+from ..utils.file_utils import boto3_available, get_boto3_requirement
+from ..utils.logger import logger
 from ..utils.settings import LayoutType, ObjectTypes
 from .base import DetectionResult, ObjectDetector, PredictorBase
 
 if boto3_available():
     import boto3  # type:ignore
 
 
@@ -64,15 +67,29 @@
     :param np_img: Image in np.array.
     :param text_lines: If True, it will return DetectionResults of Text lines as well.
     :return: A list of textract extractions wrapped in DetectionResult
     """
 
     width, height = np_img.shape[1], np_img.shape[0]
     b_img = convert_np_array_to_b64_b(np_img)
-    response = client.detect_document_text(Document={"Bytes": b_img})
+    try:
+        response = client.detect_document_text(Document={"Bytes": b_img})
+    except:  # pylint: disable=W0702
+        _, exc_val, exc_tb = sys.exc_info()
+        frame_summary = traceback.extract_tb(exc_tb)[0]
+        log_dict = {
+            "file_name": "NN",
+            "error_type": type(exc_val).__name__,
+            "error_msg": str(exc_val),
+            "orig_module": frame_summary.filename,
+            "line": frame_summary.lineno,
+        }
+        logger.warning("botocore InvalidParameterException", log_dict)
+        response = {}
+
     all_results = _textract_to_detectresult(response, width, height, text_lines)
     return all_results
 
 
 class TextractOcrDetector(ObjectDetector):
     """
     Text object detector based on AWS Textract OCR engine. Note that an AWS account as well as some additional
@@ -93,21 +110,22 @@
         df = pipe.analyze(path="path/to/document.pdf")
 
         for dp in df:
             ...
 
     """
 
-    def __init__(self, text_lines: bool = False) -> None:
+    def __init__(self, text_lines: bool = False, **credentials_kwargs: str) -> None:
         """
         :param text_lines: If True, it will return DetectionResults of Text lines as well.
+        :param credentials_kwargs: `aws_access_key_id`, `aws_secret_access_key` or `aws_session_token`
         """
         self.name = "textract"
         self.text_lines = text_lines
-        self.client = boto3.client("textract")
+        self.client = boto3.client("textract", **credentials_kwargs)
         if self.text_lines:
             self.categories = {"1": LayoutType.word, "2": LayoutType.line}
         else:
             self.categories = {"1": LayoutType.word}
 
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         """
@@ -117,15 +135,15 @@
         :return: A list of DetectionResult
         """
 
         return predict_text(np_img, self.client, self.text_lines)
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
-        return [get_aws_requirement(), get_boto3_requirement()]
+        return [get_boto3_requirement()]
 
     def clone(self) -> PredictorBase:
         return self.__class__()
 
     def possible_categories(self) -> List[ObjectTypes]:
         if self.text_lines:
             return [LayoutType.word, LayoutType.line]
```

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/__init__.py` & `deepdoctection-0.23/deepdoctection/extern/tp/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tfutils.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tfutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpcompat.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpcompat.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/common.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/config/config.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/config/config.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/predict.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/predict.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/preproc.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/preproc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py` & `deepdoctection-0.23/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/extern/tpdetect.py` & `deepdoctection-0.23/deepdoctection/extern/tpdetect.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 """
 TP Faster RCNN model as predictor for deepdoctection pipeline
 """
 
 from copy import copy
 from pathlib import Path
-from typing import List, Mapping, Optional, Union
+from typing import List, Mapping, Optional, Sequence, Union
 
 from ..utils.detection_types import ImageType, Requirement
 from ..utils.file_utils import get_tensorflow_requirement, get_tensorpack_requirement, tensorpack_available
 from ..utils.metacfg import set_config_by_yaml
-from ..utils.settings import ObjectTypes, TypeOrStr
+from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 from .base import DetectionResult, ObjectDetector, PredictorBase
 
 if tensorpack_available():
     from .tp.tpcompat import TensorpackPredictor
     from .tp.tpfrcnn.config.config import model_frcnn_config
     from .tp.tpfrcnn.modeling.generalized_rcnn import ResNetFPNModel
     from .tp.tpfrcnn.predict import tp_predict_image
@@ -60,14 +60,15 @@
     def __init__(
         self,
         path_yaml: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         config_overwrite: Optional[List[str]] = None,
         ignore_mismatch: bool = False,
+        filter_categories: Optional[Sequence[TypeOrStr]] = None,
     ):
         """
         Set up the predictor.
 
         The configuration of the model is stored in a yaml-file, which needs to be passed through. For more details,
         please check
 
@@ -79,19 +80,24 @@
         :param path_weights: The path to the model checkpoint
         :param categories: A dict with key (indices) and values (category names). Index 0 must be reserved for a
                            dummy 'BG' category.
         :param config_overwrite: Overwrite some hyperparameters defined by the yaml file with some new values. E.g.
                                  ["OUTPUT.FRCNN_NMS_THRESH=0.3","OUTPUT.RESULT_SCORE_THRESH=0.6"]
         :param ignore_mismatch: When True will ignore mismatches between checkpoint weights and models. This is needed
                                 if a pre-trained model is to be fine-tuned on a custom dataset.
+        :param filter_categories: The model might return objects that are not supposed to be predicted and that should
+                                  be filtered. Pass a list of category names that must not be returned
         """
         self.name = "_".join(Path(path_weights).parts[-3:])
         self.path_yaml = path_yaml
         self.categories = copy(categories)  # type: ignore
         self.config_overwrite = config_overwrite
+        if filter_categories:
+            filter_categories = [get_type(cat) for cat in filter_categories]
+        self.filter_categories = filter_categories
         model = TPFrcnnDetector.set_model(path_yaml, self.categories, config_overwrite)
         super().__init__(model, path_weights, ignore_mismatch)
         assert self._number_gpus > 0, "Model only support inference with GPU"
 
     @staticmethod
     def set_model(
         path_yaml: str, categories: Mapping[str, ObjectTypes], config_overwrite: Union[List[str], None]
@@ -135,19 +141,30 @@
     def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
         """
         Populating category names to detection results
 
         :param detection_results: list of detection results
         :return: List of detection results with attribute class_name populated
         """
+        filtered_detection_result: List[DetectionResult] = []
         for result in detection_results:
             result.class_name = self._model.cfg.DATA.CLASS_DICT[str(result.class_id)]
-        return detection_results
+            if self.filter_categories:
+                if result.class_name not in self.filter_categories:
+                    filtered_detection_result.append(result)
+            else:
+                filtered_detection_result.append(result)
+        return filtered_detection_result
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_tensorflow_requirement(), get_tensorpack_requirement()]
 
     def clone(self) -> PredictorBase:
         return self.__class__(
-            self.path_yaml, self.path_weights, self.categories, self.config_overwrite, self.ignore_mismatch
+            self.path_yaml,
+            self.path_weights,
+            self.categories,
+            self.config_overwrite,
+            self.ignore_mismatch,
+            self.filter_categories,
         )
```

### Comparing `deepdoctection-0.22/deepdoctection/mapper/__init__.py` & `deepdoctection-0.23/deepdoctection/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/cats.py` & `deepdoctection-0.23/deepdoctection/mapper/cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/cocostruct.py` & `deepdoctection-0.23/deepdoctection/mapper/cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/d2struct.py` & `deepdoctection-0.23/deepdoctection/mapper/d2struct.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,25 +96,25 @@
 
     output["annotations"] = annotations
 
     return output
 
 
 def pt_nms_image_annotations(
-    anns: Sequence[ImageAnnotation], threshold: float, image_id: Optional[str] = None
+    anns: Sequence[ImageAnnotation], threshold: float, image_id: Optional[str] = None, prio: str = ""
 ) -> Sequence[str]:
     """
     Processing given image annotations through NMS. This is useful, if you want to supress some specific image
     annotation, e.g. given by name or returned through different predictors. This is the pt version, for tf check
     `mapper.tpstruct`
 
     :param anns: A sequence of ImageAnnotations. All annotations will be treated as if they belong to one category
     :param threshold: NMS threshold
     :param image_id: id in order to get the embedding bounding box
-
+    :param prio: If an annotation has prio, it will overwrite its given score to 1 so that it will never be suppressed
     :return: A list of annotation_ids that belong to the given input sequence and that survive the NMS process
     """
     if len(anns) == 1:
         return [anns[0].annotation_id]
     if not anns:
         return []
     ann_ids = np.array([ann.annotation_id for ann in anns], dtype="object")
@@ -125,15 +125,23 @@
         # if we do not have image embeddings but pass an image_id
         if not boxes.shape[0]:
             boxes = torch.tensor(
                 [ann.bounding_box.to_list(mode="xyxy") for ann in anns if ann.bounding_box is not None]
             )
     else:
         boxes = torch.tensor([ann.bounding_box.to_list(mode="xyxy") for ann in anns if ann.bounding_box is not None])
-    scores = torch.tensor([ann.score for ann in anns])
+
+    def priority_to_confidence(ann: ImageAnnotation, priority: str) -> float:
+        if ann.category_name == priority:
+            return 1.0
+        if ann.score:
+            return ann.score
+        raise ValueError("score cannot be None")
+
+    scores = torch.tensor([priority_to_confidence(ann, prio) for ann in anns])
     class_mask = torch.ones(len(boxes), dtype=torch.uint8)
     keep = batched_nms(boxes, scores, class_mask, threshold)
     ann_ids_keep = ann_ids[keep]
     if not isinstance(ann_ids_keep, str):
         return ann_ids_keep.tolist()
     return []
```

### Comparing `deepdoctection-0.22/deepdoctection/mapper/hfstruct.py` & `deepdoctection-0.23/deepdoctection/mapper/hfstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/laylmstruct.py` & `deepdoctection-0.23/deepdoctection/mapper/laylmstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/maputils.py` & `deepdoctection-0.23/deepdoctection/mapper/maputils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/match.py` & `deepdoctection-0.23/deepdoctection/mapper/match.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/misc.py` & `deepdoctection-0.23/deepdoctection/mapper/misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/pascalstruct.py` & `deepdoctection-0.23/deepdoctection/mapper/pascalstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/prodigystruct.py` & `deepdoctection-0.23/deepdoctection/mapper/prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/pubstruct.py` & `deepdoctection-0.23/deepdoctection/mapper/pubstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/mapper/tpstruct.py` & `deepdoctection-0.23/deepdoctection/mapper/tpstruct.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,25 +81,25 @@
 
     output["file_name"] = dp.location  # full path
 
     return output
 
 
 def tf_nms_image_annotations(
-    anns: Sequence[ImageAnnotation], threshold: float, image_id: Optional[str] = None
+    anns: Sequence[ImageAnnotation], threshold: float, image_id: Optional[str] = None, prio: str = ""
 ) -> Sequence[str]:
     """
     Processing given image annotations through NMS. This is useful, if you want to supress some specific image
     annotation, e.g. given by name or returned through different predictors. This is the tf version, for pt check
     `mapper.d2struct`
 
     :param anns: A sequence of ImageAnnotations. All annotations will be treated as if they belong to one category
     :param threshold: NMS threshold
     :param image_id: id in order to get the embedding bounding box
-
+    :param prio: If an annotation has prio, it will overwrite its given score to 1 so that it will never be suppressed
     :return: A list of annotation_ids that belong to the given input sequence and that survive the NMS process
     """
     if len(anns) == 1:
         return [anns[0].annotation_id]
     if not anns:
         return []
     ann_ids = np.array([ann.annotation_id for ann in anns], dtype="object")
@@ -111,14 +111,22 @@
             boxes = convert_to_tensor(
                 [ann.bounding_box.to_list(mode="xyxy") for ann in anns if ann.bounding_box is not None]
             )
     else:
         boxes = convert_to_tensor(
             [ann.bounding_box.to_list(mode="xyxy") for ann in anns if ann.bounding_box is not None]
         )
-    scores = convert_to_tensor([ann.score for ann in anns])
+
+    def priority_to_confidence(ann: ImageAnnotation, priority: str) -> float:
+        if ann.category_name == priority:
+            return 1.0
+        if ann.score:
+            return ann.score
+        raise ValueError("score cannot be None")
+
+    scores = convert_to_tensor([priority_to_confidence(ann, prio) for ann in anns])
     class_mask = convert_to_tensor(len(boxes), dtype=uint8)
     keep = non_max_suppression(boxes, scores, class_mask, iou_threshold=threshold)
     ann_ids_keep = ann_ids[keep]
     if not isinstance(ann_ids_keep, str):
         return ann_ids_keep.tolist()
     return []
```

### Comparing `deepdoctection-0.22/deepdoctection/mapper/xfundstruct.py` & `deepdoctection-0.23/deepdoctection/mapper/xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/pipe/__init__.py` & `deepdoctection-0.23/deepdoctection/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/pipe/anngen.py` & `deepdoctection-0.23/deepdoctection/pipe/anngen.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/pipe/base.py` & `deepdoctection-0.23/deepdoctection/pipe/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/pipe/cell.py` & `deepdoctection-0.23/deepdoctection/pipe/cell.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/pipe/common.py` & `deepdoctection-0.23/deepdoctection/pipe/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for common pipeline components
 """
 from copy import deepcopy
-from typing import List, Literal, Optional, Sequence, Union
+from typing import List, Literal, Mapping, Optional, Sequence, Union
 
 import numpy as np
 
 from ..dataflow import DataFlow, MapData
 from ..datapoint.image import Image
 from ..datapoint.view import Page
 from ..mapper.maputils import MappingContextManager
 from ..mapper.match import match_anns_by_intersection
+from ..mapper.misc import to_image
 from ..utils.detection_types import JsonDict
 from ..utils.file_utils import detectron2_available, pytorch_available, tf_available
 from ..utils.settings import LayoutType, ObjectTypes, Relationships, TypeOrStr, get_type
 from .base import PipelineComponent
 from .registry import pipeline_component_registry
 
 if tf_available():
@@ -176,14 +177,15 @@
                                ordered within all text blocks.
         :param top_level_text_block_names: name of image annotation that have a relation with text containers (or which
                                            might be text containers themselves).
         :param text_block_names: name of image annotation that have a relation with text containers (or which might be
                                  text containers themselves). This is only necessary, when residual text_container (e.g.
                                  words that have not been assigned to any text block) should be displayed in `page.text`
         """
+        self.name = "page_parser"
         if isinstance(top_level_text_block_names, (str, ObjectTypes)):
             top_level_text_block_names = [top_level_text_block_names]
         if isinstance(text_block_names, (str, ObjectTypes)):
             text_block_names = [text_block_names]
         if text_block_names is not None:
             text_block_names = [get_type(text_block) for text_block in text_block_names]
 
@@ -213,43 +215,113 @@
 
     def _init_sanity_checks(self) -> None:
         assert self._text_container in [
             LayoutType.word,
             LayoutType.line,
         ], f"text_container must be either {LayoutType.word} or {LayoutType.line}"
 
+    @staticmethod
+    def get_meta_annotation() -> JsonDict:
+        """
+        meta annotation. We do not generate any new annotations here
+        """
+        return dict([("image_annotations", []), ("sub_categories", {}), ("relationships", {}), ("summaries", [])])
+
+    def clone(self) -> "PageParsingService":
+        """clone"""
+        return self.__class__(
+            deepcopy(self._text_container), deepcopy(self._top_level_text_block_names), deepcopy(self._text_block_names)
+        )
+
 
 @pipeline_component_registry.register("AnnotationNmsService")
 class AnnotationNmsService(PipelineComponent):
     """
     A service to pass `ImageAnnotation` to a non-maximum suppression (NMS) process for given pairs of categories.
-    `ImageAnnotation`s are subjected to NMS process in groups: If `nms_pairs=[[LayoutType.text, LayoutType.table],
-    [LayoutType.title, LayoutType.table]]` all `ImageAnnotation` subject to these categories are being selected and
-     identified as one category. After NMS the discarded image annotation will be deactivated.
+    `ImageAnnotation`s are subjected to NMS process in groups:
+    If `nms_pairs=[[LayoutType.text, LayoutType.table],[LayoutType.title, LayoutType.table]]` all `ImageAnnotation`
+    subject to these categories are being selected and identified as one category.
+    After NMS the discarded image annotation will be deactivated.
     """
 
-    def __init__(self, nms_pairs: Sequence[Sequence[TypeOrStr]], thresholds: Union[float, List[float]]):
+    def __init__(
+        self,
+        nms_pairs: Sequence[Sequence[TypeOrStr]],
+        thresholds: Union[float, List[float]],
+        priority: Optional[List[Union[Optional[TypeOrStr]]]] = None,
+    ):
         """
         :param nms_pairs: Groups of categories, either as string or by `ObjectType`.
-        :param thresholds: Suppression threshold
+        :param thresholds: Suppression threshold. If only one value is provided, it will apply the threshold to all
+                           pairs. If a list is provided, make sure to add as many list elements as `nms_pairs`.
         """
         self.nms_pairs = [[get_type(val) for val in pair] for pair in nms_pairs]
         if isinstance(thresholds, float):
             self.threshold = [thresholds for _ in self.nms_pairs]
         else:
             assert len(self.nms_pairs) == len(thresholds), "Sequences of nms_pairs and thresholds must have same length"
             self.threshold = thresholds
+        if priority:
+            assert len(self.nms_pairs) == len(priority), "Sequences of nms_pairs and priority must have same length"
+
+            def _get_type(val: Optional[str]) -> Union[ObjectTypes, str]:
+                if val is None:
+                    return ""
+                return get_type(val)
+
+            self.priority = [_get_type(val) for val in priority]
+        else:
+            self.priority = [None for _ in self.nms_pairs]  # type: ignore
         super().__init__("nms")
 
     def serve(self, dp: Image) -> None:
-        for pair, threshold in zip(self.nms_pairs, self.threshold):
+        for pair, threshold, prio in zip(self.nms_pairs, self.threshold, self.priority):
             anns = dp.get_annotation(category_names=pair)
-            ann_ids_to_keep = nms_image_annotations(anns, threshold, dp.image_id)
+            ann_ids_to_keep = nms_image_annotations(anns, threshold, dp.image_id, prio)
             for ann in anns:
                 if ann.annotation_id not in ann_ids_to_keep:
                     self.dp_manager.deactivate_annotation(ann.annotation_id)
 
     def clone(self) -> "PipelineComponent":
         return self.__class__(deepcopy(self.nms_pairs), self.threshold)
 
     def get_meta_annotation(self) -> JsonDict:
         return dict([("image_annotations", []), ("sub_categories", {}), ("relationships", {}), ("summaries", [])])
+
+
+@pipeline_component_registry.register("ImageParsingService")
+class ImageParsingService:
+    """
+    A super light service that calls `to_image` when processing datapoints. Might be useful if you build a pipeline that
+    is not derived from `DoctectionPipe`.
+    """
+
+    def __init__(self, dpi: Optional[int] = None):
+        """
+        :param dpi: dpi resolution when converting PDFs into pixel values
+        """
+        self.name = "image"
+        self.dpi = dpi
+
+    def pass_datapoint(self, dp: Union[str, Mapping[str, Union[str, bytes]]]) -> Optional[Image]:
+        """pass a datapoint"""
+        return to_image(dp, self.dpi)
+
+    def predict_dataflow(self, df: DataFlow) -> DataFlow:
+        """
+        Mapping a datapoint via `pass_datapoint` within a dataflow pipeline
+
+        :param df: An input dataflow
+        :return: A output dataflow
+        """
+        return MapData(df, self.pass_datapoint)
+
+    def clone(self) -> "ImageParsingService":
+        """clone"""
+        return self.__class__(self.dpi)
+
+    @staticmethod
+    def get_meta_annotation() -> JsonDict:
+        """
+        meta annotation. We do not generate any new annotations here
+        """
+        return dict([("image_annotations", []), ("sub_categories", {}), ("relationships", {}), ("summaries", [])])
```

### Comparing `deepdoctection-0.22/deepdoctection/pipe/doctectionpipe.py` & `deepdoctection-0.23/deepdoctection/pipe/doctectionpipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: tpdoctectionpipe.py
+# File: doctectionpipe.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -17,34 +17,99 @@
 
 """
 Module for pipeline with Tensorpack predictors
 """
 
 import os
 from pathlib import Path
-from typing import Dict, List, Optional, Sequence, Union
+from typing import List, Mapping, Optional, Sequence, Tuple, Union
 
 from ..dataflow import DataFlow, MapData
 from ..dataflow.custom_serialize import SerializerFiles, SerializerPdfDoc
 from ..datapoint.image import Image
 from ..mapper.maputils import curry
 from ..mapper.misc import to_image
 from ..utils.detection_types import Pathlike
 from ..utils.fs import maybe_path_or_pdf
 from ..utils.logger import logger
 from ..utils.settings import LayoutType
 from .base import Pipeline, PipelineComponent, PredictorPipelineComponent
 from .common import PageParsingService
 
 
+def _collect_from_kwargs(
+    **kwargs: Union[str, DataFlow, bool, int, Pathlike, Union[str, List[str]]]
+) -> Tuple[Optional[str], Optional[str], bool, int, str, DataFlow]:
+    dataset_dataflow = kwargs.get("dataset_dataflow")
+    path = kwargs.get("path")
+    if path is None and dataset_dataflow is None:
+        raise ValueError("Pass either path or dataset_dataflow as argument")
+
+    shuffle = kwargs.get("shuffle", False)
+    if not isinstance(shuffle, bool):
+        raise TypeError(f"shuffle must be of type bool but is of type {type(shuffle)}")
+
+    doc_path = None
+    if path:
+        if not isinstance(path, (str, Path)):
+            raise TypeError("path must be of type PathOrStr")
+        path_type = maybe_path_or_pdf(path)
+        if path_type == 2:
+            doc_path = path
+            path = None
+        elif not path_type:
+            raise ValueError("Pass only a path to a directory or to a pdf file")
+
+    file_type = kwargs.get("file_type", [".jpg", ".png", ".tif"])
+
+    max_datapoints = kwargs.get("max_datapoints")
+    if not isinstance(max_datapoints, (int, type(None))):
+        raise TypeError(f"max_datapoints must be of type int, but is of type {type(max_datapoints)}")
+    return path, file_type, shuffle, max_datapoints, doc_path, dataset_dataflow  # type: ignore
+
+
+@curry
+def _proto_process(
+    dp: Union[str, Mapping[str, str]], path: Optional[str], doc_path: Optional[str]
+) -> Union[str, Mapping[str, str]]:
+    if isinstance(dp, str):
+        file_name = Path(dp).name
+    elif isinstance(dp, Image):
+        file_name = dp.file_name
+    else:
+        file_name = dp["file_name"]
+    if path is None:
+        path_tmp = doc_path
+    else:
+        path_tmp = path
+    logger.info("Processing %s", file_name, {"path": path_tmp, "df": path_tmp, "file_name": file_name})
+    return dp
+
+
+@curry
+def _to_image(dp: Union[str, Mapping[str, Union[str, bytes]]], dpi: Optional[int] = None) -> Optional[Image]:
+    return to_image(dp, dpi)
+
+
+def _doc_to_dataflow(path: Pathlike, max_datapoints: Optional[int] = None) -> DataFlow:
+    if not os.path.isfile(path):
+        raise FileExistsError(f"{path} not a file")
+
+    df = SerializerPdfDoc.load(path, max_datapoints=max_datapoints)
+
+    return df
+
+
 class DoctectionPipe(Pipeline):
     """
     Prototype for a document layout pipeline. Contains implementation for loading document types (images in directory,
     single PDF document, dataflow from datasets), conversions in dataflows and building a pipeline.
 
+
+
     See `deepdoctection.analyzer.dd` for a concrete implementation.
 
     See also the explanations in `base.Pipeline`.
 
     By default, `DoctectionPipe` will instantiate a default `PageParsingService`
 
         PageParsingService(text_container=LayoutType.word,
@@ -68,62 +133,34 @@
         )
         assert all(
             isinstance(element, (PipelineComponent, PredictorPipelineComponent)) for element in pipeline_component_list
         )
         super().__init__(pipeline_component_list)
 
     def _entry(self, **kwargs: Union[str, DataFlow, bool, int, Pathlike, Union[str, List[str]]]) -> DataFlow:
-        dataset_dataflow = kwargs.get("dataset_dataflow")
-        path = kwargs.get("path")
-        if path is None and dataset_dataflow is None:
-            raise ValueError("Pass either path or dataset_dataflow as argument")
-
-        shuffle = kwargs.get("shuffle", False)
-        if not isinstance(shuffle, bool):
-            raise TypeError(f"shuffle must be of type bool but is of type {type(shuffle)}")
-
-        doc_path = None
-        if path:
-            if not isinstance(path, (str, Path)):
-                raise TypeError("path must be of type PathOrStr")
-            path_type = maybe_path_or_pdf(path)
-            if path_type == 2:
-                doc_path = path
-                path = None
-            elif not path_type:
-                raise ValueError("Pass only a path to a directory or to a pdf file")
-
-        file_type = kwargs.get("file_type", [".jpg", ".png", ".tif"])
-
-        max_datapoints = kwargs.get("max_datapoints")
-        if not isinstance(max_datapoints, (int, type(None))):
-            raise TypeError(f"max_datapoints must be of type int, but is of type {type(max_datapoints)}")
+        path, file_type, shuffle, max_datapoints, doc_path, dataset_dataflow = _collect_from_kwargs(**kwargs)
+
         df: DataFlow
 
         if isinstance(path, (str, Path)):
             if not isinstance(file_type, (str, list)):
                 raise TypeError(f"file_type must be of type string or list, but is of type {type(file_type)}")
             df = DoctectionPipe.path_to_dataflow(path, file_type, shuffle=shuffle)
-        if isinstance(doc_path, (str, Path)):
+        elif isinstance(doc_path, (str, Path)):
             df = DoctectionPipe.doc_to_dataflow(
                 path=doc_path, max_datapoints=int(max_datapoints) if max_datapoints is not None else None
             )
-        if dataset_dataflow is not None and isinstance(dataset_dataflow, DataFlow):
+        elif dataset_dataflow is not None and isinstance(dataset_dataflow, DataFlow):
             df = dataset_dataflow
+        else:
+            raise BrokenPipeError("Cannot build Dataflow")
 
-        def _proto_process(dp: Image) -> Image:
-            if path is None:
-                path_tmp = doc_path
-            else:
-                path_tmp = path  # type: ignore
-            logger.info("Processing %s", dp.file_name, {"path": path_tmp, "df": path_tmp, "file_name": dp.file_name})
-            return dp
-
-        df = MapData(df, _proto_process)
-
+        df = MapData(df, _proto_process(path, doc_path))
+        if dataset_dataflow is None:
+            df = MapData(df, _to_image(dpi=300))  # pylint: disable=E1120
         return df
 
     @staticmethod
     def path_to_dataflow(
         path: Pathlike,
         file_type: Union[str, Sequence[str]],
         max_datapoints: Optional[int] = None,
@@ -137,43 +174,26 @@
         :param max_datapoints: max number of datapoints to consider
         :param shuffle: Shuffle file names in order to stream them randomly
         :return: dataflow
         """
         if not os.path.isdir(path):
             raise NotADirectoryError(f"{path} not a directory")
         df = SerializerFiles.load(path, file_type, max_datapoints, shuffle)
-
-        def _to_image(dp: str) -> Optional[Image]:
-            _, file_name = os.path.split(dp)
-            dp_dict = {"file_name": file_name, "location": dp}
-            return to_image(dp_dict)
-
-        df = MapData(df, _to_image)
         return df
 
     @staticmethod
     def doc_to_dataflow(path: Pathlike, max_datapoints: Optional[int] = None) -> DataFlow:
         """
         Processing method for documents
 
         :param path: path to directory
         :param max_datapoints: max number of datapoints to consider
         :return: dataflow
         """
-        if not os.path.isfile(path):
-            raise FileExistsError(f"{path} not a file")
-
-        df = SerializerPdfDoc.load(path, max_datapoints=max_datapoints)
-
-        @curry
-        def _to_image(dp: Union[str, Dict[str, Union[str, bytes]]], dpi: Optional[int] = None) -> Optional[Image]:
-            return to_image(dp, dpi)
-
-        df = MapData(df, _to_image(dpi=300))  # pylint: disable=E1120
-        return df
+        return _doc_to_dataflow(path, max_datapoints)
 
     def dataflow_to_page(self, df: DataFlow) -> DataFlow:
         """
         Converts a dataflow of images to a dataflow of pages
 
         :param df: Dataflow
         :return: Dataflow
```

### Comparing `deepdoctection-0.22/deepdoctection/pipe/language.py` & `deepdoctection-0.23/deepdoctection/pipe/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         self._init_sanity_checks()
         super().__init__(
             self._get_name(self.predictor.name)
         )  # cannot use PredictorPipelineComponent class because of return type of predict meth
 
     def serve(self, dp: Image) -> None:
         if self.text_detector is None:
-            page = Page.from_image(dp, self.text_container, self.text_block_names)  # type: ignore
+            page = Page.from_image(dp, self.text_container, self.text_block_names)
             text = page.text_no_line_break
         else:
             if dp.image is None:
                 raise ValueError("dp.image cannot be None")
             detect_result_list = self.text_detector.predict(dp.image)
             # this is a concatenation of all detection result. No reading order
             text = " ".join([result.text for result in detect_result_list if result.text is not None])
```

### Comparing `deepdoctection-0.22/deepdoctection/pipe/layout.py` & `deepdoctection-0.23/deepdoctection/pipe/layout.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/pipe/lm.py` & `deepdoctection-0.23/deepdoctection/pipe/lm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/pipe/refine.py` & `deepdoctection-0.23/deepdoctection/pipe/refine.py`

 * *Files 3% similar despite different names*

```diff
@@ -455,14 +455,23 @@
 
             cells = table.image.get_annotation(category_names=self._cell_names)
             number_of_rows = max([int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells])
             number_of_cols = max([int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells])
             max_row_span = max([int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells])
             max_col_span = max([int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells])
             # TODO: the summaries should be sub categories of the underlying ann
+            if TableType.number_of_rows in table.sub_categories:
+                table.remove_sub_category(TableType.number_of_rows)
+            if TableType.number_of_columns in table.sub_categories:
+                table.remove_sub_category(TableType.number_of_columns)
+            if TableType.max_row_span in table.sub_categories:
+                table.remove_sub_category(TableType.max_row_span)
+            if TableType.max_col_span in table.sub_categories:
+                table.remove_sub_category(TableType.max_col_span)
+
             self.dp_manager.set_summary_annotation(
                 TableType.number_of_rows, TableType.number_of_rows, number_of_rows, annotation_id=table.annotation_id
             )
             self.dp_manager.set_summary_annotation(
                 TableType.number_of_columns,
                 TableType.number_of_columns,
                 number_of_cols,
```

### Comparing `deepdoctection-0.22/deepdoctection/pipe/registry.py` & `deepdoctection-0.23/deepdoctection/pipe/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/pipe/segment.py` & `deepdoctection-0.23/deepdoctection/pipe/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,23 +563,32 @@
 
     raw_table_segments = []
 
     with MappingContextManager(dp_name=dp.file_name) as segment_mapping_context:
         for idx, cell in enumerate(spanning_cells):
             cell_positions_rows = cell_index_rows == idx
             rows_of_cell = [rows[k] for k in row_index[cell_positions_rows]]
-            rs = np.count_nonzero(cell_index_rows == idx)
+            rs = (
+                max([int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell])
+                - min([int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell])
+                + 1
+            )
             if len(rows_of_cell):
                 row_number = min([int(row.get_sub_category(CellType.row_number).category_id) for row in rows_of_cell])
             else:
                 row_number = 0
 
             cell_positions_cols = cell_index_cols == idx
             cols_of_cell = [columns[k] for k in col_index[cell_positions_cols]]
-            cs = np.count_nonzero(cell_index_cols == idx)
+            cs = (
+                max([int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell])
+                - min([int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell])
+                + 1
+            )
+
             if len(cols_of_cell):
                 col_number = min(
                     [int(col.get_sub_category(CellType.column_number).category_id) for col in cols_of_cell]
                 )
             else:
                 col_number = 0
 
@@ -723,14 +732,40 @@
                 self.dp_manager.set_category_annotation(
                     CellType.row_span, segment_result.rs, CellType.row_span, segment_result.annotation_id
                 )
                 self.dp_manager.set_category_annotation(
                     CellType.column_span, segment_result.cs, CellType.column_span, segment_result.annotation_id
                 )
 
+            if table.image:
+                cells = table.image.get_annotation(category_names=self._cell_names)
+                number_of_rows = max([int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells])
+                number_of_cols = max([int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells])
+                max_row_span = max([int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells])
+                max_col_span = max([int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells])
+                # TODO: the summaries should be sub categories of the underlying ann
+                self.dp_manager.set_summary_annotation(
+                    TableType.number_of_rows,
+                    TableType.number_of_rows,
+                    number_of_rows,
+                    annotation_id=table.annotation_id,
+                )
+                self.dp_manager.set_summary_annotation(
+                    TableType.number_of_columns,
+                    TableType.number_of_columns,
+                    number_of_cols,
+                    annotation_id=table.annotation_id,
+                )
+                self.dp_manager.set_summary_annotation(
+                    TableType.max_row_span, TableType.max_row_span, max_row_span, annotation_id=table.annotation_id
+                )
+                self.dp_manager.set_summary_annotation(
+                    TableType.max_col_span, TableType.max_col_span, max_col_span, annotation_id=table.annotation_id
+                )
+
     def clone(self) -> PipelineComponent:
         return self.__class__(
             self.segment_rule,
             self.threshold_rows,
             self.threshold_cols,
             self.tile_table,
             self.remove_iou_threshold_rows,
```

### Comparing `deepdoctection-0.22/deepdoctection/pipe/text.py` & `deepdoctection-0.23/deepdoctection/pipe/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,25 @@
     """
 
     def __init__(
         self,
         text_extract_detector: Union[ObjectDetector, PdfMiner, TextRecognizer],
         extract_from_roi: Optional[Union[Sequence[TypeOrStr], TypeOrStr]] = None,
         run_time_ocr_language_selection: bool = False,
+        skip_if_text_extracted: bool = False,
     ):
         """
         :param text_extract_detector: ObjectDetector
         :param extract_from_roi: one or more category names for roi selection
+        :param run_time_ocr_language_selection: Only available for `TesseractOcrDetector` as this framework has
+                                                multiple language selections. Also requires that a language detection
+                                                pipeline component ran before. It will select the expert language OCR
+                                                model based on the determined language.
+        :param skip_if_text_extracted: Set to `True` if text has already been extracted in a previous pipeline component
+                                       and should not be extracted again. Use-case: A PDF with some scanned images.
         """
 
         if extract_from_roi is None:
             extract_from_roi = []
         self.extract_from_category = (
             [get_type(extract_from_roi)]
             if isinstance(extract_from_roi, str)
@@ -87,62 +94,77 @@
                 raise TypeError("Predicting from a cropped image requires to pass an ObjectDetector or TextRecognizer.")
         if run_time_ocr_language_selection:
             assert isinstance(self.predictor, TesseractOcrDetector), (
                 "Only TesseractOcrDetector supports multiple " "languages"
             )
 
         self.run_time_ocr_language_selection = run_time_ocr_language_selection
+        self.skip_if_text_extracted = skip_if_text_extracted
+        if self.skip_if_text_extracted and isinstance(self.predictor, TextRecognizer):
+            raise ValueError(
+                "skip_if_text_extracted=True and TextRecognizer in TextExtractionService is not " "compatible"
+            )
 
     def serve(self, dp: Image) -> None:
         maybe_batched_text_rois = self.get_text_rois(dp)
         for text_roi in maybe_batched_text_rois:
             ann_id = None
             if isinstance(text_roi, ImageAnnotation):
                 ann_id = text_roi.annotation_id
             predictor_input = self.get_predictor_input(text_roi)
             if predictor_input is None:
                 raise ValueError("predictor_input cannot be None")
-            width, height = None, None
-            if self.run_time_ocr_language_selection:
-                self.predictor.set_language(dp.summary.get_sub_category(PageType.language).value)  # type: ignore
-            detect_result_list = self.predictor.predict(predictor_input)  # type: ignore
-            if isinstance(self.predictor, PdfMiner):
-                width, height = self.predictor.get_width_height(predictor_input)  # type: ignore
-
-            for detect_result in detect_result_list:
-                if isinstance(self.predictor, TextRecognizer):
-                    detect_ann_id = detect_result.uuid
-                else:
-                    detect_ann_id = self.dp_manager.set_image_annotation(
-                        detect_result, ann_id, True, detect_result_max_width=width, detect_result_max_height=height
-                    )
-                if detect_ann_id is not None:
-                    self.dp_manager.set_container_annotation(
-                        WordType.characters,
-                        None,
-                        WordType.characters,
-                        detect_ann_id,
-                        detect_result.text if detect_result.text is not None else "",
-                        detect_result.score,
-                    )
-                    if detect_result.block:
-                        self.dp_manager.set_category_annotation(
-                            WordType.block, detect_result.block, WordType.block, detect_ann_id
+            if predictor_input in [b""]:
+                pass
+            else:
+                width, height = None, None
+                if self.run_time_ocr_language_selection:
+                    self.predictor.set_language(dp.summary.get_sub_category(PageType.language).value)  # type: ignore
+                detect_result_list = self.predictor.predict(predictor_input)  # type: ignore
+                if isinstance(self.predictor, PdfMiner):
+                    width, height = self.predictor.get_width_height(predictor_input)  # type: ignore
+
+                for detect_result in detect_result_list:
+                    if isinstance(self.predictor, TextRecognizer):
+                        detect_ann_id = detect_result.uuid
+                    else:
+                        detect_ann_id = self.dp_manager.set_image_annotation(
+                            detect_result, ann_id, True, detect_result_max_width=width, detect_result_max_height=height
                         )
-                    if detect_result.line:
-                        self.dp_manager.set_category_annotation(
-                            WordType.text_line, detect_result.line, WordType.text_line, detect_ann_id
+                    if detect_ann_id is not None:
+                        self.dp_manager.set_container_annotation(
+                            WordType.characters,
+                            None,
+                            WordType.characters,
+                            detect_ann_id,
+                            detect_result.text if detect_result.text is not None else "",
+                            detect_result.score,
                         )
+                        if detect_result.block:
+                            self.dp_manager.set_category_annotation(
+                                WordType.block, detect_result.block, WordType.block, detect_ann_id
+                            )
+                        if detect_result.line:
+                            self.dp_manager.set_category_annotation(
+                                WordType.text_line, detect_result.line, WordType.text_line, detect_ann_id
+                            )
 
     def get_text_rois(self, dp: Image) -> Sequence[Union[Image, ImageAnnotation, List[ImageAnnotation]]]:
         """
         Return image rois based on selected categories. As this selection makes only sense for specific text extractors
         (e.g. those who do proper OCR and do not mine from text from native pdfs) it will do some sanity checks.
+        It is possible that a preceding text extractor dumped text before. If the predictor must not extract text as
+        well `get_text_rois` will return an empty list.
         :return: list of ImageAnnotation or Image
         """
+        if self.skip_if_text_extracted:
+            text_categories = self.predictor.possible_categories()  # type: ignore
+            text_anns = dp.get_annotation(category_names=text_categories)
+            if text_anns:
+                return []
 
         if self.extract_from_category:
             if self.predictor.accepts_batch:
                 return [dp.get_annotation(category_names=self.extract_from_category)]
             return dp.get_annotation(category_names=self.extract_from_category)
         return [dp]
 
@@ -167,15 +189,17 @@
             if not isinstance(text_roi, Image):
                 raise ValueError("text_roi must be an image")
             return text_roi.image
         if isinstance(text_roi, list):
             assert all(roi.image is not None for roi in text_roi)
             assert all(roi.image.image is not None for roi in text_roi)  # type: ignore
             return [(roi.annotation_id, roi.image.image) for roi in text_roi]  # type: ignore
-        return text_roi.pdf_bytes
+        if isinstance(self.predictor, PdfMiner) and text_roi.pdf_bytes is not None:
+            return text_roi.pdf_bytes
+        return b""
 
     def get_meta_annotation(self) -> JsonDict:
         if self.extract_from_category:
             sub_cat_dict = {category: {WordType.characters} for category in self.extract_from_category}
         else:
             if not isinstance(self.predictor, (ObjectDetector, PdfMiner)):
                 raise TypeError(
@@ -236,16 +260,17 @@
     reading_lines.sort(key=lambda x: (rows_dict[x[0]], x[2]))
     return [(idx + 1, word[1]) for idx, word in enumerate(reading_lines)]
 
 
 def _reading_columns(
     dp: Image,
     anns: List[ImageAnnotation],
-    starting_point_tolerance: float = 0.01,
-    height_tolerance: float = 3.0,
+    starting_point_tolerance: float,
+    height_tolerance: float,
+    ignore_category_when_building_column_blocks: List[LayoutType],
 ) -> List[Tuple[int, str]]:
     reading_blocks = []
     columns: List[Dict[str, float]] = []
     anns.sort(key=lambda x: (x.bounding_box.cy, x.bounding_box.cx))  # type: ignore
     for ann in anns:
         if ann.image is not None:
             bounding_box = ann.image.get_embedding(dp.image_id)
@@ -280,18 +305,19 @@
             fourth_condition = abs(rel_coords_box.lry - col["top"]) < height_tolerance * rel_coords_box.height
 
             if (first_condition and (third_condition or fourth_condition)) or (  # pylint: disable=R0916
                 second_condition and (third_condition or fourth_condition)
             ):
                 reading_blocks.append((idx, ann.annotation_id))
                 # update the top and right with the new line added.
-                col["left"] = min(rel_coords_box.ulx, col["left"])
-                col["top"] = min(rel_coords_box.uly, col["top"])
-                col["right"] = max(rel_coords_box.lrx, col["right"])
-                col["bottom"] = max(rel_coords_box.lry, col["bottom"])
+                if ann.category_name not in ignore_category_when_building_column_blocks:
+                    col["left"] = min(rel_coords_box.ulx, col["left"])
+                    col["top"] = min(rel_coords_box.uly, col["top"])
+                    col["right"] = max(rel_coords_box.lrx, col["right"])
+                    col["bottom"] = max(rel_coords_box.lry, col["bottom"])
                 column_found = True
                 break
 
         if not column_found:
             columns.append(
                 {
                     "left": rel_coords_box.ulx,
@@ -305,36 +331,45 @@
 
     # building connected components of columns
     connected_components: List[Dict[str, Any]] = []
     for idx, col in enumerate(columns):
         col["id"] = idx
         component_found = False
         for comp in connected_components:
-            if comp["top"] < col["top"] < comp["bottom"] or comp["top"] < col["bottom"] < comp["bottom"]:
+            if (
+                comp["top"] < col["top"] < comp["bottom"]
+                or comp["top"] < col["bottom"] < comp["bottom"]
+                or col["top"] < comp["top"] < col["bottom"]
+                or col["top"] < comp["bottom"] < col["bottom"]
+            ):
                 comp["top"] = min(comp["top"], col["top"])
                 comp["bottom"] = max(comp["bottom"], col["bottom"])
                 comp["left"] = col["left"]
                 comp["column"].append(col)
                 component_found = True
                 break
         if not component_found:
             connected_components.append(
                 {"top": col["top"], "bottom": col["bottom"], "left": col["left"], "column": [col]}
             )
 
-    # next, sorting columns in connected components by increasing x-value
+    # next, sorting columns in connected components by increasing x-value. In order to be tolerant to nearby values
+    # we are rounding values we want to sort
     for comp in connected_components:
-        comp["column"].sort(key=lambda x: x["left"])
+        for col in comp["column"]:
+            col["left"] = round(col["left"], 2)
+            col["top"] = round(col["top"], 2)
+        comp["column"].sort(key=lambda x: (x["left"], x["top"]))
 
     # finally, sorting connected components by increasing y-value
     connected_components.sort(key=lambda x: x["top"])
     columns = list(chain(*[comp["column"] for comp in connected_components]))
 
     # old to new mapping
-    columns_dict = {k: col["id"] for k, col in enumerate(columns)}
+    columns_dict = {col["id"]: k for k, col in enumerate(columns)}
     _blocks = [(columns_dict[x[0]], x[1]) for x in reading_blocks]
     _blocks.sort(key=lambda x: x[0])
     reading_blocks = [(idx + 1, block[1]) for idx, block in enumerate(_blocks)]
     return reading_blocks
 
 
 @pipeline_component_registry.register("TextOrderService")
@@ -402,14 +437,17 @@
         elif text_block_names is None:
             text_block_names = []
 
         self._text_container = text_container
         self._floating_text_block_names = floating_text_block_names
         self._text_block_names = text_block_names
         self._text_containers_to_text_block = text_containers_to_text_block
+        self.starting_point_tolerance = 0.05
+        self.height_tolerance = 2.0
+        self.ignore_category_when_building_column_blocks = [LayoutType.table]
         self._init_sanity_checks()
         super().__init__("text_order")
 
     def serve(self, dp: Image) -> None:
         # select all text blocks that are considered to be relevant for page text. This does not include some layout
         # items that have to be considered independently (e.g. tables). Order the blocks by column wise reading order
         floating_text_block_anns = dp.get_annotation(category_names=self._floating_text_block_names)
@@ -424,15 +462,21 @@
             text_container_anns = [ann for ann in text_container_anns if ann.annotation_id not in text_ann_ids]
             floating_text_block_anns.extend(text_container_anns)
 
         # estimating reading columns. We will only do this if we have some text blocks that are no text_containers
         # (number_text_block_anns_orig >0) or if the text container is not a word. Otherwise, we will have to skip that
         # part
         if self._text_container != LayoutType.word or number_floating_text_block_anns_orig:
-            raw_reading_order_list = _reading_columns(dp, floating_text_block_anns, 0.05, 2.0)
+            raw_reading_order_list = _reading_columns(
+                dp,
+                floating_text_block_anns,
+                self.starting_point_tolerance,
+                self.height_tolerance,
+                self.ignore_category_when_building_column_blocks,
+            )
 
             for raw_reading_order in raw_reading_order_list:
                 self.dp_manager.set_category_annotation(
                     Relationships.reading_order, raw_reading_order[0], Relationships.reading_order, raw_reading_order[1]
                 )
 
         # next we select all blocks that might contain text. We sort all text within these blocks
```

### Comparing `deepdoctection-0.22/deepdoctection/pipe/transform.py` & `deepdoctection-0.23/deepdoctection/pipe/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/train/__init__.py` & `deepdoctection-0.23/deepdoctection/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/train/d2_frcnn_train.py` & `deepdoctection-0.23/deepdoctection/train/d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/train/hf_detr_train.py` & `deepdoctection-0.23/deepdoctection/train/hf_detr_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/train/hf_layoutlm_train.py` & `deepdoctection-0.23/deepdoctection/train/hf_layoutlm_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/train/tp_frcnn_train.py` & `deepdoctection-0.23/deepdoctection/train/tp_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/__init__.py` & `deepdoctection-0.23/deepdoctection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/concurrency.py` & `deepdoctection-0.23/deepdoctection/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/context.py` & `deepdoctection-0.23/deepdoctection/utils/context.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/detection_types.py` & `deepdoctection-0.23/deepdoctection/utils/detection_types.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/develop.py` & `deepdoctection-0.23/deepdoctection/utils/develop.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/file_utils.py` & `deepdoctection-0.23/deepdoctection/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/fs.py` & `deepdoctection-0.23/deepdoctection/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/identifier.py` & `deepdoctection-0.23/deepdoctection/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/logger.py` & `deepdoctection-0.23/deepdoctection/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/metacfg.py` & `deepdoctection-0.23/deepdoctection/utils/metacfg.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/pdf_utils.py` & `deepdoctection-0.23/deepdoctection/utils/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/settings.py` & `deepdoctection-0.23/deepdoctection/utils/settings.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/systools.py` & `deepdoctection-0.23/deepdoctection/utils/systools.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/tqdm.py` & `deepdoctection-0.23/deepdoctection/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/transform.py` & `deepdoctection-0.23/deepdoctection/utils/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/utils.py` & `deepdoctection-0.23/deepdoctection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection/utils/viz.py` & `deepdoctection-0.23/deepdoctection/utils/viz.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/deepdoctection.egg-info/PKG-INFO` & `deepdoctection-0.23/deepdoctection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.22
+Version: 0.23
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -49,19 +49,20 @@
 
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
- - Deskewing and rotating images with jdeskew. 
+ - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
  - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
    provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!) 
- - [**new!**] Table detection and table structure recognition with 
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). Check the notebook repo or 
+   the documentation on how to train a model on your custom task or how to setup a pipeline.
+ - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
@@ -140,22 +141,22 @@
 as possible. However, we are aware that there are still many areas where significant improvements can be made in terms 
 of clarity, grammar and correctness. We look forward to every hint and comment that increases the quality of the 
 documentation.
 
 
 ## Requirements
 
-![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.jpg)
+![requirements](./docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
 - Python >= 3.8
-- PyTorch >= 1.8 **or** Tensorflow >= 2.8 and CUDA. If you want to run the models provided by Tensorpack a GPU is
+- PyTorch >= 1.8 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
   required. You can run on PyTorch with a CPU only.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
```

### Comparing `deepdoctection-0.22/deepdoctection.egg-info/SOURCES.txt` & `deepdoctection-0.23/deepdoctection.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 deepdoctection/__init__.py
+deepdoctection/py.typed
 deepdoctection.egg-info/PKG-INFO
 deepdoctection.egg-info/SOURCES.txt
 deepdoctection.egg-info/dependency_links.txt
 deepdoctection.egg-info/requires.txt
 deepdoctection.egg-info/top_level.txt
 deepdoctection/analyzer/__init__.py
 deepdoctection/analyzer/dd.py
-deepdoctection/analyzer/tools.py
 deepdoctection/configs/__init__.py
 deepdoctection/configs/conf_dd_one.yaml
 deepdoctection/configs/conf_tesseract.yaml
 deepdoctection/dataflow/__init__.py
 deepdoctection/dataflow/base.py
 deepdoctection/dataflow/common.py
 deepdoctection/dataflow/custom.py
```

### Comparing `deepdoctection-0.22/deepdoctection.egg-info/requires.txt` & `deepdoctection-0.23/deepdoctection.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 numpy<1.24,>=1.21
 opencv-python==4.5.4.60
 packaging<22.0,>=20.0
 pycocotools>=2.0.2
 pypdf2<2.10.1,>=1.27.5
 pyyaml==6.0
 pyzmq>=16
+rapidfuzz<3.0,>=1.6.0
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
 types-PyYAML
 types-termcolor==1.1.3
 types-tabulate
 types-tqdm
@@ -30,15 +31,15 @@
 pylint==2.13.4
 mypy==0.942
 wandb
 
 [docs]
 tensorpack
 boto3
-transformers<=4.24
+transformers
 pdfplumber>=0.7.1
 lxml>=4.9.1
 lxml-stubs
 pycocotools>=2.0.2
 jdeskew
 jinja2==3.0.3
 mkdocs-material
@@ -58,25 +59,26 @@
 numpy<1.24,>=1.21
 opencv-python==4.5.4.60
 packaging<22.0,>=20.0
 pycocotools>=2.0.2
 pypdf2<2.10.1,>=1.27.5
 pyyaml==6.0
 pyzmq>=16
+rapidfuzz<3.0,>=1.6.0
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
 types-PyYAML
 types-termcolor==1.1.3
 types-tabulate
 types-tqdm
 lxml-stubs
 timm
-transformers<=4.24
-python-doctr<=0.5.1
+transformers
+python-doctr==0.6.0
 boto3
 pdfplumber>=0.7.1
 fasttext
 jdeskew
 
 [pt]
 apted==1.0.3
@@ -91,25 +93,26 @@
 numpy<1.24,>=1.21
 opencv-python==4.5.4.60
 packaging<22.0,>=20.0
 pycocotools>=2.0.2
 pypdf2<2.10.1,>=1.27.5
 pyyaml==6.0
 pyzmq>=16
+rapidfuzz<3.0,>=1.6.0
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
 types-PyYAML
 types-termcolor==1.1.3
 types-tabulate
 types-tqdm
 lxml-stubs
 timm
-transformers<=4.24
-python-doctr<=0.5.1
+transformers
+python-doctr==0.6.0
 boto3
 pdfplumber>=0.7.1
 fasttext
 jdeskew
 
 [test]
 pytest
@@ -128,23 +131,25 @@
 numpy<1.24,>=1.21
 opencv-python==4.5.4.60
 packaging<22.0,>=20.0
 pycocotools>=2.0.2
 pypdf2<2.10.1,>=1.27.5
 pyyaml==6.0
 pyzmq>=16
+rapidfuzz<3.0,>=1.6.0
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
 types-PyYAML
 types-termcolor==1.1.3
 types-tabulate
 types-tqdm
 lxml-stubs
 tensorpack
 protobuf==3.20.1
-tensorflow-addons>=0.13.0
-python-doctr<=0.5.1
+tensorflow-addons>=0.17.1
+tf2onnx>=1.9.2
+python-doctr==0.6.0
 boto3
 pdfplumber>=0.7.1
 fasttext
 jdeskew
```

### Comparing `deepdoctection-0.22/setup.cfg` & `deepdoctection-0.23/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/setup.py` & `deepdoctection-0.23/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,36 +54,38 @@
     "opencv-python==4.5.4.60",
     "packaging>=20.0,<22.0",
     "pycocotools>=2.0.2",
     "pypdf2>=1.27.5,<2.10.1",
     "python-prctl",
     "pyyaml==6.0",
     "pyzmq>=16",
+    "rapidfuzz>=1.6.0,<3.0",  # we need this requirement for Doctr as long they have not fixed #1186 for v.0.6.0
     "termcolor>=1.1",
     "tabulate>=0.7.7",
     "tqdm==4.64.0",
     # type-stubs
     "types-PyYAML",
     "types-termcolor==1.1.3",
     "types-tabulate",
     "types-tqdm",
     "lxml-stubs",
     # Tensorflow related dependencies
     "protobuf==3.20.1",
     "tensorpack",
     # PyTorch related dependencies
     "timm",
-    "transformers<=4.24",
+    "transformers",
     "detectron2 @ git+https://github.com/facebookresearch/detectron2.git",
     # other third party related dependencies (services or DL libraries). Must be installed by users
     "jdeskew",
     "boto3",
     "pdfplumber>=0.7.1",
-    "tensorflow-addons>=0.13.0",
-    "python-doctr<=0.5.1",
+    "tensorflow-addons>=0.17.1",
+    "tf2onnx>=1.9.2",
+    "python-doctr==0.6.0",
     "fasttext",
     # dev dependencies
     "click==8.0.4",  # version will not break black
     "black==22.3.0",
     "isort",
     "pylint==2.13.4",
     "mypy==0.942",
@@ -122,14 +124,15 @@
     "numpy",
     "opencv-python",
     "packaging",
     "pycocotools",
     "pypdf2",
     "pyyaml",
     "pyzmq",
+    "rapidfuzz",
     "termcolor",
     "tabulate",
     "tqdm",
     "types-PyYAML",
     "types-termcolor",
     "types-tabulate",
     "types-tqdm",
@@ -137,15 +140,15 @@
 )
 
 
 # remaining dependencies to use models that neither require TF nor PyTorch
 additional_deps = deps_list("boto3", "pdfplumber", "fasttext", "jdeskew")
 
 # Tensorflow dependencies
-tf_deps = deps_list("tensorpack", "protobuf", "tensorflow-addons", "python-doctr")
+tf_deps = deps_list("tensorpack", "protobuf", "tensorflow-addons", "tf2onnx", "python-doctr")
 
 # PyTorch dependencies
 pt_deps = deps_list("timm", "transformers", "python-doctr")
 source_pt_deps = pt_deps + deps_list("detectron2 @ git+https://github.com/facebookresearch/detectron2.git")
 
 # Putting all together
 tf_deps = dist_deps + tf_deps + additional_deps
@@ -182,15 +185,15 @@
 # TODO: add function that lists correct not pre-installed third party libs in package, such that requirement errors
 #  can be printed with correct version dependencies.
 # when uploading to pypi first comment all source extra dependencies so that there are no dependencies to dataflow
 
 EXTRA_DEPS = {
     "tf": tf_deps,
     "pt": pt_deps,
-#    "source-pt": source_pt_deps,
+    #"source-pt": source_pt_deps,
     "docs": docs_deps,
     "dev": dev_deps,
     "test": test_deps,
     "hf": pt_deps,
 }
 
 setup(
```

### Comparing `deepdoctection-0.22/tests/__init__.py` & `deepdoctection-0.23/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/analyzer/__init__.py` & `deepdoctection-0.23/tests/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/analyzer/test_dd.py` & `deepdoctection-0.23/tests/analyzer/test_dd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/conftest.py` & `deepdoctection-0.23/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/data.py` & `deepdoctection-0.23/tests/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/dataflow/__init__.py` & `deepdoctection-0.23/tests/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/dataflow/conftest.py` & `deepdoctection-0.23/tests/dataflow/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/dataflow/test_common.py` & `deepdoctection-0.23/tests/dataflow/test_common.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from typing import List, no_type_check
 
 import numpy as np
 from numpy.testing import assert_array_equal
 from pytest import mark
 
 from deepdoctection.dataflow import (
+    BatchData,
     ConcatData,
     CustomDataFromList,
     DataFlow,
     DataFromList,
     FakeData,
     FlattenData,
     JoinData,
@@ -165,7 +166,54 @@
     df: DataFlow
     df = JoinData([df_1, df_2])
     output = collect_datapoint_from_dataflow(df=df)
 
     # Assert
     assert len(output) == 2
     assert "foo" in output[0] and "bak" in output[0] and "baz" in output[0] and "bal" in output[0]
+
+
+@mark.basic
+def test_batch_data() -> None:
+    """Test BatchData"""
+
+    # Arrange
+    dataflow_list = [
+        {"foo": "1", "bak": "a"},
+        {"foo": "3", "bak": "c"},
+        {"baz": "2", "bal": "a"},
+        {"baz": "4", "bal": "c"},
+    ]
+    df: DataFlow
+    df = DataFromList(dataflow_list, shuffle=False)
+
+    # Act
+    df = BatchData(df, 3)
+    output = collect_datapoint_from_dataflow(df=df)
+
+    # Assert
+    assert len(output) == 1
+    assert len(output[0]) == 3
+
+
+@mark.basic
+def test_batch_data_with_remainder() -> None:
+    """Test BatchData with remainder"""
+
+    # Arrange
+    dataflow_list = [
+        {"foo": "1", "bak": "a"},
+        {"foo": "3", "bak": "c"},
+        {"baz": "2", "bal": "a"},
+        {"baz": "4", "bal": "c"},
+    ]
+    df: DataFlow
+    df = DataFromList(dataflow_list, shuffle=False)
+
+    # Act
+    df = BatchData(df, 3, remainder=True)
+    output = collect_datapoint_from_dataflow(df=df)
+
+    # Assert
+    assert len(output) == 2
+    assert len(output[0]) == 3
+    assert len(output[1]) == 1
```

### Comparing `deepdoctection-0.22/tests/dataflow/test_custom.py` & `deepdoctection-0.23/tests/dataflow/test_custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/dataflow/test_custom_serialize.py` & `deepdoctection-0.23/tests/dataflow/test_custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/dataflow/test_parallel_map.py` & `deepdoctection-0.23/tests/dataflow/test_parallel_map.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/dataflow/test_stats.py` & `deepdoctection-0.23/tests/dataflow/test_stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datapoint/__init__.py` & `deepdoctection-0.23/tests/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datapoint/conftest.py` & `deepdoctection-0.23/tests/datapoint/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datapoint/test_annotation.py` & `deepdoctection-0.23/tests/datapoint/test_annotation.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datapoint/test_box.py` & `deepdoctection-0.23/tests/datapoint/test_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datapoint/test_convert.py` & `deepdoctection-0.23/tests/datapoint/test_convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datapoint/test_image.py` & `deepdoctection-0.23/tests/datapoint/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,14 +293,24 @@
         df = SerializerJsonlines.load(get_test_path() / "test_image.jsonl")
         df = MapData(df, lambda dp: Image.from_dict(**dp))
         image_list = collect_datapoint_from_dataflow(df)
         assert len(image_list) == 1
 
     @staticmethod
     @mark.basic
+    def test_load_image_from_file() -> None:
+        """
+        test class from_file returns an image
+        """
+        test_file_path = get_test_path() / "test_image.json"
+        image = Image.from_file(test_file_path.as_posix())
+        assert isinstance(image, Image)
+
+    @staticmethod
+    @mark.basic
     def test_state_id_changes_when_annotations_added(image: WhiteImage) -> None:
         """
         state_id changes when annotations are added
         """
 
         # Arrange
         test_image = Image(location=image.loc, file_name=image.file_name)
```

### Comparing `deepdoctection-0.22/tests/datapoint/test_view.py` & `deepdoctection-0.23/tests/datapoint/test_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from deepdoctection.datapoint.annotation import CategoryAnnotation, ImageAnnotation
 from deepdoctection.datapoint.box import BoundingBox
 from deepdoctection.datapoint.image import Image
 from deepdoctection.datapoint.view import Page
 from deepdoctection.utils.settings import LayoutType, Relationships
 
+from ..test_utils import get_test_path
 from .conftest import WhiteImage
 
 
 @mark.basic
 def test_page_from_image(dp_image_with_layout_and_word_annotations: Image) -> None:
     """
     test page gets converted from an image correctly
@@ -91,7 +92,17 @@
     # Act
     page = Page.from_image(test_image, LayoutType.table, [LayoutType.table])
 
     try:
         page.save(dry=True)
     except Exception as exception:  # pylint: disable=W0703
         assert False, f"{exception}"
+
+
+@mark.basic
+def test_load_page_from_file() -> None:
+    """
+    test class from_file returns a page
+    """
+    test_file_path = get_test_path() / "test_image.json"
+    image = Page.from_file(test_file_path.as_posix())
+    assert isinstance(image, Page)
```

### Comparing `deepdoctection-0.22/tests/datasets/__init__.py` & `deepdoctection-0.23/tests/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/__init__.py` & `deepdoctection-0.23/tests/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/conftest.py` & `deepdoctection-0.23/tests/datasets/instances/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_doclaynet.py` & `deepdoctection-0.23/tests/datasets/instances/test_doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_fintabnet.py` & `deepdoctection-0.23/tests/datasets/instances/test_fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_funsd.py` & `deepdoctection-0.23/tests/datasets/instances/test_funsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     funsd.dataflow.get_workdir = get_test_path  # type: ignore
     funsd.dataflow.splits = {"test": ""}
     funsd.dataflow.annotation_files = {"test": ""}
     df = funsd.dataflow.build()
 
     # Act
     df_list = collect_datapoint_from_dataflow(df)
-    assert len(df_list) == 3  # the first three images coming from files not related to funsd data
+    assert len(df_list) == 4  # the first three images coming from files not related to funsd data
     dp = df_list[2]
     word = dp.get_annotation(category_names=LayoutType.word)[0]
     assert word.get_sub_category(WordType.token_class) is not None
     assert word.get_sub_category(WordType.characters) is not None
     assert word.get_sub_category(WordType.tag) is not None
     assert word.get_sub_category(WordType.token_tag) is not None
```

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_iiitar13k.py` & `deepdoctection-0.23/tests/datasets/instances/test_iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_layouttest.py` & `deepdoctection-0.23/tests/datasets/instances/test_layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_publaynet.py` & `deepdoctection-0.23/tests/datasets/instances/test_publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_pubtables1m.py` & `deepdoctection-0.23/tests/datasets/instances/test_pubtables1m.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_pubtabnet.py` & `deepdoctection-0.23/tests/datasets/instances/test_pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/instances/test_rvlcdip.py` & `deepdoctection-0.23/tests/datasets/instances/test_rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/test_adapter.py` & `deepdoctection-0.23/tests/datasets/test_adapter.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/test_info.py` & `deepdoctection-0.23/tests/datasets/test_info.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/datasets/test_registry.py` & `deepdoctection-0.23/tests/datasets/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/eval/__init__.py` & `deepdoctection-0.23/tests/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/eval/conftest.py` & `deepdoctection-0.23/tests/eval/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/eval/test_accmetric.py` & `deepdoctection-0.23/tests/eval/test_accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/eval/test_cocometric.py` & `deepdoctection-0.23/tests/eval/test_cocometric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/eval/test_eval.py` & `deepdoctection-0.23/tests/eval/test_eval.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/eval/test_registry.py` & `deepdoctection-0.23/tests/eval/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/eval/test_tedsmetric.py` & `deepdoctection-0.23/tests/eval/test_tedsmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/conftest.py` & `deepdoctection-0.23/tests/extern/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/data.py` & `deepdoctection-0.23/tests/extern/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/test_deskew.py` & `deepdoctection-0.23/tests/extern/test_deskew.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/test_fastlang.py` & `deepdoctection-0.23/tests/extern/test_fastlang.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/test_hfdetr.py` & `deepdoctection-0.23/tests/extern/test_hfdetr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/test_hflayoutlm.py` & `deepdoctection-0.23/tests/extern/test_hflayoutlm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/test_pdftext.py` & `deepdoctection-0.23/tests/extern/test_pdftext.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/test_tessocr.py` & `deepdoctection-0.23/tests/extern/test_tessocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/test_texocr.py` & `deepdoctection-0.23/tests/extern/test_texocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/extern/test_tpdetect.py` & `deepdoctection-0.23/tests/extern/test_tpdetect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/__init__.py` & `deepdoctection-0.23/tests/pipe/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: __init__.py
+# File: xxx.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `deepdoctection-0.22/tests/mapper/conftest.py` & `deepdoctection-0.23/tests/mapper/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/data.py` & `deepdoctection-0.23/tests/mapper/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_cats.py` & `deepdoctection-0.23/tests/mapper/test_cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_cocostruct.py` & `deepdoctection-0.23/tests/mapper/test_cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_d2struct.py` & `deepdoctection-0.23/tests/mapper/test_d2struct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_hfstruct.py` & `deepdoctection-0.23/tests/mapper/test_hfstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_iiitar13k.py` & `deepdoctection-0.23/tests/mapper/test_iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_laylmstruct.py` & `deepdoctection-0.23/tests/mapper/test_laylmstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_misc.py` & `deepdoctection-0.23/tests/mapper/test_misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_prodigystruct.py` & `deepdoctection-0.23/tests/mapper/test_prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_pubstruct.py` & `deepdoctection-0.23/tests/mapper/test_pubstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_tpstruct.py` & `deepdoctection-0.23/tests/mapper/test_tpstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_utils.py` & `deepdoctection-0.23/tests/mapper/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/mapper/test_xfundstruct.py` & `deepdoctection-0.23/tests/mapper/test_xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/__init__.py` & `deepdoctection-0.23/tests/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_anngen.py` & `deepdoctection-0.23/tests/pipe/test_anngen.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_cell.py` & `deepdoctection-0.23/tests/pipe/test_cell.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_common.py` & `deepdoctection-0.23/tests/pipe/test_common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_language.py` & `deepdoctection-0.23/tests/pipe/test_language.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_layout.py` & `deepdoctection-0.23/tests/pipe/test_layout.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_lm.py` & `deepdoctection-0.23/tests/pipe/test_lm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_refine.py` & `deepdoctection-0.23/tests/pipe/test_refine.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_registry.py` & `deepdoctection-0.23/tests/pipe/test_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 @mark.basic
 def test_pipe_registry_has_all_build_in_pipe_component_registered() -> None:
     """
     test pipe registry has all pipeline components registered
     """
-    assert len(pipeline_component_registry.get_all()) == 14
+    assert len(pipeline_component_registry.get_all()) == 15
 
 
 @mark.basic
 def test_pipe_registry_registered_new_pipeline_component() -> None:
     """
     test, that the new generated pipe component "TestPipeComponent" can be registered and retrieved from registry
     """
```

### Comparing `deepdoctection-0.22/tests/pipe/test_segment.py` & `deepdoctection-0.23/tests/pipe/test_segment.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_text.py` & `deepdoctection-0.23/tests/pipe/test_text.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/pipe/test_transform.py` & `deepdoctection-0.23/tests/pipe/test_transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/test_utils.py` & `deepdoctection-0.23/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/train/__init__.py` & `deepdoctection-0.23/tests_d2/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # -*- coding: utf-8 -*-
-# File: xxx.py
+# File: __init__.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+"""
+Cannot place these tests under the general test folder as this will result in a python segmentation error
+"""
```

### Comparing `deepdoctection-0.22/tests/train/conftest.py` & `deepdoctection-0.23/tests/train/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/train/test_d2_frcnn_train.py` & `deepdoctection-0.23/tests/train/test_d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests/train/test_tp_frcnn_train.py` & `deepdoctection-0.23/tests/train/test_tp_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests_d2/__init__.py` & `deepdoctection-0.23/deepdoctection/analyzer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,9 +12,11 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Cannot place these tests under the general test folder as this will result in a python segmentation error
+Package for pre-built pipelines
 """
+
+from .dd import *
```

### Comparing `deepdoctection-0.22/tests_d2/conftest.py` & `deepdoctection-0.23/tests_d2/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.22/tests_d2/test_d2detect.py` & `deepdoctection-0.23/tests_d2/test_d2detect.py`

 * *Files identical despite different names*

