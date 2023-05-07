# Comparing `tmp/quart-db-0.4.1.tar.gz` & `tmp/quart_db-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart-db-0.4.1.tar", max compression
+gzip compressed data, was "quart_db-0.5.0.tar", max compression
```

## Comparing `quart-db-0.4.1.tar` & `quart_db-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1050 2022-08-23 09:22:05.667998 quart-db-0.4.1/LICENSE
--rw-r--r--   0        0        0     2744 2022-10-08 16:00:37.807333 quart-db-0.4.1/README.rst
--rw-r--r--   0        0        0     2423 2022-10-09 09:17:14.168596 quart-db-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      235 2022-10-08 16:00:37.807333 quart-db-0.4.1/src/quart_db/__init__.py
--rw-r--r--   0        0        0     3040 2022-10-08 16:00:37.807333 quart-db-0.4.1/src/quart_db/_migration.py
--rw-r--r--   0        0        0        0 2022-10-08 16:00:37.807333 quart-db-0.4.1/src/quart_db/backends/__init__.py
--rw-r--r--   0        0        0     8397 2022-10-08 16:00:37.807333 quart-db-0.4.1/src/quart_db/backends/aiosqlite.py
--rw-r--r--   0        0        0     8274 2022-10-08 16:00:37.807333 quart-db-0.4.1/src/quart_db/backends/asyncpg.py
--rw-r--r--   0        0        0     8021 2022-10-08 16:00:37.807333 quart-db-0.4.1/src/quart_db/extension.py
--rw-r--r--   0        0        0     4820 2022-10-08 16:00:37.807333 quart-db-0.4.1/src/quart_db/interfaces.py
--rw-r--r--   0        0        0        7 2022-08-23 09:22:05.671998 quart-db-0.4.1/src/quart_db/py.typed
--rw-r--r--   0        0        0     3844 2022-10-09 09:17:19.451616 quart-db-0.4.1/setup.py
--rw-r--r--   0        0        0     4180 2022-10-09 09:17:19.452079 quart-db-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1050 2023-05-07 10:50:15.598252 quart_db-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2744 2023-05-07 10:50:15.598252 quart_db-0.5.0/README.rst
+-rw-r--r--   0        0        0     2469 2023-05-07 10:50:15.602252 quart_db-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-05-07 10:50:15.602252 quart_db-0.5.0/src/quart_db/__init__.py
+-rw-r--r--   0        0        0     3040 2023-05-07 10:50:15.602252 quart_db-0.5.0/src/quart_db/_migration.py
+-rw-r--r--   0        0        0        0 2023-05-07 10:50:15.602252 quart_db-0.5.0/src/quart_db/backends/__init__.py
+-rw-r--r--   0        0        0     8543 2023-05-07 10:50:15.602252 quart_db-0.5.0/src/quart_db/backends/aiosqlite.py
+-rw-r--r--   0        0        0     8435 2023-05-07 10:50:15.602252 quart_db-0.5.0/src/quart_db/backends/asyncpg.py
+-rw-r--r--   0        0        0     8951 2023-05-07 10:50:15.602252 quart_db-0.5.0/src/quart_db/extension.py
+-rw-r--r--   0        0        0     4862 2023-05-07 10:50:15.602252 quart_db-0.5.0/src/quart_db/interfaces.py
+-rw-r--r--   0        0        0        7 2023-05-07 10:50:15.602252 quart_db-0.5.0/src/quart_db/py.typed
+-rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 quart_db-0.5.0/PKG-INFO
```

### Comparing `quart-db-0.4.1/LICENSE` & `quart_db-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quart-db-0.4.1/README.rst` & `quart_db-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `quart-db-0.4.1/pyproject.toml` & `quart_db-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "quart-db"
-version = "0.4.1"
+version = "0.5.0"
 description = "Quart-DB is a Quart extension that provides managed connection(s) to database(s)."
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["src/quart_db/py.typed"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/pgjones/quart-db/"
```

### Comparing `quart-db-0.4.1/src/quart_db/_migration.py` & `quart_db-0.5.0/src/quart_db/_migration.py`

 * *Files identical despite different names*

### Comparing `quart-db-0.4.1/src/quart_db/backends/aiosqlite.py` & `quart_db-0.5.0/src/quart_db/backends/aiosqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 async with self._connection.execute(query, values) as cursor:
                     result = await cursor.fetchone()
         except ProgrammingError as error:
             raise UndefinedParameterError(str(error))
         else:
             return result[0]
 
