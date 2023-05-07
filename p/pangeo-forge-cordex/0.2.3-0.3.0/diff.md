# Comparing `tmp/pangeo-forge-cordex-0.2.3.tar.gz` & `tmp/pangeo-forge-cordex-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.2.3.tar", last modified: Fri May  5 12:29:24 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.3.0.tar", last modified: Sun May  7 18:35:50 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.2.3.tar` & `pangeo-forge-cordex-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.080386 pangeo-forge-cordex-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.084386 pangeo-forge-cordex-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.084386 pangeo-forge-cordex-0.2.3/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.084386 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 12:29:23.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/tests/test_recipe_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.873596 pangeo-forge-cordex-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.873596 pangeo-forge-cordex-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.873596 pangeo-forge-cordex-0.3.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.873596 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.2.3/.github/workflows/ci.yaml` & `pangeo-forge-cordex-0.3.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.3.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/.gitignore` & `pangeo-forge-cordex-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/LICENSE` & `pangeo-forge-cordex-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/PKG-INFO` & `pangeo-forge-cordex-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.2.3
+Version: 0.3.0
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/esgf_access.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/recipe.py` & `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/recipe.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/utils.py` & `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/PKG-INFO` & `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.2.3
+Version: 0.3.0
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/setup.cfg` & `pangeo-forge-cordex-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/tests/test_parsing.py` & `pangeo-forge-cordex-0.3.0/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.3/tests/test_recipe_creation.py` & `pangeo-forge-cordex-0.3.0/tests/test_recipe_creation.py`

 * *Files identical despite different names*

