# Comparing `tmp/hcpdiff-0.3.5.tar.gz` & `tmp/hcpdiff-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.3.5.tar", last modified: Sat May  6 12:27:12 2023, max compression
+gzip compressed data, was "hcpdiff-0.3.6.tar", last modified: Sun May  7 06:04:11 2023, max compression
```

## Comparing `hcpdiff-0.3.5.tar` & `hcpdiff-0.3.6.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.887558 hcpdiff-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-06 12:27:12.887558 hcpdiff-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.867557 hcpdiff-0.3.5/cfgs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.867557 hcpdiff-0.3.5/cfgs/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/infer/change_vae.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/infer/euler_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/infer/img2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/infer/img2img_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/infer/text2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/infer/text2img_DA++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/infer/webui_model_infer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.871558 hcpdiff-0.3.5/cfgs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/plugins/plugin_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/te_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.871558 hcpdiff-0.3.5/cfgs/train/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.871558 hcpdiff-0.3.5/cfgs/train/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/CustomDiffusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/DreamArtist++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/DreamArtist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/DreamBooth.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/TextualInversion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/fine-tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/locon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/lora_conventional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/examples/min_snr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/train_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/train/tuning_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/cfgs/unet_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.871558 hcpdiff-0.3.5/hcpdiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.875558 hcpdiff-0.3.5/hcpdiff/ckpt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/ckpt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/ckpt_manager/ckpt_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/ckpt_manager/ckpt_safetensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.875558 hcpdiff-0.3.5/hcpdiff/data/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/data/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/data/cond_pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/data/pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.875558 hcpdiff-0.3.5/hcpdiff/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/loggers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/loggers/cli_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.875558 hcpdiff-0.3.5/hcpdiff/loss/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/loss/min_snr_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/loss/mse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.879557 hcpdiff-0.3.5/hcpdiff/models/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/cfg_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/lora_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/text_emb_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/textencoder_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/models/tokenizer_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.883558 hcpdiff-0.3.5/hcpdiff/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/tools/convert_caption_txt2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/tools/create_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/tools/gen_from_ptlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/tools/init_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/tools/lora_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/tools/sd2diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26244 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/train_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/train_ac_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/train_colo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.883558 hcpdiff-0.3.5/hcpdiff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/utils/caption_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/utils/cfg_net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/utils/colo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/utils/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/utils/img_size_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/hcpdiff/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.875558 hcpdiff-0.3.5/hcpdiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-06 12:27:12.000000 hcpdiff-0.3.5/hcpdiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-06 12:27:12.000000 hcpdiff-0.3.5/hcpdiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 12:27:12.000000 hcpdiff-0.3.5/hcpdiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 12:27:12.000000 hcpdiff-0.3.5/hcpdiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-06 12:27:12.000000 hcpdiff-0.3.5/hcpdiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 12:27:12.000000 hcpdiff-0.3.5/hcpdiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:12.887558 hcpdiff-0.3.5/prompt_tuning_template/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/prompt_tuning_template/caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/prompt_tuning_template/name.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/prompt_tuning_template/name_2pt_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/prompt_tuning_template/name_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/prompt_tuning_template/object.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/prompt_tuning_template/object_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/prompt_tuning_template/style.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/prompt_tuning_template/style_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 12:27:12.887558 hcpdiff-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-06 12:26:58.000000 hcpdiff-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.975398 hcpdiff-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-07 06:04:11.975398 hcpdiff-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.955398 hcpdiff-0.3.6/cfgs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.955398 hcpdiff-0.3.6/cfgs/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/change_vae.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/euler_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/img2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/img2img_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/text2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/text2img_DA++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/webui_model_infer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.955398 hcpdiff-0.3.6/cfgs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/plugins/plugin_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/te_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.955398 hcpdiff-0.3.6/cfgs/train/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.959398 hcpdiff-0.3.6/cfgs/train/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/CustomDiffusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/DreamArtist++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/DreamArtist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/DreamBooth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/Lion_optimizer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/TextualInversion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/fine-tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/locon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/lora_conventional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/min_snr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/train_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/tuning_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/unet_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.959398 hcpdiff-0.3.6/hcpdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.963398 hcpdiff-0.3.6/hcpdiff/ckpt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/ckpt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/ckpt_manager/ckpt_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/ckpt_manager/ckpt_safetensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.963398 hcpdiff-0.3.6/hcpdiff/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/cond_pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.963398 hcpdiff-0.3.6/hcpdiff/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/cli_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.963398 hcpdiff-0.3.6/hcpdiff/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loss/min_snr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loss/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.967398 hcpdiff-0.3.6/hcpdiff/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/cfg_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/lora_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/text_emb_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/textencoder_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/tokenizer_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.967398 hcpdiff-0.3.6/hcpdiff/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/convert_caption_txt2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/create_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/gen_from_ptlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/init_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/lora_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/sd2diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27094 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/train_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/train_ac_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/train_colo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.971398 hcpdiff-0.3.6/hcpdiff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/caption_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/cfg_net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/colo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/img_size_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.959398 hcpdiff-0.3.6/hcpdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.975398 hcpdiff-0.3.6/prompt_tuning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/name.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/name_2pt_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/name_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/object.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/object_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/style.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/style_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 06:04:11.975398 hcpdiff-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/setup.py
```

### Comparing `hcpdiff-0.3.5/LICENSE` & `hcpdiff-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/PKG-INFO` & `hcpdiff-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.3.5
+Version: 0.3.6
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -54,14 +54,16 @@
 * colossal-AI
 * xformers for unet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
 * safetensors support
 * Controlnet (support train)
 * Min-SNR loss
