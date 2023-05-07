# Comparing `tmp/tpcollections-0.0.2.tar.gz` & `tmp/tpcollections-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpcollections-0.0.2.tar", last modified: Sat May  6 16:56:42 2023, max compression
+gzip compressed data, was "tpcollections-0.0.3.tar", last modified: Sat May  6 17:50:47 2023, max compression
```

## Comparing `tpcollections-0.0.2.tar` & `tpcollections-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3078 2023-05-05 19:11:26.352439 tpcollections-0.0.2/.gitignore
--rw-r--r--   0        0        0      147 2023-05-05 19:11:26.352439 tpcollections-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-05 19:11:26.352439 tpcollections-0.0.2/LICENSE
--rw-r--r--   0        0        0    11401 2023-05-05 19:11:26.352439 tpcollections-0.0.2/LICENSE.apache
--rw-r--r--   0        0        0      188 2023-05-05 19:11:26.352439 tpcollections-0.0.2/LICENSE.rst
--rw-r--r--   0        0        0       52 2023-05-05 19:11:26.352439 tpcollections-0.0.2/Makefile
--rw-r--r--   0        0        0     2679 2023-05-06 13:43:28.883045 tpcollections-0.0.2/README.md
--rwxr-xr-x   0        0        0     2026 2023-05-06 16:53:33.707281 tpcollections-0.0.2/justfile
--rw-r--r--   0        0        0     1105 2023-05-06 16:56:31.844943 tpcollections-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      188 2023-05-06 12:46:19.495293 tpcollections-0.0.2/src/tpcollections/__init__.py
--rw-r--r--   0        0        0    12063 2023-05-06 16:15:09.267981 tpcollections-0.0.2/src/tpcollections/_db.py
--rw-r--r--   0        0        0    13147 2023-05-06 16:16:37.751362 tpcollections-0.0.2/src/tpcollections/_mapping.py
--rw-r--r--   0        0        0      925 2023-05-06 12:17:50.879505 tpcollections-0.0.2/src/tpcollections/_serializers.py
--rw-r--r--   0        0        0     1623 2023-05-06 02:32:11.037046 tpcollections-0.0.2/src/tpcollections/_util.py
--rw-r--r--   0        0        0        0 2023-05-05 19:11:26.353439 tpcollections-0.0.2/src/tpcollections/py.typed
--rw-r--r--   0        0        0        0 2023-05-06 02:32:11.037046 tpcollections-0.0.2/test/__init__.py
--rw-r--r--   0        0        0     6693 2023-05-06 16:13:48.868910 tpcollections-0.0.2/test/test_mapping.py
--rw-r--r--   0        0        0     7748 2023-05-06 16:13:39.443550 tpcollections-0.0.2/test/test_ordered_mapping.py
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 tpcollections-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-05-05 19:11:26.352439 tpcollections-0.0.3/.gitignore
+-rw-r--r--   0        0        0      147 2023-05-05 19:11:26.352439 tpcollections-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-05 19:11:26.352439 tpcollections-0.0.3/LICENSE
+-rw-r--r--   0        0        0    11401 2023-05-05 19:11:26.352439 tpcollections-0.0.3/LICENSE.apache
+-rw-r--r--   0        0        0      188 2023-05-05 19:11:26.352439 tpcollections-0.0.3/LICENSE.rst
+-rw-r--r--   0        0        0       52 2023-05-05 19:11:26.352439 tpcollections-0.0.3/Makefile
+-rw-r--r--   0        0        0     2687 2023-05-06 17:00:37.665189 tpcollections-0.0.3/README.md
+-rwxr-xr-x   0        0        0     2233 2023-05-06 17:07:10.369109 tpcollections-0.0.3/justfile
+-rw-r--r--   0        0        0     1105 2023-05-06 17:49:15.122867 tpcollections-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      303 2023-05-06 17:49:49.848182 tpcollections-0.0.3/src/tpcollections/__init__.py
+-rw-r--r--   0        0        0    12061 2023-05-06 17:50:29.975701 tpcollections-0.0.3/src/tpcollections/_db.py
+-rw-r--r--   0        0        0    21898 2023-05-06 17:50:29.975701 tpcollections-0.0.3/src/tpcollections/_mapping.py
+-rw-r--r--   0        0        0      925 2023-05-06 12:17:50.879505 tpcollections-0.0.3/src/tpcollections/_serializers.py
+-rw-r--r--   0        0        0     1623 2023-05-06 02:32:11.037046 tpcollections-0.0.3/src/tpcollections/_util.py
+-rw-r--r--   0        0        0        0 2023-05-05 19:11:26.353439 tpcollections-0.0.3/src/tpcollections/py.typed
+-rw-r--r--   0        0        0        0 2023-05-06 02:32:11.037046 tpcollections-0.0.3/test/__init__.py
+-rw-r--r--   0        0        0     6693 2023-05-06 16:13:48.868910 tpcollections-0.0.3/test/test_mapping.py
+-rw-r--r--   0        0        0     7748 2023-05-06 16:13:39.443550 tpcollections-0.0.3/test/test_ordered_mapping.py
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 tpcollections-0.0.3/PKG-INFO
```

### Comparing `tpcollections-0.0.2/.gitignore` & `tpcollections-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.2/LICENSE` & `tpcollections-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.2/LICENSE.apache` & `tpcollections-0.0.3/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.2/README.md` & `tpcollections-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 * Supports many collections in one database file, ensuring all the used tables
   are the right type and that there are no collisions.
 * Supports multiple attached database files, maintaining transactions,
   consistency, and durability across the entire set.
 * Supports 
 * Supported and tested on every reasonable version of Python and SQLite.
   * Tests are run all supported versions of Python, and on all in-support
