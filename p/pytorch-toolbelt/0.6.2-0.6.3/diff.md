# Comparing `tmp/pytorch_toolbelt-0.6.2.tar.gz` & `tmp/pytorch_toolbelt-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_toolbelt-0.6.2.tar", last modified: Sun Dec 25 21:40:13 2022, max compression
+gzip compressed data, was "pytorch_toolbelt-0.6.3.tar", last modified: Sun May  7 18:50:31 2023, max compression
```

## Comparing `pytorch_toolbelt-0.6.2.tar` & `pytorch_toolbelt-0.6.3.tar`

### file list

```diff
@@ -1,131 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.013047 pytorch_toolbelt-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2022-12-25 21:40:13.013047 pytorch_toolbelt-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      516 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.001047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.005047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/mean_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.005047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/providers/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/providers/inria_aerial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.005047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/ensembling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/tiles_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/tta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.005047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/balanced_bce.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/bitempered_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/focal_cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10710 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/joint_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/logcosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/lovasz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/soft_bce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/soft_ce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/soft_f1.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/wing_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.005047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.009047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/inceptionv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16506 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/wider_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/coord_conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.009047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/can.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/deeplab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/fpn_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/fpn_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/pyramid_pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/unet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/upernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/dropblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/dsconv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.009047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/hourglass.py
--rw-r--r--   0 runner    (1001) docker     (123)    16816 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/inception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/seresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    30193 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/swin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.013047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/dpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/efficient_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/efficient_net_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/nf_regnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/nfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/res2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/wide_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/xresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/hypercolumn.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15232 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/ocnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/scse.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/srm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.013047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/optimization/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/optimization/lr_schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.013047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/bboxes_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31870 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/namesgenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/rle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/support.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.013047 pytorch_toolbelt-0.6.2/pytorch_toolbelt/zoo/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/zoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/zoo/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt/zoo/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 21:40:13.001047 pytorch_toolbelt-0.6.2/pytorch_toolbelt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2022-12-25 21:40:12.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2022-12-25 21:40:12.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-25 21:40:12.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-25 21:40:12.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-25 21:40:12.000000 pytorch_toolbelt-0.6.2/pytorch_toolbelt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-25 21:40:13.013047 pytorch_toolbelt-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2022-12-25 21:40:04.000000 pytorch_toolbelt-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.108430 pytorch_toolbelt-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-05-07 18:50:31.108430 pytorch_toolbelt-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.084430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.088430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/mean_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.088430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/providers/inria_aerial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.092430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/ensembling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/tiles_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/tta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.096430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/balanced_bce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/bitempered_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/focal_cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10710 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/logcosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/lovasz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/soft_bce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/soft_ce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/soft_f1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/wing_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.100430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.100430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/inceptionv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/wider_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/coord_conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.104430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/can.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/deeplab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/fpn_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/fpn_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/pyramid_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/unet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/upernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/dropblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/dsconv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.104430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/hourglass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16816 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/inception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/seresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/squeezenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30193 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/swin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.104430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/dpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/efficient_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/efficient_net_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/nf_regnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/nfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/res2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/wide_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/xresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/hypercolumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/ocnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/scse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/srm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.104430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/optimization/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/optimization/lr_schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.104430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/bboxes_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31870 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/namesgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/rle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.108430 pytorch_toolbelt-0.6.3/pytorch_toolbelt/zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/zoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/zoo/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt/zoo/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:50:31.088430 pytorch_toolbelt-0.6.3/pytorch_toolbelt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-05-07 18:50:30.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-07 18:50:31.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:50:30.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-07 18:50:30.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 18:50:30.000000 pytorch_toolbelt-0.6.3/pytorch_toolbelt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-07 18:50:31.108430 pytorch_toolbelt-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-07 18:50:19.000000 pytorch_toolbelt-0.6.3/setup.py
```

### Comparing `pytorch_toolbelt-0.6.2/LICENSE` & `pytorch_toolbelt-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/PKG-INFO` & `pytorch_toolbelt-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch_toolbelt
-Version: 0.6.2
+Version: 0.6.3
 Summary: PyTorch extensions for fast R&D prototyping and Kaggle farming
 Home-page: https://github.com/BloodAxe/pytorch-toolbelt
 Author: Eugene Khvedchenya
 Author-email: ekhvedchenya@gmail.com
 License: License :: OSI Approved :: MIT License
 Description: 
         # Important Update
```

### Comparing `pytorch_toolbelt-0.6.2/README.md` & `pytorch_toolbelt-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pyproject.toml` & `pytorch_toolbelt-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/classification.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/classification.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/common.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 import cv2
 
 __all__ = [
     "INPUT_IMAGE_ID_KEY",
     "INPUT_IMAGE_KEY",
     "INPUT_INDEX_KEY",
     "OUTPUT_EMBEDDINGS_KEY",
@@ -24,15 +26,17 @@
     "TARGET_MASK_KEY_STRIDE_8",
     "TARGET_MASK_WEIGHT_KEY",
     "name_for_stride",
     "read_image_rgb",
 ]
 
 
-def name_for_stride(name, stride: int):
+def name_for_stride(name, stride: Union[int, None]) -> str:
+    if stride is None:
+        return name
     return f"{name}_STRIDE_{stride}"
 
 
 INPUT_INDEX_KEY = "INPUT_INDEX_KEY"
 INPUT_IMAGE_KEY = "INPUT_IMAGE_KEY"
 INPUT_IMAGE_ID_KEY = "INPUT_IMAGE_ID_KEY"
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/mean_std.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/mean_std.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/providers/inria_aerial.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/providers/inria_aerial.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/segmentation.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/segmentation.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/datasets/wrappers.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/datasets/wrappers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 import random
-from typing import Any
+from typing import Any, Optional
 
 from torch.utils.data import Dataset
 import numpy as np
 
 __all__ = ["RandomSubsetDataset", "RandomSubsetWithMaskDataset"]
 
 from torch.utils.data.dataloader import default_collate
 
 
 class RandomSubsetDataset(Dataset):
     """
     Wrapper to get desired number of samples from underlying dataset
     """
 
-    def __init__(self, dataset, num_samples: int):
+    def __init__(self, dataset, num_samples: int, weights: Optional[np.ndarray] = None):
+        if weights is not None:
+            if len(dataset) != len(weights):
+                raise ValueError(
+                    "Length of weights must be equal to length of dataset. Got {} and {}".format(
+                        len(weights), len(dataset)
+                    )
+                )
         self.dataset = dataset
         self.num_samples = num_samples
