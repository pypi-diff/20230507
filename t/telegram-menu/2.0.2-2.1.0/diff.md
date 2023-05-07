# Comparing `tmp/telegram_menu-2.0.2.tar.gz` & `tmp/telegram_menu-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_menu-2.0.2.tar", last modified: Sun Feb 12 22:25:16 2023, max compression
+gzip compressed data, was "telegram_menu-2.1.0.tar", last modified: Sun May  7 12:03:14 2023, max compression
```

## Comparing `telegram_menu-2.0.2.tar` & `telegram_menu-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 22:25:16.078967 telegram_menu-2.0.2/
--rw-rw-rw-   0        0        0    35823 2021-12-12 22:30:43.000000 telegram_menu-2.0.2/LICENSE
--rw-rw-rw-   0        0        0       43 2021-12-12 22:30:43.000000 telegram_menu-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7146 2023-02-12 22:25:16.077959 telegram_menu-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6349 2023-01-16 22:16:39.000000 telegram_menu-2.0.2/README.md
--rw-rw-rw-   0        0        0      102 2023-02-10 17:27:19.000000 telegram_menu-2.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-12 22:25:16.078967 telegram_menu-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1357 2022-01-16 20:03:45.000000 telegram_menu-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 22:25:16.052876 telegram_menu-2.0.2/telegram_menu/
--rw-rw-rw-   0        0        0      381 2023-01-16 22:16:39.000000 telegram_menu-2.0.2/telegram_menu/__init__.py
--rw-rw-rw-   0        0        0      512 2023-02-12 22:15:38.000000 telegram_menu-2.0.2/telegram_menu/_version.py
--rw-rw-rw-   0        0        0     9227 2023-02-11 23:14:00.000000 telegram_menu-2.0.2/telegram_menu/models.py
--rw-rw-rw-   0        0        0    27379 2023-02-11 23:24:27.000000 telegram_menu-2.0.2/telegram_menu/navigation.py
--rw-rw-rw-   0        0        0        0 2021-12-12 22:30:43.000000 telegram_menu-2.0.2/telegram_menu/py.typed
-drwxrwxrwx   0        0        0        0 2023-02-12 22:25:16.074497 telegram_menu-2.0.2/telegram_menu.egg-info/
--rw-rw-rw-   0        0        0     7146 2023-02-12 22:25:15.000000 telegram_menu-2.0.2/telegram_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-02-12 22:25:15.000000 telegram_menu-2.0.2/telegram_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 22:25:15.000000 telegram_menu-2.0.2/telegram_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-06 22:45:49.000000 telegram_menu-2.0.2/telegram_menu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       97 2023-02-12 22:25:15.000000 telegram_menu-2.0.2/telegram_menu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-02-12 22:25:15.000000 telegram_menu-2.0.2/telegram_menu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-12 22:25:16.076905 telegram_menu-2.0.2/tests/
--rw-rw-rw-   0        0        0       61 2021-12-12 22:30:43.000000 telegram_menu-2.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      669 2023-02-11 23:48:03.000000 telegram_menu-2.0.2/tests/demo.py
--rw-rw-rw-   0        0        0    20164 2023-02-11 23:48:32.000000 telegram_menu-2.0.2/tests/test_connection.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/
+-rw-rw-rw-   0        0        0    35823 2021-12-12 22:30:43.000000 telegram_menu-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2021-12-12 22:30:43.000000 telegram_menu-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7259 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6458 2023-05-07 00:10:58.000000 telegram_menu-2.1.0/README.md
+-rw-rw-rw-   0        0        0      102 2023-05-07 00:11:47.000000 telegram_menu-2.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2022-01-16 20:03:45.000000 telegram_menu-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:03:14.430229 telegram_menu-2.1.0/telegram_menu/
+-rw-rw-rw-   0        0        0     1008 2023-02-20 21:30:49.000000 telegram_menu-2.1.0/telegram_menu/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-05-07 12:00:53.000000 telegram_menu-2.1.0/telegram_menu/_version.py
+-rw-rw-rw-   0        0        0    10601 2023-05-06 04:59:21.000000 telegram_menu-2.1.0/telegram_menu/models.py
+-rw-rw-rw-   0        0        0    29959 2023-05-06 05:27:34.000000 telegram_menu-2.1.0/telegram_menu/navigation.py
+-rw-rw-rw-   0        0        0       63 2023-02-20 21:36:29.000000 telegram_menu-2.1.0/telegram_menu/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/telegram_menu.egg-info/
+-rw-rw-rw-   0        0        0     7259 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-06 22:45:49.000000 telegram_menu-2.1.0/telegram_menu.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       97 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-07 12:03:14.000000 telegram_menu-2.1.0/telegram_menu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 12:03:14.445855 telegram_menu-2.1.0/tests/
+-rw-rw-rw-   0        0        0      713 2023-02-20 21:40:17.000000 telegram_menu-2.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1321 2023-02-20 21:30:49.000000 telegram_menu-2.1.0/tests/demo.py
+-rw-rw-rw-   0        0        0    20855 2023-05-06 05:12:04.000000 telegram_menu-2.1.0/tests/test_connection.py
```

### Comparing `telegram_menu-2.0.2/LICENSE` & `telegram_menu-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.0.2/PKG-INFO` & `telegram_menu-2.1.0/telegram_menu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: telegram_menu
-Version: 2.0.2
+Name: telegram-menu
+Version: 2.1.0
 Summary: A python library to generate navigation menus using Telegram Bot API.
 Home-page: https://github.com/mevellea/telegram_menu
 Author: Armel Mevellec
 Author-email: mevellea@gmail.com
 License: GNU GPLv3
 Keywords: telegram
 Platform: any
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # telegram_menu package
 
