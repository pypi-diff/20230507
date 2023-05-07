# Comparing `tmp/evalplus-0.1.1.tar.gz` & `tmp/evalplus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalplus-0.1.1.tar", last modified: Fri May  5 23:53:54 2023, max compression
+gzip compressed data, was "evalplus-0.1.2.tar", last modified: Sun May  7 04:56:48 2023, max compression
```

## Comparing `evalplus-0.1.1.tar` & `evalplus-0.1.2.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3246 2023-05-05 23:34:50.000000 evalplus-0.1.1/.gitignore
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      458 2023-04-28 04:50:47.000000 evalplus-0.1.1/.pre-commit-config.yaml
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1221 2023-05-05 20:32:21.000000 evalplus-0.1.1/CITATION.cff
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    11357 2023-04-16 19:02:05.000000 evalplus-0.1.1/LICENSE
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       39 2023-05-05 20:10:56.000000 evalplus-0.1.1/MANIFEST.in
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5562 2023-05-05 23:53:54.877694 evalplus-0.1.1/PKG-INFO
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5115 2023-05-05 23:49:45.000000 evalplus-0.1.1/README.md
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.873694 evalplus-0.1.1/codegen/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5512 2023-05-05 07:50:38.000000 evalplus-0.1.1/codegen/generate.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    22452 2023-05-04 22:42:14.000000 evalplus-0.1.1/codegen/model.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.873694 evalplus-0.1.1/evalplus/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      120 2023-05-05 20:05:00.000000 evalplus-0.1.1/evalplus/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      160 2023-05-05 23:53:54.000000 evalplus-0.1.1/evalplus/_version.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/evalplus/data/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7130 2023-05-05 23:35:22.000000 evalplus-0.1.1/evalplus/data/__init__.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/evalplus/eval/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6818 2023-05-05 23:35:22.000000 evalplus-0.1.1/evalplus/eval/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     4021 2023-04-28 20:10:51.000000 evalplus-0.1.1/evalplus/eval/utils.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7383 2023-05-05 23:35:22.000000 evalplus-0.1.1/evalplus/evaluate.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/evalplus/gen/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      753 2023-04-28 21:16:13.000000 evalplus-0.1.1/evalplus/gen/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3046 2023-04-28 21:16:13.000000 evalplus-0.1.1/evalplus/gen/chatgpt_gen.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1052 2023-04-28 21:16:13.000000 evalplus-0.1.1/evalplus/gen/mut_gen.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    10484 2023-04-28 20:25:40.000000 evalplus-0.1.1/evalplus/gen/type_mut.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/evalplus/gen/util/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      722 2023-04-23 03:12:10.000000 evalplus-0.1.1/evalplus/gen/util/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1633 2023-04-28 19:25:35.000000 evalplus-0.1.1/evalplus/gen/util/api_request.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2614 2023-05-05 23:34:50.000000 evalplus-0.1.1/evalplus/inputgen.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/evalplus.egg-info/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5562 2023-05-05 23:53:54.000000 evalplus-0.1.1/evalplus.egg-info/PKG-INFO
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1108 2023-05-05 23:53:54.000000 evalplus-0.1.1/evalplus.egg-info/SOURCES.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        1 2023-05-05 23:53:54.000000 evalplus-0.1.1/evalplus.egg-info/dependency_links.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      104 2023-05-05 23:53:54.000000 evalplus-0.1.1/evalplus.egg-info/entry_points.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       91 2023-05-05 23:53:54.000000 evalplus-0.1.1/evalplus.egg-info/requires.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        9 2023-05-05 23:53:54.000000 evalplus-0.1.1/evalplus.egg-info/top_level.txt
--rwxrwxr-x   0 jiawei    (1002) jiawei    (1002)     1894 2023-05-05 23:34:50.000000 evalplus-0.1.1/evo.sh
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/gallary/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    96092 2023-05-02 00:08:40.000000 evalplus-0.1.1/gallary/overview.png
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   403455 2023-04-28 21:23:51.000000 evalplus-0.1.1/gallary/render.gif
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      246 2023-05-05 20:09:10.000000 evalplus-0.1.1/pyproject.toml
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       19 2023-05-05 07:23:28.000000 evalplus-0.1.1/requirements-llm.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       45 2023-05-05 23:33:51.000000 evalplus-0.1.1/requirements-tools.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       49 2023-05-05 23:26:08.000000 evalplus-0.1.1/requirements.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      845 2023-05-05 23:53:54.877694 evalplus-0.1.1/setup.cfg
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/tools/
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/tools/_experimental/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       33 2023-04-28 19:21:13.000000 evalplus-0.1.1/tools/_experimental/README.md
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3238 2023-05-05 23:34:50.000000 evalplus-0.1.1/tools/_experimental/set_cover.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2405 2023-05-05 23:34:50.000000 evalplus-0.1.1/tools/_experimental/topset_distill.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3413 2023-04-29 17:26:54.000000 evalplus-0.1.1/tools/checker.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1598 2023-05-05 23:34:50.000000 evalplus-0.1.1/tools/filter_inputs.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-05 23:53:54.877694 evalplus-0.1.1/tools/humaneval/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1099 2023-05-05 23:34:50.000000 evalplus-0.1.1/tools/humaneval/check_ground_truth.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3368 2023-05-05 23:34:50.000000 evalplus-0.1.1/tools/humaneval/init_plus.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      844 2023-04-28 20:27:45.000000 evalplus-0.1.1/tools/init_ground_truth.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1340 2023-04-28 20:52:24.000000 evalplus-0.1.1/tools/merge_dataset.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6089 2023-05-05 23:34:50.000000 evalplus-0.1.1/tools/render.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3739 2023-04-28 21:35:44.000000 evalplus-0.1.1/tools/sanitize.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      741 2023-05-05 23:34:50.000000 evalplus-0.1.1/tools/stat_plus.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6533 2023-05-01 07:40:47.000000 evalplus-0.1.1/tools/viz_passrate.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      917 2023-05-03 04:36:53.000000 evalplus-0.1.1/zipper.sh
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3272 2023-05-07 04:41:37.000000 evalplus-0.1.2/.dockerignore
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3246 2023-05-05 23:34:50.000000 evalplus-0.1.2/.gitignore
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      458 2023-04-28 04:50:47.000000 evalplus-0.1.2/.pre-commit-config.yaml
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1221 2023-05-05 20:32:21.000000 evalplus-0.1.2/CITATION.cff
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      290 2023-05-07 04:49:10.000000 evalplus-0.1.2/Dockerfile
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    11357 2023-04-16 19:02:05.000000 evalplus-0.1.2/LICENSE
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       39 2023-05-05 20:10:56.000000 evalplus-0.1.2/MANIFEST.in
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6603 2023-05-07 04:56:48.282388 evalplus-0.1.2/PKG-INFO
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6156 2023-05-07 04:56:35.000000 evalplus-0.1.2/README.md
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/codegen/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5512 2023-05-05 07:50:38.000000 evalplus-0.1.2/codegen/generate.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    22452 2023-05-04 22:42:14.000000 evalplus-0.1.2/codegen/model.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      120 2023-05-05 20:05:00.000000 evalplus-0.1.2/evalplus/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      160 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus/_version.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/data/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7130 2023-05-05 23:35:22.000000 evalplus-0.1.2/evalplus/data/__init__.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/eval/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6818 2023-05-05 23:35:22.000000 evalplus-0.1.2/evalplus/eval/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     4021 2023-04-28 20:10:51.000000 evalplus-0.1.2/evalplus/eval/utils.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7446 2023-05-06 01:17:43.000000 evalplus-0.1.2/evalplus/evaluate.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/gen/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      753 2023-04-28 21:16:13.000000 evalplus-0.1.2/evalplus/gen/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3046 2023-04-28 21:16:13.000000 evalplus-0.1.2/evalplus/gen/chatgpt_gen.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1052 2023-04-28 21:16:13.000000 evalplus-0.1.2/evalplus/gen/mut_gen.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    10484 2023-04-28 20:25:40.000000 evalplus-0.1.2/evalplus/gen/type_mut.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/gen/util/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      722 2023-04-23 03:12:10.000000 evalplus-0.1.2/evalplus/gen/util/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1633 2023-04-28 19:25:35.000000 evalplus-0.1.2/evalplus/gen/util/api_request.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2614 2023-05-05 23:34:50.000000 evalplus-0.1.2/evalplus/inputgen.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus.egg-info/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6603 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/PKG-INFO
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1133 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        1 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      104 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/entry_points.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       91 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/requires.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        9 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/top_level.txt
+-rwxrwxr-x   0 jiawei    (1002) jiawei    (1002)     1894 2023-05-05 23:34:50.000000 evalplus-0.1.2/evo.sh
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/gallary/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    96092 2023-05-02 00:08:40.000000 evalplus-0.1.2/gallary/overview.png
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   403455 2023-04-28 21:23:51.000000 evalplus-0.1.2/gallary/render.gif
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      246 2023-05-05 20:09:10.000000 evalplus-0.1.2/pyproject.toml
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       19 2023-05-05 07:23:28.000000 evalplus-0.1.2/requirements-llm.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       45 2023-05-05 23:33:51.000000 evalplus-0.1.2/requirements-tools.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       49 2023-05-05 23:26:08.000000 evalplus-0.1.2/requirements.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      845 2023-05-07 04:56:48.282388 evalplus-0.1.2/setup.cfg
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/tools/
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/tools/_experimental/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       33 2023-04-28 19:21:13.000000 evalplus-0.1.2/tools/_experimental/README.md
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3238 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/_experimental/set_cover.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2405 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/_experimental/topset_distill.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3413 2023-04-29 17:26:54.000000 evalplus-0.1.2/tools/checker.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1598 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/filter_inputs.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/tools/humaneval/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1099 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/humaneval/check_ground_truth.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3368 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/humaneval/init_plus.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      844 2023-04-28 20:27:45.000000 evalplus-0.1.2/tools/init_ground_truth.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1340 2023-04-28 20:52:24.000000 evalplus-0.1.2/tools/merge_dataset.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6089 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/render.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3739 2023-04-28 21:35:44.000000 evalplus-0.1.2/tools/sanitize.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      741 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/stat_plus.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6533 2023-05-01 07:40:47.000000 evalplus-0.1.2/tools/viz_passrate.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      917 2023-05-03 04:36:53.000000 evalplus-0.1.2/zipper.sh
```

### Comparing `evalplus-0.1.1/.gitignore` & `evalplus-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/CITATION.cff` & `evalplus-0.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/LICENSE` & `evalplus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/PKG-INFO` & `evalplus-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: evalplus
-Version: 0.1.1
-Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
-Home-page: https://github.com/evalplus/evalplus
-License: Apache-2.0
-Platform: any
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `EvalPlus(📖) => 📚`
 
 <p align="center">
     <a href="#-Quick-Start">🔥Quick Start</a> •
     <a href="#-Papers">📜Papers</a> •
     <a href="#-Useful-tools">🔨Useful tools</a> •
     <a href="#-Development">👷Development</a> •
