# Comparing `tmp/selfcord.py-0.1.2.tar.gz` & `tmp/selfcord.py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.2.tar", last modified: Sat Apr 29 00:33:42 2023, max compression
+gzip compressed data, was "selfcord.py-0.1.3.tar", last modified: Sat May  6 21:57:31 2023, max compression
```

## Comparing `selfcord.py-0.1.2.tar` & `selfcord.py-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.681921 selfcord.py-0.1.2/
--rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-04-29 00:33:42.681921 selfcord.py-0.1.2/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)     2259 2023-04-24 19:11:53.000000 selfcord.py-0.1.2/README.md
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.665254 selfcord.py-0.1.2/selfcord/
--rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.1.2/selfcord/__init__.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.668587 selfcord.py-0.1.2/selfcord/api/
--rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.1.2/selfcord/api/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.1.2/selfcord/api/errors.py
--rw-r--r--   0 shell     (1000) shell     (1001)     9183 2023-04-27 18:19:43.000000 selfcord.py-0.1.2/selfcord/api/events.py
--rw-r--r--   0 shell     (1000) shell     (1001)    16788 2023-04-27 16:47:37.000000 selfcord.py-0.1.2/selfcord/api/gateway.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7975 2023-04-27 16:53:31.000000 selfcord.py-0.1.2/selfcord/api/http.py
--rw-r--r--   0 shell     (1000) shell     (1001)    17139 2023-04-28 02:03:57.000000 selfcord.py-0.1.2/selfcord/bot.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.678588 selfcord.py-0.1.2/selfcord/models/
--rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.1.2/selfcord/models/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    16677 2023-04-29 00:12:51.000000 selfcord.py-0.1.2/selfcord/models/channel.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1052 2023-04-27 15:34:24.000000 selfcord.py-0.1.2/selfcord/models/client.py
--rw-r--r--   0 shell     (1000) shell     (1001)      901 2023-04-27 15:34:29.000000 selfcord.py-0.1.2/selfcord/models/emoji.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7323 2023-04-28 16:04:21.000000 selfcord.py-0.1.2/selfcord/models/guild.py
--rw-r--r--   0 shell     (1000) shell     (1001)      933 2023-04-27 15:34:49.000000 selfcord.py-0.1.2/selfcord/models/member.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2698 2023-04-29 00:23:26.000000 selfcord.py-0.1.2/selfcord/models/message.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2130 2023-04-27 15:35:57.000000 selfcord.py-0.1.2/selfcord/models/permission.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1556 2023-04-27 15:36:19.000000 selfcord.py-0.1.2/selfcord/models/role.py
--rw-r--r--   0 shell     (1000) shell     (1001)     3898 2023-04-27 19:15:13.000000 selfcord.py-0.1.2/selfcord/models/user.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1331 2023-04-27 15:44:13.000000 selfcord.py-0.1.2/selfcord/models/webhook.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.678588 selfcord.py-0.1.2/selfcord/utils/
--rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.1.2/selfcord/utils/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    15588 2023-04-29 00:32:36.000000 selfcord.py-0.1.2/selfcord/utils/command.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.668587 selfcord.py-0.1.2/selfcord.py.egg-info/
--rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)      710 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       65 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-04-29 00:33:42.681921 selfcord.py-0.1.2/setup.cfg
--rw-r--r--   0 shell     (1000) shell     (1001)     1004 2023-04-29 00:33:34.000000 selfcord.py-0.1.2/setup.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.678588 selfcord.py-0.1.2/tests/
--rw-r--r--   0 shell     (1000) shell     (1001)      455 2023-04-27 00:48:03.000000 selfcord.py-0.1.2/tests/test_commands.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.341505 selfcord.py-0.1.3/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-05-06 21:57:31.338171 selfcord.py-0.1.3/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)     2259 2023-04-24 19:11:53.000000 selfcord.py-0.1.3/README.md
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.288169 selfcord.py-0.1.3/selfcord/
+-rw-r--r--   0 shell     (1000) shell     (1001)       80 2023-05-01 21:22:28.000000 selfcord.py-0.1.3/selfcord/__init__.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.308170 selfcord.py-0.1.3/selfcord/api/
+-rw-r--r--   0 shell     (1000) shell     (1001)       86 2023-05-04 18:44:24.000000 selfcord.py-0.1.3/selfcord/api/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      562 2023-05-01 21:29:31.000000 selfcord.py-0.1.3/selfcord/api/errors.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    11532 2023-05-05 15:18:43.000000 selfcord.py-0.1.3/selfcord/api/events.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    18766 2023-05-04 18:21:11.000000 selfcord.py-0.1.3/selfcord/api/gateway.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     8009 2023-05-02 22:11:22.000000 selfcord.py-0.1.3/selfcord/api/http.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      496 2023-05-05 15:18:26.000000 selfcord.py-0.1.3/selfcord/api/voice.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    17999 2023-05-04 23:52:27.000000 selfcord.py-0.1.3/selfcord/bot.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.331504 selfcord.py-0.1.3/selfcord/models/
+-rw-r--r--   0 shell     (1000) shell     (1001)      353 2023-05-01 18:43:46.000000 selfcord.py-0.1.3/selfcord/models/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    17143 2023-05-04 23:13:01.000000 selfcord.py-0.1.3/selfcord/models/channel.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1086 2023-05-01 21:28:53.000000 selfcord.py-0.1.3/selfcord/models/client.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      935 2023-05-01 21:28:45.000000 selfcord.py-0.1.3/selfcord/models/emoji.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7587 2023-05-04 18:10:43.000000 selfcord.py-0.1.3/selfcord/models/guild.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      967 2023-05-01 21:28:32.000000 selfcord.py-0.1.3/selfcord/models/member.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2733 2023-05-01 21:28:28.000000 selfcord.py-0.1.3/selfcord/models/message.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2164 2023-05-01 21:28:21.000000 selfcord.py-0.1.3/selfcord/models/permission.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1591 2023-05-01 21:28:16.000000 selfcord.py-0.1.3/selfcord/models/role.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     3933 2023-05-01 21:28:11.000000 selfcord.py-0.1.3/selfcord/models/user.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1367 2023-05-01 21:28:06.000000 selfcord.py-0.1.3/selfcord/models/webhook.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.334838 selfcord.py-0.1.3/selfcord/utils/
+-rw-r--r--   0 shell     (1000) shell     (1001)      106 2023-05-01 18:43:35.000000 selfcord.py-0.1.3/selfcord/utils/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    15665 2023-05-04 23:46:51.000000 selfcord.py-0.1.3/selfcord/utils/command.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.291502 selfcord.py-0.1.3/selfcord.py.egg-info/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)      732 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       65 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-05-06 21:57:31.000000 selfcord.py-0.1.3/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-05-06 21:57:31.341505 selfcord.py-0.1.3/setup.cfg
+-rw-r--r--   0 shell     (1000) shell     (1001)     1004 2023-05-06 21:57:14.000000 selfcord.py-0.1.3/setup.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-06 21:57:31.334838 selfcord.py-0.1.3/tests/
+-rw-r--r--   0 shell     (1000) shell     (1001)      455 2023-04-27 00:48:03.000000 selfcord.py-0.1.3/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.2/PKG-INFO` & `selfcord.py-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
```

### Comparing `selfcord.py-0.1.2/README.md` & `selfcord.py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.2/selfcord/api/gateway.py` & `selfcord.py-0.1.3/selfcord/api/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import asyncio
 import websockets
 from aioconsole import aprint
 import json
 import time
 import zlib
 from .events import EventHandler
