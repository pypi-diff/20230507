# Comparing `tmp/instruction_ner-0.1.2.tar.gz` & `tmp/instruction_ner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instruction_ner-0.1.2.tar", last modified: Tue Aug 30 18:49:40 2022, max compression
+gzip compressed data, was "instruction_ner-0.1.3.tar", last modified: Tue Aug 30 18:57:46 2022, max compression
```

## Comparing `instruction_ner-0.1.2.tar` & `instruction_ner-0.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:49:40.625909 instruction_ner-0.1.2/
--rw-r--r--   0 a18692338   (503) staff       (20)     1070 2022-06-30 19:45:07.000000 instruction_ner-0.1.2/LICENSE
--rw-r--r--   0 a18692338   (503) staff       (20)     7446 2022-08-30 18:49:40.626243 instruction_ner-0.1.2/PKG-INFO
--rw-r--r--   0 a18692338   (503) staff       (20)     5499 2022-08-30 18:17:32.000000 instruction_ner-0.1.2/README.md
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:49:40.590263 instruction_ner-0.1.2/instruction_ner/
--rw-r--r--   0 a18692338   (503) staff       (20)       22 2022-08-21 16:56:51.000000 instruction_ner-0.1.2/instruction_ner/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     3096 2022-08-20 11:34:42.000000 instruction_ner-0.1.2/instruction_ner/arg_parse.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1294 2022-07-18 19:04:43.000000 instruction_ner-0.1.2/instruction_ner/collator.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:49:40.596247 instruction_ner-0.1.2/instruction_ner/core/
--rw-r--r--   0 a18692338   (503) staff       (20)        0 2022-07-01 18:48:22.000000 instruction_ner-0.1.2/instruction_ner/core/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1914 2022-08-18 17:17:06.000000 instruction_ner-0.1.2/instruction_ner/core/datatypes.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1981 2022-07-24 14:04:16.000000 instruction_ner-0.1.2/instruction_ner/core/reader.py
--rw-r--r--   0 a18692338   (503) staff       (20)     3636 2022-07-18 19:04:43.000000 instruction_ner-0.1.2/instruction_ner/dataset.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1937 2022-08-21 16:44:42.000000 instruction_ner-0.1.2/instruction_ner/evaluate.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:49:40.598838 instruction_ner-0.1.2/instruction_ner/formatters/
--rw-r--r--   0 a18692338   (503) staff       (20)     1950 2022-07-18 19:04:43.000000 instruction_ner-0.1.2/instruction_ner/formatters/Answer.py
--rw-r--r--   0 a18692338   (503) staff       (20)     2630 2022-07-18 19:04:43.000000 instruction_ner-0.1.2/instruction_ner/formatters/PredictionSpan.py
--rw-r--r--   0 a18692338   (503) staff       (20)      470 2022-07-18 19:04:43.000000 instruction_ner-0.1.2/instruction_ner/formatters/__init__.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:49:40.606934 instruction_ner-0.1.2/instruction_ner/formatters/instances/
--rw-r--r--   0 a18692338   (503) staff       (20)     1267 2022-07-18 19:06:01.000000 instruction_ner-0.1.2/instruction_ner/formatters/instances/EntityExtractTask.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1487 2022-07-18 19:06:01.000000 instruction_ner-0.1.2/instruction_ner/formatters/instances/EntityTypeTask.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1236 2022-07-18 19:06:01.000000 instruction_ner-0.1.2/instruction_ner/formatters/instances/NERTask.py
--rw-r--r--   0 a18692338   (503) staff       (20)      978 2022-07-18 19:05:34.000000 instruction_ner-0.1.2/instruction_ner/formatters/instances/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     8292 2022-07-18 19:04:43.000000 instruction_ner-0.1.2/instruction_ner/metrics.py
--rw-r--r--   0 a18692338   (503) staff       (20)     2287 2022-08-18 18:58:38.000000 instruction_ner-0.1.2/instruction_ner/model.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1219 2022-08-30 18:26:30.000000 instruction_ner-0.1.2/instruction_ner/prepare_data.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:49:40.615786 instruction_ner-0.1.2/instruction_ner/readers/
--rw-r--r--   0 a18692338   (503) staff       (20)      228 2022-08-06 12:26:30.000000 instruction_ner-0.1.2/instruction_ner/readers/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     6696 2022-08-20 11:34:42.000000 instruction_ner-0.1.2/instruction_ner/readers/conll.py
--rw-r--r--   0 a18692338   (503) staff       (20)     5375 2022-08-06 12:26:30.000000 instruction_ner-0.1.2/instruction_ner/readers/mit.py
--rw-r--r--   0 a18692338   (503) staff       (20)     3685 2022-07-24 14:04:16.000000 instruction_ner-0.1.2/instruction_ner/readers/spacy.py
--rw-r--r--   0 a18692338   (503) staff       (20)     4331 2022-08-21 16:44:42.000000 instruction_ner-0.1.2/instruction_ner/train.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:49:40.624854 instruction_ner-0.1.2/instruction_ner/utils/
--rw-r--r--   0 a18692338   (503) staff       (20)        0 2022-08-30 18:12:23.000000 instruction_ner-0.1.2/instruction_ner/utils/__init__.py
--rw-r--r--   0 a18692338   (503) staff       (20)     6046 2022-08-20 11:34:42.000000 instruction_ner-0.1.2/instruction_ner/utils/evaluate_utils.py
--rw-r--r--   0 a18692338   (503) staff       (20)     6259 2022-08-30 18:31:20.000000 instruction_ner-0.1.2/instruction_ner/utils/train_utils.py
--rw-r--r--   0 a18692338   (503) staff       (20)     1773 2022-08-20 11:34:42.000000 instruction_ner-0.1.2/instruction_ner/utils/utils.py
-drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:49:40.594613 instruction_ner-0.1.2/instruction_ner.egg-info/
--rw-r--r--   0 a18692338   (503) staff       (20)     7446 2022-08-30 18:49:40.000000 instruction_ner-0.1.2/instruction_ner.egg-info/PKG-INFO
--rw-r--r--   0 a18692338   (503) staff       (20)     1225 2022-08-30 18:49:40.000000 instruction_ner-0.1.2/instruction_ner.egg-info/SOURCES.txt
--rw-r--r--   0 a18692338   (503) staff       (20)        1 2022-08-30 18:49:40.000000 instruction_ner-0.1.2/instruction_ner.egg-info/dependency_links.txt
--rw-r--r--   0 a18692338   (503) staff       (20)      192 2022-08-30 18:49:40.000000 instruction_ner-0.1.2/instruction_ner.egg-info/entry_points.txt
--rw-r--r--   0 a18692338   (503) staff       (20)      155 2022-08-30 18:49:40.000000 instruction_ner-0.1.2/instruction_ner.egg-info/requires.txt
--rw-r--r--   0 a18692338   (503) staff       (20)       16 2022-08-30 18:49:40.000000 instruction_ner-0.1.2/instruction_ner.egg-info/top_level.txt
--rw-r--r--   0 a18692338   (503) staff       (20)      131 2022-08-30 18:49:40.627179 instruction_ner-0.1.2/setup.cfg
--rw-r--r--   0 a18692338   (503) staff       (20)     1221 2022-08-30 18:28:02.000000 instruction_ner-0.1.2/setup.py
+drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.843344 instruction_ner-0.1.3/
+-rw-r--r--   0 a18692338   (503) staff       (20)     1070 2022-06-30 19:45:07.000000 instruction_ner-0.1.3/LICENSE
+-rw-r--r--   0 a18692338   (503) staff       (20)     7446 2022-08-30 18:57:46.844481 instruction_ner-0.1.3/PKG-INFO
+-rw-r--r--   0 a18692338   (503) staff       (20)     5499 2022-08-30 18:17:32.000000 instruction_ner-0.1.3/README.md
+drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.816715 instruction_ner-0.1.3/instruction_ner/
+-rw-r--r--   0 a18692338   (503) staff       (20)       22 2022-08-30 18:57:25.000000 instruction_ner-0.1.3/instruction_ner/__init__.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     3096 2022-08-20 11:34:42.000000 instruction_ner-0.1.3/instruction_ner/arg_parse.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     1294 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/collator.py
+drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.822660 instruction_ner-0.1.3/instruction_ner/core/
+-rw-r--r--   0 a18692338   (503) staff       (20)        0 2022-07-01 18:48:22.000000 instruction_ner-0.1.3/instruction_ner/core/__init__.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     1914 2022-08-18 17:17:06.000000 instruction_ner-0.1.3/instruction_ner/core/datatypes.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     1981 2022-07-24 14:04:16.000000 instruction_ner-0.1.3/instruction_ner/core/reader.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     3636 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/dataset.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     1937 2022-08-21 16:44:42.000000 instruction_ner-0.1.3/instruction_ner/evaluate.py
+drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.827373 instruction_ner-0.1.3/instruction_ner/formatters/
+-rw-r--r--   0 a18692338   (503) staff       (20)     1950 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/formatters/Answer.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     2630 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/formatters/PredictionSpan.py
+-rw-r--r--   0 a18692338   (503) staff       (20)      470 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/formatters/__init__.py
+drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.832327 instruction_ner-0.1.3/instruction_ner/formatters/instances/
+-rw-r--r--   0 a18692338   (503) staff       (20)     1267 2022-07-18 19:06:01.000000 instruction_ner-0.1.3/instruction_ner/formatters/instances/EntityExtractTask.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     1487 2022-07-18 19:06:01.000000 instruction_ner-0.1.3/instruction_ner/formatters/instances/EntityTypeTask.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     1236 2022-07-18 19:06:01.000000 instruction_ner-0.1.3/instruction_ner/formatters/instances/NERTask.py
+-rw-r--r--   0 a18692338   (503) staff       (20)      978 2022-07-18 19:05:34.000000 instruction_ner-0.1.3/instruction_ner/formatters/instances/__init__.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     8292 2022-07-18 19:04:43.000000 instruction_ner-0.1.3/instruction_ner/metrics.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     2287 2022-08-18 18:58:38.000000 instruction_ner-0.1.3/instruction_ner/model.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     1219 2022-08-30 18:26:30.000000 instruction_ner-0.1.3/instruction_ner/prepare_data.py
+drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.837315 instruction_ner-0.1.3/instruction_ner/readers/
+-rw-r--r--   0 a18692338   (503) staff       (20)      228 2022-08-06 12:26:30.000000 instruction_ner-0.1.3/instruction_ner/readers/__init__.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     6696 2022-08-20 11:34:42.000000 instruction_ner-0.1.3/instruction_ner/readers/conll.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     5375 2022-08-06 12:26:30.000000 instruction_ner-0.1.3/instruction_ner/readers/mit.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     3685 2022-07-24 14:04:16.000000 instruction_ner-0.1.3/instruction_ner/readers/spacy.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     4331 2022-08-21 16:44:42.000000 instruction_ner-0.1.3/instruction_ner/train.py
+drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.841215 instruction_ner-0.1.3/instruction_ner/utils/
+-rw-r--r--   0 a18692338   (503) staff       (20)        0 2022-08-30 18:12:23.000000 instruction_ner-0.1.3/instruction_ner/utils/__init__.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     6046 2022-08-20 11:34:42.000000 instruction_ner-0.1.3/instruction_ner/utils/evaluate_utils.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     6259 2022-08-30 18:31:20.000000 instruction_ner-0.1.3/instruction_ner/utils/train_utils.py
+-rw-r--r--   0 a18692338   (503) staff       (20)     1773 2022-08-20 11:34:42.000000 instruction_ner-0.1.3/instruction_ner/utils/utils.py
+drwxr-xr-x   0 a18692338   (503) staff       (20)        0 2022-08-30 18:57:46.820223 instruction_ner-0.1.3/instruction_ner.egg-info/
+-rw-r--r--   0 a18692338   (503) staff       (20)     7446 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/PKG-INFO
+-rw-r--r--   0 a18692338   (503) staff       (20)     1225 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/SOURCES.txt
+-rw-r--r--   0 a18692338   (503) staff       (20)        1 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/dependency_links.txt
+-rw-r--r--   0 a18692338   (503) staff       (20)      192 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/entry_points.txt
+-rw-r--r--   0 a18692338   (503) staff       (20)      155 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/requires.txt
+-rw-r--r--   0 a18692338   (503) staff       (20)       16 2022-08-30 18:57:46.000000 instruction_ner-0.1.3/instruction_ner.egg-info/top_level.txt
+-rw-r--r--   0 a18692338   (503) staff       (20)      131 2022-08-30 18:57:46.845394 instruction_ner-0.1.3/setup.cfg
+-rw-r--r--   0 a18692338   (503) staff       (20)     1426 2022-08-30 18:56:26.000000 instruction_ner-0.1.3/setup.py
```

### Comparing `instruction_ner-0.1.2/LICENSE` & `instruction_ner-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/PKG-INFO` & `instruction_ner-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instruction_ner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unofficial implementation of InstructionNER
 Home-page: https://github.com/ovbystrova/InstructionNER
 Author: Olga Bystrova
 Author-email: bystrovaolgavl@gmail.com
 License: UNKNOWN
 Description: # InstructionNER: A Multi-Task Instruction-Based Generative Framework for Few-shot NER
