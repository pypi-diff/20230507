# Comparing `tmp/bh-database-0.0.1.tar.gz` & `tmp/bh-database-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bh-database-0.0.1.tar", last modified: Wed Jan 25 02:23:09 2023, max compression
+gzip compressed data, was "bh-database-0.0.2.tar", last modified: Sun May  7 00:59:16 2023, max compression
```

## Comparing `bh-database-0.0.1.tar` & `bh-database-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 02:23:09.741732 bh-database-0.0.1/
--rw-rw-rw-   0        0        0     2484 2023-01-25 02:23:09.740733 bh-database-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1858 2023-01-24 22:01:57.000000 bh-database-0.0.1/README.md
--rw-rw-rw-   0        0        0     1022 2023-01-25 01:50:56.000000 bh-database-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-25 02:23:09.741732 bh-database-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-25 02:23:09.707731 bh-database-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-01-25 02:23:09.715733 bh-database-0.0.1/src/bh_database/
--r--r--r--   0        0        0       90 2023-01-16 08:55:46.000000 bh-database-0.0.1/src/bh_database/__init__.py
--rw-rw-rw-   0        0        0    21672 2023-01-24 23:22:06.000000 bh-database-0.0.1/src/bh_database/base_table.py
--rw-rw-rw-   0        0        0     2239 2023-01-24 13:00:51.000000 bh-database-0.0.1/src/bh_database/constant.py
--rw-rw-rw-   0        0        0    16402 2023-01-25 00:36:44.000000 bh-database-0.0.1/src/bh_database/core.py
--rw-rw-rw-   0        0        0     5120 2023-01-24 13:10:52.000000 bh-database-0.0.1/src/bh_database/paginator.py
-drwxrwxrwx   0        0        0        0 2023-01-25 02:23:09.739732 bh-database-0.0.1/src/bh_database.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-01-25 02:23:09.000000 bh-database-0.0.1/src/bh_database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-01-25 02:23:09.000000 bh-database-0.0.1/src/bh_database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 02:23:09.000000 bh-database-0.0.1/src/bh_database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      190 2023-01-25 02:23:09.000000 bh-database-0.0.1/src/bh_database.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-01-25 02:23:09.000000 bh-database-0.0.1/src/bh_database.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.832926 bh-database-0.0.2/
+-rw-rw-rw-   0        0        0     2484 2023-05-07 00:59:16.832926 bh-database-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1858 2023-01-25 03:51:11.000000 bh-database-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1026 2023-05-07 00:55:04.000000 bh-database-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 00:59:16.832926 bh-database-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.788928 bh-database-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.796929 bh-database-0.0.2/src/bh_database/
+-rw-rw-rw-   0        0        0       90 2023-01-25 04:17:39.000000 bh-database-0.0.2/src/bh_database/__init__.py
+-rw-rw-rw-   0        0        0    22724 2023-05-06 02:18:13.000000 bh-database-0.0.2/src/bh_database/base_table.py
+-rw-rw-rw-   0        0        0     2239 2023-01-25 03:51:11.000000 bh-database-0.0.2/src/bh_database/constant.py
+-rw-rw-rw-   0        0        0    17779 2023-04-08 05:23:07.000000 bh-database-0.0.2/src/bh_database/core.py
+-rw-rw-rw-   0        0        0     5120 2023-01-25 03:51:11.000000 bh-database-0.0.2/src/bh_database/paginator.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.816957 bh-database-0.0.2/src/bh_database.egg-info/
+-rw-rw-rw-   0        0        0     2484 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.831928 bh-database-0.0.2/tests/
+-rw-rw-rw-   0        0        0     5782 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_01_core_database_postgresql.py
+-rw-rw-rw-   0        0        0     5682 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_02_core_database_mysql.py
+-rw-rw-rw-   0        0        0     3956 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_05_core_basesqlalchemy_postgresql.py
+-rw-rw-rw-   0        0        0     3634 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_06_core_basesqlalchemy_mysql.py
+-rw-rw-rw-   0        0        0     3394 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_11_paginator_postgresql.py
+-rw-rw-rw-   0        0        0     3309 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_12_paginator_mysql.py
+-rw-rw-rw-   0        0        0     6937 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_15_base_table_postgresql.py
+-rw-rw-rw-   0        0        0     6413 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_16_base_table_mysql.py
+-rw-rw-rw-   0        0        0     1651 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_17_base_table_methods.py
+-rw-rw-rw-   0        0        0     1616 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_20_base_table_dunder.py
+-rw-rw-rw-   0        0        0    19258 2023-04-08 12:11:15.000000 bh-database-0.0.2/tests/test_25_base_table_crud_methods_postgresql.py
+-rw-rw-rw-   0        0        0    19133 2023-04-08 12:10:59.000000 bh-database-0.0.2/tests/test_26_base_table_crud_methods_mysql.py
+-rw-rw-rw-   0        0        0     4335 2023-04-08 08:41:22.000000 bh-database-0.0.2/tests/test_30_base_table_exception_postgresql.py
+-rw-rw-rw-   0        0        0     4270 2023-04-08 08:43:50.000000 bh-database-0.0.2/tests/test_31_base_table_exception_mysql.py
```

### Comparing `bh-database-0.0.1/PKG-INFO` & `bh-database-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bh-database
-Version: 0.0.1
+Version: 0.0.2
 Summary: Database wrapper classes for SQLAlchemy.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_database
 Project-URL: documentation, https://bh-database.readthedocs.io/
 Keywords: SQLAlchemy,database,wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bh-database-0.0.1/README.md` & `bh-database-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.1/pyproject.toml` & `bh-database-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bh-database"