@@ -274,15 +275,14 @@
         self.last_send = time.perf_counter()
         self.latency = float('inf')
         self.alive = False
 
     async def recv_msg(self):
         '''
         Receives Message from gateway, encodes as json and does things depending on op code
-
         '''
         item = await self.ws.recv()
         buffer = bytearray()
         buffer.extend(item)
         if len(item) < 4 or item[-4:] != self.zlib_suffix: return
 
         if item:
@@ -478,16 +478,16 @@
                 await aprint('Shutting down...')
                 await self.close()
             except Exception as e:
                 error = "".join(format_exception(e, e, e.__traceback__))
                 await self.bot.emit("error", error)
                 await self.close()
 
-    async def ring(self, channel: str, guild=None):
-        """Initiates a discord call
+    async def video_call(self, channel: str, guild=None):
+        """Initiates a discord video call
 
         Args:
             channel (str): Channel ID
             guild (str, optional): Guild ID. Defaults to None.
         """
         payload = {
             "op": 4,
@@ -497,15 +497,79 @@
                 "preferred_region": "rotterdam",
                 "self_mute": False,
                 "self_deaf": False,
                 "self_video": True,
             }
         }
         await self.send_json(payload)
-        await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+        if guild == None:
+            await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+
+
+    async def call(self, channel: str, guild=None):
+        """Initiates a discord call
+
+        Args:
+            channel (str): Channel ID
+            guild (str, optional): Guild ID. Defaults to None.
+        """
+        payload = {
+            "op": 4,
+            "d": {
+                "guild_id": guild,
+                "channel_id": channel,
+                "preferred_region": "rotterdam",
+                "self_mute": False,
+                "self_deaf": False,
+                "self_video": False,
+            }
+        }
+        await self.send_json(payload)
+        if guild == None:
+            await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+
+
+    async def stream_call(self, channel: str, guild=None):
+        """Initiates a discord stream call
+
+        Args:
+            channel (str): Channel ID
+            guild (str, optional): Guild ID. Defaults to None.
+        """
+        type = "guild" if guild != None else "call"
+        payload = {
+            "op": 18,
+            "d": {
+                "guild_id": guild,
+                "channel_id": channel,
+                "preferred_region": "rotterdam",
+                "type": type
+            }
+        }
+        await self.send_json(payload)
+        if guild == None:
+            await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+
+            payload = {
+                "op": 22,
+                "d": {
+                    "stream_key": f"call:{channel}:{self.user.id}",
+                    "paused": False
+                }
+            }
+        else:
+            payload = {
+                "op": 22,
+                "d": {
+                    "stream_key": f"guild:{guild}:{channel}:{self.user.id}",
+                    "paused": False
+                }
+            }
+
+        await self.send_json(payload)
 
 
 
 
     async def leave_call(self):
         """Leaves a discord call
         """
```

### Comparing `selfcord.py-0.1.2/selfcord/api/http.py` & `selfcord.py-0.1.3/selfcord/api/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+from __future__ import annotations
 from aiohttp import ClientSession
 from aioconsole import aprint
 import asyncio
 from base64 import b64encode
 import aiohttp
 from selfcord.api.errors import LoginFailure
 import random
 from ..models import User, Client
 
 class http:
     def __init__(self) -> None:
         xproperties = ['eyJvcyI6IldpbmRvd3MiLCJicm93c2VyIjoiRmlyZWZveCIsImRldmljZSI6IiIsInN5c3RlbV9sb2NhbGUiOiJmciIsImJyb3dzZXJfdXNlcl9hZ2VudCI6Ik1vemlsbGEvNS4wIChXaW5kb3dzIE5UIDEwLjA7IFdpbjY0OyB4NjQ7IHJ2OjEwMi4wKSBHZWNrby8yMDEwMDEwMSBGaXJlZm94LzEwMi4wIiwiYnJvd3Nlcl92ZXJzaW9uIjoiMTAyLjAiLCJvc192ZXJzaW9uIjoiMTAiLCJyZWZlcnJlciI6IiIsInJlZmVycmluZ19kb21haW4iOiIiLCJyZWZlcnJlcl9jdXJyZW50IjoiIiwicmVmZXJyaW5nX2RvbWFpbl9jdXJyZW50IjoiIiwicmVsZWFzZV9jaGFubmVsIjoic3RhYmxlIiwiY2xpZW50X2J1aWxkX251bWJlciI6MTU0MTg2LCJjbGllbnRfZXZlbnRfc291cmNlIjpudWxsfQ==', 'eyJvcyI6IkxpbnV4IiwiYnJvd3NlciI6IkRpc2NvcmQgQ2xpZW50IiwicmVsZWFzZV9jaGFubmVsIjoiY2FuYXJ5IiwiY2xpZW50X3ZlcnNpb24iOiIwLjAuMTQwIiwib3NfdmVyc2lvbiI6IjUuMTkuMC0zLXJ0MTAtTUFOSkFSTyIsIm9zX2FyY2giOiJ4NjQiLCJzeXN0ZW1fbG9jYWxlIjoiZW4tR0IiLCJ3aW5kb3dfbWFuYWdlciI6IktERSx1bmtub3duIiwiZGlzdHJvIjoiXCJNYW5qYXJvIExpbnV4XCIiLCJjbGllbnRfYnVpbGRfbnVtYmVyIjoxNTQyMTYsImNsaWVudF9ldmVudF9zb3VyY2UiOm51bGx9', 'eyJvcyI6IkxpbnV4IiwiYnJvd3NlciI6IkNocm9tZSIsImRldmljZSI6IiIsInN5c3RlbV9sb2NhbGUiOiJlbi1HQiIsImJyb3dzZXJfdXNlcl9hZ2VudCI6Ik1vemlsbGEvNS4wIChYMTE7IExpbnV4IHg4Nl82NCkgQXBwbGVXZWJLaXQvNTM3LjM2IChLSFRNTCwgbGlrZSBHZWNrbykgQ2hyb21lLzEwNi4wLjAuMCBTYWZhcmkvNTM3LjM2IiwiYnJvd3Nlcl92ZXJzaW9uIjoiMTA2LjAuMC4wIiwib3NfdmVyc2lvbiI6IiIsInJlZmVycmVyIjoiaHR0cHM6Ly93d3cucm9ibG94LmNvbS8iLCJyZWZlcnJpbmdfZG9tYWluIjoid3d3LnJvYmxveC5jb20iLCJyZWZlcnJlcl9jdXJyZW50IjoiIiwicmVmZXJyaW5nX2RvbWFpbl9jdXJyZW50IjoiIiwicmVsZWFzZV9jaGFubmVsIjoic3RhYmxlIiwiY2xpZW50X2J1aWxkX251bWJlciI6MTU0MTg2LCJjbGllbnRfZXZlbnRfc291cmNlIjpudWxsfQ==']
-
         self.cookies        = {}
         self.token          = None
         self.xproperties    = random.choice(xproperties)
         self.base_url       = 'https://discord.com/api/v9'
 
     async def static_login(self, token: str):
         '''Used to retrieve basic token information
@@ -155,11 +155,11 @@
 
         Returns:
             str: The b64 payload
         """
         async with ClientSession() as session:
             async with session.get(f'{url}') as resp:
                 image = b64encode(await resp.read())
