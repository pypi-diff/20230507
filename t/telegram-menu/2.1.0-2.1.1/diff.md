# Comparing `tmp/telegram_menu-2.1.0.tar.gz` & `tmp/telegram_menu-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_menu-2.1.0.tar", last modified: Sun May  7 12:03:14 2023, max compression
+gzip compressed data, was "telegram_menu-2.1.1.tar", last modified: Sun May  7 20:37:10 2023, max compression
```

## Comparing `telegram_menu-2.1.0.tar` & `telegram_menu-2.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/
--rw-rw-rw-   0        0        0    35823 2021-12-12 22:30:43.000000 telegram_menu-2.1.0/LICENSE
--rw-rw-rw-   0        0        0       43 2021-12-12 22:30:43.000000 telegram_menu-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7259 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6458 2023-05-07 00:10:58.000000 telegram_menu-2.1.0/README.md
--rw-rw-rw-   0        0        0      102 2023-05-07 00:11:47.000000 telegram_menu-2.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1357 2022-01-16 20:03:45.000000 telegram_menu-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:03:14.430229 telegram_menu-2.1.0/telegram_menu/
--rw-rw-rw-   0        0        0     1008 2023-02-20 21:30:49.000000 telegram_menu-2.1.0/telegram_menu/__init__.py
--rw-rw-rw-   0        0        0     1139 2023-05-07 12:00:53.000000 telegram_menu-2.1.0/telegram_menu/_version.py
--rw-rw-rw-   0        0        0    10601 2023-05-06 04:59:21.000000 telegram_menu-2.1.0/telegram_menu/models.py
--rw-rw-rw-   0        0        0    29959 2023-05-06 05:27:34.000000 telegram_menu-2.1.0/telegram_menu/navigation.py
--rw-rw-rw-   0        0        0       63 2023-02-20 21:36:29.000000 telegram_menu-2.1.0/telegram_menu/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/telegram_menu.egg-info/
--rw-rw-rw-   0        0        0     7259 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-06 22:45:49.000000 telegram_menu-2.1.0/telegram_menu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       97 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/tests/
--rw-rw-rw-   0        0        0      713 2023-02-20 21:40:17.000000 telegram_menu-2.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1321 2023-02-20 21:30:49.000000 telegram_menu-2.1.0/tests/demo.py
--rw-rw-rw-   0        0        0    20855 2023-05-06 05:12:04.000000 telegram_menu-2.1.0/tests/test_connection.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/
+-rw-rw-rw-   0        0        0    35823 2021-12-12 22:30:43.000000 telegram_menu-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0       43 2021-12-12 22:30:43.000000 telegram_menu-2.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7259 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6458 2023-05-07 00:10:58.000000 telegram_menu-2.1.1/README.md
+-rw-rw-rw-   0        0        0      102 2023-05-07 20:32:35.000000 telegram_menu-2.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2022-01-16 20:03:45.000000 telegram_menu-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:37:10.962821 telegram_menu-2.1.1/telegram_menu/
+-rw-rw-rw-   0        0        0     1008 2023-02-20 21:30:49.000000 telegram_menu-2.1.1/telegram_menu/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-05-07 20:33:52.000000 telegram_menu-2.1.1/telegram_menu/_version.py
+-rw-rw-rw-   0        0        0    10601 2023-05-06 04:59:21.000000 telegram_menu-2.1.1/telegram_menu/models.py
+-rw-rw-rw-   0        0        0    30013 2023-05-07 20:32:17.000000 telegram_menu-2.1.1/telegram_menu/navigation.py
+-rw-rw-rw-   0        0        0       63 2023-02-20 21:36:29.000000 telegram_menu-2.1.1/telegram_menu/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/telegram_menu.egg-info/
+-rw-rw-rw-   0        0        0     7259 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-06 22:45:49.000000 telegram_menu-2.1.1/telegram_menu.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       97 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/tests/
+-rw-rw-rw-   0        0        0      713 2023-02-20 21:40:17.000000 telegram_menu-2.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1321 2023-02-20 21:30:49.000000 telegram_menu-2.1.1/tests/demo.py
+-rw-rw-rw-   0        0        0    20858 2023-05-07 20:33:23.000000 telegram_menu-2.1.1/tests/test_connection.py
```

### Comparing `telegram_menu-2.1.0/LICENSE` & `telegram_menu-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.0/PKG-INFO` & `telegram_menu-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram_menu
-Version: 2.1.0
+Version: 2.1.1
 Summary: A python library to generate navigation menus using Telegram Bot API.
 Home-page: https://github.com/mevellea/telegram_menu
 Author: Armel Mevellec
 Author-email: mevellea@gmail.com
 License: GNU GPLv3
 Keywords: telegram
 Platform: any