-version = "0.0.1"
+version = "0.0.2"
 description = "Database wrapper classes for SQLAlchemy."
 
 readme = "README.md"
 authors = [{ name = "Van Be Hai Nguyen", email = "behai_nguyen@hotmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["SQLAlchemy", "database", "wrapper"]
 
 dependencies = [
-    'tomli; python_version < "3.11"',
+    'tomli; python_version >= "3.10"',
     'SQLAlchemy', 
     'psycopg2',
     'mysql-connector-python',
-	'bh_apistatus',
+    'bh_apistatus',
     'bh_utils'
 ]
 
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 tests = [
```

### Comparing `bh-database-0.0.1/src/bh_database/base_table.py` & `bh-database-0.0.2/src/bh_database/base_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 Please note, :py:class:`WriteCapableTable` requires the target database to implement ``unique_id`` 
 table and associated ``get_unique_id`` stored method, please see :ref:`getting-started-database-requirements`
 for more detail.
 
 Relevant test modules:
 
     * ./tests/test_25_base_table_crud_methods_postgresql.py
-    * ./tests/test_26_base_table_crud_methods_mysql.py    
+    * ./tests/test_26_base_table_crud_methods_mysql.py
+    * ./tests/test_30_base_table_exception_postgresql.py
+    * ./tests/test_31_base_table_exception_mysql.py
 """
 
 from http import HTTPStatus
 from contextlib import closing
 
 import logging
 
@@ -454,32 +456,48 @@
                 return make_500_status(id_status.text)
 
             record[self._primary_key] = id_status.data[0][self._primary_key]
 
         return make_status()
 
     def _insert(self, list):
+        """Within a transaction, any database exception is not raised at this point,
+        they will be raised when calling flush or commit the current transaction.
+        Rollback the current transaction will not raise an exception, i.e. any database
+        violations seem to be removed by the rollback.
+        """
         for record in list:
             self.session.add(self._type(**record))
 
     def _update(self, list):
+        """Within a transaction, any database exception is not raised at this point,
+        they will be raised when calling flush or commit the current transaction.
+        Rollback the current transaction will not raise an exception, i.e. any database
+        violations seem to be removed by the rollback.
+        """
         for entry in list:
-			# raise Exception('Test exception from timesheet_entry._update(...)')
-
             stmt = (
                 update(self._type)
                 .where(self._type.__table__.columns[self._primary_key] == entry[self._primary_key])
                 .values(entry)
                 .execution_options(synchronize_session="fetch")
           )
             self.session.execute(stmt)
 
     def write_to_database(self, data: list) -> ResultStatus:
         """Write new records and modified records to the underlying database table.
 
+        When all data have been written, it will flush the transaction to cause any
+        potential database violation to come out as an exception so that the result
+        can be accurately determined, freeing the callers from having to handle any
+        possible exception. Callers only have to check the returned result.
+
+        Flushing the transaction also causes intermediate pending committed data be
+        available, callers can access these without having to call flush_transcation().
+
         :Assumptions:
 
             1. The table has a single primary key of type integer.
             2. The database already has table ``unique_id`` and stored method ``get_unique_id`` \
                 defined. Please see :ref:`getting-started-database-requirements` for more detail.
 
         :Transaction: callers must either call 
@@ -570,25 +588,24 @@
             # Getting new Ids for new records.
             status = self.__set_new_id(new_list)
 
             if (status.code != HTTPStatus.OK.value): return
 
             if len(new_list) > 0:
                 self._insert(new_list)
-                """
-                self._app_logger.debug('{} New [{}] records\'ve been written.'.\
-                                            format(len(new_list), self._type.__name__))
-                """
 
             if len(updated_list) > 0:
                 self._update(updated_list)
-                """
-                self._app_logger.debug('{} Updated [{}] records\'ve been written.'.\
-                                            format(len(updated_list), self._type.__name__))
-                """
+
+            # 
+            # This is to cause any potential database violation to raise exception, so
+            # that it will be handled by the exception block below: callers just have
+            # to work with the returned result.
+            #
+            self.session.flush()
 
             status = make_status(text=BH_SAVED_SUCCESSFUL_MSG)
             status.add_data(new_list, '{}_new_list'.format(self.__tablename__.lower()))
             status.add_data(updated_list, '{}_updated_list'.format(self.__tablename__.lower()))
 
         except Exception as e:
             self._app_logger.error(str(e))
```

### Comparing `bh-database-0.0.1/src/bh_database/constant.py` & `bh-database-0.0.2/src/bh_database/constant.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.1/src/bh_database/core.py` & `bh-database-0.0.2/src/bh_database/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,24 +44,28 @@
     Database.connect(db_url, [schema | None])
 """
 
 import logging
 # from threading import get_ident
 from enum import Enum
 
+from http import HTTPStatus
+
 from sqlalchemy import create_engine
 from sqlalchemy.orm import (
     sessionmaker, 
     scoped_session,
     declarative_base,
     close_all_sessions,
     Query,
 )
 from sqlalchemy.orm.decl_api import DeclarativeMeta
 
+from bh_apistatus.result_status import ResultStatus
+
 from bh_database.paginator import Paginator
 
 #: 
 Base = declarative_base(metaclass=DeclarativeMeta)
 
 class BaseQuery(Query):
     """Custom base query class.
@@ -140,29 +144,58 @@
 
     def flush_transaction(self):
         """Flush an ongoing transaction.
 
         Make intermediate results available so that they can be accessed while the transaction 
         is still on going. An example of intermediate result is a new unique key value, this 
         value might be needed as a foreign key for detail records awaiting written.
+
+        :Note on Exception: 
+
+        Potential unhandled exception: caller must handle the exception.
+
+        Within an ongoing transaction, if there is any potential database violation, calling 
+        this method will cause the driver to raise exception on the violation.
         """
         self.session.flush()
 
     def commit_transaction(self):
         """Commit a current transaction.
+
+        :Note on Exception: 
+
+        Potential unhandled exception: caller must handle the exception.
+
+        Within an ongoing transaction, if there is any potential database violation, calling 
+        this method will cause the driver to raise exception on the violation.
+
+        It is recommended to call :py:meth:`~finalise_transaction` instead.
         """
         self.session.commit()
         self.session.close()
 
     def rollback_transaction(self):
         """Rollback a current transaction.
+
+        When absolutely certain that the ongoing transaction must be rolled back, then call
+        this method. Otherwise it is recommended to call :py:meth:`~finalise_transaction` 
+        instead.
         """
         self.session.rollback()
         self.session.close()
 
+    def finalise_transaction(self, status: ResultStatus):
+        """Commit or rollback a transaction based on ``status.code``.
+
+        :param ResultStatus status: result of the last CRUD call. \
+            `ResultStatus <https://bh-apistatus.readthedocs.io/en/latest/result-status.html>`_.
+        """
+        self.commit_transaction() \
+            if (status.code == HTTPStatus.OK.value ) else self.rollback_transaction()
+
 class DatabaseType(Enum):
     """Enumerated constants identifying supported databases.
 
     Define some enumerations for the supported database servers.
     """    
     Unknown = -1
     MySQL = 1
```

### Comparing `bh-database-0.0.1/src/bh_database/paginator.py` & `bh-database-0.0.2/src/bh_database/paginator.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.1/src/bh_database.egg-info/PKG-INFO` & `bh-database-0.0.2/src/bh_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bh-database
-Version: 0.0.1
+Version: 0.0.2
 Summary: Database wrapper classes for SQLAlchemy.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_database
 Project-URL: documentation, https://bh-database.readthedocs.io/
 Keywords: SQLAlchemy,database,wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