+        self.weights = np.cumsum(weights) if weights is not None else None
 
     def __len__(self) -> int:
         return self.num_samples
 
     def __getitem__(self, _) -> Any:
-        index = random.randrange(len(self.dataset))
+        if self.weights is not None:
+            population = range(len(self.dataset))
+            index = random.choices(population, cum_weights=self.weights, k=1)[0]
+        else:
+            index = random.randrange(len(self.dataset))
         return self.dataset[index]
 
     def get_collate_fn(self):
         get_collate_fn = getattr(self.dataset, "get_collate_fn", None)
         if callable(get_collate_fn):
             return get_collate_fn()
-        return default_collate()
+        return default_collate
 
 
 class RandomSubsetWithMaskDataset(Dataset):
     """
     Wrapper to get desired number of samples from underlying dataset only considering
     samples P for which mask[P] equals True
     """
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/ensembling.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/ensembling.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/functional.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/tiles.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/tiles.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/tiles_3d.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/tiles_3d.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/inference/tta.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/inference/tta.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/balanced_bce.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/balanced_bce.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/bitempered_loss.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/bitempered_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/dice.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/dice.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/focal_cosine.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/focal_cosine.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/functional.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/jaccard.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/jaccard.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/lovasz.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/lovasz.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/soft_bce.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/soft_bce.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/soft_ce.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/soft_ce.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/losses/soft_f1.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/losses/soft_f1.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/activations.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/activations.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/inceptionv4.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/mobilenet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/mobilenet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/senet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/senet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/backbone/wider_resnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/backbone/wider_resnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/coord_conv.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/coord_conv.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/bifpn.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/fpn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,191 @@
-from typing import List, Tuple
+from __future__ import absolute_import
+
+from typing import List
 
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch import Tensor
-from .common import DecoderModule
-from ..activations import get_activation_block, ACT_RELU
+from torch import nn, Tensor
+from torch.nn import functional as F
 
-__all__ = ["BiFPNDecoder", "BiFPNBlock", "BiFPNConvBlock", "BiFPNDepthwiseConvBlock"]
+from ..modules.activations import ABN
 
+__all__ = ["FPNContextBlock", "FPNBottleneckBlock", "FPNFuse", "FPNFuseSum", "HFF"]
 
-class BiFPNDepthwiseConvBlock(nn.Module):
-    """
-    Depthwise seperable convolution.
 
+class FPNContextBlock(nn.Module):
+    def __init__(self, in_channels: int, out_channels: int, abn_block=ABN, dropout=0.0):
+        """
+        Center FPN block that aggregates multi-scale context using strided average poolings
 