-                newobj = str(image).split('"', 2)
+                newobj = str(image).split("'", 2)
 
         return f'data:image/png;base64,{newobj[1]}'
```

### Comparing `selfcord.py-0.1.2/selfcord/bot.py` & `selfcord.py-0.1.3/selfcord/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import asyncio
 import json
 from .api import gateway, http, Activity
 import inspect
 from .models import Client, TextChannel, GroupChannel, DMChannel, VoiceChannel, Guild, User
 from collections import defaultdict
 from aioconsole import aprint, aexec
@@ -13,26 +14,28 @@
 import io
 from functools import partial
 import importlib
 import aiohttp
 
 
 class Bot:
-    def __init__(self, show_beat: bool = False, prefixes: list = ["s!"], inbuilt_help=True) -> None:
+    def __init__(self, show_beat: bool = False, prefixes: list = ["s!"], inbuilt_help=True, userbot=False, eval=False) -> None:
         self.inbuilt_help= inbuilt_help
         self.show_beat = show_beat
         self.token = None
         self.http = http()
         self.t1 = time.perf_counter()
         self.gateway = gateway(self.http, self.show_beat)
         self._events = defaultdict(list)
         self.commands = CommandCollection()
         self.prefixes = prefixes if isinstance(prefixes, list) else [prefixes]
         self.extensions = ExtensionCollection()
         self.user = None
