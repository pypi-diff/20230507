# Comparing `tmp/ParMan-0.1.0.tar.gz` & `tmp/ParMan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParMan-0.1.0.tar", last modified: Tue May  2 19:56:13 2023, max compression
+gzip compressed data, was "ParMan-0.2.0.tar", last modified: Sun May  7 14:49:42 2023, max compression
```

## Comparing `ParMan-0.1.0.tar` & `ParMan-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,103 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-05-02 19:56:13.815308 ParMan-0.1.0/
--rw-r--r--   0 toon      (1000) toon      (1000)     7652 2017-09-30 07:16:26.000000 ParMan-0.1.0/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    12651 2023-05-02 19:56:13.815308 ParMan-0.1.0/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     2792 2023-05-02 19:25:43.000000 ParMan-0.1.0/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      991 2023-05-02 19:54:08.000000 ParMan-0.1.0/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-05-02 19:56:13.815308 ParMan-0.1.0/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-05-02 19:56:13.813308 ParMan-0.1.0/src/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-05-02 19:56:13.813308 ParMan-0.1.0/src/ParMan.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    12651 2023-05-02 19:56:13.000000 ParMan-0.1.0/src/ParMan.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      870 2023-05-02 19:56:13.000000 ParMan-0.1.0/src/ParMan.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-05-02 19:56:13.000000 ParMan-0.1.0/src/ParMan.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       20 2023-05-02 19:56:13.000000 ParMan-0.1.0/src/ParMan.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        7 2023-05-02 19:56:13.000000 ParMan-0.1.0/src/ParMan.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-05-02 19:56:13.814308 ParMan-0.1.0/src/parman/
--rw-r--r--   0 toon      (1000) toon      (1000)      799 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/__init__.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-05-02 19:56:13.814308 ParMan-0.1.0/src/parman/clerks/
--rw-r--r--   0 toon      (1000) toon      (1000)      842 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/clerks/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5121 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/clerks/base.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1859 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/clerks/local.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2888 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/clerks/localtemp.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4373 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/closure.py
--rw-r--r--   0 toon      (1000) toon      (1000)    17974 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/job.py
--rw-r--r--   0 toon      (1000) toon      (1000)     7011 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/metafunc.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-05-02 19:56:13.814308 ParMan-0.1.0/src/parman/runners/
--rw-r--r--   0 toon      (1000) toon      (1000)      823 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/runners/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1257 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/runners/base.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1783 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/runners/concurrent.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1231 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/runners/dry.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4717 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/runners/future.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2103 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/runners/parsl.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1345 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/runners/serial.py
--rw-r--r--   0 toon      (1000) toon      (1000)     9238 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/scheduler.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-05-02 19:56:13.814308 ParMan-0.1.0/src/parman/tests/
--rw-r--r--   0 toon      (1000) toon      (1000)      806 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/tests/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1504 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/tests/conftest.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3376 2023-05-02 19:25:03.000000 ParMan-0.1.0/src/parman/tests/test_demos.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5536 2023-05-02 19:25:03.000000 ParMan-0.1.0/src/parman/tests/test_scheduler.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3727 2023-05-02 19:25:03.000000 ParMan-0.1.0/src/parman/tests/test_treeleaf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5794 2023-05-02 19:25:03.000000 ParMan-0.1.0/src/parman/tests/test_waitfuture.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5157 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/treeleaf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     7033 2023-05-02 19:23:54.000000 ParMan-0.1.0/src/parman/waitfuture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.722784 ParMan-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-07 14:49:33.000000 ParMan-0.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-07 14:49:33.000000 ParMan-0.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 14:49:33.000000 ParMan-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.710784 ParMan-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-07 14:49:33.000000 ParMan-0.2.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-07 14:49:33.000000 ParMan-0.2.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-07 14:49:33.000000 ParMan-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-07 14:49:33.000000 ParMan-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-07 14:49:33.000000 ParMan-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-07 14:49:33.000000 ParMan-0.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-07 14:49:33.000000 ParMan-0.2.0/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-07 14:49:33.000000 ParMan-0.2.0/HEADER
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-05-07 14:49:42.722784 ParMan-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-07 14:49:33.000000 ParMan-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/demc/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6485 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/demc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4625 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/linreg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5231 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/naivemc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/inspiration/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/inspiration/plastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/alumina.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/ibuprofen.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8333 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/plastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/jobdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/jobdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.710784 ParMan-0.2.0/demos/jobdemo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/jobdemo/templates/boot/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/boot/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/boot/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/boot/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/jobdemo/templates/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/compute/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/compute/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/compute/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/jobdemo/templates/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/sample/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/sample/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/sample/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/demos/jobdemo/templates/train/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/train/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/train/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/train/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/train/submit.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1080 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/mindmutable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/scheduledemo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/waitdemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-07 14:49:33.000000 ParMan-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 14:49:42.722784 ParMan-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.710784 ParMan-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/ParMan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/parman/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/parman/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/parman/clerks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/clerks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/clerks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/clerks/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/clerks/localtemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/metafunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/parman/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/dry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/parsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/parman/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/scripts/sbatch_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/treeleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/waitfuture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.722784 ParMan-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71045 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/jobdemo-results.sha256
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_metafunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_treeleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_waitfuture.py
```

### Comparing `ParMan-0.1.0/COPYING` & `ParMan-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `ParMan-0.1.0/PKG-INFO` & `ParMan-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParMan
-Version: 0.1.0
+Version: 0.2.0
 Summary: ParMan extends Python concurrent.futures to facilitate parallel workflows
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -174,20 +174,26 @@
 Project-URL: Changelog, https://github.com/reproducible-reporting/parman/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
-# ParMan
+[![pytest](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml)
+[![PyPI Upload](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/ParMan/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parman)
+
+# Parman
 
 At this stage, ParMan is an experimental project, so expect a rocky road ahead.
 
 The goal of ParMan is to extend `concurrent.futures` (and compatible implementations)
 with features that facilitate a transparent implementation of workflows.
 
 - `WaitFuture`: a Future subclass that is "finished" after its dependencies have finished.
```

