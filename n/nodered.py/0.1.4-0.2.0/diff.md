# Comparing `tmp/nodered.py-0.1.4.tar.gz` & `tmp/nodered.py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.1.4.tar", last modified: Tue May  2 11:31:07 2023, max compression
+gzip compressed data, was "nodered.py-0.2.0.tar", last modified: Sun May  7 12:38:52 2023, max compression
```

## Comparing `nodered.py-0.1.4.tar` & `nodered.py-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.310000 nodered.py-0.1.4/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.4/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-05-02 11:31:07.400000 nodered.py-0.1.4/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1758 2023-04-30 04:58:00.000000 nodered.py-0.1.4/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.310000 nodered.py-0.1.4/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      543 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       57 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.4/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.310000 nodered.py-0.1.4/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      496 2023-05-02 10:41:48.000000 nodered.py-0.1.4/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5580 2023-05-01 13:06:41.000000 nodered.py-0.1.4/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.1.4/noderedpy/_property.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6410 2023-04-30 03:53:02.000000 nodered.py-0.1.4/noderedpy/_server.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      805 2023-04-30 03:52:23.000000 nodered.py-0.1.4/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.320000 nodered.py-0.1.4/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2398 2023-04-29 01:58:51.000000 nodered.py-0.1.4/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.4/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.320000 nodered.py-0.1.4/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7470 2023-05-02 10:45:53.000000 nodered.py-0.1.4/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      971 2023-05-01 13:00:37.000000 nodered.py-0.1.4/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3212 2023-05-01 13:01:59.000000 nodered.py-0.1.4/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      269 2023-05-01 13:03:04.000000 nodered.py-0.1.4/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-05-02 11:31:07.400000 nodered.py-0.1.4/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1077 2023-05-01 12:49:35.000000 nodered.py-0.1.4/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.420000 nodered.py-0.2.0/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.0/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2229 2023-05-07 12:38:52.540000 nodered.py-0.2.0/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1913 2023-05-07 12:35:08.000000 nodered.py-0.2.0/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.420000 nodered.py-0.2.0/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2229 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.0/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.420000 nodered.py-0.2.0/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-05-07 12:04:58.000000 nodered.py-0.2.0/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    10262 2023-05-07 12:14:13.000000 nodered.py-0.2.0/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.0/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.430000 nodered.py-0.2.0/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.0/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      807 2023-05-07 08:57:45.000000 nodered.py-0.2.0/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.430000 nodered.py-0.2.0/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.0/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2512 2023-05-07 01:35:50.000000 nodered.py-0.2.0/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.2.0/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.430000 nodered.py-0.2.0/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7480 2023-05-07 08:38:57.000000 nodered.py-0.2.0/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      971 2023-05-01 13:00:37.000000 nodered.py-0.2.0/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.0/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      269 2023-05-01 13:03:04.000000 nodered.py-0.2.0/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-05-07 12:38:52.540000 nodered.py-0.2.0/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-05-07 01:29:24.000000 nodered.py-0.2.0/setup.py
```

### Comparing `nodered.py-0.1.4/LICENSE` & `nodered.py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.4/PKG-INFO` & `nodered.py-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.4
+Version: 0.2.0
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -39,56 +39,57 @@
 ```zsh
 python -m pip install git+https://github.com/oyajiDev/NodeRED.py.git
 ```
 
 <br/><br/>
 
 ## 🛠 usage
-### server initialize
-- default server
+### Node-RED initialize
 ```python
-from noderedpy import Server, RED
+from noderedpy import RED
 
-server = Server(
-    RED(
-        os.path.join(__dirname, ".node-red"),
-        "/node-red", 1880
-    )
+red = RED(
+    os.path.join(__dirname, ".node-red"),
+    os.path.join(__dirname, "node_red_dir"),
+    "/node-red", 1880
 )
 ```
-- standalone(with webview)
-```python
-from noderedpy import StandaloneServer, RED
 
-server = StandaloneServer(
-    RED(
-        os.path.join(__dirname, ".node-red"),
-        "/node-red", 1880
-    )
-)
-```
 <br/>
 
 ### register Node
