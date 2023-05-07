# Comparing `tmp/corecrud-0.1.4.1.tar.gz` & `tmp/corecrud-0.1.4.2.tar.gz`

## Comparing `corecrud-0.1.4.1.tar` & `corecrud-0.1.4.2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/Makefile
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.idea/.gitignore
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.idea/crud.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.idea/misc.xml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.idea/modules.xml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.idea/vcs.xml
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.idea/workspace.xml
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/corecrud/__init__.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/corecrud/arguments.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/corecrud/operations.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/corecrud/typing.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/corecrud/cursors/__init__.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/corecrud/cursors/abc.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/corecrud/cursors/mapping.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/corecrud/cursors/scalars.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/LICENSE
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/README.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/pyproject.toml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 corecrud-0.1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/Makefile
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.idea/.gitignore
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.idea/crud.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.idea/misc.xml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.idea/modules.xml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/__init__.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/arguments.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/collector.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/main.py
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/operations.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/typing.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/utils.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/cursors/__init__.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/cursors/abc.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/cursors/mapping.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/corecrud/cursors/scalars.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/LICENSE
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/README.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 corecrud-0.1.4.2/PKG-INFO
```

### Comparing `corecrud-0.1.4.1/.pre-commit-config.yaml` & `corecrud-0.1.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.4.1/Makefile` & `corecrud-0.1.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.4.1/.idea/workspace.xml` & `corecrud-0.1.4.2/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `corecrud-0.1.4.1/.idea/workspace.xml` & `corecrud-0.1.4.2/.idea/workspace.xml`

