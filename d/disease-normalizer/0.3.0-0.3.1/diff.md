# Comparing `tmp/disease-normalizer-0.3.0.tar.gz` & `tmp/disease-normalizer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disease-normalizer-0.3.0.tar", last modified: Wed Nov  2 17:58:10 2022, max compression
+gzip compressed data, was "disease-normalizer-0.3.1.tar", last modified: Wed Jan 11 18:35:26 2023, max compression
```

## Comparing `disease-normalizer-0.3.0.tar` & `disease-normalizer-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 17:58:10.446373 disease-normalizer-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4528 2022-11-02 17:58:10.446373 disease-normalizer-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 17:58:10.442373 disease-normalizer-0.3.0/disease/
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9322 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    13827 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/database.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 17:58:10.442373 disease-normalizer-0.3.0/disease/etl/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10083 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/do.py
--rw-r--r--   0 runner    (1001) docker     (121)     5216 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/merge.py
--rw-r--r--   0 runner    (1001) docker     (121)     4934 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/mondo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5408 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/ncit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/omim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/oncotree.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/etl/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    20769 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/query.py
--rw-r--r--   0 runner    (1001) docker     (121)    16878 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/disease/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 17:58:10.446373 disease-normalizer-0.3.0/disease_normalizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4528 2022-11-02 17:58:10.000000 disease-normalizer-0.3.0/disease_normalizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-11-02 17:58:10.000000 disease-normalizer-0.3.0/disease_normalizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 17:58:10.000000 disease-normalizer-0.3.0/disease_normalizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 17:58:10.000000 disease-normalizer-0.3.0/disease_normalizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-02 17:58:10.000000 disease-normalizer-0.3.0/disease_normalizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-02 17:58:10.000000 disease-normalizer-0.3.0/disease_normalizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-11-02 17:58:10.446373 disease-normalizer-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-02 17:57:59.000000 disease-normalizer-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 18:35:26.913700 disease-normalizer-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-01-11 18:35:26.913700 disease-normalizer-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 18:35:26.913700 disease-normalizer-0.3.1/disease/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 18:35:26.913700 disease-normalizer-0.3.1/disease/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/do.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/mondo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/ncit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/omim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/oncotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/etl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/disease/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 18:35:26.913700 disease-normalizer-0.3.1/disease_normalizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-01-11 18:35:26.000000 disease-normalizer-0.3.1/disease_normalizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-11 18:35:26.000000 disease-normalizer-0.3.1/disease_normalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 18:35:26.000000 disease-normalizer-0.3.1/disease_normalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 18:35:26.000000 disease-normalizer-0.3.1/disease_normalizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-11 18:35:26.000000 disease-normalizer-0.3.1/disease_normalizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-11 18:35:26.000000 disease-normalizer-0.3.1/disease_normalizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-01-11 18:35:26.913700 disease-normalizer-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-11 18:35:18.000000 disease-normalizer-0.3.1/setup.py
```

### Comparing `disease-normalizer-0.3.0/LICENSE` & `disease-normalizer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `disease-normalizer-0.3.0/PKG-INFO` & `disease-normalizer-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disease-normalizer
-Version: 0.3.0
+Version: 0.3.1
 Summary: VICC normalization routine for diseases
 Home-page: https://github.com/cancervariants/disease-normalization
 Author: VICC
 Author-email: help@cancervariants.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `disease-normalizer-0.3.0/README.md` & `disease-normalizer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `disease-normalizer-0.3.0/disease/__init__.py` & `disease-normalizer-0.3.1/disease/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 """The VICC library for normalizing diseases."""
-from pathlib import Path
 import logging
+from pathlib import Path
 
 from .version import __version__  # noqa: F401
 
-
 APP_ROOT = Path(__file__).resolve().parents[0]
 
 # set up logging
 logging.basicConfig(
     filename="disease.log",
-    format="[%(asctime)s] - %(name)s - %(levelname)s : %(message)s"
+    format="[%(asctime)s] - %(name)s - %(levelname)s : %(message)s",
 )
 logger = logging.getLogger("disease")
 logger.setLevel(logging.DEBUG)
 logger.handlers = []
 
 
 class DownloadException(Exception):
     """Exception for failures relating to source file downloads."""
 
     def __init__(self, *args, **kwargs):
         """Initialize exception."""
         super().__init__(*args, **kwargs)
 
 
-from disease.schemas import SourceName, SourceIDAfterNamespace, NamespacePrefix, ItemTypes  # noqa: E402 E501
+from disease.schemas import (  # noqa: E402 E501
+    ItemTypes,
+    NamespacePrefix,
+    SourceIDAfterNamespace,
+    SourceName,
+)
+
 ITEM_TYPES = {k.lower(): v.value for k, v in ItemTypes.__members__.items()}
 
 # use to lookup source name from lower-case string
 # technically the same as PREFIX_LOOKUP, but source namespace prefixes
 # sometimes differ from their names
 # e.g. {'ncit': 'NCIt'}
-SOURCES_LOWER_LOOKUP = {name.value.lower(): name.value for name in
-                        SourceName.__members__.values()}
+SOURCES_LOWER_LOOKUP = {
+    name.value.lower(): name.value for name in SourceName.__members__.values()
+}
 
 # use to fetch source name from schema based on concept id namespace
 # e.g. {'ncit': 'NCIt', 'doid': 'DO'}
-PREFIX_LOOKUP = {v.value.lower(): SourceName[k].value
-                 for k, v in NamespacePrefix.__members__.items()
-                 if k in SourceName.__members__.keys()}
+PREFIX_LOOKUP = {
+    v.value.lower(): SourceName[k].value
+    for k, v in NamespacePrefix.__members__.items()
+    if k in SourceName.__members__.keys()
+}
 
 # use to generate namespace prefix from source ID value
 # e.g. {'c': 'NCIt'}
-NAMESPACE_LOOKUP = {v.value.lower(): NamespacePrefix[k].value
-                    for k, v in SourceIDAfterNamespace.__members__.items()
-                    if v.value != ''}
+NAMESPACE_LOOKUP = {
+    v.value.lower(): NamespacePrefix[k].value
+    for k, v in SourceIDAfterNamespace.__members__.items()
+    if v.value != ""
+}
 
 # Use for checking whether to pull IDs for merge group generation
 SOURCES_FOR_MERGE = {SourceName.MONDO.value}
```

### Comparing `disease-normalizer-0.3.0/disease/cli.py` & `disease-normalizer-0.3.1/disease/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,62 @@
 """This module provides a CLI util to make updates to normalizer database."""
-from timeit import default_timer as timer
 from os import environ
-from typing import Optional, List
+from timeit import default_timer as timer
+from typing import List, Optional
 
 import click
-from botocore.exceptions import ClientError
 from boto3.dynamodb.conditions import Key
+from botocore.exceptions import ClientError
 
 from disease import logger
-from disease.schemas import SourceName
+from disease.database import (
+    AWS_ENV_VAR_NAME,
+    SKIP_AWS_DB_ENV_NAME,
+    VALID_AWS_ENV_NAMES,
+    Database,
+    confirm_aws_db_use,
+)
+from disease.etl import DO, OMIM, Mondo, NCIt, OncoTree  # noqa: F401
 from disease.etl.merge import Merge
-from disease.database import Database, confirm_aws_db_use, SKIP_AWS_DB_ENV_NAME, \
-    VALID_AWS_ENV_NAMES, AWS_ENV_VAR_NAME
-from disease.etl import Mondo, NCIt, DO, OncoTree, OMIM  # noqa: F401
-
+from disease.schemas import SourceName
 
 # Use to lookup class object from source name. Should be one key-value pair
 # for every functioning ETL class.
-SOURCES_CLASS_LOOKUP = {s.value.lower(): eval(s.value)
-                        for s in SourceName.__members__.values()}
+SOURCES_CLASS_LOOKUP = {
+    s.value.lower(): eval(s.value) for s in SourceName.__members__.values()
+}
 
 
 class CLI:
     """Class for updating the normalizer database via Click"""
 
     @staticmethod
     @click.command()
     @click.option(
-        '--normalizer',
-        help="The source(s) you wish to update separated by spaces."
+        "--normalizer", help="The source(s) you wish to update separated by spaces."
     )
     @click.option(
-        '--aws_instance',
+        "--aws_instance",
         help=" Must be `Dev`, `Staging`, or `Prod`. This determines the AWS instance to"
-             " use. `Dev` uses nonprod. `Staging` and `Prod` uses prod."
-    )
-    @click.option(
-        '--db_url',
-        help="URL endpoint for the application database."
-    )
-    @click.option(
-        '--update_all',
-        is_flag=True,
-        help='Update all normalizer sources.'
+        " use. `Dev` uses nonprod. `Staging` and `Prod` uses prod.",
     )
+    @click.option("--db_url", help="URL endpoint for the application database.")
+    @click.option("--update_all", is_flag=True, help="Update all normalizer sources.")
     @click.option(
-        '--update_merged',
-        is_flag=True,
-        help='Update concepts for /normalize endpoint.'
+        "--update_merged", is_flag=True, help="Update concepts for /normalize endpoint."
     )
     @click.option(
-        '--from_local',
+        "--from_local",
         is_flag=True,
         default=False,
-        help="Use most recent local source data instead of fetching latest versions."
+        help="Use most recent local source data instead of fetching latest versions.",
     )
-    def update_normalizer_db(normalizer, aws_instance, db_url, update_all,
-                             update_merged, from_local):
+    def update_normalizer_db(
+        normalizer, aws_instance, db_url, update_all, update_merged, from_local
+    ):
         """Update selected source(s) in the Disease Normalizer database."""
         # If SKIP_AWS_CONFIRMATION is accidentally set, we should verify that the
         # aws instance should actually be used
         invalid_aws_msg = f"{AWS_ENV_VAR_NAME} must be set to one of {VALID_AWS_ENV_NAMES}"  # noqa: E501
         aws_env_name = environ.get(AWS_ENV_VAR_NAME) or aws_instance
         if aws_env_name:
             assert aws_env_name in VALID_AWS_ENV_NAMES, invalid_aws_msg
@@ -86,16 +82,17 @@
             else:
                 CLI()._help_msg()
         else:
             sources_to_update = str(normalizer).lower().split()
             if len(sources_to_update) == 0:
                 CLI()._help_msg()
 
-            invalid_sources = set(sources_to_update) - {src for src
-                                                        in SOURCES_CLASS_LOOKUP}
+            invalid_sources = set(sources_to_update) - {
+                src for src in SOURCES_CLASS_LOOKUP
+            }
             if len(invalid_sources) != 0:
                 raise Exception(f"Not valid sources: {invalid_sources}")
 
             CLI()._update_sources(sources_to_update, db, update_merged, from_local)
 
     @staticmethod
     def _help_msg(message: Optional[str] = None):
@@ -103,46 +100,46 @@
         ctx = click.get_current_context()
         if message:
             click.echo(message)
         click.echo(ctx.get_help())
         ctx.exit()
 
     @staticmethod
-    def _update_sources(sources: List[str], db: Database, update_merged: bool,
-                        from_local: bool = False):
+    def _update_sources(
+        sources: List[str], db: Database, update_merged: bool, from_local: bool = False
+    ):
         """Update selected normalizer sources."""
         added_ids = []
-        for source in sources:
-            msg = f"Deleting {source}..."
+        for source_name in sources:
+            msg = f"Deleting {source_name}..."
             click.echo(f"\n{msg}")
             logger.info(msg)
             start_delete = timer()
-            CLI()._delete_data(source, db)
+            CLI()._delete_data(source_name, db)
             end_delete = timer()
             delete_time = end_delete - start_delete
-            msg = f"Deleted {source} in {delete_time:.5f} seconds."
+            msg = f"Deleted {source_name} in {delete_time:.5f} seconds."
             click.echo(f"{msg}\n")
             logger.info(msg)
 
-            msg = f"Loading {source}..."
+            msg = f"Loading {source_name}..."
             click.echo(msg)
             logger.info(msg)
             start_load = timer()
-            source = SOURCES_CLASS_LOOKUP[source](database=db)
+            source = SOURCES_CLASS_LOOKUP[source_name](database=db)
             if isinstance(source, Mondo):
                 added_ids = source.perform_etl(from_local)
             else:
                 source.perform_etl()
             end_load = timer()
             load_time = end_load - start_load
-            msg = f"Loaded {source} in {load_time:.5f} seconds."
+            msg = f"Loaded {source_name} in {load_time:.5f} seconds."
             click.echo(msg)
             logger.info(msg)