-<img src="https://img.shields.io/badge/python-3.7-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.8-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.9-blue.svg" alt="drawing"/>
+<img src="https://img.shields.io/badge/python-3.7-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.11-blue.svg" alt="drawing"/>
 <br/>
 A python library to generate navigation menus using Telegram Bot API.
 
 Features:
 
 * Menu navigation using tree structure, unlimited depth
 * Support for sending pictures (local file or url), stickers, notifications, webapps and polls
@@ -164,7 +164,16 @@
 
 <img src="https://raw.githubusercontent.com/mevellea/telegram_menu/master/resources/classes.png" width="800"/>
 
 [navigation.py]: https://github.com/mevellea/telegram_menu/blob/master/telegram_menu/navigation.py
 [models.py]: https://github.com/mevellea/telegram_menu/blob/master/telegram_menu/models.py
 [create a Telegram bot]: https://github.com/python-telegram-bot/python-telegram-bot/wiki/Introduction-to-the-API
 [Demo: TelegramMenuSession]: https://raw.githubusercontent.com/mevellea/telegram_menu/master/resources/demo.gif
+
+## Unit-tests
+
+To execute the test suite, run the following command and then start a session from a Telegram client with the keyword **/start**.
+
+```bash
+python -m unittest
+```
+
```

### Comparing `telegram_menu-2.0.2/README.md` & `telegram_menu-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # telegram_menu package
 
-<img src="https://img.shields.io/badge/python-3.7-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.8-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.9-blue.svg" alt="drawing"/>
+<img src="https://img.shields.io/badge/python-3.7-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.11-blue.svg" alt="drawing"/>
 <br/>
 A python library to generate navigation menus using Telegram Bot API.
 
 Features:
 
 * Menu navigation using tree structure, unlimited depth
 * Support for sending pictures (local file or url), stickers, notifications, webapps and polls
@@ -143,7 +143,15 @@
 
 <img src="https://raw.githubusercontent.com/mevellea/telegram_menu/master/resources/classes.png" width="800"/>
 
 [navigation.py]: https://github.com/mevellea/telegram_menu/blob/master/telegram_menu/navigation.py
 [models.py]: https://github.com/mevellea/telegram_menu/blob/master/telegram_menu/models.py
 [create a Telegram bot]: https://github.com/python-telegram-bot/python-telegram-bot/wiki/Introduction-to-the-API
 [Demo: TelegramMenuSession]: https://raw.githubusercontent.com/mevellea/telegram_menu/master/resources/demo.gif
+
+## Unit-tests
+
+To execute the test suite, run the following command and then start a session from a Telegram client with the keyword **/start**.
+
+```bash
+python -m unittest
+```
```

### Comparing `telegram_menu-2.0.2/setup.py` & `telegram_menu-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.0.2/telegram_menu/models.py` & `telegram_menu-2.1.0/telegram_menu/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,87 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# pylint: disable=too-many-arguments
+#
+# Copyright 2020-2023 Armel Mevellec
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, version 3.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+# General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
+#
 
 """Messages and navigation models."""
 
+import asyncio
 import datetime
 import logging
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import TYPE_CHECKING, Any, Callable, Coroutine, List, Optional, Union
 
 import emoji
 import tzlocal
 import validators
 from telegram import InlineKeyboardButton, InlineKeyboardMarkup, KeyboardButton, ReplyKeyboardMarkup, WebAppInfo
+from telegram.ext._callbackcontext import CallbackContext
+from telegram.ext._utils.types import BD, BT, CD, UD
 
 if TYPE_CHECKING:
     from telegram_menu import NavigationHandler
 
 
 logger = logging.getLogger(__name__)
 
 TypeCallback = Optional[Union[Callable[..., Any], Coroutine[Any, Any, None], "BaseMessage"]]
 TypeKeyboard = List[List["MenuButton"]]
 
 
+async def call_function_EAFP(method: TypeCallback, par: Any, *args: Any, **kwargs: Any) -> Any:
+    """Call a function that could be a coroutine and could not accept an argument."""
+    if asyncio.iscoroutinefunction(method):
+        try:
+            return await method(*args, par, **kwargs)
+        except TypeError:
+            return await method(*args, **kwargs)
+    else:
+        try:
+            return method(*args, par, **kwargs)  # type: ignore
+        except TypeError:
+            return method(*args, **kwargs)  # type: ignore
+
+
 class ButtonType(Enum):
     """Button type enumeration."""
 
     NOTIFICATION = auto()
     MESSAGE = auto()
     PICTURE = auto()
     STICKER = auto()
     POLL = auto()
 
 
 @dataclass
 class MenuButton:
