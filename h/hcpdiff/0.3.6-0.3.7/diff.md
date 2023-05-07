# Comparing `tmp/hcpdiff-0.3.6.tar.gz` & `tmp/hcpdiff-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.3.6.tar", last modified: Sun May  7 06:04:11 2023, max compression
+gzip compressed data, was "hcpdiff-0.3.7.tar", last modified: Sun May  7 12:16:10 2023, max compression
```

## Comparing `hcpdiff-0.3.6.tar` & `hcpdiff-0.3.7.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.975398 hcpdiff-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-07 06:04:11.975398 hcpdiff-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.955398 hcpdiff-0.3.6/cfgs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.955398 hcpdiff-0.3.6/cfgs/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/change_vae.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/euler_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/img2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/img2img_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/text2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/text2img_DA++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/infer/webui_model_infer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.955398 hcpdiff-0.3.6/cfgs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/plugins/plugin_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/te_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.955398 hcpdiff-0.3.6/cfgs/train/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.959398 hcpdiff-0.3.6/cfgs/train/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/CustomDiffusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/DreamArtist++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/DreamArtist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/DreamBooth.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/Lion_optimizer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/TextualInversion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/fine-tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/locon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/lora_conventional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/examples/min_snr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/train_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/train/tuning_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/cfgs/unet_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.959398 hcpdiff-0.3.6/hcpdiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.963398 hcpdiff-0.3.6/hcpdiff/ckpt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/ckpt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/ckpt_manager/ckpt_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/ckpt_manager/ckpt_safetensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.963398 hcpdiff-0.3.6/hcpdiff/data/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/cond_pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.963398 hcpdiff-0.3.6/hcpdiff/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/cli_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.963398 hcpdiff-0.3.6/hcpdiff/loss/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loss/min_snr_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/loss/mse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.967398 hcpdiff-0.3.6/hcpdiff/models/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/cfg_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/lora_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/text_emb_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/textencoder_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/models/tokenizer_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.967398 hcpdiff-0.3.6/hcpdiff/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/convert_caption_txt2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/create_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/gen_from_ptlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/init_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/lora_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/tools/sd2diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27094 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/train_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/train_ac_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/train_colo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.971398 hcpdiff-0.3.6/hcpdiff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/caption_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/cfg_net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/colo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/img_size_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/hcpdiff/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.959398 hcpdiff-0.3.6/hcpdiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 06:04:11.000000 hcpdiff-0.3.6/hcpdiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:11.975398 hcpdiff-0.3.6/prompt_tuning_template/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/name.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/name_2pt_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/name_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/object.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/object_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/style.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/prompt_tuning_template/style_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 06:04:11.975398 hcpdiff-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-07 06:03:56.000000 hcpdiff-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.911243 hcpdiff-0.3.7/cfgs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.911243 hcpdiff-0.3.7/cfgs/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/change_vae.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/euler_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/img2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/img2img_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/text2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/text2img_DA++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/webui_model_infer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.911243 hcpdiff-0.3.7/cfgs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/plugins/plugin_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/te_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.911243 hcpdiff-0.3.7/cfgs/train/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/cfgs/train/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/CustomDiffusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/DreamArtist++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/DreamArtist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/DreamBooth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/Lion_optimizer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/TextualInversion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/fine-tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/locon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/lora_conventional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/min_snr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/train_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/tuning_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/unet_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/ckpt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/ckpt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/ckpt_manager/ckpt_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/ckpt_manager/ckpt_safetensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/cond_pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/cli_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loss/min_snr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loss/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/hcpdiff/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/cfg_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/lora_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/text_emb_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/textencoder_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/tokenizer_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/hcpdiff/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/convert_caption_txt2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/create_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/gen_from_ptlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/init_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/lora_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/sd2diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27108 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/train_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/train_ac_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/train_colo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/hcpdiff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/caption_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/cfg_net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/colo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/img_size_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/prompt_tuning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/name.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/name_2pt_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/name_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/object.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/object_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/style.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/style_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/setup.py
```

### Comparing `hcpdiff-0.3.6/LICENSE` & `hcpdiff-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/PKG-INFO` & `hcpdiff-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.3.6
+Version: 0.3.7
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.3.6/README.md` & `hcpdiff-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/infer/euler_a.yaml` & `hcpdiff-0.3.7/cfgs/infer/euler_a.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/infer/img2img.yaml` & `hcpdiff-0.3.7/cfgs/infer/img2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/infer/img2img_controlnet.yaml` & `hcpdiff-0.3.7/cfgs/infer/img2img_controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/infer/text2img.yaml` & `hcpdiff-0.3.7/cfgs/infer/text2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/infer/text2img_DA++.yaml` & `hcpdiff-0.3.7/cfgs/infer/text2img_DA++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/infer/webui_model_infer.yaml` & `hcpdiff-0.3.7/cfgs/infer/webui_model_infer.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/te_struct.txt` & `hcpdiff-0.3.7/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/DreamArtist++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/controlnet.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/locon.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/locon.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.3.7/cfgs/train/examples/lora_conventional.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/train_base.yaml` & `hcpdiff-0.3.7/cfgs/train/train_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/train/tuning_base.yaml` & `hcpdiff-0.3.7/cfgs/train/tuning_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/cfgs/unet_struct.txt` & `hcpdiff-0.3.7/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.3.7/hcpdiff/ckpt_manager/ckpt_pkl.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.3.7/hcpdiff/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/data/__init__.py` & `hcpdiff-0.3.7/hcpdiff/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/data/bucket.py` & `hcpdiff-0.3.7/hcpdiff/data/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         rs = np.random.RandomState(42 + epoch)
         bucket_list = [x.copy() for x in self.buckets]
         # shuffle inter bucket
         for x in bucket_list:
             rs.shuffle(x)
 
         # shuffle of batches