-    versions of RHEL, CentOS, Fedora, Debian, and Alpine Linux.
+    versions of RHEL, CentOS, Fedora, Debian, Ubuntu, and Alpine Linux.
     * This includes versions of Python or SQLite otherwise considered out of
       support by upstream.  At the time of this writing, this includes CentOS 7
       and therefore Python 3.6.8 and SQLite 3.7.17.
     * This does not include extended support (i.e. Centos 6 and Debian Jessie),
       because I haven't found a free and easy way to automate testing for them.
       I would be happy to accept contributions to add this support.
 * SQLite features are version-tested, selecting the most appropriate features
```

### Comparing `tpcollections-0.0.2/justfile` & `tpcollections-0.0.3/justfile`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,36 @@
   /mnt/venv/bin/pip install --upgrade wheel
   /mnt/venv/bin/pip install --upgrade pip
   /mnt/venv/bin/pip install "/mnt/app[test]"
   cd /mnt/app
   /mnt/venv/bin/python -munittest
 '''
 
-yum_setup := '''
+yum-setup := '''
   yum update -y
   yum install -y python3 sqlite3 python3-pip python3-venv
 '''
 
-dnf_setup := '''
+dnf-setup := '''
   dnf update -y
   dnf install -y python3 sqlite python3-pip
 '''
 
-apt_setup := '''
+apt-setup := '''
   apt update
   apt upgrade -y
   apt install -y python3 sqlite3 python3-pip python3-venv
 '''
 
+apk-setup := '''
+  apk update
+  apk upgrade
+  apk add python3 sqlite
+'''
+
 all: test
 
 test: python-tests debian-tests ubuntu-tests centos-tests fedora-tests rhel-tests alpine-tests
 
 run-test $container $setup="":
   #!/bin/sh
   set -eux
@@ -45,29 +51,29 @@
       $runtest
     "
 
 test-python version="latest": (run-test ("python:" + version))
 
 python-tests: (test-python "3.6") (test-python "3.7") (test-python "3.8") (test-python "3.9") (test-python "3.10") (test-python "3.11")
 
-
-test-centos version="latest": (run-test ("centos:" + version) yum_setup)
+test-centos version="latest": (run-test ("centos:" + version) yum-setup)
 centos-tests: (test-centos "7")
 
-alpine-tests: (test-python "alpine")
+test-alpine version="latest": (run-test ("alpine:" + version) apk-setup)
+alpine-tests: (test-alpine "3.14") (test-alpine "3.15") (test-alpine "3.16") (test-alpine "3.17")
 
-test-apt image="debian:latest": (run-test image apt_setup)
+test-apt image="debian:latest": (run-test image apt-setup)
 
 test-debian version="latest": (test-apt ("debian:" + version))
 test-ubuntu version="latest": (test-apt ("ubuntu:" + version))
 
 debian-tests: (test-debian "buster") (test-debian "bullseye") (test-debian "bookworm")
 ubuntu-tests: (test-ubuntu "18.04") (test-ubuntu "20.04") (test-ubuntu "22.04")
 
-test-dnf image="fedora:latest": (run-test image dnf_setup)
+test-dnf image="fedora:latest": (run-test image dnf-setup)
 
 test-fedora version="latest": (test-dnf ("fedora:" + version))
 fedora-tests: (test-fedora "36") (test-fedora "37") (test-fedora "38")
 
 test-rhel version="ubi9": (test-dnf ("redhat/" + version))
 
 rhel-tests: (test-rhel "ubi8") (test-rhel "ubi9")
```

