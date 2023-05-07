# Comparing `tmp/Routing_flet-0.0.3.tar.gz` & `tmp/Routing_flet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Routing_flet-0.0.3.tar", last modified: Sun May  7 18:55:12 2023, max compression
+gzip compressed data, was "Routing_flet-0.0.4.tar", last modified: Sun May  7 20:11:41 2023, max compression
```

## Comparing `Routing_flet-0.0.3.tar` & `Routing_flet-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 18:55:12.582974 Routing_flet-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-05-07 15:21:51.000000 Routing_flet-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4530 2023-05-07 18:55:12.580973 Routing_flet-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3932 2023-05-07 18:51:12.000000 Routing_flet-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 18:55:12.537399 Routing_flet-0.0.3/Routing_flet/
--rw-rw-rw-   0        0        0     3028 2023-05-07 18:36:31.000000 Routing_flet-0.0.3/Routing_flet/ViewPage.py
--rw-rw-rw-   0        0        0       91 2023-05-07 18:33:57.000000 Routing_flet-0.0.3/Routing_flet/__init__.py
--rw-rw-rw-   0        0        0     2936 2023-05-07 18:33:49.000000 Routing_flet-0.0.3/Routing_flet/cli.py
--rw-rw-rw-   0        0        0     1033 2023-05-07 18:30:55.000000 Routing_flet-0.0.3/Routing_flet/config.py
--rw-rw-rw-   0        0        0     2861 2023-05-07 18:47:00.000000 Routing_flet-0.0.3/Routing_flet/route.py
-drwxrwxrwx   0        0        0        0 2023-05-07 18:55:12.568963 Routing_flet-0.0.3/Routing_flet.egg-info/
--rw-rw-rw-   0        0        0     4530 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 18:55:12.000000 Routing_flet-0.0.3/Routing_flet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 18:55:12.583969 Routing_flet-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1176 2023-05-07 18:54:57.000000 Routing_flet-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:11:41.472435 Routing_flet-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-07 15:21:51.000000 Routing_flet-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4530 2023-05-07 20:11:41.471432 Routing_flet-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3932 2023-05-07 18:51:12.000000 Routing_flet-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 20:11:41.408767 Routing_flet-0.0.4/Routing_flet/
+-rw-rw-rw-   0        0        0      886 2023-05-03 18:02:16.000000 Routing_flet-0.0.4/Routing_flet/404.py
+-rw-rw-rw-   0        0        0     3028 2023-05-07 18:36:31.000000 Routing_flet-0.0.4/Routing_flet/ViewPage.py
+-rw-rw-rw-   0        0        0       91 2023-05-07 18:33:57.000000 Routing_flet-0.0.4/Routing_flet/__init__.py
+-rw-rw-rw-   0        0        0     2898 2023-05-07 20:10:52.000000 Routing_flet-0.0.4/Routing_flet/cli.py
+-rw-rw-rw-   0        0        0     1033 2023-05-07 18:30:55.000000 Routing_flet-0.0.4/Routing_flet/config.py
+-rw-rw-rw-   0        0        0     1105 2023-05-03 18:01:12.000000 Routing_flet-0.0.4/Routing_flet/index.py
+-rw-rw-rw-   0        0        0      209 2023-05-03 17:59:59.000000 Routing_flet-0.0.4/Routing_flet/main.py
+-rw-rw-rw-   0        0        0     2861 2023-05-07 18:47:00.000000 Routing_flet-0.0.4/Routing_flet/route.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:11:41.453351 Routing_flet-0.0.4/Routing_flet.egg-info/
+-rw-rw-rw-   0        0        0     4530 2023-05-07 20:11:41.000000 Routing_flet-0.0.4/Routing_flet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-05-07 20:11:41.000000 Routing_flet-0.0.4/Routing_flet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 20:11:41.000000 Routing_flet-0.0.4/Routing_flet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-07 20:11:41.000000 Routing_flet-0.0.4/Routing_flet.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-07 20:11:41.000000 Routing_flet-0.0.4/Routing_flet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 20:11:41.000000 Routing_flet-0.0.4/Routing_flet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 20:11:41.473435 Routing_flet-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2023-05-07 20:11:05.000000 Routing_flet-0.0.4/setup.py
```

### Comparing `Routing_flet-0.0.3/LICENSE` & `Routing_flet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Routing_flet-0.0.3/PKG-INFO` & `Routing_flet-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Routing_flet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Esta es la descripcion de mi paquete
 Home-page: https://github.com/Dxsxsx/Routing_flet
 Download-URL: https://github.com/Dxsxsx/Routing_flet
 Author: Dxsxsx
 Project-URL: Bug Tracker, https://github.com/Dxsxsx/Routing_flet/issues
 Keywords: python web template,web application,development
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ♾️Routing_flet -> Enrutamiento y protección de paginas facil con flet
 ## instalar
