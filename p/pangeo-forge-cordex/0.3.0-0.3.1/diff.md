# Comparing `tmp/pangeo-forge-cordex-0.3.0.tar.gz` & `tmp/pangeo-forge-cordex-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.3.0.tar", last modified: Sun May  7 18:35:50 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.3.1.tar", last modified: Sun May  7 20:16:27 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.3.0.tar` & `pangeo-forge-cordex-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.873596 pangeo-forge-cordex-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.873596 pangeo-forge-cordex-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.873596 pangeo-forge-cordex-0.3.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.873596 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-07 18:35:50.000000 pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:50.877596 pangeo-forge-cordex-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 18:35:40.000000 pangeo-forge-cordex-0.3.0/tests/test_recipe_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.076575 pangeo-forge-cordex-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.056574 pangeo-forge-cordex-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.068575 pangeo-forge-cordex-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 20:16:27.076575 pangeo-forge-cordex-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.068575 pangeo-forge-cordex-0.3.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.072575 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.076575 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-07 20:16:27.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-07 20:16:26.000000 pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-07 20:16:27.080575 pangeo-forge-cordex-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:27.076575 pangeo-forge-cordex-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-07 20:16:13.000000 pangeo-forge-cordex-0.3.1/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.3.0/.github/workflows/ci.yaml` & `pangeo-forge-cordex-0.3.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.3.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/.gitignore` & `pangeo-forge-cordex-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/LICENSE` & `pangeo-forge-cordex-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/PKG-INFO` & `pangeo-forge-cordex-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.3.0
+Version: 0.3.1
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/esgf_access.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/recipe.py` & `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/recipe.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex/utils.py` & `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/PKG-INFO` & `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.3.0
+Version: 0.3.1
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.3.0/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.3.1/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 setup.cfg
 setup.py
 .github/workflows/ci.yaml
 .github/workflows/release.yaml
 ci/environment.yml
 pangeo_forge_cordex/__init__.py
 pangeo_forge_cordex/_version.py
+pangeo_forge_cordex/catalog.py
 pangeo_forge_cordex/esgf_access.py
 pangeo_forge_cordex/parsing.py
 pangeo_forge_cordex/recipe.py
 pangeo_forge_cordex/utils.py
 pangeo_forge_cordex.egg-info/PKG-INFO
 pangeo_forge_cordex.egg-info/SOURCES.txt
 pangeo_forge_cordex.egg-info/dependency_links.txt
```

### Comparing `pangeo-forge-cordex-0.3.0/setup.cfg` & `pangeo-forge-cordex-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/tests/test_parsing.py` & `pangeo-forge-cordex-0.3.1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.0/tests/test_recipe_creation.py` & `pangeo-forge-cordex-0.3.1/tests/test_recipe_creation.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import xarray as xr
 from pangeo_forge_recipes.patterns import pattern_from_file_sequence
 from pangeo_forge_recipes.recipes import XarrayZarrRecipe
 
 from pangeo_forge_cordex import logon, recipe_inputs_from_iids
 
 iids = [
-    "cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas.v20140620",
+    # "cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas.v20140620",
     "cordex.output.EUR-11.GERICS.ECMWF-ERAINT.evaluation.r1i1p1.REMO2015.v1.mon.tas.v20180813",
 ]
 
 
 @pytest.mark.parametrize("iid", iids)
 def test_recipe_inputs(iid):
     sslcontext = logon()
```