### Comparing `tpcollections-0.0.2/pyproject.toml` & `tpcollections-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'tpcollections'
 description = 'Persistent transactional Python collections'
-version = '0.0.2'
+version = '0.0.3'
 readme = 'README.md'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 1 - Planning',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

### Comparing `tpcollections-0.0.2/src/tpcollections/_db.py` & `tpcollections-0.0.3/src/tpcollections/_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,16 +271,16 @@
                 warnings.warn(
                     'Attaching a database inside a transaction can prevent '
                     'transactions from being atomic.'
                 )
 
             if not (self._memory or self._has_attachments or self.read_only):
                 # disable WAL mode when attaching databases
-                cursor.execute(f'PRAGMA main.journal_mode=DELETE')
-                cursor.execute(f'PRAGMA main.synchronous=FULL')
+                cursor.execute('PRAGMA main.journal_mode=DELETE')
+                cursor.execute('PRAGMA main.synchronous=FULL')
                 self._has_attachments = True
 
             cursor.execute(f'ATTACH ? AS {database_id}', (uri,))
             try:
                 if not (self.read_only or self._memory):
                     cursor.execute(f'PRAGMA {database_id}.journal_mode=DELETE')
                     cursor.execute(f'PRAGMA {database_id}.synchronous=FULL')
```

### Comparing `tpcollections-0.0.2/src/tpcollections/_mapping.py` & `tpcollections-0.0.3/src/tpcollections/_mapping.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import sqlite3
+from datetime import timedelta
 from typing import (
     Any,
-    Generic,
+    Callable,
     ItemsView,
     Iterable,
     Iterator,
     KeysView,
     Reversible,
     Tuple,
     TypeVar,
     ValuesView,
     MutableMapping,
+    cast,
 )
 from enum import unique, Enum
 
 from ._util import Identifier
 
 from . import _db, _serializers
 