+* Custom optimizer (Lion, DAdaptation, pytorch-optimizer, ...)
+* Custom lr scheduler
 
 ## Install
 
 Install with pip:
 ```bash
 pip install hcpdiff
 # Start a new project and make initialization
```

### Comparing `hcpdiff-0.3.5/README.md` & `hcpdiff-0.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 * colossal-AI
 * xformers for unet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
 * safetensors support
 * Controlnet (support train)
 * Min-SNR loss
+* Custom optimizer (Lion, DAdaptation, pytorch-optimizer, ...)
+* Custom lr scheduler
 
 ## Install
 
 Install with pip:
 ```bash
 pip install hcpdiff
 # Start a new project and make initialization
```

### Comparing `hcpdiff-0.3.5/cfgs/infer/euler_a.yaml` & `hcpdiff-0.3.6/cfgs/infer/euler_a.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/infer/img2img.yaml` & `hcpdiff-0.3.6/cfgs/infer/img2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/infer/img2img_controlnet.yaml` & `hcpdiff-0.3.6/cfgs/infer/img2img_controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/infer/text2img.yaml` & `hcpdiff-0.3.6/cfgs/infer/text2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/infer/text2img_DA++.yaml` & `hcpdiff-0.3.6/cfgs/infer/text2img_DA++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/infer/webui_model_infer.yaml` & `hcpdiff-0.3.6/cfgs/infer/webui_model_infer.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/te_struct.txt` & `hcpdiff-0.3.6/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/DreamArtist++.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -2,76 +2,91 @@
 
 unet: null
 
 lora_unet:
   - lr: 1e-4
     rank: 0.01875
     branch: p
+    dropout: 0.1
     layers:
-      - 're:.*\.attn.?$'
-      #- 're:.*\.ff\.net\.0$' # Increases fitness, but potentially reduces controllability
+      - 're:.*\.to_k$'
+      - 're:.*\.to_v$'
+      - 're:.*\.ff$'
+      #- 're:.*\.attn.?$' # Increases fitness, but potentially reduces controllability
   - lr: 4e-5 # Low negative unet lr prevents image collapse
     rank: 0.01875
     branch: n
