# Comparing `tmp/instruction_ner-0.1.3.tar.gz` & `tmp/instruction_ner-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instruction_ner-0.1.3.tar", last modified: Tue Aug 30 18:57:46 2022, max compression
+gzip compressed data, was "instruction_ner-0.1.6.tar", last modified: Sun May  7 16:30:56 2023, max compression
```

## Comparing `instruction_ner-0.1.3.tar` & `instruction_ner-0.1.6.tar`

### file list

```diff
@@ -1,46 +1,53 @@
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.843344 instruction_ner-0.1.3/
--rw-r--r--   0 a18692338   (503) staff       (20)     1070 2022-06-30 19:45:07.000000 instruction_ner-0.1.3/LICENSE
--rw-r--r--   0 a18692338   (503) staff       (20)     7446 2022-08-30 18:57:46.844481 instruction_ner-0.1.3/PKG-INFO
--rw-r--r--   0 a18692338   (503) staff       (20)     5499 2022-08-30 18:17:32.000000 instruction_ner-0.1.3/README.md
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.816715 instruction_ner-0.1.3/instruction_ner/
--rw-r--r--   0 a18692338   (503) staff       (20)       22 2022-08-30 18:57:25.000000 instruction_ner-0.1.3/instruction_ner/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     3096 2022-08-20 11:34:42.000000 instruction_ner-0.1.3/instruction_ner/arg_parse.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1294 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/collator.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.822660 instruction_ner-0.1.3/instruction_ner/core/
--rw-r--r--   0 a18692338   (503) staff       (20)        0 2022-07-01 18:48:22.000000 instruction_ner-0.1.3/instruction_ner/core/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1914 2022-08-18 17:17:06.000000 instruction_ner-0.1.3/instruction_ner/core/datatypes.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1981 2022-07-24 14:04:16.000000 instruction_ner-0.1.3/instruction_ner/core/reader.py
--rw-r--r--   0 a18692338   (503) staff       (20)     3636 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/dataset.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1937 2022-08-21 16:44:42.000000 instruction_ner-0.1.3/instruction_ner/evaluate.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.827373 instruction_ner-0.1.3/instruction_ner/formatters/
--rw-r--r--   0 a18692338   (503) staff       (20)     1950 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/formatters/Answer.py
--rw-r--r--   0 a18692338   (503) staff       (20)     2630 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/formatters/PredictionSpan.py
--rw-r--r--   0 a18692338   (503) staff       (20)      470 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/formatters/__init__.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.832327 instruction_ner-0.1.3/instruction_ner/formatters/instances/
--rw-r--r--   0 a18692338   (503) staff       (20)     1267 2022-07-18 19:06:01.000000 instruction_ner-0.1.3/instruction_ner/formatters/instances/EntityExtractTask.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1487 2022-07-18 19:06:01.000000 instruction_ner-0.1.3/instruction_ner/formatters/instances/EntityTypeTask.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1236 2022-07-18 19:06:01.000000 instruction_ner-0.1.3/instruction_ner/formatters/instances/NERTask.py
--rw-r--r--   0 a18692338   (503) staff       (20)      978 2022-07-18 19:05:34.000000 instruction_ner-0.1.3/instruction_ner/formatters/instances/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     8292 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/metrics.py
--rw-r--r--   0 a18692338   (503) staff       (20)     2287 2022-08-18 18:58:38.000000 instruction_ner-0.1.3/instruction_ner/model.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1219 2022-08-30 18:26:30.000000 instruction_ner-0.1.3/instruction_ner/prepare_data.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.837315 instruction_ner-0.1.3/instruction_ner/readers/
--rw-r--r--   0 a18692338   (503) staff       (20)      228 2022-08-06 12:26:30.000000 instruction_ner-0.1.3/instruction_ner/readers/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     6696 2022-08-20 11:34:42.000000 instruction_ner-0.1.3/instruction_ner/readers/conll.py
--rw-r--r--   0 a18692338   (503) staff       (20)     5375 2022-08-06 12:26:30.000000 instruction_ner-0.1.3/instruction_ner/readers/mit.py
--rw-r--r--   0 a18692338   (503) staff       (20)     3685 2022-07-24 14:04:16.000000 instruction_ner-0.1.3/instruction_ner/readers/spacy.py
--rw-r--r--   0 a18692338   (503) staff       (20)     4331 2022-08-21 16:44:42.000000 instruction_ner-0.1.3/instruction_ner/train.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.841215 instruction_ner-0.1.3/instruction_ner/utils/
--rw-r--r--   0 a18692338   (503) staff       (20)        0 2022-08-30 18:12:23.000000 instruction_ner-0.1.3/instruction_ner/utils/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     6046 2022-08-20 11:34:42.000000 instruction_ner-0.1.3/instruction_ner/utils/evaluate_utils.py
--rw-r--r--   0 a18692338   (503) staff       (20)     6259 2022-08-30 18:31:20.000000 instruction_ner-0.1.3/instruction_ner/utils/train_utils.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1773 2022-08-20 11:34:42.000000 instruction_ner-0.1.3/instruction_ner/utils/utils.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.820223 instruction_ner-0.1.3/instruction_ner.egg-info/
--rw-r--r--   0 a18692338   (503) staff       (20)     7446 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/PKG-INFO
--rw-r--r--   0 a18692338   (503) staff       (20)     1225 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/SOURCES.txt
--rw-r--r--   0 a18692338   (503) staff       (20)        1 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/dependency_links.txt
--rw-r--r--   0 a18692338   (503) staff       (20)      192 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/entry_points.txt
--rw-r--r--   0 a18692338   (503) staff       (20)      155 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/requires.txt
--rw-r--r--   0 a18692338   (503) staff       (20)       16 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/top_level.txt
--rw-r--r--   0 a18692338   (503) staff       (20)      131 2022-08-30 18:57:46.845394 instruction_ner-0.1.3/setup.cfg
--rw-r--r--   0 a18692338   (503) staff       (20)     1426 2022-08-30 18:56:26.000000 instruction_ner-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.599767 instruction_ner-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-07 16:30:56.599767 instruction_ner-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.587767 instruction_ner-0.1.6/instruction_ner/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/arg_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.591767 instruction_ner-0.1.6/instruction_ner/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/core/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.591767 instruction_ner-0.1.6/instruction_ner/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/formatters/Answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/formatters/PredictionSpan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/formatters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.595767 instruction_ner-0.1.6/instruction_ner/formatters/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/formatters/instances/EntityExtractTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/formatters/instances/EntityTypeTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/formatters/instances/NERTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/formatters/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/prepare_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.595767 instruction_ner-0.1.6/instruction_ner/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/readers/conll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/readers/mit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/readers/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.595767 instruction_ner-0.1.6/instruction_ner/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/utils/evaluate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/utils/train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/instruction_ner/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.591767 instruction_ner-0.1.6/instruction_ner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-07 16:30:56.000000 instruction_ner-0.1.6/instruction_ner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-07 16:30:56.000000 instruction_ner-0.1.6/instruction_ner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:30:56.000000 instruction_ner-0.1.6/instruction_ner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-07 16:30:56.000000 instruction_ner-0.1.6/instruction_ner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-07 16:30:56.000000 instruction_ner-0.1.6/instruction_ner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 16:30:56.000000 instruction_ner-0.1.6/instruction_ner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-07 16:30:56.599767 instruction_ner-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:30:56.599767 instruction_ner-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/tests/test_PredictionSpan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-07 16:30:43.000000 instruction_ner-0.1.6/tests/test_readers.py
```

### Comparing `instruction_ner-0.1.3/LICENSE` & `instruction_ner-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.3/PKG-INFO` & `instruction_ner-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,190 +1,193 @@
 Metadata-Version: 2.1
 Name: instruction_ner
-Version: 0.1.3
+Version: 0.1.6
 Summary: Unofficial implementation of InstructionNER
 Home-page: https://github.com/ovbystrova/InstructionNER
 Author: Olga Bystrova
 Author-email: bystrovaolgavl@gmail.com