@@ -137,27 +139,24 @@
             '''):
                 yield (
                     self._key_serializer.loads(key),
                     self._value_serializer.loads(value),
                 )
 
 class _MappingBase(_db._Base, MutableMapping[Key, Value]):
-    '''A database mapping.
-    '''
-
     __slots__ = (
         '_key_serializer',
         '_value_serializer',
     )
     def __init__(self,
         connection: _db.Connection,
         database: Identifier,
         table: Identifier,
-        key_serializer,
-        value_serializer,
+        key_serializer: _serializers.Serializer,
+        value_serializer: _serializers.Serializer,
         type: str,
     ) -> None:
         super().__init__(connection, Identifier(database), Identifier(table), type)
 
         self._key_serializer = key_serializer
         self._value_serializer = value_serializer
 
@@ -171,14 +170,20 @@
 
 
     def __bool__(self) -> bool:
         '''Check if the table is not empty.'''
 
         return len(self) > 0
 
+    def __iter__(self) -> Iterator[Key]:
+        return iter(cast(Callable[[],  Keys[Key]], self.keys)())
+
+    def __reversed__(self) -> Iterator[Key]:
+        return reversed(cast(Callable[[],  Keys[Key]], self.keys)())
+
     def keys(self, order: str) -> Keys[Key]:
         '''Iterate over keys in the table.
         '''
 
         return Keys(
             connection=self._connection,
             database=self._database,
@@ -291,14 +296,74 @@
     def clear(self) -> None:
         '''Delete all items from the table.
         '''
 
         with self._connection.cursor() as cursor:
             cursor.execute(f'DELETE FROM {self._database}.{self._table}')
 
+class Mapping(_MappingBase[Key, Value]):
+    '''A database mapping ordered by key.
+
+    The table is smaller than OrderedMapping, which needs to keep a separate
+    index for the keys and can't use WITHOUT ROWID.  This does not remember
+    insertion order, and is always ordered by key insertion order.
+    '''
+
+    __slots__ = ()
+
+    def __init__(self,
+        connection: _db.Connection,
+        database: str = 'main',
+        table: str = 'mapping',
+        key_serializer: _serializers.Serializer = _serializers.deterministic_json,
+        value_serializer: _serializers.Serializer = _serializers.pickle,
+    ) -> None:
+
+        super().__init__(
+            connection=connection,
+            database=Identifier(database),
+            table=Identifier(table),
+            type='mapping',
+            key_serializer=key_serializer,
+            value_serializer=value_serializer,
+        )
+
+        version = self._version
+        previous_version = version
+
+        if version < 1:
+            with self._connection.cursor() as cursor:
+                cursor.execute(f'''
+                    CREATE TABLE {self._database}.{self._table} (
+                        key {_db.ANY} PRIMARY KEY UNIQUE NOT NULL,
+                        value {_db.ANY} NOT NULL) {_db.STRICT_WITHOUT_ROWID}
+                ''')
+                version = 1
+
+        if version > 1:
+            raise ValueError('tpcollections is not forward compatible')
+
+        if version != previous_version:
+            self._version = version
+
+    def keys(self) -> Keys[Key]:
+        '''Iterate over keys in the table.
+        '''
+        return super().keys('key')
+
+    def values(self) -> Values[Value]:
+        '''Iterate over values in the table.
+        '''
+        return super().values('key')
+
+    def items(self) -> Items[Key, Value]:
+        '''Iterate over keys and values in the table.
+        '''
+        return super().items('key')
+
 class OrderedMapping(_MappingBase[Key, Value]):
     '''A database mapping.
     '''
 
     __slots__ = ()
 
     @unique
@@ -335,15 +400,15 @@
         version = self._version
         previous_version = version
 
         if version < 1:
             with self._connection.cursor() as cursor:
                 cursor.execute(f'''
                     CREATE TABLE {self._database}.{self._table} (
-                        id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
+                        id INTEGER PRIMARY KEY AUTOINCREMENT UNIQUE NOT NULL,
                         key {_db.ANY} UNIQUE NOT NULL,
                         value {_db.ANY} NOT NULL) {_db.STRICT}
                 ''')
                 version = 1
 
         if version > 1:
             raise ValueError('tpcollections is not forward compatible')
@@ -352,88 +417,280 @@
             self._version = version
 
     def keys(self, order: Order = Order.ID) -> Keys[Key]:
         '''Iterate over keys in the table.
         '''
         return super().keys(order)
 
-    def __iter__(self) -> Iterator[Key]:
-        return iter(self.keys())
-
-    def __reversed__(self) -> Iterator[Key]:
-        return reversed(self.keys())
-
     def values(self, order: Order = Order.ID) -> Values[Value]:
         '''Iterate over values in the table.
         '''
         return super().values(order)
 
     def items(self, order: Order = Order.ID) -> Items[Key, Value]:
         '''Iterate over keys and values in the table.
         '''
         return super().items(order)
 
-class Mapping(_MappingBase[Key, Value]):
-    '''A database mapping ordered by key.
+class _ExpiringMappingBase(_MappingBase[Key, Value]):
+    __slots__ = (
+        '_lifespan',
+    )
+    def __init__(self,
+        connection: _db.Connection,
+        database: Identifier,
+        table: Identifier,
+        key_serializer: _serializers.Serializer,
+        value_serializer: _serializers.Serializer,
+        type: str,
+        lifespan: int,
+    ) -> None:
+        assert lifespan > 0
 