-            msg = f"Total time for {source}: " \
-                  f"{(delete_time + load_time):.5f} seconds."
+            msg = f"Total time for {source_name}: {(delete_time + load_time):.5f} seconds."  # noqa: E501
             click.echo(msg)
             logger.info(msg)
         if update_merged:
             CLI()._update_merged(db, added_ids)
 
     def _update_merged(self, db: Database, added_ids: List[str]) -> None:
         """Update merged concepts and references.
@@ -154,88 +151,95 @@
         if not added_ids:
             CLI()._delete_merged_data(db)
             added_ids = db.get_ids_for_merge()
         merge = Merge(database=db)
         click.echo("Constructing normalized records...")
         merge.create_merged_concepts(added_ids)
         end_merge = timer()
-        click.echo(f"Merged concept generation completed in"
-                   f" {(end_merge - start_merge):.5f} seconds.")
+        click.echo(
+            f"Merged concept generation completed in"
+            f" {(end_merge - start_merge):.5f} seconds."
+        )
 
     @staticmethod
     def _delete_merged_data(database: Database):
         """Delete data pertaining to merged records.
         :param database: DynamoDB client
         """
         click.echo("\nDeleting normalized records...")
         start_delete = timer()
         try:
             while True:
                 with database.diseases.batch_writer(
-                        overwrite_by_pkeys=["label_and_type", "concept_id"]) \
-                        as batch:
+                    overwrite_by_pkeys=["label_and_type", "concept_id"]
+                ) as batch:
                     response = database.diseases.query(
                         IndexName="type_index",
                         KeyConditionExpression=Key("item_type").eq("merger"),
                     )
                     records = response["Items"]
                     if not records:
                         break
                     for record in records:
-                        batch.delete_item(Key={
-                            "label_and_type": record["label_and_type"],
-                            "concept_id": record["concept_id"]
-                        })
+                        batch.delete_item(
+                            Key={
+                                "label_and_type": record["label_and_type"],
+                                "concept_id": record["concept_id"],
+                            }
+                        )
         except ClientError as e:
             click.echo(e.response["Error"]["Message"])
         end_delete = timer()
         delete_time = end_delete - start_delete
         click.echo(f"Deleted normalized records in {delete_time:.5f} seconds.")
 
     @staticmethod
     def _delete_data(source: str, database: Database):
         # Delete source's metadata
         try:
             metadata = database.metadata.query(
-                KeyConditionExpression=Key(
-                    'src_name').eq(SourceName[f"{source.upper()}"].value)
+                KeyConditionExpression=Key("src_name").eq(
+                    SourceName[f"{source.upper()}"].value
+                )
             )
-            if metadata['Items']:
+            if metadata["Items"]:
                 database.metadata.delete_item(
-                    Key={'src_name': metadata['Items'][0]['src_name']},
+                    Key={"src_name": metadata["Items"][0]["src_name"]},
                     ConditionExpression="src_name = :src",
                     ExpressionAttributeValues={
-                        ':src': SourceName[f"{source.upper()}"].value}
+                        ":src": SourceName[f"{source.upper()}"].value
+                    },
                 )
         except ClientError as e:
-            click.echo(e.response['Error']['Message'])
+            click.echo(e.response["Error"]["Message"])
 
         # Delete source's data from diseases table
         try:
             while True:
                 response = database.diseases.query(
-                    IndexName='src_index',
-                    KeyConditionExpression=Key('src_name').eq(
-                        SourceName[f"{source.upper()}"].value)
+                    IndexName="src_index",
+                    KeyConditionExpression=Key("src_name").eq(
+                        SourceName[f"{source.upper()}"].value
+                    ),
                 )
 
-                records = response['Items']
+                records = response["Items"]
                 if not records:
                     break
 
                 with database.diseases.batch_writer(
-                        overwrite_by_pkeys=['label_and_type', 'concept_id']) \
-                        as batch:
+                    overwrite_by_pkeys=["label_and_type", "concept_id"]
+                ) as batch:
 
                     for record in records:
                         batch.delete_item(
                             Key={
-                                'label_and_type': record['label_and_type'],
-                                'concept_id': record['concept_id']
+                                "label_and_type": record["label_and_type"],
+                                "concept_id": record["concept_id"],
                             }
                         )
         except ClientError as e:
-            click.echo(e.response['Error']['Message'])
+            click.echo(e.response["Error"]["Message"])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     CLI().update_normalizer_db()
```

### Comparing `disease-normalizer-0.3.0/disease/database.py` & `disease-normalizer-0.3.1/disease/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """This module creates the database."""
 import sys
-from os import environ
-from typing import Optional, Dict, List, Any
 from enum import Enum
+from os import environ
+from typing import Any, Dict, List, Optional
 
 import boto3
+import click
 from boto3.dynamodb.conditions import Key
 from botocore.exceptions import ClientError
-import click
 
 from disease import PREFIX_LOOKUP, logger
 
-
 # can be set to either `Dev`, `Staging`, or `Prod`
 # ONLY set when wanting to access aws instance
 AWS_ENV_VAR_NAME = "DISEASE_NORM_ENV"
 
 # Set to "true" if want to skip db confirmation check. Should ONLY be used for
 # deployment needs
 SKIP_AWS_DB_ENV_NAME = "SKIP_AWS_CONFIRMATION"
@@ -30,237 +29,204 @@
 
 
 VALID_AWS_ENV_NAMES = {v.value for v in AwsEnvName.__members__.values()}
 
 
 def confirm_aws_db_use(env_name: str) -> None:
     """Check to ensure that AWS instance should actually be used."""
-    if click.confirm(f"Are you sure you want to use the AWS {env_name} database?",
-                     default=False):
+    if click.confirm(
+        f"Are you sure you want to use the AWS {env_name} database?", default=False
+    ):
         click.echo(f"***DISEASE AWS {env_name.upper()} DATABASE IN USE***")
     else:
         click.echo("Exiting.")
         sys.exit()
 
 
 class Database:
     """The database class."""
 
-    def __init__(self, db_url: str = '', region_name: str = 'us-east-2'):
+    def __init__(self, db_url: str = "", region_name: str = "us-east-2"):
         """Initialize Database class.
 
         :param str db_url: database endpoint URL to connect to
         :param str region_name: AWS region name to use
         """
         disease_concepts_table = "disease_concepts"  # default
         disease_metadata_table = "disease_metadata"  # default
         if AWS_ENV_VAR_NAME in environ:
             aws_env = environ[AWS_ENV_VAR_NAME]
-            assert aws_env in VALID_AWS_ENV_NAMES, f"{AWS_ENV_VAR_NAME} must be one of {VALID_AWS_ENV_NAMES}"  # noqa: E501
+            assert (
+                aws_env in VALID_AWS_ENV_NAMES
+            ), f"{AWS_ENV_VAR_NAME} must be one of {VALID_AWS_ENV_NAMES}"  # noqa: E501
 
             skip_confirmation = environ.get(SKIP_AWS_DB_ENV_NAME)
-            if (not skip_confirmation) or (skip_confirmation and skip_confirmation != "true"):  # noqa: E501
+            if (not skip_confirmation) or (
+                skip_confirmation and skip_confirmation != "true"
+            ):
                 confirm_aws_db_use(environ[AWS_ENV_VAR_NAME])
 
-            boto_params = {
-                "region_name": region_name
-            }
+            boto_params = {"region_name": region_name}
 
             if aws_env == AwsEnvName.DEVELOPMENT:
                 disease_concepts_table = "disease_concepts_nonprod"
                 disease_metadata_table = "disease_metadata_nonprod"
         else:
             if db_url:
                 endpoint_url = db_url
-            elif 'DISEASE_NORM_DB_URL' in environ:
-                endpoint_url = environ['DISEASE_NORM_DB_URL']
+            elif "DISEASE_NORM_DB_URL" in environ:
+                endpoint_url = environ["DISEASE_NORM_DB_URL"]
             else:
-                endpoint_url = 'http://localhost:8000'
-            click.echo(f"***Using Disease Database Endpoint: "
-                       f"{endpoint_url}***")
-            boto_params = {
-                'region_name': region_name,
-                'endpoint_url': endpoint_url
-            }
-        self.dynamodb = boto3.resource('dynamodb', **boto_params)
-        self.dynamodb_client = boto3.client('dynamodb', **boto_params)
+                endpoint_url = "http://localhost:8000"
+            click.echo(f"***Using Disease Database Endpoint: " f"{endpoint_url}***")
+            boto_params = {"region_name": region_name, "endpoint_url": endpoint_url}
+        self.dynamodb = boto3.resource("dynamodb", **boto_params)
+        self.dynamodb_client = boto3.client("dynamodb", **boto_params)
 
         # Only create tables for local instance
         if not {AWS_ENV_VAR_NAME} & set(environ):
-            existing_tables = self.dynamodb_client.list_tables()['TableNames']
+            existing_tables = self.dynamodb_client.list_tables()["TableNames"]
             self.create_diseases_table(existing_tables)
             self.create_meta_data_table(existing_tables)
 
         self.diseases = self.dynamodb.Table(disease_concepts_table)
         self.metadata = self.dynamodb.Table(disease_metadata_table)
         self.batch = self.diseases.batch_writer()
         self.cached_sources = {}
 
     def create_diseases_table(self, existing_tables: List):
         """Create Diseases table if it doesn't already exist.
 
         :param List existing_tables: list of existing table names
         """
-        table_name = 'disease_concepts'
+        table_name = "disease_concepts"
         if table_name not in existing_tables:
             self.dynamodb.create_table(
                 TableName=table_name,
                 KeySchema=[
                     {
-                        'AttributeName': 'label_and_type',
-                        'KeyType': 'HASH'  # Partition key
+                        "AttributeName": "label_and_type",
+                        "KeyType": "HASH",  # Partition key
                     },
-                    {
-                        'AttributeName': 'concept_id',
-                        'KeyType': 'RANGE'  # Sort key
-                    }
+                    {"AttributeName": "concept_id", "KeyType": "RANGE"},  # Sort key
                 ],
                 AttributeDefinitions=[
-                    {
-                        'AttributeName': 'label_and_type',
-                        'AttributeType': 'S'
-                    },
-                    {
-                        'AttributeName': 'concept_id',
-                        'AttributeType': 'S'
-                    },
-                    {
-                        'AttributeName': 'src_name',
-                        'AttributeType': 'S'
-                    },
-                    {
-                        'AttributeName': 'item_type',
-                        'AttributeType': 'S'
-                    }
-
+                    {"AttributeName": "label_and_type", "AttributeType": "S"},
+                    {"AttributeName": "concept_id", "AttributeType": "S"},
+                    {"AttributeName": "src_name", "AttributeType": "S"},
+                    {"AttributeName": "item_type", "AttributeType": "S"},
                 ],
                 GlobalSecondaryIndexes=[
                     {
-                        'IndexName': 'src_index',
-                        'KeySchema': [
-                            {
-                                'AttributeName': 'src_name',
-                                'KeyType': 'HASH'
-                            }
-                        ],
-                        'Projection': {
-                            'ProjectionType': 'KEYS_ONLY'
+                        "IndexName": "src_index",
+                        "KeySchema": [{"AttributeName": "src_name", "KeyType": "HASH"}],
+                        "Projection": {"ProjectionType": "KEYS_ONLY"},
+                        "ProvisionedThroughput": {
+                            "ReadCapacityUnits": 10,
+                            "WriteCapacityUnits": 10,
                         },
-                        'ProvisionedThroughput': {
-                            'ReadCapacityUnits': 10,
-                            'WriteCapacityUnits': 10
-                        }
                     },
                     {
-                        'IndexName': 'type_index',
-                        'KeySchema': [
-                            {
-                                'AttributeName': 'item_type',
-                                'KeyType': 'HASH'
-                            }
+                        "IndexName": "type_index",
+                        "KeySchema": [
+                            {"AttributeName": "item_type", "KeyType": "HASH"}
                         ],
-                        'Projection': {
-                            'ProjectionType': 'KEYS_ONLY'
+                        "Projection": {"ProjectionType": "KEYS_ONLY"},
+                        "ProvisionedThroughput": {
+                            "ReadCapacityUnits": 10,
+                            "WriteCapacityUnits": 10,
                         },
-                        'ProvisionedThroughput': {
-                            'ReadCapacityUnits': 10,
-                            'WriteCapacityUnits': 10
-                        }
-                    }
+                    },
                 ],
                 ProvisionedThroughput={
-                    'ReadCapacityUnits': 10,
-                    'WriteCapacityUnits': 10
-                }
+                    "ReadCapacityUnits": 10,
+                    "WriteCapacityUnits": 10,
+                },
             )
 
     def create_meta_data_table(self, existing_tables: List):
         """Create MetaData table if not exists.
 
         :param List existing_tables: list of existing table names
         """
-        table_name = 'disease_metadata'
+        table_name = "disease_metadata"
         if table_name not in existing_tables:
             self.dynamodb.create_table(
                 TableName=table_name,
                 KeySchema=[
-                    {
-                        'AttributeName': 'src_name',
-                        'KeyType': 'HASH'  # Partition key
-                    }
+                    {"AttributeName": "src_name", "KeyType": "HASH"}  # Partition key
                 ],
                 AttributeDefinitions=[
-                    {
-                        'AttributeName': 'src_name',
-                        'AttributeType': 'S'
-                    },
+                    {"AttributeName": "src_name", "AttributeType": "S"},
                 ],
                 ProvisionedThroughput={
-                    'ReadCapacityUnits': 10,
-                    'WriteCapacityUnits': 10
-                }
+                    "ReadCapacityUnits": 10,
+                    "WriteCapacityUnits": 10,
+                },
             )
 
-    def get_record_by_id(self, concept_id: str,
-                         case_sensitive: bool = True,
-                         merge: bool = False) -> Optional[Dict]:
+    def get_record_by_id(
+        self, concept_id: str, case_sensitive: bool = True, merge: bool = False
+    ) -> Optional[Dict]:
         """Fetch record corresponding to provided concept ID
 
         :param str concept_id: concept ID for disease record
         :param bool case_sensitive: if true, performs exact lookup, which is
             more efficient. Otherwise, performs filter operation, which
             doesn't require correct casing.
         :param bool merge: if true, look for merged record; look for identity
             record otherwise.
         :return: complete disease record, if match is found; None otherwise
         """
         try:
             if merge:
-                pk = f'{concept_id.lower()}##merger'
+                pk = f"{concept_id.lower()}##merger"
             else:
-                pk = f'{concept_id.lower()}##identity'
+                pk = f"{concept_id.lower()}##identity"
             if case_sensitive:
-                match = self.diseases.get_item(Key={
-                    'label_and_type': pk,
-                    'concept_id': concept_id
-                })
-                return match['Item']
+                match = self.diseases.get_item(
+                    Key={"label_and_type": pk, "concept_id": concept_id}
+                )
+                return match["Item"]
             else:
-                exp = Key('label_and_type').eq(pk)
+                exp = Key("label_and_type").eq(pk)
                 response = self.diseases.query(KeyConditionExpression=exp)
-                return response['Items'][0]
+                return response["Items"][0]
         except ClientError as e:
-            logger.error(f"boto3 client error on get_records_by_id for "
-                         f"search term {concept_id}: "
-                         f"{e.response['Error']['Message']}")
+            logger.error(
+                f"boto3 client error on get_records_by_id for "
+                f"search term {concept_id}: "
+                f"{e.response['Error']['Message']}"
+            )
             return None
         except KeyError:  # record doesn't exist
             return None
         except IndexError:  # record doesn't exist
             return None
 
-    def get_records_by_type(self, query: str,
-                            match_type: str) -> List[Dict]:
+    def get_records_by_type(self, query: str, match_type: str) -> List[Dict]:
         """Retrieve records for given query and match type.
 
         :param query: string to match against
         :param str match_type: type of match to look for. Should be one
             of {"label", "alias", "xref", "associated_with"} (use
             `get_record_by_id` for concept ID lookup)
         :return: list of matching records. Empty if lookup fails.
         """
-        pk = f'{query}##{match_type.lower()}'
-        filter_exp = Key('label_and_type').eq(pk)
+        pk = f"{query}##{match_type.lower()}"
+        filter_exp = Key("label_and_type").eq(pk)
         try:
             matches = self.diseases.query(KeyConditionExpression=filter_exp)
-            return matches.get('Items', None)
+            return matches.get("Items", None)
         except ClientError as e:
-            logger.error(f"boto3 client error on get_records_by_type for "
-                         f"search term {query}: "
-                         f"{e.response['Error']['Message']}")
+            logger.error(
+                f"boto3 client error on get_records_by_type for "
+                f"search term {query}: "
+                f"{e.response['Error']['Message']}"
+            )
             return []
 
     def get_ids_for_merge(self) -> List[str]:
         """Retrieve concept IDs for use in generating normalized records.
         :return: List of concept IDs as strings.
         """
         last_evaluated_key = None
@@ -287,69 +253,78 @@
 
     def add_record(self, record: Dict, record_type: str = "identity"):
         """Add new record to database.
 
         :param Dict record: record to upload
         :param str record_type: type of record (either 'identity' or 'merger')
         """
-        id_prefix = record['concept_id'].split(':')[0].lower()
-        record['src_name'] = PREFIX_LOOKUP[id_prefix]
+        id_prefix = record["concept_id"].split(":")[0].lower()
+        record["src_name"] = PREFIX_LOOKUP[id_prefix]
         label_and_type = f'{record["concept_id"].lower()}##{record_type}'
-        record['label_and_type'] = label_and_type
-        record['item_type'] = record_type
+        record["label_and_type"] = label_and_type
+        record["item_type"] = record_type
         try:
             self.batch.put_item(Item=record)
         except ClientError as e:
-            logger.error("boto3 client error on add_record for "
-                         f"{record['concept_id']}: "
-                         f"{e.response['Error']['Message']}")
+            logger.error(
+                "boto3 client error on add_record for "
+                f"{record['concept_id']}: "
+                f"{e.response['Error']['Message']}"
+            )
 
     def add_ref_record(self, term: str, concept_id: str, ref_type: str):
         """Add auxiliary/reference record to database.
 
         :param str term: referent term
         :param str concept_id: concept ID to refer to
         :param str ref_type: one of {'alias', 'label', 'xref',
             'associated_with'}
         """
-        label_and_type = f'{term.lower()}##{ref_type}'
-        src_name = PREFIX_LOOKUP[concept_id.split(':')[0].lower()]
+        label_and_type = f"{term.lower()}##{ref_type}"
+        src_name = PREFIX_LOOKUP[concept_id.split(":")[0].lower()]
         record = {
-            'label_and_type': label_and_type,
-            'concept_id': concept_id.lower(),
-            'src_name': src_name,
-            'item_type': ref_type,
+            "label_and_type": label_and_type,
+            "concept_id": concept_id.lower(),
+            "src_name": src_name,
+            "item_type": ref_type,
         }
         try:
             self.batch.put_item(Item=record)
         except ClientError as e:
-            logger.error(f"boto3 client error adding reference {term} for "
-                         f"{concept_id} with match type {ref_type}: "
-                         f"{e.response['Error']['Message']}")
+            logger.error(
+                f"boto3 client error adding reference {term} for "
+                f"{concept_id} with match type {ref_type}: "
+                f"{e.response['Error']['Message']}"
+            )
 
-    def update_record(self, concept_id: str, field: str, new_value: Any,
-                      item_type: str = 'identity'):
+    def update_record(
+        self, concept_id: str, field: str, new_value: Any, item_type: str = "identity"
+    ):
         """Update the field of an individual record to a new value.
 
         :param str concept_id: record to update
         :param str field: name of field to update
         :param str new_value: new value
         :param str item_type: record type, one of {'identity', 'merger'}
         """
         key = {
-            'label_and_type': f'{concept_id.lower()}##{item_type}',
-            'concept_id': concept_id
+            "label_and_type": f"{concept_id.lower()}##{item_type}",
+            "concept_id": concept_id,
         }
         update_expression = f"set {field}=:r"
-        update_values = {':r': new_value}
+        update_values = {":r": new_value}
         try:
-            self.diseases.update_item(Key=key,
-                                      UpdateExpression=update_expression,
-                                      ExpressionAttributeValues=update_values)
+            self.diseases.update_item(
+                Key=key,
+                UpdateExpression=update_expression,
+                ExpressionAttributeValues=update_values,
+            )
         except ClientError as e:
-            logger.error(f"boto3 client error in `database.update_record()`: "
-                         f"{e.response['Error']['Message']}")
+            logger.error(
+                f"boto3 client error in `database.update_record()`: "
+                f"{e.response['Error']['Message']}"
+            )
 
     def flush_batch(self):
         """Flush internal batch_writer."""
         self.batch.__exit__(*sys.exc_info())
         self.batch = self.diseases.batch_writer()
```

### Comparing `disease-normalizer-0.3.0/disease/etl/base.py` & `disease-normalizer-0.3.1/disease/etl/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """A base class for extraction, transformation, and loading of data."""
+import ftplib
+import os
+import re
 import tempfile
 import zipfile
-import os
 from abc import ABC, abstractmethod
-from typing import Set, Dict, List, Optional, Callable
 from pathlib import Path
-import re
-import ftplib
+from typing import Callable, Dict, List, Optional, Set
 
-import owlready2 as owl
 import bioversions
 import requests
+from owlready2.rdflib_store import TripleLiteRDFlibGraph as RDFGraph
 
-from disease import SOURCES_FOR_MERGE, ITEM_TYPES, logger, APP_ROOT
+from disease import APP_ROOT, ITEM_TYPES, SOURCES_FOR_MERGE, logger
 from disease.database import Database
-from disease.schemas import Disease
 from disease.etl.utils import DownloadException
-
+from disease.schemas import Disease
 
 DEFAULT_DATA_PATH = APP_ROOT / "data"
 
 
 class Base(ABC):
     """The ETL base class."""
 
@@ -66,26 +65,31 @@
         """Provide simple callback function to extract the largest file within a given
         zipfile and save it within the appropriate data directory.
         :param Path dl_path: path to temp data file
         :param Path outfile_path: path to save file within
         """
         with zipfile.ZipFile(dl_path, "r") as zip_ref:
             if len(zip_ref.filelist) > 1:
-                files = sorted(zip_ref.filelist, key=lambda z: z.file_size,
-                               reverse=True)
+                files = sorted(
+                    zip_ref.filelist, key=lambda z: z.file_size, reverse=True
+                )
                 target = files[0]
             else:
                 target = zip_ref.filelist[0]
             target.filename = outfile_path.name
             zip_ref.extract(target, path=outfile_path.parent)
         os.remove(dl_path)
 
     @staticmethod
-    def _http_download(url: str, outfile_path: Path, headers: Optional[Dict] = None,
-                       handler: Optional[Callable[[Path, Path], None]] = None) -> None:
+    def _http_download(
+        url: str,
+        outfile_path: Path,
+        headers: Optional[Dict] = None,
+        handler: Optional[Callable[[Path, Path], None]] = None,
+    ) -> None:
         """Perform HTTP download of remote data file.
         :param str url: URL to retrieve file from
         :param Path outfile_path: path to where file should be saved. Must be an actual
             Path instance rather than merely a pathlike string.
         :param Optional[Dict] headers: Any needed HTTP headers to include in request
         :param Optional[Callable[[Path, Path], None]] handler: provide if downloaded
             file requires additional action, e.g. it's a zip file.
