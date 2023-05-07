# Comparing `tmp/elasticsearch-faker-0.2.0.tar.gz` & `tmp/elasticsearch-faker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elasticsearch-faker-0.2.0.tar", last modified: Sat Mar  5 16:27:44 2022, max compression
+gzip compressed data, was "elasticsearch-faker-0.3.0.tar", last modified: Sun May  7 14:27:59 2023, max compression
```

## Comparing `elasticsearch-faker-0.2.0.tar` & `elasticsearch-faker-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-05 16:27:44.175294 elasticsearch-faker-0.2.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      203 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     5920 2022-03-05 16:27:44.175294 elasticsearch-faker-0.2.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     4639 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-05 16:27:44.175294 elasticsearch-faker-0.2.0/elasticsearch_faker/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10567 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/__main__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      503 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5297 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/_es_client.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2139 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/_generator.py
--rw-r--r--   0 toor      (1000) toor      (1000)      913 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)      445 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/_print.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2744 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/_provider.py
--rw-r--r--   0 toor      (1000) toor      (1000)      640 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/_template.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-05 16:27:44.175294 elasticsearch-faker-0.2.0/elasticsearch_faker/subcmd/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/subcmd/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1822 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/elasticsearch_faker/subcmd/provider.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-05 16:27:44.175294 elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     5920 2022-03-05 16:27:43.000000 elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      997 2022-03-05 16:27:44.000000 elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-03-05 16:27:43.000000 elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       73 2022-03-05 16:27:43.000000 elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-03-05 16:27:08.000000 elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      305 2022-03-05 16:27:43.000000 elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       20 2022-03-05 16:27:44.000000 elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1177 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-05 16:27:44.175294 elasticsearch-faker-0.2.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)      142 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       53 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2022-03-05 16:27:44.175294 elasticsearch-faker-0.2.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2690 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-05 16:27:44.175294 elasticsearch-faker-0.2.0/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      213 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/tests/common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2469 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/tests/test_generator.py
--rw-r--r--   0 toor      (1000) toor      (1000)      501 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/tests/test_help.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1524 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/tests/test_subcmd_generate.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1205 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/tests/test_subcmd_validate.py
--rw-r--r--   0 toor      (1000) toor      (1000)      447 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/tests/test_subcmd_version.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1032 2022-03-05 16:27:07.000000 elasticsearch-faker-0.2.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-07 14:27:59.282227 elasticsearch-faker-0.3.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      203 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    11642 2023-05-07 14:27:59.282227 elasticsearch-faker-0.3.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    10400 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-07 14:27:59.282227 elasticsearch-faker-0.3.0/elasticsearch_faker/
+-rw-r--r--   0 toor      (1000) toor      (1000)       88 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14802 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/__main__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      804 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6496 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/_es_client.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2139 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/_generator.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      921 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      445 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/_print.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2744 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/_provider.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      640 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/_template.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-07 14:27:59.282227 elasticsearch-faker-0.3.0/elasticsearch_faker/subcmd/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/subcmd/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2120 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/elasticsearch_faker/subcmd/provider.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-07 14:27:59.282227 elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    11642 2023-05-07 14:27:59.000000 elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      997 2023-05-07 14:27:59.000000 elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-07 14:27:59.000000 elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       73 2023-05-07 14:27:59.000000 elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/entry_points.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-07 14:27:45.000000 elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      290 2023-05-07 14:27:59.000000 elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       20 2023-05-07 14:27:59.000000 elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1178 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-07 14:27:59.282227 elasticsearch-faker-0.3.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)      142 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       66 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-05-07 14:27:59.282227 elasticsearch-faker-0.3.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2662 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-07 14:27:59.282227 elasticsearch-faker-0.3.0/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      213 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/tests/common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2354 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/tests/test_generator.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      501 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/tests/test_help.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1420 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/tests/test_subcmd_generate.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1205 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/tests/test_subcmd_validate.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      447 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/tests/test_subcmd_version.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      992 2023-05-07 14:27:34.000000 elasticsearch-faker-0.3.0/tox.ini
```

### Comparing `elasticsearch-faker-0.2.0/LICENSE` & `elasticsearch-faker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch-faker-0.2.0/elasticsearch_faker/_es_client.py` & `elasticsearch-faker-0.3.0/elasticsearch_faker/_es_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,63 @@
 import abc
 import errno
 import json
 import os
 import sys