+- register as decorator
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
 ```python
+from noderedpy.decorator import register
+
 @register("test")
 def test(props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
-- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
+- register from Node-RED object
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
+```python
+api = API()
+
+red.register("test", api.test)
+```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
+
 <br/>
 
-### start server
-- default server
-```python
-server.start("{port}")
-```
-- standalone(with webview)
+### start Node-RED
 ```python
-server.start("{title}")
+red.start({debug:bool}, {callback:MethodType})
 ```
 <br/><br/>
 
 ## Todos
 [x] type support for "list" and "dict"
+
+<br/><br/>
+
+## Roadmap To 2.0
+[x] remove aiohttp server
+
+[ ] flexible property ui
```

#### html2text {}

```diff
@@ -1,27 +1,30 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.4 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.0 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
-## ð  usage ### server initialize - default server ```python from noderedpy
-import Server, RED server = Server( RED( os.path.join(__dirname, ".node-red"),
-"/node-red", 1880 ) ) ``` - standalone(with webview) ```python from noderedpy
-import StandaloneServer, RED server = StandaloneServer( RED( os.path.join
-(__dirname, ".node-red"), "/node-red", 1880 ) ) ```
-### register Node ```python @register("test") def test(props:dict, msg:dict) -
-> dict: # user codes here return msg ``` - See noredpy.decorator.register
-function for details - See noderedpy._property for details of "Property"
-### start server - default server ```python server.start("{port}") ``` -
-standalone(with webview) ```python server.start("{title}") ```
+## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
+RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
+"node_red_dir"), "/node-red", 1880 ) ```
+### register Node - register as decorator - See noredpy.decorator.register
+function for details ```python from noderedpy.decorator import register
+@register("test") def test(props:dict, msg:dict) -> dict: # user codes here
+return msg ``` - register from Node-RED object - See noredpy.decorator.register
+function for details ```python api = API() red.register("test", api.test) ``` -
+See noderedpy._property for details of "Property"
+### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
+
 
 ## Todos [x] type support for "list" and "dict"
+
+## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.1.4/README.md` & `nodered.py-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,56 +27,57 @@
 ```zsh
 python -m pip install git+https://github.com/oyajiDev/NodeRED.py.git
 ```
 
 <br/><br/>
 
 ## 🛠 usage
-### server initialize
-- default server
+### Node-RED initialize
 ```python
-from noderedpy import Server, RED
+from noderedpy import RED
 
