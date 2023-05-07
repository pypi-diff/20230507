# Comparing `tmp/corecrud-0.1.1.tar.gz` & `tmp/corecrud-0.1.2.tar.gz`

## Comparing `corecrud-0.1.1.tar` & `corecrud-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 corecrud-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 corecrud-0.1.1/Makefile
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/crud.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/__init__.py
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/arguments.py
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/operations.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/typing.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/cursors/__init__.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/cursors/abc.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/cursors/mapping.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/cursors/scalars.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 corecrud-0.1.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 corecrud-0.1.1/LICENSE
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 corecrud-0.1.1/README.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 corecrud-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 corecrud-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 corecrud-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 corecrud-0.1.2/Makefile
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/crud.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/__init__.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/arguments.py
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/operations.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/typing.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/cursors/__init__.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/cursors/abc.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/cursors/mapping.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/cursors/scalars.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 corecrud-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 corecrud-0.1.2/LICENSE
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 corecrud-0.1.2/README.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 corecrud-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 corecrud-0.1.2/PKG-INFO
```

### Comparing `corecrud-0.1.1/.pre-commit-config.yaml` & `corecrud-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.1/Makefile` & `corecrud-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.1/.idea/workspace.xml` & `corecrud-0.1.2/.idea/workspace.xml`

 * *Files 7% similar despite different names*

#### Comparing `corecrud-0.1.1/.idea/workspace.xml` & `corecrud-0.1.2/.idea/workspace.xml`

```diff
@@ -1,17 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="91974e16-63f1-48f0-9796-891e9abba41d" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/Makefile" beforeDir="false" afterPath="$PROJECT_DIR$/Makefile" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/corecrud/operations.py" beforeDir="false" afterPath="$PROJECT_DIR$/corecrud/operations.py" afterDir="false"/>
-    </list>
+    <list default="true" id="91974e16-63f1-48f0-9796-891e9abba41d" name="Changes" comment=""/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -63,15 +60,15 @@
       <workItem from="1682940255138" duration="146000"/>
       <workItem from="1682940417201" duration="16000"/>
       <workItem from="1683310291585" duration="132000"/>
       <workItem from="1683311080325" duration="687000"/>
       <workItem from="1683370113934" duration="1128000"/>
       <workItem from="1683399575532" duration="854000"/>
       <workItem from="1683456478263" duration="9397000"/>
-      <workItem from="1683466276827" duration="811000"/>
+      <workItem from="1683466276827" duration="885000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `corecrud-0.1.1/.idea/inspectionProfiles/Project_Default.xml` & `corecrud-0.1.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.1/corecrud/__init__.py` & `corecrud-0.1.2/corecrud/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     SelectExecutor,
     SelectQuery,
     Update,
     UpdateExecutor,
     UpdateQuery,
 )
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __all__ = (
     "ABCCursor",
     "Argument",
     "Correlate",
     "CRUD",
     "CRUDOperation",
     "Delete",
```

### Comparing `corecrud-0.1.1/corecrud/arguments.py` & `corecrud-0.1.2/corecrud/arguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Optional, Sequence
+from typing import Any, Callable, Optional
 
-from corecrud.typing import DictStrAny
+from corecrud.typing import DictStrAny, TupleAny
 from sqlalchemy import delete, insert, select, update
 from sqlalchemy.sql.base import ExecutableOption, _NoArg  # noqa: W0212
 from sqlalchemy.sql.dml import Insert as StandardInsert
 
 
-def _build(main: Any, method: str, args: Sequence[Any], kwargs: DictStrAny) -> Any:
+def _build(main: Any, method: str, args: TupleAny, kwargs: DictStrAny) -> Any:
     return getattr(main, method)(*args, **kwargs)
 
 
 class Collector:
     def __init__(self, query: Main) -> None:
         self.query = query
 
@@ -25,15 +25,15 @@
         return query
 
 
 class Main:
     def __init__(self, method: Any, *args: Any, **kwargs: Any) -> None:
         self.method = method
 
-        self.args = filter(None, args)  # type: ignore[var-annotated]
+        self.args = args
         self.kwargs = kwargs
 
     def main(self) -> Any:
         return self.method(*self.args, **self.kwargs)
 
 
 class Select(Main):
@@ -68,15 +68,15 @@
         """
         Object that helps to create arguments.
 
         :param args: arguments in method.
         :param kwargs: kwargs in method.
         """
 
-        self.args = filter(None, args)  # type: ignore[var-annotated]
+        self.args = args
         self.kwargs = kwargs
 
     def query(self, main: Any) -> Any:
         return _build(main, self.method, self.args, self.kwargs)  # type: ignore[arg-type]
 
 
 class Where(Argument):
```

### Comparing `corecrud-0.1.1/corecrud/operations.py` & `corecrud-0.1.2/corecrud/operations.py`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.1/.gitignore` & `corecrud-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.1/LICENSE` & `corecrud-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.1/pyproject.toml` & `corecrud-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.1/PKG-INFO` & `corecrud-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corecrud
-Version: 0.1.1
+Version: 0.1.2
 Summary: The CRUD package for management your models
 Project-URL: Homepage, https://github.com/toymaj/corecrud/
 Project-URL: Documentation, https://github.com/toymaj/corecrud/
 Project-URL: Repository, https://github.com/toymaj/corecrud/
 Author-email: toymaj <sermed512@gmail.com>
 Maintainer-email: toymaj <sermed512@gmail.com>
 License-Expression: MIT
```