+    dropout: 0.1
     layers:
-      - 're:.*\.attn.?$'
-      #- 're:.*\.ff\.net\.0$' # Increases fitness, but potentially reduces controllability
+      - 're:.*\.to_k$'
+      - 're:.*\.to_v$'
+      - 're:.*\.ff$'
+      #- 're:.*\.attn.?$' # Increases fitness, but potentially reduces controllability
   #  - lr: 1e-4
   #    rank: 0.01875
   #    type: p
   #    layers:
   #      - 're:.*\.resnets$' # Increases fitness, but potentially reduces controllability and change style
   #  - lr: 4e-5
   #    rank: 0.01875
   #    type: n
   #    layers:
   #      - 're:.*\.resnets$' # Increases fitness, but potentially reduces controllability and change style
 
 lora_text_encoder:
-  - lr: 1e-5
-    rank: 0.01
+  - lr: 2e-5
+    rank: 2
     branch: p
+    dropout: 0.1
     layers:
       - 're:.*self_attn$'
       - 're:.*mlp$'
-  - lr: 1e-5
-    rank: 0.01
+  - lr: 2e-5
+    rank: 2
     branch: n
+    dropout: 0.1
     layers:
       - 're:.*self_attn$'
       - 're:.*mlp$'
 
 tokenizer_pt:
   train: # prompt tuning embeddings
-    - { name: 'pt-botdog1', lr: 0.003 }
-    - { name: 'pt-botdog1-neg', lr: 0.003 }
+    - { name: 'pt-botdog1', lr: 0.0025 }
+    - { name: 'pt-botdog1-neg', lr: 0.0025 }
 
 train:
   gradient_accumulation_steps: 1
   save_step: 100
 
   #cfg_scale: '1.0-3.0:cos' # dynamic CFG with timestamp
   cfg_scale: '3.0'
 
+  loss:
+    criterion: # min SNR loss
+      _target_: hcpdiff.loss.MinSNRLoss
+      gamma: 2.0
+
   scheduler:
-    name: 'constant_with_warmup'
-    num_warmup_steps: 50
+    name: one_cycle
+    num_warmup_steps: 200
     num_training_steps: 1000
+    scheduler_kwargs: { }
 
   scheduler_pt:
-    name: 'one_cycle'
+    name: one_cycle
     num_warmup_steps: 200
     num_training_steps: 1000
     scheduler_kwargs: {}
 
 model:
   pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
   tokenizer_repeats: 1
   ema_unet: 0
   ema_text_encoder: 0
+  clip_skip: 0
 
 data:
   dataset1:
     batch_size: 4
     cache_latents: True
     loss_weight: 1.0
```

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/controlnet.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/locon.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/locon.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.3.6/cfgs/train/examples/lora_conventional.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/train/train_base.yaml` & `hcpdiff-0.3.6/cfgs/train/train_base.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ckpt_type: 'safetensors' # [torch, safetensors]
 
 vis_info:
   prompt: null
   negative_prompt: ''
 
 train:
+  train_steps: 1000
   gradient_accumulation_steps: 1
   workers: 4
   max_grad_norm: 1.0
   set_grads_to_none: False
   save_step: 100
   cfg_scale: '1.0' # for DreamArtist
 
@@ -31,15 +32,18 @@
       _partial_: True
       reduction: 'none' # support for attention mask
     type: 'eps' # 'eps' or 'sample'
 
   optimizer:
     type: adamw
     weight_decay: 1e-3
-    weight_decay_pt: 5e-4
+
+  optimizer_pt:
+    type: adamw
+    weight_decay: 5e-4
 
   scale_lr: True # auto scale lr with total batch size
   scheduler:
     name: 'one_cycle'
     num_warmup_steps: 200
     num_training_steps: 1000
     scheduler_kwargs: {} # args for scheduler
@@ -54,15 +58,15 @@
     out_path: 'train.log'
     log_step: 20
 
 model:
   revision: null
   pretrained_model_name_or_path: null
   tokenizer_name: null
-  tokenizer_repeats: 3
+  tokenizer_repeats: 2
   enable_xformers: True
   gradient_checkpointing: True
   ema_unet: 0 # 0 to disable
   ema_text_encoder: 0 # 0 to disable
   clip_skip: 0
   noise_scheduler: DDPMScheduler
```