-    """
+        :param in_channels: Number of input features
+        :param out_channels: Number of output features
+        :param abn_block: Block for Activation + BatchNorm2d
+        :param dropout: Dropout rate after context fusion
+        """
+        super().__init__()
+        self.bottleneck = nn.Conv2d(in_channels, in_channels // 2, kernel_size=1)
 
-    def __init__(self, in_channels, out_channels, kernel_size=1, stride=1, padding=0, dilation=1, act=nn.ReLU):
-        super(BiFPNDepthwiseConvBlock, self).__init__()
-        self.depthwise = nn.Conv2d(
-            in_channels, in_channels, kernel_size, stride, padding, dilation, groups=in_channels, bias=False
-        )
-        self.pointwise = nn.Conv2d(
-            in_channels, out_channels, kernel_size=1, stride=1, padding=0, dilation=1, groups=1, bias=False
-        )
+        self.pool2 = nn.AvgPool2d(kernel_size=2, stride=2)
+        self.proj2 = nn.Conv2d(in_channels // 2, in_channels // 8, kernel_size=1)
 
-        self.bn = nn.BatchNorm2d(out_channels, momentum=0.9997, eps=4e-5)
-        self.act = act(inplace=True)
+        self.pool4 = nn.AvgPool2d(kernel_size=4, stride=4)
+        self.proj4 = nn.Conv2d(in_channels // 2, in_channels // 8, kernel_size=1)
 
-    def forward(self, x: Tensor) -> Tensor:
-        x = self.depthwise(x)
-        x = self.pointwise(x)
-        x = self.bn(x)
-        return self.act(x)
+        self.pool8 = nn.AvgPool2d(kernel_size=8, stride=8)
+        self.proj8 = nn.Conv2d(in_channels // 2, in_channels // 8, kernel_size=1)
 
+        self.pool_global = nn.AdaptiveAvgPool2d(1)
+        self.proj_global = nn.Conv2d(in_channels // 2, in_channels // 8, kernel_size=1)
 
-class BiFPNConvBlock(nn.Module):
-    """
-    Convolution block with Batch Normalization and ReLU activation.
+        self.blend = nn.Conv2d(4 * in_channels // 8, out_channels, kernel_size=1)
 
-    """
+        self.conv1 = nn.Conv2d(out_channels, out_channels, kernel_size=3, padding=1, bias=False)
+        self.abn1 = abn_block(out_channels)
 
-    def __init__(self, in_channels, out_channels, kernel_size=1, stride=1, padding=0, act=nn.ReLU, dilation=1):
-        super(BiFPNConvBlock, self).__init__()
-        self.conv = nn.Conv2d(in_channels, out_channels, kernel_size, stride=stride, padding=padding, bias=False)
-        self.bn = nn.BatchNorm2d(out_channels, momentum=0.9997, eps=4e-5)
-        self.act = act(inplace=True)
-
-    def forward(self, x: Tensor) -> Tensor:
-        x = self.conv(x)
-        x = self.bn(x)
-        return self.act(x)
+        self.dropout = nn.Dropout2d(dropout, inplace=True)
 
+        self.conv2 = nn.Conv2d(out_channels, out_channels, kernel_size=3, padding=1, bias=False)
+        self.abn2 = abn_block(out_channels)
 
-class BiFPNBlock(nn.Module):
-    """
-    Bi-directional Feature Pyramid Network
-    """
+    def forward(self, x: Tensor) -> Tensor:  # skipcq: PYL-W0221
+        x = self.bottleneck(x)
 
-    def __init__(self, feature_size: int = 64, epsilon: float = 0.0001, act=nn.ReLU):
-        super(BiFPNBlock, self).__init__()
-        self.epsilon = epsilon
-
-        self.p3_td = BiFPNDepthwiseConvBlock(feature_size, feature_size, act=act)
-        self.p4_td = BiFPNDepthwiseConvBlock(feature_size, feature_size, act=act)
-        self.p5_td = BiFPNDepthwiseConvBlock(feature_size, feature_size, act=act)
-        self.p6_td = BiFPNDepthwiseConvBlock(feature_size, feature_size, act=act)
-
-        self.p4_out = BiFPNDepthwiseConvBlock(feature_size, feature_size, act=act)
-        self.p5_out = BiFPNDepthwiseConvBlock(feature_size, feature_size, act=act)
-        self.p6_out = BiFPNDepthwiseConvBlock(feature_size, feature_size, act=act)
-        self.p7_out = BiFPNDepthwiseConvBlock(feature_size, feature_size, act=act)
-
-        self.w1 = nn.Parameter(torch.Tensor(2, 4), requires_grad=True)
-        self.w1_relu = nn.ReLU()
-        self.w2 = nn.Parameter(torch.Tensor(3, 4), requires_grad=True)
-        self.w2_relu = nn.ReLU()
-
-        torch.nn.init.constant_(self.w1, 1)
-        torch.nn.init.constant_(self.w2, 1)
-
-    def forward(self, inputs: List[Tensor]) -> List[Tensor]:
-        p3_x, p4_x, p5_x, p6_x, p7_x = inputs
-
-        # Calculate Top-Down Pathway
-        w1 = self.w1_relu(self.w1)
-        w1 = w1 / (torch.sum(w1, dim=0) + self.epsilon)
-
-        w2 = self.w2_relu(self.w2)
-        w2 = w2 / (torch.sum(w2, dim=0) + self.epsilon)
-
-        p7_td = p7_x
-        p6_td = self.p6_td(w1[0, 0] * p6_x + w1[1, 0] * F.interpolate(p7_td, size=p6_x.size()[2:]))
-        p5_td = self.p5_td(w1[0, 1] * p5_x + w1[1, 1] * F.interpolate(p6_td, size=p5_x.size()[2:]))
-        p4_td = self.p4_td(w1[0, 2] * p4_x + w1[1, 2] * F.interpolate(p5_td, size=p4_x.size()[2:]))
-        p3_td = self.p3_td(w1[0, 3] * p3_x + w1[1, 3] * F.interpolate(p4_td, size=p3_x.size()[2:]))
-
-        # Calculate Bottom-Up Pathway
-        p3_out = p3_td
-        p4_out = self.p4_out(
-            w2[0, 0] * p4_x + w2[1, 0] * p4_td + w2[2, 0] * F.interpolate(p3_out, size=p4_x.size()[2:])
-        )
-        p5_out = self.p5_out(
-            w2[0, 1] * p5_x + w2[1, 1] * p5_td + w2[2, 1] * F.interpolate(p4_out, size=p5_x.size()[2:])
-        )
-        p6_out = self.p6_out(
-            w2[0, 2] * p6_x + w2[1, 2] * p6_td + w2[2, 2] * F.interpolate(p5_out, size=p6_x.size()[2:])
-        )
-        p7_out = self.p7_out(
-            w2[0, 3] * p7_x + w2[1, 3] * p7_td + w2[2, 3] * F.interpolate(p6_out, size=p7_x.size()[2:])
+        p2 = self.proj2(self.pool2(x))
+        p4 = self.proj4(self.pool4(x))
+        p8 = self.proj8(self.pool8(x))
+        pg = self.proj_global(self.pool_global(x))
+
+        out_size = p2.size()[2:]
+
+        x = torch.cat(
+            [
+                p2,
+                F.interpolate(p4, size=out_size, mode="nearest"),
+                F.interpolate(p8, size=out_size, mode="nearest"),
+                F.interpolate(pg, size=out_size, mode="nearest"),
+            ],
+            dim=1,
         )
 
-        return [p3_out, p4_out, p5_out, p6_out, p7_out]
+        x = self.blend(x)
+        x = self.conv1(x)
+        x = self.abn1(x)
+        x = self.dropout(x)
+        x = self.conv2(x)
+        x = self.abn2(x)
+        return x
+
+
+class FPNBottleneckBlock(nn.Module):
+    def __init__(self, in_channels: int, out_channels: int, abn_block=ABN, dropout=0.0):
+        """
+
+        Args:
+            encoder_features:
+            decoder_features:
+            output_features:
+            supervision_channels:
+            abn_block:
+            dropout:
+        """
+        super().__init__()
+
+        self.conv1 = nn.Conv2d(in_channels, out_channels, kernel_size=3, padding=1, bias=False)
+        self.abn1 = abn_block(out_channels)
+
+        self.drop1 = nn.Dropout2d(dropout, inplace=False)
+
+        self.conv2 = nn.Conv2d(out_channels, out_channels, kernel_size=3, padding=1, bias=False)
+        self.abn2 = abn_block(out_channels)
 
+    def forward(self, x: Tensor) -> Tensor:  # skipcq: PYL-W0221
 
-class BiFPNDecoder(DecoderModule):
+        x = self.conv1(x)
+        x = self.abn1(x)
+        x = self.drop1(x)
+
+        x = self.conv2(x)
+        x = self.abn2(x)
+        return x
+
+
+class FPNFuse(nn.Module):
+    def __init__(self, mode="bilinear", align_corners=False):
+        super().__init__()
+        self.mode = mode
+        self.align_corners = align_corners
+
+    def forward(self, features: List[Tensor]):  # skipcq: PYL-W0221
+        layers = []
+        dst_size = features[0].size()[2:]  # Skip B, C, and use rest (This works for 1D, 2D, 3D and ND..)
+
+        for f in features:
+            layers.append(F.interpolate(f, size=dst_size, mode=self.mode, align_corners=self.align_corners))
+
+        return torch.cat(layers, dim=1)
+
+
+class FPNFuseSum(nn.Module):
+    """Compute a sum of individual FPN layers"""
+
+    def __init__(self, mode="bilinear", align_corners=False):
+        super().__init__()
+        self.mode = mode
+        self.align_corners = align_corners
+
+    def forward(self, features: List[Tensor]) -> Tensor:  # skipcq: PYL-W0221
+        output = features[0]
+        dst_size = features[0].size()[2:]  # Skip B, C, and use rest (This works for 1D, 2D, 3D and ND..)
+
+        for f in features[1:]:
+            output = output + F.interpolate(f, size=dst_size, mode=self.mode, align_corners=self.align_corners)
+
+        return output
+
+
+class HFF(nn.Module):
     """
-    BiFPN decoder
+    Hierarchical feature fusion module.
+    https://arxiv.org/pdf/1811.11431.pdf
+    https://arxiv.org/pdf/1803.06815.pdf
 
-    Expects input of three feature maps
+    What it does is easily explained in code:
+    feature_map_0 - feature_map of the highest resolution
+    feature_map_N - feature_map of the smallest resolution
 
-    Reference: https://arxiv.org/abs/1911.09070
+    >>> feature_map = feature_map_0 + up(feature_map[1] + up(feature_map[2] + up(feature_map[3] + ...))))
     """
 
-    def __init__(
-        self, feature_maps: List[int], strides: List[int], channels: int = 64, num_layers: int = 2, activation=ACT_RELU
-    ):
-        super(BiFPNDecoder, self).__init__()
-        act = get_activation_block(activation)
-        if len(feature_maps) != 3:
-            raise ValueError("Number of input feature maps must be equal 3")
-        self.p3 = nn.Conv2d(feature_maps[0], channels, kernel_size=(1, 1))
-        self.p4 = nn.Conv2d(feature_maps[1], channels, kernel_size=(1, 1))
-        self.p5 = nn.Conv2d(feature_maps[2], channels, kernel_size=(1, 1))
-
-        # p6 is obtained via a 3x3 stride-2 conv on C5
-        self.p6 = nn.Conv2d(feature_maps[2], channels, kernel_size=(3, 3), stride=(2, 2), padding=1)
-
-        # p7 is computed by applying ReLU followed by a 3x3 stride-2 conv on p6
-        self.p7 = BiFPNConvBlock(channels, channels, kernel_size=3, stride=2, padding=1, act=act)
-
-        bifpns: List[BiFPNBlock] = []
-        for _ in range(num_layers):
-            bifpns.append(BiFPNBlock(channels, act=act))
-        self.bifpn = nn.ModuleList(bifpns)
-
-        self._channels = [channels] * 5
-        self._strides = tuple(strides) + (strides[-1] * 2, strides[-1] * 4)
-
-    @property
-    def channels(self):
-        return self._channels
-
-    @property
-    def strides(self):
-        return self._strides
-
-    def forward(self, inputs: List[Tensor]) -> List[Tensor]:
-        c3, c4, c5 = inputs
-
-        # Calculate the input column of BiFPN
-        p3_x = self.p3(c3)
-        p4_x = self.p4(c4)
-        p5_x = self.p5(c5)
-        p6_x = self.p6(c5)
-        p7_x = self.p7(p6_x)
-
-        features = p3_x, p4_x, p5_x, p6_x, p7_x
-        for bifpn in self.bifpn:
-            features = bifpn(features)
-        return features
+    def __init__(self, sizes=None, upsample_scale=2, mode="nearest", align_corners=None):
+        super().__init__()
+        self.sizes = sizes
+        self.interpolation_mode = mode
+        self.align_corners = align_corners
+        self.upsample_scale = upsample_scale
+
+    def forward(self, features: List[Tensor]) -> Tensor:  # skipcq: PYL-W0221
+        num_feature_maps = len(features)
+
+        current_map = features[-1]
+        for feature_map_index in reversed(range(num_feature_maps - 1)):
+            if self.sizes is not None:
+                prev_upsampled = self._upsample(current_map, self.sizes[feature_map_index])
+            else:
+                prev_upsampled = self._upsample(current_map)
+
+            current_map = features[feature_map_index] + prev_upsampled
+
+        return current_map
+
+    def _upsample(self, x, output_size=None):
+        if output_size is not None:
+            x = F.interpolate(
+                x,
+                size=(output_size[0], output_size[1]),
+                mode=self.interpolation_mode,
+                align_corners=self.align_corners,
+            )
+        else:
+            x = F.interpolate(
+                x, scale_factor=self.upsample_scale, mode=self.interpolation_mode, align_corners=self.align_corners
+            )
+        return x
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/can.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/can.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/deeplab.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/deeplab.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/fpn_cat.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/fpn_cat.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/fpn_sum.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/fpn_sum.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,101 @@
-from typing import List, Union
+from typing import List, Union, Callable, Tuple
+
+import torch
 from torch import Tensor, nn
 import inspect
 
 from .common import SegmentationDecoderModule
-from .. import conv1x1, FPNContextBlock, FPNBottleneckBlock
+from .. import conv1x1, conv3x3, FPNContextBlock, FPNBottleneckBlock, InterpolateLayer
 
 __all__ = ["FPNSumDecoder"]
 
 
 class FPNSumDecoder(SegmentationDecoderModule):
     """
     Feature pyramid network decoder with summation between intermediate layers:
 
         Input
         feature_map[0] -> bottleneck[0](feature_map[0]) + upsample(fpn[1]) -> fpn[0]
         feature_map[1] -> bottleneck[1](feature_map[1]) + upsample(fpn[2]) -> fpn[1]
         feature_map[2] -> bottleneck[2](feature_map[2]) + upsample(fpn[3]) -> fpn[2]
         ...
-        feature_map[n] -> bottleneck[n](feature_map[n]) + upsample(context) -> fpn[n]
+        feature_map[n-1] -> bottleneck[n-1](feature_map[n-1]) + upsample(context) -> fpn[n]
         feature_map[n] -> context_block(feature_map[n]) -> context
     """
 
     def __init__(
         self,
         feature_maps: List[int],
+        strides: List[int],
         channels: int,
-        context_block=FPNContextBlock,
-        bottleneck_block=FPNBottleneckBlock,
-        prediction_block: Union[nn.Identity, conv1x1, nn.Module] = nn.Identity,
-        prediction_channels: int = None,
-        upsample_block=nn.Upsample,
+        bottleneck_block: Callable[[int, int], nn.Module] = conv1x1,
+        prediction_block: Union[nn.Identity, Callable[[int, int], nn.Module]] = conv3x3,
+        upsample_type: Union[str, nn.Module] = "interpolate",
+        upsample_kwargs=None,
     ):
         """
         Create a new instance of FPN decoder with summation of consecutive feature maps.
         :param feature_maps: Number of channels in input feature maps (fine to coarse).
             For instance - [64, 256, 512, 2048]
         :param channels: FPN channels
-        :param context_block:
         :param bottleneck_block:
         :param prediction_block: Optional prediction block to apply to FPN feature maps before returning from decoder
         :param prediction_channels: Number of prediction channels
         :param upsample_block:
+        :param upsample_kwargs:
         """
         super().__init__()
+        if upsample_kwargs is None:
+            upsample_kwargs = {}
+        self.upsample_kwargs = upsample_kwargs
 
-        self.context = context_block(feature_maps[-1], channels)
-
-        self.bottlenecks = nn.ModuleList(
-            [bottleneck_block(in_channels, channels) for in_channels in reversed(feature_maps)]
-        )
+        self.lateral = nn.ModuleList([bottleneck_block(in_channels, channels) for in_channels in feature_maps])
 
         if inspect.isclass(prediction_block) and issubclass(prediction_block, nn.Identity):
-            self.outputs = nn.ModuleList([prediction_block() for _ in reversed(feature_maps)])
-            self.channels = [channels] * len(feature_maps)
+            self.outputs = nn.ModuleList([prediction_block() for _ in feature_maps[:-1]])
         else:
-            self.outputs = nn.ModuleList(
-                [prediction_block(channels, prediction_channels) for _ in reversed(feature_maps)]
-            )
-            self.channels = [prediction_channels] * len(feature_maps)
+            self.outputs = nn.ModuleList([prediction_block(channels, channels) for _ in feature_maps[:-1]])
 
-        if issubclass(upsample_block, nn.Upsample):
-            self.upsamples = nn.ModuleList([upsample_block(scale_factor=2) for _ in reversed(feature_maps)])
-        else:
+        if inspect.isclass(upsample_type) and issubclass(upsample_type, nn.Upsample):
+            self.upsamples = nn.ModuleList([upsample_type(scale_factor=2) for _ in reversed(feature_maps[:-1])])
+        elif isinstance(upsample_type,str) and upsample_type == "interpolate":
             self.upsamples = nn.ModuleList(
-                [upsample_block(channels, channels) for in_channels in reversed(feature_maps)]
+                [InterpolateLayer(self.upsample_kwargs) for _ in reversed(feature_maps[:-1])]
             )
+        else:
+            raise ValueError(f"Unknown upsample type: {upsample_type}")
+
+        self._channels = tuple([channels] * len(feature_maps))
+        self._strides = tuple(strides)
+
+    @property
+    @torch.jit.ignore
+    def channels(self):
+        return self._channels
+
+    @property
+    @torch.jit.ignore
+    def strides(self):
+        return self._strides
 
     def forward(self, feature_maps: List[Tensor]) -> List[Tensor]:
-        last_feature_map = feature_maps[-1]
-        feature_maps = reversed(feature_maps)
+        # Lateral connections
+        lateral_maps = [lateral(feature_map) for feature_map, lateral in zip(feature_maps, self.lateral)]
+
+        last_feature_map = lateral_maps[-1]
+        remaining_feature_maps = lateral_maps[:-1][::-1]
 
-        outputs = []
+        outputs = [last_feature_map]
 
-        fpn = self.context(last_feature_map)
+        for feature_map, upsample, output_block in zip(remaining_feature_maps, self.upsamples, self.outputs):
+            if isinstance(upsample, (InterpolateLayer, nn.ConvTranspose2d)):
+                upsampled = upsample(outputs[-1], output_size=feature_map.shape[-2:])
+            else:
+                upsampled = upsample(outputs[-1])
 
-        for feature_map, bottleneck, upsample, output_block in zip(
-            feature_maps, self.bottlenecks, self.upsamples, self.outputs
-        ):
-            fpn = bottleneck(feature_map) + upsample(fpn)
-            outputs.append(output_block(fpn))
+            fpn = output_block(feature_map + upsampled)
+            outputs.append(fpn)
 
         # Returns list of tensors in same order as input (fine-to-coarse)
-        return outputs[::-1]
+        fine_to_coarse = outputs[::-1]
+        return fine_to_coarse
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/hrnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/hrnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/pyramid_pooling.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/pyramid_pooling.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/unet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/unet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from typing import List, Union, Type
+from typing import List, Union, Type, Tuple
 
 import torch
 from torch import nn
 
 from .common import DecoderModule
 from .. import DeconvolutionUpsample2d
 from ..unet import UnetBlock
 
 __all__ = ["UNetDecoder"]
 
 
 class UNetDecoder(DecoderModule):
+    __constant__ = ["_output_filters", "_output_strides"]
+
     def __init__(
         self,
         feature_maps: List[int],
+        strides: List[int],
         decoder_features: Union[int, List[int]] = None,
         unet_block=UnetBlock,
         upsample_block: Union[nn.Upsample, nn.ConvTranspose2d, Type[nn.PixelShuffle]] = None,
     ):
         super().__init__()
 
         # if not isinstance(decoder_features, list):
@@ -74,20 +77,26 @@
             blocks.append(unet_block(in_channels, out_channels))
 
             in_channels_for_upsample_block = out_channels
             decoder_features[block_index] = out_channels
 
         self.blocks = nn.ModuleList(blocks)
         self.upsamples = nn.ModuleList(upsamples)
-        self.output_filters = decoder_features
+        self._output_filters = decoder_features
+        self._output_strides = tuple(strides[:-1])
 
     @property
     @torch.jit.unused
     def channels(self) -> List[int]:
-        return self.output_filters
+        return self._output_filters
+
+    @property
+    @torch.jit.unused
+    def strides(self) -> Tuple[int, ...]:
+        return self._output_strides
 
     def forward(self, feature_maps: List[torch.Tensor]) -> List[torch.Tensor]:
         x = feature_maps[-1]
         outputs = []
         num_feature_maps = len(feature_maps)
         for index, (upsample_block, decoder_block) in enumerate(zip(self.upsamples, self.blocks)):
             encoder_input = feature_maps[num_feature_maps - index - 2]
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/unet_v2.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/unet_v2.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/decoders/upernet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/decoders/upernet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/dropblock.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/dropblock.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/dsconv.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/dsconv.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/__init__.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/common.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/common.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/densenet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/densenet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/hourglass.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/hourglass.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/hrnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/hrnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/inception.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/inception.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/mobilenet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/mobilenet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/resnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/seresnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/seresnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/squeezenet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/squeezenet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/swin.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/swin.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/common.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/common.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/dpn.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/dpn.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/efficient_net.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/efficient_net.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/efficient_net_v2.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/efficient_net_v2.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/hrnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/nf_regnet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,83 @@
-from .common import GenericTimmEncoder
-from ..common import EncoderModule, _take, make_n_channel_input
-from ...activations import ACT_RELU, get_activation_block
+from .common import GenericTimmEncoder, make_n_channel_input_std_conv
 
-__all__ = ["HRNetW18Encoder", "HRNetW32Encoder", "HRNetW48Encoder", "TimmHRNetW18SmallV2Encoder"]
 
+__all__ = [
+    "NFRegNetB0Encoder",
+    "NFRegNetB1Encoder",
+    "NFRegNetB2Encoder",
+    "NFRegNetB3Encoder",
+    "NFRegNetB4Encoder",
+    "NFRegNetB5Encoder",
+]
 
-class HRNetW18Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, use_incre_features: bool = True, layers=None):
-        from timm.models import hrnet
 
-        encoder = hrnet.hrnet_w18(
-            pretrained=pretrained,
-            feature_location="incre" if use_incre_features else "",
-            features_only=True,
-            out_indices=(0, 1, 2, 3, 4),
-        )
-        super().__init__(encoder, layers)
+class NFRegNetB0Encoder(GenericTimmEncoder):
+    def __init__(self, pretrained=True, layers=None):
+        from timm.models import nfnet
 
-    def forward(self, x):
-        y = self.encoder.forward(x)
-        return _take(y, self._layers)
+        encoder = nfnet.nf_regnet_b0(pretrained=pretrained, features_only=True)
+        super().__init__(encoder, layers)
 
     def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.conv1 = make_n_channel_input(self.encoder.conv1, input_channels, mode, **kwargs)
+        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
         return self
 
 
-class HRNetW32Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, use_incre_features: bool = True, layers=None):
-        from timm.models import hrnet
+class NFRegNetB1Encoder(GenericTimmEncoder):
+    def __init__(self, pretrained=True, layers=None):
+        from timm.models import nfnet
 
-        encoder = hrnet.hrnet_w32(
-            pretrained=pretrained,
-            feature_location="incre" if use_incre_features else "",
-            features_only=True,
-            out_indices=(0, 1, 2, 3, 4),
-        )
+        encoder = nfnet.nf_regnet_b1(pretrained=pretrained, features_only=True)
         super().__init__(encoder, layers)
 
-    def forward(self, x):
-        y = self.encoder.forward(x)
-        return _take(y, self._layers)
+    def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
+        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
+        return self
+
+
+class NFRegNetB2Encoder(GenericTimmEncoder):
+    def __init__(self, pretrained=True, layers=None):
+        from timm.models import nfnet
+
+        encoder = nfnet.nf_regnet_b2(pretrained=pretrained, features_only=True)
+        super().__init__(encoder, layers)
 
     def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.conv1 = make_n_channel_input(self.encoder.conv1, input_channels, mode, **kwargs)
+        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
         return self
 
 
-class HRNetW48Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, use_incre_features: bool = True, layers=None):
-        from timm.models import hrnet
+class NFRegNetB3Encoder(GenericTimmEncoder):
+    def __init__(self, pretrained=True, layers=None):
+        from timm.models import nfnet
 
-        encoder = hrnet.hrnet_w48(
-            pretrained=pretrained,
-            feature_location="incre" if use_incre_features else "",
-            features_only=True,
-            out_indices=(0, 1, 2, 3, 4),
-        )
+        encoder = nfnet.nf_regnet_b3(pretrained=pretrained, features_only=True)
         super().__init__(encoder, layers)
 
-    def forward(self, x):
-        y = self.encoder.forward(x)
-        return _take(y, self._layers)
+    def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
+        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
+        return self
+
+
+class NFRegNetB4Encoder(GenericTimmEncoder):
+    def __init__(self, pretrained=True, layers=None):
+        from timm.models import nfnet
+
+        encoder = nfnet.nf_regnet_b4(pretrained=pretrained, features_only=True)
+        super().__init__(encoder, layers)
 
     def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.conv1 = make_n_channel_input(self.encoder.conv1, input_channels, mode, **kwargs)
+        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
         return self
 
 
-class TimmHRNetW18SmallV2Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, use_incre_features: bool = True, layers=None, activation=ACT_RELU):
-        from timm.models import hrnet
+class NFRegNetB5Encoder(GenericTimmEncoder):
+    def __init__(self, pretrained=True, layers=None):
+        from timm.models import nfnet
 
-        encoder = hrnet.hrnet_w18_small_v2(
-            pretrained=pretrained,
-            feature_location="incre" if use_incre_features else "",
-            features_only=True,
-            out_indices=(0, 1, 2, 3, 4),
-        )
+        encoder = nfnet.nf_regnet_b5(pretrained=pretrained, features_only=True)
         super().__init__(encoder, layers)
 
     def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.conv1 = make_n_channel_input(self.encoder.conv1, input_channels, mode, **kwargs)
+        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
         return self
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/nf_regnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/hrnet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from .common import GenericTimmEncoder, make_n_channel_input_std_conv
+from .common import GenericTimmEncoder
+from ..common import EncoderModule, _take, make_n_channel_input
+from ...activations import ACT_RELU, get_activation_block
 
+__all__ = ["HRNetW18Encoder", "HRNetW32Encoder", "HRNetW48Encoder", "TimmHRNetW18SmallV2Encoder"]
 
-__all__ = [
-    "NFRegNetB0Encoder",
-    "NFRegNetB1Encoder",
-    "NFRegNetB2Encoder",
-    "NFRegNetB3Encoder",
-    "NFRegNetB4Encoder",
-    "NFRegNetB5Encoder",
-]
 
+class HRNetTimmEncoder(GenericTimmEncoder):
+    def __init__(self, encoder, first_conv_stride_one, layers):
+        if first_conv_stride_one:
+            encoder.conv1.stride = (1, 1)
 
-class NFRegNetB0Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, layers=None):
-        from timm.models import nfnet
-
-        encoder = nfnet.nf_regnet_b0(pretrained=pretrained, features_only=True)
         super().__init__(encoder, layers)
+        if first_conv_stride_one:
+            self._output_strides = (s // 2 for s in self._output_strides)
 
-    def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
-        return self
-
-
-class NFRegNetB1Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, layers=None):
-        from timm.models import nfnet
-
-        encoder = nfnet.nf_regnet_b1(pretrained=pretrained, features_only=True)
-        super().__init__(encoder, layers)
+    def forward(self, x):
+        y = self.encoder.forward(x)
+        return _take(y, self._layers)
 
     def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
+        self.encoder.conv1 = make_n_channel_input(self.encoder.conv1, input_channels, mode, **kwargs)
         return self
 
 
-class NFRegNetB2Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, layers=None):
-        from timm.models import nfnet
+class HRNetW18Encoder(HRNetTimmEncoder):
+    def __init__(
+        self, pretrained=True, use_incre_features: bool = True, layers=None, first_conv_stride_one: bool = False
+    ):
+        from timm.models import hrnet
 