-        bucket_list = np.hstack(bucket_list).reshape(-1, self.bs)
+        bucket_list = np.hstack(bucket_list).reshape(-1, self.bs).astype(int)
         rs.shuffle(bucket_list)
 
         self.idx_arb = bucket_list.reshape(-1)
 
     def crop_resize(self, image, size):
         return resize_crop_fix(image, size)
```

### Comparing `hcpdiff-0.3.6/hcpdiff/data/cond_pair_dataset.py` & `hcpdiff-0.3.7/hcpdiff/data/cond_pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.3.7/hcpdiff/data/pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/data/utils.py` & `hcpdiff-0.3.7/hcpdiff/data/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/loggers/base_logger.py` & `hcpdiff-0.3.7/hcpdiff/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/loggers/cli_logger.py` & `hcpdiff-0.3.7/hcpdiff/loggers/cli_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/loggers/tensorboard_logger.py` & `hcpdiff-0.3.7/hcpdiff/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/loggers/wandb_logger.py` & `hcpdiff-0.3.7/hcpdiff/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/loss/min_snr_loss.py` & `hcpdiff-0.3.7/hcpdiff/loss/min_snr_loss.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/cfg_context.py` & `hcpdiff-0.3.7/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/controlnet.py` & `hcpdiff-0.3.7/hcpdiff/models/controlnet.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/layers.py` & `hcpdiff-0.3.7/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/lora_base.py` & `hcpdiff-0.3.7/hcpdiff/models/lora_base.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/lora_layers.py` & `hcpdiff-0.3.7/hcpdiff/models/lora_layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/plugin.py` & `hcpdiff-0.3.7/hcpdiff/models/plugin.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.3.7/hcpdiff/models/text_emb_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.3.7/hcpdiff/models/textencoder_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.3.7/hcpdiff/models/tokenizer_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.3.7/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 import json
 import os
 
 from hcpdiff.utils.img_size_tool import types_support
 
 parser = argparse.ArgumentParser(description='Stable Diffusion Training')
 parser.add_argument('--data_root', type=str, default='')
+parser.add_argument('--with_imgs', action="store_true")
 args = parser.parse_args()
 
 
 def get_txt_caption(path):
     with open(path, encoding='utf8') as f:
         return f.read().strip()
 
 
 captions = {}
 for file in os.listdir(args.data_root):