-server = Server(
-    RED(
-        os.path.join(__dirname, ".node-red"),
-        "/node-red", 1880
-    )
+red = RED(
+    os.path.join(__dirname, ".node-red"),
+    os.path.join(__dirname, "node_red_dir"),
+    "/node-red", 1880
 )
 ```
-- standalone(with webview)
-```python
-from noderedpy import StandaloneServer, RED
 
-server = StandaloneServer(
-    RED(
-        os.path.join(__dirname, ".node-red"),
-        "/node-red", 1880
-    )
-)
-```
 <br/>
 
 ### register Node
+- register as decorator
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
 ```python
+from noderedpy.decorator import register
+
 @register("test")
 def test(props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
-- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
+- register from Node-RED object
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
+```python
+api = API()
+
+red.register("test", api.test)
+```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
+
 <br/>
 
-### start server
-- default server
-```python
-server.start("{port}")
-```
-- standalone(with webview)
+### start Node-RED
 ```python
-server.start("{title}")
+red.start({debug:bool}, {callback:MethodType})
 ```
 <br/><br/>
 
 ## Todos
 [x] type support for "list" and "dict"
+
+<br/><br/>
+
+## Roadmap To 2.0
+[x] remove aiohttp server
+
+[ ] flexible property ui
```

#### html2text {}

```diff
@@ -4,19 +4,22 @@
                              [MIT_License] [pypi]
 
 
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
-## ð  usage ### server initialize - default server ```python from noderedpy
-import Server, RED server = Server( RED( os.path.join(__dirname, ".node-red"),
-"/node-red", 1880 ) ) ``` - standalone(with webview) ```python from noderedpy
-import StandaloneServer, RED server = StandaloneServer( RED( os.path.join
-(__dirname, ".node-red"), "/node-red", 1880 ) ) ```
-### register Node ```python @register("test") def test(props:dict, msg:dict) -
-> dict: # user codes here return msg ``` - See noredpy.decorator.register
-function for details - See noderedpy._property for details of "Property"
-### start server - default server ```python server.start("{port}") ``` -
-standalone(with webview) ```python server.start("{title}") ```
+## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
+RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
+"node_red_dir"), "/node-red", 1880 ) ```
+### register Node - register as decorator - See noredpy.decorator.register
+function for details ```python from noderedpy.decorator import register
+@register("test") def test(props:dict, msg:dict) -> dict: # user codes here
+return msg ``` - register from Node-RED object - See noredpy.decorator.register
+function for details ```python api = API() red.register("test", api.test) ``` -
+See noderedpy._property for details of "Property"
+### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
+
 
 ## Todos [x] type support for "list" and "dict"
+
+## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.1.4/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.0/nodered.py.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.4
+Version: 0.2.0
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -39,56 +39,57 @@
 ```zsh
 python -m pip install git+https://github.com/oyajiDev/NodeRED.py.git
 ```
 
 <br/><br/>
 
 ## 🛠 usage
-### server initialize
-- default server
+### Node-RED initialize
 ```python
-from noderedpy import Server, RED
+from noderedpy import RED
 
-server = Server(
-    RED(
-        os.path.join(__dirname, ".node-red"),
-        "/node-red", 1880
-    )
+red = RED(
+    os.path.join(__dirname, ".node-red"),
+    os.path.join(__dirname, "node_red_dir"),
+    "/node-red", 1880
 )
 ```
-- standalone(with webview)
-```python
-from noderedpy import StandaloneServer, RED
 
-server = StandaloneServer(
-    RED(
-        os.path.join(__dirname, ".node-red"),
-        "/node-red", 1880
-    )
-)
-```
 <br/>
 
 ### register Node
+- register as decorator
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
 ```python
+from noderedpy.decorator import register
+
 @register("test")
 def test(props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
-- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
+- register from Node-RED object
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
+```python
+api = API()
+
+red.register("test", api.test)
+```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
+
 <br/>
 
-### start server
-- default server
-```python
-server.start("{port}")
-```
-- standalone(with webview)
+### start Node-RED
 ```python
-server.start("{title}")
+red.start({debug:bool}, {callback:MethodType})
 ```
 <br/><br/>
 
 ## Todos
 [x] type support for "list" and "dict"
+
+<br/><br/>
+
+## Roadmap To 2.0
+[x] remove aiohttp server
+
+[ ] flexible property ui
```

#### html2text {}

```diff
@@ -1,27 +1,30 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.4 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.0 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
-## ð  usage ### server initialize - default server ```python from noderedpy
-import Server, RED server = Server( RED( os.path.join(__dirname, ".node-red"),
-"/node-red", 1880 ) ) ``` - standalone(with webview) ```python from noderedpy
-import StandaloneServer, RED server = StandaloneServer( RED( os.path.join
-(__dirname, ".node-red"), "/node-red", 1880 ) ) ```
-### register Node ```python @register("test") def test(props:dict, msg:dict) -
-> dict: # user codes here return msg ``` - See noredpy.decorator.register
-function for details - See noderedpy._property for details of "Property"
-### start server - default server ```python server.start("{port}") ``` -
-standalone(with webview) ```python server.start("{title}") ```
+## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
+RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
+"node_red_dir"), "/node-red", 1880 ) ```
+### register Node - register as decorator - See noredpy.decorator.register
+function for details ```python from noderedpy.decorator import register
+@register("test") def test(props:dict, msg:dict) -> dict: # user codes here
+return msg ``` - register from Node-RED object - See noredpy.decorator.register
+function for details ```python api = API() red.register("test", api.test) ``` -
+See noderedpy._property for details of "Property"
+### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
+
 
 ## Todos [x] type support for "list" and "dict"
+
+## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.1.4/noderedpy/_property.py` & `nodered.py-0.2.0/noderedpy/_property.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.4/noderedpy/decorator.py` & `nodered.py-0.2.0/noderedpy/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from typing import List
 from types import MethodType
-from ._nodered import Node
+from ._nodered import RED, Node
 from ._property import Property
 from ._server import Server
 
 
 def register(name:str, category:str = "nodered_py", properties:List[Property] = []) -> MethodType:
     """
     Decorator to register Node function
@@ -17,12 +17,12 @@
     category: str, default nodered_py
         category of Node
     properties: List[noderedpy._property.Property]
         propertis of Node
     """
     def decorator(node_func:MethodType):
         node = Node(name if name.startswith("nodered-py") else f"nodered-py-{name}", category, properties, node_func)
-        Server.registered_nodes.append(node)
+        RED.registered_nodes.append(node)
 
         return node_func
     
     return decorator
```

