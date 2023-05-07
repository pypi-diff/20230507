# Comparing `tmp/replit-bot-4.2.8.tar.gz` & `tmp/replit-bot-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-bot-4.2.8.tar", max compression
+gzip compressed data, was "replit-bot-4.2.9.tar", max compression
```

## Comparing `replit-bot-4.2.8.tar` & `replit-bot-4.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.8/LICENSE
--rw-r--r--   0        0        0      839 2023-04-20 23:00:56.576167 replit-bot-4.2.8/pyproject.toml
--rw-r--r--   0        0        0    35912 2023-04-20 20:25:44.561475 replit-bot-4.2.8/replit_bot/AsyncBot.py
--rw-r--r--   0        0        0    50447 2023-04-20 20:25:44.953474 replit-bot-4.2.8/replit_bot/AsyncClient.py
--rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.8/replit_bot/AsyncPost_ql.py
--rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.8/replit_bot/LICENSE
--rw-r--r--   0        0        0      292 2023-04-20 23:00:05.964239 replit-bot-4.2.8/replit_bot/__init__.py
--rw-r--r--   0        0        0    18805 2023-04-17 02:54:25.529892 replit-bot-4.2.8/replit_bot/bot.py
--rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.8/replit_bot/client.py
--rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.8/replit_bot/colors.py
--rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.8/replit_bot/exceptions.py
--rw-r--r--   0        0        0      978 2023-04-20 20:25:44.157476 replit-bot-4.2.8/replit_bot/html_default_templates.py
--rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.8/replit_bot/links.py
--rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.8/replit_bot/param.py
--rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.8/replit_bot/post_ql.py
--rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.8/replit_bot/queries.js
--rw-r--r--   0        0        0    67496 2023-04-20 20:31:20.332886 replit-bot-4.2.8/replit_bot/queries.py
--rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.8/replit_bot/templates/index.html
--rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.8/replit_bot/utils/EventEmitter.py
--rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.8/replit_bot/utils/JSDict.py
--rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.8/replit_bot/utils/_uuid.py
--rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.8/replit_bot/utils/lines.py
--rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.8/replit_bot/utils/switch.py
--rw-r--r--   0        0        0      848 2023-04-20 23:01:00.531428 replit-bot-4.2.8/setup.py
--rw-r--r--   0        0        0      713 2023-04-20 23:01:00.531971 replit-bot-4.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.9/LICENSE
+-rw-r--r--   0        0        0      839 2023-04-21 04:36:12.622444 replit-bot-4.2.9/pyproject.toml
+-rw-r--r--   0        0        0    35912 2023-04-20 20:25:44.561475 replit-bot-4.2.9/replit_bot/AsyncBot.py
+-rw-r--r--   0        0        0    50438 2023-04-20 23:34:14.489365 replit-bot-4.2.9/replit_bot/AsyncClient.py
+-rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.9/replit_bot/AsyncPost_ql.py
+-rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.9/replit_bot/LICENSE
+-rw-r--r--   0        0        0      292 2023-04-21 04:36:16.002441 replit-bot-4.2.9/replit_bot/__init__.py
+-rw-r--r--   0        0        0    18805 2023-04-17 02:54:25.529892 replit-bot-4.2.9/replit_bot/bot.py
+-rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.9/replit_bot/client.py
+-rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.9/replit_bot/colors.py
+-rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.9/replit_bot/exceptions.py
+-rw-r--r--   0        0        0      977 2023-04-20 23:35:12.893283 replit-bot-4.2.9/replit_bot/html_default_templates.py
+-rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.9/replit_bot/links.py
+-rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.9/replit_bot/param.py
+-rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.9/replit_bot/post_ql.py
+-rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.9/replit_bot/queries.js
+-rw-r--r--   0        0        0    67496 2023-04-20 20:31:20.332886 replit-bot-4.2.9/replit_bot/queries.py
+-rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.9/replit_bot/templates/index.html
+-rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.9/replit_bot/utils/EventEmitter.py
+-rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.9/replit_bot/utils/JSDict.py
+-rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.9/replit_bot/utils/_uuid.py
+-rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.9/replit_bot/utils/lines.py
+-rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.9/replit_bot/utils/switch.py
+-rw-r--r--   0        0        0      848 2023-04-21 04:36:53.029708 replit-bot-4.2.9/setup.py
+-rw-r--r--   0        0        0      713 2023-04-21 04:36:53.039652 replit-bot-4.2.9/PKG-INFO
```

### Comparing `replit-bot-4.2.8/LICENSE` & `replit-bot-4.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/pyproject.toml` & `replit-bot-4.2.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit-bot"
-version = "4.2.8"
+version = "4.2.9"
 description = "make discord.py like bots on replit and/or do replapi-it style replit interactions"
 authors = ["bigminboss <you@example.com>"]
 
 [tool.poetry.dependencies]
 # python ver
 python = ">=3.7,<4.0.0"
 # replit db I think I can't remember lol
