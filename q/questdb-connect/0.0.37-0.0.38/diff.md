# Comparing `tmp/questdb-connect-0.0.37.tar.gz` & `tmp/questdb-connect-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.37.tar", last modified: Thu May  4 09:46:55 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.38.tar", last modified: Sun May  7 15:13:41 2023, max compression
```

## Comparing `questdb-connect-0.0.37.tar` & `questdb-connect-0.0.38.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-04 09:46:55.923164 questdb-connect-0.0.37/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.37/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4425 2023-05-04 09:46:55.923004 questdb-connect-0.0.37/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3718 2023-05-03 11:11:17.000000 questdb-connect-0.0.37/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2510 2023-05-04 09:45:14.000000 questdb-connect-0.0.37/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-04 09:46:55.923208 questdb-connect-0.0.37/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-04 09:46:55.918511 questdb-connect-0.0.37/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-04 09:46:55.920723 questdb-connect-0.0.37/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1960 2023-05-03 09:57:40.000000 questdb-connect-0.0.37/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11566 2023-05-03 12:23:45.000000 questdb-connect-0.0.37/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.37/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10535 2023-05-04 07:43:58.000000 questdb-connect-0.0.37/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.37/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-04 09:46:55.921717 questdb-connect-0.0.37/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4425 2023-05-04 09:46:55.000000 questdb-connect-0.0.37/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-04 09:46:55.000000 questdb-connect-0.0.37/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-04 09:46:55.000000 questdb-connect-0.0.37/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-04 09:46:55.000000 questdb-connect-0.0.37/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-04 09:46:55.000000 questdb-connect-0.0.37/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-04 09:46:55.000000 questdb-connect-0.0.37/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-04 09:46:55.922577 questdb-connect-0.0.37/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.37/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.37/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.37/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.094624 questdb-connect-0.0.38/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.38/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3375 2023-05-07 15:13:41.094456 questdb-connect-0.0.38/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2668 2023-05-07 15:11:39.000000 questdb-connect-0.0.38/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2514 2023-05-07 15:13:04.000000 questdb-connect-0.0.38/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-07 15:13:41.094663 questdb-connect-0.0.38/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.087209 questdb-connect-0.0.38/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.089887 questdb-connect-0.0.38/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-07 15:01:28.000000 questdb-connect-0.0.38/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.38/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.38/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10535 2023-05-04 07:43:58.000000 questdb-connect-0.0.38/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.38/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.092515 questdb-connect-0.0.38/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3375 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.093905 questdb-connect-0.0.38/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.38/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.38/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.38/tests/test_types.py
```

### Comparing `questdb-connect-0.0.37/LICENSE` & `questdb-connect-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.37/pyproject.toml` & `questdb-connect-0.0.38/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.37"
+version = "0.0.38"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -35,16 +35,14 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
     'psycopg2-binary~=2.9.6',
     'SQLAlchemy<=1.4.47',
-    'apache-superset>=2.1.0',
-    'sqlparse==0.4.3',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/questdb/questdb-connect/"
 "Bug Tracker" = "https://github.com/questdb/questdb-connect/issues/"
 
 [project.entry-points.'sqlalchemy.dialects']
@@ -53,14 +51,16 @@
 [project.entry-points.'superset.db_engine_specs']
 questdb = 'questdb_connect.superset:QDBEngineSpec'
 
 [project.optional-dependencies]
 test = [
     'ruff~=0.0.261',
     'pytest~=7.3.0',
+    'apache-superset>=2.1.0',
+    'sqlparse==0.4.3',
 ]
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 select = ["PL", "RUF", "TCH", "TID", "PT", "C4", "B", "S", "I"]
 line-length = 120
 exclude = [
@@ -77,8 +77,8 @@
 max-args = 10
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
 "tests/test_types.py" = ["S101"]
 "tests/test_superset.py" = ["S101"]
 "tests/conftest.py" = ["S608"]
-"examples/simple2.py" = ["S608"]
+"examples/sql_alchemy.py" = ["S608"]
```

### Comparing `questdb-connect-0.0.37/src/questdb_connect/__init__.py` & `questdb-connect-0.0.38/src/questdb_connect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 
 import psycopg2
 
-from .types import *
-
 # ===== DBAPI =====
 
 # https://peps.python.org/pep-0249/
 
 apilevel = '2.0'
 threadsafety = 2
 paramstyle = 'pyformat'
```

### Comparing `questdb-connect-0.0.37/src/questdb_connect/dialect.py` & `questdb-connect-0.0.38/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,21 @@
 #
 import abc
 
 import sqlalchemy
 from sqlalchemy import Column, MetaData, text
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector
-from sqlalchemy.exc import ArgumentError
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema
-from .types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
+from .types import *
 
 # ===== SQLAlchemy Dialect ======
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
```

### Comparing `questdb-connect-0.0.37/src/questdb_connect/function_names.py` & `questdb-connect-0.0.38/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.37/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.38/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.37/src/questdb_connect/types.py` & `questdb-connect-0.0.38/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.37/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.38/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.37/tests/test_dialect.py` & `questdb-connect-0.0.38/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.37/tests/test_superset.py` & `questdb-connect-0.0.38/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.37/tests/test_types.py` & `questdb-connect-0.0.38/tests/test_types.py`

 * *Files identical despite different names*

