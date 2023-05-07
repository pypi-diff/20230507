# Comparing `tmp/uss-0.0.3.tar.gz` & `tmp/uss-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uss-0.0.3.tar", last modified: Sat May  6 14:04:00 2023, max compression
+gzip compressed data, was "uss-0.0.4.tar", last modified: Sun May  7 06:44:35 2023, max compression
```

## Comparing `uss-0.0.3.tar` & `uss-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-06 14:04:00.785710 uss-0.0.3/
--rw-r--r--   0 tiger     (1000) tiger     (1000)      550 2023-05-04 01:50:02.000000 uss-0.0.3/LICENSE
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-04-24 22:07:00.000000 uss-0.0.3/MANIFEST.in
--rw-r--r--   0 tiger     (1000) tiger     (1000)      284 2023-05-06 14:04:00.785710 uss-0.0.3/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     5825 2023-05-06 13:57:34.000000 uss-0.0.3/README.md
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-06 14:04:00.785710 uss-0.0.3/setup.cfg
--rw-r--r--   0 tiger     (1000) tiger     (1000)      735 2023-05-06 14:03:47.000000 uss-0.0.3/setup.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-06 14:04:00.782710 uss-0.0.3/uss/
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 05:43:32.000000 uss-0.0.3/uss/__init__.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-06 14:04:00.783710 uss-0.0.3/uss/callbacks/
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 02:58:55.000000 uss-0.0.3/uss/callbacks/__init__.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     1062 2023-05-06 07:15:41.000000 uss-0.0.3/uss/callbacks/base.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3484 2023-05-06 13:57:34.000000 uss-0.0.3/uss/callbacks/evaluate.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     1922 2023-05-06 13:57:34.000000 uss-0.0.3/uss/config.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-06 14:04:00.784710 uss-0.0.3/uss/data/
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 03:01:44.000000 uss-0.0.3/uss/data/__init__.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     7896 2023-05-06 13:57:34.000000 uss-0.0.3/uss/data/anchor_segment_detectors.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2663 2023-05-06 13:57:34.000000 uss-0.0.3/uss/data/anchor_segment_mixers.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2855 2023-05-06 13:57:34.000000 uss-0.0.3/uss/data/datamodules.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     1876 2023-05-06 13:57:34.000000 uss-0.0.3/uss/data/datasets.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     5898 2023-05-06 13:57:34.000000 uss-0.0.3/uss/data/samplers.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-06 14:04:00.784710 uss-0.0.3/uss/dataset_creation/
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 08:36:22.000000 uss-0.0.3/uss/dataset_creation/__init__.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     9953 2023-05-06 13:57:34.000000 uss-0.0.3/uss/dataset_creation/create_audioset_evaluation_meta.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     6022 2023-05-06 13:57:34.000000 uss-0.0.3/uss/evaluate.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)    23903 2023-05-06 13:57:34.000000 uss-0.0.3/uss/inference.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2295 2023-05-06 07:15:41.000000 uss-0.0.3/uss/losses.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-06 14:04:00.784710 uss-0.0.3/uss/models/
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 03:03:20.000000 uss-0.0.3/uss/models/__init__.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     4855 2023-05-06 13:57:34.000000 uss-0.0.3/uss/models/base.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     4263 2023-05-06 13:57:34.000000 uss-0.0.3/uss/models/film.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     4937 2023-05-06 13:57:34.000000 uss-0.0.3/uss/models/pl_modules.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     9039 2023-05-06 13:57:34.000000 uss-0.0.3/uss/models/query_nets.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)    18238 2023-05-06 13:57:34.000000 uss-0.0.3/uss/models/resunet.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-06 14:04:00.785710 uss-0.0.3/uss/optimizers/
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 03:04:05.000000 uss-0.0.3/uss/optimizers/__init__.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2498 2023-05-06 13:57:34.000000 uss-0.0.3/uss/optimizers/lr_schedulers.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2934 2023-05-06 13:57:34.000000 uss-0.0.3/uss/parse_ontology.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)    10445 2023-05-06 13:57:34.000000 uss-0.0.3/uss/train.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     1977 2023-05-06 13:57:34.000000 uss-0.0.3/uss/uss_inference.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     6234 2023-05-06 13:57:34.000000 uss-0.0.3/uss/utils.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-06 14:04:00.782710 uss-0.0.3/uss.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)      284 2023-05-06 14:04:00.000000 uss-0.0.3/uss.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)      861 2023-05-06 14:04:00.000000 uss-0.0.3/uss.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-06 14:04:00.000000 uss-0.0.3/uss.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       47 2023-05-06 14:04:00.000000 uss-0.0.3/uss.egg-info/entry_points.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)      119 2023-05-06 14:04:00.000000 uss-0.0.3/uss.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        4 2023-05-06 14:04:00.000000 uss-0.0.3/uss.egg-info/top_level.txt
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-07 06:44:35.649615 uss-0.0.4/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      550 2023-05-04 01:50:02.000000 uss-0.0.4/LICENSE
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-04-24 22:07:00.000000 uss-0.0.4/MANIFEST.in
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      284 2023-05-07 06:44:35.648615 uss-0.0.4/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     6421 2023-05-07 06:42:45.000000 uss-0.0.4/README.md
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-07 06:44:35.649615 uss-0.0.4/setup.cfg
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      735 2023-05-07 06:41:42.000000 uss-0.0.4/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-07 06:44:35.645615 uss-0.0.4/uss/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 05:43:32.000000 uss-0.0.4/uss/__init__.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-07 06:44:35.646615 uss-0.0.4/uss/callbacks/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 02:58:55.000000 uss-0.0.4/uss/callbacks/__init__.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     1062 2023-05-06 07:15:41.000000 uss-0.0.4/uss/callbacks/base.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3484 2023-05-06 13:57:34.000000 uss-0.0.4/uss/callbacks/evaluate.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     1922 2023-05-06 13:57:34.000000 uss-0.0.4/uss/config.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-07 06:44:35.647616 uss-0.0.4/uss/data/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 03:01:44.000000 uss-0.0.4/uss/data/__init__.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     7896 2023-05-06 13:57:34.000000 uss-0.0.4/uss/data/anchor_segment_detectors.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2663 2023-05-06 13:57:34.000000 uss-0.0.4/uss/data/anchor_segment_mixers.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2855 2023-05-06 13:57:34.000000 uss-0.0.4/uss/data/datamodules.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     1876 2023-05-06 13:57:34.000000 uss-0.0.4/uss/data/datasets.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     5898 2023-05-06 13:57:34.000000 uss-0.0.4/uss/data/samplers.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-07 06:44:35.647616 uss-0.0.4/uss/dataset_creation/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 08:36:22.000000 uss-0.0.4/uss/dataset_creation/__init__.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     9953 2023-05-06 13:57:34.000000 uss-0.0.4/uss/dataset_creation/create_audioset_evaluation_meta.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     6022 2023-05-06 13:57:34.000000 uss-0.0.4/uss/evaluate.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)    23903 2023-05-06 13:57:34.000000 uss-0.0.4/uss/inference.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2295 2023-05-06 07:15:41.000000 uss-0.0.4/uss/losses.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-07 06:44:35.648615 uss-0.0.4/uss/models/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 03:03:20.000000 uss-0.0.4/uss/models/__init__.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     4855 2023-05-06 13:57:34.000000 uss-0.0.4/uss/models/base.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     4263 2023-05-06 13:57:34.000000 uss-0.0.4/uss/models/film.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     4937 2023-05-06 13:57:34.000000 uss-0.0.4/uss/models/pl_modules.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     9039 2023-05-06 13:57:34.000000 uss-0.0.4/uss/models/query_nets.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)    18238 2023-05-06 13:57:34.000000 uss-0.0.4/uss/models/resunet.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-07 06:44:35.648615 uss-0.0.4/uss/optimizers/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-06 03:04:05.000000 uss-0.0.4/uss/optimizers/__init__.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2498 2023-05-06 13:57:34.000000 uss-0.0.4/uss/optimizers/lr_schedulers.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2934 2023-05-06 13:57:34.000000 uss-0.0.4/uss/parse_ontology.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)    10445 2023-05-06 13:57:34.000000 uss-0.0.4/uss/train.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2038 2023-05-07 06:41:57.000000 uss-0.0.4/uss/uss_inference.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     6234 2023-05-06 13:57:34.000000 uss-0.0.4/uss/utils.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-07 06:44:35.646615 uss-0.0.4/uss.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      284 2023-05-07 06:44:35.000000 uss-0.0.4/uss.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      861 2023-05-07 06:44:35.000000 uss-0.0.4/uss.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-07 06:44:35.000000 uss-0.0.4/uss.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       47 2023-05-07 06:44:35.000000 uss-0.0.4/uss.egg-info/entry_points.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      119 2023-05-07 06:44:35.000000 uss-0.0.4/uss.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        4 2023-05-07 06:44:35.000000 uss-0.0.4/uss.egg-info/top_level.txt
```

### Comparing `uss-0.0.3/LICENSE` & `uss-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/README.md` & `uss-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 # Universal Source Separation (USS) with Weakly labelled Data
 