@@ -82,26 +68,34 @@
 ]
 write_jsonl("samples.jsonl", samples)
 ```
 
 <details><summary>🤔 What is in a `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
-* "task_id" is the identifier string for the task
-* "entry_point": name of the function
-* "prompt" is the function signature with docstring
-+ "canonical_solution" is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
-+ "base_input" is the test inputs in original HumanEval
-+ "plus_input" is the test inputs brought by EvalPlus
+* `task_id` is the identifier string for the task
+* `entry_point` is name of the function
+* `prompt` is the function signature with docstring
++ `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
++ `base_input` is the test inputs in original HumanEval
++ `plus_input` is the test inputs brought by EvalPlus
 
 </div>
 </details>
 
 To evaluate the samples:
 
+You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
+
+```bash
+docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl
+```
+
+...Or if you want to try it locally regardless of the risks ⚠️:
+
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
 <details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
@@ -118,14 +112,34 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
+The output should be like (below is GPT-4 greedy decoding example):
+
+```
+Computing expected output...
+Expected outputs computed in 15.18s
+Reading samples...
+164it [00:04, 37.79it/s]
+Evaluating samples...
+100%|██████████████████████████████████████████| 164/164 [00:03<00:00, 44.75it/s]
+Base
+{'pass@1': 0.8841463414634146}
+Base + Extra
+{'pass@1': 0.75}
+```
+
+- `Base` is the `pass@k` for the original HumanEval
+- `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
+- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
+- A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
+
 ### MBPP+ (TBD)
 
 
 ## 📜 Papers
 
 Read our [**paper**](https://arxiv.org/abs/2305.01210) for more detailed findings!
```

#### html2text {}

```diff
@@ -1,14 +1,8 @@
-Metadata-Version: 2.1 Name: evalplus Version: 0.1.1 Summary: "EvalPlus for
-rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
-evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
-(ð) => ð`
+# `EvalPlus(ð) => ð`
   ð¥Quick_Start â¢ ðPapers â¢ ð¨Useful_tools â¢ ð·Development â¢
                               ðAcknowledgement
 > **Warning** >
   > > ð¨ Evaluating LLM-generated code over datasets with "3 test-cases" is
                            **NOT** enough! ð¨ > >
 To address this, we started the EvalPlus project -- a rigourous evaluation
 framework for LLM4Code that: + â¨ improves code benchmarks by adding up to
@@ -28,47 +22,60 @@
 need to implement the `generate_one_completion` function! ```python from
 evalplus.data import get_human_eval_plus, write_jsonl problems =
 get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
 (task_id=task_id, completion=generate_one_completion(problems[task_id]
 ["prompt"])) for task_id in problems for _ in range(num_samples_per_task) ]
 write_jsonl("samples.jsonl", samples) ``` ð¤ What is in a `problem`? :: click
 to expand ::
-* "task_id" is the identifier string for the task * "entry_point": name of the
-function * "prompt" is the function signature with docstring +
-"canonical_solution" is the ground-truth implementation (re-implemented to fix
-bugs in HumanEval) + "base_input" is the test inputs in original HumanEval +
-"plus_input" is the test inputs brought by EvalPlus
- To evaluate the samples: ```bash evalplus.evaluate --dataset humaneval --
-samples samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to
-expand ::
+* `task_id` is the identifier string for the task * `entry_point` is name of
+the function * `prompt` is the function signature with docstring +
+`canonical_solution` is the ground-truth implementation (re-implemented to fix
+bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
+`plus_input` is the test inputs brought by EvalPlus
+ To evaluate the samples: You are strongly recommended to use a sandbox such as
+[docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
+app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
+...Or if you want to try it locally regardless of the risks â ï¸: ```bash
+evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð¤ Want to
+use local GitHub repo? :: click to expand ::
 ```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
  â¨ï¸ More command-line flags:: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
- ### MBPP+ (TBD) ## ð Papers Read our [**paper**](https://arxiv.org/abs/
-2305.01210) for more detailed findings! ```bibtex @article{evalplus, title={Is
-Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large
-Language Models for Code Generation}, author={Jiawei Liu and Chunqiu Steven Xia
-and Yuyao Wang and Lingming Zhang}, journal={arXiv preprint arXiv:2305.01210},
-year={2023}, } ``` ## ð¨ Useful tools To use these tools, please first
-install the repository from GitHub: ```bash git clone https://github.com/
-evalplus/evalplus.git cd evalplus pip install -r requirements-tools.txt ``` ###
-Syntax checker for LLM-generated code Check LLM-produced code and answer the
-following questions: 1. Is the generation entirely done for all samples / all
-problems in the dataset? 2. Are LLM-generated code compilable? (if no,
-something could be wrong and you'd better check) ```shell python tools/
-checker.py --folder /path/to/[model]-[??]b_temp_[??] --dataset humaneval ```
-### Post code sanitizer LLM-generated code may contain some syntax errors. But
-some of them can be easily fixable by doing simple post-processing. This tool
-will make the LLM-generated code more clean/compilable by doing certain post-
-processing such as trimming with more magical EOFs and some garbage non-code
-tokens. ```shell python tools/sanitize.py --eof --folder /path/to/vicuna-
-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/vicuna-
-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to `rich` and LaTeX
-tables ```shell python tools/render.py --type /path/to/[model]-[??]b # NOTE: no
-`_temp_[??]` ``` ![](./gallary/render.gif) ### Perform test input generation
-from scratch (TBD) ## ð· Development Before you start: ```bash pip install
-pre-commit pre-commit install export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name
-convention - `evalplus` is the package name. - `${DATASET}_plus` is the name of
-dataset applied with `evalplus`. ## ð Acknowledgement - [HumanEval](https://
-github.com/openai/human-eval)
+ The output should be like (below is GPT-4 greedy decoding example): ```
+Computing expected output... Expected outputs computed in 15.18s Reading
+samples... 164it [00:04, 37.79it/s] Evaluating samples...
+100%|ââââââââââââââââââââââââââââââââââââââââââ|
+164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
+Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
+- `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
+- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be
+used - A cache file named like `samples_eval_results.jsonl` will be cached.
+Remove it to re-run the evaluation ### MBPP+ (TBD) ## ð Papers Read our
+[**paper**](https://arxiv.org/abs/2305.01210) for more detailed findings!
+```bibtex @article{evalplus, title={Is Your Code Generated by ChatGPT Really
+Correct? Rigorous Evaluation of Large Language Models for Code Generation},
+author={Jiawei Liu and Chunqiu Steven Xia and Yuyao Wang and Lingming Zhang},
+journal={arXiv preprint arXiv:2305.01210}, year={2023}, } ``` ## ð¨ Useful
+tools To use these tools, please first install the repository from GitHub:
+```bash git clone https://github.com/evalplus/evalplus.git cd evalplus pip
+install -r requirements-tools.txt ``` ### Syntax checker for LLM-generated code
+Check LLM-produced code and answer the following questions: 1. Is the
+generation entirely done for all samples / all problems in the dataset? 2. Are
+LLM-generated code compilable? (if no, something could be wrong and you'd
+better check) ```shell python tools/checker.py --folder /path/to/[model]-
+[??]b_temp_[??] --dataset humaneval ``` ### Post code sanitizer LLM-generated
+code may contain some syntax errors. But some of them can be easily fixable by
+doing simple post-processing. This tool will make the LLM-generated code more
+clean/compilable by doing certain post-processing such as trimming with more
+magical EOFs and some garbage non-code tokens. ```shell python tools/
+sanitize.py --eof --folder /path/to/vicuna-[??]b_temp_[??] # Sanitized code
+will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ### Render
+`pass@k` results to `rich` and LaTeX tables ```shell python tools/render.py --
+type /path/to/[model]-[??]b # NOTE: no `_temp_[??]` ``` ![](./gallary/
+render.gif) ### Perform test input generation from scratch (TBD) ## ð·
+Development Before you start: ```bash pip install pre-commit pre-commit install
+export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name convention - `evalplus` is
+the package name. - `${DATASET}_plus` is the name of dataset applied with
+`evalplus`. ## ð Acknowledgement - [HumanEval](https://github.com/openai/
+human-eval)
```

### Comparing `evalplus-0.1.1/README.md` & `evalplus-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: evalplus
+Version: 0.1.2
+Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
+Home-page: https://github.com/evalplus/evalplus
+License: Apache-2.0
+Platform: any
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `EvalPlus(📖) => 📚`
 
 <p align="center">
     <a href="#-Quick-Start">🔥Quick Start</a> •
     <a href="#-Papers">📜Papers</a> •
     <a href="#-Useful-tools">🔨Useful tools</a> •
     <a href="#-Development">👷Development</a> •
@@ -68,26 +82,34 @@
 ]
 write_jsonl("samples.jsonl", samples)
 ```
 
 <details><summary>🤔 What is in a `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