-        encoder = nfnet.nf_regnet_b2(pretrained=pretrained, features_only=True)
-        super().__init__(encoder, layers)
+        encoder = hrnet.hrnet_w18(
+            pretrained=pretrained,
+            feature_location="incre" if use_incre_features else "",
+            features_only=True,
+            out_indices=(0, 1, 2, 3, 4),
+        )
+        super().__init__(encoder, first_conv_stride_one=first_conv_stride_one, layers=layers)
 
-    def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
-        return self
 
+class HRNetW32Encoder(HRNetTimmEncoder):
+    def __init__(
+        elf, pretrained=True, use_incre_features: bool = True, layers=None, first_conv_stride_one: bool = False
+    ):
+        from timm.models import hrnet
 
-class NFRegNetB3Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, layers=None):
-        from timm.models import nfnet
+        encoder = hrnet.hrnet_w32(
+            pretrained=pretrained,
+            feature_location="incre" if use_incre_features else "",
+            features_only=True,
+            out_indices=(0, 1, 2, 3, 4),
+        )
+        super().__init__(encoder, first_conv_stride_one=first_conv_stride_one, layers=layers)
 
-        encoder = nfnet.nf_regnet_b3(pretrained=pretrained, features_only=True)
-        super().__init__(encoder, layers)
 