```

### Comparing `instruction_ner-0.1.2/README.md` & `instruction_ner-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/arg_parse.py` & `instruction_ner-0.1.3/instruction_ner/arg_parse.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/collator.py` & `instruction_ner-0.1.3/instruction_ner/collator.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/core/datatypes.py` & `instruction_ner-0.1.3/instruction_ner/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/core/reader.py` & `instruction_ner-0.1.3/instruction_ner/core/reader.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/dataset.py` & `instruction_ner-0.1.3/instruction_ner/dataset.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/evaluate.py` & `instruction_ner-0.1.3/instruction_ner/evaluate.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/formatters/Answer.py` & `instruction_ner-0.1.3/instruction_ner/formatters/Answer.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/formatters/PredictionSpan.py` & `instruction_ner-0.1.3/instruction_ner/formatters/PredictionSpan.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/formatters/instances/EntityExtractTask.py` & `instruction_ner-0.1.3/instruction_ner/formatters/instances/EntityExtractTask.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/formatters/instances/EntityTypeTask.py` & `instruction_ner-0.1.3/instruction_ner/formatters/instances/EntityTypeTask.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/formatters/instances/NERTask.py` & `instruction_ner-0.1.3/instruction_ner/formatters/instances/NERTask.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/formatters/instances/__init__.py` & `instruction_ner-0.1.3/instruction_ner/formatters/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/metrics.py` & `instruction_ner-0.1.3/instruction_ner/metrics.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/model.py` & `instruction_ner-0.1.3/instruction_ner/model.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/prepare_data.py` & `instruction_ner-0.1.3/instruction_ner/prepare_data.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/readers/conll.py` & `instruction_ner-0.1.3/instruction_ner/readers/conll.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/readers/mit.py` & `instruction_ner-0.1.3/instruction_ner/readers/mit.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/readers/spacy.py` & `instruction_ner-0.1.3/instruction_ner/readers/spacy.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/train.py` & `instruction_ner-0.1.3/instruction_ner/train.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/utils/evaluate_utils.py` & `instruction_ner-0.1.3/instruction_ner/utils/evaluate_utils.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/utils/train_utils.py` & `instruction_ner-0.1.3/instruction_ner/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner/utils/utils.py` & `instruction_ner-0.1.3/instruction_ner/utils/utils.py`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/instruction_ner.egg-info/PKG-INFO` & `instruction_ner-0.1.3/instruction_ner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instruction-ner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unofficial implementation of InstructionNER
 Home-page: https://github.com/ovbystrova/InstructionNER
 Author: Olga Bystrova
 Author-email: bystrovaolgavl@gmail.com
 License: UNKNOWN
 Description: # InstructionNER: A Multi-Task Instruction-Based Generative Framework for Few-shot NER
```

### Comparing `instruction_ner-0.1.2/instruction_ner.egg-info/SOURCES.txt` & `instruction_ner-0.1.3/instruction_ner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instruction_ner-0.1.2/setup.py` & `instruction_ner-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,15 +19,25 @@
     entry_points={
         "console_scripts": [
             "instruction_ner-prepare-data = instruction_ner.prepare_data:main",
             "instruction_ner-train = instruction_ner.train:main",
             "instruction_ner-evaluate = instruction_ner.evaluate:main",
         ],
     },
-    install_requires=open("./requirements/requirements.in", "r").readlines(),
+    install_requires=[
+        "dataclasses==0.6",
+        "openpyxl==3.0.10",
+        "pandas==1.4.3",
+        "pyyaml==6.0",
+        "SentencePiece==0.1.96",
+        "scikit-learn==1.1.2",
+        "torch==1.12.0",
+        "tensorboard==2.9.1",
+        "transformers==4.3.3"
+    ],
     keywords=["python", "nlp", "deep learning", "ner", "t5"],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers"
     ]
```