### Comparing `nodered.py-0.1.4/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.0/noderedpy/node-red-starter/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -40,20 +40,21 @@
 
 
 // create express and node-red server
 const exapp = express();
 const RED_server = http.createServer(exapp);
 
 // set configs
+var editorTheme = JSON.parse(fs.readFileSync(path.join(__dirname, "editorTheme.json")))
+editorTheme["projects"] = {
+    enabled: false
+};
+
 let opts = {
-    editorTheme: {
-        projects: {
-            enabled: false
-        }
-    },
+    editorTheme: editorTheme,
     httpAdminRoot: args["admin_root"].startsWith("/") ? args["admin_root"] : `/${args["admin_root"]}`,
     httpNodeRoot: "/",
     flowFile: "noderedpy.json",
     userDir: args["user_dir"],
     paletteCategories: args["show_default_category"] == "true" ? args["user_category"].concat(["subflows", "common", "function", "network", "sequence", "parser", "storage"]) : args["user_category"]
 };
 // if (![ "None", "null", "" ].includes(args["admin_auth"])) {
```

### Comparing `nodered.py-0.1.4/noderedpy/templates/__init__.py` & `nodered.py-0.2.0/noderedpy/templates/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,18 +164,18 @@
         "{$properties_js_prepare}", "\n".join(properties_js_prepare)
     ).replace(
         "{$properties_js_cancel}", "\n".join(properties_js_cancel)
     ).replace(
         "{$properties_js_save}", "\n".join(properties_js_save)
     )
 
-def node_js(node:"noderedpy._nodered.Node", port:int) -> str:
+def node_js(node:"noderedpy._nodered.Node", cache_dir:str) -> str:
     with open(os.path.join(__path__[0], "template.js"), "r", encoding = "utf-8") as tr:
         tt = tr.read()
 
     return tt.replace(
         "{$node_name}", node.name
     ).replace(
         "{$node_properties}", str([ property.name for property in node.properties])
     ).replace(
-        "{$port}", str(port)
+        "{$cache_dir}", cache_dir
     )