-    def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
-        return self
-
-
-class NFRegNetB4Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, layers=None):
-        from timm.models import nfnet
+class HRNetW48Encoder(HRNetTimmEncoder):
+    def __init__(
+        elf, pretrained=True, use_incre_features: bool = True, layers=None, first_conv_stride_one: bool = False
+    ):
+        from timm.models import hrnet
 
-        encoder = nfnet.nf_regnet_b4(pretrained=pretrained, features_only=True)
-        super().__init__(encoder, layers)
+        encoder = hrnet.hrnet_w48(
+            pretrained=pretrained,
+            feature_location="incre" if use_incre_features else "",
+            features_only=True,
+            out_indices=(0, 1, 2, 3, 4),
+        )
+        super().__init__(encoder, first_conv_stride_one=first_conv_stride_one, layers=layers)
 
-    def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
-        return self
 
+class TimmHRNetW18SmallV2Encoder(HRNetTimmEncoder):
+    def __init__(
+        self, elf, pretrained=True, use_incre_features: bool = True, layers=None, first_conv_stride_one: bool = False
+    ):
+        from timm.models import hrnet
 
-class NFRegNetB5Encoder(GenericTimmEncoder):
-    def __init__(self, pretrained=True, layers=None):
-        from timm.models import nfnet
-
-        encoder = nfnet.nf_regnet_b5(pretrained=pretrained, features_only=True)
-        super().__init__(encoder, layers)
-
-    def change_input_channels(self, input_channels: int, mode="auto", **kwargs):
-        self.encoder.stem_conv = make_n_channel_input_std_conv(self.encoder.stem_conv, input_channels, mode, **kwargs)
-        return self
+        encoder = hrnet.hrnet_w18_small_v2(
+            pretrained=pretrained,
+            feature_location="incre" if use_incre_features else "",
+            features_only=True,
+            out_indices=(0, 1, 2, 3, 4),
+        )
+        super().__init__(encoder, first_conv_stride_one=first_conv_stride_one, layers=layers)
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/nfnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/nfnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/res2net.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/res2net.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/timm/resnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/timm/resnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/unet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/unet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/wide_resnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/wide_resnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/encoders/xresnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/encoders/xresnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/ocnet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/ocnet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/pooling.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/scse.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/scse.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/srm.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/srm.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/unet.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/unet.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/modules/upsample.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/modules/upsample.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import warnings
-from typing import Optional, List
+from typing import Optional, List, Dict, Any, Tuple
 
 import torch
 from torch import nn, Tensor
 from math import hypot
 
 __all__ = [
     "bilinear_upsample_initializer",
     "icnr_init",
     "DepthToSpaceUpsample2d",
     "BilinearAdditiveUpsample2d",
     "DeconvolutionUpsample2d",
     "ResidualDeconvolutionUpsample2d",
+    "InterpolateLayer",
 ]
 
 
 def bilinear_upsample_initializer(x):
     cc = x.size(2) // 2
     cr = x.size(3) // 2
 
