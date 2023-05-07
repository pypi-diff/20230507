# Comparing `tmp/corecrud-0.1.tar.gz` & `tmp/corecrud-0.1.1.tar.gz`

## Comparing `corecrud-0.1.tar` & `corecrud-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 corecrud-0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 corecrud-0.1/Makefile
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 corecrud-0.1/.idea/.gitignore
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 corecrud-0.1/.idea/crud.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 corecrud-0.1/.idea/misc.xml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 corecrud-0.1/.idea/modules.xml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 corecrud-0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 corecrud-0.1/.idea/workspace.xml
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 corecrud-0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 corecrud-0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 corecrud-0.1/corecrud/__init__.py
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 corecrud-0.1/corecrud/arguments.py
--rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 corecrud-0.1/corecrud/operations.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 corecrud-0.1/corecrud/typing.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 corecrud-0.1/corecrud/cursors/__init__.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 corecrud-0.1/corecrud/cursors/abc.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 corecrud-0.1/corecrud/cursors/mapping.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 corecrud-0.1/corecrud/cursors/scalars.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 corecrud-0.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 corecrud-0.1/LICENSE
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 corecrud-0.1/README.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 corecrud-0.1/pyproject.toml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 corecrud-0.1/PKG-INFO
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 corecrud-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 corecrud-0.1.1/Makefile
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/crud.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 corecrud-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/__init__.py
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/arguments.py
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/operations.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/typing.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/cursors/__init__.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/cursors/abc.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/cursors/mapping.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 corecrud-0.1.1/corecrud/cursors/scalars.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 corecrud-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 corecrud-0.1.1/LICENSE
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 corecrud-0.1.1/README.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 corecrud-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 corecrud-0.1.1/PKG-INFO
```

### Comparing `corecrud-0.1/.pre-commit-config.yaml` & `corecrud-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1/Makefile` & `corecrud-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `corecrud-0.1/.idea/workspace.xml` & `corecrud-0.1.1/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `corecrud-0.1/.idea/workspace.xml` & `corecrud-0.1.1/.idea/workspace.xml`

```diff
@@ -1,24 +1,27 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="91974e16-63f1-48f0-9796-891e9abba41d" name="Changes" comment=""/>
+    <list default="true" id="91974e16-63f1-48f0-9796-891e9abba41d" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/Makefile" beforeDir="false" afterPath="$PROJECT_DIR$/Makefile" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/corecrud/operations.py" beforeDir="false" afterPath="$PROJECT_DIR$/corecrud/operations.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
-        <option value="Python Script"/>
         <option value="MIT"/>
+        <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
@@ -40,29 +43,35 @@
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
+  <component name="RecentsManager">
+    <key name="CopyFile.RECENT_KEYS">
+      <recent name="$PROJECT_DIR$"/>
+    </key>
+  </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="91974e16-63f1-48f0-9796-891e9abba41d" name="Changes" comment=""/>
       <created>1682940253712</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1682940253712</updated>
       <workItem from="1682940255138" duration="146000"/>
       <workItem from="1682940417201" duration="16000"/>
       <workItem from="1683310291585" duration="132000"/>
       <workItem from="1683311080325" duration="687000"/>
       <workItem from="1683370113934" duration="1128000"/>
       <workItem from="1683399575532" duration="854000"/>
-      <workItem from="1683456478263" duration="9317000"/>
+      <workItem from="1683456478263" duration="9397000"/>
+      <workItem from="1683466276827" duration="811000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `corecrud-0.1/.idea/inspectionProfiles/Project_Default.xml` & `corecrud-0.1.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1/corecrud/__init__.py` & `corecrud-0.1.1/corecrud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     SelectExecutor,
     SelectQuery,
     Update,
     UpdateExecutor,
     UpdateQuery,
 )
 