-    The table is smaller than OrderedMapping, which needs to keep a separate
-    index for the keys and can't use WITHOUT ROWID.  This does not remember
-    insertion order, and is always ordered by key insertion order.
+        super().__init__(
+            connection=connection,
+            database=database,
+            table=table,
+            key_serializer=key_serializer,
+            value_serializer=value_serializer,
+            type=type,
+        )
+        self._lifespan = lifespan
+
+    @property
+    def lifespan(self) -> timedelta:
+        return timedelta(seconds=self._lifespan)
+
+    @lifespan.setter
+    def lifespan(self, value: timedelta) -> None:
+        lifespan = int(value.total_seconds())
+        assert lifespan > 0
+        self._lifespan = lifespan
+
+    def _setup_triggers(self) -> None:
+        with self._connection.cursor() as cursor:
+            trigger_name_base = self._database + "." + self._table
+            update_trigger = trigger_name_base + ".update"
+            insert_trigger = trigger_name_base + ".insert"
+
+            cursor.execute(f'''
+                CREATE TEMP TRIGGER IF NOT EXISTS {insert_trigger}
+                    AFTER INSERT ON {self._database}.{self._table}
+                BEGIN
+                    DELETE FROM {self._database}.{self._table}
+                        WHERE expire <= {_db.UNIXEPOCH};
+                END
+            ''')
+
+            cursor.execute(f'''
+                CREATE TEMP TRIGGER IF NOT EXISTS {update_trigger}
+                    AFTER UPDATE OF value ON {self._database}.{self._table}
+                BEGIN
+                    DELETE FROM {self._database}.{self._table}
+                        WHERE expire <= {_db.UNIXEPOCH};
+                END
+            ''')
+
+    def __setitem__(self, key: Key, value: Value) -> None:
+        '''Set or replace the item.
+        '''
+
+        with self._connection.cursor() as cursor:
+            if sqlite3.sqlite_version_info >= (3, 24):
+                cursor.execute(f'''
+                        INSERT INTO {self._database}.{self._table} (key, expires, value)
+                            VALUES (?, ({_db.UNIXEPOCH} + ?), ?)
+                            ON CONFLICT (key) DO UPDATE
+                            SET expires=excluded.expires, value=excluded.value
+                    ''',
+                    (
+                        self._key_serializer.dumps(key),
+                        self._lifespan,
+                        self._value_serializer.dumps(value),
+                    ),
+                )
+            elif key in self:
+                cursor.execute(f'''
+                        UPDATE {self._database}.{self._table}
+                            SET value=?3,
+                                expires=({_db.UNIXEPOCH} + ?2)
+                            WHERE key=?1
+                    ''',
+                    (
+                        self._key_serializer.dumps(key),
+                        self._lifespan,
+                        self._value_serializer.dumps(value),
+                    ),
+                )
+            else:
+                cursor.execute(f'''
+                        INSERT INTO {self._database}.{self._table} (key, expires, value)
+                            VALUES (?, ({_db.UNIXEPOCH} + ?), ?)
+                    ''',
+                    (
+                        self._key_serializer.dumps(key),
+                        self._lifespan,
+                        self._value_serializer.dumps(value),
+                    ),
+                )
+
+class ExpiringMapping(_ExpiringMappingBase[Key, Value]):
+    '''A database mapping.
     '''
 
     __slots__ = ()
 
+    @unique
+    class Order(str, Enum):
+        '''An ordering enum for iteration methods.
+        '''
+
+        KEY = 'key'
+        EXPIRE = 'expire'
+
+        def __str__(self) -> str:
+            return self.value
+
+        def __format__(self, format_spec: str) -> str:
+            return self.value.__format__(format_spec)
+
     def __init__(self,
         connection: _db.Connection,
         database: str = 'main',
-        table: str = 'mapping',
+        table: str = 'expiringmapping',
         key_serializer: _serializers.Serializer = _serializers.deterministic_json,
         value_serializer: _serializers.Serializer = _serializers.pickle,
+        lifespan: timedelta = timedelta(weeks=1),
     ) -> None:
 
         super().__init__(
             connection=connection,
             database=Identifier(database),
             table=Identifier(table),
-            type='mapping',
+            type='expiringmapping',
             key_serializer=key_serializer,
             value_serializer=value_serializer,
+            lifespan=int(lifespan.total_seconds()),
         )
 
         version = self._version
         previous_version = version
 
         if version < 1:
             with self._connection.cursor() as cursor:
                 cursor.execute(f'''
                     CREATE TABLE {self._database}.{self._table} (
                         key {_db.ANY} PRIMARY KEY UNIQUE NOT NULL,
-                        value {_db.ANY} NOT NULL) {_db.STRICT_WITHOUT_ROWID}
+                        expires INTEGER NOT NULL,
+                        value {_db.ANY} NOT NULL) {_db.STRICT}
+                ''')
+
+                cursor.execute(f'''
+                    CREATE INDEX {self._database}.{self._table + "_expires"}
+                        ON {self._database}.{self._table} (expires ASC)
                 ''')
                 version = 1
 
         if version > 1:
             raise ValueError('tpcollections is not forward compatible')
 
         if version != previous_version:
             self._version = version
 
-    def keys(self) -> Keys[Key]:
+        self._setup_triggers()
+
+    def keys(self, order: Order = Order.KEY) -> Keys[Key]:
         '''Iterate over keys in the table.
         '''
-        return super().keys('key')
+        return super().keys(order)
 
-    def __iter__(self) -> Iterator[Key]:
-        return iter(self.keys())
+    def values(self, order: Order = Order.KEY) -> Values[Value]:
+        '''Iterate over values in the table.
+        '''
+        return super().values(order)
 