```

### Comparing `replit-bot-4.2.8/replit_bot/AsyncBot.py` & `replit-bot-4.2.9/replit_bot/AsyncBot.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/AsyncClient.py` & `replit-bot-4.2.9/replit_bot/AsyncClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -869,15 +869,15 @@
     async def setFollowing(self, should_follow: bool = True) -> bool:
         """follow a user and return whether they are following you"""
         res = await self.c.gql(
             "follow",
             vars={
                 "input": {
                     "targetUserId": self.id,
-                    "shouldFollow": should_follow and True,
+                    "shouldFollow": should_follow,
                 }
             },
         )
         if res["setFollowing"]:
             return False
         await self.update(res["setFollowing"]["targetUser"])
         return self.isFollowedBycurrentUser
```

### Comparing `replit-bot-4.2.8/replit_bot/AsyncPost_ql.py` & `replit-bot-4.2.9/replit_bot/AsyncPost_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/LICENSE` & `replit-bot-4.2.9/replit_bot/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/bot.py` & `replit-bot-4.2.9/replit_bot/bot.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/client.py` & `replit-bot-4.2.9/replit_bot/client.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/html_default_templates.py` & `replit-bot-4.2.9/replit_bot/html_default_templates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Some html templates. Will convert to jina and add to replit-bot/templates/ later"""
 
-ORIGINAL_HTML = """<center><h1>Commands are as followed</h1></center>
+ORIGINAL_HTML = """<center><h1>Commands are as follows</h1></center>
 <pre><code>@{} {}command-here param1:here param2:here</code></pre>
 <hr><center><h1>Commands</h1></center>{}<hr>"""
 
 HTML_LIST = """<li>{}</li>
 <ul>
     <li>Description: <em style="color: red; background: black">{}</em></li>
     <li>required = {}</li>
```

### Comparing `replit-bot-4.2.8/replit_bot/param.py` & `replit-bot-4.2.9/replit_bot/param.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/post_ql.py` & `replit-bot-4.2.9/replit_bot/post_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/queries.js` & `replit-bot-4.2.9/replit_bot/queries.js`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/queries.py` & `replit-bot-4.2.9/replit_bot/queries.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/utils/EventEmitter.py` & `replit-bot-4.2.9/replit_bot/utils/EventEmitter.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/replit_bot/utils/lines.py` & `replit-bot-4.2.9/replit_bot/utils/lines.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.8/setup.py` & `replit-bot-4.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'replit>=3.2.4,<4.0.0',
  'requests>=2.28.1,<3.0.0',
  'uvloop>=0.17.0,<0.18.0',
  'waitress>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'replit-bot',
-    'version': '4.2.8',
+    'version': '4.2.9',
     'description': 'make discord.py like bots on replit and/or do replapi-it style replit interactions',
     'long_description': None,
     'author': 'bigminboss',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `replit-bot-4.2.8/PKG-INFO` & `replit-bot-4.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-bot
-Version: 4.2.8
+Version: 4.2.9
 Summary: make discord.py like bots on replit and/or do replapi-it style replit interactions
 Author: bigminboss
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