@@ -148,7 +149,16 @@
     def forward(self, x: Tensor) -> Tensor:  # skipcq: PYL-W0221
         residual_up = self.residual(x)
         return self.conv(x, output_size=residual_up.size()) + residual_up
 
     def init_weights(self):
         torch.nn.init.kaiming_normal_(self.conv.weight, nonlinearity="linear")
         torch.nn.init.zeros_(self.conv.bias)
+
+
+class InterpolateLayer(nn.Module):
+    def __init__(self, interpolate_kwargs: Dict[str, Any]):
+        super().__init__()
+        self.interpolate_kwargs = interpolate_kwargs
+
+    def forward(self, x: Tensor, output_size: Tuple[int, int]) -> Tensor:
+        return torch.nn.functional.interpolate(x, size=output_size, **self.interpolate_kwargs)
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/optimization/functional.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/optimization/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/optimization/lr_schedules.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/optimization/lr_schedules.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/bboxes_utils.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/bboxes_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/distributed.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/distributed.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "is_dist_avail_and_initialized",
     "is_main_process",
     "master_print",
     "reduce_dict_sum",
     "split_across_nodes",
 ]
 
-logger = logging.getLogger("DistributedGuard")
+logger = logging.getLogger("pytorch_toolbelt.utils.distributed")
 
 
 class DistributedGuard:
     def __init__(
         self,
         local_rank: int = os.environ.get("LOCAL_RANK", 0),
         world_size: int = os.environ.get("WORLD_SIZE", 1),
@@ -154,15 +154,15 @@
     """
     world_size = get_world_size()
     if world_size == 1:
         return [data]
 
     # serialized to a Tensor
     buffer = pickle.dumps(data)
-    storage = torch.ByteStorage.from_buffer(buffer)
+    storage = torch.UntypedStorage.from_buffer(buffer, dtype=torch.uint8)
     tensor = torch.ByteTensor(storage).to("cuda")
 
     # obtain Tensor size of each rank
     local_size = torch.tensor([tensor.numel()], device="cuda")
     size_list = [torch.tensor([0], device="cuda") for _ in range(world_size)]
     dist.all_gather(size_list, local_size)
     size_list = [int(size.item()) for size in size_list]
@@ -226,17 +226,15 @@
         None
     """
     if is_main_process():
         print(*args, **kwargs)
 
 
 def split_across_nodes(
-    collection: List,
-    world_size: Optional[int] = None,
-    local_rank: Optional[int] = None,
+    collection: List, world_size: Optional[int] = None, local_rank: Optional[int] = None, cost: Optional[List] = None
 ) -> List:
     """
     Split input collection such that each node receives 1/N of the total collection elements to process, where
     N is the number of nodes.
 
     Example:
 
@@ -244,29 +242,51 @@
     >>> print(local_values, get_rank())
     >>> # [0,1,2], 0
     >>> # [3,4,5], 1
     >>> # [6,7,8], 2
     >>> # [9], 3
 
     Args:
-        collection:
-        world_size:
-        local_rank:
+        collection: Initial collection of size N to split into K nodes
+        world_size: World size (Number of nodes K)
+        local_rank: Current node
+        cost: A vector of size N that represents the cost of processing associated with each item.
+              If present, it will affect the order of elements each node will receive to even the total cost each node
+              will get.
 
     Returns:
 
     """
     if world_size is None:
         world_size = get_world_size()
     if local_rank is None:
         local_rank = get_rank()
 
     if world_size > 1:
-        indexes = np.linspace(0, len(collection), int(world_size + 1), dtype=int)
-        rank_local_indexes = slice(indexes[local_rank], indexes[local_rank + 1])
-        rank_specific_subset = collection[rank_local_indexes]
-        logger.debug(
-            f"split_across_nodes returning slice {rank_local_indexes} from collection of size {len(collection)} for rank {local_rank}"
-        )
+        if cost is not None:
+            if len(cost) != len(collection):
+                raise RuntimeError()
+            ordered_indexes = np.argsort(cost)
+            rank_local_indexes = (ordered_indexes % world_size) == local_rank
+
+            logger.debug(
+                f"Node {local_rank} get {np.count_nonzero(rank_local_indexes)} items with total cost {sum(cost[rank_local_indexes])}"
+            )
+
+            if isinstance(collection, np.ndarray):
+                rank_specific_subset = collection[rank_local_indexes]
+            else:
+                rank_specific_subset = [
+                    collection[index] for index, should_pick in enumerate(rank_local_indexes) if should_pick
+                ]
+
+        else:
+            indexes = np.linspace(0, len(collection), int(world_size + 1), dtype=int)
+            rank_local_indexes = slice(indexes[local_rank], indexes[local_rank + 1])
+            rank_specific_subset = collection[rank_local_indexes]
+
+            logger.debug(
+                f"split_across_nodes returning slice {rank_local_indexes} from collection of size {len(collection)} for rank {local_rank}"
+            )
         return rank_specific_subset
     else:
         return collection
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/fs.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/fs.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/namesgenerator.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/namesgenerator.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/python_utils.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/random.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/random.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/rle.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/rle.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/support.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/support.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/torch_utils.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/torch_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "tensor_from_rgb_image",
     "to_numpy",
     "to_tensor",
     "transfer_weights",
     "move_to_device_non_blocking",
     "describe_outputs",
     "get_collate_for_dataset",
+    "get_non_wrapped_model",
 ]
 
 
 def softmax_over_dim_0(x: Tensor) -> Tensor:
     return torch.softmax(x, dim=0)
 
 