+        self.eval = eval
+        self.userbot = userbot
 
 
     def run(self, token: str):
         """Used to start connection to gateway as well as gather user information
 
         Args:
             token (str): _description_
@@ -129,36 +132,36 @@
 
                                     msg += f"```"
                                     return await ctx.reply(f"{msg}")
 
 
 
 
+        if self.eval:
+            def clean_code(content):
+                if content.startswith("```") and content.endswith("```"):
+                    return "\n".join(content.split("\n")[1:])[:-3]
+                else:
+                    return content
 
-        def clean_code(content):
-            if content.startswith("```") and content.endswith("```"):
-                return "\n".join(content.split("\n")[1:])[:-3]
-            else:
-                return content
+            @self.cmd(description="Executes and runs code", aliases=['exec'])
+            async def eval(ctx, *, code: str):
+                """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution.
+                """
+                code = clean_code(code)
 
-        @self.cmd(description="Executes and runs code", aliases=['exec'])
-        async def eval(ctx, *, code: str):
-            """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution.
-            """
-            code = clean_code(code)
-
-            try:
-                with contextlib.redirect_stdout(io.StringIO()) as f:
-                    await aexec(code)
-                    result = f"```{f.getvalue()}\n```"
-            except Exception as e:
-                error = "".join(format_exception(e, e, e.__traceback__))
-                result = f"```\n{error}```"
+                try:
+                    with contextlib.redirect_stdout(io.StringIO()) as f:
+                        await aexec(code)
+                        result = f"```{f.getvalue()}\n```"
+                except Exception as e:
+                    error = "".join(format_exception(e, e, e.__traceback__))
+                    result = f"```\n{error}```"
 
-            await ctx.reply(result)
+                await ctx.reply(result)
 
     def on(self, event: str):
         """Decorator for events
 
         Args:
             event (str): The event to check for
         """
@@ -339,15 +342,15 @@
         Returns:
             Guild: The Guild object
         """
         for guild in self.user.guilds:
             if guild.id == guild_id:
                 return guild
 