```

### Comparing `Routing_flet-0.0.3/README.md` & `Routing_flet-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Routing_flet-0.0.3/Routing_flet/ViewPage.py` & `Routing_flet-0.0.4/Routing_flet/ViewPage.py`

 * *Files identical despite different names*

### Comparing `Routing_flet-0.0.3/Routing_flet/cli.py` & `Routing_flet-0.0.4/Routing_flet/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 @struct_app.command(help='Crea una estructura: [views,controllers,models]')
 def mvc():
     # creacion archivo main.pypip
     file_path_main = Path('./') / 'main.py'
     file_path_main.touch()
 
-    source_path = Path(__file__).parent / 'struct/main.py'
+    source_path = Path(__file__).parent / 'main.py'
 
     with open(source_path, 'r') as source_file:
         content = source_file.read()
 
     with open(file_path_main, 'w') as file:
         file.write(content)
 
@@ -30,15 +30,15 @@
 
     file_list = ['index.py', '404.py']
 
     for file_name in file_list:
         file = Path('views') / file_name
         file.touch()
 
-        source_path = Path(__file__).parent / f'struct/{file_name}'
+        source_path = Path(__file__).parent / file_name
 
         with open(source_path, 'r') as source_file:
             content = source_file.read()
 
         with open(file, 'w') as file:
             file.write(content)
 
@@ -50,15 +50,15 @@
 # views
 @struct_app.command(help='Crea una estructura: main.py [views]')
 def v():
     # creacion archivo main.pypip
     file_path_main = Path('./') / 'main.py'
     file_path_main.touch()
 
-    source_path = Path(__file__).parent / 'struct/main.py'
+    source_path = Path(__file__).parent / 'main.py'
 
     with open(source_path, 'r') as source_file:
         content = source_file.read()
 
     with open(file_path_main, 'w') as file:
         file.write(content)
 
@@ -69,15 +69,15 @@
 
     file_list = ['index.py', '404.py']
 
     for file_name in file_list:
         file = Path('views') / file_name
         file.touch()
 
-        source_path = Path(__file__).parent / f'struct/{file_name}'
+        source_path = Path(__file__).parent / file_name
 
         with open(source_path, 'r') as source_file:
             content = source_file.read()
 
         with open(file, 'w') as file:
             file.write(content)
```

### Comparing `Routing_flet-0.0.3/Routing_flet/config.py` & `Routing_flet-0.0.4/Routing_flet/config.py`

 * *Files identical despite different names*

### Comparing `Routing_flet-0.0.3/Routing_flet/route.py` & `Routing_flet-0.0.4/Routing_flet/route.py`

 * *Files identical despite different names*

### Comparing `Routing_flet-0.0.3/Routing_flet.egg-info/PKG-INFO` & `Routing_flet-0.0.4/Routing_flet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Routing-flet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Esta es la descripcion de mi paquete
 Home-page: https://github.com/Dxsxsx/Routing_flet
 Download-URL: https://github.com/Dxsxsx/Routing_flet
 Author: Dxsxsx
 Project-URL: Bug Tracker, https://github.com/Dxsxsx/Routing_flet/issues
 Keywords: python web template,web application,development
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ♾️Routing_flet -> Enrutamiento y protección de paginas facil con flet
 ## instalar
```

### Comparing `Routing_flet-0.0.3/setup.py` & `Routing_flet-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = e.read()
 
 print(long_description)
 
 
 setup(
     name='Routing_flet', 
-    version='0.0.3',
+    version='0.0.4',
     author='Dxsxsx',
     description='Esta es la descripcion de mi paquete',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Dxsxsx/Routing_flet',
     download_url='https://github.com/Dxsxsx/Routing_flet',
     project_urls = {
```

