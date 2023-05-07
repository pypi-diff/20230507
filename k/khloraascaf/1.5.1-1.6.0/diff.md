# Comparing `tmp/khloraascaf-1.5.1.tar.gz` & `tmp/khloraascaf-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf-1.5.1.tar", last modified: Tue Apr 18 15:06:31 2023, max compression
+gzip compressed data, was "khloraascaf-1.6.0.tar", last modified: Sun May  7 15:16:58 2023, max compression
```

## Comparing `khloraascaf-1.5.1.tar` & `khloraascaf-1.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:06:31.450515 khloraascaf-1.5.1/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)    45979 2023-04-18 15:06:31.449515 khloraascaf-1.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4599 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:06:31.450515 khloraascaf-1.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:06:31.433513 khloraascaf-1.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:06:31.441514 khloraascaf-1.5.1/src/khloraascaf/
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    12407 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5164 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:06:31.447515 khloraascaf-1.5.1/src/khloraascaf/ilp/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/dirf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)    10725 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/invf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     3418 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_max_dirf.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_max_invf.py
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_max_presscore.py
--rw-rw-rw-   0 root         (0) root         (0)    12009 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_repeated_fragments.py
--rw-rw-rw-   0 root         (0) root         (0)     2977 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_to_solver.py
--rw-rw-rw-   0 root         (0) root         (0)    10512 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_var_db.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/lib.py
--rw-rw-rw-   0 root         (0) root         (0)    12867 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/multiplied_doubled_contig_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     8303 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    21767 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/result.py
--rw-rw-rw-   0 root         (0) root         (0)     9071 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/run_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    20366 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/scaffolding_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     7104 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/src/khloraascaf/utils_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:06:31.443515 khloraascaf-1.5.1/src/khloraascaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45979 2023-04-18 15:06:31.000000 khloraascaf-1.5.1/src/khloraascaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1148 2023-04-18 15:06:31.000000 khloraascaf-1.5.1/src/khloraascaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:06:31.000000 khloraascaf-1.5.1/src/khloraascaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-18 15:06:31.000000 khloraascaf-1.5.1/src/khloraascaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-18 15:06:31.000000 khloraascaf-1.5.1/src/khloraascaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:06:31.449515 khloraascaf-1.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13426 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/tests/test_assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/tests/test_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)    22646 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/tests/test_toy_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-04-18 15:06:06.000000 khloraascaf-1.5.1/tests/test_utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.924577 khloraascaf-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    45914 2023-05-07 15:16:58.923661 khloraascaf-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4534 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 15:16:58.924577 khloraascaf-1.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.908993 khloraascaf-1.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.916327 khloraascaf-1.6.0/src/khloraascaf/
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12600 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.921827 khloraascaf-1.6.0/src/khloraascaf/ilp/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/dirf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/invf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_dirf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_invf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_presscore.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_repeated_fragments.py
+-rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_to_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_var_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/multiplied_doubled_contig_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     8309 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    21836 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/result.py
+-rw-rw-rw-   0 root         (0) root         (0)    27071 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/run_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/scaffolding_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     7146 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.917244 khloraascaf-1.6.0/src/khloraascaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45914 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.923661 khloraascaf-1.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13426 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_toy_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_utils_debug.py
```

### Comparing `khloraascaf-1.5.1/LICENCE` & `khloraascaf-1.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/PKG-INFO` & `khloraascaf-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.5.1
+Version: 1.6.0
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -731,18 +731,15 @@
 
 from khloraascaf import IR_REGION_ID, SC_REGION_ID, scaffolding
 from khloraascaf.inputs import INSTANCE_NAME_DEF, SOLVER_CBC
 from khloraascaf.outputs import (
     fmt_contigs_of_regions_filename,
     fmt_map_of_regions_filename,
 )
-from khloraascaf.run_metadata import (
-    fmt_io_config_metadata_filename,
-    fmt_solutions_metadata_filename,
-)
+from khloraascaf.run_metadata import IOConfig, MetadataAllSolutions
 
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
@@ -778,19 +775,19 @@
 assert outdir_gen / fmt_map_of_regions_filename(
     INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
 ) in files
 #
 # * YAML file containing all the arguments and options you used
 #   to run khloraascaf
 #
-assert outdir_gen / fmt_io_config_metadata_filename() in files
+assert outdir_gen / IOConfig.YAML_FILE in files
 #
 # * YAML file that contains metadata on the solutions
 #
-assert outdir_gen / fmt_solutions_metadata_filename() in files
+assert outdir_gen / MetadataAllSolutions.YAML_FILE in files
 ```
 
 
 ## Changelog
 
 You can refer to the [docs/src/changelog.md](docs/src/changelog.md) file for details.
```

### Comparing `khloraascaf-1.5.1/README.md` & `khloraascaf-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,15 @@
 
 from khloraascaf import IR_REGION_ID, SC_REGION_ID, scaffolding
 from khloraascaf.inputs import INSTANCE_NAME_DEF, SOLVER_CBC
 from khloraascaf.outputs import (
     fmt_contigs_of_regions_filename,
     fmt_map_of_regions_filename,
 )
-from khloraascaf.run_metadata import (
-    fmt_io_config_metadata_filename,
-    fmt_solutions_metadata_filename,
-)
+from khloraascaf.run_metadata import IOConfig, MetadataAllSolutions
 
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
@@ -82,19 +79,19 @@
 assert outdir_gen / fmt_map_of_regions_filename(
     INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
 ) in files
 #
 # * YAML file containing all the arguments and options you used
 #   to run khloraascaf
 #
-assert outdir_gen / fmt_io_config_metadata_filename() in files
+assert outdir_gen / IOConfig.YAML_FILE in files
 #
 # * YAML file that contains metadata on the solutions
 #
-assert outdir_gen / fmt_solutions_metadata_filename() in files
+assert outdir_gen / MetadataAllSolutions.YAML_FILE in files
 ```
 
 
 ## Changelog
 
 You can refer to the [docs/src/changelog.md](docs/src/changelog.md) file for details.
```

### Comparing `khloraascaf-1.5.1/pyproject.toml` & `khloraascaf-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf"
-version = "1.5.1"
+version = "1.6.0"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf/__init__.py` & `khloraascaf-1.6.0/src/khloraascaf/__init__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/__main__.py` & `khloraascaf-1.6.0/src/khloraascaf/__main__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/assembly_graph.py` & `khloraascaf-1.6.0/src/khloraascaf/assembly_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     IndexT,
     IndOrIndT,
     IndOrT,
     OrT,
 )
 
 from khloraascaf.inputs import STR_ORIENT