-__version__ = "0.1"
+__version__ = "0.1.1"
 __all__ = (
     "ABCCursor",
     "Argument",
     "Correlate",
     "CRUD",
     "CRUDOperation",
     "Delete",
```

### Comparing `corecrud-0.1/corecrud/arguments.py` & `corecrud-0.1.1/corecrud/arguments.py`

 * *Files identical despite different names*

### Comparing `corecrud-0.1/corecrud/operations.py` & `corecrud-0.1.1/corecrud/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,32 +59,34 @@
         cursor = self.cursor_cls(await self.executor.execute(*args, **kwargs))
         return await cursor.many_unique()
 
 
 class SelectQuery(_ABCQuery[ModelT]):
     def build(
         self,
-        nested_select: Optional[Sequence[Any]] = None,
         *arguments: Argument,
+        nested_select: Optional[Sequence[Any]] = None,
     ) -> Any:
-        collector = Collector(SelectMain(self.model))
+        nested_select = [] if not nested_select else nested_select
+
+        collector = Collector(SelectMain(self.model, *nested_select))
         return collector.build(*arguments)
 
 
 class SelectExecutor(_Executor[ModelT], Generic[ModelT]):
     def __init__(self, model: Type[ModelT]) -> None:
         super(SelectExecutor, self).__init__(query=SelectQuery(model=model))
 
     async def execute(
         self,
+        *arguments: Argument,
         session: AsyncSession,
         nested_select: Optional[Sequence[Any]] = None,
-        *arguments: Argument,
     ) -> AsyncResult[Any]:
-        return await session.stream(self.query.build(nested_select=nested_select, *arguments))
+        return await session.stream(self.query.build(*arguments, nested_select=nested_select))
 
 
 class Select(CRUDOperation[ModelT]):
     def __init__(
         self,
         model: Type[ModelT],
         *,
@@ -93,60 +95,64 @@
         super(Select, self).__init__(
             cursor_cls=cursor_cls,
             executor=SelectExecutor(model=model),
         )
 
     async def one(
         self,
+        *arguments: Argument,
         session: AsyncSession,
         nested_select: Optional[Sequence[Any]] = None,
-        *arguments: Argument,
     ) -> Optional[ModelT]:
-        return await super(Select, self).one(session, nested_select=nested_select, *arguments)
+        return await super(Select, self).one(
+            *arguments, session=session, nested_select=nested_select
+        )
 
     async def many(
         self,
+        *arguments: Argument,
         session: AsyncSession,
         nested_select: Optional[Sequence[Any]] = None,
-        *arguments: Argument,
     ) -> Sequence[ModelT]:
-        return await super(Select, self).many(session, nested_select=nested_select, *arguments)
+        return await super(Select, self).many(
+            *arguments, session=session, nested_select=nested_select
+        )
 
     async def many_unique(
         self,
+        *arguments: Argument,
         session: AsyncSession,
         nested_select: Optional[Sequence[Any]] = None,
-        *arguments: Argument,
     ) -> Sequence[ModelT]:
         return await super(Select, self).many_unique(
-            session, nested_select=nested_select, *arguments
+            *arguments, session=session, nested_select=nested_select
         )
 
 
 class InsertQuery(_ABCQuery[ModelT]):
     def build(
         self,
-        dialect: Any = insert,
         *arguments: Argument,
+        dialect: Any = insert,
     ) -> Any:
         collector = Collector(InsertMain(self.model, dialect=dialect))
         return collector.build(*arguments)
 
 
 class InsertExecutor(_Executor[ModelT], Generic[ModelT]):
     def __init__(self, model: Type[ModelT]) -> None:
         super(InsertExecutor, self).__init__(query=InsertQuery(model=model))
 
     async def execute(
         self,
+        *arguments: Argument,
         session: AsyncSession,
         dialect: Any = insert,
-        *arguments: Argument,
     ) -> AsyncResult[Any]:
-        return await session.stream(self.query.build(dialect=dialect, *arguments))
+        return await session.stream(self.query.build(*arguments, dialect=dialect))
 
 
 class Insert(CRUDOperation[ModelT]):
     def __init__(
         self,
         model: Type[ModelT],
         *,
@@ -155,54 +161,51 @@
         super(Insert, self).__init__(
             cursor_cls=cursor_cls,
             executor=InsertExecutor(model=model),
         )
 
     async def one(
         self,
+        *arguments: Argument,
         session: AsyncSession,
         dialect: Any = insert,
-        *arguments: Argument,
     ) -> Optional[ModelT]:
-        return await super(Insert, self).one(session, dialect=dialect, *arguments)
+        return await super(Insert, self).one(*arguments, session=session, dialect=dialect)
 
     async def many(
         self,
+        *arguments: Argument,
         session: AsyncSession,
         dialect: Any = insert,
-        *arguments: Argument,
     ) -> Sequence[ModelT]:
-        return await super(Insert, self).many(session, dialect=dialect, *arguments)
+        return await super(Insert, self).many(*arguments, session=session, dialect=dialect)
 
     async def many_unique(
         self,
+        *arguments: Argument,
         session: AsyncSession,
         dialect: Any = insert,
-        *arguments: Argument,
     ) -> Sequence[ModelT]:
-        return await super(Insert, self).many_unique(session, dialect=dialect, *arguments)
+        return await super(Insert, self).many_unique(*arguments, session=session, dialect=dialect)
 
 
 class UpdateQuery(_ABCQuery[ModelT]):
-    def build(
-        self,
-        *arguments: Argument,
-    ) -> Any:
+    def build(self, *arguments: Argument) -> Any:
         collector = Collector(UpdateMain(self.model))
         return collector.build(*arguments)
 
 
 class UpdateExecutor(_Executor[ModelT], Generic[ModelT]):
     def __init__(self, model: Type[ModelT]) -> None:
         super(UpdateExecutor, self).__init__(query=UpdateQuery(model=model))
 
     async def execute(
         self,
-        session: AsyncSession,
         *arguments: Argument,
+        session: AsyncSession,
     ) -> AsyncResult[Any]:
         return await session.stream(self.query.build(*arguments))
 
 
 class Update(CRUDOperation[ModelT]):
     def __init__(
         self,
@@ -213,48 +216,48 @@
         super(Update, self).__init__(
             cursor_cls=cursor_cls,
             executor=UpdateExecutor(model=model),
         )
 
     async def one(
         self,
-        session: AsyncSession,
         *arguments: Argument,
+        session: AsyncSession,
     ) -> Optional[ModelT]:
-        return await super(Update, self).one(session, *arguments)
+        return await super(Update, self).one(*arguments, session=session)
 
     async def many(
         self,
-        session: AsyncSession,
         *arguments: Argument,
+        session: AsyncSession,
     ) -> Sequence[ModelT]:
-        return await super(Update, self).many(session, *arguments)
+        return await super(Update, self).many(*arguments, session=session)
 
     async def many_unique(
         self,
-        session: AsyncSession,
         *arguments: Argument,
+        session: AsyncSession,
     ) -> Sequence[ModelT]:
-        return await super(Update, self).many_unique(session, *arguments)
+        return await super(Update, self).many_unique(*arguments, session=session)
 
 
 class DeleteQuery(_ABCQuery[ModelT]):
     def build(self, *arguments: Argument) -> Any:
         collector = Collector(DeleteMain(self.model))
         return collector.build(*arguments)
 
 
 class DeleteExecutor(_Executor[ModelT], Generic[ModelT]):
     def __init__(self, model: Type[ModelT]) -> None:
         super(DeleteExecutor, self).__init__(query=DeleteQuery(model=model))
 
     async def execute(
         self,
-        session: AsyncSession,
         *arguments: Argument,
+        session: AsyncSession,
     ) -> AsyncResult[Any]:
         return await session.stream(self.query.build(*arguments))
 
 
 class Delete(CRUDOperation[ModelT]):
     def __init__(
         self,
@@ -265,32 +268,32 @@
         super(Delete, self).__init__(
             cursor_cls=cursor_cls,
             executor=DeleteExecutor(model=model),
         )
 
     async def one(
         self,
-        session: AsyncSession,
         *arguments: Argument,
+        session: AsyncSession,
     ) -> Optional[ModelT]:
-        return await super(Delete, self).one(session, *arguments)
+        return await super(Delete, self).one(*arguments, session=session)
 
     async def many(
         self,
-        session: AsyncSession,
         *arguments: Argument,
+        session: AsyncSession,
     ) -> Sequence[ModelT]:
-        return await super(Delete, self).many(session, *arguments)
+        return await super(Delete, self).many(*arguments, session=session)
 
     async def many_unique(
         self,
-        session: AsyncSession,
         *arguments: Argument,
+        session: AsyncSession,
     ) -> Sequence[ModelT]:
-        return await super(Delete, self).many_unique(session, *arguments)
+        return await super(Delete, self).many_unique(*arguments, session=session)
 
 
 class CRUD(Generic[ModelT]):
     def __init__(
         self,
         model: Type[ModelT],
         *,
```

### Comparing `corecrud-0.1/.gitignore` & `corecrud-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `corecrud-0.1/LICENSE` & `corecrud-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corecrud-0.1/pyproject.toml` & `corecrud-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1/PKG-INFO` & `corecrud-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corecrud
-Version: 0.1
+Version: 0.1.1
 Summary: The CRUD package for management your models
 Project-URL: Homepage, https://github.com/toymaj/corecrud/
 Project-URL: Documentation, https://github.com/toymaj/corecrud/
 Project-URL: Repository, https://github.com/toymaj/corecrud/
 Author-email: toymaj <sermed512@gmail.com>
 Maintainer-email: toymaj <sermed512@gmail.com>
 License-Expression: MIT
```