-from typing import Dict, List
+from dataclasses import dataclass
+from typing import Dict, List, Optional, Tuple
 
 from elasticsearch import Elasticsearch
-from elasticsearch.exceptions import NotFoundError, RequestError, TransportError
+from elasticsearch.exceptions import (
+    AuthenticationException,
+    BadRequestError,
+    ConnectionError,
+    NotFoundError,
+    RequestError,
+    TransportError,
+)
 
 from ._const import Default
 from ._logger import logger
 
 
 class ElasticsearchClientInterface(metaclass=abc.ABCMeta):
-    @abc.abstractclassmethod
-    def create_index(self, index_name: str, mapping_filepath: str) -> None:
-        pass
+    @abc.abstractmethod
+    def create_index(self, index_name: str, mapping_filepath: str) -> int:
+        return 0
 
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     def delete_index(self, index_name: str) -> None:
         pass
 
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     def put(self, index_name: str, doc: Dict) -> int:
         pass
 
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     def bulk_put(self, index_name: str, docs: List[Dict]) -> int:
         pass
 
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     def refresh(self, index_name: str) -> None:
         pass
 
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     def count_docs(self, index_name: str) -> int:
         pass
 
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     def fetch_stats(self, index_name: str) -> Dict:
         pass
 
 
 class NullElasticsearchClient(ElasticsearchClientInterface):
-    def create_index(self, index_name: str, mapping_filepath: str) -> None:
+    def create_index(self, index_name: str, mapping_filepath: str) -> int:
         logger.debug(f"create index: {index_name}")
+        return 0
 
     def delete_index(self, index_name: str) -> None:
         logger.debug(f"delete index: {index_name}")
 
     def put(self, index_name: str, doc: Dict) -> int:
         logger.debug(f"put a doc to {index_name}")
         print(json.dumps(doc, indent=4))
@@ -70,36 +79,43 @@
         return {"primaries": {"store": {"size_in_bytes": 0}}}
 
 
 class ElasticsearchClient(ElasticsearchClientInterface):
     def __init__(self, es: Elasticsearch) -> None:
         self.__es = es
 
-    def create_index(self, index_name: str, mapping_filepath: str) -> None:
+    def create_index(self, index_name: str, mapping_filepath: str) -> int:
         logger.debug(f"create index: {index_name}")
 
         mappings = {}
         if mapping_filepath:
             if not os.path.exists(mapping_filepath):
                 logger.error(f"mapping file not found: {mapping_filepath}")
-                sys.exit(errno.ENOENT)
+                return errno.ENOENT
 
             with open(mapping_filepath) as f:
                 mappings = json.load(f)
 
         try:
             result = self.__es.indices.create(index=index_name, body=mappings)
             logger.debug(result)
-        except TransportError as e:
+        except AuthenticationException as e:
+            logger.error(e)
+            return errno.EACCES
+        except ConnectionError as e:
+            logger.error(e)
+            return errno.ECOMM
+        except BadRequestError as e:
             if e.error == "resource_already_exists_exception":
-                # ignore already existing index
-                logger.debug(e)
+                logger.debug(f"skip existing index creation: {e}")
             else:
                 raise
 
+        return 0
+
     def delete_index(self, index_name: str) -> None:
         logger.debug(f"delete index: {index_name}")
         self.__es.indices.delete(index=index_name, ignore=404, request_timeout=Default.TIMEOUT)
 
     def put(self, index_name: str, doc: Dict) -> int:
         logger.debug(doc)
 
@@ -144,30 +160,58 @@
         self.__es.indices.flush(index=index_name, request_timeout=Default.TIMEOUT)
 
     def refresh(self, index_name: str) -> None:
         logger.debug(f"refresh {index_name}")
         self.__es.indices.refresh(index=index_name, request_timeout=Default.TIMEOUT)
 
     def count_docs(self, index_name: str) -> int:
-        return int(self.__es.cat.count(index=index_name, params={"h": "count"}))
+        resp = self.__es.cat.count(index=index_name, params={"h": "count"})
+        return int(str(resp))
 
     def fetch_stats(self, index_name: str) -> Dict:
         try:
             stats = self.__es.indices.stats(index=index_name, metric="_all")
+        except AuthenticationException as e:
+            logger.error(e)
+            sys.exit(errno.EPERM)
         except NotFoundError as e:
             logger.error(e)
             sys.exit(errno.ENOENT)
 
         return stats["indices"][index_name]
 
 
