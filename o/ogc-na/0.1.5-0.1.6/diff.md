# Comparing `tmp/ogc_na-0.1.5.tar.gz` & `tmp/ogc_na-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.1.5.tar", last modified: Sun May  7 09:54:58 2023, max compression
+gzip compressed data, was "ogc_na-0.1.6.tar", last modified: Sun May  7 18:04:12 2023, max compression
```

## Comparing `ogc_na-0.1.5.tar` & `ogc_na-0.1.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.347285 ogc_na-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.335284 ogc_na-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.339284 ogc_na-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 09:54:47.000000 ogc_na-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-07 09:54:47.000000 ogc_na-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 09:54:47.000000 ogc_na-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-07 09:54:58.347285 ogc_na-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-07 09:54:47.000000 ogc_na-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.339284 ogc_na-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-07 09:54:47.000000 ogc_na-0.1.5/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-07 09:54:47.000000 ogc_na-0.1.5/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-07 09:54:47.000000 ogc_na-0.1.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-07 09:54:47.000000 ogc_na-0.1.5/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-07 09:54:47.000000 ogc_na-0.1.5/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.335284 ogc_na-0.1.5/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.339284 ogc_na-0.1.5/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    31309 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.339284 ogc_na-0.1.5/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-07 09:54:47.000000 ogc_na-0.1.5/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.339284 ogc_na-0.1.5/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-07 09:54:58.000000 ogc_na-0.1.5/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-07 09:54:58.000000 ogc_na-0.1.5/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:54:58.000000 ogc_na-0.1.5/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-07 09:54:58.000000 ogc_na-0.1.5/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-07 09:54:58.000000 ogc_na-0.1.5/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-07 09:54:47.000000 ogc_na-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.339284 ogc_na-0.1.5/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-07 09:54:47.000000 ogc_na-0.1.5/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-07 09:54:47.000000 ogc_na-0.1.5/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-07 09:54:47.000000 ogc_na-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 09:54:58.347285 ogc_na-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-07 09:54:47.000000 ogc_na-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.343284 ogc_na-0.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:58.347285 ogc_na-0.1.5/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-07 09:54:47.000000 ogc_na-0.1.5/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.602810 ogc_na-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.594810 ogc_na-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 18:03:58.000000 ogc_na-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-07 18:03:58.000000 ogc_na-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 18:03:58.000000 ogc_na-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-07 18:04:12.602810 ogc_na-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-07 18:03:58.000000 ogc_na-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-07 18:03:58.000000 ogc_na-0.1.6/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-07 18:03:58.000000 ogc_na-0.1.6/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-07 18:03:58.000000 ogc_na-0.1.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-07 18:03:58.000000 ogc_na-0.1.6/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-07 18:03:58.000000 ogc_na-0.1.6/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.594810 ogc_na-0.1.6/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31680 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-07 18:03:58.000000 ogc_na-0.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-07 18:03:58.000000 ogc_na-0.1.6/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-07 18:03:58.000000 ogc_na-0.1.6/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-07 18:03:58.000000 ogc_na-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:04:12.602810 ogc_na-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-07 18:03:58.000000 ogc_na-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.602810 ogc_na-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.602810 ogc_na-0.1.6/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/test_profile.py
```

### Comparing `ogc_na-0.1.5/.github/workflows/python-publish.yml` & `ogc_na-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/.gitignore` & `ogc_na-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/PKG-INFO` & `ogc_na-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.1.5
+Version: 0.1.6
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.5/README.md` & `ogc_na-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/docs/examples.md` & `ogc_na-0.1.6/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/docs/gen_ref_pages.py` & `ogc_na-0.1.6/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/docs/index.md` & `ogc_na-0.1.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/docs/tutorials.md` & `ogc_na-0.1.6/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/mkdocs.yml` & `ogc_na-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/annotate_schema.py` & `ogc_na-0.1.6/ogc/na/annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/domain_config.py` & `ogc_na-0.1.6/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/download.py` & `ogc_na-0.1.6/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/ingest_json.py` & `ogc_na-0.1.6/ogc/na/ingest_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -647,15 +647,15 @@
             if isinstance(input_file, str):
                 remaining_fn.extend(input_file.split(','))
             else:
                 remaining_fn.append(input_file)
         while remaining_fn:
             fn = str(remaining_fn.popleft())
 
