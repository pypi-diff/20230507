# Comparing `tmp/discord-qalib-2.2.2.tar.gz` & `tmp/discord-qalib-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.2.2.tar", last modified: Fri May  5 16:45:39 2023, max compression
+gzip compressed data, was "discord-qalib-2.2.3.tar", last modified: Sun May  7 14:12:19 2023, max compression
```

## Comparing `discord-qalib-2.2.2.tar` & `discord-qalib-2.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.025977 discord-qalib-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-05 16:45:39.025977 discord-qalib-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.021977 discord-qalib-2.2.2/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-05 16:45:25.000000 discord-qalib-2.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.021977 discord-qalib-2.2.2/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-05 16:45:25.000000 discord-qalib-2.2.2/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.021977 discord-qalib-2.2.2/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.025977 discord-qalib-2.2.2/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/templater.py
--rw-r--r--   0 runner    (1001) docker     (123)    30812 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:45:39.025977 discord-qalib-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 16:45:25.000000 discord-qalib-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.407762 discord-qalib-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-07 14:12:19.407762 discord-qalib-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.403762 discord-qalib-2.2.3/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 14:12:19.000000 discord-qalib-2.2.3/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-07 14:12:09.000000 discord-qalib-2.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.403762 discord-qalib-2.2.3/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-07 14:12:09.000000 discord-qalib-2.2.3/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.403762 discord-qalib-2.2.3/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:12:19.407762 discord-qalib-2.2.3/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/templater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30812 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 14:11:55.000000 discord-qalib-2.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 14:12:19.407762 discord-qalib-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-07 14:12:09.000000 discord-qalib-2.2.3/setup.py
```

### Comparing `discord-qalib-2.2.2/LICENSE` & `discord-qalib-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/PKG-INFO` & `discord-qalib-2.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.2.2
+Version: 2.2.3
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
@@ -94,15 +94,15 @@
             <author>
                 <name>Test Author</name>
                 <icon>https://cdn.discordapp.com/embed/avatars/0.png</icon>
                 <url>https://discordapp.com</url>
             </author>
         </embed>
         <view>
-            <components>        
+            <components>
                 <button key="understood_button">
                     <label>Understood</label>
                     <style>success</style>
                 </button>
             </components>
         </view>
     </message>
@@ -121,14 +121,15 @@
 import qalib
 from qalib.template_engines import formatter
 
 bot = commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
 
 Messages = Literal["test_key"]
 
+
 async def acknowledged(interaction: discord.Interaction):
     await interaction.response.send_message("Acknowledged", ephemeral=True)
 
 
 @bot.command()
 @qalib.qalib_context(formatter.Formatter(), "templates/test.xml")
 async def test(ctx: qalib.QalibContext[Messages]):
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.2 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.3 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.2.2/README.md` & `discord-qalib-2.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             <author>
                 <name>Test Author</name>
                 <icon>https://cdn.discordapp.com/embed/avatars/0.png</icon>
                 <url>https://discordapp.com</url>
             </author>
         </embed>
         <view>
-            <components>        
+            <components>
                 <button key="understood_button">
                     <label>Understood</label>
                     <style>success</style>
                 </button>
             </components>
         </view>
     </message>
@@ -104,14 +104,15 @@
 import qalib
 from qalib.template_engines import formatter
 
 bot = commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
 
 Messages = Literal["test_key"]
 
+
 async def acknowledged(interaction: discord.Interaction):
     await interaction.response.send_message("Acknowledged", ephemeral=True)
 
 
 @bot.command()
 @qalib.qalib_context(formatter.Formatter(), "templates/test.xml")
 async def test(ctx: qalib.QalibContext[Messages]):
```

### Comparing `discord-qalib-2.2.2/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.2.3/discord_qalib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.2.2
+Version: 2.2.3
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
@@ -94,15 +94,15 @@
             <author>
                 <name>Test Author</name>
                 <icon>https://cdn.discordapp.com/embed/avatars/0.png</icon>
                 <url>https://discordapp.com</url>
             </author>
         </embed>
         <view>
-            <components>        
+            <components>
                 <button key="understood_button">
                     <label>Understood</label>
                     <style>success</style>
                 </button>
             </components>
         </view>
     </message>
@@ -121,14 +121,15 @@
 import qalib
 from qalib.template_engines import formatter
 
 bot = commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
 
 Messages = Literal["test_key"]
 
+
 async def acknowledged(interaction: discord.Interaction):
     await interaction.response.send_message("Acknowledged", ephemeral=True)
 
 
 @bot.command()
 @qalib.qalib_context(formatter.Formatter(), "templates/test.xml")
 async def test(ctx: qalib.QalibContext[Messages]):
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.2 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.3 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.2.2/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.2.3/discord_qalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/pyproject.toml` & `discord-qalib-2.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.2.2"
+version = "2.2.3"
 authors = [
     { name = "YousefEZ", email = "syberprojects@gmail.com" },
 ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.poetry]
 name = "discord-qalib"
-version = "2.2.2"
+version = "2.2.3"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
```

### Comparing `discord-qalib-2.2.2/qalib/__init__.py` & `discord-qalib-2.2.3/qalib/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,23 +11,21 @@
 
 import discord
 from discord.ext import commands
 
 from .context import QalibContext
 from .interaction import QalibInteraction
 from .renderer import Renderer, RenderingOptions
-from .template_engines.formatter import Formatter
-from .template_engines.jinja2 import Jinja2
 from .template_engines.template_engine import TemplateEngine
 
 __title__ = "qalib"
 __author__ = "YousefEZ"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present YousefEZ"
-__version__ = "2.2.2"
+__version__ = "2.2.3"
 
 T = TypeVar("T")
 Coro = Coroutine[Any, Any, T]
 
 
 def qalib_context(
         template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
```

### Comparing `discord-qalib-2.2.2/qalib/context.py` & `discord-qalib-2.2.3/qalib/context.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/interaction.py` & `discord-qalib-2.2.3/qalib/interaction.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/renderer.py` & `discord-qalib-2.2.3/qalib/renderer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/template_engines/formatter.py` & `discord-qalib-2.2.3/qalib/template_engines/formatter.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/translators/__init__.py` & `discord-qalib-2.2.3/qalib/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/translators/deserializer.py` & `discord-qalib-2.2.3/qalib/translators/deserializer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/translators/factory.py` & `discord-qalib-2.2.3/qalib/translators/factory.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/translators/json.py` & `discord-qalib-2.2.3/qalib/translators/json.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/translators/message_parsing.py` & `discord-qalib-2.2.3/qalib/translators/message_parsing.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/translators/templater.py` & `discord-qalib-2.2.3/qalib/translators/templater.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/qalib/translators/xml.py` & `discord-qalib-2.2.3/qalib/translators/xml.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.2/setup.py` & `discord-qalib-2.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 setup(
     name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.2.2",
+    version="2.2.3",
     description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
     license="MIT",
     python_requires=">=3.8.0",
     install_requires=requirements,
     package_data={"qalib": ["py.typed"]},
 )
```