+from khloraascaf.lib import RegionIDT
 from khloraascaf.outputs import (
     ORC_ID_IND,
     ORC_OR_IND,
     ORIENT_INT_STR,
     OrCT,
     read_contigs_of_regions,
     read_map_of_regions,
@@ -129,14 +130,16 @@
         """Iterate over all the paths of oriented contigs.
 
         Yields
         ------
         list of IndOrT
             Path of oriented contigs
         """
+        # TODO don't use self method, to avoid verify path validity
+        # (because it is known valid)
         for region_path in self.all_region_paths():
             yield list(self.region_path_to_oriented_contigs(region_path))
 
     def region_path_to_oriented_contigs(
             self, region_path: Iterable[IndOrT]) -> Iterator[OrCT]:
         """Iterate over the oriented contigs of a given region path.
 
@@ -146,14 +149,15 @@
             Path of oriented regions
 
         Yields
         ------
         OrCT
             Oriented contig
         """
+        # TODO raise error if not a valid path
         for reg_ind, reg_or in region_path:
             yield from self.oriented_contigs_of_region(reg_ind, reg_or)
 
     # ~*~ Getter ~*~
 
     def revsymg(self) -> RevSymGraph:
         """Return the reverse symmetric graph associated.
@@ -300,22 +304,22 @@
                     ),
                 )
                 k += 2
             yield region_path
 
 
 def fmt_region_paths_filename(instance_name: str,
-                              ilp_combination: Iterable[str]) -> str:
+                              ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the region paths filename.
 
     Parameters
     ----------
     instance_name : str
         Instance name
-    ilp_combination : iterable of str
+    ilp_combination : iterable of RegionIDT
         ILP string code combination
 
     Returns
     -------
     str
         Formatted filename
     """
@@ -374,23 +378,24 @@
                         STR_ORIENT[l_orc[k + 1]],  # type: ignore
                     ),
                 )
                 k += 2
             yield oriented_contig_path
 
 
-def fmt_oriented_contig_paths_filename(instance_name: str,
-                                       ilp_combination: Iterable[str]) -> str:
+def fmt_oriented_contig_paths_filename(
+        instance_name: str,
+        ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the oriented contig paths filename.
 
     Parameters
     ----------
     instance_name : str
         Instance name
-    ilp_combination : iterable of str
+    ilp_combination : iterable of RegionIDT
         ILP string code combination
 
     Returns
     -------
     str
         Formatted filename
     """
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf/cli.py` & `khloraascaf-1.6.0/src/khloraascaf/cli.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/exceptions.py` & `khloraascaf-1.6.0/src/khloraascaf/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding=utf-8 -*-
 
 """Scaffolding exceptions module."""
 
 from collections.abc import Iterable
 from pathlib import Path
 
-from pulp import LpStatus
-
-from khloraascaf.lib import REGION_CODE_TO_ID, RegionCodeT
+from khloraascaf.lib import RegionIDT
 
 
 # ============================================================================ #
 #                                    CLASSES                                   #
 # ============================================================================ #
 # ---------------------------------------------------------------------------- #
 #                               Scaffolding Error                              #
@@ -61,31 +59,31 @@
         """
         return 'The scaffolding combination has failed'
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Region Types                                 #
 # ---------------------------------------------------------------------------- #
-class WrongRegionCode(Exception):
-    """Wrong region code exception."""
+class WrongRegionID(Exception):
+    """Wrong region identifier exception."""
 
-    def __init__(self, region_code: int):
+    def __init__(self, region_id: str):
         """The Initializer."""
         super().__init__()
-        self.__region_code = region_code
+        self.__region_id = region_id
 
     def __str__(self) -> str:
         """Print the exception message.
 
         Returns
         -------
         str
             Exception message
         """
-        return f'The region code {self.__region_code} is not correct'
+        return f"The region identifier '{self.__region_id}' is not correct"
 
 
 # ---------------------------------------------------------------------------- #
 #                                    Solver                                    #
 # ---------------------------------------------------------------------------- #
 class WrongSolverName(Exception):
     """Wrong solver name exception."""
@@ -110,33 +108,33 @@
 #                                Unfeasible ILP                                #
 # ---------------------------------------------------------------------------- #
 class _UnfeasibleILP(Exception):
     """ILP problem unfeasible exception."""
 
     _PROBLEM_ID = 'THE PROBLEM'
 
-    def __init__(self, status: int, ilp_codes: Iterable[RegionCodeT]):
+    def __init__(self, status: str, ilp_combi: Iterable[RegionIDT]):
         super().__init__()
-        self.__status: int = status
-        self.__ilp_codes: tuple[RegionCodeT, ...] = tuple(ilp_codes)
+        self.__status: str = status
+        self.__ilp_combi: tuple[RegionIDT, ...] = tuple(ilp_combi)
 
     def __str__(self) -> str:
         """Print the exception message.
 
         Returns
         -------
         str
             Exception message
         """
         return (
             f'The {self._PROBLEM_ID} problem is unfeasible:\n'
             '\t* ILP codes: '
-            + '-'.join(REGION_CODE_TO_ID[code] for code in self.__ilp_codes)
+            + '-'.join(self.__ilp_combi)
             + '\n'
-            f'\t* Status: {LpStatus[self.__status]}'
+            f'\t* Status: {self.__status}'
         )
 
 
 class UnfeasibleIR(_UnfeasibleILP):
     """IR optimisation problem unfeasible exception."""
 
     _PROBLEM_ID = 'Find the best inverted repeats'
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/dirf_sets.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/dirf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/invf_sets.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/invf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_circuit.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_circuit.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_max_dirf.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_dirf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_max_invf.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_invf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_max_presscore.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_presscore.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_repeated_fragments.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_repeated_fragments.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_to_solver.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_to_solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pathlib import Path
 from typing import Optional
 
 from pulp import GUROBI_CMD, PULP_CBC_CMD, LpProblem
 
 from khloraascaf.exceptions import WrongSolverName
 from khloraascaf.inputs import SOLVER_CBC, SOLVER_GUROBI
+from khloraascaf.lib import RegionIDT
 
 
 # ============================================================================ #
 #                                   CONSTANTS                                  #
 # ============================================================================ #
 # ---------------------------------------------------------------------------- #
 #                                   Log File                                   #
@@ -61,24 +62,24 @@
 
 
 # ---------------------------------------------------------------------------- #
 #                                Logs Formatters                               #
 # ---------------------------------------------------------------------------- #
 def fmt_solver_log_name(solver: str,
                         instance_name: str,
-                        ilp_combination: Iterable[str]) -> str:
+                        ilp_combination: Iterable[RegionIDT]) -> str:
     """Format solver log file name.
 
     Parameters
     ----------
     solver : str
         Solver name
     instance_name : str
         Instance name
-    ilp_combination : iterable of str
+    ilp_combination : iterable of RegionIDT
         ILP string code combination
 
     Returns
     -------
     str
         Formatted filename
     """
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf/ilp/pulp_var_db.py` & `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_var_db.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/inputs.py` & `khloraascaf-1.6.0/src/khloraascaf/inputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/src/khloraascaf/multiplied_doubled_contig_graph.py` & `khloraascaf-1.6.0/src/khloraascaf/multiplied_doubled_contig_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,16 +165,16 @@
         Yield
         -----
         OccOrCT
             Multiplied oriented sucessors
         """
         for (w_ind, w_or), _ in self._edges.succs((v[CIND_IND], v[COR_IND])):
             w_mult = self._vertices.attr(w_ind, MULT_ATTR)
-            for u_occ in range(w_mult):
-                yield w_ind, w_or, u_occ
+            for w_occ in range(w_mult):
+                yield w_ind, w_or, w_occ
 
     # ~*~ Getter ~*~
 
     def repeated_contigs(self) -> list[IndexT]:
         """Return the list of repeated contigs' indices.
 
         Returns
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf/outputs.py` & `khloraascaf-1.6.0/src/khloraascaf/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from khloraascaf.inputs import (
     FORWARD_STR,
     REVERSE_STR,
     STR_ORIENT,
     IdCT,
     OrStrT,
 )