### Comparing `ParMan-0.1.0/README.md` & `ParMan-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-# ParMan
+[![pytest](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml)
+[![PyPI Upload](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/ParMan/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parman)
+
+# Parman
 
 At this stage, ParMan is an experimental project, so expect a rocky road ahead.
 
 The goal of ParMan is to extend `concurrent.futures` (and compatible implementations)
 with features that facilitate a transparent implementation of workflows.
 
 - `WaitFuture`: a Future subclass that is "finished" after its dependencies have finished.
```

### Comparing `ParMan-0.1.0/src/ParMan.egg-info/PKG-INFO` & `ParMan-0.2.0/src/ParMan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParMan
-Version: 0.1.0
+Version: 0.2.0
 Summary: ParMan extends Python concurrent.futures to facilitate parallel workflows
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -174,20 +174,26 @@
 Project-URL: Changelog, https://github.com/reproducible-reporting/parman/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
-# ParMan
+[![pytest](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml)
+[![PyPI Upload](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/ParMan/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parman)
+
+# Parman
 
 At this stage, ParMan is an experimental project, so expect a rocky road ahead.
 
 The goal of ParMan is to extend `concurrent.futures` (and compatible implementations)
 with features that facilitate a transparent implementation of workflows.
 
 - `WaitFuture`: a Future subclass that is "finished" after its dependencies have finished.
```

### Comparing `ParMan-0.1.0/src/parman/__init__.py` & `ParMan-0.2.0/src/parman/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,12 +9,18 @@
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """ParMan package."""
+
+try:
+    from _version import __version__
+except ImportError:
+    __version__ = "0.0.0a-dev"
+    __version_tuple__ = (0, 0, 0, "a-dev")
```

### Comparing `ParMan-0.1.0/src/parman/clerks/__init__.py` & `ParMan-0.2.0/src/parman/runners/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Mapping between local job files and global storage layout."""
+"""Wrappers around Future-based libraries."""
```

### Comparing `ParMan-0.1.0/src/parman/clerks/base.py` & `ParMan-0.2.0/src/parman/clerks/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Base class for mapping between local and global file structure."""
 
+from collections.abc import Generator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Generator
+from typing import Any
 
 import attrs
 
 from ..treeleaf import transform_tree
 
 __all__ = ("ClerkBase",)
```

### Comparing `ParMan-0.1.0/src/parman/clerks/local.py` & `ParMan-0.2.0/src/parman/clerks/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Local to global mapping for in-tree calculations."""
 
 import os
+from collections.abc import Generator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Generator
 
 import attrs
 
 from .base import ClerkBase
 
 __all__ = ("LocalClerk",)
```

### Comparing `ParMan-0.1.0/src/parman/clerks/localtemp.py` & `ParMan-0.2.0/src/parman/clerks/localtemp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Local to global mapping for in-tree calculations."""
 
 import os
 import shutil
 import tempfile
+from collections.abc import Generator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Generator
 
 import attrs
 
 from .base import ClerkBase
 
 __all__ = ("LocalTempClerk",)
```

### Comparing `ParMan-0.1.0/src/parman/closure.py` & `ParMan-0.2.0/src/parman/closure.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Bundled information for a function to be submitted."""
 
-import inspect
 from concurrent.futures import Future
 from copy import deepcopy
 from typing import Any
 
 import attrs
 
 from .metafunc import MetaFuncBase, validate
@@ -62,15 +61,15 @@
 
     def cached_result(self) -> Any:
         """Get the cached result."""
         return self.metafunc.cached_result(*self.args, **self.kwargs)
 
     def get_parameters(self) -> dict[str, Any]:
         """Return a dictionary with all parameters (including positional ones)."""
-        signature = inspect.signature(self.metafunc.__call__)
+        signature = self.metafunc.get_signature()
         bound_arguments = signature.bind(*self.args, **self.kwargs)
         bound_arguments.apply_defaults()
         return dict(bound_arguments.arguments)
 
     def get_parameter_api(self) -> dict[str, Any]:
         """Return a type checking API for the parameters."""
         return self.metafunc.get_parameters_api(*self.args, **self.kwargs)
```

### Comparing `ParMan-0.1.0/src/parman/job.py` & `ParMan-0.2.0/src/parman/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Pythonic interface to (templates for) job scripts with configurable execution.
 
 A job script can be prepared in a template directory with the following elements:
 
@@ -29,25 +29,25 @@
 in the work directory from which the job script can read it parameters. Only keyword arguments
 are allowed to make the arguments more self-explaining. The job writes its results to
 ``result.json``. If the jobs fails, not writing this file will raise an exception and end the
 workflow (after other running jobs have completed).
 
 The ``jobinfo.py`` can specify three things:
 
-1) ``get_result_mock`` is mandatory.
+1) ``mock`` is mandatory.
    This is a function mimicking the Python interface to the job script.
    The arguments must have type hints to infer the API.
    The result must be a "mocked" result with the correct types of the return values.
    References to files, e.g. inputs needed from previous jobs or results from this job,
    are only recognized properly when they are ``Path`` instances from the built-in
    Python ``pathlib`` module.
 2) ``resources`` is optional. This is a dictionary specifying resources, which are specific to
    the runner used. Currently, this is only used by the ParslRunner.
-3) ``get_parameter_api`` is optional.
-   This function takes the same arguments as ``get_result_mock`` and can be used to return
+3) ``parameters`` is optional.
+   This function takes the same arguments as ``mock`` and can be used to return
    a more detailed parameters API than what is possible with type hints.
    It can also be useful when the parameters API depends on values in the parameters,
    although this seems to be a rather exotic scenario.
 
 Other files in the work directory that may be relevant or useful:
 
 - ``kwargs.sha256``: SHA256 sums of all files present in ``kwargs.json``, used to check if the
@@ -58,27 +58,28 @@
 - ``run.err``: the standard error of the run script.
 """
 
 import hashlib
 import inspect
 import json
 import os
+import re
 import shutil
 import string
 import subprocess
 import sys
 import types
 from pathlib import Path
 from typing import Any
 
 import attrs
 import cattrs
 
 from .clerks.base import ClerkBase
-from .clerks.localtemp import LocalTempClerk
+from .clerks.local import LocalClerk
 from .closure import Closure
 from .metafunc import MetaFuncBase, type_api_from_mock, type_api_from_signature
 from .treeleaf import iterate_tree, transform_tree
 
 __all__ = ("job", "structure", "unstructure")
 
 
@@ -105,16 +106,16 @@
     result_mock_func
         The result_mock_func defined in ``jobinfo.py``.
     """
 
     template: Path = attrs.field()
     jobinfo_source: str = attrs.field()
     resources: dict[str, Any] = attrs.field(init=False)
-    parameters_api_func: callable = attrs.field(init=False)
-    result_mock_func: callable = attrs.field(init=False)
+    parameters_func: callable = attrs.field(init=False)
+    mock_func: callable = attrs.field(init=False)
 
     def __getstate__(self):
         """Return state for pickle"""
         return self.template, self.jobinfo_source
 
     def __setstate__(self, d):
         """State from pickle"""
@@ -123,19 +124,19 @@
 
     def __attrs_post_init__(self):
         """Finalize the initializations of a Job."""
         # Execute the jobinfo source to fill in the other attributes.
         ns = {}
         exec(self.jobinfo_source, ns)
         self.resources = ns.get("resources", {})
-        self.parameters_api_func = ns.get("get_parameter_api")
-        self.result_mock_func = ns["get_result_mock"]
+        self.parameters_func = ns.get("parameters")
+        self.mock_func = ns["mock"]
 
     @classmethod
-    def from_template(cls, template: str):
+    def from_template(cls, template: str) -> "Job":
         """Initialize a job script from a template directory.
 
         Parameters
         ----------
         template
             The template directory must contain a ``jobinfo.py`` file with the metadata
             needed to schedule the job in ParMan.
@@ -143,22 +144,36 @@
             When the template is a relative path, it gets converted to an absolute one.
         """
         template = Path(template).absolute()
         with open(template / "jobinfo.py") as f:
             jobinfo_source = f.read()
         return cls(template, jobinfo_source)
 
-    def describe(self, clerk: ClerkBase, locator: str, script: str, kwargs: dict[str, Any]) -> Any:
+    def describe(
+        self,
+        clerk: ClerkBase,
+        locator: str,
+        script: str,
+        kwargs: dict[str, Any],
+        env: dict[str, str],
+    ) -> Any:
         """Short descriptor of the job.
 
         See ``__call__`` method for parameter documentation.
         """
         return locator
 
-    def __call__(self, clerk: ClerkBase, locator: str, script: str, kwargs: dict[str, Any]) -> Any:
+    def __call__(
+        self,
+        clerk: ClerkBase,
+        locator: str,
+        script: str,
+        kwargs: dict[str, Any],
+        env: dict[str, str],
+    ) -> Any:
         """Execute the job unconditionally.
 
         Parameters
         ----------
         clerk
             A clerk instance for getting files in the work directory and keeping track of the
             job output files.
@@ -167,25 +182,31 @@
             the overall workflow.
         script
             The name of the script to be executed.
             This name is also used for stdout and stderr files, by appending ``.out`` and ``.err``,
             respectively.
         kwargs
             Keyword arguments to be stored in the ``kwargs.json`` input for the jobs cript.
+        env
+            A dictionary with environment variables for the subprocess.
 
         Returns
         -------
         result
             The structured contents of the ``result.json`` file created by the job script.
             Output files needed by following jobs must be included here.
         """
 
         def run(workdir: Path) -> bool:
             print(f"Starting {locator}")
 
+            # Define useful environment variable
+            parman_env = env | {"PARMAN_WORKDIR": os.getcwd()}
+            write_sh_env(workdir / "jobenv.sh", parman_env)
+
             # Initialize the work directory
             shutil.copytree(self.template, workdir, dirs_exist_ok=True)
             local_kwargs = clerk.localize(kwargs, locator, workdir)
             with open(workdir / "kwargs.json", "w") as f:
                 json.dump(unstructure(local_kwargs), f)
             dump_hashes(workdir / "kwargs.sha256", compute_hashes(local_kwargs, workdir))
 
@@ -198,14 +219,15 @@
                         f"./{script}",
                         stdin=subprocess.DEVNULL,
                         stdout=fo,
                         stderr=fe,
                         shell=True,
                         cwd=workdir,
                         check=True,
+                        env=os.environ | parman_env,
                     )
             except subprocess.CalledProcessError as exc:
                 if fn_err.is_file():
                     with open(fn_err) as f:
                         sys.stderr.write(f.read())
                 raise RuntimeError(f"Script {locator} failed: {script}.") from exc
 
@@ -231,15 +253,20 @@
         result = self._in_workdir(run, clerk, locator, kwargs)
         if result is NotImplemented:
             raise OSError(f"No result.json after completion of {locator}")
         print(f"Completed {locator}")
         return result
 
     def cached_result(
-        self, clerk: ClerkBase, locator: str, script: str, kwargs: dict[str, Any]
+        self,
+        clerk: ClerkBase,
+        locator: str,
+        script: str,
+        kwargs: dict[str, Any],
+        env: dict[str, str],
     ) -> Any:
         """Return the result from a previous run if available.
 
         See ``__call__`` method for parameter documentation.
 
         Returns
         -------
@@ -291,59 +318,82 @@
 
         return self._in_workdir(run, clerk, locator, kwargs)
 
     def _in_workdir(
         self, run: callable, clerk: ClerkBase, locator: str, kwargs: dict[str, Any]
     ) -> dict[str, Any]:
         """Internal method for running something in a job work directory."""
-        result_api = type_api_from_mock(self.result_mock_func(**kwargs))
+        result_api = type_api_from_mock(self.mock_func(**kwargs))
         with clerk.workdir(locator) as workdir:
             path_result = workdir / clerk.pull(locator / Path("result.json"), locator, workdir)
             success = run(workdir)
             if success and path_result.exists():
                 clerk.push("result.json", locator, workdir)
                 with open(path_result) as f:
                     result = structure("result", json.load(f), result_api)
                     return clerk.globalize(result, locator, workdir)
             return NotImplemented
 
     def get_parameters_api(
-        self, clerk: ClerkBase, locator: str, script: str, kwargs: dict[str, Any]
+        self,
+        clerk: ClerkBase,
+        locator: str,
+        script: str,
+        kwargs: dict[str, Any],
+        env: dict[str, str],
     ) -> dict[str, Any]:
         """Return the parameter API derived from the ``jobinfo.py`` metadata.
 
         See ``__call__`` method for parameter documentation.
         """
         parameters_api = MetaFuncBase.get_parameters_api(self)
-        if self.parameters_api_func is None:
-            parameters_api["kwargs"] = type_api_from_signature(
-                inspect.signature(self.result_mock_func)
-            )
+        if self.parameters_func is None:
+            parameters_api["kwargs"] = type_api_from_signature(inspect.signature(self.mock_func))
         else:
-            parameters_api["kwargs"] = self.parameters_api_func(**kwargs)
+            parameters_api["kwargs"] = self.parameters_func(**kwargs)
         return parameters_api
 
     def get_result_mock(
-        self, clerk: ClerkBase, locator: str, script: str, kwargs: dict[str, Any]
+        self,
+        clerk: ClerkBase,
+        locator: str,
+        script: str,
+        kwargs: dict[str, Any],
+        env: dict[str, str],
     ) -> Any:
         """Return a mock result, derived from the ``jobinfo.py`` metadata.
 
         See ``__call__`` method for parameter documentation.
         """
-        return self.result_mock_func(**kwargs)
+        return self.mock_func(**kwargs)
 
     def get_resources(
-        self, clerk: ClerkBase, locator: str, script: str, kwargs: dict[str, Any]
+        self,
+        clerk: ClerkBase,
+        locator: str,
+        script: str,
+        kwargs: dict[str, Any],
+        env: dict[str, str],
     ) -> dict:
         """Return the value of the resources dictionary in ``jobinfo.py``
 
         See ``__call__`` method for parameter documentation.
         """
         return self.resources
 
+    def get_defaults(self):
+        """Get the default keyword arguments specified in the jobinfo file."""
+        signature = inspect.signature(self.mock_func)
+        defaults = {}
+        for name, parameter in signature.parameters.items():
+            default = parameter.default
+            if default != parameter.empty:
+                defaults[name] = default
+        return defaults
+
 
 def structure(prefix: str, json_data: Any, data_api: Any) -> Any:
     """Structure the unstructured data loaded from a JSON file.
 
     Parameters
     ----------
     prefix
@@ -359,15 +409,15 @@
     Returns
     -------
     structured
         A structured copy of the JSON data.
     """
 
     def transform(mulidx, json_leaf, leaf_api):
-        if not isinstance(leaf_api, (type, types.GenericAlias)):
+        if not isinstance(leaf_api, type | types.GenericAlias):
             raise TypeError(f"{prefix} at {mulidx}: cannot structure type {leaf_api}")
         try:
             return cattrs.structure(json_leaf, leaf_api)
         except cattrs.IterableValidationError as exc:
             raise TypeError(
                 f"{prefix} at {mulidx}: {json_leaf} does not conform {leaf_api}"
             ) from exc
@@ -426,25 +476,36 @@
     """Strip comment from line and strip whitespace."""
     comment_pos = line.find("#")
     if comment_pos >= 0:
         line = line[:comment_pos]
     return line.strip()
 
 
+def write_sh_env(path_rc, env):
+    with open(path_rc, "w") as f:
+        for key, value in env.items():
+            if not (isinstance(key, str) and re.match("[_a-zA-Z][_a-zA-Z0-9]*", key)):
+                raise ValueError(f"Invalid shell variable name: {key}")
+            f.write(f'export {key}="{value}"\n')
+
+
 @attrs.define
 class JobFactory:
     """Convenience class for instantiating new jobs"""
 
-    clerk: ClerkBase = attrs.field(default=attrs.Factory(LocalTempClerk))
+    clerk: ClerkBase = attrs.field(default=attrs.Factory(LocalClerk))
     script: str = attrs.field(default="run")
+    env: dict[str, str] = attrs.field(default=attrs.Factory(dict))
     _cache: dict[str, Job] = attrs.field(init=False, default=attrs.Factory(dict))
 
-    def __call__(self, template, locator, **kwargs):
+    def __call__(self, template: str, locator: str, **kwargs) -> Closure:
         """Create a new job with the locator and keyword arguments."""
         job = self._cache.get(template)
         if job is None:
             job = Job.from_template(template)
             self._cache[template] = job
-        return Closure(job, [self.clerk, locator, self.script, kwargs])
+        all_kwargs = job.get_defaults()
+        all_kwargs.update(kwargs)
+        return Closure(job, [self.clerk, locator, self.script, all_kwargs, self.env])
 
 
 job = JobFactory()
```

### Comparing `ParMan-0.1.0/src/parman/metafunc.py` & `ParMan-0.2.0/src/parman/metafunc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Function definition with metadata needed to setup the workflow.
 
 The MetaFuncBase class below defines two API methods:
 
@@ -45,15 +45,21 @@
 from typing import Any
 
 import attrs
 import cattrs
 
 from .treeleaf import iterate_tree, transform_tree
 
-__all__ = ("MetaFuncBase", "validate", "type_api_from_signature", "type_api_from_mock")
+__all__ = (
+    "MetaFuncBase",
+    "validate",
+    "type_api_from_signature",
+    "type_api_from_mock",
+    "MinimalMetaFunc",
+)
 
 
 @attrs.define
 class MetaFuncBase:
     """A callable and its metadata for use in a parallel workflow.
 
     Subclasses override the following methods:
@@ -75,14 +81,17 @@
         """Describe this metafunc."""
         return "unnamed"
 
     def __call__(self, *args, **kwargs) -> Any:
         """The method to be submitted to an executor."""
         raise NotImplementedError
 
+    def get_signature(self):
+        return inspect.signature(self.__call__)
+
     def cached_result(self, *args, **kwargs) -> Any:
         """Return a cached result in case recomputation can be avoided.
 
         This should give the same result as __call__, but fast enough for the main process.
         When no cached result is available, NotImplemented is returned.
         """
         return NotImplemented
@@ -96,15 +105,15 @@
 
         Returns
         -------
         type_api
             A dictionary mapping each argument name to an API specification.
             See module docstring for details on the API spec.
         """
-        return type_api_from_signature(inspect.signature(self.__call__))
+        return type_api_from_signature(self.get_signature())
 
     def get_result_mock(self, *args, **kwargs) -> Any:
         """A method returning API of the result, in the form of a mock.
 
         There is no default behavior to derive this from the __call__ signature,
         because the return value must be a mock example consistent with the parameters.
 
@@ -146,25 +155,32 @@
 
     Raises
     ------
     TypeError
         When a type error is encountered in the data.
     """
     for mulidx, (leaf, leaf_type) in iterate_tree(data, type_api):
-        # Use cattrs magic to check the type
-        if not isinstance(leaf_type, (type, types.GenericAlias)):
+        if isinstance(leaf_type, types.GenericAlias):
+            # Use cattrs magic to check the type
+            try:
+                cattrs.structure(leaf, leaf_type)
+            except cattrs.IterableValidationError as exc:
+                raise TypeError(
+                    f"{prefix} at {mulidx}: {leaf} does not conform {leaf_type}"
+                ) from exc
+            except cattrs.StructureHandlerNotFoundError as exc:
+                raise TypeError(
+                    f"{prefix} at {mulidx}: type {leaf_type} cannot be instantiated"
+                ) from exc
+        elif isinstance(leaf_type, type):
+            # Standard Python type check
+            if not isinstance(leaf, leaf_type):
+                raise TypeError(f"{prefix} at {mulidx} is not of type {leaf_type}")
+        else:
             raise TypeError(f"{prefix} at {mulidx}: cannot type-check {leaf} with {leaf_type}")
-        try:
-            cattrs.structure(leaf, leaf_type)
-        except cattrs.IterableValidationError as exc:
-            raise TypeError(f"{prefix} at {mulidx}: {leaf} does not conform {leaf_type}") from exc
-        except cattrs.StructureHandlerNotFoundError as exc:
-            raise TypeError(
-                f"{prefix} at {mulidx}: type {leaf_type} cannot be instantiated"
-            ) from exc
 
 
 def type_api_from_signature(signature):
     """Construct a type api from a function signature (inspect module)."""
     result = {}
     for name, parameter in signature.parameters.items():
         if parameter.annotation != parameter.empty:
@@ -180,11 +196,47 @@
 
 
 def type_api_from_mock(mock_api):
     """Derive a type_api (suitable for the validate function) from example data, mock_api."""
 
     def transform(_, mock_leaf):
         if isinstance(mock_leaf, type):
-            raise TypeError("A mock_api cannot contain types.")
+            raise TypeError("A mock result cannot contain types.")
         return type(mock_leaf)
 
     return transform_tree(transform, mock_api)
+
+
+@attrs.define
+class MinimalMetaFunc(MetaFuncBase):
+    """A bare-bones implementation of MetaFuncBase without caching."""
+
+    function: callable = attrs.field()
+    mock: callable = attrs.field(default=None)
+
+    def describe(self, *args, **kwargs) -> str:
+        """Describe this metafunc."""
+        return self.function.__name__
+
+    def __call__(self, *args, **kwargs) -> Any:
+        """The method to be submitted to an executor."""
+        return self.function(*args, **kwargs)
+
+    def get_signature(self) -> inspect.Signature:
+        """Return a signature of __call__, used for type checking."""
+        return inspect.signature(self.function)
+
+    def get_result_mock(self, *args, **kwargs) -> Any:
+        """A method returning API of the result, in the form of a mock.
+
+        There is no default behavior to derive this from the __call__ signature,
+        because the return value must be a mock example consistent with the parameters.
+
+        Returns
+        -------
+        result_api
+            An API specification for the result.
+            See module docstring for details on the API spec.
+        """
+        if self.mock is None:
+            return object()
+        return self.mock(*args, **kwargs)
```

### Comparing `ParMan-0.1.0/src/parman/runners/__init__.py` & `ParMan-0.2.0/HEADER`

 * *Files 14% similar despite different names*

```diff
@@ -9,12 +9,11 @@
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Wrappers around Future-based libraries."""
```

### Comparing `ParMan-0.1.0/src/parman/runners/base.py` & `ParMan-0.2.0/src/parman/runners/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Base class for all future-library wrappers."""
 
 from typing import Any
```

### Comparing `ParMan-0.1.0/src/parman/runners/concurrent.py` & `ParMan-0.2.0/src/parman/runners/concurrent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Concurrent job runner, wrapper around a standard Executor from concurrent.futures."""
 
 from concurrent.futures import Future, ThreadPoolExecutor
```

### Comparing `ParMan-0.1.0/src/parman/runners/dry.py` & `ParMan-0.2.0/src/parman/runners/dry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Dry runner, for testing the workflow API."""
 
 from typing import Any
```

### Comparing `ParMan-0.1.0/src/parman/runners/future.py` & `ParMan-0.2.0/src/parman/runners/future.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Abstract future job runner."""
 
 from concurrent.futures import Future, as_completed
 from functools import partial
```

### Comparing `ParMan-0.1.0/src/parman/runners/parsl.py` & `ParMan-0.2.0/src/parman/runners/parsl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Parsl job runner, wraps around Parsl AppFuture.
 
 From the ``resources`` dictionary attribute of the MetaFunc and Closure, only the
 file ``parsl_executors`` is used. (If not present, ``all`` is used by default.)
```

### Comparing `ParMan-0.1.0/src/parman/runners/serial.py` & `ParMan-0.2.0/src/parman/runners/serial.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Serial job runner, mainly useful for debugging, not using any Future instances."""
 
 from typing import Any
```

### Comparing `ParMan-0.1.0/src/parman/scheduler.py` & `ParMan-0.2.0/src/parman/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Schedule futures with dependencies.
 
 See `../demo/scheduledemo.py` for a simple usage example.
```

### Comparing `ParMan-0.1.0/src/parman/tests/__init__.py` & `ParMan-0.2.0/src/parman/clerks/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Unit tests for ParMan."""
+"""Mapping between local job files and global storage layout."""
```

### Comparing `ParMan-0.1.0/src/parman/tests/conftest.py` & `ParMan-0.2.0/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Shared fixtures for the unit tests."""
 
 import pathlib
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
```

### Comparing `ParMan-0.1.0/src/parman/tests/test_scheduler.py` & `ParMan-0.2.0/tests/test_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for parman.scheduler."""
 
 import random
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed, wait
 from functools import partial
 from time import sleep
 
 import pytest
-
-from ..scheduler import Scheduler
+from parman.scheduler import Scheduler
 
 
 def func(x, t):
     sleep(t)
     return 2 * x
 
 
@@ -139,23 +138,23 @@
 
         def user_submit(dependencies, t):
             # Get results outside submit call...
             x = sum(dependency.result() for dependency in dependencies)
             return pool.submit(func, x, t)
 
         with Scheduler(user_submit) as scheduler:
-            for i in range(size):
+            for _i in range(size):
                 step = random.randrange(1, 10)
                 offset = random.randrange(size)
                 delay = random.uniform(0.001, 0.010)
                 dependencies = futures[offset::step]
                 futures.append(scheduler.submit([dependencies, delay], {}, dependencies))
                 expected.append(2 * sum(expected[offset::step]))
 
-        pairs = list(zip(futures, expected))
+        pairs = list(zip(futures, expected, strict=True))
         if end == "reverse":
             pairs = pairs[::-1]
         elif end == "wait":
             wait(futures, timeout=5)
         elif end == "as_completed":
             list(as_completed(futures, timeout=5))
         else:
```

### Comparing `ParMan-0.1.0/src/parman/tests/test_treeleaf.py` & `ParMan-0.2.0/tests/test_treeleaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for parman.treeleaf."""
 
 
 import pytest
-
-from ..treeleaf import get_tree, iterate_tree, same, transform_tree
+from parman.treeleaf import get_tree, iterate_tree, same, transform_tree
 
 
 @pytest.mark.parametrize(
     "tree, mulidx, value",
     [
         ("aaa", (), "aaa"),
         (1, (), 1),
```

### Comparing `ParMan-0.1.0/src/parman/tests/test_waitfuture.py` & `ParMan-0.2.0/tests/test_waitfuture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for parman.waitfuture."""
 
 import random
 from concurrent.futures import (
@@ -26,16 +26,15 @@
     ThreadPoolExecutor,
     as_completed,
     wait,
 )
 from time import sleep
 
 import pytest
-
-from ..waitfuture import WaitGraph
+from parman.waitfuture import WaitGraph
 
 
 def func(x, t):
     sleep(t)
     return 2 * x
 
 
@@ -124,17 +123,17 @@
     assert f2.done()
     assert wf.done()
 
 
 def test_cancel(pool1):
     wait_graph = WaitGraph()
     f1 = pool1.submit(func, 1.0, 0.1)
-    f2 = pool1.submit(func, 2.0, 0.2)
+    f2 = pool1.submit(func, 2.0, 5.0)
     wf = wait_graph.submit([f1, f2], digest_tuple)
-    assert f2.cancel()
+    f2.cancel()
     assert wf.result(timeout=1) == (2.0, None)
     assert wf.done()
     assert f1.done()
     assert f2.cancelled()
 
 
 def test_exception(pool):
@@ -177,20 +176,20 @@
         return hash(args)
 
     random.seed(seed)
     wait_graph = WaitGraph()
     with Executor(max_workers) as pool:
         futures = [pool.submit(func, i, random.uniform(0.001, 0.010)) for i in range(size)]
         expected = [2 * i for i in range(size)]
-        for i in range(size):
+        for _i in range(size):
             step = random.randrange(1, 10)
             offset = random.randrange(size)
             futures.append(wait_graph.submit(futures[offset::step], digest))
             expected.append(digest(*expected[offset::step]))
-        pairs = list(zip(futures, expected))
+        pairs = list(zip(futures, expected, strict=True))
         if end == "reverse":
             pairs = pairs[::-1]
         elif end == "wait":
             wait(futures, timeout=5)
         elif end == "as_completed":
             list(as_completed(futures, timeout=5))
         else:
```

### Comparing `ParMan-0.1.0/src/parman/treeleaf.py` & `ParMan-0.2.0/src/parman/treeleaf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
 # This file is part of ParMan.
 #
 # ParMan is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Recursive processing of hierarchical trees of lists and dictionaries.
 
 The functions below facilitate operations on nested lists + dictionaries + other types.
 
@@ -29,16 +29,16 @@
 The name ``leaf`` is used for a list item or dictionary value in a ``tree``
 that is itself not a list or dictionary.
 The functions below treat leafs (including tuples) as opaque objects that cannot
 be recursed into.
 """
 
 
-from collections.abc import Iterator
-from typing import Any, Generator
+from collections.abc import Generator, Iterator
+from typing import Any
 
 __all__ = ("get_tree", "iterate_tree", "transform_tree", "same")
 
 
 def get_tree(tree: Any, mulidx: tuple) -> Any:
     """Get an leaf (or subtree) from a tree.
 
@@ -85,23 +85,23 @@
     leafs
         When one tree is given, a sinlge leaf is yielded at a time.
         When multiple trees are given, a tuple of corresponding leafs is yielded.
     """
     handled = False
     if same(type(tree) for tree in trees):
         if isinstance(trees[0], list) and same(len(tree) for tree in trees):
-            for intidx, items in enumerate(zip(*trees)):
+            for intidx, items in enumerate(zip(*trees, strict=True)):
                 for subidx, subtrees in iterate_tree(*items):
-                    yield (intidx,) + subidx, subtrees
+                    yield (intidx, *subidx), subtrees
             handled = True
         elif isinstance(trees[0], dict) and same(set(tree.keys()) for tree in trees):
             for keyidx in trees[0].keys():
                 items = [tree[keyidx] for tree in trees]
                 for subidx, subtrees in iterate_tree(*items):
-                    yield (keyidx,) + subidx, subtrees
+                    yield (keyidx, *subidx), subtrees
             handled = True
     if not handled:
         if len(trees) == 1:
             yield (), trees[0]
         else:
             yield (), trees
 
@@ -128,17 +128,17 @@
     outtree
         The result of the transformation:
         a new tree whose leaf equal the return values of the transform function calls.
     """
     if same(type(tree) for tree in trees):
         if isinstance(trees[0], list) and same(len(tree) for tree in trees):
             result = []
-            for intidx, items in enumerate(zip(*trees)):
-                result.append(transform_tree(transform, *items, _mulidx=_mulidx + (intidx,)))
+            for intidx, items in enumerate(zip(*trees, strict=True)):
+                result.append(transform_tree(transform, *items, _mulidx=(*_mulidx, intidx)))
             return result
         if isinstance(trees[0], dict) and same(set(tree.keys()) for tree in trees):
             result = {}
             for keyidx in trees[0].keys():
                 items = [tree[keyidx] for tree in trees]
-                result[keyidx] = transform_tree(transform, *items, _mulidx=_mulidx + (keyidx,))
+                result[keyidx] = transform_tree(transform, *items, _mulidx=(*_mulidx, keyidx))
             return result
     return transform(_mulidx, *trees)
```

### Comparing `ParMan-0.1.0/src/parman/waitfuture.py` & `ParMan-0.2.0/src/parman/waitfuture.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # of the License, or (at your option) any later version.
 #
 # ParMan is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
+# You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Generic dependency tracking for Future objects.
 
 See `../demo/waitdemo.py` for a simple usage example.
```