-            if not fn or not os.path.isfile():
+            if not fn or not os.path.isfile(fn):
                 continue
 
             if re.match(r'.*\.ya?ml$', fn):
                 # Context file found, try to find corresponding JSON/JSON-LD file(s)
                 logger.info('Potential YAML context file found: %s', fn)
                 remaining_fn.extend(filenames_from_context(fn, domain_config=domain_cfg) or [])
                 continue
@@ -702,15 +702,15 @@
 
 
 def _process_cmdln():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "input",
-        nargs='+',
+        nargs='*',
         help="Source file (instead of service)",
     )
 
     parser.add_argument(
         '-j',
         '--json-ld',
         action='store_true',
@@ -779,22 +779,33 @@
     parser.add_argument(
         '--url-whitelist',
         '-w',
         nargs='*',
         help='Regular expression for URL whitelisting'
     )
 
+    parser.add_argument(
+        '--use-git-status',
+        action='store_true',
+        help='Use git status for obtaining batch filenames'
+    )
+
     args = parser.parse_args()
 
     if args.domain_config:
         domain_cfg = DomainConfiguration(args.domain_config)
     else:
         domain_cfg = None
 
-    result = process(args.input,
+    input_files = args.input
+    if args.batch and args.use_git_status:
+        git_status = util.git_status()
+        input_files = git_status['added'] + git_status['modified'] + [r[1] for r in git_status['renamed']]
+
+    result = process(input_files,
                      context_fn=args.context,
                      domain_cfg=domain_cfg,
                      jsonld_fn=args.json_ld_file if args.json_ld else False,
                      ttl_fn=args.ttl_file if args.ttl else False,
                      batch=args.batch,
                      skip_on_missing_context=args.skip_on_missing_context,
                      provenance_base_uri=False if args.no_provenance else args.provenance_base_uri,
```

### Comparing `ogc_na-0.1.5/ogc/na/input_filters/__init__.py` & `ogc_na-0.1.6/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/input_filters/csv.py` & `ogc_na-0.1.6/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/profile.py` & `ogc_na-0.1.6/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/provenance.py` & `ogc_na-0.1.6/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/update_vocabs.py` & `ogc_na-0.1.6/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc/na/util.py` & `ogc_na-0.1.6/ogc/na/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from glob import glob
 from pathlib import Path
 from time import time
 from typing import Optional, Union, Any, Mapping, Hashable
 
 import requests
 import rfc3987
+import git
 from rdflib import Graph
 from pyshacl import validate as shacl_validate
 from urllib.parse import urlparse
 
 from ogc.na.validation import ValidationReport
 
 import yaml
@@ -235,7 +236,28 @@
     dest = orig_dict if replace else {**orig_dict}
     for k, v in with_dict.items():
         if isinstance(v, Mapping):
             dest[k] = deep_update(orig_dict.get(k, {}), with_dict, replace)
         else:
             dest[k] = v
     return dest
+
+
+def git_status(repo_path: str | Path = '.'):
+    repo = git.Repo(repo_path)
+    added = repo.untracked_files
+    modified = []
+    deleted = []
+    renamed = []
+    for diff in repo.head.commit.diff(None):
+        if diff.change_type == 'D':
+            deleted.append(diff.a_path)
+        elif diff.change_type == 'M':
+            modified.append(diff.a_path)
+        elif diff.chhange_type == 'R':
+            renamed.append((diff.a_path, diff.b_path))
+    return {
+        'added': added,
+        'modified': modified,
+        'deleted': deleted,
+        'renamed': renamed,
+    }
```

### Comparing `ogc_na-0.1.5/ogc/na/validation.py` & `ogc_na-0.1.6/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.1.6/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.1.5
+Version: 0.1.6
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.5/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.1.6/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/pyproject.toml` & `ogc_na-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/rdf/domaincfg.vocab.ttl` & `ogc_na-0.1.6/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/test/data/headers.csv` & `ogc_na-0.1.6/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/test/data/uplift_context_valid.yml` & `ogc_na-0.1.6/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/test/test_annotate_schema.py` & `ogc_na-0.1.6/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/test/test_ingest_json.py` & `ogc_na-0.1.6/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/test/test_input_filters_csv.py` & `ogc_na-0.1.6/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.5/test/test_profile.py` & `ogc_na-0.1.6/test/test_profile.py`

 * *Files identical despite different names*