-    async def get_user(self, user_id: str):
+    async def get_user(self, user_id: str) -> User:
         """
         Function to retrieve user data. Probably need to be friends with them to retrieve the details.
 
         Args:
             user_id (Str): ID of the other user.
 
         Returns:
@@ -356,24 +359,32 @@
         """
 
         data = await self.http.request(method="get", endpoint=f"/users/{user_id}")
 
         user = User(data, bot=self, http=self.http)
         return user
 
+    async def create_guild(self, name: str, icon_url: str = None, template: str = "2TffvPucqHkN"):
+        """Creates a guild
+        """
+        image = await self.http.encode_image(icon_url)
+        await self.http.request(method="post", endpoint=f"/guilds", headers={"origin": "https://discord.com", "referer": "https://discord.com/channels/@me"}, json={"name": name, "icon": image, "template": template })
+
+
     async def add_friend(self, user_id: str):
         """
-        Function to add random user as a friend.
+        Function to add a specific user as a friend.
 
         Args:
             user_id (str): ID of the possible random user.
 
         Returns:
             No return value.
         """
+
         await self.http.request(method="put", endpoint=f"/users/@me/relationships/{user_id}",
                                 headers={"origin": "https://discord.com",
                                          "referer": f"https://discord.com/channels/@me/{random.choice(self.user.private_channels).id}"},
                                 json={})
 
     async def edit_profile(self, bio: str = None, accent: int = None):
         """ Edits user profile
@@ -432,25 +443,32 @@
             async with session.post(f"https://canary.discord.com/api/v9/entitlements/gift-codes/{code}/redeem", headers={"authorization": f"{self.token}", "user-agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/112.0", "content-type":"application/json"}, json={}) as resp:
                 j = await resp.json()
                 await aprint(j, resp.status)
 
 
 
 
-    async def change_hypesquad(self, house: str):
+    async def change_hypesquad(self, house: "str"):
         """Helper function to change hypesquad
 
         Args:
             house (str): Hypesquad name
         """
         if house.lower() == "bravery":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 1})
         if house.lower() == "brilliance":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 2})
         if house.lower() == "balance":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 3})
 
     async def change_presence(self, status: str, afk: bool, activity: dict):
+        """Change discord activity presence
+
+        Args:
+            status (str): Online, Offline, Dnd, Invisible
+            afk (bool): True or False
+            activity (dict): Selfcord.Activity method.
+        """
         await self.gateway.change_presence(status, afk, activity=activity)
```

### Comparing `selfcord.py-0.1.2/selfcord/models/channel.py` & `selfcord.py-0.1.3/selfcord/models/channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
+from __future__ import annotations
 from .message import Message
 import time
 from .user import User
 from .webhook import Webhook
 import asyncio
 
 from selfcord.models import message
 
 
-
-
-
-
 class Messageable:
     """Parent class specific for those classes that include a textchat for sending messages.
     """
     def __init__(self, http, bot) -> None:
         self.http = http
         self.bot = bot
 
@@ -141,14 +138,60 @@
                                     json={"content": content, "tts": tts,
                                         "message_reference": {"channel_id": f"{self.id}", "message_id": f"{message.id}"},
                                         "allowed_mentions": {"parse": ["users", "roles", "everyone"],
                                                             "replied_user": False}})
         return Message(resp, self.bot, self.http)
 
 
+class Voiceable(Messageable):
+    """Parent class specific for those classes that include a voice chat, or call functionality
+    """
+    def __init__(self, http, bot) -> None:
+        super().__init__(http, bot)
+        self.http = http
+        self.bot = bot
+
+    async def video_call(self):
+        """Initiates a video call on the specified channel
+        """
+        if hasattr(self, "guild_id"):
+            await self.bot.gateway.video_call(self.id, self.guild_id)
+        else:
+            await self.bot.gateway.video_call(self.id)
+
+    async def stream_call(self):
+        """Initiates a stream call on the specified channel
+        """
+        if hasattr(self, "guild_id"):
+            await self.bot.gateway.stream_call(self.id, self.guild_id)
+        else:
+            await self.bot.gateway.stream_call(self.id)
+
+    async def call(self):
+        """Initiates a call on the specified channel
+        """
+
+        if hasattr(self, "guild_id"):
+
+            await self.bot.gateway.call(self.id, self.guild_id)
+        else:
+            await self.bot.gateway.call(self.id)
+
+
+    async def leave_call(self):
+        """Leaves call on the specified channel
+        """
+        await self.bot.gateway.leave_call()
+
+
+
+
+
+
+
 
 
 
 class TextChannel(Messageable):
     """
     Text Channel Object
         Represents a Guild/Server channel within Discord.