-    ext_idx = file.rfind('.')
-    file_name = file[:ext_idx]
-    if file[ext_idx + 1:] in types_support:
-        captions[file] = get_txt_caption(os.path.join(args.data_root, f'{file_name}.txt'))
+    file_name, file_ext = file.rsplit('.', 1)
+    if args.with_imgs:
+        if file_ext in types_support:
+            captions[file] = get_txt_caption(os.path.join(args.data_root, f'{file_name}.txt'))
+    else:
+        if file_ext == 'txt':
+            captions[file] = get_txt_caption(os.path.join(args.data_root, f'{file_name}.txt'))
 
 with open(os.path.join(args.data_root, f'image_captions.json'), "w", encoding='utf8') as f:
     json.dump(captions, f, indent=2, ensure_ascii=False)
```

### Comparing `hcpdiff-0.3.6/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.3.7/hcpdiff/tools/create_embedding.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.3.7/hcpdiff/tools/gen_from_ptlist.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/tools/init_proj.py` & `hcpdiff-0.3.7/hcpdiff/tools/init_proj.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/tools/lora_convert.py` & `hcpdiff-0.3.7/hcpdiff/tools/lora_convert.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/tools/sd2diffusers.py` & `hcpdiff-0.3.7/hcpdiff/tools/sd2diffusers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/train_ac.py` & `hcpdiff-0.3.7/hcpdiff/train_ac.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
             cfg_opt = self.cfgs.train.optimizer
             if self.cfgs.train.scale_lr:
                 self.scale_lr(parameters)
 
             if isinstance(cfg_opt, partial):
                 if 'type' in cfg_opt.keywords:
                     del cfg_opt.keywords['type']
-                self.optimizer = cfg_opt(parameters, lr=self.lr)
+                self.optimizer = cfg_opt(params=parameters, lr=self.lr)
             elif cfg_opt.type == 'adamw_8bit':
                 import bitsandbytes as bnb
                 self.optimizer = bnb.optim.AdamW8bit(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
             elif cfg_opt.type == 'deepspeed' and self.accelerator.state.deepspeed_plugin is not None:
                 from deepspeed.ops.adam import FusedAdam
                 self.optimizer = FusedAdam(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
             elif cfg_opt.type == 'adamw':
@@ -358,15 +358,15 @@
         if len(parameters_pt)>0:  # do prompt-tuning
             cfg_opt_pt = self.cfgs.train.optimizer_pt
             if self.cfgs.train.scale_lr_pt:
                 self.scale_lr(parameters_pt)
             if isinstance(cfg_opt_pt, partial):
                 if 'type' in cfg_opt_pt.keywords:
                     del cfg_opt_pt.keywords['type']
-                self.optimizer_pt = cfg_opt_pt(parameters_pt, lr=self.lr)
+                self.optimizer_pt = cfg_opt_pt(params=parameters_pt, lr=self.lr)
             else:
                 self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt_pt.weight_decay)
 
             if isinstance(self.cfgs.train.scheduler_pt, partial):
                 self.lr_scheduler_pt = self.cfgs.train.scheduler_pt(optimizer=self.optimizer_pt)
             else:
                 self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
```

### Comparing `hcpdiff-0.3.6/hcpdiff/train_ac_single.py` & `hcpdiff-0.3.7/hcpdiff/train_ac_single.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/train_colo.py` & `hcpdiff-0.3.7/hcpdiff/train_colo.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.3.7/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.3.7/hcpdiff/utils/cfg_net_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.3.7/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/utils/ema.py` & `hcpdiff-0.3.7/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.3.7/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/utils/net_utils.py` & `hcpdiff-0.3.7/hcpdiff/utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/utils/utils.py` & `hcpdiff-0.3.7/hcpdiff/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff/visualizer.py` & `hcpdiff-0.3.7/hcpdiff/visualizer.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.3.7/hcpdiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.3.6
+Version: 0.3.7
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.3.6/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.3.7/hcpdiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/prompt_tuning_template/object.txt` & `hcpdiff-0.3.7/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/prompt_tuning_template/object_caption.txt` & `hcpdiff-0.3.7/prompt_tuning_template/object_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/prompt_tuning_template/style.txt` & `hcpdiff-0.3.7/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/prompt_tuning_template/style_caption.txt` & `hcpdiff-0.3.7/prompt_tuning_template/style_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.6/setup.py` & `hcpdiff-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.3.6",
+    version="0.3.7",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

