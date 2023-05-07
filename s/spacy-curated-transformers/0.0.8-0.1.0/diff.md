# Comparing `tmp/spacy-curated-transformers-0.0.8.tar.gz` & `tmp/spacy-curated-transformers-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-curated-transformers-0.0.8.tar", last modified: Fri May  5 11:57:30 2023, max compression
+gzip compressed data, was "spacy-curated-transformers-0.1.0.tar", last modified: Sun May  7 10:23:44 2023, max compression
```

## Comparing `spacy-curated-transformers-0.0.8.tar` & `spacy-curated-transformers-0.1.0.tar`

### file list

```diff
@@ -1,76 +1,82 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.436277 spacy-curated-transformers-0.0.8/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1088 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)      101 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/MANIFEST.in
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1285 2023-05-05 11:57:30.436277 spacy-curated-transformers-0.0.8/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      960 2023-05-04 14:55:43.000000 spacy-curated-transformers-0.0.8/README.md
--rw-r--r--   0 daniel    (1000) daniel    (1000)      102 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4230 2023-05-05 11:57:30.436277 spacy-curated-transformers-0.0.8/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      210 2023-05-04 14:53:41.000000 spacy-curated-transformers-0.0.8/setup.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.431277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       41 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/_compat.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.432277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/cli/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/cli/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4050 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/cli/debug_pieces.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4697 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/cli/quantize.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4694 2023-05-04 14:55:43.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/errors.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.433277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      438 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    24297 2023-05-04 15:20:41.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/architectures.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1225 2023-05-04 15:07:44.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/hf_loader.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    19182 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/listeners.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2704 2023-05-04 15:20:41.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/output.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4016 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/pooling.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2192 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/remove_eos_bos.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4669 2023-05-04 15:07:44.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/scalar_weight.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2271 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/types.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7876 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/with_non_ws_tokens.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10279 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/with_strided_spans.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.433277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/pipeline/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       37 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/pipeline/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17299 2023-05-04 14:55:43.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/pipeline/transformer.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.433277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2222 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/conftest.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.434277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3177 2023-05-04 15:22:08.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2644 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_listeners.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4556 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_pooling.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1425 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_scalar_weight.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6181 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_transformer_model.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3194 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4325 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_with_strided_spans.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.434277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/pipeline/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/pipeline/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17414 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/pipeline/test_transformer.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      418 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/test_cli_app.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      794 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/test_torchscript_wrapper.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.435277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3393 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4090 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1365 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_registry.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2761 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7943 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4861 2023-05-04 15:02:55.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      482 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/util.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.436277 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      568 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3612 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/bbpe_encoder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3713 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/char_encoder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5394 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/hf_loader.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2500 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3823 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      557 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/types.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5890 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/wordpiece_encoder.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2711 2023-05-04 13:58:59.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers/util.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-05 11:57:30.431277 spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1285 2023-05-05 11:57:30.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3146 2023-05-05 11:57:30.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-05 11:57:30.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3466 2023-05-05 11:57:30.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       91 2023-05-05 11:57:30.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       27 2023-05-05 11:57:30.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-05 11:57:30.000000 spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      960 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-05-07 10:23:44.589398 spacy-curated-transformers-0.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      210 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.577397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/debug_pieces.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/quantize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3433 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24297 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1225 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2704 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/output.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/remove_eos_bos.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4669 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17299 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/pipeline/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2222 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3177 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2644 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4556 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1425 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6181 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3194 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4325 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17414 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/test_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
+-rw-r--r--   0 vsts      (1001) docker     (122)      418 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/test_torchscript_wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3393 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4090 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1365 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2761 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7943 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4861 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy-chars.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.585398 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3612 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3823 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5890 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-05-07 10:23:34.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-07 10:23:44.581397 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3507 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     3466 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       91 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-07 10:23:44.000000 spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/zip-safe
```

### Comparing `spacy-curated-transformers-0.0.8/LICENSE` & `spacy-curated-transformers-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/PKG-INFO` & `spacy-curated-transformers-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-curated-transformers
-Version: 0.0.8
+Version: 0.1.0
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/spacy-curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `spacy-curated-transformers-0.0.8/README.md` & `spacy-curated-transformers-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/setup.cfg` & `spacy-curated-transformers-0.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.8
+version = 0.1.0
 description = Curated transformer models
 url = https://github.com/explosion/spacy-curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/_compat.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/cli/debug_pieces.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/debug_pieces.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/cli/quantize.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/cli/quantize.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/errors.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,30 @@
 class ErrorsWithCodes(type):
     def __getattribute__(self, code):
         msg = super().__getattribute__(code)
         if code.startswith("__"):  # python system attributes like __class__
             return msg
         else:
-            return "(spacy-curated-transformers) [{code}] {msg}".format(code=code, msg=msg)
+            return "(spacy-curated-transformers) [{code}] {msg}".format(
+                code=code, msg=msg
+            )
 
 
 # fmt: off
 
 class Warnings(metaclass=ErrorsWithCodes):
     W001 = ("Skipping transfomer pipe with TorchScript model - Model "
             "is likely already quantized")
 
 
 class Errors(metaclass=ErrorsWithCodes):
     E001 = ("Attempting to quantize a transformer pipe with a "
             "non-PyTorch model ('{model_name}'). Quantization "
             "is only supported by PyTorch-specific curated "
             "transformer models")
-    E002 = ("The number of hidden layers ({num_hidden_layers}) in the "
-            "ALBERT encoder must be divisable by number of hidden groups "
-            "({num_hidden_groups})")
-    E003 = ("The hidden width of the transformer ({hidden_width}) must be "
-            "divisible by the number of self-attention heads ({num_heads})")
-    E004 = ("The point-wise feed-forward network in the transformer only "
-            "supports the following activation functions: {activation_funcs}")
-    E007 = ("Attempting to load the weights of an unsupported Hugging "
-            "Face `transformers` model ({unsupported_model}). Currently "
-            "supported models: {supported_models}")
-    E008 = ("The number of layers in the scalar weighting listener model ({num_layers_scalar_weight})"
-            "needs to be the same as the number of hidden layers in the "
-            "transformer ({num_layers_transformer}). You can use the config's "
-            "interpolation functionality to link the former's `num_layers` "
-            "parameter with the latter")
     E009 = ("At least one sequence in the transformer's input has a length "
             "of {seq_len}, which is larger than the model's maximum sequence "
             "length of {max_seq_len} tokens")
     E010 = ("Curated transformers do not currently support listener replacement")
     E011 = ("`{loader_name}` requires the Hugging Face `transformers` package to be installed")
     E012 = ("`{listener_name}` requires the upstream transformer pipe to output "
             "all hidden layer outputs. This can be enabled by setting the pipe's "
@@ -65,12 +52,9 @@
             "{supported_tokenizers}")
     E023 = ("Japanese BERT models currently only support character subword encoding")
     E024 = ("Attempting to initialize an incompatible piece encoder ('{model_name}') "
             "with the Hugging Face Japanese BERT tokenizer. It can only be used with the "
             "`CharEncoder` piece encoder")
     E025 = ("Attempting to perform gradual unfreezing of a non-transformer pipe "
             "('{pipe_name}'}. Only transformer pipes support this feature")
-    E026 = ("Attempting to load the weights of a Hugging Face `transformers` model "
-            "into an unsupported curated encoder ({unsupported_encoder}). Currently "
-            "supported encoders: {supported_encoders}")
 
 # fmt: on
```

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/architectures.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/architectures.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/hf_loader.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/hf_loader.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/listeners.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/listeners.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/output.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/pooling.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/remove_eos_bos.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/remove_eos_bos.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/scalar_weight.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/types.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/with_non_ws_tokens.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/models/with_strided_spans.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/models/with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/pipeline/transformer.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/pipeline/transformer.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/conftest.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_hf_model.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_hf_model.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_listeners.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_listeners.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_pooling.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_scalar_weight.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_transformer_model.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/models/test_with_strided_spans.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/models/test_with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/pipeline/test_transformer.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/pipeline/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/test_torchscript_wrapper.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/test_torchscript_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_char_encoder.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_registry.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_registry.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/__init__.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/bbpe_encoder.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/char_encoder.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/hf_loader.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/hf_loader.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/sentencepiece_adapters.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/sentencepiece_adapters.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/sentencepiece_encoder.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/types.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/tokenization/wordpiece_encoder.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/tokenization/wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers/util.py` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers/util.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/PKG-INFO` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-curated-transformers
-Version: 0.0.8
+Version: 0.1.0
 Summary: Curated transformer models
 Home-page: https://github.com/explosion/spacy-curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/SOURCES.txt` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,27 @@
 spacy_curated_transformers/tests/models/test_pooling.py
 spacy_curated_transformers/tests/models/test_scalar_weight.py
 spacy_curated_transformers/tests/models/test_transformer_model.py
 spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
 spacy_curated_transformers/tests/models/test_with_strided_spans.py
 spacy_curated_transformers/tests/pipeline/__init__.py
 spacy_curated_transformers/tests/pipeline/test_transformer.py
+spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
 spacy_curated_transformers/tests/tokenization/__init__.py
 spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
 spacy_curated_transformers/tests/tokenization/test_char_encoder.py
 spacy_curated_transformers/tests/tokenization/test_registry.py
 spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
 spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
 spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
+spacy_curated_transformers/tests/tokenization/toy-chars.txt
+spacy_curated_transformers/tests/tokenization/toy-merges.txt
+spacy_curated_transformers/tests/tokenization/toy-vocab.json
+spacy_curated_transformers/tests/tokenization/toy.model
+spacy_curated_transformers/tests/tokenization/toy.wordpieces
 spacy_curated_transformers/tokenization/__init__.py
 spacy_curated_transformers/tokenization/bbpe_encoder.py
 spacy_curated_transformers/tokenization/char_encoder.py
 spacy_curated_transformers/tokenization/hf_loader.py
 spacy_curated_transformers/tokenization/sentencepiece_adapters.py
 spacy_curated_transformers/tokenization/sentencepiece_encoder.py
 spacy_curated_transformers/tokenization/types.py
```

### Comparing `spacy-curated-transformers-0.0.8/spacy_curated_transformers.egg-info/entry_points.txt` & `spacy-curated-transformers-0.1.0/spacy_curated_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