@@ -122,16 +126,17 @@
                 ftp.cwd(host_dir)
                 with open(self._src_dir / host_fn, "wb") as fp:
                     ftp.retrbinary(f"RETR {host_fn}", fp.write)
         except ftplib.all_errors as e:
             logger.error(f"FTP download failed: {e}")
             raise Exception(e)
 
-    def _parse_version(self, file_path: Path, pattern: Optional[re.Pattern] = None
-                       ) -> str:
+    def _parse_version(
+        self, file_path: Path, pattern: Optional[re.Pattern] = None
+    ) -> str:
         """Get version number from provided file path.
         :param Path file_path: path to located source data file
         :param Optional[re.Pattern] pattern: regex pattern to use
         :return: source data version
         :raises: FileNotFoundError if version parsing fails
         """
         if pattern is None:
@@ -184,72 +189,71 @@
     @abstractmethod
     def _load_meta(self, *args, **kwargs):
         raise NotImplementedError
 
     def _load_disease(self, disease: Dict):
         """Load individual disease record."""
         assert Disease(**disease)
-        concept_id = disease['concept_id']
+        concept_id = disease["concept_id"]
 
         for attr_type, item_type in ITEM_TYPES.items():
             if attr_type in disease:
                 value = disease[attr_type]
                 if value is not None and value != []:
                     if isinstance(value, str):
                         items = [value.lower()]
                     else:
                         disease[attr_type] = list(set(value))
                         items = {item.lower() for item in value}
-                        if attr_type == 'aliases':
+                        if attr_type == "aliases":
                             if len(items) > 20:
                                 logger.debug(f"{concept_id} has > 20 aliases.")
                                 del disease[attr_type]
                                 continue
 
                     for item in items:
-                        self.database.add_ref_record(item, concept_id,
-                                                     item_type)
+                        self.database.add_ref_record(item, concept_id, item_type)
                 else:
                     del disease[attr_type]
 
-        if 'pediatric_disease' in disease \
-                and disease['pediatric_disease'] is None:
-            del disease['pediatric_disease']
+        if "pediatric_disease" in disease and disease["pediatric_disease"] is None:
+            del disease["pediatric_disease"]
 
         self.database.add_record(disease)
         if self._store_ids:
             self._added_ids.append(concept_id)
 
 
 class OWLBase(Base):
     """Base class for sources that use OWL files."""
 
-    def _get_subclasses(self, uri: str) -> Set[str]:
+    def _get_subclasses(self, uri: str, graph: RDFGraph) -> Set[str]:
         """Retrieve URIs for all terms that are subclasses of given URI.
 
-        :param str uri: URI for class
+        :param uri: URI for class
+        :param graph: RDFLib graph of ontology default world
         :return: Set of URIs (strings) for all subclasses of `uri`
         """
-        graph = owl.default_world.as_rdflib_graph()
         query = f"""
             SELECT ?c WHERE {{
                 ?c rdfs:subClassOf* <{uri}>
             }}
             """
         return {item.c.toPython() for item in graph.query(query)}
 
-    def _get_by_property_value(self, prop: str,
-                               value: str) -> Set[str]:
+    def _get_by_property_value(
+        self, prop: str, value: str, graph: RDFGraph
+    ) -> Set[str]:
         """Get all classes with given value for a specific property.
 
-        :param str prop: property URI
-        :param str value: property value
+        :param prop: property URI
+        :param value: property value
+        :param graph: RDFLib graph of ontology default world
         :return: Set of URIs (as strings) matching given property/value
         """
-        graph = owl.default_world.as_rdflib_graph()
         query = f"""
             SELECT ?c WHERE {{
                 ?c <{prop}>
                 "{value}"
             }}
             """
         return {item.c.toPython() for item in graph.query(query)}
```

### Comparing `disease-normalizer-0.3.0/disease/etl/do.py` & `disease-normalizer-0.3.1/disease/etl/do.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Disease Ontology ETL module."""
-import owlready2 as owl
 import bioversions
+import owlready2 as owl
 
 from disease import PREFIX_LOOKUP, logger
-from disease.schemas import SourceMeta, SourceName, NamespacePrefix
 from disease.etl.base import OWLBase
-
+from disease.schemas import NamespacePrefix, SourceMeta, SourceName
 
 DO_PREFIX_LOOKUP = {
     "EFO": NamespacePrefix.EFO.value,
     "GARD": NamespacePrefix.GARD.value,
     "ICDO": NamespacePrefix.ICDO.value,
     "MESH": NamespacePrefix.MESH.value,
     "NCI": NamespacePrefix.NCIT.value,
@@ -31,43 +30,46 @@
         sources not added to Bioversions yet, or other special-case sources.
         :return: most recent version, as a str
         """
         return bioversions.get_version("disease ontology")
 
     def _download_data(self):
         """Download DO source file for loading into normalizer."""
-        logger.info('Retrieving source data for Disease Ontology')
+        logger.info("Retrieving source data for Disease Ontology")
         output_file = self._src_dir / f"do_{self._version}.owl"
-        self._http_download("http://purl.obolibrary.org/obo/doid/doid-merged.owl",
-                            output_file)
+        self._http_download(
+            "http://purl.obolibrary.org/obo/doid/doid-merged.owl", output_file
+        )
         logger.info("Successfully retrieved source data for Disease Ontology")
 
     def _load_meta(self):
         """Load metadata"""
         metadata_params = {
             "data_license": "CC0 1.0",
             "data_license_url": "https://creativecommons.org/publicdomain/zero/1.0/legalcode",  # noqa: E501
             "version": self._version,
             "data_url": "http://www.obofoundry.org/ontology/doid.html",
             "rdp_url": None,
             "data_license_attributes": {
                 "non_commercial": False,
                 "share_alike": False,
-                "attribution": False
-            }
+                "attribution": False,
+            },
         }
         assert SourceMeta(**metadata_params)
-        metadata_params['src_name'] = SourceName.DO.value
+        metadata_params["src_name"] = SourceName.DO.value
         self.database.metadata.put_item(Item=metadata_params)
 
     def _transform_data(self):
         """Transform source data and send to loading method."""
         do = owl.get_ontology(self._data_file.absolute().as_uri()).load()
-        disease_uri = 'http://purl.obolibrary.org/obo/DOID_4'
-        diseases = self._get_subclasses(disease_uri)
+        disease_uri = "http://purl.obolibrary.org/obo/DOID_4"
+        diseases = self._get_subclasses(
+            disease_uri, owl.default_world.as_rdflib_graph()
+        )
         for uri in diseases:
             disease_class = do.search(iri=uri)[0]
             if disease_class.deprecated:
                 continue
 
             concept_id = f"{NamespacePrefix.DO.value}:{uri.split('_')[-1]}"
             label = disease_class.label[0]
