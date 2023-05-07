# Comparing `tmp/Routing_flet-0.0.2.tar.gz` & `tmp/Routing_flet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Routing_flet-0.0.2.tar", last modified: Sun Apr 30 02:08:54 2023, max compression
+gzip compressed data, was "Routing_flet-0.0.3.tar", last modified: Sun May  7 18:55:12 2023, max compression
```

## Comparing `Routing_flet-0.0.2.tar` & `Routing_flet-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 02:08:54.205343 Routing_flet-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-29 23:40:07.000000 Routing_flet-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      989 2023-04-30 02:08:54.204333 Routing_flet-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-04-30 01:54:43.000000 Routing_flet-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 02:08:54.206339 Routing_flet-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1059 2023-04-30 02:08:35.000000 Routing_flet-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 02:08:54.135652 Routing_flet-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 02:08:54.164200 Routing_flet-0.0.2/src/Routing_flet/
--rw-rw-rw-   0        0        0     2598 2023-04-30 01:54:43.000000 Routing_flet-0.0.2/src/Routing_flet/ViewPage.py
--rw-rw-rw-   0        0        0       84 2023-04-30 01:14:13.000000 Routing_flet-0.0.2/src/Routing_flet/__init__.py
--rw-rw-rw-   0        0        0     1092 2023-04-29 23:40:07.000000 Routing_flet-0.0.2/src/Routing_flet/config.py
--rw-rw-rw-   0        0        0     2976 2023-04-30 01:54:43.000000 Routing_flet-0.0.2/src/Routing_flet/route.py
-drwxrwxrwx   0        0        0        0 2023-04-30 02:08:54.202321 Routing_flet-0.0.2/src/Routing_flet.egg-info/
--rw-rw-rw-   0        0        0      989 2023-04-30 02:08:54.000000 Routing_flet-0.0.2/src/Routing_flet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-04-30 02:08:54.000000 Routing_flet-0.0.2/src/Routing_flet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 02:08:54.000000 Routing_flet-0.0.2/src/Routing_flet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 02:08:54.000000 Routing_flet-0.0.2/src/Routing_flet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 18:55:12.582974 Routing_flet-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-07 15:21:51.000000 Routing_flet-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4530 2023-05-07 18:55:12.580973 Routing_flet-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3932 2023-05-07 18:51:12.000000 Routing_flet-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 18:55:12.537399 Routing_flet-0.0.3/Routing_flet/
+-rw-rw-rw-   0        0        0     3028 2023-05-07 18:36:31.000000 Routing_flet-0.0.3/Routing_flet/ViewPage.py
+-rw-rw-rw-   0        0        0       91 2023-05-07 18:33:57.000000 Routing_flet-0.0.3/Routing_flet/__init__.py
+-rw-rw-rw-   0        0        0     2936 2023-05-07 18:33:49.000000 Routing_flet-0.0.3/Routing_flet/cli.py
+-rw-rw-rw-   0        0        0     1033 2023-05-07 18:30:55.000000 Routing_flet-0.0.3/Routing_flet/config.py
+-rw-rw-rw-   0        0        0     2861 2023-05-07 18:47:00.000000 Routing_flet-0.0.3/Routing_flet/route.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:55:12.568963 Routing_flet-0.0.3/Routing_flet.egg-info/
+-rw-rw-rw-   0        0        0     4530 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 18:55:12.583969 Routing_flet-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2023-05-07 18:54:57.000000 Routing_flet-0.0.3/setup.py
```

### Comparing `Routing_flet-0.0.2/LICENSE` & `Routing_flet-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Routing_flet-0.0.2/setup.py` & `Routing_flet-0.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 with open("./README.md", "r", encoding="utf-8") as e:
     long_description = e.read()
 
 print(long_description)
 
 
 setup(
     name='Routing_flet', 
-    version='0.0.2',
+    version='0.0.3',
     author='Dxsxsx',
-    description='Enrutamiento y login requerido facil con flet',
+    description='Esta es la descripcion de mi paquete',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Dxsxsx/Routing_flet',
     download_url='https://github.com/Dxsxsx/Routing_flet',
-    requires=['flet'],
     project_urls = {
-        "Bug Tracker":"https://github.com/Dxsxsx/Routing_flet/releases"
+        "Bug Tracker":"https://github.com/Dxsxsx/Routing_flet/issues"
     },
+    install_requires=["typer[all]", "flet"],
     classifiers={
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     },
-    package_dir={"":"src"},
-    packages=find_packages(where='src'),
+    packages=["Routing_flet"],
     python_requires=">=3.6",
+    entry_points={
+        "console_scripts": ["dxs=Routing_flet.cli:main"],
+    },
+    keywords=["python web template", "web application", "development"],
 )
 
 """ 
 py -m pip install --upgrade build
 py -m build
 
 py -m pip install --upgrade twine
```

### Comparing `Routing_flet-0.0.2/src/Routing_flet/ViewPage.py` & `Routing_flet-0.0.3/Routing_flet/ViewPage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 from flet import Page, View, Column, Text, MainAxisAlignment, CrossAxisAlignment
 
+class Params:
+    def __init__(self, params: list = None) -> list:
+        self.params = params
+    
+    def get_all(self):
+        return self.params
+
+    def get(self, key: str):
+        return self.params[key]
+
 
 class ViewPage:
     """ 
     Usar el siguiente metodo dentro de la clase si se requiere un login requerido a la página (True: para acceder | None: Por defecto) o denegar (False: Renvia a la ruta -> '/' )
     ```
     def login_requi(self):
         return None
@@ -23,16 +33,17 @@
     class View(ViewPage):
         def __init__(self) -> None:
             self.route = '/about/1/2'
 
         def math_url(self):
             return ['id', 'name', 'edad']
 
-        def view(self, page: ft.Page):
+        def view(self, page: ft.Page, params:Params): # Params: para acceder a los parametros enviados en la url
             page.title = 'contact'
+            print('Mi params:' params.get_all())
             return ft.View(
                 self.route,
                 controls=[
                     ft.Column(
                         [
                             ft.Container(
                                 content=ft.Text('index about', size=50),
@@ -55,28 +66,29 @@
             )
     ``` 
     """
 
     def __init__(self) -> None:
         self.route = '/'
 
-    def math_url(self) -> dict:
+    def math_url(self) -> list:
         return None
 
     def route(self) -> str:
         return self.route
-    
-    def login_requi(self):
+
+    def login_requi(self) -> bool:
         return None
 
-    def view(self, page: Page):
+    def view(self, page: Page, params: Params = None) -> object:
         page.title = 'WiewPage'
+        print('parametro:', params.get('id'))
         return View(
             self.route,
             controls=[
                 Column(
                     Text('View Page', size=90)
                 )
             ],
             vertical_alignment=MainAxisAlignment.CENTER,
             horizontal_alignment=CrossAxisAlignment.CENTER
-        )
+        )
```

### Comparing `Routing_flet-0.0.2/src/Routing_flet/config.py` & `Routing_flet-0.0.3/Routing_flet/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import os
 import importlib.util
 _moduleList = {}
 _modList = {}
 
+
 def pages_view():
     _moduleList.clear()
     for root, dirs, __ in os.walk(r'./'):
         for dir in dirs:
             if dir == 'views':
                 for filename in os.listdir('views'):
                     _file = os.path.join('views', filename)
                     if os.path.isfile(_file):
                         filename = filename.strip('.py')
                         if filename != '__init__':
                             _moduleList[filename] = importlib.util.spec_from_file_location(
                                 filename, _file)
     return _moduleList
 
+
 class WiewModel:
     def __init__(self) -> None:
         pass
+
     def route(self):
         pass
+
     def view(self):
         pass
 
-def routing()->WiewModel:
+
+def routing() -> WiewModel:
     _modList.clear()
     for view in pages_view():
         page = pages_view().get(view).loader.load_module().View()
         route = page.route
         _modList[route] = page
-    print('urls->', _modList)
     return _modList
-
-if __name__ == '__main__':
-    pass
```

### Comparing `Routing_flet-0.0.2/src/Routing_flet/route.py` & `Routing_flet-0.0.3/Routing_flet/route.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from flet import Page
 from Routing_flet.config import routing
+from Routing_flet import Params
+from rich import print as pt
 
 route_page = routing()
 
+
 class RoutePage:
 
     """ 
     Uso de la clase:
     ```
     RoutePage(
         page=page # Clase Page de Flet que llega como referencia
@@ -30,56 +33,52 @@
         self.page.views.clear()
         pg_404 = True
 
         for key, value in route_page.items():
             if key != '/404':
                 if key == route.route[0:len(key)]:
                     if value.math_url() != None:
-                        params = {}
+                        params_u = {}
                         k = 0
                         url_value = route.route.replace(key+'/', '').split('/')
                         if '' not in url_value:
                             url_ext = len(url_value)
                             if len(value.math_url()) == url_ext:
                                 pg_404 = False
                                 if value.login_requi() == None or value.login_requi() == True:
-                                    """ verificacion """
-                                    params.clear()
-                                    self.page.views.append(
-                                        value.view(self.page))
+                                    params_u.clear()
                                     for i in value.math_url():
-                                        params[i] = url_value[k]
+                                        params_u[i] = url_value[k]
                                         k += 1
-                                    print('♾️  params:', params)
+                                    params = Params(params_u)
+                                    self.page.views.append(
+                                        value.view(self.page, params))
                                     break
                                 else:
                                     self.page.go('/')
                                     break
 
                     elif route.route == key:
                         pg_404 = False
                         if value.login_requi() == None or value.login_requi() == True:
-                            """ Verificacion """
                             self.page.views.append(value.view(self.page))
                             break
                         else:
                             self.page.go('/')
                             break
 
         if pg_404:
-            params = route.route
-            print('ruta 404:', route_page['/404'].route)
             self.page.views.append(route_page['/404'].view(self.page))
 
         self.page.update()
 
     def view_pop(self, view):
         self.page.views.pop()
         top_view = self.page.views[-1]
         self.page.go(top_view.route)
 
     def run(self):
         self.page.on_route_change = self.route_change
         self.page.on_view_pop = self.view_pop
         self.page.go(self.page.route)
         self.page.update()
-        print('>>Reload')
+        pt('[green]>> Reload[/green]')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

