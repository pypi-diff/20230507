# Comparing `tmp/reactpy_django-3.0.1.tar.gz` & `tmp/reactpy_django-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_django-3.0.1.tar", last modified: Fri Apr  7 03:45:33 2023, max compression
+gzip compressed data, was "reactpy_django-3.1.0.tar", last modified: Sun May  7 04:47:31 2023, max compression
```

## Comparing `reactpy_django-3.0.1.tar` & `reactpy_django-3.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.936506 reactpy_django-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.936506 reactpy_django-3.0.1/src/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/src/reactpy_django/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/http/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/http/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/src/reactpy_django/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.936506 reactpy_django-3.0.1/src/reactpy_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/src/reactpy_django/static/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-04-07 03:45:33.000000 reactpy_django-3.0.1/src/reactpy_django/static/reactpy_django/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.936506 reactpy_django-3.0.1/src/reactpy_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/src/reactpy_django/templates/reactpy/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/templates/reactpy/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/src/reactpy_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/templatetags/reactpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/src/reactpy_django/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/websocket/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-07 03:44:59.000000 reactpy_django-3.0.1/src/reactpy_django/websocket/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:45:33.940506 reactpy_django-3.0.1/src/reactpy_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-07 03:45:33.000000 reactpy_django-3.0.1/src/reactpy_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-07 03:45:33.000000 reactpy_django-3.0.1/src/reactpy_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 03:45:33.000000 reactpy_django-3.0.1/src/reactpy_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 03:45:26.000000 reactpy_django-3.0.1/src/reactpy_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 03:45:33.000000 reactpy_django-3.0.1/src/reactpy_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-07 03:45:33.000000 reactpy_django-3.0.1/src/reactpy_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.828732 reactpy_django-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.832732 reactpy_django-3.1.0/src/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.832732 reactpy_django-3.1.0/src/reactpy_django/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/http/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/http/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.832732 reactpy_django-3.1.0/src/reactpy_django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.828732 reactpy_django-3.1.0/src/reactpy_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/src/reactpy_django/static/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django/static/reactpy_django/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.828732 reactpy_django-3.1.0/src/reactpy_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/src/reactpy_django/templates/reactpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/templates/reactpy/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/src/reactpy_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/templatetags/reactpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/src/reactpy_django/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/websocket/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/websocket/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.832732 reactpy_django-3.1.0/src/reactpy_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:47:24.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/top_level.txt
```

### Comparing `reactpy_django-3.0.1/LICENSE` & `reactpy_django-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/PKG-INFO` & `reactpy_django-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy_django
-Version: 3.0.1
+Version: 3.1.0
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
@@ -49,15 +49,15 @@
         <td>
             <a href="https://reactpy.dev/docs/guides/getting-started/installing-reactpy.html#officially-supported-servers">
                 Flask, FastAPI, Sanic, Tornado
             </a>
         </td>
         <td>
             <a href="https://github.com/reactive-python/reactpy-django">Django</a>,
-            <a href="https://github.com/idom-team/idom-jupyter">Jupyter</a>,
+            <a href="https://github.com/reactive-python/reactpy-jupyter">Jupyter</a>,
             <a href="https://github.com/idom-team/idom-dash">Plotly-Dash</a>
         </td>
         </tr>
     </tbody>
 </table>
 
 <!--intro-end-->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reactpy_django Version: 3.0.1 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy_django Version: 3.1.0 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
```

### Comparing `reactpy_django-3.0.1/README.md` & `reactpy_django-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         <td>
             <a href="https://reactpy.dev/docs/guides/getting-started/installing-reactpy.html#officially-supported-servers">
                 Flask, FastAPI, Sanic, Tornado
             </a>
         </td>
         <td>
             <a href="https://github.com/reactive-python/reactpy-django">Django</a>,