```diff
@@ -63,14 +63,15 @@
       <workItem from="1683311080325" duration="687000"/>
       <workItem from="1683370113934" duration="1128000"/>
       <workItem from="1683399575532" duration="854000"/>
       <workItem from="1683456478263" duration="9397000"/>
       <workItem from="1683466276827" duration="885000"/>
       <workItem from="1683467976471" duration="348000"/>
       <workItem from="1683472759002" duration="646000"/>
+      <workItem from="1683473510631" duration="497000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `corecrud-0.1.4.1/.idea/inspectionProfiles/Project_Default.xml` & `corecrud-0.1.4.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.4.1/corecrud/__init__.py` & `corecrud-0.1.4.2/corecrud/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from corecrud.arguments import Argument, Correlate
-from corecrud.arguments import Delete as DeleteMain
-from corecrud.arguments import Filter, GroupBy, Having
-from corecrud.arguments import Insert as InsertMain
-from corecrud.arguments import (
+from .arguments import (
+    Argument,
+    Correlate,
+    Filter,
+    GroupBy,
+    Having,
     Join,
     Limit,
-    Main,
     Offset,
     Options,
     OrderBy,
     OuterJoin,
     Returning,
+    SelectFrom,
+    Values,
+    Where,
 )
-from corecrud.arguments import Select as SelectMain
-from corecrud.arguments import SelectFrom
-from corecrud.arguments import Update as UpdateMain
-from corecrud.arguments import Values, Where
-from corecrud.cursors import ABCCursor, Mappings, Scalars
-from corecrud.operations import (
+from .cursors import ABCCursor, Mappings, Scalars
+from .main import Delete as DeleteMain
+from .main import Insert as InsertMain
+from .main import Main
+from .main import Select as SelectMain
+from .main import Update as UpdateMain
+from .operations import (
     CRUD,
     CRUDOperation,
     Delete,
     DeleteExecutor,
     DeleteQuery,
     Insert,
     InsertExecutor,
@@ -30,15 +34,15 @@
     SelectExecutor,
     SelectQuery,
     Update,
     UpdateExecutor,
     UpdateQuery,
 )
 
-__version__ = "0.1.4.1"
+__version__ = "0.1.4.2"
 __all__ = (
     "ABCCursor",
     "Argument",
     "Correlate",
     "CRUD",
     "CRUDOperation",
     "Delete",
```

### Comparing `corecrud-0.1.4.1/corecrud/arguments.py` & `corecrud-0.1.4.2/corecrud/arguments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,13 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Optional
+from typing import Any, Optional
 
-from corecrud.typing import DictStrAny, TupleAny
-from sqlalchemy import delete, insert, select, update
-from sqlalchemy.sql.base import ExecutableOption, _NoArg  # noqa: W0212
-from sqlalchemy.sql.dml import Insert as StandardInsert
-
-
-def _build(main: Any, method: str, args: TupleAny, kwargs: DictStrAny) -> Any:
-    return getattr(main, method)(*args, **kwargs)
-
-
-class Collector:
-    def __init__(self, query: Main) -> None:
-        self.query = query
-
-    def build(self, *arguments: Any) -> Any:
-        query = self.query.main()
-
-        for argument in arguments:
-            query = argument.query(query)
-
-        return query
-
-
-class Main:
-    def __init__(self, method: Any, *args: Any, **kwargs: Any) -> None:
-        self.method = method
-
-        self.args = (i for i in args if i is not None)
-        self.kwargs = kwargs
-
-    def main(self) -> Any:
-        return self.method(*self.args, **self.kwargs)
-
-
-class Select(Main):
-    def __init__(self, *entities: Any) -> None:
-        super(Select, self).__init__(select, *entities)
-
-
-class Insert(Main):
-    def __init__(
-        self,
-        table: Any,
-        *,
-        dialect: Callable[..., StandardInsert] = insert,
-    ) -> None:
-        super(Insert, self).__init__(dialect, table)
-
-
-class Update(Main):
-    def __init__(self, table: Any) -> None:
-        super(Update, self).__init__(update, table)
-
-
-class Delete(Main):
-    def __init__(self, table: Any) -> None:
-        super(Delete, self).__init__(delete, table)
+from corecrud.utils import call_next
+from sqlalchemy.sql.base import ExecutableOption
 
 
 class Argument:
     method: str
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """
@@ -72,15 +17,15 @@
         :param kwargs: kwargs in method.
         """
 
         self.args = args
         self.kwargs = kwargs
 
     def query(self, main: Any) -> Any:
-        return _build(main, self.method, self.args, self.kwargs)  # type: ignore[arg-type]
+        return call_next(main, self.method, self.args, self.kwargs)  # type: ignore[arg-type]
 
 
 class Where(Argument):
     method = "where"
 
     def __init__(self, *whereclause: Any) -> None:
         super(Where, self).__init__(*whereclause)
@@ -150,26 +95,26 @@
 
 
 class OrderBy(Argument):
     method = "order_by"
 
     def __init__(
         self,
-        __first: Any = _NoArg.NO_ARG,
+        __first: Any = 0,
         *clauses: Any,
     ) -> None:
         super(OrderBy, self).__init__(__first, *clauses)
 
 
 class GroupBy(Argument):
     method = "group_by"
 
     def __init__(
         self,
-        __first: Any = _NoArg.NO_ARG,
+        __first: Any = 0,
         *clauses: Any,
     ) -> None:
         super(GroupBy, self).__init__(__first, *clauses)
 
 
 class Having(Argument):
     method = "having"
```

### Comparing `corecrud-0.1.4.1/corecrud/operations.py` & `corecrud-0.1.4.2/corecrud/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import abc
 from typing import TYPE_CHECKING, Any, Generic, Optional, Sequence, Type, TypeVar
 
-from corecrud.arguments import Collector
-from corecrud.arguments import Delete as DeleteMain
-from corecrud.arguments import Insert as InsertMain
-from corecrud.arguments import Select as SelectMain
-from corecrud.arguments import Update as UpdateMain
+from corecrud.collector import Collector
 from corecrud.cursors import Scalars
 from corecrud.cursors.abc import ABCCursor
+from corecrud.main import Delete as DeleteMain
+from corecrud.main import Insert as InsertMain
+from corecrud.main import Select as SelectMain
+from corecrud.main import Update as UpdateMain
 from sqlalchemy import insert
 from sqlalchemy.ext.asyncio import AsyncResult, AsyncSession
 
 ModelT = TypeVar("ModelT")
 
 if TYPE_CHECKING:
     from corecrud.arguments import Argument
@@ -62,17 +62,17 @@
 
 class SelectQuery(_ABCQuery[ModelT]):
     def build(
         self,
         *arguments: Argument,
         nested_select: Optional[Sequence[Any]] = None,
     ) -> Any:
-        nested_select = [] if not nested_select else nested_select
-
-        collector = Collector(SelectMain(self.model, *nested_select))
+        collector = Collector(
+            SelectMain(self.model, *([] if not nested_select else nested_select))
+        )
         return collector.build(*arguments)
 
 
 class SelectExecutor(_Executor[ModelT], Generic[ModelT]):
     def __init__(self, model: Type[ModelT]) -> None:
         super(SelectExecutor, self).__init__(query=SelectQuery(model=model))
```

### Comparing `corecrud-0.1.4.1/.gitignore` & `corecrud-0.1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.4.1/LICENSE` & `corecrud-0.1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.4.1/pyproject.toml` & `corecrud-0.1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.4.1/PKG-INFO` & `corecrud-0.1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corecrud
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: The CRUD package for management your models
 Project-URL: Homepage, https://github.com/toymaj/corecrud/
 Project-URL: Documentation, https://github.com/toymaj/corecrud/
 Project-URL: Repository, https://github.com/toymaj/corecrud/
 Author-email: toymaj <sermed512@gmail.com>
 Maintainer-email: toymaj <sermed512@gmail.com>
 License-Expression: MIT
```