-def create_es_client(endpoint: str, dry_run: bool) -> ElasticsearchClientInterface:
+@dataclass
+class ElasticsearchClientParameter:
+    endpoint: str
+    verify_certs: bool = False
+    basic_auth_user: Optional[str] = None
+    basic_auth_password: Optional[str] = None
+    ssl_assert_fingerprint: Optional[str] = None
+
+    @property
+    def basic_auth(self) -> Optional[Tuple[str, str]]:
+        if self.basic_auth_user is None or self.basic_auth_password is None:
+            return None
+
+        return (self.basic_auth_user, self.basic_auth_password)
+
+
+def create_es_client(
+    es_client_param: ElasticsearchClientParameter, dry_run: bool
+) -> ElasticsearchClientInterface:
     if dry_run:
         return NullElasticsearchClient()
 
     try:
-        es = Elasticsearch(hosts=[endpoint], sniff_on_start=False)
+        es = Elasticsearch(
+            hosts=[es_client_param.endpoint],
+            sniff_on_start=False,
+            verify_certs=es_client_param.verify_certs,
+            basic_auth=es_client_param.basic_auth,
+            ssl_assert_fingerprint=es_client_param.ssl_assert_fingerprint,
+        )
     except TransportError as e:
         logger.error(e)
         sys.exit(errno.ENETUNREACH)
 
     return ElasticsearchClient(es)
```

### Comparing `elasticsearch-faker-0.2.0/elasticsearch_faker/_generator.py` & `elasticsearch-faker-0.3.0/elasticsearch_faker/_generator.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-faker-0.2.0/elasticsearch_faker/_logger.py` & `elasticsearch-faker-0.3.0/elasticsearch_faker/_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class LogLevel:
     DEBUG = "DEBUG"
     INFO = "INFO"
     QUIET = "QUIET"
 
 
-def set_logger(is_enable: bool, propagation_depth: int = 1):
+def set_logger(is_enable: bool, propagation_depth: int = 1) -> None:
     if is_enable:
         logger.enable(MODULE_NAME)
     else:
         logger.disable(MODULE_NAME)
 
 
 def initialize_logger(name: str, log_level: str) -> None:
```

### Comparing `elasticsearch-faker-0.2.0/elasticsearch_faker/_provider.py` & `elasticsearch-faker-0.3.0/elasticsearch_faker/_provider.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-faker-0.2.0/elasticsearch_faker/_template.py` & `elasticsearch-faker-0.3.0/elasticsearch_faker/_template.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-faker-0.2.0/elasticsearch_faker/subcmd/provider.py` & `elasticsearch-faker-0.3.0/elasticsearch_faker/subcmd/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 from faker.exceptions import UnsupportedFeature
 
 from .._const import COMMAND_EPILOG, Context
 from .._logger import logger
 from .._provider import get_providers
 
 