-            <a href="https://github.com/idom-team/idom-jupyter">Jupyter</a>,
+            <a href="https://github.com/reactive-python/reactpy-jupyter">Jupyter</a>,
             <a href="https://github.com/idom-team/idom-dash">Plotly-Dash</a>
         </td>
         </tr>
     </tbody>
 </table>
 
 <!--intro-end-->
```

### Comparing `reactpy_django-3.0.1/pyproject.toml` & `reactpy_django-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/setup.py` & `reactpy_django-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/src/reactpy_django/components.py` & `reactpy_django-3.1.0/src/reactpy_django/components.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/src/reactpy_django/config.py` & `reactpy_django-3.1.0/src/reactpy_django/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 from django.conf import settings
 from django.core.cache import DEFAULT_CACHE_ALIAS
 from django.db import DEFAULT_DB_ALIAS
 from reactpy.config import REACTPY_DEBUG_MODE
 from reactpy.core.types import ComponentConstructor
 
-from reactpy_django.types import Postprocessor, ViewComponentIframe
+from reactpy_django.types import (
+    AsyncPostprocessor,
+    SyncPostprocessor,
+    ViewComponentIframe,
+)
 from reactpy_django.utils import import_dotted_path
 
 
 # Not user configurable settings
 REACTPY_DEBUG_MODE.set_current(getattr(settings, "DEBUG"))
 REACTPY_REGISTERED_COMPONENTS: dict[str, ComponentConstructor] = {}
 REACTPY_VIEW_COMPONENT_IFRAMES: dict[str, ViewComponentIframe] = {}
@@ -33,14 +37,16 @@
     DEFAULT_CACHE_ALIAS,
 )
 REACTPY_DATABASE: str = getattr(
     settings,
     "REACTPY_DATABASE",
     DEFAULT_DB_ALIAS,
 )