@@ -78,24 +80,24 @@
             else:
                 aliases = []
 
             xrefs = []
             associated_with = []
             db_associated_with = set(disease_class.hasDbXref)
             for xref in db_associated_with:
-                prefix, id_no = xref.split(':', 1)
+                prefix, id_no = xref.split(":", 1)
                 normed_prefix = DO_PREFIX_LOOKUP.get(prefix, None)
                 if normed_prefix:
-                    xref_no = f'{normed_prefix}:{id_no}'
+                    xref_no = f"{normed_prefix}:{id_no}"
                     if normed_prefix.lower() in PREFIX_LOOKUP:
                         xrefs.append(xref_no)
                     else:
                         associated_with.append(xref_no)
 
             disease = {
                 "concept_id": concept_id,
                 "label": label,
                 "aliases": aliases,
                 "xrefs": xrefs,
-                "associated_with": associated_with
+                "associated_with": associated_with,
             }
             self._load_disease(disease)
```

### Comparing `disease-normalizer-0.3.0/disease/etl/merge.py` & `disease-normalizer-0.3.1/disease/etl/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Create concept groups and merged records."""
+from timeit import default_timer as timer
+from typing import Dict, List, Set, Tuple
+
 from disease import logger
 from disease.database import Database
 from disease.schemas import SourcePriority
-from typing import Set, Dict, List
-from timeit import default_timer as timer
 
 
 class Merge:
     """Handles record merging."""
 
     def __init__(self, database: Database):
         """Initialize Merge instance.
@@ -22,97 +23,103 @@
         """Create concept groups, generate merged concept records, and
         update database.
 
         :param List[str] record_ids: concept identifiers from which groups
             should be generated.
         """
         # build groups
-        logger.info(f'Generating record ID sets from {len(record_ids)} records')  # noqa E501
+        logger.info(
+            f"Generating record ID sets from {len(record_ids)} records"
+        )  # noqa E501
         start = timer()
         for concept_id in record_ids:
             try:
                 record = self._database.get_record_by_id(concept_id)
             except AttributeError:
-                logger.error(f"`create_merged_concepts` received invalid "
-                             f"concept ID: {concept_id}")
+                logger.error(
+                    f"`create_merged_concepts` received invalid "
+                    f"concept ID: {concept_id}"
+                )
                 continue
             if not record:
-                logger.error(f"generate_merged_concepts couldn't find "
-                             f"{concept_id}")
+                logger.error(f"generate_merged_concepts couldn't find " f"{concept_id}")
                 continue
-            xrefs = record.get('xrefs', None)
+            xrefs = record.get("xrefs", None)
             if xrefs:
                 group = set(xrefs + [concept_id])
             else:
                 group = {concept_id}
             self._groups.append((concept_id, group))
         end = timer()
-        logger.debug(f'Built record ID sets in {end - start} seconds')
+        logger.debug(f"Built record ID sets in {end - start} seconds")
 
         # build merged concepts
-        logger.info('Creating merged records and updating database...')
+        logger.info("Creating merged records and updating database...")
         start = timer()
         for record_id, group in self._groups:
             try:
                 merged_record, merged_ids = self._generate_merged_record(group)
             except AttributeError:
-                logger.error("`create_merged_concepts` received invalid group:"
-                             f"{group} for concept {record_id}")
+                logger.error(
+                    "`create_merged_concepts` received invalid group:"
+                    f"{group} for concept {record_id}"
+                )
                 continue
-            self._database.add_record(merged_record, 'merger')
-            merge_ref = merged_record['concept_id'].lower()
+            self._database.add_record(merged_record, "merger")
+            merge_ref = merged_record["concept_id"].lower()
 
             for concept_id in merged_ids:
-                self._database.update_record(concept_id, 'merge_ref',
-                                             merge_ref)
+                self._database.update_record(concept_id, "merge_ref", merge_ref)
         end = timer()
         logger.info("merged concept generation successful.")
-        logger.debug(f'Generated and added concepts in {end - start} seconds)')
+        logger.debug(f"Generated and added concepts in {end - start} seconds)")
 
-    def _generate_merged_record(self, record_id_set: Set[str]) -> (Dict, List):
+    def _generate_merged_record(self, record_id_set: Set[str]) -> Tuple[Dict, List]:
         """Generate merged record from provided concept ID group.
         Where attributes are sets, they should be merged, and where they are
         scalars, assign from the highest-priority source where that attribute
         is non-null.
 
-        Priority is NCIt > Mondo > OncoTree> DO.
+        Priority is NCIt > Mondo > OMIM > OncoTree> DO.
 
         :param Set record_id_set: group of concept IDs
         :return: completed merged drug object to be stored in DB, as well as
             a list of the IDs ultimately included in said record
         """
         records = []
         final_ids = []
         for record_id in record_id_set:
             record = self._database.get_record_by_id(record_id)
             if record:
                 records.append(record)
-                final_ids.append(record['concept_id'])
+                final_ids.append(record["concept_id"])
             else:
-                logger.error(f"generate_merged_record could not retrieve "
-                             f"record for {record_id} in {record_id_set}")
+                logger.error(
+                    f"generate_merged_record could not retrieve "
+                    f"record for {record_id} in {record_id_set}"
+                )
 
         def record_order(record):
             """Provide priority values of concepts for sort function."""
-            src = record['src_name'].upper()
+            src = record["src_name"].upper()
             source_rank = SourcePriority[src].value
-            return source_rank, record['concept_id']
+            return source_rank, record["concept_id"]
+
         records.sort(key=record_order)
 
         merged_properties = {
-            'concept_id': records[0]['concept_id'],
-            'aliases': set(),
-            'associated_with': set()
+            "concept_id": records[0]["concept_id"],
+            "aliases": set(),
+            "associated_with": set(),
         }
         if len(records) > 1:
-            merged_properties['xrefs'] = [r['concept_id'] for r
-                                          in records[1:]]
+            merged_properties["xrefs"] = [r["concept_id"] for r in records[1:]]
 
-        set_fields = ['aliases', 'associated_with']
-        scalar_fields = ['label', 'pediatric_disease']
+        set_fields = ["aliases", "associated_with"]
+        scalar_fields = ["label", "pediatric_disease"]
         for record in records:
             for field in set_fields:
                 if field in record:
                     merged_properties[field] |= set(record[field])
             for field in scalar_fields:
                 if field not in merged_properties and field in record:
                     merged_properties[field] = record[field]
@@ -120,10 +127,11 @@
         for field in set_fields:
             field_value = merged_properties[field]
             if field_value:
                 merged_properties[field] = list(field_value)
             else:
                 del merged_properties[field]
 
-        merged_properties['label_and_type'] = \
-            f'{merged_properties["concept_id"].lower()}##merger'
+        merged_properties[
+            "label_and_type"
+        ] = f'{merged_properties["concept_id"].lower()}##merger'
         return merged_properties, final_ids
```

### Comparing `disease-normalizer-0.3.0/disease/etl/ncit.py` & `disease-normalizer-0.3.1/disease/etl/ncit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Module to load disease data from NCIt."""
-import requests
+import re
 from typing import Set
+
 import owlready2 as owl
-import re
+import requests
 
 from disease import logger
-from disease.schemas import SourceMeta, SourceName, NamespacePrefix
 from disease.etl.base import OWLBase
 from disease.etl.utils import DownloadException
-
+from disease.schemas import NamespacePrefix, SourceMeta, SourceName
 
 icdo_re = re.compile("[0-9]+/[0-9]+")
 
 
 class NCIt(OWLBase):
     """Gather and load data from NCIt."""
 
@@ -44,46 +44,52 @@
                     logger.error(msg)
                     raise DownloadException(msg)
                 else:
                     src_url = old_archive_url
             else:
                 src_url = archive_url
 
-        self._http_download(src_url, self._src_dir / f"ncit_{self._version}.owl",
-                            handler=self._zip_handler)
+        self._http_download(
+            src_url,
+            self._src_dir / f"ncit_{self._version}.owl",
+            handler=self._zip_handler,
+        )
         logger.info("Successfully retrieved source data for NCIt")
 
     def _load_meta(self):
         """Load metadata"""
-        metadata = SourceMeta(data_license="CC BY 4.0",
-                              data_license_url="https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa F401
-                              version=self._version,
-                              data_url="https://evs.nci.nih.gov/ftp1/NCI_Thesaurus/",
-                              rdp_url='http://reusabledata.org/ncit.html',
-                              data_license_attributes={
-                                  'non_commercial': False,
-                                  'share_alike': False,
-                                  'attribution': True
-                              })
+        metadata = SourceMeta(
+            data_license="CC BY 4.0",
+            data_license_url="https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa F401
+            version=self._version,
+            data_url="https://evs.nci.nih.gov/ftp1/NCI_Thesaurus/",
+            rdp_url="http://reusabledata.org/ncit.html",
+            data_license_attributes={
+                "non_commercial": False,
+                "share_alike": False,
+                "attribution": True,
+            },
+        )
         params = dict(metadata)
-        params['src_name'] = SourceName.NCIT.value
+        params["src_name"] = SourceName.NCIT.value
         self.database.metadata.put_item(Item=params)
 
     def _get_disease_classes(self) -> Set[str]:
         """Get all nodes with semantic_type 'Neoplastic Process' or 'Disease
         or Syndrome'.
 
         :return: uq_nodes with additions from above types added
         :rtype: Set[str]
         """
+        graph = owl.default_world.as_rdflib_graph()
         p106 = "http://ncicb.nci.nih.gov/xml/owl/EVS/Thesaurus.owl#P106"
-        neopl = self._get_by_property_value(p106, "Neoplastic Process")
-        dos = self._get_by_property_value(p106, "Disease or Syndrome")
+        neopl = self._get_by_property_value(p106, "Neoplastic Process", graph)
+        dos = self._get_by_property_value(p106, "Disease or Syndrome", graph)
         p310 = "http://ncicb.nci.nih.gov/xml/owl/EVS/Thesaurus.owl#P106"
-        retired = self._get_by_property_value(p310, "Retired_Concept")
+        retired = self._get_by_property_value(p310, "Retired_Concept", graph)
         uris = neopl.union(dos) - retired
         return uris
 
     def _transform_data(self):
         """Get data from file and construct object for loading."""
         ncit = owl.get_ontology(self._data_file.absolute().as_uri()).load()
         disease_uris = self._get_disease_classes()
@@ -95,28 +101,31 @@
             else:
                 logger.warning(f"No label for concept {concept_id}")
                 continue
             aliases = [a for a in disease_class.P90 if a != label]
 
             associated_with = []
             if disease_class.P207:
-                associated_with.append(f"{NamespacePrefix.UMLS.value}:"
-                                       f"{disease_class.P207.first()}")
+                associated_with.append(
+                    f"{NamespacePrefix.UMLS.value}:" f"{disease_class.P207.first()}"
+                )
             maps_to = disease_class.P375
             if maps_to:
                 icdo_list = list(filter(lambda s: icdo_re.match(s), maps_to))
                 if len(icdo_list) == 1:
-                    associated_with.append(f"{NamespacePrefix.ICDO.value}:"
-                                           f"{icdo_list[0]}")
+                    associated_with.append(
+                        f"{NamespacePrefix.ICDO.value}:" f"{icdo_list[0]}"
+                    )
             imdrf = disease_class.hasDbXref
             if imdrf:
-                associated_with.append(f"{NamespacePrefix.IMDRF.value}:"
-                                       f"{imdrf[0].split(':')[1]}")
+                associated_with.append(
+                    f"{NamespacePrefix.IMDRF.value}:" f"{imdrf[0].split(':')[1]}"
+                )
 
             disease = {
-                'concept_id': concept_id,
-                'src_name': SourceName.NCIT.value,
-                'label': label,
-                'aliases': aliases,
-                'associated_with': associated_with
+                "concept_id": concept_id,
+                "src_name": SourceName.NCIT.value,
+                "label": label,
+                "aliases": aliases,
+                "associated_with": associated_with,
             }
             self._load_disease(disease)
```

### Comparing `disease-normalizer-0.3.0/disease/etl/omim.py` & `disease-normalizer-0.3.1/disease/etl/omim.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module to load disease data from OMIM."""
-from .base import Base
 from disease import DownloadException, logger