+from khloraascaf.lib import RegionIDT
 from khloraascaf.multiplied_doubled_contig_graph import (
     CIND_IND,
     COR_IND,
     MDCGraphIDContainer,
 )
 from khloraascaf.result import ScaffoldingResult
 
@@ -158,23 +159,23 @@
                 orc_of_region.append(
                     (l_orc[k], STR_ORIENT[l_orc[k + 1]]),  # type: ignore
                 )
                 k += 2
             yield orc_of_region
 
 
-def fmt_contigs_of_regions_filename(instance_name: str,
-                                    ilp_combination: Iterable[str]) -> str:
+def fmt_contigs_of_regions_filename(
+        instance_name: str, ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the contigs of regions filename.
 
     Parameters
     ----------
     instance_name : str
         Instance name
-    ilp_combination : iterable of str
+    ilp_combination : iterable of RegionIDT
         ILP string code combination
 
     Returns
     -------
     str
         Formatted filename
     """
@@ -221,16 +222,16 @@
     """
     with open(map_of_regions_path, 'r', encoding='utf-8') as mof_in:
         for line in mof_in:
             reg_indstr, reg_orstr = line.split()
             yield IndexT(reg_indstr), STR_ORIENT[reg_orstr]  # type: ignore
 
 
-def fmt_map_of_regions_filename(instance_name: str,
-                                ilp_combination: Iterable[str]) -> str:
+def fmt_map_of_regions_filename(
+        instance_name: str, ilp_combination: Iterable[RegionIDT]) -> str:
     """Format map of the regions filename.
 
     Parameters
     ----------
     instance_name : str
         Instance name
     ilp_combination : iterable of str
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf/result.py` & `khloraascaf-1.6.0/src/khloraascaf/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from __future__ import annotations
 
 from collections.abc import Iterable, Iterator
 from queue import LifoQueue, Queue
 from typing import Optional, Union
 
-from pulp import LpProblem
+from pulp import LpProblem, LpStatus
 from revsymg.index_lib import FORWARD_INT, REVERSE_INT, IndexT, OrT
 
 from khloraascaf.exceptions import NotACircuit
 from khloraascaf.ilp.dirf_sets import dirf_canonical, dirf_other
 from khloraascaf.ilp.invf_sets import invf_canonical, invf_other
 from khloraascaf.ilp.pulp_var_db import (
     BIN_THRESHOLD,
     PuLPVarDirFModel,
     PuLPVarInvFModel,
     PuLPVarModelT,
 )
-from khloraascaf.lib import DR_CODE, IR_CODE, SC_CODE, RegionCodeT
+from khloraascaf.lib import DR_REGION_ID, IR_REGION_ID, SC_REGION_ID, RegionIDT
 from khloraascaf.multiplied_doubled_contig_graph import (
     COCC_IND,
     COR_IND,
     MDCGraph,
     OccOrCT,
 )
 
@@ -67,69 +67,69 @@
     You can use the class name to type your variables.
     """
 
     # DOCU update docstring
     # DOCU add to docstring example to get regions' orc from result
 
     # pylint: disable=too-many-arguments
-    def __init__(self, ilp_codes: tuple[RegionCodeT, ...],
-                 status: int, opt_value: float,
+    def __init__(self, ilp_combi: tuple[RegionIDT, ...],
+                 status: str, opt_value: float,
                  region_map: OrRegMapT,
                  regions_occorc: tuple[RegOccOrCT, ...],
                  sc_regions: tuple[IndexT, ...],
                  ir_regions: tuple[IndexT, ...],
                  dr_regions: tuple[IndexT, ...]):
         """The Initializer."""
         #
         # Ilp origin
         #
-        self.__ilp_codes: tuple[RegionCodeT, ...] = ilp_codes
+        self.__ilp_combi: tuple[RegionIDT, ...] = ilp_combi
         #
         # ILP result
         #
-        self.__status: int = status
+        self.__status: str = status
         self.__opt_value: float = opt_value
         #
         # Genomic region
         #
         self.__region_map: OrRegMapT = region_map
         self.__regions_occorc: tuple[RegOccOrCT, ...] = regions_occorc
         self.__sc_regions: tuple[IndexT, ...] = sc_regions
         self.__ir_regions: tuple[IndexT, ...] = ir_regions
         self.__dr_regions: tuple[IndexT, ...] = dr_regions
 
     # ~*~ Getter ~*~
 
-    def last_ilp(self) -> RegionCodeT:
+    def last_ilp(self) -> RegionIDT:
         """Return last ILP code.
 
         Returns
         -------
-        RegionCodeT
+        RegionIDT
             Last ILP code
         """
-        return self.__ilp_codes[-1]
+        return self.__ilp_combi[-1]
 
-    def ilp_codes(self) -> Iterator[RegionCodeT]:
+    def ilp_combination(self) -> Iterator[RegionIDT]:
         """Iterate over ILP codes.
 
         Yields
         ------
-        RegionCodeT
+        RegionIDT
             ILP code
         """
-        yield from self.__ilp_codes
+        yield from self.__ilp_combi
 
-    def status(self) -> int:
-        """Returns status code.
+    def status(self) -> str:
+        """Returns ILP status.
 
         Returns
         -------
-        int
-            Status code
+        str
+            ILP status
         """
         return self.__status
 
     def opt_value(self) -> float:
         """ILP optimal value.
 
         Returns
@@ -240,24 +240,24 @@
         self.__sc_regions: list[IndexT] = []
         self.__ir_regions: list[IndexT] = []
         self.__dr_regions: list[IndexT] = []
 
     # ~*~ Setter ~*~
 
     def add_region(self,
-                   region_code: RegionCodeT,
+                   region_code: RegionIDT,
                    region_index: Optional[IndexT] = None) -> IndexT:
         """Add a region.
 
          # XXX region_index provides the first repeat
          * this works because we build pair of repeated regions
 
         Parameters
         ----------
-        region_code : RegionCodeT
+        region_code : RegionIDT
             Region code
         region_index : IndexT, optional
             Index of an already existing region, else None
 
         Returns
         -------
         IndexT
@@ -266,27 +266,27 @@
         #
         # Non-existing region
         #
         if region_index is None:
             region_index = len(self.__regions_occorc)
             self.__regions_occorc.append([])
             self.__region_map.append((region_index, FORWARD_INT))
-            if region_code == IR_CODE:
+            if region_code == IR_REGION_ID:
                 self.__ir_regions.append(region_index)
-            elif region_code == DR_CODE:
+            elif region_code == DR_REGION_ID:
                 self.__dr_regions.append(region_index)
             else:
                 self.__sc_regions.append(region_index)
         #
         # Already existing region (repeat)
         #
         else:
-            if region_code == IR_CODE:
+            if region_code == IR_REGION_ID:
                 self.__region_map.append((region_index, REVERSE_INT))
-            elif region_code == DR_CODE:
+            elif region_code == DR_REGION_ID:
                 self.__region_map.append((region_index, FORWARD_INT))
         return region_index
 
     def add_occorc_to_region(self, v: OccOrCT, region_index: IndexT):
         """Add v to the region denoted by its index.
 
         Parameters
@@ -297,32 +297,32 @@
             Region's index
         """
         self.__regions_occorc[region_index].append(v)
 
     # ~*~ Getter ~*~
 
     def view(self, prob: LpProblem,
-             ilp_codes: Iterable[RegionCodeT]) -> ScaffoldingResult:
+             ilp_combi: Iterable[RegionIDT]) -> ScaffoldingResult:
         """Return a ScaffoldingResult view from the builder.
 
         Parameters
         ----------
         prob : LpProblem
             PuLP problem
-        ilp_codes : iterable of RegionCodeT
+        ilp_combi : iterable of RegionIDT
             ILP codes
 
         Returns
         -------
         ScaffoldingResult
             Scaffolding result view
         """
         return ScaffoldingResult(
-            tuple(ilp_codes),
-            prob.status,
+            tuple(ilp_combi),
+            LpStatus[prob.status],
             self.__fix_opt_value(prob),
             tuple(self.__region_map),
             tuple(tuple(regoccorc) for regoccorc in self.__regions_occorc),
             tuple(self.__sc_regions),
             tuple(self.__ir_regions),
             tuple(self.__dr_regions),
         )
@@ -332,27 +332,27 @@
 #                                   FUNCTIONS                                  #
 # ============================================================================ #
 # ---------------------------------------------------------------------------- #
 #                               Build The Regions                              #
 # ---------------------------------------------------------------------------- #
 # pylint: disable=too-many-arguments
 def path_to_regions(mdcg: MDCGraph, starter_vertex: OccOrCT,
-                    ilp_codes: Iterable[RegionCodeT],
+                    ilp_combi: Iterable[RegionIDT],
                     prob: LpProblem, var: PuLPVarModelT,
                     fix_result: Optional[ScaffoldingResult] = None) -> (
                         ScaffoldingResult):
     """Extract regions from optimal path.
 
     Parameters
     ----------
     mdcg : MDCGraph
         Multiplied doubled contig graph
     starter_vertex : OccOrCT
         Starter vertex
-    ilp_codes : iterable of RegionCodeT
+    ilp_combi : iterable of RegionIDT
         Code of the regions that have been scaffolded
     prob : LpProblem
         PuLP problem
     var : PuLPVarModelT
         PuLP variables
     fix_result : ScaffoldingResult, optional
         Scaffolding result with regions, by default `None`
@@ -369,16 +369,16 @@
     set_invf_paired = __create_set_invf_paired(var, fix_result)
     set_dirf_paired = __create_set_dirf_paired(var, fix_result)
 
     # ------------------------------------------------------------------------ #
     # Init regions
     # ------------------------------------------------------------------------ #
     result_builder = _ScaffoldingResultBuilder()
-    prev_region_code = SC_CODE
-    region_index = result_builder.add_region(SC_CODE)
+    prev_region_code = SC_REGION_ID
+    region_index = result_builder.add_region(SC_REGION_ID)
 
     initial_vertex = __find_initial(
         mdcg, starter_vertex, var, set_invf_paired, set_dirf_paired)
 
     u: OccOrCT = initial_vertex  # previous v
     v: Optional[OccOrCT] = initial_vertex
     #
@@ -397,43 +397,43 @@
     # Walk into the solution path
     # ------------------------------------------------------------------------ #
     while v is not None:
         region_code = __get_region_code(v, set_invf_paired, set_dirf_paired)
         #
         # Single-copy
         #
-        if region_code == SC_CODE:
+        if region_code == SC_REGION_ID:
             #
             # New single-copy
             #
             if prev_region_code != region_code:
                 region_index = result_builder.add_region(region_code)
             result_builder.add_occorc_to_region(v, region_index)
         #
         # IR and DR
         #
         else:
             canonical_repf = (
-                invf_canonical(v) if region_code == IR_CODE
+                invf_canonical(v) if region_code == IR_REGION_ID
                 else dirf_canonical(v)
             )
             #
             # First region of the repeat
             #
             if canonical_repf not in v_canonical_rep:
                 if not __is_repeat_contiguous(
                         u, v, var, prev_region_code, region_code):
                     region_index = result_builder.add_region(region_code)
                     rep_queue[region_index] = (
-                        LifoQueue() if region_code == IR_CODE
+                        LifoQueue() if region_code == IR_REGION_ID
                         else Queue()
                     )
                 result_builder.add_occorc_to_region(v, region_index)
                 rep_queue[region_index].put(
-                    invf_other(v) if region_code == IR_CODE
+                    invf_other(v) if region_code == IR_REGION_ID
                     else dirf_other(v),
                 )
                 v_canonical_rep[canonical_repf] = region_index
             #
             # Seconde region of the repeat
             #
             else:
@@ -446,15 +446,15 @@
         prev_region_code = region_code
         u = v
         v = __succ_in_path(v, mdcg, var, initial_vertex)
 
     # ------------------------------------------------------------------------ #
     # To view
     # ------------------------------------------------------------------------ #
-    return result_builder.view(prob, ilp_codes)
+    return result_builder.view(prob, ilp_combi)
 
 
 # ---------------------------------------------------------------------------- #
 #                               Walk In The Path                               #
 # ---------------------------------------------------------------------------- #
 def __pred_in_path(v: OccOrCT, mdcg: MDCGraph,
                    var: PuLPVarModelT, initial_vertex: OccOrCT) -> (
@@ -642,71 +642,71 @@
     return v
 
 
 # ---------------------------------------------------------------------------- #
 #                               Region Management                              #
 # ---------------------------------------------------------------------------- #
 def __get_region_code(v: OccOrCT, set_invf_paired: set[OccOrCT],
-                      set_dirf_paired: set[OccOrCT]) -> RegionCodeT:
+                      set_dirf_paired: set[OccOrCT]) -> RegionIDT:
     """Get the code of the region for the multiplied oriented contig.
 
     Parameters
     ----------
     v : OccOrCT
         Multiplied oriented contig
     set_invf_paired : set of OccOrCT
         Set of canonical of paired inverted fragments
     set_dirf_paired : set of OccOrCT
         Set of canonical of paired direct fragments
 
     Returns
     -------
-    RegionCodeT
-        Code of the region (0: SC; 1: IR; 2: DR)
+    RegionIDT
+        Region identifier (SC, DR, or IR)
     """
     if dirf_canonical(v) in set_dirf_paired:
-        return DR_CODE
+        return DR_REGION_ID
     if ((v[COCC_IND] - v[COR_IND]) % 2 == 0  # pylint: disable=compare-to-zero
             and invf_canonical(v) in set_invf_paired):
-        return IR_CODE
-    return SC_CODE
+        return IR_REGION_ID
+    return SC_REGION_ID
 
 
 def __is_repeat_contiguous(u: OccOrCT, v: OccOrCT, var: PuLPVarModelT,
-                           prev_region_code: RegionCodeT,
-                           region_code: RegionCodeT) -> bool:
+                           prev_region_code: RegionIDT,
+                           region_code: RegionIDT) -> bool:
     """Answer yes if the repeat given by its code is contiguous.
 
     Parameters
     ----------
     u : OccOrCT
         Multiplied oriented contig
     v : OccOrCT
         Multiplied oriented contig
     var : PuLPVarModelT
         PuLP variables
-    prev_region_code : RegionCodeT
+    prev_region_code : RegionIDT
         Previous region's code
-    region_code : RegionCodeT
+    region_code : RegionIDT
         Current region's code
 
     Returns
     -------
     bool
         True if repeat is contiguous, else False
     """
     if prev_region_code != region_code:
         return False
     #
     # IR:
     #   i (= u) -> k(= v): ok, so is there l -> j?
     #
-    if region_code == IR_CODE:
+    if region_code == IR_REGION_ID:
         return var.x[invf_other(v), invf_other(u)].varValue > BIN_THRESHOLD
     #
     # DR:
     #   i (= u) -> k(= v): ok, so is there j -> l?
     #
-    if region_code == DR_CODE:
+    if region_code == DR_REGION_ID:
         return var.x[dirf_other(u), dirf_other(v)].varValue > BIN_THRESHOLD
     # TODO error out of code
     return False
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf/scaffolding_methods.py` & `khloraascaf-1.6.0/src/khloraascaf/scaffolding_methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 """Scaffolding module."""
 
 
 from collections.abc import Callable
 from pathlib import Path
 from typing import Optional, Type
 
-from pulp import LpProblem, LpStatusOptimal
+from pulp import LpProblem, LpStatus, LpStatusOptimal
 
 from khloraascaf.exceptions import (
     CombineScaffoldingError,
     RepeatScaffoldingError,
     ScaffoldingError,
     SingleCopyScaffoldingError,
     UnfeasibleDR,
     UnfeasibleIR,
     UnfeasibleSC,
-    WrongRegionCode,
+    WrongRegionID,
 )
 from khloraascaf.ilp.pulp_max_dirf import intersected_dirf_model
 from khloraascaf.ilp.pulp_max_invf import nested_invf_model
 from khloraascaf.ilp.pulp_max_presscore import best_presscore_model
 from khloraascaf.ilp.pulp_to_solver import (
     fmt_solver_log_name,
     solve_pulp_problem,
@@ -38,21 +38,15 @@
     OUTDIR_DEF,
     PRESSCORE_UPB_DEF,
     SOLVER_CBC,
     IdCT,
     MultT,
     PresScoreT,
 )
-from khloraascaf.lib import (
-    DR_CODE,
-    IR_CODE,
-    REGION_CODE_TO_ID,
-    SC_CODE,
-    RegionCodeT,
-)
+from khloraascaf.lib import DR_REGION_ID, IR_REGION_ID, SC_REGION_ID, RegionIDT
 from khloraascaf.multiplied_doubled_contig_graph import (
     MDCGraph,
     MDCGraphIDContainer,
     OccOrCT,
     first_forward_occurrence,
     mdcg_with_id_from_input_files,
 )
@@ -61,17 +55,19 @@
     fmt_map_of_regions_filename,
     generate_output_directory,
     write_contigs_of_regions,
     write_map_of_regions,
 )
 from khloraascaf.result import ScaffoldingResult, path_to_regions
 from khloraascaf.run_metadata import (
-    bump_debug_to_yaml,
-    bump_io_config_to_yaml,
-    bump_solutions_to_yaml,
+    IOConfig,
+    MetadataAllDebugs,
+    MetadataAllSolutions,
+    MetadataDebug,
+    MetadataSolution,
 )
 from khloraascaf.utils_debug import (
     fmt_found_repeated_fragments_filename,
     fmt_vertices_of_regions_filename,
     write_found_repeated_fragments,
     write_vertices_of_regions,
 )