```

### Comparing `telegram_menu-2.1.0/README.md` & `telegram_menu-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.0/setup.py` & `telegram_menu-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.0/telegram_menu/__init__.py` & `telegram_menu-2.1.1/telegram_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.0/telegram_menu/_version.py` & `telegram_menu-2.1.1/telegram_menu/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 
 """Package description."""
 
 __title__ = "telegram_menu"
 __description__ = "A python library to generate navigation menus using Telegram Bot API."
 __url__ = "https://github.com/mevellea/telegram_menu"
 __raw_url__ = "https://raw.githubusercontent.com/mevellea/telegram_menu/master"
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 __author__ = "Armel Mevellec"
 __author_email__ = "mevellea@gmail.com"
 __license__ = "GNU GPLv3"
 __copyright__ = "Copyright 2020-2023 " + __author__
```

### Comparing `telegram_menu-2.1.0/telegram_menu/models.py` & `telegram_menu-2.1.1/telegram_menu/models.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.0/telegram_menu/navigation.py` & `telegram_menu-2.1.1/telegram_menu/navigation.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
                 menu_message.picture, notification=menu_message.notification, keyboard=keyboard, caption=content
             )
         else:
             message = await self.send_message(content, keyboard, notification=menu_message.notification)
         if message is None:
             return -1  # message was not sent, abort
         menu_message.is_alive()
+        menu_message.message_id = message.message_id
         self._menu_queue.append(menu_message)
         return message.message_id
 
     async def goto_home(self, context: Optional[CallbackContext[BT, UD, CD, BD]] = None) -> int:
         """Go to home menu, empty menu_queue."""
         if not self._menu_queue:
             return -1
```

### Comparing `telegram_menu-2.1.0/telegram_menu.egg-info/PKG-INFO` & `telegram_menu-2.1.1/telegram_menu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-menu
-Version: 2.1.0
+Version: 2.1.1
 Summary: A python library to generate navigation menus using Telegram Bot API.
 Home-page: https://github.com/mevellea/telegram_menu
 Author: Armel Mevellec
 Author-email: mevellea@gmail.com
 License: GNU GPLv3
 Keywords: telegram
 Platform: any
```

### Comparing `telegram_menu-2.1.0/tests/__init__.py` & `telegram_menu-2.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.0/tests/demo.py` & `telegram_menu-2.1.1/tests/demo.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.0/tests/test_connection.py` & `telegram_menu-2.1.1/tests/test_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
         # try broadcasting a message to all opened sessions
         msg_h = await Test.session.broadcast_message("Broadcast message")
         self.assertIsInstance(msg_h[0], Message)
 
         # select 'Action' menu from home, check that level is still 'Home' since flag 'home_after' is True
         msg_home = await _navigation.select_menu_button("Action")
-        self.assertEqual(msg_home, -1)
+        self.assertNotEqual(msg_home, -1)
         await asyncio.sleep(0.5)
 
         await self.go_check_id(label="Home", expected_id=msg_home)
 
         # Open second menu and check that message id has increased
         msg_menu2_id = await _navigation.select_menu_button("Second menu")
         self.assertGreater(msg_menu2_id, 1)
```