-REACTPY_DEFAULT_QUERY_POSTPROCESSOR: Postprocessor | None = import_dotted_path(
-    getattr(
-        settings,
-        "REACTPY_DEFAULT_QUERY_POSTPROCESSOR",
-        "reactpy_django.utils.django_query_postprocessor",
+REACTPY_DEFAULT_QUERY_POSTPROCESSOR: AsyncPostprocessor | SyncPostprocessor | None = (
+    import_dotted_path(
+        getattr(
+            settings,
+            "REACTPY_DEFAULT_QUERY_POSTPROCESSOR",
+            "reactpy_django.utils.django_query_postprocessor",
+        )
     )
 )
```

### Comparing `reactpy_django-3.0.1/src/reactpy_django/decorators.py` & `reactpy_django-3.1.0/src/reactpy_django/decorators.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/src/reactpy_django/hooks.py` & `reactpy_django-3.1.0/src/reactpy_django/hooks.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,38 +9,35 @@
     DefaultDict,
     Sequence,
     Union,
     cast,
     overload,
 )
 
-from channels.db import database_sync_to_async as _database_sync_to_async
+from channels.db import database_sync_to_async
 from reactpy import use_callback, use_ref
 from reactpy.backend.hooks import use_connection as _use_connection
 from reactpy.backend.hooks import use_location as _use_location
 from reactpy.backend.hooks import use_scope as _use_scope
 from reactpy.backend.types import Location
 from reactpy.core.hooks import use_effect, use_state
 
 from reactpy_django.types import (
     Connection,
     Mutation,
+    MutationOptions,
     Query,
     QueryOptions,
     _Params,
     _Result,
 )
 from reactpy_django.utils import generate_obj_name
 
 
 _logger = logging.getLogger(__name__)
-database_sync_to_async = cast(
-    Callable[..., Callable[..., Awaitable[Any]]],
-    _database_sync_to_async,
-)
 _REFETCH_CALLBACKS: DefaultDict[
     Callable[..., Any], set[Callable[[], None]]
 ] = DefaultDict(set)
 
 
 def use_location() -> Location:
     """Get the current route as a `Location` object"""
@@ -78,26 +75,27 @@
     """Get the current `Connection` object"""
     return _use_connection()
 
 
 @overload
 def use_query(
     options: QueryOptions,
-    query: Callable[_Params, _Result | None],
     /,
+    query: Callable[_Params, _Result | None]
+    | Callable[_Params, Awaitable[_Result | None]],
     *args: _Params.args,
     **kwargs: _Params.kwargs,
 ) -> Query[_Result | None]:
     ...
 
 
 @overload
 def use_query(
-    query: Callable[_Params, _Result | None],
-    /,
+    query: Callable[_Params, _Result | None]
+    | Callable[_Params, Awaitable[_Result | None]],
     *args: _Params.args,
     **kwargs: _Params.kwargs,
 ) -> Query[_Result | None]:
     ...
 
 
 def use_query(
@@ -110,123 +108,222 @@
         options: An optional `QueryOptions` object that can modify how the query is executed.
         query: A callable that returns a Django `Model` or `QuerySet`.
         *args: Positional arguments to pass into `query`.
 
     Keyword Args:
         **kwargs: Keyword arguments to pass into `query`."""
 
+    should_execute, set_should_execute = use_state(True)
+    data, set_data = use_state(cast(Union[_Result, None], None))
+    loading, set_loading = use_state(True)
+    error, set_error = use_state(cast(Union[Exception, None], None))
     if isinstance(args[0], QueryOptions):
-        query_options = args[0]
-        query = args[1]
-        args = args[2:]
-
+        query_options, query, query_args, query_kwargs = _use_query_args_1(
+            *args, **kwargs
+        )
     else:
-        query_options = QueryOptions()
-        query = args[0]
-        args = args[1:]
-
+        query_options, query, query_args, query_kwargs = _use_query_args_2(
+            *args, **kwargs
+        )
     query_ref = use_ref(query)
     if query_ref.current is not query:
         raise ValueError(f"Query function changed from {query_ref.current} to {query}.")
 
-    should_execute, set_should_execute = use_state(True)
-    data, set_data = use_state(cast(Union[_Result, None], None))
-    loading, set_loading = use_state(True)
-    error, set_error = use_state(cast(Union[Exception, None], None))
-
-    @use_callback
-    def refetch() -> None:
-        set_should_execute(True)
-        set_loading(True)
-        set_error(None)
-
-    @use_effect(dependencies=[])
-    def add_refetch_callback() -> Callable[[], None]:
-        # By tracking callbacks globally, any usage of the query function will be re-run
-        # if the user has told a mutation to refetch it.
-        _REFETCH_CALLBACKS[query].add(refetch)
-        return lambda: _REFETCH_CALLBACKS[query].remove(refetch)
-
-    @use_effect(dependencies=None)
-    @database_sync_to_async
-    def execute_query() -> None:
-        if not should_execute:
-            return
-
+    # The main "running" function for `use_query`
+    async def execute_query() -> None:
         try:
-            # Run the initial query
-            new_data = query(*args, **kwargs)
+            # Run the query
+            if asyncio.iscoroutinefunction(query):
+                new_data = await query(*query_args, **query_kwargs)
+            else:
+                new_data = await database_sync_to_async(
+                    query,
+                    thread_sensitive=query_options.thread_sensitive,
+                )(*query_args, **query_kwargs)
 
+            # Run the postprocessor
             if query_options.postprocessor:
-                new_data = query_options.postprocessor(
-                    new_data, **query_options.postprocessor_kwargs
-                )
+                if asyncio.iscoroutinefunction(query_options.postprocessor):
+                    new_data = await query_options.postprocessor(
+                        new_data, **query_options.postprocessor_kwargs
+                    )
+                else:
+                    new_data = await database_sync_to_async(
+                        query_options.postprocessor,
+                        thread_sensitive=query_options.thread_sensitive,
+                    )(new_data, **query_options.postprocessor_kwargs)
 
+        # Log any errors and set the error state
         except Exception as e:
             set_data(None)
             set_loading(False)
             set_error(e)
             _logger.exception(
                 f"Failed to execute query: {generate_obj_name(query) or query}"
             )
             return
-        finally:
-            set_should_execute(False)
 
-        set_data(new_data)
-        set_loading(False)
+        # Query was successful
+        else:
+            set_data(new_data)
+            set_loading(False)
+            set_error(None)
+
+    # Schedule the query to be run when needed
+    @use_effect(dependencies=None)
+    def schedule_query() -> None:
+        # Make sure we don't re-execute the query unless we're told to
+        if not should_execute:
+            return
+        set_should_execute(False)
+
+        # Execute the query in the background
+        asyncio.create_task(execute_query())
+
+    # Used when the user has told us to refetch this query
+    @use_callback
+    def refetch() -> None:
+        set_should_execute(True)
+        set_loading(True)
         set_error(None)
 
+    # Track the refetch callback so we can re-execute the query
+    @use_effect(dependencies=[])
+    def add_refetch_callback() -> Callable[[], None]:
+        # By tracking callbacks globally, any usage of the query function will be re-run
+        # if the user has told a mutation to refetch it.
+        _REFETCH_CALLBACKS[query].add(refetch)
+        return lambda: _REFETCH_CALLBACKS[query].remove(refetch)
+
+    # The query's user API
     return Query(data, loading, error, refetch)
 
 
+@overload
+def use_mutation(
+    options: MutationOptions,
+    mutation: Callable[_Params, bool | None]
+    | Callable[_Params, Awaitable[bool | None]],
+    refetch: Callable[..., Any] | Sequence[Callable[..., Any]] | None = None,
+) -> Mutation[_Params]:
+    ...
+
+
+@overload
 def use_mutation(
-    mutate: Callable[_Params, bool | None],
+    mutation: Callable[_Params, bool | None]
+    | Callable[_Params, Awaitable[bool | None]],
     refetch: Callable[..., Any] | Sequence[Callable[..., Any]] | None = None,
 ) -> Mutation[_Params]:
+    ...
+
+
+def use_mutation(*args: Any, **kwargs: Any) -> Mutation[_Params]:
     """Hook to create, update, or delete Django ORM objects.
 
     Args:
         mutate: A callable that performs Django ORM create, update, or delete
             functionality. If this function returns `False`, then your `refetch`
             function will not be used.
         refetch: A `query` function (used by the `use_query` hook) or a sequence of `query`
             functions that will be called if the mutation succeeds. This is useful for
             refetching data after a mutation has been performed.
     """
 
     loading, set_loading = use_state(False)
     error, set_error = use_state(cast(Union[Exception, None], None))
+    if isinstance(args[0], MutationOptions):
+        mutation_options, mutation, refetch = _use_mutation_args_1(*args, **kwargs)
+    else:
+        mutation_options, mutation, refetch = _use_mutation_args_2(*args, **kwargs)
 
-    @use_callback
-    def call(*args: _Params.args, **kwargs: _Params.kwargs) -> None:
-        set_loading(True)
-
-        @database_sync_to_async
-        def execute_mutation() -> None:
-            try:
-                should_refetch = mutate(*args, **kwargs)
-            except Exception as e:
-                set_loading(False)
-                set_error(e)
-                _logger.exception(
-                    f"Failed to execute mutation: {generate_obj_name(mutate) or mutate}"
-                )
+    # The main "running" function for `use_mutation`
+    async def execute_mutation(exec_args, exec_kwargs) -> None:
+        # Run the mutation
+        try:
+            if asyncio.iscoroutinefunction(mutation):
+                should_refetch = await mutation(*exec_args, **exec_kwargs)
             else:
-                set_loading(False)
-                set_error(None)
+                should_refetch = await database_sync_to_async(
+                    mutation, thread_sensitive=mutation_options.thread_sensitive
+                )(*exec_args, **exec_kwargs)
+
+        # Log any errors and set the error state
+        except Exception as e:
+            set_loading(False)
+            set_error(e)
+            _logger.exception(
+                f"Failed to execute mutation: {generate_obj_name(mutation) or mutation}"
+            )
+
+        # Mutation was successful
+        else:
+            set_loading(False)
+            set_error(None)
+
+            # `refetch` will execute unless explicitly told not to
+            # or if `refetch` was not defined.
+            if should_refetch is not False and refetch:
+                for query in (refetch,) if callable(refetch) else refetch:
+                    for callback in _REFETCH_CALLBACKS.get(query) or ():
+                        callback()
 
-                # `refetch` will execute unless explicitly told not to
-                # or if `refetch` was not defined.
-                if should_refetch is not False and refetch:
-                    for query in (refetch,) if callable(refetch) else refetch:
-                        for callback in _REFETCH_CALLBACKS.get(query) or ():
-                            callback()
+    # Schedule the mutation to be run when needed
+    @use_callback
+    def schedule_mutation(
+        *exec_args: _Params.args, **exec_kwargs: _Params.kwargs
+    ) -> None:
+        # Set the loading state.
+        # It's okay to re-execute the mutation if we're told to. The user
+        # can use the `loading` state to prevent this.
+        set_loading(True)
 
-        asyncio.ensure_future(execute_mutation())
+        # Execute the mutation in the background
+        asyncio.ensure_future(
+            execute_mutation(exec_args=exec_args, exec_kwargs=exec_kwargs)
+        )
 
+    # Used when the user has told us to reset this mutation
     @use_callback
     def reset() -> None:
         set_loading(False)
         set_error(None)
 
-    return Mutation(call, loading, error, reset)
+    # The mutation's user API
+    return Mutation(schedule_mutation, loading, error, reset)
+
+
+def _use_query_args_1(
+    options: QueryOptions,
+    /,
+    query: Callable[_Params, _Result | None]
+    | Callable[_Params, Awaitable[_Result | None]],
+    *args: _Params.args,
+    **kwargs: _Params.kwargs,
+):
+    return options, query, args, kwargs
+
+
+def _use_query_args_2(
+    query: Callable[_Params, _Result | None]
+    | Callable[_Params, Awaitable[_Result | None]],
+    *args: _Params.args,
+    **kwargs: _Params.kwargs,
+):
+    return QueryOptions(), query, args, kwargs
+
+
+def _use_mutation_args_1(
+    options: MutationOptions,
+    mutation: Callable[_Params, bool | None]
+    | Callable[_Params, Awaitable[bool | None]],
+    refetch: Callable[..., Any] | Sequence[Callable[..., Any]] | None = None,
+):
+    return options, mutation, refetch
+
+
+def _use_mutation_args_2(
+    mutation: Callable[_Params, bool | None]
+    | Callable[_Params, Awaitable[bool | None]],
+    refetch: Callable[..., Any] | Sequence[Callable[..., Any]] | None = None,
+):
+    return MutationOptions(), mutation, refetch
```

### Comparing `reactpy_django-3.0.1/src/reactpy_django/http/views.py` & `reactpy_django-3.1.0/src/reactpy_django/http/views.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/src/reactpy_django/migrations/0001_initial.py` & `reactpy_django-3.1.0/src/reactpy_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py` & `reactpy_django-3.1.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/src/reactpy_django/static/reactpy_django/client.js` & `reactpy_django-3.1.0/src/reactpy_django/static/reactpy_django/client.js`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.0.1/src/reactpy_django/templatetags/reactpy.py` & `reactpy_django-3.1.0/src/reactpy_django/templatetags/reactpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from uuid import uuid4
 
 import dill as pickle
 from django import template
 from django.urls import reverse
 
 from reactpy_django import models
-from reactpy_django.config import REACTPY_RECONNECT_MAX, REACTPY_WEBSOCKET_URL
+from reactpy_django.config import (
+    REACTPY_DATABASE,
+    REACTPY_RECONNECT_MAX,
+    REACTPY_WEBSOCKET_URL,
+)
 from reactpy_django.types import ComponentParamData
 from reactpy_django.utils import _register_component, func_has_params
 
 
 REACTPY_WEB_MODULES_URL = reverse("reactpy:web_modules", args=["x"])[:-1][1:]
 register = template.Library()
 
@@ -43,15 +47,15 @@
     # Store the component's args/kwargs in the database if needed
     # This will be fetched by the websocket consumer later
     try:
         if func_has_params(component, *args, **kwargs):
             params = ComponentParamData(args, kwargs)
             model = models.ComponentSession(uuid=uuid, params=pickle.dumps(params))
             model.full_clean()
-            model.save()
+            model.save(using=REACTPY_DATABASE)
     except TypeError as e:
         raise TypeError(
             f"The provided parameters are incompatible with component '{dotted_path}'."
         ) from e
 
     return {
         "class": class_,
```

### Comparing `reactpy_django-3.0.1/src/reactpy_django/types.py` & `reactpy_django-3.1.0/src/reactpy_django/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,16 +26,18 @@
     "_Params",
     "_Data",
     "ComponentWebsocket",
     "Query",
     "Mutation",
     "Connection",
     "ViewComponentIframe",
-    "Postprocessor",
+    "AsyncPostprocessor",
+    "SyncPostprocessor",
     "QueryOptions",
+    "MutationOptions",
     "ComponentParamData",
 ]
 
 _Result = TypeVar("_Result", bound=Union[Model, QuerySet[Any]])
 _Params = ParamSpec("_Params")
 _Data = TypeVar("_Data")
 
@@ -75,26 +77,33 @@
 @dataclass
 class ViewComponentIframe:
     view: View | Callable
     args: Sequence
     kwargs: dict
 
 
-class Postprocessor(Protocol):
+class AsyncPostprocessor(Protocol):
+    async def __call__(self, data: Any) -> Any:
+        ...
+
+
+class SyncPostprocessor(Protocol):
     def __call__(self, data: Any) -> Any:
         ...
 
 
 @dataclass
 class QueryOptions:
     """Configuration options that can be provided to `use_query`."""
 
     from reactpy_django.config import REACTPY_DEFAULT_QUERY_POSTPROCESSOR
 
-    postprocessor: Postprocessor | None = REACTPY_DEFAULT_QUERY_POSTPROCESSOR
+    postprocessor: AsyncPostprocessor | SyncPostprocessor | None = (
+        REACTPY_DEFAULT_QUERY_POSTPROCESSOR
+    )
     """A callable that can modify the query `data` after the query has been executed.
 
     The first argument of postprocessor must be the query `data`. All proceeding arguments
     are optional `postprocessor_kwargs` (see below). This postprocessor function must return
     the modified `data`.
 
     If `None`, the default postprocessor is used.
@@ -102,14 +111,25 @@
     This default Django query postprocessor prevents Django's lazy query execution, and
     additionally can be configured via `postprocessor_kwargs` to recursively fetch
     `many_to_many` and `many_to_one` fields."""
 
     postprocessor_kwargs: MutableMapping[str, Any] = field(default_factory=lambda: {})
     """Keyworded arguments directly passed into the `postprocessor` for configuration."""
 
+    thread_sensitive: bool = True
+    """Whether to run the query in thread-sensitive mode. This setting only applies to sync query functions."""
+
+
+@dataclass
+class MutationOptions:
+    """Configuration options that can be provided to `use_mutation`."""
+
+    thread_sensitive: bool = True
+    """Whether to run the mutation in thread-sensitive mode. This setting only applies to sync mutation functions."""
+
 
 @dataclass
 class ComponentParamData:
     """Container used for serializing component parameters.
     This dataclass is pickled & stored in the database, then unpickled when needed."""
 
     args: Sequence
```

### Comparing `reactpy_django-3.0.1/src/reactpy_django/utils.py` & `reactpy_django-3.1.0/src/reactpy_django/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from fnmatch import fnmatch
 from importlib import import_module
 from inspect import iscoroutinefunction
 from typing import Any, Callable, Sequence
 
 from channels.db import database_sync_to_async
 from django.core.cache import caches
-from django.db.models import ManyToManyField, prefetch_related_objects
+from django.db.models import ManyToManyField, ManyToOneRel, prefetch_related_objects
 from django.db.models.base import Model
-from django.db.models.fields.reverse_related import ManyToOneRel
 from django.db.models.query import QuerySet
 from django.http import HttpRequest, HttpResponse
 from django.template import engines
 from django.utils import timezone
 from django.utils.encoding import smart_str
 from django.views import View
 
@@ -61,24 +60,28 @@
         else:  # View
             response = view_or_template_view
 
     # Render Check 3: Sync class view
     elif getattr(view, "as_view", None):
         # MyPy does not know how to properly interpret this as a `View` type
         # And `isinstance(view, View)` does not work due to some weird Django internal shenanigans
-        async_cbv = database_sync_to_async(view.as_view())  # type: ignore
+        async_cbv = database_sync_to_async(view.as_view(), thread_sensitive=False)  # type: ignore
         view_or_template_view = await async_cbv(request, *args, **kwargs)
         if getattr(view_or_template_view, "render", None):  # TemplateView
-            response = await database_sync_to_async(view_or_template_view.render)()
+            response = await database_sync_to_async(
+                view_or_template_view.render, thread_sensitive=False
+            )()
         else:  # View
             response = view_or_template_view
 
     # Render Check 4: Sync function view
     else:
-        response = await database_sync_to_async(view)(request, *args, **kwargs)
+        response = await database_sync_to_async(view, thread_sensitive=False)(
+            request, *args, **kwargs
+        )
 
     return response
 
 
 def _register_component(dotted_path: str) -> Callable:
     """Adds a component to the mapping of registered components.
     This should only be called on startup to maintain synchronization during mulitprocessing.
@@ -246,18 +249,16 @@
                 many_to_one=many_to_one,
             )
 
     # `Model` instances
     elif isinstance(data, Model):
         prefetch_fields: list[str] = []
         for field in data._meta.get_fields():
-            # `ForeignKey` relationships will cause an `AttributeError`
-            # This is handled within the `ManyToOneRel` conditional below.
-            with contextlib.suppress(AttributeError):
-                getattr(data, field.name)
+            # Force the query to execute
+            getattr(data, field.name, None)
 
             if many_to_one and type(field) == ManyToOneRel:
                 prefetch_fields.append(field.related_name or f"{field.name}_set")
 
             elif many_to_many and isinstance(field, ManyToManyField):
                 prefetch_fields.append(field.name)
 
@@ -306,15 +307,15 @@
     if not args:
         raise ValueError("At least one argument is required to create a cache key.")
 
     return f"reactpy_django:{':'.join(str(arg) for arg in args)}"
 
 
 def db_cleanup(immediate: bool = False):
-    """Deletes expired component parameters from the database.
+    """Deletes expired component sessions from the database.
     This function may be expanded in the future to include additional cleanup tasks."""
     from .config import REACTPY_CACHE, REACTPY_DATABASE, REACTPY_RECONNECT_MAX
     from .models import ComponentSession
 
     cache_key: str = create_cache_key("last_cleaned")
     now_str: str = datetime.strftime(timezone.now(), DATE_FORMAT)
     cleaned_at_str: str = caches[REACTPY_CACHE].get(cache_key)
@@ -334,8 +335,8 @@
 
     # Delete expired component parameters
     # Use timestamps in cache (`cleaned_at_str`) as a no-dependency rate limiter
     if immediate or not cleaned_at_str or timezone.now() >= clean_needed_by:
         ComponentSession.objects.using(REACTPY_DATABASE).filter(
             last_accessed__lte=expires_by
         ).delete()
-        caches[REACTPY_CACHE].set(cache_key, now_str)
+        caches[REACTPY_CACHE].set(cache_key, now_str, timeout=None)
```

### Comparing `reactpy_django-3.0.1/src/reactpy_django/websocket/consumer.py` & `reactpy_django-3.1.0/src/reactpy_django/websocket/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import asyncio
 import logging
 from datetime import timedelta
 from typing import Any, MutableMapping, Sequence
 
 import dill as pickle
 from channels.auth import login
-from channels.db import database_sync_to_async as convert_to_async
+from channels.db import database_sync_to_async
 from channels.generic.websocket import AsyncJsonWebsocketConsumer
 from django.utils import timezone
 from reactpy.backend.hooks import ConnectionContext
 from reactpy.backend.types import Connection, Location
 from reactpy.core.layout import Layout
 from reactpy.core.serve import serve_layout
 
@@ -31,15 +31,15 @@
 
         await super().connect()
 
         user: AbstractBaseUser = self.scope.get("user")
         if user and user.is_authenticated:
             try:
                 await login(self.scope, user)
-                await convert_to_async(self.scope["session"].save)()
+                await database_sync_to_async(self.scope["session"].save)()
             except Exception:
                 _logger.exception("ReactPy websocket authentication has failed!")
         elif user is None:
             _logger.warning("ReactPy websocket is missing AuthMiddlewareStack!")
 
         self._reactpy_dispatcher_future = asyncio.ensure_future(
             self._run_dispatch_loop()
@@ -90,26 +90,28 @@
             return
 
         # Fetch the component's args/kwargs from the database, if needed
         try:
             if func_has_params(component_constructor):
                 try:
                     # Always clean up expired entries first
-                    await convert_to_async(db_cleanup)()
+                    await database_sync_to_async(db_cleanup, thread_sensitive=False)()
 
                     # Get the queries from a DB
                     params_query = await models.ComponentSession.objects.using(
                         REACTPY_DATABASE
                     ).aget(
                         uuid=uuid,
                         last_accessed__gt=now
                         - timedelta(seconds=REACTPY_RECONNECT_MAX),
                     )
                     params_query.last_accessed = timezone.now()
-                    await convert_to_async(params_query.save)()
+                    await database_sync_to_async(
+                        params_query.save, thread_sensitive=False
+                    )()
                 except models.ComponentSession.DoesNotExist:
                     _logger.warning(
                         f"Browser has attempted to access '{dotted_path}', "
                         f"but the component has already expired beyond REACTPY_RECONNECT_MAX. "
                         "If this was expected, this warning can be ignored."
                     )
                     return
```

### Comparing `reactpy_django-3.0.1/src/reactpy_django.egg-info/PKG-INFO` & `reactpy_django-3.1.0/src/reactpy_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-django
-Version: 3.0.1
+Version: 3.1.0
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
@@ -49,15 +49,15 @@
         <td>
             <a href="https://reactpy.dev/docs/guides/getting-started/installing-reactpy.html#officially-supported-servers">
                 Flask, FastAPI, Sanic, Tornado
             </a>
         </td>
         <td>
             <a href="https://github.com/reactive-python/reactpy-django">Django</a>,
-            <a href="https://github.com/idom-team/idom-jupyter">Jupyter</a>,
+            <a href="https://github.com/reactive-python/reactpy-jupyter">Jupyter</a>,
             <a href="https://github.com/idom-team/idom-dash">Plotly-Dash</a>
         </td>
         </tr>
     </tbody>
 </table>
 
 <!--intro-end-->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reactpy-django Version: 3.0.1 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy-django Version: 3.1.0 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
```

### Comparing `reactpy_django-3.0.1/src/reactpy_django.egg-info/SOURCES.txt` & `reactpy_django-3.1.0/src/reactpy_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