@@ -283,15 +326,15 @@
             fields['avatar'] = data
         data = await self.http.request(method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields)
         webhook = Webhook(data, self.bot, http=self.http)
         self.webhooks.append(webhook)
         return webhook
 
 
-class VoiceChannel(Messageable):
+class VoiceChannel(Voiceable, Messageable):
     """Voice Channel Object
     """
 
     def __init__(self, data, bot, http) -> None:
         super().__init__(http, bot)
         self.permissions = []
         self.webhooks = []
@@ -350,23 +393,15 @@
             data = await self.http.encode_image(avatar_url)
             fields['avatar'] = data
         data = await self.http.request(method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields)
         webhook = Webhook(data, self.bot, self.http)
         self.webhooks.append(webhook)
         return webhook
 
-    async def call(self):
-        """Initiates a call on the specified channel
-        """
-        await self.bot.gateway.ring(self.id, self.guild_id)
 
-    async def leave(self):
-        """Leaves call on the specified channel
-        """
-        await self.bot.gateway.leave_call()
 
 
 class Category:
     """Category Object
     """
 
     def __init__(self, data, bot, http) -> None:
@@ -393,15 +428,15 @@
     async def delete(self):
         """Deletes the Category object.
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
 
 
-class DMChannel(Messageable):
+class DMChannel(Voiceable, Messageable):
     """DM Channel Object
     """
 
     def __init__(self, data, bot, http) -> None:
         super().__init__(http, bot)
         self.http = http
         self.bot = bot
@@ -423,26 +458,18 @@
 
     async def delete(self):
         """Deletes the DM Channel object.
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}?silent=false")
         del self
 
