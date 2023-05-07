# Comparing `tmp/tpcollections-0.1.0.tar.gz` & `tmp/tpcollections-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpcollections-0.1.0.tar", last modified: Sun May  7 15:17:17 2023, max compression
+gzip compressed data, was "tpcollections-0.1.1.tar", last modified: Sun May  7 15:19:56 2023, max compression
```

## Comparing `tpcollections-0.1.0.tar` & `tpcollections-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     3078 2023-05-05 19:11:26.352439 tpcollections-0.1.0/.gitignore
--rw-r--r--   0        0        0    12288 2023-05-07 14:21:45.975212 tpcollections-0.1.0/:memory
--rw-r--r--   0        0        0      147 2023-05-05 19:11:26.352439 tpcollections-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-05 19:11:26.352439 tpcollections-0.1.0/LICENSE
--rw-r--r--   0        0        0    11401 2023-05-05 19:11:26.352439 tpcollections-0.1.0/LICENSE.apache
--rw-r--r--   0        0        0      188 2023-05-05 19:11:26.352439 tpcollections-0.1.0/LICENSE.rst
--rw-r--r--   0        0        0       52 2023-05-05 19:11:26.352439 tpcollections-0.1.0/Makefile
--rw-r--r--   0        0        0     2687 2023-05-06 17:00:37.665189 tpcollections-0.1.0/README.md
--rwxr-xr-x   0        0        0     2233 2023-05-06 17:07:10.369109 tpcollections-0.1.0/justfile
--rw-r--r--   0        0        0     1102 2023-05-07 15:17:02.012216 tpcollections-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      347 2023-05-07 15:10:44.113643 tpcollections-0.1.0/src/tpcollections/__init__.py
--rw-r--r--   0        0        0    12061 2023-05-06 17:50:29.975701 tpcollections-0.1.0/src/tpcollections/_db.py
--rw-r--r--   0        0        0    21724 2023-05-07 15:12:39.143781 tpcollections-0.1.0/src/tpcollections/_mapping.py
--rw-r--r--   0        0        0      960 2023-05-07 15:13:03.680664 tpcollections-0.1.0/src/tpcollections/_serializers.py
--rw-r--r--   0        0        0     1623 2023-05-07 15:10:44.109643 tpcollections-0.1.0/src/tpcollections/_util.py
--rw-r--r--   0        0        0        0 2023-05-05 19:11:26.353439 tpcollections-0.1.0/src/tpcollections/py.typed
--rw-r--r--   0        0        0        0 2023-05-06 02:32:11.037046 tpcollections-0.1.0/test/__init__.py
--rw-r--r--   0        0        0     2646 2023-05-07 15:10:44.108643 tpcollections-0.1.0/test/test_expiring_mapping.py
--rw-r--r--   0        0        0     4691 2023-05-07 15:15:00.601862 tpcollections-0.1.0/test/test_expiring_ordered_mapping.py
--rw-r--r--   0        0        0     6532 2023-05-07 14:31:53.066104 tpcollections-0.1.0/test/test_mapping.py
--rw-r--r--   0        0        0     8099 2023-05-07 15:16:24.278863 tpcollections-0.1.0/test/test_ordered_mapping.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 tpcollections-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-05-05 19:11:26.352439 tpcollections-0.1.1/.gitignore
+-rw-r--r--   0        0        0    12288 2023-05-07 14:21:45.975212 tpcollections-0.1.1/:memory
+-rw-r--r--   0        0        0      147 2023-05-05 19:11:26.352439 tpcollections-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-05 19:11:26.352439 tpcollections-0.1.1/LICENSE
+-rw-r--r--   0        0        0    11401 2023-05-05 19:11:26.352439 tpcollections-0.1.1/LICENSE.apache
+-rw-r--r--   0        0        0      188 2023-05-05 19:11:26.352439 tpcollections-0.1.1/LICENSE.rst
+-rw-r--r--   0        0        0       52 2023-05-05 19:11:26.352439 tpcollections-0.1.1/Makefile
+-rw-r--r--   0        0        0     2687 2023-05-06 17:00:37.665189 tpcollections-0.1.1/README.md
+-rwxr-xr-x   0        0        0     2233 2023-05-06 17:07:10.369109 tpcollections-0.1.1/justfile
+-rw-r--r--   0        0        0     1102 2023-05-07 15:19:34.716692 tpcollections-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      347 2023-05-07 15:10:44.113643 tpcollections-0.1.1/src/tpcollections/__init__.py
+-rw-r--r--   0        0        0    12061 2023-05-06 17:50:29.975701 tpcollections-0.1.1/src/tpcollections/_db.py
+-rw-r--r--   0        0        0    21739 2023-05-07 15:19:19.094132 tpcollections-0.1.1/src/tpcollections/_mapping.py
+-rw-r--r--   0        0        0      960 2023-05-07 15:13:03.680664 tpcollections-0.1.1/src/tpcollections/_serializers.py
+-rw-r--r--   0        0        0     1623 2023-05-07 15:10:44.109643 tpcollections-0.1.1/src/tpcollections/_util.py
+-rw-r--r--   0        0        0        0 2023-05-05 19:11:26.353439 tpcollections-0.1.1/src/tpcollections/py.typed
+-rw-r--r--   0        0        0        0 2023-05-06 02:32:11.037046 tpcollections-0.1.1/test/__init__.py
+-rw-r--r--   0        0        0     2646 2023-05-07 15:10:44.108643 tpcollections-0.1.1/test/test_expiring_mapping.py
+-rw-r--r--   0        0        0     4691 2023-05-07 15:15:00.601862 tpcollections-0.1.1/test/test_expiring_ordered_mapping.py
+-rw-r--r--   0        0        0     6532 2023-05-07 14:31:53.066104 tpcollections-0.1.1/test/test_mapping.py
+-rw-r--r--   0        0        0     8099 2023-05-07 15:16:24.278863 tpcollections-0.1.1/test/test_ordered_mapping.py
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 tpcollections-0.1.1/PKG-INFO
```

### Comparing `tpcollections-0.1.0/.gitignore` & `tpcollections-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/:memory` & `tpcollections-0.1.1/:memory`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/LICENSE` & `tpcollections-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/LICENSE.apache` & `tpcollections-0.1.1/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/README.md` & `tpcollections-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/justfile` & `tpcollections-0.1.1/justfile`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/pyproject.toml` & `tpcollections-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'tpcollections'
 description = 'Persistent transactional Python collections'
