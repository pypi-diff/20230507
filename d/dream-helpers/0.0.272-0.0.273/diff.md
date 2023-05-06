# Comparing `tmp/dream_helpers-0.0.272.tar.gz` & `tmp/dream_helpers-0.0.273.tar.gz`

## Comparing `dream_helpers-0.0.272.tar` & `dream_helpers-0.0.273.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/.bumpversion.cfg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/Makefile
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/src/dream_helpers/__init__.py
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/src/dream_helpers/datahub_helper.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/src/dream_helpers/kubeflow_helper.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/src/dream_helpers/minio_helper.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/README.md
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/pyproject.toml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/.bumpversion.cfg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/Makefile
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/src/dream_helpers/__init__.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/src/dream_helpers/datahub_helper.py
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/src/dream_helpers/kubeflow_helper.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/src/dream_helpers/minio_helper.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/README.md
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/pyproject.toml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/PKG-INFO
```

### Comparing `dream_helpers-0.0.272/src/dream_helpers/datahub_helper.py` & `dream_helpers-0.0.273/src/dream_helpers/datahub_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 Dataset Helpers  
 
 '''
 def upsert_datasets(dataset_urns: List[str],
                    platform_urn: str,
                    datahub_endpoint: str,
-                   dataset_schema: list[SchemaFieldClass],
+                   dataset_schema: List[SchemaFieldClass],
                    dataset_ver: int=0) -> None: 
     
     for dataset_urn in dataset_urns:
         event: MetadataChangeProposalWrapper = MetadataChangeProposalWrapper(
             entityUrn=dataset_urn,
             aspect=SchemaMetadataClass(
                 schemaName="",
```

### Comparing `dream_helpers-0.0.272/src/dream_helpers/kubeflow_helper.py` & `dream_helpers-0.0.273/src/dream_helpers/kubeflow_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.272/src/dream_helpers/minio_helper.py` & `dream_helpers-0.0.273/src/dream_helpers/minio_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.272/.gitignore` & `dream_helpers-0.0.273/.gitignore`

 * *Files identical despite different names*