-    """
-    Base button class, wrapper for label with callback.
-
-    Parameters
-    ----------
-    label: button label
-    callback: method called on button selection
-    btype: button type
-    args: argument passed to the callback
-    notification: send notification to user
+    """Base button class, wrapper for label with callback.
 
+    Args:
+        label: button label
+        callback: method called on button selection
+        btype: button type
+        args: argument passed to the callback
+        notification: send notification to user
     """
 
     def __init__(
         self,
         label: str,
         callback: TypeCallback = None,
         btype: ButtonType = ButtonType.NOTIFICATION,
@@ -66,48 +94,49 @@
         self.callback = callback
         self.btype = btype
         self.args = args
         self.notification = notification
         self.web_app_url = web_app_url
 
 
-class BaseMessage(ABC):  # pylint: disable=too-many-instance-attributes
-    """
-    Base message class, buttons array and label updater.
-
-    Parameters
-    ----------
-    navigation: navigation manager
-    label: message label
-    expiry_period: duration before the message is deleted
-    inlined: create an inlined message instead of a menu message
-    home_after: go back to home menu after executing the action
-    notification: show a notification in Telegram interface
+class BaseMessage(ABC):
+    """Base message class, buttons array and label updater.
 
+    Args:
+        navigation: navigation manager
+        label: message label
+        picture: path of the picture to send. Leave None if no picure
+                 should be sent
+        expiry_period: duration before the message is deleted
+        inlined: create an inlined message instead of a menu message
+        home_after: go back to home menu after executing the action
+        notification: show a notification in Telegram interface
     """
 
     EXPIRING_DELAY = 12  # minutes
 
     time_alive: datetime.datetime
 
     def __init__(
         self,
         navigation: "NavigationHandler",
         label: str = "",
+        picture: str = "",
         expiry_period: Optional[datetime.timedelta] = None,
         inlined: bool = False,
         home_after: bool = False,
         notification: bool = True,
         input_field: str = "",
         **args: Any,
     ) -> None:
         """Init BaseMessage class."""
         self.keyboard: TypeKeyboard = [[]]
         self.label = emoji_replace(label)
         self.inlined = inlined
+        self.picture = picture
         self.notification = notification
         self.navigation = navigation
         self.input_field = input_field
 
         # previous values are used to check if it has changed, to skip sending identical message
         self.keyboard_previous: TypeKeyboard = [[]]
         self.content_previous: str = ""
@@ -121,53 +150,28 @@
             if isinstance(expiry_period, datetime.timedelta)
             else datetime.timedelta(minutes=self.EXPIRING_DELAY)
         )
 
         self._status = None
 
     @abstractmethod
-    def update(self) -> str:
-        """
-        Update message content.
-
-        Returns
-        -------
-        Message content formatted with HTML formatting.
-
-        """
+    def update(self, context: Optional[CallbackContext[BT, UD, CD, BD]] = None) -> str:
+        """Update message content with HTML formatting. It can be also implemented as a coroutine (async) method."""
         raise NotImplementedError
 
-    async def text_input(self, text: str) -> None:
-        """
-        Receive text from console.
-
-        If used, this function must be instantiated in the child class.
+    async def get_updated_content(self, context: Optional[CallbackContext[BT, UD, CD, BD]] = None) -> str:
+        """Update method that detects if update is a coroutine or not and calls it doing also the emoji replacement."""
+        v = await call_function_EAFP(self.update, context)
+        return emoji_replace(v) if v else v
 
-        Parameters
-        ----------
-        text: text received from console
-        """
+    async def text_input(self, text: str, context: Optional[CallbackContext[BT, UD, CD, BD]] = None) -> None:
+        """Receive text from console. If used, this function must be instantiated in the child class."""
 
     def get_button(self, label: str) -> Optional[MenuButton]:
-        """
-        Get button matching given label.
-
-        Parameters
-        ----------
-        label: message label
-
-        Returns
-        -------
-        Button matching label
-
-        Raises
-        ------
-        EnvironmentError: too many buttons matching label
-
-        """
+        """Get button matching given label."""
         return next(iter(y for x in self.keyboard for y in x if y.label == label), None)
 
     def add_button_back(self, **args: Any) -> None:
         """Add a button to go back to previous menu."""
         self.add_button(label="Back", callback=None, **args)
 
     def add_button_home(self, **args: Any) -> None:
@@ -180,27 +184,24 @@
         callback: TypeCallback = None,
         btype: ButtonType = ButtonType.NOTIFICATION,
         args: Any = None,
         notification: bool = True,
         new_row: bool = False,
         web_app_url: str = "",
     ) -> None:
-        """
-        Add a button to keyboard attribute.
-
-        Parameters
-        ----------
-        label: button label
-        callback: method called on button selection
-        btype: button type
-        args: argument passed to the callback
-        notification: send notification to user
-        new_row: add a new row
-        web_app_url: URL of the web-app
+        """Add a button to keyboard attribute.
 