### Comparing `hcpdiff-0.3.5/cfgs/train/tuning_base.yaml` & `hcpdiff-0.3.6/cfgs/train/tuning_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/cfgs/unet_struct.txt` & `hcpdiff-0.3.6/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.3.6/hcpdiff/ckpt_manager/ckpt_pkl.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.3.6/hcpdiff/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/data/__init__.py` & `hcpdiff-0.3.6/hcpdiff/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/data/bucket.py` & `hcpdiff-0.3.6/hcpdiff/data/bucket.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/data/cond_pair_dataset.py` & `hcpdiff-0.3.6/hcpdiff/data/cond_pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.3.6/hcpdiff/data/pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/data/utils.py` & `hcpdiff-0.3.6/hcpdiff/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         datas['cond'] = torch.stack(datas['cond'])
     datas['prompt'] = torch.stack(sn_list)
 
     return datas
 
 class CycleData():
     def __init__(self, data_loader):
-        print(data_loader)
         self.data_loader = data_loader
 
     def __iter__(self):
         self.epoch = 0
         def cycle():
             while True:
                 self.data_loader.dataset.bucket.rest(self.epoch)
```

### Comparing `hcpdiff-0.3.5/hcpdiff/loggers/base_logger.py` & `hcpdiff-0.3.6/hcpdiff/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/loggers/cli_logger.py` & `hcpdiff-0.3.6/hcpdiff/loggers/cli_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/loggers/tensorboard_logger.py` & `hcpdiff-0.3.6/hcpdiff/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/loggers/wandb_logger.py` & `hcpdiff-0.3.6/hcpdiff/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/loss/min_snr_loss.py` & `hcpdiff-0.3.6/hcpdiff/loss/min_snr_loss.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/cfg_context.py` & `hcpdiff-0.3.6/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/controlnet.py` & `hcpdiff-0.3.6/hcpdiff/models/controlnet.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/layers.py` & `hcpdiff-0.3.6/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/lora_base.py` & `hcpdiff-0.3.6/hcpdiff/models/lora_base.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/lora_layers.py` & `hcpdiff-0.3.6/hcpdiff/models/lora_layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/plugin.py` & `hcpdiff-0.3.6/hcpdiff/models/plugin.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.3.6/hcpdiff/models/text_emb_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.3.6/hcpdiff/models/textencoder_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.3.6/hcpdiff/models/tokenizer_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.3.6/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 for file in os.listdir(args.data_root):
     ext_idx = file.rfind('.')
     file_name = file[:ext_idx]
     if file[ext_idx + 1:] in types_support:
         captions[file] = get_txt_caption(os.path.join(args.data_root, f'{file_name}.txt'))
 
 with open(os.path.join(args.data_root, f'image_captions.json'), "w", encoding='utf8') as f:
-    json.dump(captions, f)
+    json.dump(captions, f, indent=2, ensure_ascii=False)
```

### Comparing `hcpdiff-0.3.5/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.3.6/hcpdiff/tools/create_embedding.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.3.6/hcpdiff/tools/gen_from_ptlist.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/tools/init_proj.py` & `hcpdiff-0.3.6/hcpdiff/tools/init_proj.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/tools/lora_convert.py` & `hcpdiff-0.3.6/hcpdiff/tools/lora_convert.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/tools/sd2diffusers.py` & `hcpdiff-0.3.6/hcpdiff/tools/sd2diffusers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/train_ac.py` & `hcpdiff-0.3.6/hcpdiff/train_ac.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import transformers
 from accelerate import Accelerator, DistributedDataParallelKwargs
 from accelerate.utils import set_seed
 from diffusers import AutoencoderKL, UNet2DConditionModel
 from diffusers.utils.import_utils import is_xformers_available
 from omegaconf import OmegaConf
 from transformers import AutoTokenizer