-License: UNKNOWN
-Description: # InstructionNER: A Multi-Task Instruction-Based Generative Framework for Few-shot NER
-        
-        [![tests](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml/badge.svg)](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml)
-        [![codecov](https://codecov.io/gh/ovbystrova/InstructionNER/branch/main/graph/badge.svg?token=L2OOZKLPJL)](https://codecov.io/gh/ovbystrova/InstructionNER)
-        [![python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/ovbystrova/InstructionNER#requirements)
-        [![license](https://img.shields.io/github/license/ovbystrova/InstructionNER?color=blue)](https://github.com/ovbystrova/InstructionNER/blob/main/LICENSE)
-        
-        Unofficial implementation of [InstructionNER](https://arxiv.org/pdf/2203.03903v1.pdf).
-        
-        ![Screenshot](resources/overall_intro.jpg)
-        
-        ## Requirements
-        Python >=3.8
-        
-        ## Installation
-        ```shell
-        pip install instruction-ner
-        ```
-        
-        (Alternative via requirements)
-        ```shell
-        pip install -r requirements/requirements.in # for training purposes
-        pip install -r requirements/requirements_test.in # for tests
-        pip install -r requirements/requirements_dev.in # for inference only
-        ```
-        
-        ## Data Preparation
-        In order to make a unified training interface, 
-        you can convert your raw input data (supported dataset formats: **conll**, **spacy**, **mit**)
-        with the following script:
-        ```
-        instruction_ner-prepare-data \
-        --path_to_file 'data/conll2003/train.txt' \
-        --dataset_type 'conll2003' \
-        --output_folder 'data/conll2003' \
-        ```
-        
-        This script converts every dataset to a list of sentences.
-        Every sentence is like this:
-        ```
-        {
-            "context": "SOCCER - JAPAN GET LUCKY WIN , CHINA IN SURPRISE DEFEAT .",
-            "entity_values": {
-                    "LOC": [
-                        "JAPAN"
-                    ],
-                    "PER": [
-                        "CHINA"
-                    ]
-                },
-            "entity_spans": [
-                    {
-                        "start": 9,
-                        "end": 14,
-                        "label": "LOC"
-                    },
-                    {
-                        "start": 31,
-                        "end": 36,
-                        "label": "PER"
-                    }
-                ]
-        }
-        ```
-        
-        ## Training
-        Script for training T5 model:
-        ```
-        instruction_ner-train \
-        --path_to_instructions 'instructions.json' \
-        --path_to_options 'options.json' \
-        --log_dir 'runs/test_run' \
-        --eval_every_n_batches 200 \
-        --pred_every_n_batches 200 \
-        --path_to_model_config 'config.yaml' \
-        --path_to_model_save 'runs/model/' \
-        ```
-        
-        Arguments:
-        - **--path_to_instructions** - file with instruction prompts
-        - **--path_to_options** - file with mapping dataset to its entities
-        - **--log_dir** - where to log tensorboard
-        - **--eval_every_n_batches** - do evaluation every n batches
-        - **--pred_every_n_batches** - write n sample prediction every n batches
-        - **--path_to_model_config** - path to all necessary information for model
-        - **--path_to_model_save** - where to save model
-        
-        ## Evaluation
-        Script for evaluation of the trained model:
-        ```
-        instruction_ner-evaluate \
-        --model_path_or_name 'olgaduchovny/t5-base-qa-ner-conll' \
-        --path_to_model_config 'config.yaml' \
-        --path_to_instructions 'instructions.json' \
-        --path_to_options 'options.json' \
-        ```
-        
-        Arguments:
-        - **--model_path_or_name** - path to trained model or HF model name
-        - **--path_to_model_config** - path to all necessary information for model
-        - **--path_to_instructions** - file with instruction prompts
-        - **--path_to_options** - file with mapping dataset to its entities
-        
-        ## Evaluation Results
-        
-        
-        
-        Dataset | Precision | Recall | F1-Score (weighted)
-        --- | --- | --- | --- | 
-        CONLL-2003 | 0.862 | 0.843 | 0.852 
-        MIT MOVIE | 0.792 | 0.845 | 0.809 | 
-        MIT REST | 0.766 | 0.771 | 0.768 | 
-        
-        ## Prediction Sample
-        ```
-        Sentence: The protest , which attracted several thousand supporters , coincided with the 18th anniversary of Spain 's constitution .
-        Instruction: please extract entities and their types from the input sentence, all entity types are in options
-        Options: ORG, PER, LOC
-        
-        Prediction (raw text): Spain is a LOC.
-        ```
-        ## Inference 
-        
-        ### Models
-        [t5-base-ner-conll](https://huggingface.co/olgaduchovny/t5-base-ner-conll)
-        
-        [t5-base-ner-mit-restaurant](https://huggingface.co/olgaduchovny/t5-base-ner-mit-restaurant)
-        
-        [t5-base-ner-mit-movie](https://huggingface.co/olgaduchovny/t5-base-ner-mit-movie)
-        
-        ### Code
-        ```python
-        from instruction_ner.model import Model
-        
-        model = Model(
-            model_path_or_name="olgaduchovny/t5-base-ner-conll",
-            tokenizer_path_or_name="olgaduchovny/t5-base-ner-conll"
-        )
-        
-        options = ["LOC", "PER", "ORG", "MISC"]
-        
-        instruction = "please extract entities and their types from the input sentence, " \
-                      "all entity types are in options"
-        
-        text = "My name is Olga. I am 24 years old. I live in Moscow and work at Sber AI Center as a Senior NLP Data Scientist." \
-                "This is my reporitory to test generative NER problem with T5 model."
-        
-        generation_kwargs = {
-            "num_beams": 2,
-            "max_length": 128
-        }
-        
-        pred_text, pred_spans = model.predict(
-            text=text,
-            generation_kwargs=generation_kwargs,
-            instruction=instruction,
-            options=options
-        )
-        
-        >>> ('Olga is a PER, Moscow is a LOC, Sber AI Center is an ORG, NLP is a MISC.',
-         [(11, 15, 'PER'), (46, 52, 'LOC'), (65, 79, 'ORG'), (92, 95, 'MISC')])
-        ```
-        
-        
-        
-        # Citation
-        ```bibtex
-        @article{wang2022instructionner,
-          title={Instructionner: A multi-task instruction-based generative framework for few-shot ner},
-          author={Wang, Liwen and Li, Rumei and Yan, Yang and Yan, Yuanmeng and Wang, Sirui and Wu, Wei and Xu, Weiran},
-          journal={arXiv preprint arXiv:2203.03903},
-          year={2022}
-        }
-        ```
-        
 Keywords: python,nlp,deep learning,ner,t5
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# InstructionNER: A Multi-Task Instruction-Based Generative Framework for Few-shot NER
+
+[![python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/ovbystrova/InstructionNER#requirements)
+[![license](https://img.shields.io/github/license/ovbystrova/InstructionNER?color=blue)](https://github.com/ovbystrova/InstructionNER/blob/main/LICENSE)
+[![pypi version](https://img.shields.io/pypi/v/instruction_ner)](https://pypi.org/project/instruction_ner)
+[![pypi downloads](https://img.shields.io/pypi/dm/instruction_ner)](https://pypi.org/project/instruction_ner)
+
+
+[![tests](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml/badge.svg)](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml)
+[![codecov](https://codecov.io/gh/ovbystrova/InstructionNER/branch/main/graph/badge.svg?token=L2OOZKLPJL)](https://codecov.io/gh/ovbystrova/InstructionNER)
+
+Unofficial implementation of [InstructionNER](https://arxiv.org/pdf/2203.03903v1.pdf).
+
+![Screenshot](resources/overall_intro.jpg)
+
+## Requirements
+Python >=3.8
+
+## Installation
+```shell
+pip install instruction-ner
+```
+
+(Alternative via requirements)
+```shell
+pip install -r requirements/requirements.in # for training purposes
+pip install -r requirements/requirements_test.in # for tests
+pip install -r requirements/requirements_dev.in # for inference only
+```
+
+## Data Preparation
+In order to make a unified training interface,
+you can convert your raw input data (supported dataset formats: **conll**, **spacy**, **mit**)
+with the following script:
+```
+instruction_ner-prepare-data \
+--path_to_file 'data/conll2003/train.txt' \
+--dataset_type 'conll2003' \
+--output_folder 'data/conll2003' \
+```
+
+This script converts every dataset to a list of sentences.
+Every sentence is like this:
+```
+{
+    "context": "SOCCER - JAPAN GET LUCKY WIN , CHINA IN SURPRISE DEFEAT .",
+    "entity_values": {
+            "LOC": [
+                "JAPAN"
+            ],
+            "PER": [
+                "CHINA"
+            ]
+        },
+    "entity_spans": [
+            {
+                "start": 9,
+                "end": 14,
+                "label": "LOC"
+            },
+            {
+                "start": 31,
+                "end": 36,
+                "label": "PER"
+            }
+        ]
+}
+```
+
+## Training
+Script for training T5 model:
+```
+instruction_ner-train \
+--path_to_instructions 'instructions.json' \
+--path_to_options 'options.json' \
+--log_dir 'runs/test_run' \
+--eval_every_n_batches 200 \
+--pred_every_n_batches 200 \
+--path_to_model_config 'config.yaml' \
+--path_to_model_save 'runs/model/' \
+```
+
+Arguments:
+- **--path_to_instructions** - file with instruction prompts
+- **--path_to_options** - file with mapping dataset to its entities
+- **--log_dir** - where to log tensorboard
+- **--eval_every_n_batches** - do evaluation every n batches
+- **--pred_every_n_batches** - write n sample prediction every n batches
+- **--path_to_model_config** - path to all necessary information for model
+- **--path_to_model_save** - where to save model
+
+## Evaluation
+Script for evaluation of the trained model:
+```
+instruction_ner-evaluate \
+--model_path_or_name 'olgaduchovny/t5-base-qa-ner-conll' \
+--path_to_model_config 'config.yaml' \
+--path_to_instructions 'instructions.json' \
+--path_to_options 'options.json' \
+```
+
+Arguments:
+- **--model_path_or_name** - path to trained model or HF model name
+- **--path_to_model_config** - path to all necessary information for model
+- **--path_to_instructions** - file with instruction prompts
+- **--path_to_options** - file with mapping dataset to its entities
+
+## Evaluation Results
+
+
+
+Dataset | Precision | Recall | F1-Score (weighted)
+--- | --- | --- | --- |
+CONLL-2003 | 0.862 | 0.843 | 0.852
+MIT MOVIE | 0.792 | 0.845 | 0.809 |
+MIT REST | 0.766 | 0.771 | 0.768 |
+
+## Prediction Sample
+```
+Sentence: The protest , which attracted several thousand supporters , coincided with the 18th anniversary of Spain 's constitution .
+Instruction: please extract entities and their types from the input sentence, all entity types are in options
+Options: ORG, PER, LOC
+
+Prediction (raw text): Spain is a LOC.
+```
+## Inference
+
+### Models
+[t5-base-ner-conll](https://huggingface.co/olgaduchovny/t5-base-ner-conll)
+
+[t5-base-ner-mit-restaurant](https://huggingface.co/olgaduchovny/t5-base-ner-mit-restaurant)
+
+[t5-base-ner-mit-movie](https://huggingface.co/olgaduchovny/t5-base-ner-mit-movie)
+
+### Code
+```python
+from instruction_ner.model import Model
+
+model = Model(
+    model_path_or_name="olgaduchovny/t5-base-ner-conll",
+    tokenizer_path_or_name="olgaduchovny/t5-base-ner-conll"
+)
+
+options = ["LOC", "PER", "ORG", "MISC"]
+
+instruction = "please extract entities and their types from the input sentence, " \
+              "all entity types are in options"
+
+text = "My name is Olga. I am 24 years old. I live in Moscow and work at Sber AI Center as a Senior NLP Data Scientist." \
+        "This is my reporitory to test generative NER problem with T5 model."
+
+generation_kwargs = {
+    "num_beams": 2,
+    "max_length": 128
+}
+
+pred_text, pred_spans = model.predict(
+    text=text,
+    generation_kwargs=generation_kwargs,
+    instruction=instruction,
+    options=options
+)
+
+>>> ('Olga is a PER, Moscow is a LOC, Sber AI Center is an ORG, NLP is a MISC.',
+ [(11, 15, 'PER'), (46, 52, 'LOC'), (65, 79, 'ORG'), (92, 95, 'MISC')])
+```
+
+
+
+# Citation
+```bibtex
+@article{wang2022instructionner,
+  title={Instructionner: A multi-task instruction-based generative framework for few-shot ner},
+  author={Wang, Liwen and Li, Rumei and Yan, Yang and Yan, Yuanmeng and Wang, Sirui and Wu, Wei and Xu, Weiran},
+  journal={arXiv preprint arXiv:2203.03903},
+  year={2022}
+}
+```
```

### Comparing `instruction_ner-0.1.3/README.md` & `instruction_ner-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # InstructionNER: A Multi-Task Instruction-Based Generative Framework for Few-shot NER
 
-[![tests](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml/badge.svg)](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml)
-[![codecov](https://codecov.io/gh/ovbystrova/InstructionNER/branch/main/graph/badge.svg?token=L2OOZKLPJL)](https://codecov.io/gh/ovbystrova/InstructionNER)
 [![python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/ovbystrova/InstructionNER#requirements)
 [![license](https://img.shields.io/github/license/ovbystrova/InstructionNER?color=blue)](https://github.com/ovbystrova/InstructionNER/blob/main/LICENSE)
+[![pypi version](https://img.shields.io/pypi/v/instruction_ner)](https://pypi.org/project/instruction_ner)
+[![pypi downloads](https://img.shields.io/pypi/dm/instruction_ner)](https://pypi.org/project/instruction_ner)
+
+
+[![tests](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml/badge.svg)](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml)
+[![codecov](https://codecov.io/gh/ovbystrova/InstructionNER/branch/main/graph/badge.svg?token=L2OOZKLPJL)](https://codecov.io/gh/ovbystrova/InstructionNER)
 
 Unofficial implementation of [InstructionNER](https://arxiv.org/pdf/2203.03903v1.pdf).
 
 ![Screenshot](resources/overall_intro.jpg)
 
 ## Requirements
 Python >=3.8
@@ -21,15 +25,15 @@
 ```shell
 pip install -r requirements/requirements.in # for training purposes
 pip install -r requirements/requirements_test.in # for tests
 pip install -r requirements/requirements_dev.in # for inference only
 ```
 
 ## Data Preparation
-In order to make a unified training interface, 
+In order to make a unified training interface,
 you can convert your raw input data (supported dataset formats: **conll**, **spacy**, **mit**)
 with the following script:
 ```
 instruction_ner-prepare-data \
 --path_to_file 'data/conll2003/train.txt' \
 --dataset_type 'conll2003' \
 --output_folder 'data/conll2003' \
@@ -102,28 +106,28 @@
 - **--path_to_options** - file with mapping dataset to its entities
 
 ## Evaluation Results
 
 
 
 Dataset | Precision | Recall | F1-Score (weighted)
---- | --- | --- | --- | 
-CONLL-2003 | 0.862 | 0.843 | 0.852 
-MIT MOVIE | 0.792 | 0.845 | 0.809 | 
-MIT REST | 0.766 | 0.771 | 0.768 | 
+--- | --- | --- | --- |
+CONLL-2003 | 0.862 | 0.843 | 0.852
+MIT MOVIE | 0.792 | 0.845 | 0.809 |
+MIT REST | 0.766 | 0.771 | 0.768 |
 
 ## Prediction Sample
 ```
 Sentence: The protest , which attracted several thousand supporters , coincided with the 18th anniversary of Spain 's constitution .
 Instruction: please extract entities and their types from the input sentence, all entity types are in options
 Options: ORG, PER, LOC
 
 Prediction (raw text): Spain is a LOC.
 ```
-## Inference 
+## Inference
 
 ### Models
 [t5-base-ner-conll](https://huggingface.co/olgaduchovny/t5-base-ner-conll)
 
 [t5-base-ner-mit-restaurant](https://huggingface.co/olgaduchovny/t5-base-ner-mit-restaurant)
 
 [t5-base-ner-mit-movie](https://huggingface.co/olgaduchovny/t5-base-ner-mit-movie)
```

### Comparing `instruction_ner-0.1.3/instruction_ner/arg_parse.py` & `instruction_ner-0.1.6/instruction_ner/arg_parse.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.3/instruction_ner/collator.py` & `instruction_ner-0.1.6/instruction_ner/collator.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.3/instruction_ner/core/datatypes.py` & `instruction_ner-0.1.6/instruction_ner/core/datatypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,51 @@
-from enum import Enum
-from typing import Dict, List, Optional
-
 from dataclasses import dataclass
+from enum import Enum
+from typing import Dict, List, Optional, Tuple, Union
 
 
 @dataclass(frozen=True, eq=True)
 class Span:
     """
     Core Span dataclass
     :param start(int): start index of an entity
     :param end(int): end index of an entity
     :param label(str): entity label
     """
+
     start: int
     end: int
     label: str
 
     def to_json(self):
         return {"start": self.start, "end": self.end, "label": self.label}
 
     @staticmethod
     def from_json(data):
-        return Span(
-            start=int(data["start"]),
-            end=int(data["end"]),
-            label=data["label"]
-        )
+        return Span(start=int(data["start"]), end=int(data["end"]), label=data["label"])
 
     @staticmethod
     def from_tuple(data):
-        return Span(
-            start=int(data[0]),
-            end=int(data[1]),
-            label=data[2]
-        )
+        return Span(start=int(data[0]), end=int(data[1]), label=data[2])
 
 
 @dataclass()
 class Instance:
     """
     Core Instance dataclass.
     :param context (str): initial text
     :param question (str): question for QA model
     :param answer (optional): raw answer from QA model
     :param spans (optional): List of Spans
     """
+
     context: str
     question: str
     answer: Optional[str]
-    entity_spans: Optional[List[Span]]
+    entity_spans: Optional[Union[List[Span], List[Tuple[int, int, str]]]]
     entity_values: Optional[Dict[str, List[str]]]
 
     def __str__(self):
 
         if self.answer is not None:
             return self.context + " " + self.question + " " + self.answer
```

### Comparing `instruction_ner-0.1.3/instruction_ner/core/reader.py` & `instruction_ner-0.1.6/instruction_ner/core/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from abc import ABC, abstractmethod
 import json
+from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Union, List, Dict
+from typing import Any, Dict, List, Union
 
 from instruction_ner.core.datatypes import DatasetField, Span
 
 
 class Reader(ABC):
     """
     Abstract class for Reading different datasets
     """
+
     @abstractmethod
     def read(self, data: Any):
         raise NotImplementedError
 
     @abstractmethod
     def read_from_file(self, path_to_file: Union[str, Path]):
         raise NotImplementedError
@@ -48,20 +49,20 @@
         """
         Get dict of {label: [values]} from sentence and entity Spans
         :param sentence: text in string format  (eg. 'London is the capital of Great Britain')
         :param entity_spans: List of Span object
         :return:
         """
 
-        entity_values = {}
+        entity_values: Dict[str, List[str]] = {}
 
         for entity in entity_spans:
             start, end, label = entity.start, entity.end, entity.label
 
-            entity_value = sentence[start: end]
+            entity_value = sentence[start:end]
 
             if label not in entity_values:
                 entity_values[label] = []
 
             if entity_value not in entity_values[label]:
                 entity_values[label].append(entity_value)
```

### Comparing `instruction_ner-0.1.3/instruction_ner/dataset.py` & `instruction_ner-0.1.6/instruction_ner/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-from typing import Dict, List, Any
+from typing import Any, Dict, List, Tuple, Union
 
 from torch.utils.data import Dataset
 from tqdm import tqdm
 
 from instruction_ner.core.datatypes import Instance, TaskType
 from instruction_ner.formatters import (
     EntityExtractTaskFormatter,
     EntityTypeTaskFormatter,
-    NERTaskFormatter
+    NERTaskFormatter,
 )
 
 
 class T5NERDataset(Dataset):
-
     def __init__(
-            self,
-            data: List[Dict[str, Any]],
-            instructions: Dict[str, str],
-            options: List[str],
-            tasks: List[TaskType] = (
-                    TaskType.NER,
-                    TaskType.ENTITY_EXTRACTOR,
-                    TaskType.ENTITY_TYPING
-            )
+        self,
+        data: List[Dict[str, Any]],
+        instructions: Dict[str, str],
+        options: List[str],
+        tasks: Union[Tuple[TaskType, TaskType, TaskType], List[TaskType]] = (
+            TaskType.NER,
+            TaskType.ENTITY_EXTRACTOR,
+            TaskType.ENTITY_TYPING,
+        ),
     ):
         super().__init__()
 
         self.instances = self._convert_list_to_instances(
-            data=data,
-            instructions=instructions,
-            options=options,
-            tasks=tasks
+            data=data, instructions=instructions, options=options, tasks=list(tasks)
         )
 
     def __len__(self) -> int:
         return len(self.instances)
 
     def __getitem__(self, index: int) -> Instance:
         return self.instances[index]
 
     def _convert_list_to_instances(
-            self,
-            data: List[Dict[str, Any]],
-            instructions: Dict[str, str],
-            options: List[str],
-            tasks: List[TaskType],
-            language: str = "en"
+        self,
+        data: List[Dict[str, Any]],
+        instructions: Dict[str, str],
+        options: List[str],
+        tasks: List[TaskType],
+        language: str = "en",
     ) -> List[Instance]:
         """
         Converts raw data into list of Instance objects
         :param data:
         :param instructions: mapping dictionary from task type to relevant instruction
         :param options: list of labels relevant to the whole dataset
         :param tasks: for what tasks create Instances (each task has its own instruction)
@@ -61,27 +57,27 @@
         for item in tqdm(data, desc="Prepare Dataset"):
 
             instances_per_item = self._convert_item_to_instances(
                 data_item=item,
                 instructions=instructions,
                 options=options,
                 tasks=tasks,
-                language=language
+                language=language,
             )
 
             instances.extend(instances_per_item)
         return instances
 
     def _convert_item_to_instances(
-            self,
-            data_item: Dict[str, Any],
-            instructions: Dict[str, str],
-            options: List[str],
-            tasks: List[TaskType],
-            language: str = "en"  # TODO uncomment this
+        self,
+        data_item: Dict[str, Any],
+        instructions: Dict[str, str],
+        options: List[str],
+        tasks: List[TaskType],
+        language: str = "en",  # TODO uncomment this
     ):
         """
         Creates all task instances from one element of data
         :param data_item:
         :param instructions: mapping dictionary from task type to relevant instruction
         :param options: list of labels relevant to the whole dataset
         :param tasks: for what tasks create Instances (each task has its own instruction)
@@ -90,15 +86,15 @@
 
         instances = []
 
         # TODO think about this dict and whether it is good for DIP
         task_to_formatter = {
             TaskType.ENTITY_EXTRACTOR: EntityExtractTaskFormatter(),
             TaskType.ENTITY_TYPING: EntityTypeTaskFormatter(),
-            TaskType.NER: NERTaskFormatter()
+            TaskType.NER: NERTaskFormatter(),
         }
 
         for task in tasks:
 
             if task.value not in instructions:
                 continue
 
@@ -107,13 +103,13 @@
             entity_spans = data_item["entity_spans"]
 
             instance = task_to_formatter[task].format_instance(
                 context=context,
                 entity_values=entity_values,
                 entity_spans=entity_spans,
                 instruction=instructions[task.value],
-                options=options
+                options=options,
             )
 
             instances.append(instance)
 
         return instances
```

### Comparing `instruction_ner-0.1.3/instruction_ner/evaluate.py` & `instruction_ner-0.1.6/instruction_ner/evaluate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+import warnings
+
 import torch
 from torch.utils.data import DataLoader
+from utils.evaluate_utils import evaluate
 
 from instruction_ner.arg_parse import get_evaluate_args
-from instruction_ner.model import Model
 from instruction_ner.collator import Collator
 from instruction_ner.dataset import T5NERDataset
-from instruction_ner.utils.utils import set_global_seed, load_config, load_json, loads_json
-from utils.evaluate_utils import evaluate
+from instruction_ner.model import Model
+from instruction_ner.utils.utils import (
+    load_config,
+    load_json,
+    loads_json,
+    set_global_seed,
+)
 
-import warnings
 warnings.filterwarnings("ignore")
 
 
 def main():
     args = get_evaluate_args()
     config = load_config(args.path_to_model_config)
 
@@ -22,27 +28,24 @@
     options = load_json(args.path_to_options)
     options = options[config["data"]["dataset"]]
     instructions = load_json(args.path_to_instructions)
 
     data_test = loads_json(config["data"]["test"])
 
     test_dataset = T5NERDataset(
-        data=data_test,
-        instructions=instructions["test"],
-        options=options
+        data=data_test, instructions=instructions["test"], options=options
     )
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     print(f"Using device: {device}")
 
     # load model
     model_path_or_name = args.model_path_or_name
     model = Model(
-        model_path_or_name=model_path_or_name,
-        tokenizer_path_or_name=model_path_or_name
+        model_path_or_name=model_path_or_name, tokenizer_path_or_name=model_path_or_name
     )
     model.model.to(device)
 
     tokenizer_kwargs = dict(config["tokenizer"])
     generation_kwargs = dict(config["generation"])
 
     collator = Collator(
@@ -61,13 +64,13 @@
         model=model.model,
         tokenizer=model.tokenizer,
         dataloader=test_dataloader,
         writer=None,
         device=device,
         epoch=0,
         generation_kwargs=generation_kwargs,
-        options=options
+        options=options,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `instruction_ner-0.1.3/instruction_ner/formatters/Answer.py` & `instruction_ner-0.1.6/instruction_ner/formatters/Answer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,71 @@
-from typing import Dict, List, Tuple, Optional
+from typing import Dict, List, Optional, Tuple
 
 from instruction_ner.core.datatypes import Language
 
-
 # TODO Think about adding Preffix.Answer
 # TODO separate functions based on language.
 
+
 class AnswerFormatter:
 
     available_languages = [Language.EN.value]
     patterns = {
         Language.EN.value: "{0} is {1} {2}",  # value is a/and label
     }
 
     @classmethod
     def from_values(
-            cls,
-            entity_values: Optional[Dict[str, List[str]]],
-            language: str = "en"
+        cls, entity_values: Optional[Dict[str, List[str]]], language: str = "en"
     ) -> Optional[str]:
 
         if language not in cls.available_languages:
-            raise ValueError(f"Expected language to be one of {cls.available_languages}")
+            raise ValueError(
+                f"Expected language to be one of {cls.available_languages}"
+            )
 
         if entity_values is None:
             return None
 
         answers = []
 
         for entity_label, values in entity_values.items():
 
             if entity_label.lower()[0] in ["a", "e", "u", "o"]:
-                answers.extend([cls.patterns[language].format(value, "an", entity_label) for value in values])
+                answers.extend(
+                    [
+                        cls.patterns[language].format(value, "an", entity_label)
+                        for value in values
+                    ]
+                )
             else:
-                answers.extend([cls.patterns[language].format(value, "a", entity_label) for value in values])
+                answers.extend(
+                    [
+                        cls.patterns[language].format(value, "a", entity_label)
+                        for value in values
+                    ]
+                )
 
         answer = ", ".join(answers) + "."
 
         return answer
 
     @classmethod
     def from_spans(
-            cls,
-            context: str,
-            entity_spans: List[Tuple[int, int, str]],
-            language: str = "en"
+        cls,
+        context: str,
+        entity_spans: List[Tuple[int, int, str]],
+        language: str = "en",
     ) -> str:
         answers = []
 
         if language not in cls.available_languages:
-            raise ValueError(f"Expected language to be one of {cls.available_languages}")
+            raise ValueError(
+                f"Expected language to be one of {cls.available_languages}"
+            )
 
         for span in entity_spans:
 
             start, end, label = span[0], span[1], span[2]
             value = context[start:end]
 
             if value.lower().startswith("a"):
```

### Comparing `instruction_ner-0.1.3/instruction_ner/formatters/PredictionSpan.py` & `instruction_ner-0.1.6/instruction_ner/formatters/PredictionSpan.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,45 +4,53 @@
 from instruction_ner.core.datatypes import Preffix, Span
 
 
 class PredictionSpanFormatter:
     """
     Turns raw Model output into NER spans (start_idx, end_idx, label)
     """
+
     answer_templates = ["is an", "is a"]  # TODO move this (get rid of literals)
 
-    def format_answer_spans(self, context: str, prediction: str, options: List[str]) -> List[Span]:
+    def format_answer_spans(
+        self, context: str, prediction: str, options: List[str]
+    ) -> List[Span]:
         """
         Based on model prediction and context create entity spans
         :param options:
         :param context:
         :param prediction:
         :return:
         """
 
         entity_spans = []
-        source_sentence = context.lstrip(Preffix.CONTEXT.value)
-
-        prediction = prediction.strip(".")  # Because answer in train data always ends with '.'
+        source_sentence = context.replace(
+            Preffix.CONTEXT.value,
+            "",
+            1  # replace only the first occurrence of substring
+        )
+
+        prediction = prediction.strip(
+            "."
+        )  # Because answer in train data always ends with '.'
         prediction_parts = prediction.split(",")
 
         for prediction_part in prediction_parts:
-            spans = self._get_span_from_part(
-                prediction_part,
-                source_sentence
-            )
+            spans = self._get_span_from_part(prediction_part, source_sentence)
             if spans is None:
                 continue
 
             spans = [span for span in spans if span.label in options]
             entity_spans.extend(spans)
 
         return entity_spans
 
-    def _get_span_from_part(self, prediction_part: str, source_sentence: str) -> Optional[List[Span]]:
+    def _get_span_from_part(
+        self, prediction_part: str, source_sentence: str
+    ) -> Optional[List[Span]]:
         """
         Gets entity span from part of prediction
         :param prediction_part: Olga is a PER
         :param source_sentence: Today Olga decided to sleep a lot.
         :return: (6, 10, "PER")
         """
 
@@ -56,32 +64,26 @@
                 continue
 
             value, label = _prediction_part[0], _prediction_part[1]
             value = value.strip(" ").rstrip(" ")
             label = label.strip(" ").rstrip(" ")
 
             try:
-                matches = re.finditer(value, source_sentence)
+                matches = list(re.finditer(value, source_sentence))
             except re.error:  # unbalanced parenthesis at position
                 return None
 
-            matches = list(matches)
-
             if len(matches) == 0:
                 return None
 
             spans = []
 
             for match in matches:
 
                 start = match.start()
                 end = match.end()
-                span = Span(
-                    start=start,
-                    end=end,
-                    label=label
-                )
+                span = Span(start=start, end=end, label=label)
                 spans.append(span)
 
             return spans
 
         return None
```

### Comparing `instruction_ner-0.1.3/instruction_ner/formatters/instances/EntityExtractTask.py` & `instruction_ner-0.1.6/instruction_ner/formatters/instances/EntityExtractTask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-from typing import Dict, List, Union, Optional
+from typing import Dict, List, Optional, Tuple
 
 from instruction_ner.core.datatypes import Instance, Preffix, Span
 from instruction_ner.formatters.instances import InstanceFormatter
 
 
 class EntityExtractTaskFormatter(InstanceFormatter):
     """
     Task: Extract all entity values from the text without their labels
     """
+
     def format_instance(
-            self,
-            context: str,
-            entity_values: Optional[Dict[str, List[str]]],
-            entity_spans: Optional[List[Dict[str, Union[int, str]]]],
-            instruction: str,
-            options: List[str]
+        self,
+        context: str,
+        entity_values: Optional[Dict[str, List[str]]],
+        entity_spans: Optional[List[Tuple[int, int, str]]],
+        instruction: str,
+        options: List[str],
     ) -> Instance:
 
         question = Preffix.INSTRUCTION.value + instruction
 
         answer = None
 
         if entity_values is not None:
             answers = []
             for _entity_values in entity_values.values():
                 answers.extend(_entity_values)
             answer = ", ".join(answers) + "."
 
         if entity_spans is not None:
-            entity_spans = [Span.from_json(span)for span in entity_spans]
+            entity_spans = [
+                Span.from_json(span)
+                for span in entity_spans
+                if not isinstance(span, Span)
+            ]
 
         instance = Instance(
             context=Preffix.CONTEXT.value + context,
             question=question,
             answer=answer,
             entity_spans=entity_spans,
-            entity_values=entity_values
+            entity_values=entity_values,
         )
 
         return instance
```

### Comparing `instruction_ner-0.1.3/instruction_ner/formatters/instances/EntityTypeTask.py` & `instruction_ner-0.1.6/instruction_ner/formatters/instances/EntityTypeTask.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-from typing import Dict, List, Union, Optional
+from typing import Dict, List, Optional, Tuple
 
 from instruction_ner.core.datatypes import Instance, Preffix, Span
 from instruction_ner.formatters.Answer import AnswerFormatter
 from instruction_ner.formatters.instances import InstanceFormatter
 
 
 class EntityTypeTaskFormatter(InstanceFormatter):
     """
     Task: Given sentence and entity values map them with entity labels
     """
+
     def format_instance(
-            self,
-            context: str,
-            entity_values: Optional[Dict[str, List[str]]],
-            entity_spans: Optional[List[Dict[str, Union[int, str]]]],
-            instruction: str,
-            options: List[str]
+        self,
+        context: str,
+        entity_values: Optional[Dict[str, List[str]]],
+        entity_spans: Optional[List[Tuple[int, int, str]]],
+        instruction: str,
+        options: List[str],
     ) -> Instance:
 
         entity_values_total = None
         if entity_values is not None:
             entity_values_total = []
             for values in entity_values.values():
                 entity_values_total.extend(values)
 
-        instruction = Preffix.INSTRUCTION.value + instruction + ": " + ", ".join(entity_values_total)
-        options = Preffix.OPTIONS.value + ", ".join(options)
-        question = instruction + " " + options
+        instruction = (
+            Preffix.INSTRUCTION.value
+            + instruction
+            + ": "
+            + ", ".join(entity_values_total)
+        )
+        options_str = Preffix.OPTIONS.value + ", ".join(options)
+        question = instruction + " " + options_str
 
         if entity_spans is not None:
-            entity_spans = [Span.from_json(span)for span in entity_spans]
+            entity_spans = [
+                Span.from_json(span)
+                for span in entity_spans
+                if not isinstance(span, Span)
+            ]
 
         instance = Instance(
             context=Preffix.CONTEXT.value + context,
             question=question,
             answer=AnswerFormatter.from_values(entity_values),
             entity_spans=entity_spans,
-            entity_values=entity_values
+            entity_values=entity_values,
         )
 
         return instance
```

### Comparing `instruction_ner-0.1.3/instruction_ner/formatters/instances/NERTask.py` & `instruction_ner-0.1.6/instruction_ner/formatters/instances/NERTask.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-from typing import Dict, List, Union, Optional
+from typing import Dict, List, Optional, Tuple
 
 from instruction_ner.core.datatypes import Instance, Preffix, Span
-from instruction_ner.formatters.instances import InstanceFormatter
 from instruction_ner.formatters.Answer import AnswerFormatter
+from instruction_ner.formatters.instances import InstanceFormatter
 
 
 class NERTaskFormatter(InstanceFormatter):
     """
     Task: Given sentence extract entity values and map them with entity labels
     """
+
     def format_instance(
-            self,
-            context: str,
-            entity_values: Optional[Dict[str, List[str]]],
-            entity_spans: Optional[List[Dict[str, Union[int, str]]]],
-            instruction: str,
-            options: List[str]
+        self,
+        context: str,
+        entity_values: Optional[Dict[str, List[str]]],
+        entity_spans: Optional[List[Tuple[int, int, str]]],
+        instruction: str,
+        options: List[str],
     ) -> Instance:
 
         instruction = Preffix.INSTRUCTION.value + instruction
-        options = Preffix.OPTIONS.value + ", ".join(options)
-        question = instruction + " " + options
+        options_joined = ", ".join(options)
+        options_string = Preffix.OPTIONS.value + options_joined
+        question = instruction + " " + options_string
 
         if entity_spans is not None:
-            entity_spans = [Span.from_json(span)for span in entity_spans]
+            entity_spans = [
+                Span.from_json(span)
+                for span in entity_spans
+                if not isinstance(span, Span)
+            ]
 
         instance = Instance(
             context=Preffix.CONTEXT.value + context,
             question=question,
             answer=AnswerFormatter.from_values(entity_values),
             entity_values=entity_values,
-            entity_spans=entity_spans
+            entity_spans=entity_spans,
         )
 
         return instance
```

### Comparing `instruction_ner-0.1.3/instruction_ner/formatters/instances/__init__.py` & `instruction_ner-0.1.6/instruction_ner/formatters/instances/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from abc import ABC, abstractmethod
-from typing import Dict, List, Tuple, Optional
+from typing import Dict, List, Optional, Tuple
 
 from instruction_ner.core.datatypes import Instance
 
 
 class InstanceFormatter(ABC):
-
     @abstractmethod
     def format_instance(
-            self,
-            context: str,
-            entity_values: Optional[Dict[str, List[str]]],
-            entity_spans: Optional[List[Tuple[int, int, str]]],
-            instruction: str,
-            options: List[str]
+        self,
+        context: str,
+        entity_values: Optional[Dict[str, List[str]]],
+        entity_spans: Optional[List[Tuple[int, int, str]]],
+        instruction: str,
+        options: List[str],
     ) -> Instance:
         """
         Based on text, values, instruction and list of labels creates Instance objects
         :param context: eg. 'SOCCER - JAPAN GET LUCKY WIN , CHINA IN SURPRISE DEFEAT .'
         :param entity_values: eg. {'LOC': ['JAPAN'], 'PER': ['CHINA']}
         :param entity_spans: eg. [(9, 15, 'LOC'), (31, 37, 'PER')]
         :param instruction: eg. 'Please extract all entities'
```

### Comparing `instruction_ner-0.1.3/instruction_ner/metrics.py` & `instruction_ner-0.1.6/instruction_ner/metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 import numpy as np
 
 from instruction_ner.core.datatypes import Span
 
 
 def calculate_metrics(
-        spans_pred: List[List[Span]],
-        spans_true: List[List[Span]],
-        options: List[str]
+    spans_pred: List[List[Span]], spans_true: List[List[Span]], options: List[str]
 ):
     """
     Built confusion matrix and calculate metrics (precision, recall, f1-score)
     average options: micro, macro, weighted
     :param spans_pred: predicted spans over batch / epoch
     :param spans_true: true spans over batch / epoch
     :param options: list of labels presented in data
@@ -25,32 +23,56 @@
 
     confusion_matrix = build_confusion_matrix(
         spans_pred=spans_pred,
         spans_true=spans_true,
         label2index=label2index
     )
 
+    support_per_label = calculate_support_classes(
+        spans=spans_true
+    )
+
     metrics_per_label = calculate_metrics_from_confusion_matrix(
         confusion_matrix=confusion_matrix,
         label2index=label2index
     )
 
+    metrics_per_label = merge_metrics_and_support(
+        metrics_per_label=metrics_per_label,
+        support_per_label=support_per_label
+    )
+
     metrics = add_average_metrics(
         confusion_matrix=confusion_matrix,
         label2index=label2index,
-        metrics=metrics_per_label
+        metrics=metrics_per_label,
     )
 
     return metrics
 
 
+def calculate_support_classes(spans: List[List[Span]]):
+    """
+    Calculate how many items there are for every label
+    :param spans: true spans
+    """
+    support_dict = {}
+    spans = [span for sub_spans in spans for span in sub_spans]
+    for span in spans:
+        if span.label not in support_dict:
+            support_dict[span.label] = 1
+        else:
+            support_dict[span.label] += 1
+    return support_dict
+
+
 def build_confusion_matrix(
-        spans_pred: List[List[Span]],
-        spans_true: List[List[Span]],
-        label2index: Dict[str, int]
+    spans_pred: List[List[Span]],
+    spans_true: List[List[Span]],
+    label2index: Dict[str, int],
 ) -> np.array:
     """
     Build confusion matrix based on true and predicted spans
     :param spans_pred: predicted spans over batch / epoch
     :param spans_true: true spans over batch / epoch
     :param label2index: mapping between label and its index in confusion matrix
     :return: confusion matrix
@@ -60,25 +82,25 @@
 
     for spans_pred_batch, spans_true_batch in zip(spans_pred, spans_true):
 
         confusion_matrix = update_confusion_matrix(
             spans_pred=spans_pred_batch,
             spans_true=spans_true_batch,
             confusion_matrix=confusion_matrix,
-            label2index=label2index
+            label2index=label2index,
         )
 
     return confusion_matrix
 
 
 def update_confusion_matrix(
-        spans_pred: List[Span],
-        spans_true: List[Span],
-        confusion_matrix: np.array,
-        label2index: Dict[str, int]
+    spans_pred: List[Span],
+    spans_true: List[Span],
+    confusion_matrix: np.array,
+    label2index: Dict[str, int],
 ) -> np.array:
     """
     Update confusion matrix based on spans from one data item
     :param spans_pred: predicted spans from text
     :param spans_true: true spans for text
     :param confusion_matrix: matrix (n_labels, n_labels)
     :param label2index: mapping between label and its index in confusion matrix
@@ -94,30 +116,51 @@
 
         j = label2index[span_pred.label]
 
         if span_pred in spans_true:
             confusion_matrix[j][j] += 1  # True Positive
             continue
 
-        equal_start = [span for span in spans_true if span.start == span_pred.start and span.end != span_pred.end
-                       and span.label == span_pred.label]
-        equal_end = [span for span in spans_true if span.end == span_pred.end and span.label == span_pred.label
-                     and span.start != span_pred.start]
-        equal_start_end = [span for span in spans_true if span.end == span_pred.end and span.start == span_pred.start
-                           and span.label != span_pred.label]
-
-        if len(equal_start_end) > 0:  # If model found the right boundaries but wrong label
+        equal_start = [
+            span
+            for span in spans_true
+            if span.start == span_pred.start
+            and span.end != span_pred.end
+            and span.label == span_pred.label
+        ]
+        equal_end = [
+            span
+            for span in spans_true
+            if span.end == span_pred.end
+            and span.label == span_pred.label
+            and span.start != span_pred.start
+        ]
+        equal_start_end = [
+            span
+            for span in spans_true
+            if span.end == span_pred.end
+            and span.start == span_pred.start
+            and span.label != span_pred.label
+        ]
+
+        if (
+            len(equal_start_end) > 0
+        ):  # If model found the right boundaries but wrong label
             equal_start_end_span = equal_start_end[0]
             confusion_matrix[label2index[equal_start_end_span.label]][j] += 1
             if equal_start_end_span in spans_true_missed_in_pred:
                 spans_true_missed_in_pred.remove(equal_start_end_span)
             continue
 
-        elif len(equal_start) == 0 and len(equal_end) == 0:  # If model found wrong boundaries
-            confusion_matrix[label2index["O"]][j] += 1  # False Positive   # TODO remove 'O' with special variable
+        elif (
+            len(equal_start) == 0 and len(equal_end) == 0
+        ):  # If model found wrong boundaries
+            confusion_matrix[label2index["O"]][
+                j
+            ] += 1  # False Positive   # TODO remove 'O' with special variable
             continue
 
         for equal_start_span in equal_start:  # If start matches  # TODO simplify
             if span_pred.end < equal_start_span.end:
                 confusion_matrix[j][label2index["O"]] += 1  # False Negative
             elif span_pred.end > equal_start_span.end:
                 confusion_matrix[label2index["O"]][j] += 1  # False Positive
@@ -138,16 +181,15 @@
     for span in spans_true_missed_in_pred:
         confusion_matrix[label2index[span.label]][label2index["O"]] += 1
 
     return confusion_matrix
 
 
 def calculate_metrics_from_confusion_matrix(
-        confusion_matrix: np.array,
-        label2index: Dict[str, int]
+    confusion_matrix: np.array, label2index: Dict[str, int]
 ) -> Dict[str, Dict[str, float]]:
     """
     Calculate Precision, Recall, F1-Score per label (without average)
     :param confusion_matrix: np.array
     :param label2index: mapping between label and its index in confusion matrix
     :return:
     """
@@ -158,32 +200,60 @@
 
         if label == "O":
             continue
 
         metrics_per_label = {}
 
         true_positive = confusion_matrix[idx][idx]
-        precision = true_positive / (np.sum(confusion_matrix[:, idx])) if true_positive > 0 else 0
-        recall = true_positive / (np.sum(confusion_matrix[idx, :])) if true_positive > 0 else 0
+        precision = (
+            true_positive / (np.sum(confusion_matrix[:, idx]))
+            if true_positive > 0
+            else 0
+        )
+        recall = (
+            true_positive / (np.sum(confusion_matrix[idx, :]))
+            if true_positive > 0
+            else 0
+        )
 
         metrics_per_label["precision"] = precision
         metrics_per_label["recall"] = recall
-        metrics_per_label["f1-score"] = 2 * precision * recall / (precision + recall) \
-            if precision > 0 and recall > 0 else 0
-        metrics_per_label["support"] = np.sum(confusion_matrix[idx][:])
+        metrics_per_label["f1-score"] = (
+            2 * precision * recall / (precision + recall)
+            if precision > 0 and recall > 0
+            else 0
+        )
 
         metrics[label] = metrics_per_label
 
     return metrics
 
 
+def merge_metrics_and_support(
+        metrics_per_label: Dict[str, Dict[str, float]],
+        support_per_label: Dict[str, float]
+) -> Dict[str, Dict[str, float]]:
+    """
+    Merge dictionary with metrics with support for every label
+    :param metrics_per_label: dictionary with label and its metrics
+    :param support_per_label: dictionary with label and its support
+    """
+    for label in metrics_per_label:
+        if label in support_per_label:
+            metrics_per_label[label]["support"] = support_per_label[label]
+        else:
+            metrics_per_label[label]["support"] = 0
+
+    return metrics_per_label
+
+
 def add_average_metrics(
-        confusion_matrix: np.array,
-        label2index: Dict[str, int],
-        metrics: Dict[str, Dict[str, float]]
+    confusion_matrix: np.array,
+    label2index: Dict[str, int],
+    metrics: Dict[str, Dict[str, float]],
 ) -> Dict[str, Dict[str, float]]:
     """
     Add micro average, marco average, and weighted average metrics
     :param confusion_matrix: np.array
     :param label2index: mapping between label and its index in confusion matrix
     :param metrics: metrics per label
     :return:
@@ -199,31 +269,39 @@
         supports.append(metrics_label["support"])
 
     supports_proportions = [support / np.sum(supports) for support in supports]
 
     metrics["macro_avg"] = {
         "precision": np.mean(precisions),
         "recall": np.mean(recalls),
-        "f1-score": np.mean(f1scores)
+        "f1-score": np.mean(f1scores),
     }
 
     idxs = [value for key, value in label2index.items() if key != "O"]
     true_positive_total = np.sum(np.diag(confusion_matrix))  # TODO simplify this
-    false_positive_total = np.sum([np.sum(confusion_matrix[:][idx]) - confusion_matrix[idx][idx] for idx in idxs])
-    false_negative_total = np.sum([np.sum(confusion_matrix[idx][:]) - confusion_matrix[idx][idx] for idx in idxs])
+    false_positive_total = np.sum(
+        [np.sum(confusion_matrix[:][idx]) - confusion_matrix[idx][idx] for idx in idxs]
+    )
+    false_negative_total = np.sum(
+        [np.sum(confusion_matrix[idx][:]) - confusion_matrix[idx][idx] for idx in idxs]
+    )
     precision_micro = true_positive_total / (true_positive_total + false_positive_total)
     recall_micro = true_positive_total / (true_positive_total + false_negative_total)
 
     metrics["micro_avg"] = {
         "precision": precision_micro,
         "recall": recall_micro,
-        "f1-score": 2 * precision_micro * recall_micro / (precision_micro + recall_micro)
-        if precision_micro > 0 and recall_micro > 0 else 0
+        "f1-score": 2
+        * precision_micro
+        * recall_micro
+        / (precision_micro + recall_micro)
+        if precision_micro > 0 and recall_micro > 0
+        else 0,
     }
 
     metrics["weighted_avg"] = {
         "precision": np.average(precisions, weights=supports_proportions),
         "recall": np.average(recalls, weights=supports_proportions),
-        "f1-score": np.average(f1scores, weights=supports_proportions)
+        "f1-score": np.average(f1scores, weights=supports_proportions),
     }
 
     return metrics
```

### Comparing `instruction_ner-0.1.3/instruction_ner/model.py` & `instruction_ner-0.1.6/instruction_ner/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,39 @@
+from dataclasses import astuple
 from typing import Any, Dict, List, Tuple
 
-from dataclasses import astuple
 import torch
-from transformers import T5Tokenizer, T5ForConditionalGeneration
+from transformers import T5ForConditionalGeneration, T5Tokenizer
 
-from instruction_ner.formatters import (
-    NERTaskFormatter,
-    PredictionSpanFormatter
-)
+from instruction_ner.formatters import NERTaskFormatter, PredictionSpanFormatter
 
 
 class Model:
+    def __init__(self, model_path_or_name: str, tokenizer_path_or_name: str):
 
-    def __init__(self,
-                 model_path_or_name: str,
-                 tokenizer_path_or_name: str
-                 ):
-
-        self.tokenizer = T5Tokenizer.from_pretrained(model_path_or_name,
-                                                     # local_files_only=True
-                                                     )
-        self.model = T5ForConditionalGeneration.from_pretrained(tokenizer_path_or_name,
-                                                                # local_files_only=True
-                                                                )
+        self.tokenizer = T5Tokenizer.from_pretrained(
+            model_path_or_name,
+            # local_files_only=True
+        )
+        self.model = T5ForConditionalGeneration.from_pretrained(
+            tokenizer_path_or_name,
+            # local_files_only=True
+        )
 
         self.formatter = NERTaskFormatter()
 
         self.answer_formatter = PredictionSpanFormatter()
 
-    def predict(self,
-                text: str,
-                generation_kwargs: Dict[str, Any],
-                instruction: str,
-                options: List[str]
-                ) -> Tuple[str, List[Tuple[int, int, str]]]:
+    def predict(
+        self,
+        text: str,
+        generation_kwargs: Dict[str, Any],
+        instruction: str,
+        options: List[str],
+    ) -> Tuple[Any, List[Tuple[Any, ...]]]:
         """
         Generate prediction and format spans based on TaskType
         :param options:
         :param instruction:
         :param generation_kwargs:
         :param text: input text
         :return:
@@ -46,27 +42,26 @@
         self.model.eval()
 
         instance = self.formatter.format_instance(
             context=text,
             instruction=instruction,
             options=options,
             entity_spans=None,
-            entity_values=None
+            entity_values=None,
         )
 
         input_ids = self.tokenizer(
-            [instance.context], [instance.question], return_tensors="pt").input_ids
+            [instance.context], [instance.question], return_tensors="pt"
+        ).input_ids
 
         with torch.no_grad():
             outputs = self.model.generate(input_ids, **generation_kwargs)
 
         # change to false if labels are special tokens
         answer_raw = self.tokenizer.decode(outputs[0], skip_special_tokens=True)
 
         answer_spans = self.answer_formatter.format_answer_spans(
-            context=instance.context,
-            prediction=answer_raw,
-            options=options
+            context=instance.context, prediction=answer_raw, options=options
         )
-        answer_spans = [astuple(span) for span in answer_spans]
+        answer_spans_raw = [astuple(span) for span in answer_spans]
 
-        return answer_raw, answer_spans
+        return answer_raw, answer_spans_raw
```

### Comparing `instruction_ner-0.1.3/instruction_ner/prepare_data.py` & `instruction_ner-0.1.6/instruction_ner/prepare_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from instruction_ner.arg_parse import get_data_args
 from instruction_ner.core.datatypes import DatasetType
-from instruction_ner.readers import CONLLReader, SpacyReader, MITReader
+from instruction_ner.readers import CONLLReader, MITReader, SpacyReader
 
 dataset2reader = {
     DatasetType.CONLL2003.value: CONLLReader,
     DatasetType.SPACY.value: SpacyReader,
     DatasetType.MIT.value: MITReader,
 }
 
@@ -18,28 +18,25 @@
     dataset = args.dataset_type
     filepath = Path(args.path_to_file)
     if not filepath.exists():
         raise FileNotFoundError(f"File {filepath.as_posix()} not exists")
     output_dir = args.output_folder
     if output_dir is None:
         output_dir = filepath.parent
-        print(f"--output_dir not specified. Going to save at {filepath.parent.as_posix()}")
+        print(
+            f"--output_dir not specified. Going to save at {filepath.parent.as_posix()}"
+        )
     else:
         output_dir = Path(output_dir)
 
     if dataset not in dataset2reader:
         raise ValueError(f"Expected dataset to be on of {dataset2reader.keys()}")
 
     reader = dataset2reader[dataset]()
-    data = reader.read_from_file(
-        path_to_file=filepath
-    )
+    data = reader.read_from_file(path_to_file=filepath)
 
     filepath_save = output_dir / (filepath.stem + ".json")
-    reader.save_to_json(
-        data=data,
-        path=filepath_save
-    )
+    reader.save_to_json(data=data, path=filepath_save)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `instruction_ner-0.1.3/instruction_ner/readers/conll.py` & `instruction_ner-0.1.6/instruction_ner/readers/conll.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Dict, List, Union, Tuple
+from typing import Any, Dict, List, Tuple, Union
 
 from instruction_ner.core.datatypes import DatasetField, Span
 from instruction_ner.core.reader import Reader
 
 
 class CONLLReader(Reader):
 
@@ -25,25 +25,29 @@
 
         documents = self._split_lines_by_documents(data)
         sentences = []
         for document in documents:
             sentence_tokens = self._split_documents_by_sentences(document)
             sentences.extend(sentence_tokens)
 
-        sentences = [sentence for sentence in sentences if len(sentence) > self.MIN_SENTENCE_LENGTH]
+        sentences = [
+            sentence
+            for sentence in sentences
+            if len(sentence) > self.MIN_SENTENCE_LENGTH
+        ]
 
         data_processed = []
         for sentence in sentences:
             text, entity_spans = self._get_text_and_spans_from_sentence(sentence)
             entity_values = self._get_entity_values_from_text(text, entity_spans)
 
             dataset_item = {
                 DatasetField.CONTEXT.value: text,
                 DatasetField.ENTITY_VALUES.value: entity_values,
-                DatasetField.ENTITY_SPANS.value: entity_spans
+                DatasetField.ENTITY_SPANS.value: entity_spans,
             }
             data_processed.append(dataset_item)
         return data_processed
 
     def read_from_file(self, path_to_file: Union[str, Path]):
         """
         Wrapper around self.read(). Read 'path_to_file' and run self.read()
@@ -71,25 +75,27 @@
         :param file_lines: initial file lines
         :return: List of documents. Each document is a list of tokens
         """
 
         documents = []
 
         i = 0
-        document_tokens = []
+        document_tokens: List[str] = []
         while i < len(file_lines):
             line = file_lines[i]
             if line.startswith(self.token_doc_start):
                 i += 2
 
-                if len(document_tokens) == 0:  # When processing first line document_tokens is empty
+                if (
+                    len(document_tokens) == 0
+                ):  # When processing first line document_tokens is empty
                     continue
 
                 documents.append(document_tokens)
-                document_tokens = []
+                document_tokens = list()
                 continue
 
             document_tokens.append(line)
             i += 1
 
         if len(document_tokens) != 0:
             documents.append(document_tokens)
@@ -101,15 +107,15 @@
         Get list of sentence tokes from document
         :param document: initial document lines
         :return: List of sentences. Each sentence is a list of tokens
         """
         sentences = []
 
         i = 0
-        sentence_tokens = []
+        sentence_tokens: List[str] = []
         while i < len(document):
             line = document[i]
 
             if line == self.sentence_separator:
                 sentences.append(sentence_tokens)
                 sentence_tokens = []
                 i += 1
@@ -119,15 +125,17 @@
             i += 1
 
         if len(sentence_tokens) != 0:
             sentences.append(sentence_tokens)
 
         return sentences
 
-    def _get_text_and_spans_from_sentence(self, sentence: List[str]) -> Tuple[str, List[Span]]:
+    def _get_text_and_spans_from_sentence(
+        self, sentence: List[str]
+    ) -> Tuple[str, List[Span]]:
         """
         Get raw text from sentence token lines. Along with raw text return list of Span entities
         :param sentence: List of tokens (eg. ['-DOCSTART- -X- -X- O', '\n', '\n', 'JAPAN NNP B-NP B-LOC'])
         :return: raw text and entity Spans
         """
 
         text_tokens = []
@@ -136,48 +144,52 @@
         current_start_idx = 0
         entity_length = 0
         entity_label = None
         for token_line in sentence:
             tokens = token_line.split(self.token_separator)
 
             if len(tokens) != 4:
-                raise ValueError(f"Expected 4 elements after split, got {len(tokens)}: {token_line}")
+                raise ValueError(
+                    f"Expected 4 elements after split, got {len(tokens)}: {token_line}"
+                )
 
             token, label = tokens[0], tokens[-1]
             text_tokens.append(token)
 
             if label == "O":
 
                 if entity_label is not None and entity_length != 0:
                     # It means that previous token was entity and we should create Span
                     entity_span = Span(
                         start=current_start_idx,
-                        end=current_start_idx+entity_length-1,
-                        label=entity_label
+                        end=current_start_idx + entity_length - 1,
+                        label=entity_label,
                     )
                     entity_spans.append(entity_span)
 
                     entity_label = None
                     entity_length = 0
 
                     current_start_idx = entity_span.end + 1
 
                 current_start_idx += len(token)
-                current_start_idx += 1  # Because in the end we join them with space symbol
+                current_start_idx += (
+                    1  # Because in the end we join them with space symbol
+                )
                 continue
 
             # If we have two entities one after another
             if label.startswith("B" + self.label_prefix) and entity_label is not None:
 
                 self.C_B += 1
 
                 entity_span = Span(
                     start=current_start_idx,
                     end=current_start_idx + entity_length - 1,
-                    label=entity_label
+                    label=entity_label,
                 )
                 entity_spans.append(entity_span)
 
                 entity_length = 0
                 current_start_idx = entity_span.end + 1
 
             tag, entity_label = label.split(self.label_prefix, maxsplit=1)
@@ -185,14 +197,14 @@
 
         # if last tokens of sentence are entity
         if entity_length is not None and entity_label is not None:
             self.C_LAST += 1
             entity_span = Span(
                 start=current_start_idx,
                 end=current_start_idx + entity_length - 1,
-                label=entity_label
+                label=entity_label,
             )
             entity_spans.append(entity_span)
 
         text = " ".join(text_tokens)
 
         return text, entity_spans
```

### Comparing `instruction_ner-0.1.3/instruction_ner/readers/mit.py` & `instruction_ner-0.1.6/instruction_ner/readers/mit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Dict, Union, List
+from typing import Any, Dict, List, Union
 
 from instruction_ner.core.datatypes import DatasetField, Span
 from instruction_ner.core.reader import Reader
 
 
 # TODO this code duplicates CONLL parser a lot. Think about moving to ABC class
 class MITReader(Reader):
@@ -19,25 +19,29 @@
         Main function of MIT Reader. Takes lines of strings as input, splits them into sentences.
         And return data in unified format
         :param data: List of string from .bio file
         :return: List of sentences with spans and entity values
         """
 
         sentences = self._split_by_sentences(data)
-        sentences = [sentence for sentence in sentences if len(sentence) > self.MIN_SENTENCE_LENGTH]
+        sentences = [
+            sentence
+            for sentence in sentences
+            if len(sentence) > self.MIN_SENTENCE_LENGTH
+        ]
 
         data_processed = []
         for sentence in sentences:
             text, entity_spans = self._get_text_and_spans_from_sentence(sentence)
             entity_values = self._get_entity_values_from_text(text, entity_spans)
 
             dataset_item = {
                 DatasetField.CONTEXT.value: text,
                 DatasetField.ENTITY_VALUES.value: entity_values,
-                DatasetField.ENTITY_SPANS.value: entity_spans
+                DatasetField.ENTITY_SPANS.value: entity_spans,
             }
             data_processed.append(dataset_item)
 
         return data_processed
 
     def read_from_file(self, path_to_file: Union[str, Path]) -> List[Dict[str, Any]]:
         """
@@ -45,15 +49,17 @@
         :param path_to_file: string or Path
         :return: List of Dicts where each element is a sentence with entities
         """
         if isinstance(path_to_file, str):
             path_to_file = Path(path_to_file)
 
         if path_to_file.suffix.lower() not in self.supported_extensions:
-            raise ValueError(f"Expected file to be on of {self.supported_extensions}. Got {path_to_file.suffix}")
+            raise ValueError(
+                f"Expected file to be on of {self.supported_extensions}. Got {path_to_file.suffix}"
+            )
 
         with open(path_to_file, "r") as f:
             file_lines = f.readlines()
             file_lines = [x.strip("\n") for x in file_lines]
 
         data = self.read(data=file_lines)
 
@@ -64,15 +70,15 @@
         Get list of sentence tokes from document
         :param document: initial lines
         :return: List of sentences. Each sentence is a list of tokens
         """
         sentences = []
 
         i = 0
-        sentence_tokens = []
+        sentence_tokens: List[str] = []
         while i < len(document):
             line = document[i]
 
             if line == self.sentence_separator:
                 sentences.append(sentence_tokens)
                 sentence_tokens = []
                 i += 1
@@ -94,59 +100,66 @@
         current_start_idx = 0
         entity_length = 0
         entity_label = None
         for token_line in sentence:
             tokens = token_line.split(self.token_separator)
 
             if len(tokens) != 2:
-                raise ValueError(f"Expected 2 elements after split, got {len(tokens)}: {token_line}")
+                raise ValueError(
+                    f"Expected 2 elements after split, got {len(tokens)}: {token_line}"
+                )
 
-            token, label = tokens[-1], tokens[0]  # this is the only difference from CONLL
+            token, label = (
+                tokens[-1],
+                tokens[0],
+            )  # this is the only difference from CONLL
             text_tokens.append(token)
 
             if label == "O":
 
                 if entity_label is not None and entity_length != 0:
                     # It means that previous token was entity and we should create Span
                     entity_span = Span(
                         start=current_start_idx,
                         end=current_start_idx + entity_length - 1,
-                        label=entity_label
+                        label=entity_label,
                     )
                     entity_spans.append(entity_span)
 
                     entity_label = None
                     entity_length = 0
 
                     current_start_idx = entity_span.end + 1
 
                 current_start_idx += len(token)
-                current_start_idx += 1  # Because in the end we join them with space symbol
+                current_start_idx += (
+                    1  # Because in the end we join them with space symbol
+                )
                 continue
 
             # If we have two entities one after another
             if label.startswith("B" + self.label_prefix) and entity_label is not None:
                 entity_span = Span(
                     start=current_start_idx,
                     end=current_start_idx + entity_length - 1,
-                    label=entity_label
+                    label=entity_label,
                 )
                 entity_spans.append(entity_span)
 
                 entity_length = 0
                 current_start_idx = entity_span.end + 1
 
             tag, entity_label = label.split(self.label_prefix, maxsplit=1)
             entity_length += len(token) + 1
 
         # if last tokens of sentence are entity
         if entity_length is not None and entity_label is not None:
             entity_span = Span(
-                        start=current_start_idx,
-                        end=current_start_idx + entity_length - 1,
-                        label=entity_label
-                    )
+                start=current_start_idx,
+                end=current_start_idx + entity_length - 1,
+                label=entity_label,
+            )
             entity_spans.append(entity_span)
 
         text = " ".join(text_tokens)
 
         return text, entity_spans
```

### Comparing `instruction_ner-0.1.3/instruction_ner/readers/spacy.py` & `instruction_ner-0.1.6/instruction_ner/readers/spacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 import ast
 from pathlib import Path
-from typing import Any, Dict, Union, List
+from typing import Any, Dict, List, Union
 
 import pandas as pd
 
 from instruction_ner.core.datatypes import DatasetField, Span
 from instruction_ner.core.reader import Reader
 
 
 class SpacyReader(Reader):
 
     text_column = "text"
     entities_column = "labels"
 
     supported_extensions = [".csv", ".xlsx"]
 
-    def read(self, data: pd.DataFrame, text_column=None, entities_column=None) -> List[Dict[str, Any]]:
+    def read(
+        self, data: pd.DataFrame, text_column=None, entities_column=None
+    ) -> List[Dict[str, Any]]:
         """
         Main function of SpacyReader. Based on pd.DataFrame with two specific columns
         create json with text, entity spans and values
         :param data: pd.DataFrame with two columns: text_column, entities_column
         :param text_column: str or None (ex. "text")
         :param entities_column: str or None (ex. "labels")
         :return:  List of Dicts where each element is a text with entities
         """
         text_column = text_column if text_column is not None else self.text_column
-        entities_column = entities_column if entities_column is not None else self.entities_column
+        entities_column = (
+            entities_column if entities_column is not None else self.entities_column
+        )
 
         for column in [text_column, entities_column]:
             if column not in data.columns:
-                raise ValueError(f"Expected dataframe to be with column {column}. Got {data.columns}"
-                                 f"Either rename your columns to default: {self.text_column, self.entities_column}"
-                                 f"Or pass your column names as parameters to this function.")
-
-        data = self.literal_eval(
-            df=data,
-            columns=[self.entities_column]
-        )
+                raise ValueError(
+                    f"Expected dataframe to be with column {column}. Got {data.columns}"
+                    f"Either rename your columns to default: {self.text_column, self.entities_column}"
+                    f"Or pass your column names as parameters to this function."
+                )
+
+        data = self.literal_eval(df=data, columns=[self.entities_column])
 
         data_processed = []
-        texts, entities = data[self.text_column].tolist(), data[self.entities_column].tolist()
+        texts, entities = (
+            data[self.text_column].tolist(),
+            data[self.entities_column].tolist(),
+        )
 
         for text, entity_spans in zip(texts, entities):
 
             entity_spans = [
-                Span(
-                    start=span[0],
-                    end=span[1],
-                    label=span[2]
-                ) for span in entity_spans
+                Span(start=span[0], end=span[1], label=span[2]) for span in entity_spans
             ]
 
             entity_values = self._get_entity_values_from_text(text, entity_spans)
 
             dataset_item = {
                 DatasetField.CONTEXT.value: text,
                 DatasetField.ENTITY_VALUES.value: entity_values,
-                DatasetField.ENTITY_SPANS.value: entity_spans
+                DatasetField.ENTITY_SPANS.value: entity_spans,
             }
             data_processed.append(dataset_item)
 
         return data_processed
 
-    def read_from_file(self, path_to_file: Union[str, Path], sep: str = ";") -> List[Dict[str, Any]]:
+    def read_from_file(
+        self, path_to_file: Union[str, Path], sep: str = ";"
+    ) -> List[Dict[str, Any]]:
         """
         Wrapper around self.read(). Read "path_to_file" and run self.read()
         :param path_to_file: string or Path
         :param sep: separator for pd.DataFrame (default is ";")
         :return: List of Dicts where each element is a sentence with entities
         """
         if isinstance(path_to_file, str):
@@ -75,19 +79,19 @@
         if path_to_file.suffix.lower() == ".csv":
             df = pd.read_csv(path_to_file, sep=sep)
 
         elif path_to_file.suffix.lower() == ".xlsx":
             df = pd.read_excel(path_to_file, engine="openpyxl")
 
         else:
-            raise ValueError(f"Expected file to be on of {self.supported_extensions}. Got {path_to_file.suffix}")
+            raise ValueError(
+                f"Expected file to be on of {self.supported_extensions}. Got {path_to_file.suffix}"
+            )
 
-        data = self.read(
-            data=df
-        )
+        data = self.read(data=df)
 
         return data
 
     @staticmethod
     def literal_eval(df: pd.DataFrame, columns: List[str]) -> pd.DataFrame:
         """
         Helper function to run ast.literal_eval on specific columns in pd.DataFrame
```

### Comparing `instruction_ner-0.1.3/instruction_ner/train.py` & `instruction_ner-0.1.6/instruction_ner/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import datetime
+import warnings
 from pathlib import Path
 
-from sklearn.model_selection import train_test_split
 import torch
+from sklearn.model_selection import train_test_split
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
-from transformers import T5Tokenizer, T5ForConditionalGeneration
+from transformers import T5ForConditionalGeneration, T5Tokenizer
 
 from instruction_ner.arg_parse import get_train_args
 from instruction_ner.collator import Collator
 from instruction_ner.dataset import T5NERDataset
-from instruction_ner.utils.utils import set_global_seed, load_config, load_json, loads_json
 from instruction_ner.utils.train_utils import train
+from instruction_ner.utils.utils import (
+    load_config,
+    load_json,
+    loads_json,
+    set_global_seed,
+)
 
-import warnings
 warnings.filterwarnings("ignore")
 
 
 def main():
     args = get_train_args()
 
     config = load_config(args.path_to_model_config)
@@ -36,32 +41,26 @@
 
     # load data files
     data_train = loads_json(config["data"]["train"])
 
     valid_path = config["data"]["valid"]
     if valid_path is None:
         data_train, data_valid = train_test_split(
-            data_train,
-            test_size=0.15,
-            random_state=config["seed"]
+            data_train, test_size=0.15, random_state=config["seed"]
         )
     else:
         data_valid = loads_json(config["data"]["valid"])
 
     # Create Datasets
     train_dataset = T5NERDataset(
-        data=data_train,
-        instructions=instructions["train"],
-        options=options
+        data=data_train, instructions=instructions["train"], options=options
     )
 
     valid_dataset = T5NERDataset(
-        data=data_valid,
-        instructions=instructions["test"],
-        options=options
+        data=data_valid, instructions=instructions["test"], options=options
     )
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     print(f"Using device: {device}")
 
     # load model
     tokenizer = T5Tokenizer.from_pretrained(config["model"]["name"])
@@ -122,15 +121,15 @@
         device=device,
         eval_every_n_batches=eval_every_n_batches,
         pred_every_n_batches=pred_every_n_batches,
         generation_kwargs=generation_kwargs,
         options=options,
         path_to_save_model=path_to_save_best_checkpoint.as_posix(),
         metric_name_to_choose_best=config["training"]["metric_name"],
-        metric_avg_to_choose_best=config["training"]["metric_avg"]
+        metric_avg_to_choose_best=config["training"]["metric_avg"],
     )
 
     path_to_save_model_last = path_to_save_trained_model / "last"
     path_to_save_model_last.mkdir(exist_ok=True)
 
     model.save_pretrained(path_to_save_trained_model)
     tokenizer.save_pretrained(path_to_save_trained_model)
```

### Comparing `instruction_ner-0.1.3/instruction_ner/utils/evaluate_utils.py` & `instruction_ner-0.1.6/instruction_ner/utils/evaluate_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import json
 import random
-from typing import List, Dict, Any, Optional
+from typing import Any, Dict, List, Optional
 
 import pandas as pd
 import torch
 from torch.utils.tensorboard import SummaryWriter
 from tqdm import tqdm
 from transformers import T5ForConditionalGeneration, T5Tokenizer
 
-from instruction_ner.metrics import calculate_metrics
 from instruction_ner.formatters.PredictionSpan import PredictionSpanFormatter
+from instruction_ner.metrics import calculate_metrics
 
 prediction_span_formatter = PredictionSpanFormatter()
 
 
 def evaluate(
-        model: T5ForConditionalGeneration,
-        tokenizer: T5Tokenizer,
-        dataloader: torch.utils.data.DataLoader,
-        writer: Optional[SummaryWriter],
-        device: torch.device,
-        generation_kwargs: Dict[str, Any],
-        epoch: int,
-        options: List[str]
+    model: T5ForConditionalGeneration,
+    tokenizer: T5Tokenizer,
+    dataloader: torch.utils.data.DataLoader,
+    writer: Optional[SummaryWriter],
+    device: torch.device,
+    generation_kwargs: Dict[str, Any],
+    epoch: int,
+    options: List[str],
 ):
     model.eval()
 
     epoch_loss = []
 
     spans_true = []
     spans_pred = []
 
     with torch.no_grad():
         for i, inputs in tqdm(
-                enumerate(dataloader),
-                total=len(dataloader),
-                desc="Evaluating",
+            enumerate(dataloader),
+            total=len(dataloader),
+            desc="Evaluating",
         ):
 
             instances = inputs.pop("instances")
             contexts = [instance.context for instance in instances]
             spans_true_batch = [instance.entity_spans for instance in instances]
             spans_true.extend(spans_true_batch)
 
@@ -51,58 +51,60 @@
 
             inputs.to(device)
             answers = answers.to(device)
             outputs = model(**inputs, labels=answers)
             loss = outputs.loss
 
             prediction_texts = model.generate(**inputs, **generation_kwargs)
-            prediction_texts = tokenizer.batch_decode(prediction_texts, skip_special_tokens=True)
+            prediction_texts = tokenizer.batch_decode(
+                prediction_texts, skip_special_tokens=True
+            )
             if writer:
                 writer.add_text("sample_prediction", prediction_texts[0])
 
-            spans_pred_batch = [prediction_span_formatter.format_answer_spans(context, prediction, options)
-                                for context, prediction in zip(contexts, prediction_texts)]
+            spans_pred_batch = [
+                prediction_span_formatter.format_answer_spans(
+                    context, prediction, options
+                )
+                for context, prediction in zip(contexts, prediction_texts)
+            ]
             spans_pred.extend(spans_pred_batch)
 
             batch_metrics = calculate_metrics(
-                spans_pred_batch,
-                spans_true_batch,
-                options=options
+                spans_pred_batch, spans_true_batch, options=options
             )
 
             if writer:
                 for metric_class, metric_dict in batch_metrics.items():
-                    writer.add_scalars(metric_class, metric_dict, epoch * len(dataloader) + i)
+                    writer.add_scalars(
+                        metric_class, metric_dict, epoch * len(dataloader) + i
+                    )
 
             epoch_loss.append(loss.item())
 
             if writer:
                 writer.add_scalar(
                     "batch loss / evaluation", loss.item(), epoch * len(dataloader) + i
                 )
 
-        epoch_metrics = calculate_metrics(
-            spans_pred,
-            spans_true,
-            options=options
-        )
+        epoch_metrics = calculate_metrics(spans_pred, spans_true, options=options)
 
         show_classification_report(epoch_metrics)
 
         return epoch_metrics
 
 
 def get_sample_text_prediction(
-        model: T5ForConditionalGeneration,
-        dataloader: torch.utils.data.DataLoader,
-        tokenizer: T5Tokenizer,
-        generation_kwargs,
-        device: str,
-        options: List[str],
-        n: int = 3
+    model: T5ForConditionalGeneration,
+    dataloader: torch.utils.data.DataLoader,
+    tokenizer: T5Tokenizer,
+    generation_kwargs,
+    device: str,
+    options: List[str],
+    n: int = 3,
 ):
     """
     Generate sample N predictions
     :param model:
     :param dataloader:
     :param tokenizer:
     :param generation_kwargs: arguments for generation process
@@ -120,38 +122,39 @@
     for _id in ids_to_pick:
         dataset_item = dataset[_id]
 
         print(f"Input: {dataset_item.context}")
         print(f"{dataset_item.question}")
 
         input_ids = tokenizer(
-            [dataset_item.context], [dataset_item.question], return_tensors="pt").input_ids
+            [dataset_item.context], [dataset_item.question], return_tensors="pt"
+        ).input_ids
 
         input_ids = input_ids.to(device)
         answer = model.generate(input_ids, **generation_kwargs)
-        answer = tokenizer.decode(answer[0], skip_special_tokens=True)  # TODO change to false
+        answer = tokenizer.decode(
+            answer[0], skip_special_tokens=True
+        )  # TODO change to false
 
         answer_spans = prediction_span_formatter.format_answer_spans(
-            context=dataset_item.context,
-            prediction=answer,
-            options=options
+            context=dataset_item.context, prediction=answer, options=options
         )
 
         print(f"Prediction: {answer}")
         print(f"Found {len(answer_spans)} spans. {answer_spans}\n")
 
 
 def update_best_checkpoint(
-        metrics_new: Dict[str, Dict[str, float]],
-        metrics_best: Dict[str, Dict[str, float]],
-        metric_name: str,
-        metric_avg: str,
-        model: T5ForConditionalGeneration,
-        tokenizer: T5Tokenizer,
-        path_to_save_model: str
+    metrics_new: Dict[str, Dict[str, float]],
+    metrics_best: Dict[str, Dict[str, float]],
+    metric_name: str,
+    metric_avg: str,
+    model: T5ForConditionalGeneration,
+    tokenizer: T5Tokenizer,
+    path_to_save_model: Optional[str],
 ):
     """
     Compares specific metric in two metric dictionaries: current and best.
     If new metric value is better -> new best model checkpoint saved
     :param metrics_new:
     :param metrics_best:
     :param metric_name:
@@ -160,27 +163,32 @@
     :param tokenizer:
     :param path_to_save_model:
     :return:
     """
 
     metric_current_value = metrics_new[metric_avg][metric_name]
 
-    metric_best_value = 0
+    metric_best_value = 0.0
     if len(metrics_best) > 0:
         metric_best_value = metrics_best[metric_avg][metric_name]
 
     if metric_current_value > metric_best_value:
-        print(f"Got Better results for {metric_name}. \n"
-              f"{metric_current_value} > {metric_best_value}. Updating the best checkpoint")
+        print(
+            f"Got Better results for {metric_name}. \n"
+            f"{metric_current_value} > {metric_best_value}. Updating the best checkpoint"
+        )
         metrics_best = metrics_new
 
         model.save_pretrained(path_to_save_model)
         tokenizer.save_pretrained(path_to_save_model)
 
-        save_metrics_path = path_to_save_model + "/metrics.json"
+        if path_to_save_model is not None:
+            save_metrics_path = path_to_save_model + "/metrics.json"
+        else:
+            save_metrics_path = "metrics.json"
 
         with open(save_metrics_path, "w", encoding="utf-8") as f:
             json.dump(metrics_best, ensure_ascii=False, indent=4, fp=f)
 
     return metrics_best
```

### Comparing `instruction_ner-0.1.3/instruction_ner/utils/train_utils.py` & `instruction_ner-0.1.6/instruction_ner/utils/train_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-from typing import List, Dict, Any, Optional
+from typing import Any, Dict, List, Optional
 
 import numpy as np
 import torch
 from torch.utils.tensorboard import SummaryWriter
 from tqdm import tqdm
 from transformers import T5ForConditionalGeneration, T5Tokenizer
 
-from instruction_ner.utils.evaluate_utils import evaluate, get_sample_text_prediction, update_best_checkpoint
+from instruction_ner.utils.evaluate_utils import (
+    evaluate,
+    get_sample_text_prediction,
+    update_best_checkpoint,
+)
 
 
 def train(
-        n_epochs: int,
-        model: T5ForConditionalGeneration,
-        tokenizer: T5Tokenizer,
-        train_dataloader: torch.utils.data.DataLoader,
-        test_dataloader: torch.utils.data.DataLoader,
-        optimizer: torch.optim.Optimizer,
-        writer: Optional[SummaryWriter],
-        device: torch.device,
-        eval_every_n_batches: int,
-        pred_every_n_batches: int,
-        generation_kwargs: Dict[str, Any],
-        options: List[str],
-        path_to_save_model: Optional[str],
-        metric_name_to_choose_best: Optional[str],
-        metric_avg_to_choose_best: Optional[str]
+    n_epochs: int,
+    model: T5ForConditionalGeneration,
+    tokenizer: T5Tokenizer,
+    train_dataloader: torch.utils.data.DataLoader,
+    test_dataloader: torch.utils.data.DataLoader,
+    optimizer: torch.optim.Optimizer,
+    writer: Optional[SummaryWriter],
+    device: torch.device,
+    eval_every_n_batches: int,
+    pred_every_n_batches: int,
+    generation_kwargs: Dict[str, Any],
+    options: List[str],
+    path_to_save_model: Optional[str],
+    metric_name_to_choose_best: str = "f1-score",
+    metric_avg_to_choose_best: str = "weighted",
 ) -> None:
 
-    metrics_best = {}
+    metrics_best: Dict[str, Dict[str, float]] = {}
 
     for epoch in range(n_epochs):
         print(f"Epoch [{epoch + 1} / {n_epochs}]\n")
 
         metrics_best = train_epoch(
             model=model,
             tokenizer=tokenizer,
@@ -44,60 +48,59 @@
             eval_every_n_batches=eval_every_n_batches,
             pred_every_n_batches=pred_every_n_batches,
             generation_kwargs=generation_kwargs,
             options=options,
             path_to_save_model=path_to_save_model,
             metrics_best=metrics_best,
             metric_name_to_choose_best=metric_name_to_choose_best,
-            metric_avg_to_choose_best=metric_avg_to_choose_best
+            metric_avg_to_choose_best=metric_avg_to_choose_best,
         )
 
         evaluate_metrics = evaluate(
             model=model,
             tokenizer=tokenizer,
             dataloader=test_dataloader,
             writer=writer,
             device=device,
             epoch=epoch,
             generation_kwargs=generation_kwargs,
-            options=options
+            options=options,
         )
 
         if path_to_save_model is None:
             continue
 
         metrics_best = update_best_checkpoint(
             metrics_best=metrics_best,
             metrics_new=evaluate_metrics,
             metric_name=metric_name_to_choose_best,
             metric_avg=metric_avg_to_choose_best,
             model=model,
             tokenizer=tokenizer,
-            path_to_save_model=path_to_save_model
+            path_to_save_model=path_to_save_model,
         )
 
 
 def train_epoch(
-        model: T5ForConditionalGeneration,
-        tokenizer: T5Tokenizer,
-        train_dataloader: torch.utils.data.DataLoader,
-        optimizer: torch.optim.Optimizer,
-        writer: Optional[SummaryWriter],
-        device: torch.device,
-        epoch: int,
-        eval_every_n_batches: int,
-        pred_every_n_batches: int,
-        generation_kwargs: Dict[str, Any],
-        options: List[str],
-        path_to_save_model: Optional[str],
-        metrics_best: Dict[str, Dict[str, float]],
-        metric_name_to_choose_best: Optional[str],
-        metric_avg_to_choose_best: Optional[str],
-        test_dataloader: torch.utils.data.DataLoader = None,
-
+    model: T5ForConditionalGeneration,
+    tokenizer: T5Tokenizer,
+    train_dataloader: torch.utils.data.DataLoader,
+    optimizer: torch.optim.Optimizer,
+    writer: Optional[SummaryWriter],
+    device: torch.device,
+    epoch: int,
+    eval_every_n_batches: int,
+    pred_every_n_batches: int,
+    generation_kwargs: Dict[str, Any],
+    options: List[str],
+    path_to_save_model: Optional[str],
+    metrics_best: Dict[str, Dict[str, float]],
+    metric_name_to_choose_best: str = "f1-score",
+    metric_avg_to_choose_best: str = "weighted",
+    test_dataloader: torch.utils.data.DataLoader = None,
 ) -> Dict[str, Dict[str, float]]:
     """
     One training cycle (loop).
     Args:
         :param metric_avg_to_choose_best:
         :param metric_name_to_choose_best:
         :param metrics_best:
@@ -115,17 +118,17 @@
         :param device: cpu or cuda
         :param tokenizer:
     """
 
     epoch_loss = []
 
     for i, inputs in tqdm(
-            enumerate(train_dataloader),
-            total=len(train_dataloader),
-            desc="Training",
+        enumerate(train_dataloader),
+        total=len(train_dataloader),
+        desc="Training",
     ):
         model.train()
         optimizer.zero_grad()
 
         inputs.pop("instances")
         answers = inputs.pop("answers")
 
@@ -152,35 +155,35 @@
                     model=model,
                     tokenizer=tokenizer,
                     dataloader=test_dataloader,
                     writer=writer,
                     device=device,
                     epoch=epoch,
                     generation_kwargs=generation_kwargs,
-                    options=options
+                    options=options,
                 )
 
                 metrics_best = update_best_checkpoint(
                     metrics_best=metrics_best,
                     metrics_new=evaluate_metrics,
                     metric_name=metric_name_to_choose_best,
                     metric_avg=metric_avg_to_choose_best,
                     model=model,
                     tokenizer=tokenizer,
-                    path_to_save_model=path_to_save_model
+                    path_to_save_model=path_to_save_model,
                 )
 
         if i % pred_every_n_batches == 0 and i >= pred_every_n_batches:
             get_sample_text_prediction(
                 model=model,
                 tokenizer=tokenizer,
                 dataloader=test_dataloader,
                 device=device,
                 generation_kwargs=generation_kwargs,
-                options=options
+                options=options,
             )
 
     avg_loss = np.mean(epoch_loss)
     print(f"Train loss: {avg_loss}\n")
     if writer:
         writer.add_scalar("loss / train", avg_loss, epoch)
```

### Comparing `instruction_ner-0.1.3/instruction_ner/utils/utils.py` & `instruction_ner-0.1.6/instruction_ner/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import configparser
 import json
-from pathlib import Path
 import random
+from pathlib import Path
+from typing import Union
 
 import numpy as np
 import torch
 import yaml
 
 
 def set_global_seed(seed: int):
@@ -19,15 +20,15 @@
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
     torch.backends.cudnn.benchmark = False
     torch.backends.cudnn.deterministic = True
 
 
-def load_config(config_file: str) -> configparser.ConfigParser:
+def load_config(config_file: Union[str, Path]) -> configparser.ConfigParser:
     """
     Load configuration file.
     :param str config_file: location of configuration file.
     :return: config.
     :rtype: configparser.ConfigParser
     """
 
@@ -37,21 +38,22 @@
         raise FileNotFoundError(
             f"Config file not found at path '{config_file.absolute()}'. "
             "Please, create it if it doesn't exist"
         )
 
     if config_file.suffix == ".ini":
         config = configparser.ConfigParser()
-        config.read(str(config_file), encoding='utf-8')
-    elif config_file.suffix in {'.yaml', '.yml'}:
-        config = yaml.safe_load(open(config_file, encoding='utf-8'))
+        config.read(str(config_file), encoding="utf-8")
+    elif config_file.suffix in {".yaml", ".yml"}:
+        config = yaml.safe_load(open(config_file, encoding="utf-8"))
     else:
         raise NotImplementedError(
             f"Not implemented reading from '{config_file.suffix}' files. "
-            f"Current file path is '{config_file.absolute()}'")
+            f"Current file path is '{config_file.absolute()}'"
+        )
 
     return config
 
 
 def loads_json(filepath: str):
     """
     Load json file
```

### Comparing `instruction_ner-0.1.3/instruction_ner.egg-info/PKG-INFO` & `instruction_ner-0.1.6/instruction_ner.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,190 +1,193 @@
 Metadata-Version: 2.1
 Name: instruction-ner
-Version: 0.1.3
+Version: 0.1.6
 Summary: Unofficial implementation of InstructionNER
 Home-page: https://github.com/ovbystrova/InstructionNER
 Author: Olga Bystrova
 Author-email: bystrovaolgavl@gmail.com
-License: UNKNOWN
-Description: # InstructionNER: A Multi-Task Instruction-Based Generative Framework for Few-shot NER
-        
-        [![tests](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml/badge.svg)](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml)
-        [![codecov](https://codecov.io/gh/ovbystrova/InstructionNER/branch/main/graph/badge.svg?token=L2OOZKLPJL)](https://codecov.io/gh/ovbystrova/InstructionNER)
-        [![python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/ovbystrova/InstructionNER#requirements)
-        [![license](https://img.shields.io/github/license/ovbystrova/InstructionNER?color=blue)](https://github.com/ovbystrova/InstructionNER/blob/main/LICENSE)
-        
-        Unofficial implementation of [InstructionNER](https://arxiv.org/pdf/2203.03903v1.pdf).
-        
-        ![Screenshot](resources/overall_intro.jpg)
-        
-        ## Requirements
-        Python >=3.8
-        
-        ## Installation
-        ```shell
-        pip install instruction-ner
-        ```
-        
-        (Alternative via requirements)
-        ```shell
-        pip install -r requirements/requirements.in # for training purposes
-        pip install -r requirements/requirements_test.in # for tests
-        pip install -r requirements/requirements_dev.in # for inference only
-        ```
-        
-        ## Data Preparation
-        In order to make a unified training interface, 
-        you can convert your raw input data (supported dataset formats: **conll**, **spacy**, **mit**)
-        with the following script:
-        ```
-        instruction_ner-prepare-data \
-        --path_to_file 'data/conll2003/train.txt' \
-        --dataset_type 'conll2003' \
-        --output_folder 'data/conll2003' \
-        ```
-        
-        This script converts every dataset to a list of sentences.
-        Every sentence is like this:
-        ```
-        {
-            "context": "SOCCER - JAPAN GET LUCKY WIN , CHINA IN SURPRISE DEFEAT .",
-            "entity_values": {
-                    "LOC": [
-                        "JAPAN"
-                    ],
-                    "PER": [
-                        "CHINA"
-                    ]
-                },
-            "entity_spans": [
-                    {
-                        "start": 9,
-                        "end": 14,
-                        "label": "LOC"
-                    },
-                    {
-                        "start": 31,
-                        "end": 36,
-                        "label": "PER"
-                    }
-                ]
-        }
-        ```
-        
-        ## Training
-        Script for training T5 model:
-        ```
-        instruction_ner-train \
-        --path_to_instructions 'instructions.json' \
-        --path_to_options 'options.json' \
-        --log_dir 'runs/test_run' \
-        --eval_every_n_batches 200 \
-        --pred_every_n_batches 200 \
-        --path_to_model_config 'config.yaml' \
-        --path_to_model_save 'runs/model/' \
-        ```
-        
-        Arguments:
-        - **--path_to_instructions** - file with instruction prompts
-        - **--path_to_options** - file with mapping dataset to its entities
-        - **--log_dir** - where to log tensorboard
-        - **--eval_every_n_batches** - do evaluation every n batches
-        - **--pred_every_n_batches** - write n sample prediction every n batches
-        - **--path_to_model_config** - path to all necessary information for model
-        - **--path_to_model_save** - where to save model
-        
-        ## Evaluation
-        Script for evaluation of the trained model:
-        ```
-        instruction_ner-evaluate \
-        --model_path_or_name 'olgaduchovny/t5-base-qa-ner-conll' \
-        --path_to_model_config 'config.yaml' \
-        --path_to_instructions 'instructions.json' \
-        --path_to_options 'options.json' \
-        ```
-        
-        Arguments:
-        - **--model_path_or_name** - path to trained model or HF model name
-        - **--path_to_model_config** - path to all necessary information for model
-        - **--path_to_instructions** - file with instruction prompts
-        - **--path_to_options** - file with mapping dataset to its entities
-        
-        ## Evaluation Results
-        
-        
-        
-        Dataset | Precision | Recall | F1-Score (weighted)
-        --- | --- | --- | --- | 
-        CONLL-2003 | 0.862 | 0.843 | 0.852 
-        MIT MOVIE | 0.792 | 0.845 | 0.809 | 
-        MIT REST | 0.766 | 0.771 | 0.768 | 
-        
-        ## Prediction Sample
-        ```
-        Sentence: The protest , which attracted several thousand supporters , coincided with the 18th anniversary of Spain 's constitution .
-        Instruction: please extract entities and their types from the input sentence, all entity types are in options
-        Options: ORG, PER, LOC
-        
-        Prediction (raw text): Spain is a LOC.
-        ```
-        ## Inference 
-        
-        ### Models
-        [t5-base-ner-conll](https://huggingface.co/olgaduchovny/t5-base-ner-conll)
-        
-        [t5-base-ner-mit-restaurant](https://huggingface.co/olgaduchovny/t5-base-ner-mit-restaurant)
-        
-        [t5-base-ner-mit-movie](https://huggingface.co/olgaduchovny/t5-base-ner-mit-movie)
-        
-        ### Code
-        ```python
-        from instruction_ner.model import Model
-        
-        model = Model(
-            model_path_or_name="olgaduchovny/t5-base-ner-conll",
-            tokenizer_path_or_name="olgaduchovny/t5-base-ner-conll"
-        )
-        
-        options = ["LOC", "PER", "ORG", "MISC"]
-        
-        instruction = "please extract entities and their types from the input sentence, " \
-                      "all entity types are in options"
-        
-        text = "My name is Olga. I am 24 years old. I live in Moscow and work at Sber AI Center as a Senior NLP Data Scientist." \
-                "This is my reporitory to test generative NER problem with T5 model."
-        
-        generation_kwargs = {
-            "num_beams": 2,
-            "max_length": 128
-        }
-        
-        pred_text, pred_spans = model.predict(
-            text=text,
-            generation_kwargs=generation_kwargs,
-            instruction=instruction,
-            options=options
-        )
-        
-        >>> ('Olga is a PER, Moscow is a LOC, Sber AI Center is an ORG, NLP is a MISC.',
-         [(11, 15, 'PER'), (46, 52, 'LOC'), (65, 79, 'ORG'), (92, 95, 'MISC')])
-        ```
-        
-        
-        
-        # Citation
-        ```bibtex
-        @article{wang2022instructionner,
-          title={Instructionner: A multi-task instruction-based generative framework for few-shot ner},
-          author={Wang, Liwen and Li, Rumei and Yan, Yang and Yan, Yuanmeng and Wang, Sirui and Wu, Wei and Xu, Weiran},
-          journal={arXiv preprint arXiv:2203.03903},
-          year={2022}
-        }
-        ```
-        
 Keywords: python,nlp,deep learning,ner,t5
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# InstructionNER: A Multi-Task Instruction-Based Generative Framework for Few-shot NER
+
+[![python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/ovbystrova/InstructionNER#requirements)
+[![license](https://img.shields.io/github/license/ovbystrova/InstructionNER?color=blue)](https://github.com/ovbystrova/InstructionNER/blob/main/LICENSE)
+[![pypi version](https://img.shields.io/pypi/v/instruction_ner)](https://pypi.org/project/instruction_ner)
+[![pypi downloads](https://img.shields.io/pypi/dm/instruction_ner)](https://pypi.org/project/instruction_ner)
+
+
+[![tests](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml/badge.svg)](https://github.com/ovbystrova/InstructionNER/actions/workflows/tests.yml)
+[![codecov](https://codecov.io/gh/ovbystrova/InstructionNER/branch/main/graph/badge.svg?token=L2OOZKLPJL)](https://codecov.io/gh/ovbystrova/InstructionNER)
+
+Unofficial implementation of [InstructionNER](https://arxiv.org/pdf/2203.03903v1.pdf).
+
+![Screenshot](resources/overall_intro.jpg)
+
+## Requirements
+Python >=3.8
+
+## Installation
+```shell
+pip install instruction-ner
+```
+
+(Alternative via requirements)
+```shell
+pip install -r requirements/requirements.in # for training purposes
+pip install -r requirements/requirements_test.in # for tests
+pip install -r requirements/requirements_dev.in # for inference only
+```
+
+## Data Preparation
+In order to make a unified training interface,
+you can convert your raw input data (supported dataset formats: **conll**, **spacy**, **mit**)
+with the following script:
+```
+instruction_ner-prepare-data \
+--path_to_file 'data/conll2003/train.txt' \
+--dataset_type 'conll2003' \
+--output_folder 'data/conll2003' \
+```
+
+This script converts every dataset to a list of sentences.
+Every sentence is like this:
+```
+{
+    "context": "SOCCER - JAPAN GET LUCKY WIN , CHINA IN SURPRISE DEFEAT .",
+    "entity_values": {
+            "LOC": [
+                "JAPAN"
+            ],
+            "PER": [
+                "CHINA"
+            ]
+        },
+    "entity_spans": [
+            {
+                "start": 9,
+                "end": 14,
+                "label": "LOC"
+            },
+            {
+                "start": 31,
+                "end": 36,
+                "label": "PER"
+            }
+        ]
+}
+```
+
+## Training
+Script for training T5 model:
+```
+instruction_ner-train \
+--path_to_instructions 'instructions.json' \
+--path_to_options 'options.json' \
+--log_dir 'runs/test_run' \
+--eval_every_n_batches 200 \
+--pred_every_n_batches 200 \
+--path_to_model_config 'config.yaml' \
+--path_to_model_save 'runs/model/' \
+```
+
+Arguments:
+- **--path_to_instructions** - file with instruction prompts
+- **--path_to_options** - file with mapping dataset to its entities
+- **--log_dir** - where to log tensorboard
+- **--eval_every_n_batches** - do evaluation every n batches
+- **--pred_every_n_batches** - write n sample prediction every n batches
+- **--path_to_model_config** - path to all necessary information for model
+- **--path_to_model_save** - where to save model
+
+## Evaluation
+Script for evaluation of the trained model:
+```
+instruction_ner-evaluate \
+--model_path_or_name 'olgaduchovny/t5-base-qa-ner-conll' \
+--path_to_model_config 'config.yaml' \
+--path_to_instructions 'instructions.json' \
+--path_to_options 'options.json' \
+```
+
+Arguments:
+- **--model_path_or_name** - path to trained model or HF model name
+- **--path_to_model_config** - path to all necessary information for model
+- **--path_to_instructions** - file with instruction prompts
+- **--path_to_options** - file with mapping dataset to its entities
+
+## Evaluation Results
+
+
+
+Dataset | Precision | Recall | F1-Score (weighted)
+--- | --- | --- | --- |
+CONLL-2003 | 0.862 | 0.843 | 0.852
+MIT MOVIE | 0.792 | 0.845 | 0.809 |
+MIT REST | 0.766 | 0.771 | 0.768 |
+
+## Prediction Sample
+```
+Sentence: The protest , which attracted several thousand supporters , coincided with the 18th anniversary of Spain 's constitution .
+Instruction: please extract entities and their types from the input sentence, all entity types are in options
+Options: ORG, PER, LOC
+
+Prediction (raw text): Spain is a LOC.
+```
+## Inference
+
+### Models
+[t5-base-ner-conll](https://huggingface.co/olgaduchovny/t5-base-ner-conll)
+
+[t5-base-ner-mit-restaurant](https://huggingface.co/olgaduchovny/t5-base-ner-mit-restaurant)
+
+[t5-base-ner-mit-movie](https://huggingface.co/olgaduchovny/t5-base-ner-mit-movie)
+
+### Code
+```python
+from instruction_ner.model import Model
+
+model = Model(
+    model_path_or_name="olgaduchovny/t5-base-ner-conll",
+    tokenizer_path_or_name="olgaduchovny/t5-base-ner-conll"
+)
+
+options = ["LOC", "PER", "ORG", "MISC"]
+
+instruction = "please extract entities and their types from the input sentence, " \
+              "all entity types are in options"
+
+text = "My name is Olga. I am 24 years old. I live in Moscow and work at Sber AI Center as a Senior NLP Data Scientist." \
+        "This is my reporitory to test generative NER problem with T5 model."
+
+generation_kwargs = {
+    "num_beams": 2,
+    "max_length": 128
+}
+
+pred_text, pred_spans = model.predict(
+    text=text,
+    generation_kwargs=generation_kwargs,
+    instruction=instruction,
+    options=options
+)
+
+>>> ('Olga is a PER, Moscow is a LOC, Sber AI Center is an ORG, NLP is a MISC.',
+ [(11, 15, 'PER'), (46, 52, 'LOC'), (65, 79, 'ORG'), (92, 95, 'MISC')])
+```
+
+
+
+# Citation
+```bibtex
+@article{wang2022instructionner,
+  title={Instructionner: A multi-task instruction-based generative framework for few-shot ner},
+  author={Wang, Liwen and Li, Rumei and Yan, Yang and Yan, Yuanmeng and Wang, Sirui and Wu, Wei and Xu, Weiran},
+  journal={arXiv preprint arXiv:2203.03903},
+  year={2022}
+}
+```
```

### Comparing `instruction_ner-0.1.3/setup.py` & `instruction_ner-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 from instruction_ner import __version__
 
 with open("README.md", mode="r", encoding="utf-8") as fp:
     long_description = fp.read()
 
 setup(
@@ -26,19 +26,20 @@
     install_requires=[
         "dataclasses==0.6",
         "openpyxl==3.0.10",
         "pandas==1.4.3",
         "pyyaml==6.0",
         "SentencePiece==0.1.96",
         "scikit-learn==1.1.2",
-        "torch==1.12.0",
+        "torch==1.13.1",
         "tensorboard==2.9.1",
-        "transformers==4.3.3"
+        "tokenizers==0.13.2",
+        "transformers==4.27.1",
     ],
     keywords=["python", "nlp", "deep learning", "ner", "t5"],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
-        "Intended Audience :: Developers"
-    ]
+        "Intended Audience :: Developers",
+    ],
 )
```