-    def __reversed__(self) -> Iterator[Key]:
-        return reversed(self.keys())
+    def items(self, order: Order = Order.KEY) -> Items[Key, Value]:
+        '''Iterate over keys and values in the table.
+        '''
+        return super().items(order)
 
-    def values(self) -> Values[Value]:
+class ExpiringOrderedMapping(_ExpiringMappingBase[Key, Value]):
+    '''A database mapping.
+    '''
+
+    __slots__ = ()
+
+    @unique
+    class Order(str, Enum):
+        '''An ordering enum for iteration methods.
+        '''
+
+        ID = 'id'
+        KEY = 'key'
+        EXPIRE = 'expire'
+
+        def __str__(self) -> str:
+            return self.value
+
+        def __format__(self, format_spec: str) -> str:
+            return self.value.__format__(format_spec)
+
+    def __init__(self,
+        connection: _db.Connection,
+        database: str = 'main',
+        table: str = 'expiringorderedmapping',
+        key_serializer: _serializers.Serializer = _serializers.deterministic_json,
+        value_serializer: _serializers.Serializer = _serializers.pickle,
+        lifespan: timedelta = timedelta(weeks=1),
+    ) -> None:
+
+        super().__init__(
+            connection=connection,
+            database=Identifier(database),
+            table=Identifier(table),
+            type='expiringorderedmapping',
+            key_serializer=key_serializer,
+            value_serializer=value_serializer,
+            lifespan=int(lifespan.total_seconds()),
+        )
+
+        version = self._version
+        previous_version = version
+
+        if version < 1:
+            with self._connection.cursor() as cursor:
+                cursor.execute(f'''
+                    CREATE TABLE {self._database}.{self._table} (
+                        id INTEGER PRIMARY KEY AUTOINCREMENT UNIQUE NOT NULL,
+                        key {_db.ANY} UNIQUE NOT NULL,
+                        expires INTEGER NOT NULL,
+                        value {_db.ANY} NOT NULL) {_db.STRICT}
+                ''')
+
+                cursor.execute(f'''
+                    CREATE INDEX {self._database}.{self._table + "_expires"}
+                        ON {self._database}.{self._table} (expires ASC)
+                ''')
+                version = 1
+
+        if version > 1:
+            raise ValueError('tpcollections is not forward compatible')
+
+        if version != previous_version:
+            self._version = version
+
+        self._setup_triggers()
+
+    def keys(self, order: Order = Order.ID) -> Keys[Key]:
+        '''Iterate over keys in the table.
+        '''
+        return super().keys(order)
+
+    def values(self, order: Order = Order.ID) -> Values[Value]:
         '''Iterate over values in the table.
         '''
-        return super().values('key')
+        return super().values(order)
 
-    def items(self) -> Items[Key, Value]:
+    def items(self, order: Order = Order.ID) -> Items[Key, Value]:
         '''Iterate over keys and values in the table.
         '''
-        return super().items('key')
+        return super().items(order)
```

### Comparing `tpcollections-0.0.2/src/tpcollections/_serializers.py` & `tpcollections-0.0.3/src/tpcollections/_serializers.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.2/src/tpcollections/_util.py` & `tpcollections-0.0.3/src/tpcollections/_util.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.2/test/test_mapping.py` & `tpcollections-0.0.3/test/test_mapping.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.2/test/test_ordered_mapping.py` & `tpcollections-0.0.3/test/test_ordered_mapping.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.2/PKG-INFO` & `tpcollections-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpcollections
-Version: 0.0.2
+Version: 0.0.3
 Summary: Persistent transactional Python collections
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -64,15 +64,15 @@
 * Supports many collections in one database file, ensuring all the used tables
   are the right type and that there are no collisions.
 * Supports multiple attached database files, maintaining transactions,
   consistency, and durability across the entire set.
 * Supports 
 * Supported and tested on every reasonable version of Python and SQLite.
   * Tests are run all supported versions of Python, and on all in-support
-    versions of RHEL, CentOS, Fedora, Debian, and Alpine Linux.
+    versions of RHEL, CentOS, Fedora, Debian, Ubuntu, and Alpine Linux.
     * This includes versions of Python or SQLite otherwise considered out of
       support by upstream.  At the time of this writing, this includes CentOS 7
       and therefore Python 3.6.8 and SQLite 3.7.17.
     * This does not include extended support (i.e. Centos 6 and Debian Jessie),
       because I haven't found a free and easy way to automate testing for them.
       I would be happy to accept contributions to add this support.
 * SQLite features are version-tested, selecting the most appropriate features
```