+DEFAULT_MAX_DISPLAY_LEN = 64
+
+
 @click.group(epilog=COMMAND_EPILOG)
 def provider():
     """
-    Show or search providers for template.
+    Show or search providers for doc templates.
     """
 
 
 @provider.command()
 @click.pass_context
 def list(ctx):
     """
@@ -46,33 +49,40 @@
             continue
 
         click.echo(provider)
 
 
 @provider.command()
 @click.argument("providers", type=str, nargs=-1)
+@click.option(
+    "--max-len",
+    metavar="LENGTH",
+    type=int,
+    default=DEFAULT_MAX_DISPLAY_LEN,
+    help=f"Maximum display length per example. Defaults to {DEFAULT_MAX_DISPLAY_LEN}.",
+)
 @click.pass_context
-def example(ctx, providers: List[str]):
+def example(ctx, providers: List[str], max_len: int):
     """
     List available providers with examples.
     """
 
     locale = ctx.obj[Context.LOCALE]
     seed = ctx.obj[Context.SEED]
-    limit = 64
 
     fake = Factory.create(locale)
     if seed is not None:
         Faker.seed(seed)
 
     for provider in sorted(get_providers(locale)):
         try:
             value = getattr(fake, provider)()
         except AttributeError:
             # implemented providers may differ locale to locale
             logger.debug(f"provider not found: locale={locale}, provider={provider}")
             continue
-        except UnsupportedFeature as e:
+        except (TypeError, UnsupportedFeature) as e:
             logger.warning(f"provider={provider}: {e}")
             continue
 
-        click.echo(f"{provider}: {str(value)[:limit]}")
+        str_value = str(value)
+        click.echo(f"{provider} (len={len(str_value)}): {str_value[:max_len]}")
```

### Comparing `elasticsearch-faker-0.2.0/elasticsearch_faker.egg-info/SOURCES.txt` & `elasticsearch-faker-0.3.0/elasticsearch_faker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elasticsearch-faker-0.2.0/pyproject.toml` & `elasticsearch-faker-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.coverage.run]
 source = ['elasticsearch-faker']
 branch = true
 
 [tool.coverage.report]
 show_missing = true
@@ -50,15 +50,15 @@
     '*/.eggs/*',
     '*/.pytype/*',
     '*/.tox/*',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.7
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
```

### Comparing `elasticsearch-faker-0.2.0/setup.py` & `elasticsearch-faker-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "elasticsearch-faker"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -29,15 +29,15 @@
 
 with open(os.path.join(REQUIREMENT_DIR, "requirements.txt")) as f:
     INSTALL_REQUIRES = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
 
-build_exe_requires = ["pyinstaller>=4.9", "text-unidecode"]
+build_exe_requires = ["pyinstaller>=5.10.1", "text-unidecode"]
 
 setuptools.setup(
     name=MODULE_NAME,
     version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
@@ -48,34 +48,33 @@
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["tests*"]),
     project_urls={
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=INSTALL_REQUIRES,
     extras_require={
         "buildexe": build_exe_requires,
-        "es7": ["elasticsearch>=7.0.5,<8"],
         "es8": ["elasticsearch>=8,<9"],
         "test": TESTS_REQUIRES,
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Terminals",
     ],
     cmdclass=get_release_command_class(),
     zip_safe=False,
     entry_points={
         "console_scripts": [
```

### Comparing `elasticsearch-faker-0.2.0/tests/test_generator.py` & `elasticsearch-faker-0.3.0/tests/test_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import json
-import sys
 from textwrap import dedent
 
-import pytest
 from faker import Factory, Faker
 
 from elasticsearch_faker._generator import FakeDocGenerator
 from elasticsearch_faker._provider import re_provider
 
 
 class TestFakeDocGenerator:
-    @pytest.mark.skipif(sys.version_info < (3, 6), reason="requires python3.6 or higher")
     def test_normal_generate_docs(self):
         fake = Factory.create()
         Faker.seed(0)
 
         template_text = dedent(
             """\
             {
```

### Comparing `elasticsearch-faker-0.2.0/tests/test_subcmd_generate.py` & `elasticsearch-faker-0.3.0/tests/test_subcmd_generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import sys
 
-import pytest
 from click.testing import CliRunner
 
 from elasticsearch_faker.__main__ import cmd
 
 
 class Test_generate_subcmd:
-    @pytest.mark.skipif(sys.version_info < (3, 6), reason="requires python3.6 or higher")
     def test_normal(self, mocker):
         runner = CliRunner()
         template_filename = "valid.tmpl"
 
         with runner.isolated_filesystem():
             with open(template_filename, "w") as f:
                 f.write(
```

### Comparing `elasticsearch-faker-0.2.0/tests/test_subcmd_validate.py` & `elasticsearch-faker-0.3.0/tests/test_subcmd_validate.py`

 * *Files identical despite different names*

### Comparing `elasticsearch-faker-0.2.0/tox.ini` & `elasticsearch-faker-0.3.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 [tox]
 envlist =
-    py{36,37,38,39,310}
+    py{37,38,39,310,311}
     pypy3
     build
-    clean
     cov
     fmt
     lint
 
 [testenv]
 passenv = *
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
-basepython = python3.8
 deps =
     twine
     wheel
 commands =
     python setup.py sdist bdist_wheel
     twine check dist/*.whl dist/*.tar.gz
     python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.3.1
+    cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
 [testenv:cov]
 passenv = *
 extras =
     test
@@ -41,24 +39,24 @@
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:fmt]
 skip_install = true
 deps =
-    autoflake>=1.4
-    black>=22.1
+    autoflake>=2
+    black>=23.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
     black setup.py tests elasticsearch_faker
 
 [testenv:lint]
 skip_install = true
 deps =
-    mypy>=0.931
-    pylama>=8.3.7
+    mypy>=1
+    pylama>=8.4.1
 commands =
     python setup.py check
     mypy elasticsearch_faker setup.py
     pylama
```