@@ -79,15 +75,15 @@
 
 # DOCU constants, functions
 # ============================================================================ #
 #                                   CONSTANTS                                  #
 # ============================================================================ #
 # FIXME use constant args something like that
 __HEIGHT_LIM = 2
-__OTHER_REPEAT_CODE = {IR_CODE: DR_CODE, DR_CODE: IR_CODE}
+__OTHER_REPEAT_CODE = {IR_REGION_ID: DR_REGION_ID, DR_REGION_ID: IR_REGION_ID}
 
 
 # ============================================================================ #
 #                                   FUNCTIONS                                  #
 # ============================================================================ #
 # ---------------------------------------------------------------------------- #
 #                        From User's Files Main Function                       #
@@ -143,19 +139,20 @@
     # ------------------------------------------------------------------------ #
     # Manage options
     # ------------------------------------------------------------------------ #
     # REFACTOR find less confusable name for outdir / output_dir / outdir_gen...
     outdir_gen = outdir / generate_output_directory(instance_name)
     outdir_gen.mkdir()
 
-    bump_io_config_to_yaml(
-        outdir_gen, contig_attrs, contig_links, contig_starter,
+    IOConfig(
+        outdir_gen,
+        contig_attrs, contig_links, contig_starter,
         multiplicity_upperbound, presence_score_upperbound,
         solver, outdir, instance_name, debug,
-    )
+    ).write_yaml()
 
     # ------------------------------------------------------------------------ #
     # Generate scaffolding data from input files
     # ------------------------------------------------------------------------ #
     # DOCU verify docstring
     mdcg, id_container = mdcg_with_id_from_input_files(
         contig_attrs, contig_links,
@@ -313,23 +310,23 @@
         If one of the repeat solve fails during the combination
     """
     best_opt_value = 0.0
     new_results: list[ScaffoldingResult] = []
 
     for opti_result in (opti_results if opti_results else (None,)):
 
-        l_scaffolding_to_apply: list[RegionCodeT] = (
-            [IR_CODE, DR_CODE] if opti_result is None
+        l_scaffolding_to_apply: list[RegionIDT] = (
+            [IR_REGION_ID, DR_REGION_ID] if opti_result is None
             else [__OTHER_REPEAT_CODE[opti_result.last_ilp()]]
         )
 
-        for region_code in l_scaffolding_to_apply:
+        for region_id in l_scaffolding_to_apply:
             try:
                 result = scaffolding_region(
-                    region_code, mdcg, starter_vertex,
+                    region_id, mdcg, starter_vertex,
                     solver, outdir, instance_name,
                     fix_result=opti_result,
                     debug=debug,
                 )
             except (UnfeasibleIR, UnfeasibleDR) as exc:
                 # TODO logging print(exc, file=sys.stderr)
                 raise RepeatScaffoldingError() from exc
@@ -378,15 +375,15 @@
         One of the single copy region scaffolding has failed
     """
     best_opt_value = 0.0
     new_results = []
     for opti_result in (opti_results if opti_results else (None,)):
         try:
             result = scaffolding_region(
-                SC_CODE, mdcg, starter_vertex,
+                SC_REGION_ID, mdcg, starter_vertex,
                 solver, outdir, instance_name,
                 fix_result=opti_result,
                 debug=debug,
             )
         except UnfeasibleSC as exc:
             # TODO logging here print(exc, file=sys.stderr)
             raise SingleCopyScaffoldingError() from exc
@@ -399,24 +396,24 @@
 
     return tuple(new_results)
 
 
 # ---------------------------------------------------------------------------- #
 #                         Specific Regions Scaffolding                         #
 # ---------------------------------------------------------------------------- #
-def scaffolding_region(region_code: RegionCodeT,
+def scaffolding_region(region_id: RegionIDT,
                        mdcg: MDCGraph, starter_vertex: OccOrCT,
                        solver: str, outdir: Path, instance_name: str,
                        fix_result: Optional[ScaffoldingResult] = None,
                        debug: bool = OUTDEBUG_DEF) -> ScaffoldingResult:
     """Scaffolding of a specific region.
 
     Parameters
     ----------
-    region_code : RegionCodeT
+    region_id : RegionIDT
         Code of the region to scaffold
     mdcg : MDCGraph
         Multiplied doubled contig graph
     starter_vertex : OccOrCT
         Starter vertex
     solver : str
         MILP solver to use ('cbc' or 'gurobi')
@@ -432,132 +429,155 @@
     Returns
     -------
     ScaffoldingResult
         Scaffolding result
 
     Raises
     ------
-    WrongRegionCode
+    WrongRegionID
         The given code of the regions is wrong
     UnfeasibleIR
         The combinatorial problem is unfeasible
     UnfeasibleDR
         The combinatorial problem is unfeasible
     UnfeasibleSC
         The combinatorial problem is unfeasible
 
     Warnings
     --------
     Files in the output directory can be erased.
     """
     # ------------------------------------------------------------------------ #
-    # ILP codes
+    # ILP combi
     # ------------------------------------------------------------------------ #
     if fix_result is not None:
-        ilp_codes = tuple(fix_result.ilp_codes()) + (region_code,)
+        ilp_combi = tuple(fix_result.ilp_combination()) + (region_id,)
     else:
-        ilp_codes = (region_code,)
+        ilp_combi = (region_id,)
 
     # ------------------------------------------------------------------------ #
     # Instantiate functions and exceptions
     # ------------------------------------------------------------------------ #
     model_fn: Callable[..., tuple[LpProblem, PuLPVarModelT]]
     unfeasible_exc: Type[Exception]
-    if region_code == IR_CODE:
+    if region_id == IR_REGION_ID:
         model_fn = nested_invf_model
         unfeasible_exc = UnfeasibleIR
-    elif region_code == DR_CODE:
+    elif region_id == DR_REGION_ID:
         model_fn = intersected_dirf_model
         unfeasible_exc = UnfeasibleDR
-    elif region_code == SC_CODE:
+    elif region_id == SC_REGION_ID:
         model_fn = best_presscore_model
         unfeasible_exc = UnfeasibleSC
     else:
-        raise WrongRegionCode(region_code)
+        raise WrongRegionID(region_id)
 
     prob, var = model_fn(mdcg, starter_vertex, fix_result=fix_result)
 
     log_path = None
     if debug:
         log_path = outdir / fmt_solver_log_name(
-            solver, instance_name,
-            (REGION_CODE_TO_ID[code] for code in ilp_codes),
+            solver, instance_name, ilp_combi,
         )
     solve_pulp_problem(prob, solver, log_path=log_path)
 
     if prob.status != LpStatusOptimal:
         if debug:
-            bump_debug_to_yaml(
-                outdir, instance_name, ilp_codes,
-                starter_vertex, prob.status, None,
-            )
-        raise unfeasible_exc(prob.status, ilp_codes)
+            MetadataAllDebugs(
+                outdir,
+                (
+                    MetadataDebug(
+                        outdir, ilp_combi, starter_vertex,
+                        LpStatus[prob.status],
+                    ),
+                ),
+            ).write_yaml(append_yaml=True)
+        raise unfeasible_exc(prob.status, ilp_combi)
 
-    result = path_to_regions(mdcg, starter_vertex, ilp_codes,
+    result = path_to_regions(mdcg, starter_vertex, ilp_combi,
                              prob, var, fix_result)
 
     # ------------------------------------------------------------------------ #
     # Debug
     # ------------------------------------------------------------------------ #
     if debug:
-        __region_scaffolding_debug(instance_name, outdir, var, result)
-        bump_debug_to_yaml(
-            outdir, instance_name, result.ilp_codes(),
-            starter_vertex, result.status(), result.opt_value(),
-        )
+        __region_scaffolding_debug(instance_name, outdir,
+                                   starter_vertex, var, result)
     return result
 
 
 def __region_scaffolding_debug(instance_name: str, outdir: Path,
+                               starter_vertex: OccOrCT,
                                var: PuLPVarModelT, result: ScaffoldingResult):
     """Write debug files and metadata.
 
     Parameters
     ----------
     instance_name : str
         Instance name
     outdir : Path
         Output directory path
+    starter_vertex : OccOrCT
+        Starter vertex
+    var : PuLPVarModelT
+        PuLP variables
     result : ScaffoldingResult
         Scaffolding result
     """
     # ------------------------------------------------------------------------ #
     # The order of vertices for each region
     # ------------------------------------------------------------------------ #
     vertices_of_regions_path = (
         outdir / fmt_vertices_of_regions_filename(
-            instance_name,
-            (REGION_CODE_TO_ID[code] for code in result.ilp_codes()),
+            instance_name, result.ilp_combination(),
         )
     )
     write_vertices_of_regions(result, vertices_of_regions_path)
 
     # ------------------------------------------------------------------------ #
     # The map of regions (debug version)
     # ------------------------------------------------------------------------ #
     map_of_regions_path = (
         outdir / fmt_map_of_regions_filename(
-            instance_name,
-            (REGION_CODE_TO_ID[code] for code in result.ilp_codes()),
+            instance_name, result.ilp_combination(),
         )
     )
     write_map_of_regions(result, map_of_regions_path)
 
     # ------------------------------------------------------------------------ #
     # The repeated fragments
     # ------------------------------------------------------------------------ #
+    repeat_fragments_path = None
     if isinstance(var, (PuLPVarInvFModel, PuLPVarDirFModel)):
         repeat_fragments_path = (
             outdir / fmt_found_repeated_fragments_filename(
-                instance_name,
-                (REGION_CODE_TO_ID[code] for code in result.ilp_codes()),
+                instance_name, result.ilp_combination(),
             )
         )
         write_found_repeated_fragments(var, repeat_fragments_path)
 
+    # ------------------------------------------------------------------------ #
+    # Debug metadata
+    # ------------------------------------------------------------------------ #
+    MetadataAllDebugs(
+        outdir,
+        (
+            MetadataDebug(
+                outdir, result.ilp_combination(), starter_vertex,
+                result.status(), result.opt_value(),
+                Path(vertices_of_regions_path.name),
+                Path(map_of_regions_path.name),
+                (
+                    Path(repeat_fragments_path.name)
+                    if repeat_fragments_path is not None else None
+                ),
+            ),
+        ),
+    ).write_yaml(append_yaml=True)
+
 
 def __solution_scaffolding(solution: ScaffoldingResult, outdir_gen: Path,
                            id_container: MDCGraphIDContainer, debug: bool,
                            instance_name: str):
     """Output the solution in files and in YAML.
 
     Parameters
@@ -570,35 +590,43 @@
         Container connecting contig identifiers and vertex indices
     debug : bool
         Debugging option
     instance_name : str
         Instance name
     """
     # -------------------------------------------------------------------- #
-    # Write the solution in files
-    # -------------------------------------------------------------------- #
-    #
     # The order of oriented contigs for each region
-    #
+    # -------------------------------------------------------------------- #
     contigs_of_regions_path = (
         outdir_gen / fmt_contigs_of_regions_filename(
-            instance_name,
-            (REGION_CODE_TO_ID[code] for code in solution.ilp_codes()),
+            instance_name, solution.ilp_combination(),
         )
     )
     write_contigs_of_regions(
         solution, contigs_of_regions_path,
         id_container=id_container,
     )
-    #
+
+    # -------------------------------------------------------------------- #
     # The order of oriented regions
-    #
-    if not debug:  # already generated if debug is True
-        map_of_regions_path = (
-            outdir_gen / fmt_map_of_regions_filename(
-                instance_name,
-                (REGION_CODE_TO_ID[code] for code in solution.ilp_codes()),
-            )
+    # -------------------------------------------------------------------- #
+    map_of_regions_path = (
+        outdir_gen / fmt_map_of_regions_filename(
+            instance_name, solution.ilp_combination(),
         )
+    )
+    if not debug:  # already generated if debug is True
         write_map_of_regions(solution, map_of_regions_path)
 
-    bump_solutions_to_yaml(outdir_gen, instance_name, solution.ilp_codes())
+    # -------------------------------------------------------------------- #
+    # Add solution metadata
+    # -------------------------------------------------------------------- #
+    MetadataAllSolutions(
+        outdir_gen,
+        (
+            MetadataSolution(
+                outdir_gen, solution.ilp_combination(),
+                Path(contigs_of_regions_path.name),
+                Path(map_of_regions_path.name),
+            ),
+        ),
+    ).write_yaml(append_yaml=True)
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf/utils_debug.py` & `khloraascaf-1.6.0/src/khloraascaf/utils_debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from pathlib import Path
 from typing import Iterable, Iterator, Union
 
 from revsymg.index_lib import IndexT
 
 from khloraascaf.ilp.pulp_var_db import PuLPVarDirF, PuLPVarInvF
+from khloraascaf.lib import RegionIDT
 from khloraascaf.multiplied_doubled_contig_graph import OccOrCT
 from khloraascaf.outputs import ORIENT_INT_STR, STR_ORIENT
 from khloraascaf.result import ScaffoldingResult
 
 
 # DOCU module debug
 # ============================================================================ #
@@ -100,23 +101,24 @@
                         IndexT(l_occorcstr[k + 2]),
                     ),
                 )
                 k += 3
             yield vertices_of_region
 
 
-def fmt_vertices_of_regions_filename(instance_name: str,
-                                     ilp_combination: Iterable[str]) -> str:
+def fmt_vertices_of_regions_filename(
+        instance_name: str,
+        ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the vertices of regions file name.
 
     Parameters
     ----------
     instance_name : str
         Instance name
-    ilp_combination : iterable of str
+    ilp_combination : iterable of RegionIDT
         ILP string code combination
 
     Returns
     -------
     str
         Formatted file name
     """
@@ -194,22 +196,22 @@
                 STR_ORIENT[code_canonical[2]],  # type: ignore
                 IndexT(code_canonical[3]),
             )
 
 
 def fmt_found_repeated_fragments_filename(
         instance_name: str,
-        ilp_combination: Iterable[str]) -> str:
+        ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the found repeated fragments file name.
 
     Parameters
     ----------
     instance_name : str
         Instance name
-    ilp_combination : iterable of str
+    ilp_combination : iterable of RegionIDT
         ILP string code combination
 
     Returns
     -------
     str
         Formatted file name
     """
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf.egg-info/PKG-INFO` & `khloraascaf-1.6.0/src/khloraascaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.5.1
+Version: 1.6.0
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -731,18 +731,15 @@
 
 from khloraascaf import IR_REGION_ID, SC_REGION_ID, scaffolding
 from khloraascaf.inputs import INSTANCE_NAME_DEF, SOLVER_CBC
 from khloraascaf.outputs import (
     fmt_contigs_of_regions_filename,
     fmt_map_of_regions_filename,
 )
-from khloraascaf.run_metadata import (
-    fmt_io_config_metadata_filename,
-    fmt_solutions_metadata_filename,
-)
+from khloraascaf.run_metadata import IOConfig, MetadataAllSolutions
 
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
@@ -778,19 +775,19 @@
 assert outdir_gen / fmt_map_of_regions_filename(
     INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
 ) in files
 #
 # * YAML file containing all the arguments and options you used
 #   to run khloraascaf
 #
-assert outdir_gen / fmt_io_config_metadata_filename() in files
+assert outdir_gen / IOConfig.YAML_FILE in files
 #
 # * YAML file that contains metadata on the solutions
 #
-assert outdir_gen / fmt_solutions_metadata_filename() in files
+assert outdir_gen / MetadataAllSolutions.YAML_FILE in files
 ```
 
 
 ## Changelog
 
 You can refer to the [docs/src/changelog.md](docs/src/changelog.md) file for details.
```

### Comparing `khloraascaf-1.5.1/src/khloraascaf.egg-info/SOURCES.txt` & `khloraascaf-1.6.0/src/khloraascaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/tests/test_assembly_graph.py` & `khloraascaf-1.6.0/tests/test_assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.5.1/tests/test_exceptions.py` & `khloraascaf-1.6.0/tests/test_exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 """Unit testing for assembly graph."""
 
 # pylint: disable=compare-to-zero, missing-raises-doc
 
 from pathlib import Path
 
+from pulp import LpStatus, LpStatusInfeasible
+
 from khloraascaf.exceptions import (
     CombineScaffoldingError,
     NotACircuit,
     RepeatScaffoldingError,
     ScaffoldingError,
     SingleCopyScaffoldingError,
     UnfeasibleDR,
     UnfeasibleIR,
     UnfeasibleSC,
-    WrongRegionCode,
+    WrongRegionID,
     WrongSolverName,
 )
-from khloraascaf.lib import IR_CODE, SC_CODE
+from khloraascaf.lib import IR_REGION_ID, SC_REGION_ID
 
 
 # ============================================================================ #
 #                                TEST FUNCTIONS                                #
 # ============================================================================ #
 def test_scaffolding_error():
     """Test ScaffoldingError exception."""
@@ -48,53 +50,53 @@
 def test_combine_scaffolding_error():
     """Test CombineScaffoldingError exception."""
     exc = CombineScaffoldingError()
     assert str(exc) == 'The scaffolding combination has failed'
 
 
 def test_wrong_region_code():
-    """Test WrongRegionCode exception."""
-    exc = WrongRegionCode(IR_CODE)
-    assert str(exc) == 'The region code 1 is not correct'
+    """Test WrongRegionID exception."""
+    exc = WrongRegionID(IR_REGION_ID)
+    assert str(exc) == "The region identifier 'ir' is not correct"
 
 
 def test_wrong_solver_name():
     """Test WrongSolverName exception."""
     exc = WrongSolverName('wrong_solver')
     assert str(exc) == 'The solver name wrong_solver is not correct'
 
 
 def test_unfeasible_ir():
     """Test UnfeasibleIR exception."""
     exc = UnfeasibleIR(
-        -1, (IR_CODE, SC_CODE),
+        LpStatus[LpStatusInfeasible], (IR_REGION_ID, SC_REGION_ID),
     )
     assert str(exc) == (
         'The Find the best inverted repeats problem is unfeasible:\n'
         '\t* ILP codes: ir-sc\n'
         '\t* Status: Infeasible'
     )
 
 
 def test_unfeasible_dr():
     """Test UnfeasibleDR exception."""
     exc = UnfeasibleDR(
-        -1, (IR_CODE, SC_CODE),
+        LpStatus[LpStatusInfeasible], (IR_REGION_ID, SC_REGION_ID),
     )
     assert str(exc) == (
         'The Find the best direct repeats problem is unfeasible:\n'
         '\t* ILP codes: ir-sc\n'
         '\t* Status: Infeasible'
     )
 
 
 def test_unfeasible_sc():
     """Test UnfeasibleSC exception."""
     exc = UnfeasibleSC(
-        -1, (IR_CODE, SC_CODE),
+        LpStatus[LpStatusInfeasible], (IR_REGION_ID, SC_REGION_ID),
     )
     assert str(exc) == (
         'The Find the best single copy regions problem is unfeasible:\n'
         '\t* ILP codes: ir-sc\n'
         '\t* Status: Infeasible'
     )
```

### Comparing `khloraascaf-1.5.1/tests/test_toy_examples.py` & `khloraascaf-1.6.0/tests/test_toy_examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     outdir_gen : Path
         Output directory
     """
     #
     # Test output files
     #
     assert {p.name for p in outdir_gen.glob('*')} == {
-        'all_scaffolding.yaml',
+        'debugs.yaml',
         'contigs_of_regions_khloraascaf_ir_sc.tsv',
         'io_config.yaml',
         'map_of_regions_khloraascaf_dr.tsv',
         'map_of_regions_khloraascaf_ir_dr.tsv',
         'map_of_regions_khloraascaf_ir_sc.tsv',
         'map_of_regions_khloraascaf_ir.tsv',
         'repfrag_khloraascaf_dr.tsv',
@@ -259,15 +259,15 @@
     outdir_gen : Path
         Output directory
     """
     #
     # Test output files
     #
     assert {p.name for p in outdir_gen.glob('*')} == {
-        'all_scaffolding.yaml',
+        'debugs.yaml',
         'contigs_of_regions_khloraascaf_dr_sc.tsv',
         'io_config.yaml',
         'map_of_regions_khloraascaf_dr_ir.tsv',
         'map_of_regions_khloraascaf_dr_sc.tsv',
         'map_of_regions_khloraascaf_dr.tsv',
         'map_of_regions_khloraascaf_ir.tsv',
         'repfrag_khloraascaf_dr_ir.tsv',
@@ -372,15 +372,15 @@
     outdir_gen : Path
         Output directory
     """
     #
     # Test output files
     #
     assert {p.name for p in outdir_gen.glob('*')} == {
-        'all_scaffolding.yaml',
+        'debugs.yaml',
         'contigs_of_regions_khloraascaf_sc.tsv',
         'io_config.yaml',
         'map_of_regions_khloraascaf_dr.tsv',
         'map_of_regions_khloraascaf_ir.tsv',
         'map_of_regions_khloraascaf_sc.tsv',
         'repfrag_khloraascaf_dr.tsv',
         'repfrag_khloraascaf_ir.tsv',
@@ -483,15 +483,15 @@
     outdir_gen : Path
         Output directory
     """
     #
     # Test output files
     #
     assert {p.name for p in outdir_gen.glob('*')} == {
-        'all_scaffolding.yaml',
+        'debugs.yaml',
         'contigs_of_regions_khloraascaf_ir_dr_sc.tsv',
         'io_config.yaml',
         'map_of_regions_khloraascaf_dr.tsv',
         'map_of_regions_khloraascaf_ir_dr_sc.tsv',
         'map_of_regions_khloraascaf_ir_dr.tsv',
         'map_of_regions_khloraascaf_ir.tsv',
         'repfrag_khloraascaf_dr.tsv',
@@ -602,15 +602,15 @@
     outdir_gen : Path
         Output directory
     """
     #
     # Test output files
     #
     assert {p.name for p in outdir_gen.glob('*')} == {
-        'all_scaffolding.yaml',
+        'debugs.yaml',
         'contigs_of_regions_khloraascaf_dr_ir_sc.tsv',
         'io_config.yaml',
         'map_of_regions_khloraascaf_dr_ir_sc.tsv',
         'map_of_regions_khloraascaf_dr_ir.tsv',
         'map_of_regions_khloraascaf_dr.tsv',
         'map_of_regions_khloraascaf_ir.tsv',
         'repfrag_khloraascaf_dr_ir.tsv',
```

### Comparing `khloraascaf-1.5.1/tests/test_utils_debug.py` & `khloraascaf-1.6.0/tests/test_utils_debug.py`

 * *Files identical despite different names*