-    async def iterate(  # type: ignore[override]
+    async def iterate(
         self,
         query: str,
         values: Optional[Dict[str, Any]] = None,
     ) -> AsyncGenerator[RecordType, None]:
         try:
             async with self._lock:
                 async with self._connection.execute(query, values) as cursor:
@@ -139,17 +139,18 @@
             raise UndefinedParameterError(str(error))
 
     def transaction(self, *, force_rollback: bool = False) -> "Transaction":
         return Transaction(self, force_rollback=force_rollback)
 
 
 class Backend(BackendABC):
-    def __init__(self, url: str, type_converters: TypeConverters) -> None:
+    def __init__(self, url: str, options: Dict[str, Any], type_converters: TypeConverters) -> None:
         _, _, path, *_ = urlsplit(url)
         self._path = path[1:]
+        self._options = options
         self._connections: Set[aiosqlite.Connection] = set()
         for _, converters in type_converters.items():
             for typename, (encoder, decoder, pytype) in converters.items():
                 aiosqlite.register_adapter(pytype, encoder)
                 aiosqlite.register_converter(typename, decoder)
 
     async def connect(self) -> None:
@@ -160,14 +161,15 @@
         await asyncio.wait_for(asyncio.gather(*tasks), timeout)
 
     async def acquire(self) -> Connection:
         connection = aiosqlite.connect(
             database=self._path,
             isolation_level=None,
             detect_types=PARSE_COLNAMES,
+            **self._options,
         )
         await connection.__aenter__()
         connection.row_factory = aiosqlite.Row
         self._connections.add(connection)
         return Connection(connection)
 
     async def release(self, connection: Connection) -> None:  # type: ignore[override]
@@ -184,27 +186,29 @@
         return Connection(connection)
 
     async def _release_migration_connection(self, connection: Connection) -> None:  # type: ignore[override]  # noqa: E501
         await connection._connection.__aexit__(None, None, None)
 
 
 class TestingBackend(BackendABC):
-    def __init__(self, url: str, type_converters: TypeConverters) -> None:
+    def __init__(self, url: str, options: Dict[str, Any], type_converters: TypeConverters) -> None:
         _, _, path, *_ = urlsplit(url)
         self._path = path[1:]
+        self._options = options
         for _, converters in type_converters.items():
             for typename, (encoder, decoder, pytype) in converters.items():
                 aiosqlite.register_adapter(pytype, encoder)
                 aiosqlite.register_converter(typename, decoder)
 
     async def connect(self) -> None:
         connection = aiosqlite.connect(
             database=self._path,
             isolation_level=None,
             detect_types=PARSE_COLNAMES,
+            **self._options,
         )
         await connection.__aenter__()
         self._connection = Connection(connection)
 
     async def disconnect(self, timeout: Optional[int] = None) -> None:
         await asyncio.wait_for(self._connection._connection.close(), timeout)
```

### Comparing `quart-db-0.4.1/src/quart_db/backends/asyncpg.py` & `quart_db-0.5.0/src/quart_db/backends/asyncpg.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         compiled_query, args = self._compile(query, values)
         try:
             async with self._lock:
                 return await self._connection.fetchval(compiled_query, *args)
         except asyncpg.exceptions.UndefinedParameterError as error:
             raise UndefinedParameterError(str(error))
 
-    async def iterate(  # type: ignore[override]
+    async def iterate(
         self,
         query: str,
         values: Optional[Dict[str, Any]] = None,
     ) -> AsyncGenerator[RecordType, None]:
         compiled_query, args = self._compile(query, values)
         async with self._lock:
             async with self._connection.transaction():
@@ -145,25 +145,27 @@
             try:
                 return render(query, **(values or {}))
             except BuildError as error:
                 raise UndefinedParameterError(str(error))
 
 
 class Backend(BackendABC):
-    def __init__(self, url: str, type_converters: TypeConverters) -> None:
+    def __init__(self, url: str, options: Dict[str, Any], type_converters: TypeConverters) -> None:
         self._pool: Optional[asyncpg.Pool] = None
         self._url = url
+        self._options = options
         self._type_converters = {**DEFAULT_TYPE_CONVERTERS, **type_converters}  # type: ignore
 
     async def connect(self) -> None:
         if self._pool is None:
-            self._pool = await asyncpg.create_pool(dsn=self._url, init=self._init)
+            self._pool = await asyncpg.create_pool(dsn=self._url, init=self._init, **self._options)
 
     async def disconnect(self, timeout: Optional[int] = None) -> None:
-        await asyncio.wait_for(self._pool.close(), timeout)
+        if self._pool is not None:
+            await asyncio.wait_for(self._pool.close(), timeout)
         self._pool = None
 
     async def acquire(self) -> Connection:
         connection = await self._pool.acquire()
         return Connection(connection)
 
     async def release(self, connection: Connection) -> None:  # type: ignore[override]
@@ -178,20 +180,21 @@
         await connection._connection.close()
 
     async def _init(self, connection: asyncpg.Connection) -> None:
         await _init_connection(connection, self._type_converters)  # type: ignore
 
 
 class TestingBackend(BackendABC):
-    def __init__(self, url: str, type_converters: TypeConverters) -> None:
+    def __init__(self, url: str, options: Dict[str, Any], type_converters: TypeConverters) -> None:
         self._url = url
+        self._options = options
         self._type_converters = {**DEFAULT_TYPE_CONVERTERS, **type_converters}  # type: ignore
 
     async def connect(self) -> None:
-        self._connection = Connection(await asyncpg.connect(dsn=self._url))
+        self._connection = Connection(await asyncpg.connect(dsn=self._url, **self._options))
         await _init_connection(self._connection._connection, self._type_converters)  # type: ignore
 
     async def disconnect(self, timeout: Optional[int] = None) -> None:
         await asyncio.wait_for(self._connection._connection.close(), timeout)
 
     async def acquire(self) -> Connection:
         return self._connection
```

### Comparing `quart-db-0.4.1/src/quart_db/extension.py` & `quart_db-0.5.0/src/quart_db/extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import asyncio
 from collections import defaultdict
 from contextlib import asynccontextmanager
-from typing import AsyncIterator, Callable, Optional, Type
+from typing import Any, AsyncIterator, Callable, Dict, Optional, Type
 from urllib.parse import urlsplit
 
 import click
 from quart import g, Quart, Response
 from quart.cli import pass_script_info, ScriptInfo
 
 from ._migration import setup_schema
@@ -47,36 +48,44 @@
              and QUART_DB_DATABASE_URL used instead.
         migrations_folder: Location of migrations relative to the
              app's root path, defaults to "migrations".
         data_path: Location of any initial data relative to the apps'
              root path. Can be None.
         auto_request_connection: If True (the default) a connection
              is acquired and placed on g for each request.
+        backend_options: Options to pass directly to the backend
+             engines. Will depend on the backend used.
     """
 
     def __init__(
         self,
         app: Optional[Quart] = None,
         *,
         url: Optional[str] = None,
         migrations_folder: Optional[str] = "migrations",
         data_path: Optional[str] = None,
         auto_request_connection: bool = True,
+        backend_options: Optional[Dict[str, Any]] = None,
     ) -> None:
         self._close_timeout = 5  # Seconds
         self._url = url
+        self._backend_options = backend_options
+        if self._backend_options is None:
+            self._backend_options = {}
         self._backend: Optional[BackendABC] = None
         self._type_converters: TypeConverters = defaultdict(dict)
         self._migrations_folder = migrations_folder
         self._data_path = data_path
         self._auto_request_connection = auto_request_connection
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app: Quart) -> None:
+        app.extensions.setdefault("QUART_DB", []).append(self)
+
         if self._url is None:
             self._url = app.config["QUART_DB_DATABASE_URL"]
         if self._migrations_folder is None:
             self._migrations_folder = app.config.get("QUART_DB_MIGRATIONS_FOLDER")
         if self._data_path is None:
             self._data_path = app.config.get("QUART_DB_DATA_PATH")
         self._root_path = app.root_path
@@ -90,14 +99,15 @@
         app.before_serving(self.before_serving)
         app.after_serving(self.after_serving)
 
         if app.config.get("QUART_DB_AUTO_REQUEST_CONNECTION", self._auto_request_connection):
             app.before_request(self.before_request)
             app.after_request(self.after_request)
 
+        app.cli.add_command(_migrate_command)
         app.cli.add_command(_schema_command)
 
     async def before_serving(self) -> None:
         self._backend = self._create_backend()
 
         if self._migrations_folder is not None or self._data_path is not None:
             await self.migrate()
@@ -191,28 +201,28 @@
             pytype: Optional Python type, required for SQLite.
             schema: Optional Postgres schema, defaults to "public".
         """
         self._type_converters[schema][typename] = (encoder, decoder, pytype)
 
     def _create_backend(self) -> BackendABC:
         scheme, *_ = urlsplit(self._url)
-        if scheme == "postgresql":
+        if scheme in {"postgresql", "postgres"}:
             from .backends.asyncpg import Backend, TestingBackend
 
             if self._testing:
-                return TestingBackend(self._url, self._type_converters)
+                return TestingBackend(self._url, self._backend_options, self._type_converters)
             else:
-                return Backend(self._url, self._type_converters)
+                return Backend(self._url, self._backend_options, self._type_converters)
         elif scheme == "sqlite":
             from .backends.aiosqlite import Backend, TestingBackend  # type: ignore
 
             if self._testing:
-                return TestingBackend(self._url, self._type_converters)
+                return TestingBackend(self._url, self._backend_options, self._type_converters)
             else:
-                return Backend(self._url, self._type_converters)
+                return Backend(self._url, self._backend_options, self._type_converters)
         else:
             raise ValueError(f"{scheme} is not a supported backend")
 
 
 @click.command("db-schema")
 @click.option(
     "--output",
@@ -227,7 +237,21 @@
 
     try:
         from eralchemy2 import render_er  # type: ignore
     except ImportError:
         click.echo("Quart-DB needs to be installed with the erdiagram extra")
     else:
         render_er(app.config["QUART_DB_DATABASE_URL"], output, exclude_tables=["schema_migration"])
+
+
+@click.command("db-migrate")
+@pass_script_info
+def _migrate_command(info: ScriptInfo) -> None:
+    app = info.load_app()
+
+    async def _inner() -> None:
+        for extension in app.extensions["QUART_DB"]:
+            extension._backend = extension._create_backend()
+            await extension.migrate()
+
+    asyncio.run(_inner())
+    click.echo("Quart-DB migration complete")
```

### Comparing `quart-db-0.4.1/src/quart_db/interfaces.py` & `quart_db-0.5.0/src/quart_db/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         The query accepts named arguments i.e. `:name`in the query
         with values set being a dictionary.
 
         """
         pass
 
     @abstractmethod
-    async def iterate(
+    def iterate(
         self,
         query: str,
         values: Optional[Dict[str, Any]] = None,
     ) -> AsyncGenerator[RecordType, None]:
         """Execute a query, and iterate over the result rows
 
         The query accepts named arguments i.e. `:name`in the query
@@ -119,15 +119,17 @@
             force_rollback: Force the transaction to rollback on completion.
         """
         pass
 
 
 class BackendABC(ABC):
     @abstractmethod
-    def __init__(self, url: str, type_converters: TypeConverters) -> None:
+    def __init__(
+        self, url: str, options: Optional[Dict[str, Any]], type_converters: TypeConverters
+    ) -> None:
         pass
 
     @abstractmethod
     async def connect(self) -> None:
         """Connect to the database.
 
         This will establish a connection pool if the backend supports
@@ -144,15 +146,14 @@
         complete.
 
         """
         pass
 
     @abstractmethod
     async def acquire(self) -> ConnectionABC:
-
         """Acquire a connection to the database.
 
         Don't forget to release it after usage,
 
         .. code-block::: python
 
             connection = await backend.acquire()
```

### Comparing `quart-db-0.4.1/PKG-INFO` & `quart_db-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 Metadata-Version: 2.1
 Name: quart-db
-Version: 0.4.1
+Version: 0.5.0
 Summary: Quart-DB is a Quart extension that provides managed connection(s) to database(s).
 Home-page: https://github.com/pgjones/quart-db/
 License: MIT
 Author: pgjones
 Author-email: philip.graham.jones@googlemail.com
 Requires-Python: >=3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: erdiagram
 Provides-Extra: sqlite
-Requires-Dist: aiosqlite (>=0.17.0); extra == "sqlite"
+Requires-Dist: aiosqlite (>=0.17.0) ; extra == "sqlite"
 Requires-Dist: asyncpg (>=0.25.0)
 Requires-Dist: buildpg (>=0.4)
-Requires-Dist: eralchemy2 (>=1.3.2); extra == "erdiagram"
-Requires-Dist: psycopg2 (>=2.9.3); extra == "erdiagram"
-Requires-Dist: pydata_sphinx_theme; extra == "docs"
+Requires-Dist: eralchemy2 (>=1.3.2) ; extra == "erdiagram"
+Requires-Dist: psycopg2 (>=2.9.3) ; extra == "erdiagram"
+Requires-Dist: pydata_sphinx_theme ; extra == "docs"
 Requires-Dist: quart (>=0.16.3)
 Project-URL: Repository, https://github.com/pgjones/quart-db/
 Description-Content-Type: text/x-rst
 
 Quart-DB
 ========
```