+        Args:
+            label: button label
+            callback: method called on button selection
+            btype: button type
+            args: argument passed to the callback
+            notification: send notification to user
+            new_row: add a new row
+            web_app_url: URL of the web-app
         """
         # arrange buttons per row, depending on inlined property
         buttons_per_row = 2 if not self.inlined else 4
 
         if not isinstance(self.keyboard, list) or not self.keyboard:
             self.keyboard = [[]]
 
@@ -266,10 +267,10 @@
         logger.debug(f"Removing message '{self.label}' ({self.message_id})")
 
 
 def emoji_replace(label: str) -> str:
     """Replace emoji token with utf-16 code."""
     match_emoji = re.findall(r"(:\w+:)", label)
     for item in match_emoji:
-        emoji_str = emoji.emojize(item, language="alias")  # pylint: disable=unexpected-keyword-arg
+        emoji_str = emoji.emojize(item, language="alias")
         label = label.replace(item, emoji_str)
     return label
```

### Comparing `telegram_menu-2.0.2/telegram_menu/navigation.py` & `telegram_menu-2.1.0/telegram_menu/navigation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+#
+# Copyright 2020-2023 Armel Mevellec
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, version 3.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+# General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
+#
 
 """Telegram menu navigation."""
 
 from __future__ import annotations
 
 import asyncio
 import datetime
 import imghdr
 import logging
 import mimetypes
 from pathlib import Path
-from typing import Any, List, Optional, Type, Union
+from typing import Any, List, Optional, Sequence, Type, Union
 
 import telegram.ext
 import tzlocal
 import validators
 from apscheduler.schedulers.base import BaseScheduler
 from telegram import Bot, Chat, InlineKeyboardMarkup, Message, ReplyKeyboardMarkup, Update
+from telegram._utils.defaultvalue import DEFAULT_NONE
+from telegram._utils.types import ODVInput
 from telegram.constants import ChatAction, ParseMode
 from telegram.ext import Application, CallbackQueryHandler, CommandHandler, MessageHandler, PicklePersistence
 from telegram.ext._callbackcontext import CallbackContext
+from telegram.ext._utils.types import BD, BT, CD, UD
 
 from ._version import __raw_url__
-from .models import BaseMessage, ButtonType, TypeCallback, emoji_replace
+from .models import BaseMessage, ButtonType, TypeCallback, call_function_EAFP, emoji_replace
 
 logger = logging.getLogger(__name__)
 
 
 class NavigationException(Exception):
     """Base exception."""
 
@@ -36,28 +54,25 @@
     """Session manager, send start message to each new user connecting to the bot."""
 
     # delays in seconds
     READ_TIMEOUT = 6
     CONNECT_TIMEOUT = 7
     START_MESSAGE = "start"
 
-    def __init__(self, api_key: str, start_message: str = START_MESSAGE) -> None:
-        """
-        Initialize the session object.
-
-        Parameters
-        ----------
-        api_key: Telegram bot API key
-        start_message: text used to start a session, e.g. /start
+    def __init__(self, api_key: str, start_message: str = START_MESSAGE, persistence_path: str = "") -> None:
+        """Initialize the session object.
 
+        Args:
+            api_key: Telegram bot API key
+            start_message: text used to start a session, e.g. /start
         """
         if not isinstance(api_key, str):
             raise KeyError("API_KEY must be a string!")
 
-        persistence = PicklePersistence(filepath="arbitrarycallbackdatabot")
+        persistence = PicklePersistence(filepath=persistence_path if persistence_path else "arbitrarycallbackdatabot")
         self.application = (
             Application.builder().token(api_key).persistence(persistence).arbitrary_callback_data(True).build()
         )
         self.scheduler = self.application.job_queue.scheduler  # type: ignore
 
         self._api_key = api_key
         self.sessions: List[NavigationHandler] = []
@@ -77,24 +92,23 @@
 
     def start(
         self,
         start_message_class: Type[BaseMessage],
         start_message_args: Optional[List[Any]] = None,
         polling: bool = True,
         navigation_handler_class: Optional[Type[NavigationHandler]] = None,
+        stop_signals: ODVInput[Sequence[int]] = DEFAULT_NONE,
     ) -> None:
-        """
-        Set the start message and run the dispatcher.
+        """Set the start message and run the dispatcher.
 