-version = '0.1.0'
+version = '0.1.1'
 readme = 'README.md'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

### Comparing `tpcollections-0.1.0/src/tpcollections/_db.py` & `tpcollections-0.1.1/src/tpcollections/_db.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/src/tpcollections/_mapping.py` & `tpcollections-0.1.1/src/tpcollections/_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import (
     Any,
     Callable,
     ItemsView,
     Iterable,
     Iterator,
     KeysView,
+    Optional,
     Reversible,
     Tuple,
     TypeVar,
     ValuesView,
     MutableMapping,
     cast,
 )
@@ -70,15 +71,15 @@
         self._serializer = serializer
         self._order = order
     
     def _iterator(self, order: str) -> Iterator[Key]:
         with self._connection.cursor() as cursor:
             for key, in cursor.execute(f'''
                 SELECT key FROM {self._database}.{self._table}
-                    ORDER BY {self._order} {order}',
+                    ORDER BY {self._order} {order}
             '''):
                 yield self._serializer.loads(key)
 
 class Values(_ViewsBase[Any], ValuesView[Value]):
     __slots__ = (
         '_connection',
         '_database',
@@ -470,15 +471,15 @@
 
     @lifespan.setter
     def lifespan(self, value: timedelta) -> None:
         lifespan = int(value.total_seconds())
         assert lifespan > 0
         self._lifespan = lifespan
 
-    def now_function(self, function: Callable[[], int] | None) -> None:
+    def now_function(self, function: Optional[Callable[[], int]]) -> None:
         function_name = self._database + "." + self._table + '_now'
         self._connection.connection.create_function(
             function_name.value,
             0,
             function,
         )
```

### Comparing `tpcollections-0.1.0/src/tpcollections/_serializers.py` & `tpcollections-0.1.1/src/tpcollections/_serializers.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/src/tpcollections/_util.py` & `tpcollections-0.1.1/src/tpcollections/_util.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/test/test_expiring_mapping.py` & `tpcollections-0.1.1/test/test_expiring_mapping.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/test/test_expiring_ordered_mapping.py` & `tpcollections-0.1.1/test/test_expiring_ordered_mapping.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/test/test_mapping.py` & `tpcollections-0.1.1/test/test_mapping.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/test/test_ordered_mapping.py` & `tpcollections-0.1.1/test/test_ordered_mapping.py`

 * *Files identical despite different names*

### Comparing `tpcollections-0.1.0/PKG-INFO` & `tpcollections-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpcollections
-Version: 0.1.0
+Version: 0.1.1
 Summary: Persistent transactional Python collections
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