-from disease.schemas import SourceMeta, SourceName, Disease, NamespacePrefix
+from disease.schemas import Disease, NamespacePrefix, SourceMeta, SourceName
+
+from .base import Base
 
 
 class OMIM(Base):
     """Gather and load data from OMIM."""
 
     def _extract_data(self, use_existing: bool = False):
         """Override parent extract method to enforce OMIM-specific data file
@@ -18,62 +19,68 @@
                 "Overruling provided `use_existing` parameter. OMIM data is not "
                 "publicly available - see README for details - and must be manually "
                 f"placed in {self._src_dir.absolute().as_uri()}"
             )
         try:
             super()._extract_data(True)
         except FileNotFoundError:
-            raise FileNotFoundError("Could not locate OMIM data. Per README, OMIM "
-                                    "source files must be manually placed in "
-                                    f"{self._src_dir.absolute().as_uri()}")
+            raise FileNotFoundError(
+                "Could not locate OMIM data. Per README, OMIM "
+                "source files must be manually placed in "
+                f"{self._src_dir.absolute().as_uri()}"
+            )
 
     def _download_data(self):
         """Download OMIM source data for loading into normalizer."""
         raise DownloadException("OMIM data not available for public download")
 
     def _load_meta(self):
         """Load source metadata."""
-        metadata = SourceMeta(data_license="custom",
-                              data_license_url="https://omim.org/help/agreement",
-                              version=self._data_file.stem.split('_', 1)[1],
-                              data_url="https://www.omim.org/downloads",
-                              rdp_url='http://reusabledata.org/omim.html',
-                              data_license_attributes={
-                                  'non_commercial': False,
-                                  'share_alike': True,
-                                  'attribution': True
-                              })
+        metadata = SourceMeta(
+            data_license="custom",
+            data_license_url="https://omim.org/help/agreement",
+            version=self._data_file.stem.split("_", 1)[1],
+            data_url="https://www.omim.org/downloads",
+            rdp_url="http://reusabledata.org/omim.html",
+            data_license_attributes={
+                "non_commercial": False,
+                "share_alike": True,
+                "attribution": True,
+            },
+        )
         params = dict(metadata)
-        params['src_name'] = SourceName.OMIM.value
+        params["src_name"] = SourceName.OMIM.value
         self.database.metadata.put_item(Item=params)
 
     def _transform_data(self):
         """Modulate data and prepare for loading."""
-        with open(self._data_file, 'r') as f:
+        with open(self._data_file, "r") as f:
             rows = f.readlines()
-        rows = [r.rstrip() for r in rows if not r.startswith('#')]
-        rows = [[g for g in r.split('\t')] for r in rows]
-        rows = [r for r in rows if r[0] not in ('Asterisk', 'Caret', 'Plus')]
+        rows = [r.rstrip() for r in rows if not r.startswith("#")]
+        rows = [[g for g in r.split("\t")] for r in rows]
+        rows = [r for r in rows if r[0] not in ("Asterisk", "Caret", "Plus")]
         for row in rows:
             disease = {
-                'concept_id': f'{NamespacePrefix.OMIM.value}:{row[1]}',
+                "concept_id": f"{NamespacePrefix.OMIM.value}:{row[1]}",
             }
             aliases = set()
 
             label_item = row[2]
-            if ';' in label_item:
-                label_split = label_item.split(';')
-                disease['label'] = label_split[0]
+            if ";" in label_item:
+                label_split = label_item.split(";")
+                disease["label"] = label_split[0]
                 aliases.add(label_split[1])
             else:
-                disease['label'] = row[2]
+                disease["label"] = row[2]
 
             if len(row) > 3:
-                aliases |= {t for t in row[3].split(';') if t}
+                aliases |= {t for t in row[3].split(";") if t}
             if len(row) > 4:
-                aliases |= {t for t in row[4].split(';') if t}
-            aliases = {alias[:-10] if alias.endswith(', INCLUDED') else alias
-                       for alias in aliases}
-            disease['aliases'] = [a.lstrip() for a in aliases]
+                aliases |= {t for t in row[4].split(";") if t}
+            aliases = {
+                alias[:-10] if alias.endswith(", INCLUDED") else alias
+                for alias in aliases
+            }
+            disease["aliases"] = [a.lstrip() for a in aliases]
 
             assert Disease(**disease)
             self._load_disease(disease)
```

### Comparing `disease-normalizer-0.3.0/disease/etl/oncotree.py` & `disease-normalizer-0.3.1/disease/etl/oncotree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 """Module to load disease data from OncoTree."""
 import json
 
-from .base import Base
 from disease import logger
-from disease.schemas import SourceMeta, SourceName, NamespacePrefix, Disease
+from disease.schemas import Disease, NamespacePrefix, SourceMeta, SourceName
+
+from .base import Base
 
 
 class OncoTree(Base):
     """Gather and load data from OncoTree."""
 
     def _download_data(self):
         """Download Oncotree source data for loading into normalizer."""
-        logger.info('Retrieving source data for OncoTree')
+        logger.info("Retrieving source data for OncoTree")
         url_version = self._version.replace("-", "_")
-        url = f'http://oncotree.mskcc.org/api/tumorTypes/tree?version=oncotree_{url_version}'  # noqa: E501
+        url = f"http://oncotree.mskcc.org/api/tumorTypes/tree?version=oncotree_{url_version}"  # noqa: E501
         output_file = self._src_dir / f"oncotree_{self._version}.json"
         self._http_download(url, output_file)
-        logger.info('Successfully retrieved source data for OncoTree')
+        logger.info("Successfully retrieved source data for OncoTree")
 
     def _load_meta(self):
         """Load metadata"""
-        metadata = SourceMeta(data_license="CC BY 4.0",
-                              data_license_url="https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa F401
-                              version=self._version,
-                              data_url="http://oncotree.mskcc.org/#/home?tab=api",  # noqa: E501
-                              rdp_url=None,
-                              data_license_attributes={
-                                  'non_commercial': False,
-                                  'share_alike': False,
-                                  'attribution': True
-                              })
+        metadata = SourceMeta(
+            data_license="CC BY 4.0",
+            data_license_url="https://creativecommons.org/licenses/by/4.0/legalcode",
+            version=self._version,
+            data_url="http://oncotree.mskcc.org/#/home?tab=api",
+            rdp_url=None,
+            data_license_attributes={
+                "non_commercial": False,
+                "share_alike": False,
+                "attribution": True,
+            },
+        )
         params = dict(metadata)
-        params['src_name'] = SourceName.ONCOTREE.value
+        params["src_name"] = SourceName.ONCOTREE.value
         self.database.metadata.put_item(Item=params)
 
     def _traverse_tree(self, disease_node):
         """Traverse JSON tree and load diseases where possible.
 
         :param Dict disease_node: node in tree containing info for individual
             disease.
         """
-        if disease_node.get('level', None) >= 2:
+        if disease_node.get("level", None) >= 2:
             disease = {
                 "concept_id": f"{NamespacePrefix.ONCOTREE.value}:{disease_node['code']}",  # noqa: E501
-                "label": disease_node['name'],
+                "label": disease_node["name"],
                 "xrefs": [],
                 "associated_with": [],
             }
-            refs = disease_node.get('externalReferences', [])
+            refs = disease_node.get("externalReferences", [])
             for prefix, codes in refs.items():
-                if prefix == 'UMLS':
+                if prefix == "UMLS":
                     normed_prefix = NamespacePrefix.UMLS.value
                     for code in codes:
                         normed_id = f"{normed_prefix}:{code}"
-                        disease['associated_with'].append(normed_id)
-                elif prefix == 'NCI':
+                        disease["associated_with"].append(normed_id)
+                elif prefix == "NCI":
                     normed_prefix = NamespacePrefix.NCIT.value
                     for code in codes:
                         normed_id = f"{normed_prefix}:{code}"
-                        disease['xrefs'].append(normed_id)
+                        disease["xrefs"].append(normed_id)
                 else:
                     logger.warning(f"Unrecognized prefix: {prefix}")
                     continue
             assert Disease(**disease)
             self._load_disease(disease)
-        if disease_node.get('children', None):
-            for child in disease_node['children'].values():
+        if disease_node.get("children", None):
+            for child in disease_node["children"].values():
                 self._traverse_tree(child)
 
     def _transform_data(self):
         """Initiate OncoTree data transformation."""
-        with open(self._data_file, 'r') as f:
+        with open(self._data_file, "r") as f:
             oncotree = json.load(f)
-        self._traverse_tree(oncotree['TISSUE'])
+        self._traverse_tree(oncotree["TISSUE"])
```

### Comparing `disease-normalizer-0.3.0/disease/main.py` & `disease-normalizer-0.3.1/disease/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,117 @@
 """Main application for FastAPI"""
-from disease import __version__
-from disease.query import QueryHandler, InvalidParameterException
-from disease.schemas import SearchService, NormalizationService
-from fastapi import FastAPI, HTTPException, Query
-from fastapi.openapi.utils import get_openapi
 import html
 from typing import Optional
 
+from fastapi import FastAPI, HTTPException, Query
+from fastapi.openapi.utils import get_openapi
+
+from disease import __version__
+from disease.query import InvalidParameterException, QueryHandler
+from disease.schemas import NormalizationService, SearchService
 
 query_handler = QueryHandler()
 app = FastAPI(
     docs_url="/disease",
     openapi_url="/disease/openapi.json",
-    swagger_ui_parameters={"tryItOutEnabled": True}
+    swagger_ui_parameters={"tryItOutEnabled": True},
 )
 
 
 def custom_openapi():
     """Generate custom fields for OpenAPI response"""
     if app.openapi_schema:
         return app.openapi_schema
     openapi_schema = get_openapi(
         title="The VICC Disease Normalizer",
         version=__version__,
         openapi_version="3.0.3",
         description="Normalize disease terms.",
-        routes=app.routes
+        routes=app.routes,
     )
-#    openapi_schema['info']['license'] = {  # TODO
-#        "name": "Name-of-license",
-#        "url": "http://www.to-be-determined.com"
-#    }
-    openapi_schema['info']['contact'] = {
+    #    openapi_schema['info']['license'] = {  # TODO
+    #        "name": "Name-of-license",
+    #        "url": "http://www.to-be-determined.com"
+    #    }
+    openapi_schema["info"]["contact"] = {
         "name": "Alex H. Wagner",
         "email": "Alex.Wagner@nationwidechildrens.org",
-        "url": "https://www.nationwidechildrens.org/specialties/institute-for-genomic-medicine/research-labs/wagner-lab"  # noqa: E501
+        "url": "https://www.nationwidechildrens.org/specialties/institute-for-genomic-medicine/research-labs/wagner-lab",  # noqa: E501
     }
     app.openapi_schema = openapi_schema
     return app.openapi_schema
 
 
 app.openapi = custom_openapi
 
 # endpoint description text
-get_matches_summary = ("Given query, provide highest matches from "
-                       "each source.")
+get_matches_summary = "Given query, provide highest matches from " "each source."
 search_descr = "Search for disease term."
 response_descr = "A response to a validly-formed query."
 q_descr = "Disease term to search for."
-keyed_descr = ("If true, return response as key-value pairs of "
-               "sources to source matches. False by default")
-incl_descr = ("Comma-separated list of source names to include in "
-              "response. Will exclude all other sources. Will return HTTP "
-              "status code 422: Unprocessable Entity if both 'incl' and "
-              "'excl' parameters are given.")
-excl_descr = ("Comma-separated list of source names to exclude in "
-              "response. Will include all other sources. Will return HTTP "
-              "status code 422: Unprocessable Entity if both 'incl' and"
-              "'excl' parameters are given.")
-normalize_description = ("Return merged strongest-match concept for query "
-                         "string provided by user.")
-
-
-@app.get("/disease/search",
-         summary=get_matches_summary,
-         description=search_descr,
-         operation_id="getQueryResponse",
-         response_description=response_descr,
-         response_model=SearchService)
-def search(q: str = Query(..., description=q_descr),
-           keyed: Optional[bool] = Query(False, description=keyed_descr),
-           incl: Optional[str] = Query('', description=incl_descr),
-           excl: Optional[str] = Query('', description=excl_descr)):
+keyed_descr = (
+    "If true, return response as key-value pairs of "
+    "sources to source matches. False by default"
+)
+incl_descr = (
+    "Comma-separated list of source names to include in "
+    "response. Will exclude all other sources. Will return HTTP "
+    "status code 422: Unprocessable Entity if both 'incl' and "
+    "'excl' parameters are given."
+)
+excl_descr = (
+    "Comma-separated list of source names to exclude in "
+    "response. Will include all other sources. Will return HTTP "
+    "status code 422: Unprocessable Entity if both 'incl' and"
+    "'excl' parameters are given."
+)
+normalize_description = (
+    "Return merged strongest-match concept for query " "string provided by user."
+)
+
+
+@app.get(
+    "/disease/search",
+    summary=get_matches_summary,
+    description=search_descr,
+    operation_id="getQueryResponse",
+    response_description=response_descr,
+    response_model=SearchService,
+)
+def search(
+    q: str = Query(..., description=q_descr),
+    keyed: Optional[bool] = Query(False, description=keyed_descr),
+    incl: Optional[str] = Query("", description=incl_descr),
+    excl: Optional[str] = Query("", description=excl_descr),
+):
     """For each source, return strongest-match concepts for query string
     provided by user.
     """
     try:
-        response = query_handler.search(html.unescape(q), keyed=keyed,
-                                        incl=incl, excl=excl)
+        response = query_handler.search(
+            html.unescape(q), keyed=keyed, incl=incl, excl=excl
+        )
     except InvalidParameterException as e:
         raise HTTPException(status_code=422, detail=str(e))
     return response
 
 
 merged_matches_summary = "Given query, provide normalized record."
 merged_response_descr = "A response to a validly-formed query."
 merged_q_descr = "Disease to normalize."
 
 
-@app.get("/disease/normalize",
-         summary=merged_matches_summary,
-         operation_id="getQuerymergedResponse",
-         response_description=merged_response_descr,
-         response_model=NormalizationService,
-         description=normalize_description)
+@app.get(
+    "/disease/normalize",
+    summary=merged_matches_summary,
+    operation_id="getQuerymergedResponse",
+    response_description=merged_response_descr,
+    response_model=NormalizationService,
+    description=normalize_description,
+)
 def normalize(q: str = Query(..., description=merged_q_descr)):
     """Return strongest-match normalized concept for query string provided by
     user.
     :param q: therapy search term
     """
     try:
         response = query_handler.normalize(q)
```

### Comparing `disease-normalizer-0.3.0/disease/query.py` & `disease-normalizer-0.3.1/disease/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 """This module provides methods for handling queries."""
 import re
-from typing import Dict, Set, Optional, Tuple
-from .version import __version__
-from disease import NAMESPACE_LOOKUP, PREFIX_LOOKUP, SOURCES_LOWER_LOOKUP,\
-    ITEM_TYPES, logger
-from disease.database import Database
-from disease.schemas import Disease, SourceMeta, MatchType, SourceName, \
-    ServiceMeta, NormalizationService, SearchService
-from botocore.exceptions import ClientError
-from urllib.parse import quote
 from datetime import datetime
+from typing import Dict, Optional, Set, Tuple
+from urllib.parse import quote
+
+from botocore.exceptions import ClientError
+
+from disease import (
+    ITEM_TYPES,
+    NAMESPACE_LOOKUP,
+    PREFIX_LOOKUP,
+    SOURCES_LOWER_LOOKUP,
+    logger,
+)
+from disease.database import Database
+from disease.schemas import (
+    Disease,
+    MatchType,
+    NormalizationService,
+    SearchService,
+    ServiceMeta,
+    SourceMeta,
+    SourceName,
+)
+
+from .version import __version__
 
 
 class InvalidParameterException(Exception):
     """Exception for invalid parameter args provided by the user."""
 
     def __init__(self, message):
         """Create new instance