+from  functools import partial
 
 from hcpdiff.ckpt_manager import CkptManagerPKL, CkptManagerSafe
 from hcpdiff.data import RatioBucket, DataGroup, collate_fn_ft
 from hcpdiff.loggers import LoggerGroup
 from hcpdiff.models import EmbeddingPTHook, TEEXHook, CFGContext, DreamArtistPTContext
 from hcpdiff.utils.cfg_net_tools import make_hcpdiff, make_plugin
 from hcpdiff.utils.ema import ModelEMA
@@ -325,45 +326,61 @@
 
         return train_params_unet+train_params_text_encoder, train_params_emb
 
     def build_optimizer_scheduler(self):
         # set optimizer
         parameters, parameters_pt = self.get_param_group_train()
 
-        cfg_opt = self.cfgs.train.optimizer
         if len(parameters)>0:  # do fine-tuning
+            cfg_opt = self.cfgs.train.optimizer
             if self.cfgs.train.scale_lr:
                 self.scale_lr(parameters)
 
-            if cfg_opt.type == 'adamw_8bit':
+            if isinstance(cfg_opt, partial):
+                if 'type' in cfg_opt.keywords:
+                    del cfg_opt.keywords['type']
+                self.optimizer = cfg_opt(parameters, lr=self.lr)
+            elif cfg_opt.type == 'adamw_8bit':
                 import bitsandbytes as bnb
                 self.optimizer = bnb.optim.AdamW8bit(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
             elif cfg_opt.type == 'deepspeed' and self.accelerator.state.deepspeed_plugin is not None:
                 from deepspeed.ops.adam import FusedAdam
                 self.optimizer = FusedAdam(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
             elif cfg_opt.type == 'adamw':
                 self.optimizer = torch.optim.AdamW(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
             else:
-                self.optimizer = cfg_opt.optimizer.opt(parameters, lr=self.lr)
+                raise NotImplementedError(f'Unknown optimizer {cfg_opt.type}')
 
-            self.lr_scheduler = get_scheduler(optimizer=self.optimizer, **self.cfgs.train.scheduler)
+            if isinstance(self.cfgs.train.scheduler, partial):
+                self.lr_scheduler = self.cfgs.train.scheduler(optimizer=self.optimizer)
+            else:
+                self.lr_scheduler = get_scheduler(optimizer=self.optimizer, **self.cfgs.train.scheduler)
 
         if len(parameters_pt)>0:  # do prompt-tuning
+            cfg_opt_pt = self.cfgs.train.optimizer_pt
             if self.cfgs.train.scale_lr_pt:
                 self.scale_lr(parameters_pt)
+            if isinstance(cfg_opt_pt, partial):
+                if 'type' in cfg_opt_pt.keywords:
+                    del cfg_opt_pt.keywords['type']
+                self.optimizer_pt = cfg_opt_pt(parameters_pt, lr=self.lr)
+            else:
+                self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt_pt.weight_decay)
 
-            self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt.weight_decay_pt)
-            self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
+            if isinstance(self.cfgs.train.scheduler_pt, partial):
+                self.lr_scheduler_pt = self.cfgs.train.scheduler_pt(optimizer=self.optimizer_pt)
+            else:
+                self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
 
     def train(self):
         total_batch_size = sum(self.batch_size_list)*self.world_size*self.cfgs.train.gradient_accumulation_steps
 
         self.loggers.info("***** Running training *****")
         self.loggers.info(f"  Num batches each epoch = {len(self.train_loader_group.loader_list[0])}")
-        self.loggers.info(f"  Num Steps = {self.cfgs.train.scheduler.num_training_steps}")
+        self.loggers.info(f"  Num Steps = {self.cfgs.train.train_steps}")
         self.loggers.info(f"  Instantaneous batch size per device = {sum(self.batch_size_list)}")
         self.loggers.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_batch_size}")
         self.loggers.info(f"  Gradient Accumulation steps = {self.cfgs.train.gradient_accumulation_steps}")
         self.global_step = 0
         if self.cfgs.train.resume is not None:
             self.global_step = self.cfgs.train.resume.start_step
 
