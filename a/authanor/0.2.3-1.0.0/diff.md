# Comparing `tmp/authanor-0.2.3.tar.gz` & `tmp/authanor-1.0.0.tar.gz`

## Comparing `authanor-0.2.3.tar` & `authanor-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,37 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/_version.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/database/__init__.py
--rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/database/handler.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/database/models.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/database/utils.py
--rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/testing/helpers.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 authanor-0.2.3/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-0.2.3/COPYING
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-0.2.3/LICENSE
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 authanor-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 authanor-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 authanor-1.0.0/Makefile
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 authanor-1.0.0/README.md
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 authanor-1.0.0/_vimrc_local.vim
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 authanor-1.0.0/config.mk
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 authanor-1.0.0/requirements.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    10513 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/index.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/api/database.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/api/testing.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/_version.py
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/database/__init__.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/database/handler.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/database/models.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/database/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/testing/__init__.py
+-rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/testing/helpers.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/database/test_db.py
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/database/test_handler.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/database/test_models.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/database/test_utils.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/helpers/test_helpers.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 authanor-1.0.0/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-1.0.0/COPYING
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 authanor-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 authanor-1.0.0/PKG-INFO
```

### Comparing `authanor-0.2.3/authanor/database/__init__.py` & `authanor-1.0.0/src/authanor/database/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,29 +92,32 @@
             An existing database interface instance to potentially use.
 
         Returns
         -------
         decorator : func
             The wrapper function that sets the database interface.
         """
+
         def _inner_decorator(init_app_func):
             @functools.wraps(init_app_func)
             def wrapper(app):
                 # Prepare database access with SQLAlchemy
                 #   - Use the `app.db` attribute like the `app.extensions` dict
                 #     (but not actually that dict because this is not an extension)
                 app.db = cls() if app.testing else interface_instance
                 app.db.setup_engine(db_path=app.config["DATABASE"])
                 init_app_func(app)
                 # Establish behavior for closing the database
                 app.teardown_appcontext(app.db.close)
                 # If testing, the database still needs to be initialized/prepopulated
                 if app.testing:
                     app.db.initialize(app)
+
             return wrapper
+
         return _inner_decorator
 
 
 @event.listens_for(Engine, "connect")
 def set_sqlite_pragma(dbapi_connection, connection_record):
     cursor = dbapi_connection.cursor()
     cursor.execute("PRAGMA foreign_keys=ON")
```

### Comparing `authanor-0.2.3/authanor/database/handler.py` & `authanor-1.0.0/src/authanor/database/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,21 +338,23 @@
         operation to succeed, and the saved entry should also be
         validated to ensure that it belongs to an authorized user. This
         method performs both functions: it takes the saved entry and
         queries the database for the up-to-date version, using the
         handler logic to choose either the entry or the corresponding
         view; that process implicitly guarantees authorization.
         """
+
         @functools.wraps(method)
         def wrapper(cls, *args, **kwargs):
             entry = method(cls, *args, **kwargs)
             # Return either the entry or its view (implicitly confirming authorizatio)
             entry_id = getattr(entry, entry.primary_key_field.name)
             entry = cls.get_entry(entry_id)
             return entry
+
         return wrapper
 
     @classmethod
     @entry_saver
     def add_entry(cls, **field_values):
         """
         Create a new entry in the database given field values.
```

### Comparing `authanor-0.2.3/authanor/database/models.py` & `authanor-1.0.0/src/authanor/database/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 ORM model definitions corresponding to tables in the SQLite database.
 """
 from datetime import date
 
 from flask import g
 from sqlalchemy import event, inspect, select
-from sqlalchemy.orm import DeclarativeBase, declared_attr
 from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy.orm import DeclarativeBase, declared_attr
 from sqlalchemy.sql.expression import TableClause
 from sqlalchemy_views import CreateView as _CreateView
 
 
 class Model(DeclarativeBase):
     """A declarative base for all models."""
 