@@ -197,15 +198,15 @@
 
     if len(image.shape) == 2:
         if dummy_channels_dim:
             image = np.expand_dims(image, 0)
     else:
         # HWC -> CHW
         image = np.moveaxis(image, -1, 0)
-    image = np.ascontiguousarray(image)
+    image = np.require(image, requirements="C")
     image = torch.from_numpy(image)
     return image
 
 
 @pytorch_toolbelt_deprecated("This function is deprecated, please use image_to_tensor instead")
 def tensor_from_rgb_image(image: np.ndarray) -> torch.Tensor:
     return image_to_tensor(image)
@@ -342,18 +343,39 @@
 
     Returns:
         Collate function to put into DataLoader
     """
     collate_fn = default_collate
 
     if hasattr(dataset, "get_collate_fn"):
-        collate_fn = dataset.get_collate_fn()
-
-    if isinstance(dataset, ConcatDataset):
+        return dataset.get_collate_fn()
+    elif isinstance(dataset, ConcatDataset):
         collates = set(get_collate_for_dataset(ds) for ds in dataset.datasets)
         if len(collates) != 1:
             raise RuntimeError(
                 "Detected ConcatDataset with datasets having different collate functions. " "This is not supported."
             )
         collate_fn = collates[0]
 
     return collate_fn
+
+
+def get_non_wrapped_model(model: nn.Module) -> nn.Module:
+    """
+    Return real model from (maybe) wrapped in DP / DDP
+
+    Args:
+        model:
+
+    Returns:
+
+    """
+    from torch.nn import DataParallel
+    from torch.nn.parallel import DistributedDataParallel
+
+    if not isinstance(model, nn.Module):
+        raise RuntimeError("Input model must be a subclass of nn.Module.")
+
+    if isinstance(model, (DataParallel, DistributedDataParallel)):
+        model = model.module
+
+    return model
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/utils/visualization.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt/zoo/segmentation.py` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt/zoo/segmentation.py`

 * *Files identical despite different names*

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt.egg-info/PKG-INFO` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-toolbelt
-Version: 0.6.2
+Version: 0.6.3
 Summary: PyTorch extensions for fast R&D prototyping and Kaggle farming
 Home-page: https://github.com/BloodAxe/pytorch-toolbelt
 Author: Eugene Khvedchenya
 Author-email: ekhvedchenya@gmail.com
 License: License :: OSI Approved :: MIT License
 Description: 
         # Important Update
```

### Comparing `pytorch_toolbelt-0.6.2/pytorch_toolbelt.egg-info/SOURCES.txt` & `pytorch_toolbelt-0.6.3/pytorch_toolbelt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 pytorch_toolbelt/losses/balanced_bce.py
 pytorch_toolbelt/losses/bitempered_loss.py
 pytorch_toolbelt/losses/dice.py
 pytorch_toolbelt/losses/focal.py
 pytorch_toolbelt/losses/focal_cosine.py
 pytorch_toolbelt/losses/functional.py
 pytorch_toolbelt/losses/jaccard.py
-pytorch_toolbelt/losses/joint_loss.py
 pytorch_toolbelt/losses/logcosh.py
 pytorch_toolbelt/losses/lovasz.py
 pytorch_toolbelt/losses/soft_bce.py
 pytorch_toolbelt/losses/soft_ce.py
 pytorch_toolbelt/losses/soft_f1.py
 pytorch_toolbelt/losses/wing_loss.py
 pytorch_toolbelt/modules/__init__.py
```

### Comparing `pytorch_toolbelt-0.6.2/setup.py` & `pytorch_toolbelt-0.6.3/setup.py`

 * *Files identical despite different names*

