# Comparing `tmp/ooliver_botbase-2.0.1.tar.gz` & `tmp/ooliver_botbase-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooliver_botbase-2.0.1.tar", max compression
+gzip compressed data, was "ooliver_botbase-2.0.2.tar", max compression
```

## Comparing `ooliver_botbase-2.0.1.tar` & `ooliver_botbase-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      144 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/README.md
--rw-r--r--   0        0        0      275 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/__init__.py
--rw-r--r--   0        0        0    13364 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/botbase.py
--rw-r--r--   0        0        0       73 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/db/__init__.py
--rw-r--r--   0        0        0      625 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/db/blacklist.py
--rw-r--r--   0        0        0      727 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/db/commands.py
--rw-r--r--   0        0        0      364 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/db/metadata.py
--rw-r--r--   0        0        0     6064 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/exts/blacklist.py
--rw-r--r--   0        0        0     1343 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/exts/log_commands.py
--rw-r--r--   0        0        0     1637 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/exts/log_guilds.py
--rw-r--r--   0        0        0      288 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/models.py
--rw-r--r--   0        0        0        1 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/py.typed
--rw-r--r--   0        0        0      309 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/wraps/__init__.py
--rw-r--r--   0        0        0      590 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/wraps/channel.py
--rw-r--r--   0        0        0     1391 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/wraps/inter.py
--rw-r--r--   0        0        0      253 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/botbase/wraps/member.py
--rw-r--r--   0        0        0      253 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/botbase/wraps/thread.py
--rw-r--r--   0        0        0      245 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/botbase/wraps/user.py
--rw-r--r--   0        0        0     4398 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/botbase/wraps/wrap.py
--rw-r--r--   0        0        0      800 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 ooliver_botbase-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/README.md
+-rw-r--r--   0        0        0      275 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/__init__.py
+-rw-r--r--   0        0        0    13364 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/botbase.py
+-rw-r--r--   0        0        0       73 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/db/__init__.py
+-rw-r--r--   0        0        0      625 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/db/blacklist.py
+-rw-r--r--   0        0        0      727 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/db/commands.py
+-rw-r--r--   0        0        0      364 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/db/metadata.py
+-rw-r--r--   0        0        0     6064 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/exts/blacklist.py
+-rw-r--r--   0        0        0     1343 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/exts/log_commands.py
+-rw-r--r--   0        0        0     1758 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/exts/log_guilds.py
+-rw-r--r--   0        0        0      288 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/models.py
+-rw-r--r--   0        0        0        1 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/py.typed
+-rw-r--r--   0        0        0      309 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/channel.py
+-rw-r--r--   0        0        0     1391 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/inter.py
+-rw-r--r--   0        0        0      253 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/member.py
+-rw-r--r--   0        0        0      253 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/thread.py
+-rw-r--r--   0        0        0      245 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/user.py
+-rw-r--r--   0        0        0     4398 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/wrap.py
+-rw-r--r--   0        0        0      800 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 ooliver_botbase-2.0.2/PKG-INFO
```

### Comparing `ooliver_botbase-2.0.1/botbase/botbase.py` & `ooliver_botbase-2.0.2/botbase/botbase.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.1/botbase/db/blacklist.py` & `ooliver_botbase-2.0.2/botbase/db/blacklist.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.1/botbase/db/commands.py` & `ooliver_botbase-2.0.2/botbase/db/commands.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.1/botbase/exts/blacklist.py` & `ooliver_botbase-2.0.2/botbase/exts/blacklist.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.1/botbase/exts/log_commands.py` & `ooliver_botbase-2.0.2/botbase/exts/log_commands.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.1/botbase/exts/log_guilds.py` & `ooliver_botbase-2.0.2/botbase/exts/log_guilds.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ..models import CogBase
 
 if TYPE_CHECKING:
     from nextcord import Guild
 
 
 class GuildLogging(CogBase[BotBase]):
+    @CogBase.listener()
     async def on_guild_join(self, guild: Guild):
         if not self.bot.log_channel:
             return
 
         assert guild.owner_id is not None
 
         embed = Embed(
@@ -29,16 +30,20 @@
         members: `{guild.member_count}`
         owner: `{guild.owner or await self.bot.fetch_user(guild.owner_id)}`
 
         """
             ),
             color=self.bot.colour,
         )
-        await self.get_channel(self.log_channel).send(embed=embed)  # type: ignore
+        try:
+            await self.bot.get_channel(self.bot.log_channel).send(embed=embed)  # type: ignore
+        except AttributeError:
+            pass
 
+    @CogBase.listener()
     async def on_guild_remove(self, guild: Guild):
         if guild.unavailable:
             return
 
         if not self.bot.log_channel:
             return
```

### Comparing `ooliver_botbase-2.0.1/botbase/wraps/channel.py` & `ooliver_botbase-2.0.2/botbase/wraps/channel.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.1/botbase/wraps/inter.py` & `ooliver_botbase-2.0.2/botbase/wraps/inter.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.1/botbase/wraps/wrap.py` & `ooliver_botbase-2.0.2/botbase/wraps/wrap.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.1/pyproject.toml` & `ooliver_botbase-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ooliver-botbase"
-version = "2.0.1"
+version = "2.0.2"
 description = "A personal nextcord bot base package for bots."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 repository = "https://github.com/ooliver1/botbase"
 packages = [{ include = "botbase" }]
 readme = "README.md"
```

### Comparing `ooliver_botbase-2.0.1/PKG-INFO` & `ooliver_botbase-2.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooliver-botbase
-Version: 2.0.1
+Version: 2.0.2
 Summary: A personal nextcord bot base package for bots.
 Home-page: https://github.com/ooliver1/botbase
 License: MIT
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