```

### Comparing `nodered.py-0.1.4/noderedpy/templates/template.html` & `nodered.py-0.2.0/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.4/noderedpy/templates/template.js` & `nodered.py-0.2.0/noderedpy/templates/template.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,10 @@
+const fs = require("fs"),
+    path = require("path");
+
 let messageCache = {};
 
 module.exports = function(RED) {
     function fnNode(config) {
         var node = this;
         RED.nodes.createNode(this, config);
 
@@ -21,15 +24,15 @@
                 reqToSend = {
                     payload: message.req.payload,
                     body: message.req.body,
                     cookie: message.req.cookie,
                     header: {}
                 };
                 for (var idx = 0; idx < message.req.rawHeaders.length / 2; idx++) {
-                    reqToSend.header[message.req.rawHeaders[idx * 2]] = message.req.rawHeaders[idx * 2 + 1];
+                    reqToSend.header[message.req.rawHeaders[idx * 2]] = message.req.rawHeaders[idx * 2 + 1].replaceAll('"', "'");
                 }
 
                 message.req = reqToSend;
             }
             if (message.res != undefined && typeof(message.res) == "object") {
                 messageCache.res = message.res;
                 delete message.res;
@@ -48,53 +51,71 @@
 
             node.status({
                 fill: "green",
                 shape: "dot",
                 text: "Running"
             });
 
+            const inpFile = path.join("{$cache_dir}", "input.json");
+            const outFile = path.join("{$cache_dir}", "output.json");
+
+            // remove if outFile exists before run
+            if (fs.existsSync(outFile)) {
+                fs.unlinkSync(outFile);
+            }
+
+            // send inputs to python
+            fs.writeFileSync(inpFile, JSON.stringify({
+                name: "{$node_name}",
+                props: configToSend,
+                msg: message
+            }, null, "    "));
+
+            // wait until job done
+            var resp = null;
+            while (true) {
+                if (fs.existsSync(outFile)) {
+                    try {
+                        resp = JSON.parse(fs.readFileSync(outFile));
+                        fs.unlinkSync(outFile);
+                        break;
+                    } catch {
+                        continue;
+                    }
+                }
+            }
+
+            // get result ans parse
             try {
-                fetch("http://127.0.0.1:{$port}/nodes/{$node_name}", {
-                    method: "POST",
-                    headers: {
-                        "Content-Type": "application/json"
-                    },
-                    body: JSON.stringify({
-                        props: configToSend,
-                        msg: message
-                    })
-                }).then(async (resp) => {
-                    var message = await resp.json();
-                    const state = message.state;
-                    delete message.state;
-
-                    if (state == "success") {
-                        message._msgid = messageCache._msgid;
-                        if (messageCache.req != undefined) {
-                            message.req = messageCache.req;
-                        }
-                        if (messageCache.res != undefined) {
-                            message.res = messageCache.res;
-                        }
-
-                        node.send(message);
-                        node.status({
-                            fill: "green",
-                            shape: "dot",
-                            text: "Finished"
-                        });
-                    } else {
-                        node.error(message.message);
-                        node.status({
-                            fill: "red",
-                            shape: "dot",
-                            text: "Stopped, see debug panel"
-                        });
+                const state = resp.state;
+                delete resp.state;
+
+                if (state == "success") {
+                    resp._msgid = messageCache._msgid;
+                    if (messageCache.req != undefined) {
+                        resp.req = messageCache.req;
                     }
-                });
+                    if (messageCache.res != undefined) {
+                        resp.res = messageCache.res;
+                    }
+
+                    node.send(resp);
+                    node.status({
+                        fill: "green",
+                        shape: "dot",
+                        text: "Finished"
+                    });
+                } else {
+                    node.error(resp.message);
+                    node.status({
+                        fill: "red",
+                        shape: "dot",
+                        text: "Stopped, see debug panel"
+                    });
+                }
             } catch (err) {
                 node.error(err.message);
                 node.status({
                     fill: "red",
                     shape: "dot",
                     text: "Stopped, see debug panel"
                 });
```

### Comparing `nodered.py-0.1.4/setup.py` & `nodered.py-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     setup_requires = requires,
     license = "MIT license",
     description = "make python function to Node-RED node",
     long_description = readme,
     long_description_content_type = "text/markdown",
     # package informations
     packages = [
-        "noderedpy", "noderedpy/templates", "noderedpy/node-red-starter"
+        "noderedpy", "noderedpy/assets", "noderedpy/templates", "noderedpy/node-red-starter"
     ],
     package_data = {
         "": [
-            "*.html", "*.js", "*.json"
+            "*.png", "*.html", "*.js", "*.json"
         ]
     },
     include_package_data = True,
     zip_safe = True
 )
```