@@ -140,14 +140,15 @@
     Notes
     -----
     This object uses a combination of the tooling provided by the
     `sqlalchemy_views` package (https://pypi.org/project/sqlalchemy-views/)
     and the SQLAlchemy wiki resource on 'Views'
     (https://github.com/sqlalchemy/sqlalchemy/wiki/Views).
     """
+
     inherit_cache = True
 
     def __init__(self, name, metadata, selectable):
         super().__init__(name)
         self._columns._populate_separate_keys(
             col._make_proxy(self) for col in selectable.selected_columns
         )
```

### Comparing `authanor-0.2.3/authanor/database/utils.py` & `authanor-1.0.0/src/authanor/database/utils.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.3/authanor/testing/helpers.py` & `authanor-1.0.0/src/authanor/testing/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Helper tools to improve testing of authorized database interactions.
 """
-import textwrap
 import functools
 import os
 import tempfile
+import textwrap
 from collections import namedtuple
 from contextlib import contextmanager
 from pprint import pformat
 
 import pytest
 from sqlalchemy import inspect, select
 from sqlalchemy.sql.expression import func
 from werkzeug.exceptions import NotFound
 
-
 registry = {"app_manager": None}
 
 
 class DefaultTestingConfig:
     """A Flask configuration designed for testing."""
+
     TESTING = True
     SECRET_KEY = "testing key"
 
     def __init__(self, db_path=None):
         self.DATABASE = db_path
 
 
@@ -37,19 +37,20 @@
     to persist the app and database throughout the duration of testing.
     However, tests that consist of complete SQLAlchemy transactions
     which alter the database (e.g., additions, updates, deletions;
     operations that include a commit) would change this persistent
     database version and impact subsequent tests. Since simply rolling
     back the changes is insufficient to restore the database, this
     object manages which app (and database) are used for a transaction.
-    The current app options are either
-        (1) A persistent app, which survives through the entire test
-            process and provides quick database access; or
-        (2) An ephemeral app, which is designed to survive through only
-            one single test.
+    The current app options are either:
+
+    #. A persistent app, which survives through the entire test
+       process and provides quick database access; or
+    #. An ephemeral app, which is designed to survive through only
+       one single test.
 
     To enable switching between the two types of apps, this class relies
     on two Pytest fixtures (`app_context` and `app_transaction_context`)
     to control the scope of the two apps. The `app_context` fixture is
     created just once for the session and is then automatically used in
     all tests. On the other hand, the `app_transaction_context` fixture
     may be manually included in any test, which causes an ephemeral app
@@ -152,18 +153,20 @@
         a lifetime of just this test (one database transaction).
 
     Returns
     -------
     wrapped_test_function : callable
         The wrapped test.
     """
+
     @pytest.mark.usefixtures("app_transaction_context")
     @functools.wraps(test_function)
     def wrapper(*args, **kwargs):
         test_function(*args, **kwargs)
+
     return wrapper
 
 
 class TestHandler:
     """A base class for testing database handlers."""
 
     @pytest.fixture(autouse=True)
@@ -233,25 +236,23 @@
         query = select(func.count(handler.model.primary_key_field))
         entry_count = self._app.db.session.execute(query).scalar()
         # Ensure that the mapping cannot be added for the invalid user
         with pytest.raises(NotFound):
             handler.add_entry(**mapping)
         # Rollback and ensure that an entry was not added
         self._app.db.close()
-        self.assert_number_of_matches(
-            entry_count, handler.model.primary_key_field
-        )
+        self.assert_number_of_matches(entry_count, handler.model.primary_key_field)
 
     def assert_entry_deletion_succeeds(self, handler, entry_id):
         handler.delete_entry(entry_id)
         # Check that the entry was deleted
         self.assert_number_of_matches(
             0,
             handler.model.primary_key_field,
-            handler.model.primary_key_field == entry_id
+            handler.model.primary_key_field == entry_id,
         )
 
 
 def pytest_generate_tests(metafunc):
     """
     Control test generation.
```

### Comparing `authanor-0.2.3/.gitignore` & `authanor-1.0.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -69,8 +69,8 @@
 # Mac custom attributes file
 .DS_Store
 
 # Virtual environment
 authanor-env/
 
 # Hatch-generated version file
-authanor/_version.py
+src/authanor/_version.py
```

### Comparing `authanor-0.2.3/COPYING` & `authanor-1.0.0/COPYING`

 * *Files identical despite different names*