@@ -376,21 +393,21 @@
             if self.is_local_main_process:
                 if self.global_step%self.cfgs.train.save_step == 0:
                     self.save_model()
                 if self.global_step%self.min_log_step == 0:
                     lr_model = self.lr_scheduler.get_last_lr()[0] if hasattr(self, 'lr_scheduler') else 0.
                     lr_word = self.lr_scheduler_pt.get_last_lr()[0] if hasattr(self, 'lr_scheduler_pt') else 0.
                     self.loggers.log(datas={
-                        'Step':{'format':'[{}/{}]', 'data':[self.global_step, self.cfgs.train.scheduler.num_training_steps]},
+                        'Step':{'format':'[{}/{}]', 'data':[self.global_step, self.cfgs.train.train_steps]},
                         'LR_model':{'format':'{:.2e}', 'data':[lr_model]},
                         'LR_word':{'format':'{:.2e}', 'data':[lr_word]},
                         'Loss':{'format':'{:.5f}', 'data':[loss_sum.mean()]},
                     }, step=self.global_step)
 
-            if self.global_step>=self.cfgs.train.scheduler.num_training_steps:
+            if self.global_step>=self.cfgs.train.train_steps:
                 break
 
         self.wait_for_everyone()
         if self.is_local_main_process:
             self.save_model()
 
     def wait_for_everyone(self):
```

### Comparing `hcpdiff-0.3.5/hcpdiff/train_ac_single.py` & `hcpdiff-0.3.6/hcpdiff/train_ac_single.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/train_colo.py` & `hcpdiff-0.3.6/hcpdiff/train_colo.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.3.6/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.3.6/hcpdiff/utils/cfg_net_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.3.6/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/utils/ema.py` & `hcpdiff-0.3.6/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.3.6/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/utils/net_utils.py` & `hcpdiff-0.3.6/hcpdiff/utils/net_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
-from typing import Optional, Union, Tuple, Dict, Callable
+from typing import Optional, Union
 
 import torch
+from diffusers.optimization import SchedulerType, TYPE_TO_SCHEDULER_FUNCTION, Optimizer
 from torch import nn
 from torch.optim import lr_scheduler
-from diffusers.optimization import SchedulerType, TYPE_TO_SCHEDULER_FUNCTION, Optimizer
 from transformers import PretrainedConfig
-from collections import OrderedDict
 
 class TEUnetWrapper(nn.Module):
     def __init__(self, unet, TE):
         super().__init__()
         self.unet = unet
         self.TE = TE
 