-    async def call(self):
-        """Initiates the call on the specified channel
-        """
-        await self.bot.gateway.ring(self.id)
 
-    async def leave(self):
-        """Leaves the call on the specified channel
-        """
-        await self.bot.gateway.leave_call()
 
 
-class GroupChannel(Messageable):
+class GroupChannel(Voiceable, Messageable):
     """Group Channel Object
     """
 
     def __init__(self, data, bot, http) -> None:
         super().__init__(http, bot)
         self.recipients = []
         self.http = http
@@ -469,17 +496,8 @@
 
     async def delete(self):
         """Deletes the Group Channel Object
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}?silent=true")
         del self
 
-    async def call(self):
-        """Initiates the call on the specified channel
-        """
-        await self.bot.gateway.ring(self.id)
-
-    async def leave(self):
-        """Leaves the call on the specified channel
-        """
-        await self.bot.gateway.leave_call()
```

### Comparing `selfcord.py-0.1.2/selfcord/models/client.py` & `selfcord.py-0.1.3/selfcord/models/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from __future__ import annotations
 
 class Client:
     """Client Object
     """
     def __init__(self, UserPayload: dict) -> None:
 
         self.guilds = []
```

### Comparing `selfcord.py-0.1.2/selfcord/models/emoji.py` & `selfcord.py-0.1.3/selfcord/models/emoji.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from __future__ import annotations
 
 class Emoji:
     """Emoji Object
     """
     def __init__(self, data, bot, http) -> None:
         self.bot = bot
         self.http = http
```

### Comparing `selfcord.py-0.1.2/selfcord/models/guild.py` & `selfcord.py-0.1.3/selfcord/models/guild.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from .user import User
 from .channel import TextChannel, VoiceChannel, Category
 from .role import Role
 from .emoji import Emoji
 from itertools import zip_longest
 from aiohttp import ClientSession
 from base64 import b64encode
@@ -58,31 +59,36 @@
 
                 self.members.append(user)
 
             if channel != None:
                 type = channel.get("type")
                 if type == self.TEXTCHANNEL:
                     channel = TextChannel(channel, self.bot, self.http)
+                    channel.guild_id = self.id
                     self.channels.append(channel)
                 elif type == self.VOICECHANNEL:
                     channel = VoiceChannel(channel, self.bot, self.http)
+                    channel.guild_id = self.id
                     self.channels.append(channel)
                 elif type == self.CATEGORY:
                     channel = Category(channel, self.bot, self.http)
+                    channel.guild_id = self.id
                     self.channels.append(channel)
                 else:
                     channel = TextChannel(channel, self.bot, self.http)
+                    channel.guild_id = self.id
                     self.channels.append(channel)
 
             if role != None:
                 role = Role(role, self.http, guild_id = self.id)
                 self.roles.append(role)
 
             if emoji != None:
                 emoji = Emoji(emoji, self.bot, self.http)
+                emoji.guild_id = self.id
                 self.emojis.append(emoji)
 
     async def ban(self, user_id: str):
         """Bans a user from the guild
 
         Args:
             user_id (str): User ID specified to ban
```

### Comparing `selfcord.py-0.1.2/selfcord/models/member.py` & `selfcord.py-0.1.3/selfcord/models/member.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from __future__ import annotations
 
 class Member:
     """Member Object
     """
     def __init__(self, UserPayload: dict) -> None:
         self.roles = []
```

### Comparing `selfcord.py-0.1.2/selfcord/models/message.py` & `selfcord.py-0.1.3/selfcord/models/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from .user import User
 import asyncio
 import urllib
 
 class Message:
     """Message Object
     """