-This is the PyTorch implementation of the Universal Source Separation with Weakly labelled Data [1]. The USS system can automatically detect and separate sound classes from a real recording. The USS system can separate up to hundreds of sound classes sound classes in a hierarchical ontology structure. The USS system is trained on the weakly labelled AudioSet dataset only.
+This is the PyTorch implementation of the Universal Source Separation with Weakly labelled Data [1]. The USS system can automatically detect and separate sound classes from a real recording. The USS system can separate up to hundreds of sound classes sound classes in a hierarchical ontology structure. The USS system is trained on the weakly labelled AudioSet dataset only. Here is a demo:
+
+![alt text](resources/harry_potter.jpg)
+Fig. The hierarchical separation result of the trailer of *Harry Potter and the Sorcerer's Stone*. Copyright: [https://www.youtube.com/watch?v=VyHV0BRtdxo](https://www.youtube.com/watch?v=VyHV0BRtdxo)
 
 ## 1. Installation
+
+Prepare environment (optional)
+```bash
+conda create -n uss python=3.8
+conda activate uss
+```
+
+Install the package
 ```bash
 pip install uss
 ```
 
 ## 2. Separate Your Favorite Audio
 
 ### 2.1 Download test audio (optional)
 ```bash
-wget -O "harry_potter.flac" "https://sandbox.zenodo.org/record/1196562/files/harry_potter.flac?download=1"
+wget -O "harry_potter.flac" "https://huggingface.co/RSNuts/Universal_Source_Separation/resolve/main/uss_material/harry_potter.flac"
 ```
 
