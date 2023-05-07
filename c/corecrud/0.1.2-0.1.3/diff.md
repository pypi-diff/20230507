# Comparing `tmp/corecrud-0.1.2.tar.gz` & `tmp/corecrud-0.1.3.tar.gz`

## Comparing `corecrud-0.1.2.tar` & `corecrud-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 corecrud-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 corecrud-0.1.2/Makefile
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/crud.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 corecrud-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/__init__.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/arguments.py
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/operations.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/typing.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/cursors/__init__.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/cursors/abc.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/cursors/mapping.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 corecrud-0.1.2/corecrud/cursors/scalars.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 corecrud-0.1.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 corecrud-0.1.2/LICENSE
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 corecrud-0.1.2/README.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 corecrud-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 corecrud-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 corecrud-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 corecrud-0.1.3/Makefile
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 corecrud-0.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 corecrud-0.1.3/.idea/crud.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 corecrud-0.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 corecrud-0.1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 corecrud-0.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 corecrud-0.1.3/.idea/workspace.xml
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 corecrud-0.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 corecrud-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 corecrud-0.1.3/corecrud/__init__.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 corecrud-0.1.3/corecrud/arguments.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 corecrud-0.1.3/corecrud/operations.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 corecrud-0.1.3/corecrud/typing.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 corecrud-0.1.3/corecrud/cursors/__init__.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 corecrud-0.1.3/corecrud/cursors/abc.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 corecrud-0.1.3/corecrud/cursors/mapping.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 corecrud-0.1.3/corecrud/cursors/scalars.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 corecrud-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 corecrud-0.1.3/LICENSE
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 corecrud-0.1.3/README.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 corecrud-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 corecrud-0.1.3/PKG-INFO
```

### Comparing `corecrud-0.1.2/.pre-commit-config.yaml` & `corecrud-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.2/Makefile` & `corecrud-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.2/.idea/workspace.xml` & `corecrud-0.1.3/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `corecrud-0.1.2/.idea/workspace.xml` & `corecrud-0.1.3/.idea/workspace.xml`

```diff
@@ -25,29 +25,29 @@
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2PBpJ6j5cGfREELAPVYcExLoEca"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "WebServerToolWindowFactoryState": "false",
-    "git-widget-placeholder": "master",
-    "last_opened_file_path": "/home/copper_boy/Documents/core/crud",
-    "node.js.detected.package.eslint": "true",
-    "node.js.detected.package.tslint": "true",
-    "node.js.selected.package.eslint": "(autodetect)",
-    "node.js.selected.package.tslint": "(autodetect)",
-    "nodejs_package_manager_path": "npm",
-    "vue.rearranger.settings.migration": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;master&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/home/copper_boy/Documents/core/crud&quot;,
+    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
+    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
+    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
+    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$"/>
     </key>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
@@ -61,14 +61,15 @@
       <workItem from="1682940417201" duration="16000"/>
       <workItem from="1683310291585" duration="132000"/>
       <workItem from="1683311080325" duration="687000"/>
       <workItem from="1683370113934" duration="1128000"/>
       <workItem from="1683399575532" duration="854000"/>
       <workItem from="1683456478263" duration="9397000"/>
       <workItem from="1683466276827" duration="885000"/>
+      <workItem from="1683467976471" duration="348000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `corecrud-0.1.2/.idea/inspectionProfiles/Project_Default.xml` & `corecrud-0.1.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.2/corecrud/__init__.py` & `corecrud-0.1.3/corecrud/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     SelectExecutor,
     SelectQuery,
     Update,
     UpdateExecutor,
     UpdateQuery,
 )
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __all__ = (
     "ABCCursor",
     "Argument",
     "Correlate",
     "CRUD",
     "CRUDOperation",
     "Delete",
```

### Comparing `corecrud-0.1.2/corecrud/arguments.py` & `corecrud-0.1.3/corecrud/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return query
 
 
 class Main:
     def __init__(self, method: Any, *args: Any, **kwargs: Any) -> None:
         self.method = method
 
-        self.args = args
+        self.args = filter(None, args)
         self.kwargs = kwargs
 
     def main(self) -> Any:
         return self.method(*self.args, **self.kwargs)
 
 
 class Select(Main):
```

### Comparing `corecrud-0.1.2/corecrud/operations.py` & `corecrud-0.1.3/corecrud/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,11 +299,13 @@
         *,
         cursor_cls: Type[ABCCursor] = Scalars,
         select: Type[Select[ModelT]] = Select,
         insert: Type[Insert[ModelT]] = Insert,
         update: Type[Update[ModelT]] = Update,
         delete: Type[Delete[ModelT]] = Delete,
     ) -> None:
+        self.model = model
+
         self.select = select(model=model, cursor_cls=cursor_cls)
         self.insert = insert(model=model, cursor_cls=cursor_cls)
         self.update = update(model=model, cursor_cls=cursor_cls)
         self.delete = delete(model=model, cursor_cls=cursor_cls)
```

### Comparing `corecrud-0.1.2/.gitignore` & `corecrud-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.2/LICENSE` & `corecrud-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.2/pyproject.toml` & `corecrud-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `corecrud-0.1.2/PKG-INFO` & `corecrud-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corecrud
-Version: 0.1.2
+Version: 0.1.3
 Summary: The CRUD package for management your models
 Project-URL: Homepage, https://github.com/toymaj/corecrud/
 Project-URL: Documentation, https://github.com/toymaj/corecrud/
 Project-URL: Repository, https://github.com/toymaj/corecrud/
 Author-email: toymaj <sermed512@gmail.com>
 Maintainer-email: toymaj <sermed512@gmail.com>
 License-Expression: MIT
```