```

### Comparing `selfcord.py-0.1.2/selfcord/models/permission.py` & `selfcord.py-0.1.3/selfcord/models/permission.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from __future__ import annotations
 class Permission:
     """Permission Object
     """
 
     def __init__(self, data) -> None:
         self.perms = {
             "CREATE_INSTANT_INVITE": 0x1,
```

### Comparing `selfcord.py-0.1.2/selfcord/models/role.py` & `selfcord.py-0.1.3/selfcord/models/role.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from .permission import Permission
 
 class Role:
     """Role Object
     """
     def __init__(self, data: dict, http, **kwargs) -> None:
         self.guild_id = kwargs.get("guild_id")
```

### Comparing `selfcord.py-0.1.2/selfcord/models/user.py` & `selfcord.py-0.1.3/selfcord/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from __future__ import annotations
 from base64 import b64encode
 import datetime
 
 
 class Profile:
     def __init__(self, UserPayload: dict, bot, http) -> None:
         self.bot = bot
@@ -111,14 +111,15 @@
 
 
     async def create_dm(self):
         """Create a dm for the user
         """
         await self.http.request(method="post", endpoint="/users/@me/channels", json={"recipients": [self.id]})
 
+
     async def get_profile(self) -> Profile:
         """Get the User profile
 
         Returns:
             Profile: The User Profile object
         """
         data = await self.http.request(method="get", endpoint=f"/users/{self.id}/profile?with_mutual_guilds=true")
```

### Comparing `selfcord.py-0.1.2/selfcord/models/webhook.py` & `selfcord.py-0.1.3/selfcord/models/webhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 class Webhook:
     def __init__(self, data: dict, bot, http) -> None:
         self.http = http
         self.bot = bot
         self._update(data)
 
     def _update(self, data):
```

### Comparing `selfcord.py-0.1.2/selfcord/utils/command.py` & `selfcord.py-0.1.3/selfcord/utils/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from __future__ import annotations
 import inspect
 import re
 from collections import defaultdict
 
 
 class Extension:
     """Extension object. Discord.py equivalent of cogs, a helper system to help manage and organise code into multiple files
@@ -291,14 +291,16 @@
         if not inspect.iscoroutinefunction(coro):
             raise RuntimeWarning("Not an async function!")
         else:
 
 
             cmd = Command(name=name, description=description, aliases=aliases, func=coro, ext=cls)
             cls.commands.add(cmd)
+
+
 class Context:
     """Context related for commands, and invocation
     """
     def __init__(self, bot, message, http) -> None:
         self.bot = bot
         self.message = message
         self.http = http
@@ -459,16 +461,17 @@
 
 
     async def invoke(self):
         """Used to actually run the command
         """
         if self.command is None:
             return
-        if self.message.author.id != self.bot.user.id:
-            return
+        if not self.bot.userbot:
+            if self.message.author.id != self.bot.user.id:
+                return
         if self.command_content != None:
             args, kwargs = await self.get_arguments()
             func = self.command.func
             if func.__code__.co_varnames[0] == "self":
 
                 args.insert(0, self.extension)
                 args.insert(1, self)
```

### Comparing `selfcord.py-0.1.2/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.1.3/selfcord.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
```

### Comparing `selfcord.py-0.1.2/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.3/selfcord.py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 selfcord.py.egg-info/requires.txt
 selfcord.py.egg-info/top_level.txt
 selfcord/api/__init__.py
 selfcord/api/errors.py
 selfcord/api/events.py
 selfcord/api/gateway.py
 selfcord/api/http.py
+selfcord/api/voice.py
 selfcord/models/__init__.py
 selfcord/models/channel.py
 selfcord/models/client.py
 selfcord/models/emoji.py
 selfcord/models/guild.py
 selfcord/models/member.py
 selfcord/models/message.py
```

### Comparing `selfcord.py-0.1.2/setup.py` & `selfcord.py-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
     this_directory = Path(__file__).parent
     long_description = ( this_directory /"README.md").read_text()
     setup(
         name="selfcord.py",
         packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models']),
-        version="0.1.2",
+        version="0.1.3",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell of OMEGA",
         license="MIT",
         install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "requests"],
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
```