-### 2.2 Default: automatic detect and separate
+### 2.2 Detect and separate sound classes in hierarchical levels (default)
 ```bash
 uss -i "harry_potter.flac"
 ```
 
-### 2.3 Separate with different AudioSet hierarchy levels (The same as default)
+### 2.3 The same as default
 ```bash
 uss -i "harry_potter.flac" --levels 1 2 3
 ```
 
 ### 2.4 Separate by class IDs
 ```bash
 uss -i "harry_potter.flac" --class_ids 0 1 2 3 4
 ```
 
 ### 2.5 Separate by queries
 
 Download query audios (optional)
 
 ```bash
-wget -O "queries.zip" "https://sandbox.zenodo.org/record/1196562/files/queries.zip?download=1"
+wget -O "queries.zip" "https://huggingface.co/RSNuts/Universal_Source_Separation/resolve/main/uss_material/queries.zip"
 unzip queries.zip
 ```
 
 Do separation 
 
 ```bash
 uss -i "harry_potter.flac" --queries_dir "queries/speech"
@@ -54,20 +65,28 @@
 conda create -n uss python=3.8
 conda activate uss
 pip install -r requirements.txt
 ```
 
 ### 3.2 Inference
 
+Download our pretrained checkpoint: 
+
+```bash
+wget -O "pretrained.ckpt" "https://huggingface.co/RSNuts/Universal_Source_Separation/resolve/main/uss_material/ss_model%3Dresunet30%2Cquerynet%3Dat_soft%2Cdata%3Dfull%2Cdevices%3D8%2Cstep%3D1000000.ckpt"
+```
+
+Then perform the inference:
+
 ```python
 CUDA_VISIBLE_DEVICES=0 python3 uss/inference.py \
     --audio_path=./resources/harry_potter.flac \
     --levels 1 2 3 \
     --config_yaml="./scripts/train/ss_model=resunet30,querynet=at_soft,data=full.yaml" \
-    --checkpoint_path="${HOME}/.cache/uss/checkpoints/ss_model=resunet30,querynet=at_soft,data=full,devices=8,step=100000.ckpt"
+    --checkpoint_path="pretrained.ckpt"
 ```
 
 ## 4. Train the USS system from scratch
 
 ### 4.0 Download dataset
 
 Download the AudioSet dataset from the internet. The total size of AudioSet is around 1.1 TB. For reproducibility, our downloaded dataset can be accessed at: link: [https://pan.baidu.com/s/13WnzI1XDSvqXZQTS-Kqujg](https://pan.baidu.com/s/13WnzI1XDSvqXZQTS-Kqujg), password: 0vc2. Users may only download the balanced set (10.36 Gb, 1% of the full set) to train a baseline system.
@@ -186,8 +205,8 @@
 CUDA_VISIBLE_DEVICES=0 python3 uss/train.py \
     --workspace=$WORKSPACE \
     --config_yaml="./scripts/train/ss_model=resunet30,querynet=at_soft,data=balanced.yaml"
 ```
 
 ## Reference
 
-To appear
+To appear
```

### Comparing `uss-0.0.3/setup.py` & `uss-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 
 setup(
     name='uss',
-    version='0.0.3',
+    version='0.0.4',
     description='Universal source separation (USS) with weakly labelled data.',
     author='Qiuqiang Kong',
     author_email='qiuqiangkong@gmail.com',
     license='Apache2.0',
     packages=find_packages(),
     url="https://github.com/bytedance/uss",
     include_package_data=True,
```

### Comparing `uss-0.0.3/uss/callbacks/base.py` & `uss-0.0.4/uss/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/callbacks/evaluate.py` & `uss-0.0.4/uss/callbacks/evaluate.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/config.py` & `uss-0.0.4/uss/config.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/data/anchor_segment_detectors.py` & `uss-0.0.4/uss/data/anchor_segment_detectors.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/data/anchor_segment_mixers.py` & `uss-0.0.4/uss/data/anchor_segment_mixers.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/data/datamodules.py` & `uss-0.0.4/uss/data/datamodules.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/data/datasets.py` & `uss-0.0.4/uss/data/datasets.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/data/samplers.py` & `uss-0.0.4/uss/data/samplers.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/dataset_creation/create_audioset_evaluation_meta.py` & `uss-0.0.4/uss/dataset_creation/create_audioset_evaluation_meta.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/evaluate.py` & `uss-0.0.4/uss/evaluate.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/inference.py` & `uss-0.0.4/uss/inference.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/losses.py` & `uss-0.0.4/uss/losses.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/models/base.py` & `uss-0.0.4/uss/models/base.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/models/film.py` & `uss-0.0.4/uss/models/film.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/models/pl_modules.py` & `uss-0.0.4/uss/models/pl_modules.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/models/query_nets.py` & `uss-0.0.4/uss/models/query_nets.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/models/resunet.py` & `uss-0.0.4/uss/models/resunet.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/optimizers/lr_schedulers.py` & `uss-0.0.4/uss/optimizers/lr_schedulers.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/parse_ontology.py` & `uss-0.0.4/uss/parse_ontology.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/train.py` & `uss-0.0.4/uss/train.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss/uss_inference.py` & `uss-0.0.4/uss/uss_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from uss.inference import separate
 from uss.utils import get_path
 
 model_paths_dict = {
     "at_soft": {
         "config_yaml": {
             "path": Path(Path.home(), ".cache/uss/scripts/ss_model=resunet30,querynet=at_soft,data=full.yaml"),
-            "remote_path": "https://sandbox.zenodo.org/record/1196562/files/ss_model%3Dresunet30%2Cquerynet%3Dat_soft%2Cdata%3Dfull.yaml?download=1",
+            "remote_path": "https://huggingface.co/RSNuts/Universal_Source_Separation/resolve/main/uss_material/ss_model%3Dresunet30%2Cquerynet%3Dat_soft%2Cdata%3Dfull.yaml?download=1",
             "size": 1558,
         },
         "checkpoint": {
             "path": Path(Path.home(), ".cache/uss/checkpoints/ss_model=resunet30,querynet=at_soft,data=full,devices=8,step=1000000.ckpt"),
-            "remote_path": "https://sandbox.zenodo.org/record/1196562/files/ss_model%3Dresunet30%2Cquerynet%3Dat_soft%2Cdata%3Dfull%2Cdevices%3D8%2Cstep%3D1000000.ckpt?download=1",
+            "remote_path": "https://huggingface.co/RSNuts/Universal_Source_Separation/resolve/main/uss_material/ss_model%3Dresunet30%2Cquerynet%3Dat_soft%2Cdata%3Dfull%2Cdevices%3D8%2Cstep%3D1000000.ckpt",
             "size": 1121024828,
         },
     }
 }
 
 
 def main():
```

### Comparing `uss-0.0.3/uss/utils.py` & `uss-0.0.4/uss/utils.py`

 * *Files identical despite different names*

### Comparing `uss-0.0.3/uss.egg-info/SOURCES.txt` & `uss-0.0.4/uss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