@@ -29,15 +28,15 @@
         return model_pred
 
 def get_scheduler(
     name: Union[str, SchedulerType],
     optimizer: Optimizer,
     num_warmup_steps: Optional[int] = None,
     num_training_steps: Optional[int] = None,
-    scheduler_kwargs = {},
+    scheduler_kwargs={},
 ):
     """
     Unified API to get any scheduler from its name.
 
     Args:
         name (`str` or `SchedulerType`):
             The name of the scheduler to use.
@@ -60,19 +59,19 @@
     if num_training_steps is None:
         raise ValueError(f"{name} requires `num_training_steps`, please provide that argument.")
 
     # All other schedulers require `num_warmup_steps`
     if num_warmup_steps is None:
         raise ValueError(f"{name} requires `num_warmup_steps`, please provide that argument.")
 
-    #One Cycle for super convergence
-    if name=='one_cycle':
+    # One Cycle for super convergence
+    if name == 'one_cycle':
         scheduler = lr_scheduler.OneCycleLR(optimizer, max_lr=[x['lr'] for x in optimizer.state_dict()['param_groups']],
-                                steps_per_epoch=num_training_steps, epochs=1,
-                                pct_start=num_warmup_steps/num_training_steps, **scheduler_kwargs)
+                                            steps_per_epoch=num_training_steps, epochs=1,
+                                            pct_start=num_warmup_steps/num_training_steps, **scheduler_kwargs)
         return scheduler
 
     name = SchedulerType(name)
     schedule_func = TYPE_TO_SCHEDULER_FUNCTION[name]
     if name == SchedulerType.CONSTANT:
         return schedule_func(optimizer, **scheduler_kwargs)
 
@@ -113,55 +112,58 @@
 def remove_all_hooks(model: nn.Module) -> None:
     for name, child in model.named_modules():
         child._forward_hooks.clear()
         child._forward_pre_hooks.clear()
         child._backward_hooks.clear()
 
 def remove_layers(model: nn.Module, layer_class):
-    named_modules = {k: v for k, v in model.named_modules()}
-    for k,v in named_modules.items():
+    named_modules = {k:v for k, v in model.named_modules()}
+    for k, v in named_modules.items():
         if isinstance(v, layer_class):
             parent, name = named_modules[k.rsplit('.', 1)]
             delattr(parent, name)
             del v
 
 def load_emb(path):
-    emb=torch.load(path, map_location='cpu')['string_to_param']['*']
+    emb = torch.load(path, map_location='cpu')['string_to_param']['*']
     emb.requires_grad_(False)
     return emb
 
-def save_emb(path, emb:torch.Tensor, replace=False):
+def save_emb(path, emb: torch.Tensor, replace=False):
     name = os.path.basename(path)
     if os.path.exists(path) and not replace:
         raise FileExistsError(f'embedding "{name}" already exist.')
-    name=name[:name.rfind('.')]
+    name = name[:name.rfind('.')]
     torch.save({'string_to_param':{'*':emb}, 'name':name}, path)
 
-
 def hook_compile(model):
     named_modules = {k:v for k, v in model.named_modules()}
 
     for name, block in named_modules.items():
         if len(block._forward_hooks)>0:
-            for hook in block._forward_hooks.values(): # 从前往后执行
+            for hook in block._forward_hooks.values():  # 从前往后执行
                 old_forward = block.forward
+
                 def new_forward(*args, **kwargs):
                     result = old_forward(*args, **kwargs)
                     hook_result = hook(block, args, result)
                     if hook_result is not None:
                         result = hook_result
                     return result
+
                 block.forward = new_forward
 
         if len(block._forward_pre_hooks)>0:
-            for hook in list(block._forward_pre_hooks.values())[::-1]: # 从前往后执行
+            for hook in list(block._forward_pre_hooks.values())[::-1]:  # 从前往后执行
                 old_forward = block.forward
+
                 def new_forward(*args, **kwargs):
                     result = hook(block, args)
                     if result is not None:
                         if not isinstance(result, tuple):
                             result = (result,)
                     else:
                         result = args
                     return old_forward(*result, **kwargs)
+
                 block.forward = new_forward
-    remove_all_hooks(model)
+    remove_all_hooks(model)
```

### Comparing `hcpdiff-0.3.5/hcpdiff/utils/utils.py` & `hcpdiff-0.3.6/hcpdiff/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/hcpdiff/visualizer.py` & `hcpdiff-0.3.6/hcpdiff/visualizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,29 +120,30 @@
             if hasattr(self.pipe.unet, 'input_feeder'):
                 for feeder in self.pipe.unet.input_feeder:
                     feeder(ex_input_dict)
 
             images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, **kwargs).images
         return images
 
-    @torch.no_grad()
-    def vis_to_dir(self, root, prompt, negative_prompt='', save_cfg=True, **kwargs):
+    def save_images(self, images, root, prompt, negative_prompt='', save_cfg=True):
         os.makedirs(root, exist_ok=True)
-        num_img_exist = max([int(x.split('-',1)[0]) for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support])+1
-
-        images = self.vis_images(prompt, negative_prompt, **kwargs)
+        num_img_exist = max([int(x.split('-', 1)[0]) for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support]) + 1
 
         for p, pn, img in zip(prompt, negative_prompt, images):
             img.save(os.path.join(root, f"{num_img_exist}-{to_validate_file(prompt[0])}.{self.cfgs.save.image_type}"), quality=self.cfgs.save.quality)
 
             if save_cfg:
                 with open(os.path.join(root, f"{num_img_exist}-info.yaml"), 'w', encoding='utf-8') as f:
                     f.write(OmegaConf.to_yaml(self.cfgs_raw))
             num_img_exist += 1
 
+    def vis_to_dir(self, root, prompt, negative_prompt='', save_cfg=True, **kwargs):
+        images = self.vis_images(prompt, negative_prompt, **kwargs)
+        self.save_images(images, root, prompt, negative_prompt, save_cfg=save_cfg)
+
     def show_latent(self, prompt, negative_prompt='', **kwargs):
         emb_n, emb_p = self.te_hook.encode_prompt_to_emb(negative_prompt + prompt).chunk(2)
         emb_p = self.te_hook.mult_attn(emb_p, self.token_ex.parse_attn_mult(prompt))
         emb_n = self.te_hook.mult_attn(emb_n, self.token_ex.parse_attn_mult(negative_prompt))
         images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, output_type='latent', **kwargs).images
 
         for img in images:
```

### Comparing `hcpdiff-0.3.5/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.3.6/hcpdiff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.3.5
+Version: 0.3.6
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -54,14 +54,16 @@
 * colossal-AI
 * xformers for unet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
 * safetensors support
 * Controlnet (support train)
 * Min-SNR loss
+* Custom optimizer (Lion, DAdaptation, pytorch-optimizer, ...)
+* Custom lr scheduler
 
 ## Install
 
 Install with pip:
 ```bash
 pip install hcpdiff
 # Start a new project and make initialization
```

### Comparing `hcpdiff-0.3.5/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.3.6/hcpdiff.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 cfgs/plugins/plugin_controlnet.yaml
 cfgs/train/train_base.yaml
 cfgs/train/tuning_base.yaml
 cfgs/train/examples/CustomDiffusion.yaml
 cfgs/train/examples/DreamArtist++.yaml
 cfgs/train/examples/DreamArtist.yaml
 cfgs/train/examples/DreamBooth.yaml
+cfgs/train/examples/Lion_optimizer.yaml
 cfgs/train/examples/TextualInversion.yaml
 cfgs/train/examples/controlnet.yaml
 cfgs/train/examples/fine-tuning.yaml
 cfgs/train/examples/locon.yaml
 cfgs/train/examples/lora_conventional.yaml
 cfgs/train/examples/min_snr.yaml
 hcpdiff/__init__.py
```

### Comparing `hcpdiff-0.3.5/prompt_tuning_template/object.txt` & `hcpdiff-0.3.6/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/prompt_tuning_template/object_caption.txt` & `hcpdiff-0.3.6/prompt_tuning_template/object_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/prompt_tuning_template/style.txt` & `hcpdiff-0.3.6/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/prompt_tuning_template/style_caption.txt` & `hcpdiff-0.3.6/prompt_tuning_template/style_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.5/setup.py` & `hcpdiff-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.3.5",
+    version="0.3.6",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