@@ -23,203 +38,194 @@
 
 
 class QueryHandler:
     """Class for normalizer management. Stores reference to database instance
     and normalizes query input.
     """
 
-    def __init__(self, db_url: str = '', db_region: str = 'us-east-2'):
+    def __init__(self, db_url: str = "", db_region: str = "us-east-2"):
         """Initialize Normalizer instance.
         :param str db_url: URL to database source.
         :param str db_region: AWS default region.
         """
         self.db = Database(db_url=db_url, region_name=db_region)
 
     def _emit_warnings(self, query_str) -> Optional[Dict]:
         """Emit warnings if query contains non breaking space characters.
         :param str query_str: query string
         :return: dict keying warning type to warning description
         """
         warnings = None
-        nbsp = re.search('\xa0|&nbsp;', query_str)
+        nbsp = re.search("\xa0|&nbsp;", query_str)
         if nbsp:
-            warnings = {
-                'nbsp': 'Query contains non breaking space characters.'
-            }
+            warnings = {"nbsp": "Query contains non breaking space characters."}
             logger.warning(
-                f'Query ({query_str}) contains non breaking space characters.'
+                f"Query ({query_str}) contains non breaking space characters."
             )
         return warnings
 
     def _fetch_meta(self, src_name: str) -> SourceMeta:
         """Fetch metadata for src_name.
         :param str src_name: name of source to get metadata for
         :return: Meta object containing source metadata
         """
         if src_name in self.db.cached_sources.keys():
             return self.db.cached_sources[src_name]
         else:
             try:
-                db_response = self.db.metadata.get_item(
-                    Key={'src_name': src_name}
-                )
-                response = SourceMeta(**db_response['Item'])
+                db_response = self.db.metadata.get_item(Key={"src_name": src_name})
+                response = SourceMeta(**db_response["Item"])
                 self.db.cached_sources[src_name] = response
                 return response
             except ClientError as e:
-                logger.error(e.response['Error']['Message'])
+                logger.error(e.response["Error"]["Message"])
 
-    def _add_record(self,
-                    response: Dict[str, Dict],
-                    item: Dict,
-                    match_type: str) -> Tuple[Dict, str]:
+    def _add_record(
+        self, response: Dict[str, Dict], item: Dict, match_type: str
+    ) -> Tuple[Dict, str]:
         """Add individual record to response object
         :param Dict[str, Dict] response: in-progress response object to return
             to client
         :param Dict item: Item retrieved from DynamoDB
         :param str match_type: type of query match
         :return: Tuple containing updated response object, and string
             containing name of the source of the match
         """
-        del item['label_and_type']
+        del item["label_and_type"]
         disease = Disease(**item)
-        src_name = item['src_name']
+        src_name = item["src_name"]
 
-        matches = response['source_matches']
+        matches = response["source_matches"]
         if src_name not in matches.keys():
             pass
         elif matches[src_name] is None:
             matches[src_name] = {
-                'match_type': MatchType[match_type.upper()],
-                'records': [disease],
-                'source_meta_': self._fetch_meta(src_name)
+                "match_type": MatchType[match_type.upper()],
+                "records": [disease],
+                "source_meta_": self._fetch_meta(src_name),
             }
-        elif matches[src_name]['match_type'] == MatchType[match_type.upper()]:
-            matches[src_name]['records'].append(disease)
+        elif matches[src_name]["match_type"] == MatchType[match_type.upper()]:
+            matches[src_name]["records"].append(disease)
 
         return response, src_name
 
-    def _fetch_records(self,
-                       response: Dict[str, Dict],
-                       concept_ids: Set[str],
-                       match_type: str) -> Tuple[Dict, Set]:
+    def _fetch_records(
+        self, response: Dict[str, Dict], concept_ids: Set[str], match_type: str
+    ) -> Tuple[Dict, Set]:
         """Return matched Disease records as a structured response for a given
         collection of concept IDs.
         :param Dict[str, Dict] response: in-progress response object to return
             to client.
         :param List[str] concept_ids: List of concept IDs to build from.
             Should be all lower-case.
         :param str match_type: record should be assigned this type of
             match.
         :return: response Dict with records filled in via provided concept
             IDs, and Set of source names of matched records
         """
         matched_sources = set()
         for concept_id in concept_ids:
             try:
-                match = self.db.get_record_by_id(concept_id.lower(),
-                                                 case_sensitive=False)
-                (response, src) = self._add_record(response, match, match_type)
-                matched_sources.add(src)
+                match = self.db.get_record_by_id(
+                    concept_id.lower(), case_sensitive=False
+                )
+                if match is None:
+                    logger.error(f"Reference to {concept_id} failed.")
+                else:
+                    (response, src) = self._add_record(response, match, match_type)
+                    matched_sources.add(src)
             except ClientError as e:
-                logger.error(e.response['Error']['Message'])
+                logger.error(e.response["Error"]["Message"])
         return response, matched_sources
 
     def _fill_no_matches(self, resp: Dict[str, Dict]) -> Dict:
         """Fill all empty source_matches slots with NO_MATCH results.
         :param Dict[str, Dict] resp: incoming response object
         :return: response object with empty source slots filled with
                 NO_MATCH results and corresponding source metadata
         """