-* "task_id" is the identifier string for the task
-* "entry_point": name of the function
-* "prompt" is the function signature with docstring
-+ "canonical_solution" is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
-+ "base_input" is the test inputs in original HumanEval
-+ "plus_input" is the test inputs brought by EvalPlus
+* `task_id` is the identifier string for the task
+* `entry_point` is name of the function
+* `prompt` is the function signature with docstring
++ `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
++ `base_input` is the test inputs in original HumanEval
++ `plus_input` is the test inputs brought by EvalPlus
 
 </div>
 </details>
 
 To evaluate the samples:
 
+You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
+
+```bash
+docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl
+```
+
+...Or if you want to try it locally regardless of the risks ⚠️:
+
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
 <details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
@@ -104,14 +126,34 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
+The output should be like (below is GPT-4 greedy decoding example):
+
+```
+Computing expected output...
+Expected outputs computed in 15.18s
+Reading samples...
+164it [00:04, 37.79it/s]
+Evaluating samples...
+100%|██████████████████████████████████████████| 164/164 [00:03<00:00, 44.75it/s]
+Base
+{'pass@1': 0.8841463414634146}
+Base + Extra
+{'pass@1': 0.75}
+```
+
+- `Base` is the `pass@k` for the original HumanEval
+- `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
+- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
+- A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
+
 ### MBPP+ (TBD)
 
 
 ## 📜 Papers
 
 Read our [**paper**](https://arxiv.org/abs/2305.01210) for more detailed findings!
```

#### html2text {}

```diff
@@ -1,8 +1,14 @@
-# `EvalPlus(ð) => ð`
+Metadata-Version: 2.1 Name: evalplus Version: 0.1.2 Summary: "EvalPlus for
+rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
+evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
+(ð) => ð`
   ð¥Quick_Start â¢ ðPapers â¢ ð¨Useful_tools â¢ ð·Development â¢
                               ðAcknowledgement
 > **Warning** >
   > > ð¨ Evaluating LLM-generated code over datasets with "3 test-cases" is
                            **NOT** enough! ð¨ > >
 To address this, we started the EvalPlus project -- a rigourous evaluation
 framework for LLM4Code that: + â¨ improves code benchmarks by adding up to
@@ -22,47 +28,60 @@
 need to implement the `generate_one_completion` function! ```python from
 evalplus.data import get_human_eval_plus, write_jsonl problems =
 get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
 (task_id=task_id, completion=generate_one_completion(problems[task_id]
 ["prompt"])) for task_id in problems for _ in range(num_samples_per_task) ]
 write_jsonl("samples.jsonl", samples) ``` ð¤ What is in a `problem`? :: click
 to expand ::
-* "task_id" is the identifier string for the task * "entry_point": name of the
-function * "prompt" is the function signature with docstring +
-"canonical_solution" is the ground-truth implementation (re-implemented to fix
-bugs in HumanEval) + "base_input" is the test inputs in original HumanEval +
-"plus_input" is the test inputs brought by EvalPlus
- To evaluate the samples: ```bash evalplus.evaluate --dataset humaneval --
-samples samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to
-expand ::
+* `task_id` is the identifier string for the task * `entry_point` is name of
+the function * `prompt` is the function signature with docstring +
+`canonical_solution` is the ground-truth implementation (re-implemented to fix
+bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
+`plus_input` is the test inputs brought by EvalPlus
+ To evaluate the samples: You are strongly recommended to use a sandbox such as
+[docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
+app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
+...Or if you want to try it locally regardless of the risks â ï¸: ```bash
+evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð¤ Want to
+use local GitHub repo? :: click to expand ::
 ```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
  â¨ï¸ More command-line flags:: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
- ### MBPP+ (TBD) ## ð Papers Read our [**paper**](https://arxiv.org/abs/
-2305.01210) for more detailed findings! ```bibtex @article{evalplus, title={Is
-Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large
-Language Models for Code Generation}, author={Jiawei Liu and Chunqiu Steven Xia
-and Yuyao Wang and Lingming Zhang}, journal={arXiv preprint arXiv:2305.01210},
-year={2023}, } ``` ## ð¨ Useful tools To use these tools, please first
-install the repository from GitHub: ```bash git clone https://github.com/
-evalplus/evalplus.git cd evalplus pip install -r requirements-tools.txt ``` ###
-Syntax checker for LLM-generated code Check LLM-produced code and answer the
-following questions: 1. Is the generation entirely done for all samples / all
-problems in the dataset? 2. Are LLM-generated code compilable? (if no,
-something could be wrong and you'd better check) ```shell python tools/
-checker.py --folder /path/to/[model]-[??]b_temp_[??] --dataset humaneval ```
-### Post code sanitizer LLM-generated code may contain some syntax errors. But
-some of them can be easily fixable by doing simple post-processing. This tool
-will make the LLM-generated code more clean/compilable by doing certain post-
-processing such as trimming with more magical EOFs and some garbage non-code
-tokens. ```shell python tools/sanitize.py --eof --folder /path/to/vicuna-
-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/vicuna-
-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to `rich` and LaTeX
-tables ```shell python tools/render.py --type /path/to/[model]-[??]b # NOTE: no
-`_temp_[??]` ``` ![](./gallary/render.gif) ### Perform test input generation
-from scratch (TBD) ## ð· Development Before you start: ```bash pip install
-pre-commit pre-commit install export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name
-convention - `evalplus` is the package name. - `${DATASET}_plus` is the name of
-dataset applied with `evalplus`. ## ð Acknowledgement - [HumanEval](https://
-github.com/openai/human-eval)
+ The output should be like (below is GPT-4 greedy decoding example): ```
+Computing expected output... Expected outputs computed in 15.18s Reading
+samples... 164it [00:04, 37.79it/s] Evaluating samples...
+100%|ââââââââââââââââââââââââââââââââââââââââââ|
+164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
+Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
+- `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
+- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be
+used - A cache file named like `samples_eval_results.jsonl` will be cached.
+Remove it to re-run the evaluation ### MBPP+ (TBD) ## ð Papers Read our
+[**paper**](https://arxiv.org/abs/2305.01210) for more detailed findings!
+```bibtex @article{evalplus, title={Is Your Code Generated by ChatGPT Really
+Correct? Rigorous Evaluation of Large Language Models for Code Generation},
+author={Jiawei Liu and Chunqiu Steven Xia and Yuyao Wang and Lingming Zhang},
+journal={arXiv preprint arXiv:2305.01210}, year={2023}, } ``` ## ð¨ Useful
+tools To use these tools, please first install the repository from GitHub:
+```bash git clone https://github.com/evalplus/evalplus.git cd evalplus pip
+install -r requirements-tools.txt ``` ### Syntax checker for LLM-generated code
+Check LLM-produced code and answer the following questions: 1. Is the
+generation entirely done for all samples / all problems in the dataset? 2. Are
+LLM-generated code compilable? (if no, something could be wrong and you'd
+better check) ```shell python tools/checker.py --folder /path/to/[model]-
+[??]b_temp_[??] --dataset humaneval ``` ### Post code sanitizer LLM-generated
+code may contain some syntax errors. But some of them can be easily fixable by
+doing simple post-processing. This tool will make the LLM-generated code more
+clean/compilable by doing certain post-processing such as trimming with more
+magical EOFs and some garbage non-code tokens. ```shell python tools/
+sanitize.py --eof --folder /path/to/vicuna-[??]b_temp_[??] # Sanitized code
+will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ### Render
+`pass@k` results to `rich` and LaTeX tables ```shell python tools/render.py --
+type /path/to/[model]-[??]b # NOTE: no `_temp_[??]` ``` ![](./gallary/
+render.gif) ### Perform test input generation from scratch (TBD) ## ð·
+Development Before you start: ```bash pip install pre-commit pre-commit install
+export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name convention - `evalplus` is
+the package name. - `${DATASET}_plus` is the name of dataset applied with
+`evalplus`. ## ð Acknowledgement - [HumanEval](https://github.com/openai/
+human-eval)
```

### Comparing `evalplus-0.1.1/codegen/generate.py` & `evalplus-0.1.2/codegen/generate.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/codegen/model.py` & `evalplus-0.1.2/codegen/model.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/data/__init__.py` & `evalplus-0.1.2/evalplus/data/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/eval/__init__.py` & `evalplus-0.1.2/evalplus/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/eval/utils.py` & `evalplus-0.1.2/evalplus/eval/utils.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/evaluate.py` & `evalplus-0.1.2/evalplus/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,17 @@
 
         # sort the results for each problem by completion_id
         for task_id, task_results in eval_results.items():
             task_results.sort(key=lambda x: x["completion_id"])
             results["eval"][task_id] = {
                 "nfiles": len(task_results),
                 "base": [x["base"] for x in task_results],
-                "plus": [x["plus"] for x in task_results],
+                "plus": [x["plus"] for x in task_results]
+                if not flags.base_only
+                else [],
             }
 
     if os.path.isfile(result_path) and flags.i_just_wanna_run:
         decision = ""
         while decision.lower() not in ["y", "n"]:
             print(f"{result_path} already exists. Press [Y/N] to overwrite or exit...")
             decision = input()
```

### Comparing `evalplus-0.1.1/evalplus/gen/__init__.py` & `evalplus-0.1.2/evalplus/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/gen/chatgpt_gen.py` & `evalplus-0.1.2/evalplus/gen/chatgpt_gen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/gen/mut_gen.py` & `evalplus-0.1.2/evalplus/gen/mut_gen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/gen/type_mut.py` & `evalplus-0.1.2/evalplus/gen/type_mut.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/gen/util/__init__.py` & `evalplus-0.1.2/evalplus/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/gen/util/api_request.py` & `evalplus-0.1.2/evalplus/gen/util/api_request.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus/inputgen.py` & `evalplus-0.1.2/evalplus/inputgen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/evalplus.egg-info/PKG-INFO` & `evalplus-0.1.2/evalplus.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalplus
-Version: 0.1.1
+Version: 0.1.2
 Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
 Home-page: https://github.com/evalplus/evalplus
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -82,26 +82,34 @@
 ]
 write_jsonl("samples.jsonl", samples)
 ```
 
 <details><summary>🤔 What is in a `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