-        Parameters
-        ----------
-        start_message_class: class used to create start message
-        start_message_args: optional arguments passed to the start class
-        polling: if True, start polling updates from Telegram
-        navigation_handler_class: optional class used to extend the base NavigationHandler
+        Args:
+            start_message_class: class used to create start message
+            start_message_args: optional arguments passed to the start class
+            polling: if True, start polling updates from Telegram
+            navigation_handler_class: optional class used to extend the base NavigationHandler
 
         """
         self.start_message_class = start_message_class
         self.start_message_args = start_message_args
         self.navigation_handler_class = navigation_handler_class or NavigationHandler
         if not issubclass(start_message_class, BaseMessage):
             raise NavigationException("start_message_class must be a BaseMessage!")
@@ -102,71 +116,71 @@
             raise NavigationException("start_message_args is not a list!")
         if not issubclass(self.navigation_handler_class, NavigationHandler):
             raise NavigationException("navigation_handler_class must be a NavigationHandler!")
 
         if not self.scheduler.running:
             self.scheduler.start()
         if polling:
-            self.application.run_polling()
+            self.application.run_polling(stop_signals=stop_signals)
 
-    async def _send_start_message(self, update: Update, _: Any) -> None:  # type: ignore
+    async def _send_start_message(self, update: Update, context: CallbackContext[BT, UD, CD, BD]) -> None:
         """Start main message, app choice."""
         chat = update.effective_chat
         if chat is None:
             raise NavigationException("Chat object was not created")
         if self.navigation_handler_class is None:
             raise NavigationException("Navigation Handler class not defined")
         session = self.navigation_handler_class(self.application.bot, chat, self.scheduler)
         self.sessions.append(session)
         if self.start_message_class is None:
             raise NavigationException("Message class not defined")
         if self.start_message_args is not None:
             start_message = self.start_message_class(session, message_args=self.start_message_args)
         else:
             start_message = self.start_message_class(session)
-        await session.goto_menu(start_message)
+        await session.goto_menu(start_message, context)
 
     def get_session(self, chat_id: int = 0) -> Optional[NavigationHandler]:
         """Get session from list."""
         sessions = [x for x in self.sessions if chat_id in (x.chat_id, 0)]
         if not sessions:
             return None
         return sessions[0]
 
-    async def _button_select_callback(self, update: Update, context: CallbackContext) -> None:  # type: ignore
+    async def _button_select_callback(self, update: Update, context: CallbackContext[BT, UD, CD, BD]) -> None:
         """Menu message main entry point."""
         if update.effective_chat is None or update.message is None:
             raise NavigationException("Chat object was not created")
         session = self.get_session(update.effective_chat.id)
         if session is None:
             await self._send_start_message(update, context)
             return
         if update.message.text:
-            await session.select_menu_button(update.message.text)
+            await session.select_menu_button(update.message.text, context)
 
-    async def _poll_answer(self, update: Update, _: CallbackContext) -> None:  # type: ignore
+    async def _poll_answer(self, update: Update, _: CallbackContext[BT, UD, CD, BD]) -> None:
         """Entry point for poll selection."""
         if update.effective_user is None or update.poll_answer is None:
             raise NavigationException("User object was not created")
         session = next((x for x in self.sessions if x.user_name == update.effective_user.first_name), None)
         if session:
             await session.poll_answer(update.poll_answer.option_ids[0])
 
-    async def _button_inline_select_callback(self, update: Update, context: CallbackContext) -> None:  # type: ignore
+    async def _button_inline_select_callback(self, update: Update, context: CallbackContext[BT, UD, CD, BD]) -> None:
         """Execute inline callback of an BaseMessage."""
         if update.effective_chat is None or update.callback_query is None:
             raise NavigationException("Chat object was not created")
         session = self.get_session(update.effective_chat.id)
         if session is None:
             await self._send_start_message(update, context)
             return
         if update.callback_query.data and update.callback_query.id:
-            await session.app_message_button_callback(update.callback_query.data, update.callback_query.id)
+            await session.app_message_button_callback(update.callback_query.data, update.callback_query.id, context)
 
-    async def _button_webapp_callback(self, update: Update, context: CallbackContext) -> None:  # type: ignore
+    async def _button_webapp_callback(self, update: Update, context: CallbackContext[BT, UD, CD, BD]) -> None:
         """Execute webapp callback."""
         if (
             update.effective_chat is None
             or update.effective_message is None
             or update.effective_message.web_app_data is None
         ):
             raise NavigationException("Chat object was not created")
@@ -175,15 +189,15 @@
             await self._send_start_message(update, context)
             return
         await session.app_message_webapp_callback(
             update.effective_message.web_app_data.data, update.effective_message.web_app_data.button_text
         )
 
     @staticmethod
-    async def _msg_error_handler(update: object, context: CallbackContext) -> None:  # type: ignore
+    async def _msg_error_handler(update: object, context: CallbackContext[BT, UD, CD, BD]) -> None:  # type: ignore
         """Log Errors caused by Updates."""
         if not isinstance(update, Update):
             raise NavigationException("Incorrect update object")
         error_message = str(context.error) if update is None else f"Update {update.update_id} - {str(context.error)}"
         logger.error(error_message)
 
     async def broadcast_message(self, message: str, notification: bool = True) -> List[telegram.Message]:
@@ -264,57 +278,77 @@
         """Delete a message, remove from queue."""
         message.kill_message()
         if message in self._message_queue:
             self._message_queue.remove(message)
             await self.delete_message(message.message_id)
         del message
 
-    async def goto_menu(self, menu_message: BaseMessage) -> int:
+    async def goto_menu(
+        self, menu_message: BaseMessage, context: Optional[CallbackContext[BT, UD, CD, BD]] = None
+    ) -> int:
         """Send menu message and add to queue."""
-        content = menu_message.update()
+        content = await menu_message.get_updated_content(context)
         logger.info(f"Opening menu {menu_message.label}")
         keyboard = menu_message.gen_keyboard_content()
-        message = await self.send_message(emoji_replace(content), keyboard, notification=menu_message.notification)
+        if menu_message.picture:
+            message = await self.send_photo(
+                menu_message.picture, notification=menu_message.notification, keyboard=keyboard, caption=content
+            )
+        else:
+            message = await self.send_message(content, keyboard, notification=menu_message.notification)
+        if message is None:
+            return -1  # message was not sent, abort
         menu_message.is_alive()
         self._menu_queue.append(menu_message)
         return message.message_id
 
-    async def goto_home(self) -> int:
+    async def goto_home(self, context: Optional[CallbackContext[BT, UD, CD, BD]] = None) -> int:
         """Go to home menu, empty menu_queue."""
+        if not self._menu_queue:
+            return -1
         if len(self._menu_queue) == 1:
             # already at 'home' level
             return self._menu_queue[0].message_id
         menu_previous = self._menu_queue.pop()
         while self._menu_queue:
             menu_previous = self._menu_queue.pop()
-        return await self.goto_menu(menu_previous)
+        return await self.goto_menu(menu_previous, context)
 
     @staticmethod
     def filter_unicode(input_string: str) -> str:
         """Remove non-unicode characters from input string."""
         return input_string.encode("ascii", "ignore").decode("utf-8")
 
-    async def _send_app_message(self, message: BaseMessage, label: str) -> int:
+    async def _send_app_message(
+        self, message: BaseMessage, label: str, context: Optional[CallbackContext[BT, UD, CD, BD]] = None
+    ) -> int:
         """Send an application message."""
-        content = emoji_replace(message.update())
+        content = await message.get_updated_content(context)
         # if message with this label already exist in message_queue, delete it and replace it
         info_message = self.filter_unicode(f"Send message '{message.label}': '{label}'")
         logger.info(str(info_message))
         if "_" not in message.label:
             message.label = f"{message.label}_{label}"
 
         # delete message if already displayed
         message_existing = self.get_message(message.label)
         if message_existing is not None:
             await self._delete_queued_message(message)
 
         message.is_alive()
 
         keyboard = message.gen_inline_keyboard_content()
-        msg = await self.send_message(content, keyboard, message.notification)
+        if message.picture:
+            msg = await self.send_photo(
+                message.picture, notification=message.notification, caption=content, keyboard=keyboard
+            )
+        else:
+            msg = await self.send_message(content, keyboard, message.notification)
+        if msg is None:
+            return -1  # message was not sent, abort
         message.message_id = msg.message_id
         self._message_queue.append(message)
 
         message.content_previous = content
         message.keyboard_previous = message.keyboard.copy()
         return message.message_id
 
@@ -329,34 +363,45 @@
             chat_id=self.chat_id,
             text=content,
             parse_mode=ParseMode.HTML,
             reply_markup=keyboard,
             disable_notification=not notification,
         )
 
-    async def edit_message(self, message: BaseMessage) -> bool:
+    async def edit_message(
+        self, message: BaseMessage, context: Optional[CallbackContext[BT, UD, CD, BD]] = None
+    ) -> bool:
         """Edit an inline message asynchronously."""
         message_updt = self.get_message(message.label)
         if message_updt is None:
             return False
 
         # check if content and keyboard have changed since previous message
-        content = emoji_replace(message_updt.update())
+        content = await message_updt.get_updated_content(context)
         if not self._message_check_changes(message_updt, content):
             return False
 
         keyboard_format = message_updt.gen_inline_keyboard_content()
         try:
-            await self._bot.edit_message_text(
-                text=content,
-                chat_id=self.chat_id,
-                message_id=message_updt.message_id,
-                parse_mode=ParseMode.HTML,
-                reply_markup=keyboard_format,
-            )
+            if message_updt.picture:
+                await self._bot.edit_message_caption(
+                    caption=content,
+                    chat_id=self.chat_id,
+                    message_id=message_updt.message_id,
+                    parse_mode=ParseMode.HTML,
+                    reply_markup=keyboard_format,
+                )
+            else:
+                await self._bot.edit_message_text(
+                    text=content,
+                    chat_id=self.chat_id,
+                    message_id=message_updt.message_id,
+                    parse_mode=ParseMode.HTML,
+                    reply_markup=keyboard_format,
+                )
         except telegram.error.BadRequest as error:
             logger.error(error)
             return False
         return True
 
     @staticmethod
     def _message_check_changes(message: BaseMessage, content: str) -> bool:
@@ -367,71 +412,72 @@
         ]
         if content_identical and keyboard_identical:
             return False
         message.content_previous = content
         message.keyboard_previous = message.keyboard.copy()
         return True
 
-    async def select_menu_button(self, label: str) -> Optional[int]:  # noqa: C901
+    async def select_menu_button(
+        self, label: str, context: Optional[CallbackContext[BT, UD, CD, BD]] = None
+    ) -> Optional[int]:  # noqa: C901
         """Select menu button using label."""
         msg_id = 0
         if label == "Back":
             if len(self._menu_queue) == 1:
                 # already at 'home' level
                 return self._menu_queue[0].message_id
             menu_previous = self._menu_queue.pop()  # delete actual menu
             if self._menu_queue:
                 menu_previous = self._menu_queue.pop()
-            return await self.goto_menu(menu_previous)
+            return await self.goto_menu(menu_previous, context)
         if label == "Home":
-            return await self.goto_home()
+            return await self.goto_home(context)
 
         for menu_item in self._menu_queue[::-1]:
             btn = menu_item.get_button(label)
             if not btn:
                 continue
             if isinstance(btn.callback, BaseMessage):
                 if btn.callback.inlined:
-                    msg_id = await self._send_app_message(btn.callback, label)
+                    msg_id = await self._send_app_message(btn.callback, label, context)
                     if btn.callback.home_after:
-                        msg_id = await self.goto_home()
+                        msg_id = await self.goto_home(context)
                 else:
-                    msg_id = await self.goto_menu(btn.callback)
+                    msg_id = await self.goto_menu(btn.callback, context)
             elif btn.callback is not None and hasattr(btn.callback, "__call__"):
-                if asyncio.iscoroutinefunction(btn.callback):
-                    await btn.callback()  # type: ignore
-                else:
-                    btn.callback()  # type: ignore
+                await call_function_EAFP(btn.callback, context)
             return msg_id
 
         # label does not match any sub-menu, just process the user input
-        await self.capture_user_input(label)
+        await self.capture_user_input(label, context)
         return None
 
-    async def capture_user_input(self, label: str) -> None:
+    async def capture_user_input(self, label: str, context: Optional[CallbackContext[BT, UD, CD, BD]] = None) -> None:
         """Process the user input in the last message updated."""
         last_menu_message = self._menu_queue[-1]
         if self._message_queue:
             last_app_message = self._message_queue[-1]
             if last_app_message.time_alive > last_menu_message.time_alive:
                 last_menu_message = last_app_message
-        await last_menu_message.text_input(label)
+        await last_menu_message.text_input(label, context)
 
     async def app_message_webapp_callback(self, webapp_data: str, button_text: str) -> None:
         """Execute the callback associated to this webapp."""
         last_menu = self._menu_queue[-1]
         webapp_message = next(iter(y for x in last_menu.keyboard for y in x if y.label == button_text), None)
         if webapp_message is not None and callable(webapp_message.callback):
             if asyncio.iscoroutinefunction(webapp_message.callback):
                 html_response = await webapp_message.callback(webapp_data)
             else:
                 html_response = webapp_message.callback(webapp_data)
             await self.send_message(html_response, notification=webapp_message.notification)
 
-    async def app_message_button_callback(self, callback_label: str, callback_id: str) -> None:
+    async def app_message_button_callback(
+        self, callback_label: str, callback_id: str, context: Optional[CallbackContext[BT, UD, CD, BD]] = None
+    ) -> None:
         """Entry point to execute an action after message button selection."""
         label_message, label_action = callback_label.split(".")
         log_message = self.filter_unicode(f"Received action request from '{label_message}': '{label_action}'")
         logger.info(log_message)
         message = self.get_message(label_message)
         if message is None:
             logger.error(f"Message with label {label_message} not found, return")
@@ -454,22 +500,17 @@
             await self._bot.answer_callback_query(callback_id, text="Select an answer...")
             return
 
         if not callable(btn.callback):
             return
 
         if btn.args is not None:
-            if asyncio.iscoroutinefunction(btn.callback):
-                action_status = await btn.callback(btn.args)
-            else:
-                action_status = btn.callback(btn.args)
-        elif asyncio.iscoroutinefunction(btn.callback):
-            action_status = await btn.callback()
+            action_status = await call_function_EAFP(btn.callback, context, btn.args)
         else:
-            action_status = btn.callback()
+            action_status = await call_function_EAFP(btn.callback, context)
 
         # send picture if custom label found
         if btn.btype == ButtonType.PICTURE:
             await self.send_photo(picture_path=action_status, notification=btn.notification)
             await self._bot.answer_callback_query(callback_id, text="Picture sent!")
             return
         if btn.btype == ButtonType.STICKER:
@@ -480,15 +521,15 @@
             await self.send_message(action_status, notification=btn.notification)
             await self._bot.answer_callback_query(callback_id, text="Message sent!")
             return
         await self._bot.answer_callback_query(callback_id, text=action_status)
 
         # update expiry period and update
         message.is_alive()
-        await self.edit_message(message)
+        await self.edit_message(message, context)
 
     @staticmethod
     def _sticker_check_replace(sticker_path: str) -> Union[str, bytes]:
         """Check if sticker is correct file type."""
         try:
             if not sticker_path.lower().endswith(".webp"):
                 raise ValueError("Sticker has no .webp format")
@@ -519,20 +560,30 @@
                     return file_h.read()
             raise ValueError("Path is not a picture")
         except ValueError:
             url_default = f"{__raw_url__}/resources/stats_default.png"
             logger.error(f"Picture path '{picture_path}' is invalid, replacing with default {url_default}")
             return url_default
 
-    async def send_photo(self, picture_path: str, notification: bool = True) -> Optional[telegram.Message]:
+    async def send_photo(
+        self,
+        picture_path: str,
+        notification: bool = True,
+        caption: str = "",
+        keyboard: Optional[Union[ReplyKeyboardMarkup, InlineKeyboardMarkup]] = None,
+    ) -> Optional[telegram.Message]:
         """Send a picture."""
         picture_obj = self._picture_check_replace(picture_path=picture_path)
         try:
             return await self._bot.send_photo(
-                chat_id=self.chat_id, photo=picture_obj, disable_notification=not notification
+                chat_id=self.chat_id,
+                photo=picture_obj,
+                caption=caption,
+                reply_markup=keyboard,
+                disable_notification=not notification,
             )
         except telegram.error.BadRequest as error:
             logger.error(f"Failed to send picture {picture_path}: {error}")
         return None
 
     async def send_sticker(self, sticker_path: str, notification: bool = True) -> Optional[telegram.Message]:
         """Send a picture."""
```

### Comparing `telegram_menu-2.0.2/telegram_menu.egg-info/PKG-INFO` & `telegram_menu-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: telegram-menu
-Version: 2.0.2
+Name: telegram_menu
+Version: 2.1.0
 Summary: A python library to generate navigation menus using Telegram Bot API.
 Home-page: https://github.com/mevellea/telegram_menu
 Author: Armel Mevellec
 Author-email: mevellea@gmail.com
 License: GNU GPLv3
 Keywords: telegram
 Platform: any
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # telegram_menu package
 
-<img src="https://img.shields.io/badge/python-3.7-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.8-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.9-blue.svg" alt="drawing"/>
+<img src="https://img.shields.io/badge/python-3.7-blue.svg" alt="drawing"/> <img src="https://img.shields.io/badge/python-3.11-blue.svg" alt="drawing"/>
 <br/>
 A python library to generate navigation menus using Telegram Bot API.
 
 Features:
 
 * Menu navigation using tree structure, unlimited depth
 * Support for sending pictures (local file or url), stickers, notifications, webapps and polls
@@ -164,7 +164,16 @@
 
 <img src="https://raw.githubusercontent.com/mevellea/telegram_menu/master/resources/classes.png" width="800"/>
 
 [navigation.py]: https://github.com/mevellea/telegram_menu/blob/master/telegram_menu/navigation.py
 [models.py]: https://github.com/mevellea/telegram_menu/blob/master/telegram_menu/models.py
 [create a Telegram bot]: https://github.com/python-telegram-bot/python-telegram-bot/wiki/Introduction-to-the-API
 [Demo: TelegramMenuSession]: https://raw.githubusercontent.com/mevellea/telegram_menu/master/resources/demo.gif
+
+## Unit-tests
+
+To execute the test suite, run the following command and then start a session from a Telegram client with the keyword **/start**.
+
+```bash
+python -m unittest
+```
+
```

### Comparing `telegram_menu-2.0.2/tests/test_connection.py` & `telegram_menu-2.1.0/tests/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,24 @@
 #!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+#
+# Copyright 2020-2023 Armel Mevellec
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, version 3.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+# General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
+#
 
 """Test telegram_menu package."""
 
 import asyncio
 import datetime
 import json
 import logging
@@ -97,15 +113,15 @@
     def _toggle_play_button(self) -> None:
         """Toggle the first button between play and pause mode."""
         self.play_pause = not self.play_pause
 
     @staticmethod
     def action_poll(poll_answer: str) -> None:
         """Display poll answer."""
-        logging.info(f"Answer is {poll_answer}")  # pylint: disable=logging-fstring-interpolation
+        logging.info(f"Answer is {poll_answer}")
 
     def update(self) -> str:
         """Update message content."""
         poll_question = "Select one option:"
         poll_choices = [":play_button: Option " + str(x) for x in range(6)]
         play_pause_button = ":play_button:" if self.play_pause else ":pause_button:"
         self.keyboard = [
@@ -192,14 +208,15 @@
 
     def __init__(self, navigation: MyNavigationHandler, update_callback: Optional[List[UpdateCallback]] = None) -> None:
         """Init SecondMenuMessage class."""
         super().__init__(
             navigation,
             SecondMenuMessage.LABEL,
             notification=False,
+            picture=(ROOT_FOLDER / "resources" / "packages.png").resolve().as_posix(),
             expiry_period=datetime.timedelta(seconds=5),
             input_field="Enter an option",
         )
 
         third_menu = ThirdMenuMessage(navigation, update_callback)
         self.add_button(label="Third menu", callback=third_menu, new_row=True)
         self.add_button_back(new_row=True)
```