-        for src_name in resp['source_matches'].keys():
-            if resp['source_matches'][src_name] is None:
-                resp['source_matches'][src_name] = {
-                    'match_type': MatchType.NO_MATCH,
-                    'records': [],
-                    'source_meta_': self._fetch_meta(src_name)
+        for src_name in resp["source_matches"].keys():
+            if resp["source_matches"][src_name] is None:
+                resp["source_matches"][src_name] = {
+                    "match_type": MatchType.NO_MATCH,
+                    "records": [],
+                    "source_meta_": self._fetch_meta(src_name),
                 }
         return resp
 
-    def _check_concept_id(self,
-                          query: str,
-                          resp: Dict,
-                          sources: Set[str]) -> (Dict, Set):
+    def _check_concept_id(
+        self, query: str, resp: Dict, sources: Set[str]
+    ) -> (Dict, Set):
         """Check query for concept ID match. Should only find 0 or 1 matches.
         :param str query: search string
         :param Dict resp: in-progress response object to return to client
         :param Set[str] sources: remaining unmatched sources
         :return: Tuple with updated resp object and updated set of unmatched
             sources
         """
         concept_id_items = []
         if [p for p in PREFIX_LOOKUP.keys() if query.startswith(p)]:
             record = self.db.get_record_by_id(query, False)
             if record:
                 concept_id_items.append(record)
-        for prefix in [p for p in NAMESPACE_LOOKUP.keys()
-                       if query.startswith(p)]:
-            concept_id = f'{NAMESPACE_LOOKUP[prefix]}:{query}'
+        for prefix in [p for p in NAMESPACE_LOOKUP.keys() if query.startswith(p)]:
+            concept_id = f"{NAMESPACE_LOOKUP[prefix]}:{query}"
             id_lookup = self.db.get_record_by_id(concept_id, False)
             if id_lookup:
                 concept_id_items.append(id_lookup)
         for item in concept_id_items:
-            (resp, src_name) = self._add_record(resp, item,
-                                                MatchType.CONCEPT_ID.name)
+            (resp, src_name) = self._add_record(resp, item, MatchType.CONCEPT_ID.name)
             sources = sources - {src_name}
         return resp, sources
 
-    def _check_match_type(self,
-                          query: str,
-                          resp: Dict,
-                          sources: Set[str],
-                          match_type: str) -> Tuple[Dict, Set]:
+    def _check_match_type(
+        self, query: str, resp: Dict, sources: Set[str], match_type: str
+    ) -> Tuple[Dict, Set]:
         """Check query for selected match type.
         :param str query: search string
         :param Dict resp: in-progress response object to return to client
         :param Set[str] sources: remaining unmatched sources
         :param str match_type: Match type to check for. Should be one of
             {'label', 'alias', 'xref', 'associated_with'}
         :return: Tuple with updated resp object and updated set of unmatched
                  sources
         """
         matches = self.db.get_records_by_type(query, match_type)
         if matches:
-            concept_ids = {i['concept_id'] for i in matches}
-            (resp, matched_srcs) = self._fetch_records(resp, concept_ids,
-                                                       match_type)
+            concept_ids = {i["concept_id"] for i in matches}
+            (resp, matched_srcs) = self._fetch_records(resp, concept_ids, match_type)
             sources = sources - matched_srcs
         return resp, sources
 
     def _response_keyed(self, query: str, sources: Set[str]) -> Dict:
         """Return response as dict where key is source name and value
         is a list of records. Corresponds to `keyed=true` API parameter.
         :param str query: string to match against
         :param Set[str] sources: sources to match from
         :return: completed response object to return to client
         """
         response = {
-            'query': query,
-            'warnings': self._emit_warnings(query),
-            'source_matches': {
-                source: None for source in sources
-            }
+            "query": query,
+            "warnings": self._emit_warnings(query),
+            "source_matches": {source: None for source in sources},
         }
-        if query == '':
+        if query == "":
             response = self._fill_no_matches(response)
             return response
         query = query.lower()
 
         # check if concept ID match
         (response, sources) = self._check_concept_id(query, response, sources)
         if len(sources) == 0:
             return response
 
         for match_type in ITEM_TYPES.values():
-            (response, sources) = self._check_match_type(query, response,
-                                                         sources, match_type)
+            (response, sources) = self._check_match_type(
+                query, response, sources, match_type
+            )
             if len(sources) == 0:
                 return response
 
         # remaining sources get no match
         return self._fill_no_matches(response)
 
     def _response_list(self, query: str, sources: Set[str]) -> Dict:
@@ -227,28 +233,27 @@
         is the source name. Corresponds to `keyed=false` API parameter.
         :param str query: string to match against
         :param Set[str] sources: sources to match from
         :return: Completed response object to return to client
         """
         response_dict = self._response_keyed(query, sources)
         source_list = []
-        for src_name in response_dict['source_matches'].keys():
+        for src_name in response_dict["source_matches"].keys():
             src = {
                 "source": src_name,
             }
-            to_merge = response_dict['source_matches'][src_name]
+            to_merge = response_dict["source_matches"][src_name]
             src.update(to_merge)
 
             source_list.append(src)
-        response_dict['source_matches'] = source_list
+        response_dict["source_matches"] = source_list
 
         return response_dict
 
-    def search(self, query_str, keyed=False, incl="",
-               excl="") -> SearchService:
+    def search(self, query_str, keyed=False, incl="", excl="") -> SearchService:
         """Fetch normalized disease objects.
         :param str query_str: query, a string, to search for
         :param bool keyed: if true, return response as dict keying source names
             to source objects; otherwise, return list of source objects
         :param str incl: str containing comma-separated names of sources to
             use. Will exclude all other sources. Case-insensitive.
         :param str excl: str containing comma-separated names of source to
@@ -256,35 +261,35 @@
         :return: dict containing all matches found in sources.
         :rtype: dict
         :raises InvalidParameterException: if both incl and excl args are
             provided, or if invalid source names are given.
         """
         sources = dict()
         for k, v in SOURCES_LOWER_LOOKUP.items():
-            if self.db.metadata.get_item(Key={'src_name': v}).get('Item'):
+            if self.db.metadata.get_item(Key={"src_name": v}).get("Item"):
                 sources[k] = v
         if not incl and not excl:
             query_sources = set(sources.values())
         elif incl and excl:
             detail = "Cannot request both source inclusions and exclusions."
             raise InvalidParameterException(detail)
         elif incl:
-            req_sources = [n.strip() for n in incl.split(',')]
+            req_sources = [n.strip() for n in incl.split(",")]
             invalid_sources = []
             query_sources = set()
             for source in req_sources:
                 if source.lower() in sources.keys():
                     query_sources.add(sources[source.lower()])
                 else:
                     invalid_sources.append(source)
             if invalid_sources:
                 detail = f"Invalid source name(s): {invalid_sources}"
                 raise InvalidParameterException(detail)
         else:
-            req_exclusions = [n.strip() for n in excl.lower().split(',')]
+            req_exclusions = [n.strip() for n in excl.lower().split(",")]
             req_excl_dict = {r.lower(): r for r in req_exclusions}
             invalid_sources = []
             query_sources = set()
             for req_l, req in req_excl_dict.items():
                 if req_l not in sources.keys():
                     invalid_sources.append(req)
             for src_l, src in sources.items():
@@ -297,188 +302,190 @@
         query_str = query_str.strip()
 
         if keyed:
             response = self._response_keyed(query_str, query_sources)
         else:
             response = self._response_list(query_str, query_sources)
 
-        response['service_meta_'] = ServiceMeta(
+        response["service_meta_"] = ServiceMeta(
             version=__version__,
             response_datetime=datetime.now(),
         ).dict()
         return SearchService(**response)
 
     def _add_merged_meta(self, response: Dict) -> Dict:
         """Add source metadata to response object.
 
         :param Dict response: in-progress response object
         :return: completed response object.
         """
         sources_meta = {}
-        vod = response['disease_descriptor']
-        ids = [vod['disease']] + vod.get('xrefs', [])
+        vod = response["disease_descriptor"]
+        ids = [vod["disease"]] + vod.get("xrefs", [])
         for concept_id in ids:
-            prefix = concept_id.split(':')[0]
+            prefix = concept_id.split(":")[0]
             src_name = PREFIX_LOOKUP[prefix.lower()]
             if src_name not in sources_meta:
                 sources_meta[src_name] = self._fetch_meta(src_name)
-        response['source_meta_'] = sources_meta
+        response["source_meta_"] = sources_meta
         return response
 
-    def _add_vod(self, response: Dict, record: Dict, query: str,
-                 match_type: MatchType) -> NormalizationService:
+    def _add_vod(
+        self, response: Dict, record: Dict, query: str, match_type: MatchType
+    ) -> NormalizationService:
         """Format received DB record as VOD and update response object.
 
         :param Dict response: in-progress response object
         :param Dict record: record as stored in DB
         :param str query: query string from user request
         :param MatchType match_type: type of match achieved
         :return: completed normalized response object ready to return to user
         """
         vod = {
-            'id': f'normalize.disease:{quote(query)}',
-            'type': 'DiseaseDescriptor',
-            'disease': record['concept_id'],
-            'label': record['label'],
-            'extensions': [],
+            "id": f"normalize.disease:{quote(query)}",
+            "type": "DiseaseDescriptor",
+            "disease": record["concept_id"],
+            "label": record["label"],
+            "extensions": [],
         }
-        if 'xrefs' in record:
-            vod['xrefs'] = record['xrefs']
-        if 'aliases' in record:
-            vod['alternate_labels'] = record['aliases']
-        if 'pediatric_disease' in record and \
-                record['pediatric_disease'] is not None:
-            vod['extensions'].append({
-                'type': 'Extension',
-                'name': 'pediatric_disease',
-                'value': record['pediatric_disease']
-            })
-        if 'associated_with' in record and record['associated_with']:
-            vod['extensions'].append({
-                'type': 'Extension',
-                'name': 'associated_with',
-                'value': record['associated_with']
-            })
-        if not vod['extensions']:
-            del vod['extensions']
-        response['match_type'] = match_type
-        response['disease_descriptor'] = vod
+        if "xrefs" in record:
+            vod["xrefs"] = record["xrefs"]
+        if "aliases" in record:
+            vod["alternate_labels"] = record["aliases"]
+        if "pediatric_disease" in record and record["pediatric_disease"] is not None:
+            vod["extensions"].append(
+                {
+                    "type": "Extension",
+                    "name": "pediatric_disease",
+                    "value": record["pediatric_disease"],
+                }
+            )
+        if "associated_with" in record and record["associated_with"]:
+            vod["extensions"].append(
+                {
+                    "type": "Extension",
+                    "name": "associated_with",
+                    "value": record["associated_with"],
+                }
+            )
+        if not vod["extensions"]:
+            del vod["extensions"]
+        response["match_type"] = match_type
+        response["disease_descriptor"] = vod
         response = self._add_merged_meta(response)
         return NormalizationService(**response)
 
     def _record_order(self, record: Dict) -> (int, str):
         """Construct priority order for matching. Only called by sort().
 
         :param Dict record: individual record item in iterable to sort
         :return: tuple with rank value and concept ID
         """
-        src = record['src_name']
+        src = record["src_name"]
         if src == SourceName.NCIT.value:
             source_rank = 1
         elif src == SourceName.MONDO.value:
             source_rank = 2
         elif src == SourceName.ONCOTREE.value:
             source_rank = 3
         elif src == SourceName.OMIM.value:
             source_rank = 4
         elif src == SourceName.DO.value:
             source_rank = 5
         else:
-            logger.warning(f"query.record_order: Invalid source name for "
-                           f"{record}")
+            logger.warning(f"query.record_order: Invalid source name for " f"{record}")
             source_rank = 4
-        return source_rank, record['concept_id']
+        return source_rank, record["concept_id"]
 
-    def _handle_failed_merge_ref(self, record, response,
-                                 query) -> NormalizationService:
+    def _handle_failed_merge_ref(self, record, response, query) -> NormalizationService:
         """Log + fill out response for a failed merge reference lookup.
 
         :param Dict record: record containing failed merge_ref
         :param Dict response: in-progress response object
         :param str query: original query value
         :return: Normalized response with no match
         """
-        logger.error(f"Merge ref lookup failed for ref {record['merge_ref']} "
-                     f"in record {record['concept_id']} from query {query}")
-        response['match_type'] = MatchType.NO_MATCH
+        logger.error(
+            f"Merge ref lookup failed for ref {record['merge_ref']} "
+            f"in record {record['concept_id']} from query {query}"
+        )
+        response["match_type"] = MatchType.NO_MATCH
         return NormalizationService(**response)
 
     def normalize(self, query: str) -> NormalizationService:
         """Return normalized concept for given search term.
         :param str query: string to search against
         :return: NormalizationService object with complete response
         """
         # prepare basic response
         response = {
-            'query': query,
-            'warnings': self._emit_warnings(query),
-            'service_meta_': ServiceMeta(
+            "query": query,
+            "warnings": self._emit_warnings(query),
+            "service_meta_": ServiceMeta(
                 version=__version__,
                 response_datetime=datetime.now(),
-            )
+            ),
         }
-        if query == '':
-            response['match_type'] = MatchType.NO_MATCH
+        if query == "":
+            response["match_type"] = MatchType.NO_MATCH
             return NormalizationService(**response)
         query_str = query.lower().strip()
 
         # check merged concept ID match
-        record = self.db.get_record_by_id(query_str, case_sensitive=False,
-                                          merge=True)
+        record = self.db.get_record_by_id(query_str, case_sensitive=False, merge=True)
         if record:
             return self._add_vod(response, record, query, MatchType.CONCEPT_ID)
 
         non_merged_match = None
 
         # check concept ID match
         record = self.db.get_record_by_id(query_str, case_sensitive=False)
         if record:
-            if 'merge_ref' in record:
-                merge = self.db.get_record_by_id(record['merge_ref'],
-                                                 case_sensitive=False,
-                                                 merge=True)
+            if "merge_ref" in record:
+                merge = self.db.get_record_by_id(
+                    record["merge_ref"], case_sensitive=False, merge=True
+                )
                 if merge is None:
-                    return self._handle_failed_merge_ref(record, response,
-                                                         query_str)
+                    return self._handle_failed_merge_ref(record, response, query_str)
                 else:
-                    return self._add_vod(response, merge, query,
-                                         MatchType.CONCEPT_ID)
+                    return self._add_vod(response, merge, query, MatchType.CONCEPT_ID)
             else:
-                non_merged_match = (record, 'concept_id')
+                non_merged_match = (record, "concept_id")
 
         # check other match types
-        for match_type in ['label', 'alias', 'xref', 'associated_with']:
+        for match_type in ["label", "alias", "xref", "associated_with"]:
             # get matches list for match tier
             query_matches = self.db.get_records_by_type(query_str, match_type)
-            query_matches = [self.db.get_record_by_id(m['concept_id'],
-                                                      case_sensitive=False)
-                             for m in query_matches]
+            query_matches = [
+                self.db.get_record_by_id(m["concept_id"], case_sensitive=False)
+                for m in query_matches
+            ]
             query_matches.sort(key=self._record_order)
 
             # attempt merge ref resolution until successful
             for match in query_matches:
-                record = self.db.get_record_by_id(match['concept_id'], False)
+                record = self.db.get_record_by_id(match["concept_id"], False)
                 if record:
-                    if 'merge_ref' in record:
-                        merge = self.db.get_record_by_id(record['merge_ref'],
-                                                         case_sensitive=False,
-                                                         merge=True)
+                    if "merge_ref" in record:
+                        merge = self.db.get_record_by_id(
+                            record["merge_ref"], case_sensitive=False, merge=True
+                        )
                         if merge is None:
-                            return self._handle_failed_merge_ref(record,
-                                                                 response,
-                                                                 query_str)
+                            return self._handle_failed_merge_ref(
+                                record, response, query_str
+                            )
                         else:
-                            return self._add_vod(response, merge, query,
-                                                 MatchType[match_type.upper()])
+                            return self._add_vod(
+                                response, merge, query, MatchType[match_type.upper()]
+                            )
                     else:
                         if not non_merged_match:
                             non_merged_match = (record, match_type)
 
         # if no successful match, try available non-merged match
         if non_merged_match:
             match_type = MatchType[non_merged_match[1].upper()]
-            return self._add_vod(response, non_merged_match[0], query,
-                                 match_type)
+            return self._add_vod(response, non_merged_match[0], query, match_type)
 
         if not query_matches:
-            response['match_type'] = MatchType.NO_MATCH
+            response["match_type"] = MatchType.NO_MATCH
         return NormalizationService(**response)
```

### Comparing `disease-normalizer-0.3.0/disease/schemas.py` & `disease-normalizer-0.3.1/disease/schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """This module contains data models for representing VICC normalized
 disease records.
 """
-from typing import Any, Dict, Type, List, Optional, Union
-from enum import Enum, IntEnum
-from pydantic import BaseModel, StrictBool
 from datetime import datetime
+from enum import Enum, IntEnum
+from typing import Any, Dict, List, Optional, Type, Union
+
 from ga4gh.vrsatile.pydantic.vrsatile_models import DiseaseDescriptor
+from pydantic import BaseModel, StrictBool
 
 
 class MatchType(IntEnum):
     """Define string constraints for use in Match Type attributes."""
 
     CONCEPT_ID = 100
     LABEL = 80
@@ -49,35 +50,40 @@
     NCIT = "ncit"
     MONDO = "mondo"
     DO = "DOID"
     OMIM = "omim"
     ONCOTREE = "oncotree"
     # external sources
     COHD = "cohd"
+    DECIPHER = "decipher"
     EFO = "efo"
     GARD = "gard"
     HPO = "HP"
     ICD9 = "icd9"
     ICD9CM = "icd9.cm"
     ICD10 = "icd10"
     ICD10CM = "icd10.cm"
+    ICD11 = "icd11"
     ICDO = "icdo"
     IDO = "ido"
     IMDRF = "imdrf"
     KEGG = "kegg.disease"
     MEDDRA = "meddra"
     MEDGEN = "medgen"
     MESH = "mesh"
     MF = "mf"
     MP = "MP"
+    MPATH = "mpath"
     NIFSTD = "nifstd"
+    OBI = "obi"
     OGMS = "ogms"
     OMIMPS = "omimps"
     ORPHANET = "orphanet"
     PATO = "pato"
+    SCDO = "scdo"
     UMLS = "umls"
     WIKIPEDIA = "wikipedia.en"
     WIKIDATA = "wikidata"
 
 
 class SourcePriority(IntEnum):
     """Define priorities for sources in building merged concepts."""
@@ -99,30 +105,29 @@
     associated_with: Optional[List[str]] = []
     pediatric_disease: Optional[bool]
 
     class Config:
         """Configure model."""
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any],
-                         model: Type['Disease']) -> None:
+        def schema_extra(schema: Dict[str, Any], model: Type["Disease"]) -> None:
             """Configure OpenAPI schema."""
-            if 'title' in schema.keys():
-                schema.pop('title', None)
-            for prop in schema.get('properties', {}).values():
-                prop.pop('title', None)
-            schema['example'] = {
+            if "title" in schema.keys():
+                schema.pop("title", None)
+            for prop in schema.get("properties", {}).values():
+                prop.pop("title", None)
+            schema["example"] = {
                 "label": "Von Hippel-Lindau Syndrome",
                 "concept_id": "ncit:C3105",
                 "aliases": [
                     "Von Hippel-Lindau Syndrome (VHL)",
                     "Von Hippel-Lindau Disease",
                     "Cerebroretinal Angiomatosis",
                     "von Hippel-Lindau syndrome",
-                    "VHL syndrome"
+                    "VHL syndrome",
                 ],
                 "xrefs": [],
                 "associated_with": ["umls:C0019562"],
                 "pediatric_disease": None,
             }
 
 
@@ -134,18 +139,18 @@
     attribution: StrictBool
 
 
 class ItemTypes(str, Enum):
     """Item types used in DynamoDB."""
 
     # Must be in descending MatchType order.
-    LABEL = 'label'
-    ALIASES = 'alias'
-    XREFS = 'xref'
-    ASSOCIATED_WITH = 'associated_with'
+    LABEL = "label"
+    ALIASES = "alias"
+    XREFS = "xref"
+    ASSOCIATED_WITH = "associated_with"
 
 
 class SourceMeta(BaseModel):
     """Metadata for a given source to return in response object."""
 
     data_license: str
     data_license_url: str
@@ -154,32 +159,31 @@
     rdp_url: Optional[str]
     data_license_attributes: Dict[str, StrictBool]
 
     class Config:
         """Enables orm_mode"""
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any],
-                         model: Type['SourceMeta']) -> None:
+        def schema_extra(schema: Dict[str, Any], model: Type["SourceMeta"]) -> None:
             """Configure OpenAPI schema"""
-            if 'title' in schema.keys():
-                schema.pop('title', None)
-            for prop in schema.get('properties', {}).values():
-                prop.pop('title', None)
-            schema['example'] = {
+            if "title" in schema.keys():
+                schema.pop("title", None)
+            for prop in schema.get("properties", {}).values():
+                prop.pop("title", None)
+            schema["example"] = {
                 "data_license": "CC BY 4.0",
                 "data_license_url": "https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa: E501
                 "version": "21.01d",
                 "data_url": "https://evs.nci.nih.gov/ftp1/NCI_Thesaurus/archive/21.01d_Release/",  # noqa: E501
                 "rdp_url": "http://reusabledata.org/ncit.html",
                 "data_license_attributes": {
                     "non_commercial": False,
                     "attribution": True,
-                    "share_alike": False
-                }
+                    "share_alike": False,
+                },
             }
 
 
 class MatchesKeyed(BaseModel):
     """Container for matching information from an individual source.
     Used when matches are requested as an object, not an array.
     """
@@ -188,49 +192,50 @@
     records: List[Disease]
     source_meta_: SourceMeta
 
     class Config:
         """Enables orm_mode"""
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any],
-                         model: Type['MatchesKeyed']) -> None:
+        def schema_extra(schema: Dict[str, Any], model: Type["MatchesKeyed"]) -> None:
             """Configure OpenAPI schema"""
-            if 'title' in schema.keys():
-                schema.pop('title', None)
-            for prop in schema.get('properties', {}).values():
-                prop.pop('title', None)
-            schema['example'] = {
+            if "title" in schema.keys():
+                schema.pop("title", None)
+            for prop in schema.get("properties", {}).values():
+                prop.pop("title", None)
+            schema["example"] = {
                 "match_type": 80,
-                "records": [{
-                    "label": "Von Hippel-Lindau Syndrome",
-                    "concept_id": "ncit:C3105",
-                    "aliases": [
-                        "Von Hippel-Lindau Syndrome (VHL)",
-                        "Von Hippel-Lindau Disease",
-                        "Cerebroretinal Angiomatosis",
-                        "von Hippel-Lindau syndrome",
-                        "VHL syndrome"
-                    ],
-                    "xrefs": [],
-                    "associated_with": ["umls:C0019562"],
-                    "pediatric_disease": None,
-                }],
+                "records": [
+                    {
+                        "label": "Von Hippel-Lindau Syndrome",
+                        "concept_id": "ncit:C3105",
+                        "aliases": [
+                            "Von Hippel-Lindau Syndrome (VHL)",
+                            "Von Hippel-Lindau Disease",
+                            "Cerebroretinal Angiomatosis",
+                            "von Hippel-Lindau syndrome",
+                            "VHL syndrome",
+                        ],
+                        "xrefs": [],
+                        "associated_with": ["umls:C0019562"],
+                        "pediatric_disease": None,
+                    }
+                ],
                 "source_meta_": {
                     "data_license": "CC BY 4.0",
                     "data_license_url": "https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa: E501
                     "version": "21.01d",
                     "data_url": "https://evs.nci.nih.gov/ftp1/NCI_Thesaurus/archive/21.01d_Release/",  # noqa: E501
                     "rdp_url": "http://reusabledata.org/ncit.html",
                     "data_license_attributes": {
                         "non_commercial": False,
                         "attribution": True,
-                        "share_alike": False
-                    }
-                }
+                        "share_alike": False,
+                    },
+                },
             }
 
 
 class MatchesListed(BaseModel):
     """Container for matching information from an individual source.
     Used when matches are requested as an array, not an object.
     """
@@ -240,77 +245,77 @@
     records: List[Disease]
     source_meta_: SourceMeta
 
     class Config:
         """Enables orm_mode"""
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any],
-                         model: Type['MatchesListed']) -> None:
+        def schema_extra(schema: Dict[str, Any], model: Type["MatchesListed"]) -> None:
             """Configure OpenAPI schema"""
-            if 'title' in schema.keys():
-                schema.pop('title', None)
-            for prop in schema.get('properties', {}).values():
-                prop.pop('title', None)
-            schema['example'] = {
+            if "title" in schema.keys():
+                schema.pop("title", None)
+            for prop in schema.get("properties", {}).values():
+                prop.pop("title", None)
+            schema["example"] = {
                 "source": "NCIt",
                 "match_type": 80,
-                "records": [{
-                    "label": "Von Hippel-Lindau Syndrome",
-                    "concept_id": "ncit:C3105",
-                    "aliases": [
-                        "Von Hippel-Lindau Syndrome (VHL)",
-                        "Von Hippel-Lindau Disease",
-                        "Cerebroretinal Angiomatosis",
-                        "von Hippel-Lindau syndrome",
-                        "VHL syndrome"
-                    ],
-                    "xrefs": [],
-                    "associated_with": ["umls:C0019562"],
-                    "pediatric_disease": None
-                }],
+                "records": [
+                    {
+                        "label": "Von Hippel-Lindau Syndrome",
+                        "concept_id": "ncit:C3105",
+                        "aliases": [
+                            "Von Hippel-Lindau Syndrome (VHL)",
+                            "Von Hippel-Lindau Disease",
+                            "Cerebroretinal Angiomatosis",
+                            "von Hippel-Lindau syndrome",
+                            "VHL syndrome",
+                        ],
+                        "xrefs": [],
+                        "associated_with": ["umls:C0019562"],
+                        "pediatric_disease": None,
+                    }
+                ],
                 "source_meta_": {
                     "data_license": "CC BY 4.0",
                     "data_license_url": "https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa: E501
                     "version": "21.01d",
                     "data_url": "https://evs.nci.nih.gov/ftp1/NCI_Thesaurus/archive/21.01d_Release/",  # noqa: E501
                     "rdp_url": "http://reusabledata.org/ncit.html",
                     "data_license_attributes": {
                         "non_commercial": False,
                         "attribution": True,
-                        "share_alike": False
-                    }
-                }
+                        "share_alike": False,
+                    },
+                },
             }
 
 
 class ServiceMeta(BaseModel):
     """Metadata regarding the disease-normalization service."""
 
-    name = 'disease-normalizer'
+    name = "disease-normalizer"
     version: str
     response_datetime: datetime
-    url = 'https://github.com/cancervariants/disease-normalization'
+    url = "https://github.com/cancervariants/disease-normalization"
 
     class Config:
         """Enables orm_mode"""
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any],
-                         model: Type['ServiceMeta']) -> None:
+        def schema_extra(schema: Dict[str, Any], model: Type["ServiceMeta"]) -> None:
             """Configure OpenAPI schema"""
-            if 'title' in schema.keys():
-                schema.pop('title', None)
-            for prop in schema.get('properties', {}).values():
-                prop.pop('title', None)
-            schema['example'] = {
-                'name': 'disease-normalizer',
-                'version': '0.1.0',
-                'response_datetime': '2021-04-05T16:44:15.367831',
-                'url': 'https://github.com/cancervariants/disease-normalization'  # noqa: E501
+            if "title" in schema.keys():
+                schema.pop("title", None)
+            for prop in schema.get("properties", {}).values():
+                prop.pop("title", None)
+            schema["example"] = {
+                "name": "disease-normalizer",
+                "version": "0.1.0",
+                "response_datetime": "2021-04-05T16:44:15.367831",
+                "url": "https://github.com/cancervariants/disease-normalization",
             }
 
 
 class NormalizationService(BaseModel):
     """Response containing one or more merged records and source data."""
 
     query: str
@@ -320,98 +325,96 @@
     source_meta_: Optional[Dict[SourceName, SourceMeta]]
     service_meta_: ServiceMeta
 
     class Config:
         """Configure model."""
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any],
-                         model: Type['NormalizationService']) -> None:
+        def schema_extra(
+            schema: Dict[str, Any], model: Type["NormalizationService"]
+        ) -> None:
             """Configure OpenAPI schema"""
-            if 'title' in schema.keys():
-                schema.pop('title', None)
-            for prop in schema.get('properties', {}).values():
-                prop.pop('title', None)
-            schema['example'] = {
+            if "title" in schema.keys():
+                schema.pop("title", None)
+            for prop in schema.get("properties", {}).values():
+                prop.pop("title", None)
+            schema["example"] = {
                 "query": "childhood leukemia",
                 "warnings": None,
                 "match_type": 80,
                 "disease_descriptor": {
                     "id": "normalize:childhood%20leukemia",
                     "type": "DiseaseDescriptor",
                     "disease": "ncit:C4989",
                     "label": "Childhood Leukemia",
-                    "xrefs": [
-                        "mondo:0004355",
-                        "DOID:7757"
-                    ],
+                    "xrefs": ["mondo:0004355", "DOID:7757"],
                     "alternate_labels": [
                         "childhood leukemia (disease)",
                         "leukemia",
                         "pediatric leukemia (disease)",
                         "Leukemia",
-                        "leukemia (disease) of childhood"
+                        "leukemia (disease) of childhood",
                     ],
                     "extensions": [
                         {
                             "type": "Extension",
                             "name": "pediatric_disease",
-                            "value": True
+                            "value": True,
                         },
                         {
                             "type": "Extension",
                             "name": "associated_with",
-                            "value": ["umls:C1332977"]
-                        }
-                    ]
+                            "value": ["umls:C1332977"],
+                        },
+                    ],
                 },
                 "source_meta_": {
                     "NCIt": {
                         "data_license": "CC BY 4.0",
                         "data_license_url": "https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa: E501
                         "version": "21.01d",
                         "data_url": "https://evs.nci.nih.gov/ftp1/NCI_Thesaurus/archive/21.01d_Release/",  # noqa: E501
                         "rdp_url": "http://reusabledata.org/ncit.html",
                         "data_license_attributes": {
                             "non_commercial": False,
                             "attribution": True,
-                            "share_alike": False
-                        }
+                            "share_alike": False,
+                        },
                     },
                     "Mondo": {
                         "data_license": "CC BY 4.0",
                         "data_license_url": "https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa: E501
                         "version": "20210129",
                         "data_url": "https://mondo.monarchinitiative.org/pages/download/",  # noqa: E501
                         "rdp_url": "http://reusabledata.org/monarch.html",
                         "data_license_attributes": {
                             "non_commercial": False,
                             "attribution": True,
-                            "share_alike": False
-                        }
+                            "share_alike": False,
+                        },
                     },
                     "DO": {
                         "data_license": "CC0 1.0",
                         "data_license_url": "https://creativecommons.org/publicdomain/zero/1.0/legalcode",  # noqa: E501
                         "version": "20210305",
-                        "data_url": "http://www.obofoundry.org/ontology/doid.html",  # noqa: E501
+                        "data_url": "http://www.obofoundry.org/ontology/doid.html",
                         "rdp_url": None,
                         "data_license_attributes": {
                             "non_commercial": False,
                             "attribution": False,
-                            "share_alike": False
-                        }
-                    }
+                            "share_alike": False,
+                        },
+                    },
                 },
                 "service_meta_": {
-                    'name': 'disease-normalizer',
-                    'version': '0.1.0',
-                    'response_datetime': '2021-04-05T16:44:15.367831',
-                    'url': 'https://github.com/cancervariants/disease-normalization'  # noqa: E501
-                }
+                    "name": "disease-normalizer",
+                    "version": "0.1.0",
+                    "response_datetime": "2021-04-05T16:44:15.367831",
+                    "url": "https://github.com/cancervariants/disease-normalization",
+                },
             }
 
 
 class SearchService(BaseModel):
     """Core response schema containing matches for each source"""
 
     query: str
@@ -419,54 +422,57 @@
     source_matches: Union[Dict[SourceName, MatchesKeyed], List[MatchesListed]]
     service_meta_: ServiceMeta
 
     class Config:
         """Enables orm_mode"""
 
         @staticmethod
-        def schema_extra(schema: Dict[str, Any],
-                         model: Type['SearchService']) -> None:
+        def schema_extra(schema: Dict[str, Any], model: Type["SearchService"]) -> None:
             """Configure OpenAPI schema"""
-            if 'title' in schema.keys():
-                schema.pop('title', None)
-            for prop in schema.get('properties', {}).values():
-                prop.pop('title', None)
-            schema['example'] = {
+            if "title" in schema.keys():
+                schema.pop("title", None)
+            for prop in schema.get("properties", {}).values():
+                prop.pop("title", None)
+            schema["example"] = {
                 "query": "Von Hippel-Lindau Syndrome",
                 "warnings": None,
-                "source_matches": [{
-                    "source": "NCIt",
-                    "match_type": 80,
-                    "records": [{
-                        "label": "Von Hippel-Lindau Syndrome",
-                        "concept_id": "ncit:C3105",
-                        "aliases": [
-                            "Von Hippel-Lindau Syndrome (VHL)",
-                            "Von Hippel-Lindau Disease",
-                            "Cerebroretinal Angiomatosis",
-                            "von Hippel-Lindau syndrome",
-                            "VHL syndrome"
+                "source_matches": [
+                    {
+                        "source": "NCIt",
+                        "match_type": 80,
+                        "records": [
+                            {
+                                "label": "Von Hippel-Lindau Syndrome",
+                                "concept_id": "ncit:C3105",
+                                "aliases": [
+                                    "Von Hippel-Lindau Syndrome (VHL)",
+                                    "Von Hippel-Lindau Disease",
+                                    "Cerebroretinal Angiomatosis",
+                                    "von Hippel-Lindau syndrome",
+                                    "VHL syndrome",
+                                ],
+                                "xrefs": [],
+                                "associated_with": ["umls:C0019562"],
+                                "pediatric_disease": None,
+                            }
                         ],
-                        "xrefs": [],
-                        "associated_with": ["umls:C0019562"],
-                        "pediatric_disease": None,
-                    }],
-                    "source_meta_": {
-                        "data_license": "CC BY 4.0",
-                        "data_license_url": "https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa: E501
-                        "version": "21.01d",
-                        "data_url": "https://evs.nci.nih.gov/ftp1/NCI_Thesaurus/archive/21.01d_Release/",  # noqa: E501
-                        "rdp_url": "http://reusabledata.org/ncit.html",
-                        "data_license_attributes": {
-                            "non_commercial": False,
-                            "attribution": True,
-                            "share_alike": False
-                        }
+                        "source_meta_": {
+                            "data_license": "CC BY 4.0",
+                            "data_license_url": "https://creativecommons.org/licenses/by/4.0/legalcode",  # noqa: E501
+                            "version": "21.01d",
+                            "data_url": "https://evs.nci.nih.gov/ftp1/NCI_Thesaurus/archive/21.01d_Release/",  # noqa: E501
+                            "rdp_url": "http://reusabledata.org/ncit.html",
+                            "data_license_attributes": {
+                                "non_commercial": False,
+                                "attribution": True,
+                                "share_alike": False,
+                            },
+                        },
                     }
-                }],
+                ],
                 "service_meta_": {
-                    'name': 'disease-normalizer',
-                    'version': '0.1.0',
-                    'response_datetime': '2021-04-05T16:44:15.367831',
-                    'url': 'https://github.com/cancervariants/disease-normalization'  # noqa: E501
-                }
+                    "name": "disease-normalizer",
+                    "version": "0.1.0",
+                    "response_datetime": "2021-04-05T16:44:15.367831",
+                    "url": "https://github.com/cancervariants/disease-normalization",  # noqa: E501
+                },
             }
```

### Comparing `disease-normalizer-0.3.0/disease_normalizer.egg-info/PKG-INFO` & `disease-normalizer-0.3.1/disease_normalizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disease-normalizer
-Version: 0.3.0
+Version: 0.3.1
 Summary: VICC normalization routine for diseases
 Home-page: https://github.com/cancervariants/disease-normalization
 Author: VICC
 Author-email: help@cancervariants.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `disease-normalizer-0.3.0/disease_normalizer.egg-info/SOURCES.txt` & `disease-normalizer-0.3.1/disease_normalizer.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 disease/__init__.py
 disease/cli.py
 disease/database.py
 disease/main.py
 disease/query.py
```

### Comparing `disease-normalizer-0.3.0/setup.cfg` & `disease-normalizer-0.3.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -30,18 +30,21 @@
 	click
 
 [options.extras_require]
 dev = 
 	owlready2
 	rdflib
 	requests
+	typing-extensions
 	bioversions
 	pre-commit
 	flake8
 	flake8-docstrings
+	black
+	isort
 test = 
 	pytest
 	pytest-cov
 	coveralls
 	coverage
 
 [tool:pytest]
```