-* "task_id" is the identifier string for the task
-* "entry_point": name of the function
-* "prompt" is the function signature with docstring
-+ "canonical_solution" is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
-+ "base_input" is the test inputs in original HumanEval
-+ "plus_input" is the test inputs brought by EvalPlus
+* `task_id` is the identifier string for the task
+* `entry_point` is name of the function
+* `prompt` is the function signature with docstring
++ `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
++ `base_input` is the test inputs in original HumanEval
++ `plus_input` is the test inputs brought by EvalPlus
 
 </div>
 </details>
 
 To evaluate the samples:
 
+You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
+
+```bash
+docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl
+```
+
+...Or if you want to try it locally regardless of the risks ⚠️:
+
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
 <details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
@@ -118,14 +126,34 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
+The output should be like (below is GPT-4 greedy decoding example):
+
+```
+Computing expected output...
+Expected outputs computed in 15.18s
+Reading samples...
+164it [00:04, 37.79it/s]
+Evaluating samples...
+100%|██████████████████████████████████████████| 164/164 [00:03<00:00, 44.75it/s]
+Base
+{'pass@1': 0.8841463414634146}
+Base + Extra
+{'pass@1': 0.75}
+```
+
+- `Base` is the `pass@k` for the original HumanEval
+- `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
+- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
+- A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
+
 ### MBPP+ (TBD)
 
 
 ## 📜 Papers
 
 Read our [**paper**](https://arxiv.org/abs/2305.01210) for more detailed findings!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalplus Version: 0.1.1 Summary: "EvalPlus for
+Metadata-Version: 2.1 Name: evalplus Version: 0.1.2 Summary: "EvalPlus for
 rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
 evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
 (ð) => ð`
   ð¥Quick_Start â¢ ðPapers â¢ ð¨Useful_tools â¢ ð·Development â¢
@@ -28,47 +28,60 @@
 need to implement the `generate_one_completion` function! ```python from
 evalplus.data import get_human_eval_plus, write_jsonl problems =
 get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
 (task_id=task_id, completion=generate_one_completion(problems[task_id]
 ["prompt"])) for task_id in problems for _ in range(num_samples_per_task) ]
 write_jsonl("samples.jsonl", samples) ``` ð¤ What is in a `problem`? :: click
 to expand ::
-* "task_id" is the identifier string for the task * "entry_point": name of the
-function * "prompt" is the function signature with docstring +
-"canonical_solution" is the ground-truth implementation (re-implemented to fix
-bugs in HumanEval) + "base_input" is the test inputs in original HumanEval +
-"plus_input" is the test inputs brought by EvalPlus
- To evaluate the samples: ```bash evalplus.evaluate --dataset humaneval --
-samples samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to
-expand ::
+* `task_id` is the identifier string for the task * `entry_point` is name of
+the function * `prompt` is the function signature with docstring +
+`canonical_solution` is the ground-truth implementation (re-implemented to fix
+bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
+`plus_input` is the test inputs brought by EvalPlus
+ To evaluate the samples: You are strongly recommended to use a sandbox such as
+[docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
+app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
+...Or if you want to try it locally regardless of the risks â ï¸: ```bash
+evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð¤ Want to
+use local GitHub repo? :: click to expand ::
 ```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
  â¨ï¸ More command-line flags:: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
- ### MBPP+ (TBD) ## ð Papers Read our [**paper**](https://arxiv.org/abs/
-2305.01210) for more detailed findings! ```bibtex @article{evalplus, title={Is
-Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large
-Language Models for Code Generation}, author={Jiawei Liu and Chunqiu Steven Xia
-and Yuyao Wang and Lingming Zhang}, journal={arXiv preprint arXiv:2305.01210},
-year={2023}, } ``` ## ð¨ Useful tools To use these tools, please first
-install the repository from GitHub: ```bash git clone https://github.com/
-evalplus/evalplus.git cd evalplus pip install -r requirements-tools.txt ``` ###
-Syntax checker for LLM-generated code Check LLM-produced code and answer the
-following questions: 1. Is the generation entirely done for all samples / all
-problems in the dataset? 2. Are LLM-generated code compilable? (if no,
-something could be wrong and you'd better check) ```shell python tools/
-checker.py --folder /path/to/[model]-[??]b_temp_[??] --dataset humaneval ```
-### Post code sanitizer LLM-generated code may contain some syntax errors. But
-some of them can be easily fixable by doing simple post-processing. This tool
-will make the LLM-generated code more clean/compilable by doing certain post-
-processing such as trimming with more magical EOFs and some garbage non-code
-tokens. ```shell python tools/sanitize.py --eof --folder /path/to/vicuna-
-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/vicuna-
-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to `rich` and LaTeX
-tables ```shell python tools/render.py --type /path/to/[model]-[??]b # NOTE: no
-`_temp_[??]` ``` ![](./gallary/render.gif) ### Perform test input generation
-from scratch (TBD) ## ð· Development Before you start: ```bash pip install
-pre-commit pre-commit install export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name
-convention - `evalplus` is the package name. - `${DATASET}_plus` is the name of
-dataset applied with `evalplus`. ## ð Acknowledgement - [HumanEval](https://
-github.com/openai/human-eval)
+ The output should be like (below is GPT-4 greedy decoding example): ```
+Computing expected output... Expected outputs computed in 15.18s Reading
+samples... 164it [00:04, 37.79it/s] Evaluating samples...
+100%|ââââââââââââââââââââââââââââââââââââââââââ|
+164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
+Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
+- `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
+- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be
+used - A cache file named like `samples_eval_results.jsonl` will be cached.
+Remove it to re-run the evaluation ### MBPP+ (TBD) ## ð Papers Read our
+[**paper**](https://arxiv.org/abs/2305.01210) for more detailed findings!
+```bibtex @article{evalplus, title={Is Your Code Generated by ChatGPT Really
+Correct? Rigorous Evaluation of Large Language Models for Code Generation},
+author={Jiawei Liu and Chunqiu Steven Xia and Yuyao Wang and Lingming Zhang},
+journal={arXiv preprint arXiv:2305.01210}, year={2023}, } ``` ## ð¨ Useful
+tools To use these tools, please first install the repository from GitHub:
+```bash git clone https://github.com/evalplus/evalplus.git cd evalplus pip
+install -r requirements-tools.txt ``` ### Syntax checker for LLM-generated code
+Check LLM-produced code and answer the following questions: 1. Is the
+generation entirely done for all samples / all problems in the dataset? 2. Are
+LLM-generated code compilable? (if no, something could be wrong and you'd
+better check) ```shell python tools/checker.py --folder /path/to/[model]-
+[??]b_temp_[??] --dataset humaneval ``` ### Post code sanitizer LLM-generated
+code may contain some syntax errors. But some of them can be easily fixable by
+doing simple post-processing. This tool will make the LLM-generated code more
+clean/compilable by doing certain post-processing such as trimming with more
+magical EOFs and some garbage non-code tokens. ```shell python tools/
+sanitize.py --eof --folder /path/to/vicuna-[??]b_temp_[??] # Sanitized code
+will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ### Render
+`pass@k` results to `rich` and LaTeX tables ```shell python tools/render.py --
+type /path/to/[model]-[??]b # NOTE: no `_temp_[??]` ``` ![](./gallary/
+render.gif) ### Perform test input generation from scratch (TBD) ## ð·
+Development Before you start: ```bash pip install pre-commit pre-commit install
+export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name convention - `evalplus` is
+the package name. - `${DATASET}_plus` is the name of dataset applied with
+`evalplus`. ## ð Acknowledgement - [HumanEval](https://github.com/openai/
+human-eval)
```

### Comparing `evalplus-0.1.1/evalplus.egg-info/SOURCES.txt` & `evalplus-0.1.2/evalplus.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+.dockerignore
 .gitignore
 .pre-commit-config.yaml
 CITATION.cff
+Dockerfile
 LICENSE
 MANIFEST.in
 README.md
 evo.sh
 pyproject.toml
 requirements-llm.txt
 requirements-tools.txt
```

### Comparing `evalplus-0.1.1/evo.sh` & `evalplus-0.1.2/evo.sh`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/gallary/overview.png` & `evalplus-0.1.2/gallary/overview.png`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/gallary/render.gif` & `evalplus-0.1.2/gallary/render.gif`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/setup.cfg` & `evalplus-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/_experimental/set_cover.py` & `evalplus-0.1.2/tools/_experimental/set_cover.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/_experimental/topset_distill.py` & `evalplus-0.1.2/tools/_experimental/topset_distill.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/checker.py` & `evalplus-0.1.2/tools/checker.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/filter_inputs.py` & `evalplus-0.1.2/tools/filter_inputs.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/humaneval/check_ground_truth.py` & `evalplus-0.1.2/tools/humaneval/check_ground_truth.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/humaneval/init_plus.py` & `evalplus-0.1.2/tools/humaneval/init_plus.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/init_ground_truth.py` & `evalplus-0.1.2/tools/init_ground_truth.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/merge_dataset.py` & `evalplus-0.1.2/tools/merge_dataset.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/render.py` & `evalplus-0.1.2/tools/render.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/sanitize.py` & `evalplus-0.1.2/tools/sanitize.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/stat_plus.py` & `evalplus-0.1.2/tools/stat_plus.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/tools/viz_passrate.py` & `evalplus-0.1.2/tools/viz_passrate.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.1/zipper.sh` & `evalplus-0.1.2/zipper.sh`

 * *Files identical despite different names*

