# Comparing `tmp/rotate-screen-0.1.4.tar.gz` & `tmp/rotate-screen-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotate-screen-0.1.4.tar", last modified: Sat Apr  8 11:10:25 2023, max compression
+gzip compressed data, was "rotate-screen-0.1.5.tar", last modified: Sun May  7 20:04:28 2023, max compression
```

## Comparing `rotate-screen-0.1.4.tar` & `rotate-screen-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 danny     (1000) danny     (1000)        0 2023-04-08 11:10:25.945055 rotate-screen-0.1.4/
--rw-r--r--   0 danny     (1000) danny     (1000)     1070 2023-04-03 20:51:17.000000 rotate-screen-0.1.4/LICENSE
--rw-r--r--   0 danny     (1000) danny     (1000)     4828 2023-04-08 11:10:25.945055 rotate-screen-0.1.4/PKG-INFO
--rw-r--r--   0 danny     (1000) danny     (1000)     3862 2023-04-03 20:51:17.000000 rotate-screen-0.1.4/README.md
-drwxr-xr-x   0 danny     (1000) danny     (1000)        0 2023-04-08 11:10:25.945055 rotate-screen-0.1.4/rotate_screen.egg-info/
--rw-r--r--   0 danny     (1000) danny     (1000)     4828 2023-04-08 11:10:25.000000 rotate-screen-0.1.4/rotate_screen.egg-info/PKG-INFO
--rw-r--r--   0 danny     (1000) danny     (1000)      259 2023-04-08 11:10:25.000000 rotate-screen-0.1.4/rotate_screen.egg-info/SOURCES.txt
--rw-r--r--   0 danny     (1000) danny     (1000)        1 2023-04-08 11:10:25.000000 rotate-screen-0.1.4/rotate_screen.egg-info/dependency_links.txt
--rw-r--r--   0 danny     (1000) danny     (1000)       71 2023-04-08 11:10:25.000000 rotate-screen-0.1.4/rotate_screen.egg-info/requires.txt
--rw-r--r--   0 danny     (1000) danny     (1000)       13 2023-04-08 11:10:25.000000 rotate-screen-0.1.4/rotate_screen.egg-info/top_level.txt
-drwxr-xr-x   0 danny     (1000) danny     (1000)        0 2023-04-08 11:10:25.945055 rotate-screen-0.1.4/rotatescreen/
--rw-r--r--   0 danny     (1000) danny     (1000)       23 2023-04-08 10:50:06.000000 rotate-screen-0.1.4/rotatescreen/__init__.py
--rw-r--r--   0 danny     (1000) danny     (1000)     2481 2023-04-08 10:50:06.000000 rotate-screen-0.1.4/rotatescreen/display.py
--rw-r--r--   0 danny     (1000) danny     (1000)       38 2023-04-08 11:10:25.945055 rotate-screen-0.1.4/setup.cfg
--rw-r--r--   0 danny     (1000) danny     (1000)     1690 2023-04-08 10:59:07.000000 rotate-screen-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:04:28.188455 rotate-screen-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-11 23:16:19.000000 rotate-screen-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4937 2023-05-07 20:04:28.187956 rotate-screen-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3946 2023-05-07 19:59:43.000000 rotate-screen-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 20:04:28.182950 rotate-screen-0.1.5/rotate_screen.egg-info/
+-rw-rw-rw-   0        0        0     4937 2023-05-07 20:04:28.000000 rotate-screen-0.1.5/rotate_screen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-05-07 20:04:28.000000 rotate-screen-0.1.5/rotate_screen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 20:04:28.000000 rotate-screen-0.1.5/rotate_screen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-05-07 20:04:28.000000 rotate-screen-0.1.5/rotate_screen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 20:04:28.000000 rotate-screen-0.1.5/rotate_screen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 20:04:28.186465 rotate-screen-0.1.5/rotatescreen/
+-rw-rw-rw-   0        0        0       24 2023-05-07 19:59:43.000000 rotate-screen-0.1.5/rotatescreen/__init__.py
+-rw-rw-rw-   0        0        0     2548 2023-05-07 20:03:07.000000 rotate-screen-0.1.5/rotatescreen/display.py
+-rw-rw-rw-   0        0        0     4991 2023-05-07 20:00:16.000000 rotate-screen-0.1.5/rotatescreen/display_linux.py
+-rw-rw-rw-   0        0        0       42 2023-05-07 20:04:28.188455 rotate-screen-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-05-07 20:03:21.000000 rotate-screen-0.1.5/setup.py
```

### Comparing `rotate-screen-0.1.4/PKG-INFO` & `rotate-screen-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-Metadata-Version: 2.1
-Name: rotate-screen
-Version: 0.1.4
-Summary: A small Python package for rotating the screen.
-Home-page: https://github.com/danny-burrows/rotate-screen
-Author: Danny Burrows
-Author-email: dannyburrows@protonmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Desktop Environment
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: shortcuts_example
-License-File: LICENSE
-
-<div align="center">
-  <img src="rotate-screen.svg" alt="Rotate Screen">
-</div>
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rotate-screen)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/rotate-screen)
-![GitHub](https://img.shields.io/github/license/danny-burrows/rotate-screen)
-
-## Platforms Supported
-Windows is currently the only platform supported.
-
-## Installation
-Clone the repo, download as a zip file, or use the following command...
-```sh
-pip install rotate-screen
-```
-
-## Documentation
-The package comes with some functions to get available displays in the form of \<rotatescreen Display\> objects. You can then use the \<rotatescreen Display\> object methods to change the orientation of the display. 
-
-#### Here are a few of the available package functions...
-
-| Function | Returns |
-|----------|---------|
-| `rotatescreen.get_displays()` | Returns a list of \<rotatescreen Display\> objects for each available display.  |
-| `rotatescreen.get_secondary_displays()` | Returns a list of \<rotatescreen Display\> objects for every display apart from the primary display. |
-| `rotatescreen.get_primary_display()` | Returns a \<rotatescreen Display\> object for the primary display. |
-
-#### Here are the available methods (no return value) for a \<rotatescreen Display\> object...
-
-| Procedure | Arguments | Result |
-|-----------|-----------|--------|
-| `.rotate_to(pos)`         | pos (int): Degrees to rotate the screen to. Must be one of 0, 90, 180, 270. | Rotates the screen to desired. |
-| `.set_landscape()`        || Rotates the screen to landscape. |
-| `.set_landscape_flipped()`|| Rotates the screen to upside down landscape.|
-| `.set_portrait()`         || Rotates the screen to portrait.|
-| `.set_portrait_flipped()` || Rotates the screen to upside down portrait.|
-
-#### Here are the available attributes for a \<rotatescreen Display\> object...
-
-| Attribute | Returns |
-|-----------|---------|
-| `.current_orientation` | Returns (int) the current orientation of the display, will be one of 0, 90, 180, 270. |
-| `.is_primary`          | Returns (bool) if the display is the primary monitor. |
-| `.info`                | Returns (dict) monitor info. |
-| `.device`              | Returns monitor device info. |
-| `.device_description`  | Returns (str) visable name for display device. |
-
-## Example: ![Ctrl+Alt+Arrow Shortcut](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/shortcuts.py)
-This is a simple example that implements the 'Ctrl+Alt+Arrow' keyboard shortcut for rotating the display. This is because some graphics cards don't come with this capability by default.
-
-This example requires the keyboard module...
-```sh
-pip install keyboard
-```
-Here is the code! It adds hotkeys to rotate the primary display in the desired direction upon the user entering Ctrl, Alt and an arrow key. It then waits until the script is exited.
-```python
-import rotatescreen
-import keyboard
-
-screen = rotatescreen.get_primary_display()
-
-keyboard.add_hotkey('ctrl+alt+up', screen.set_landscape, suppress=True)
-keyboard.add_hotkey('ctrl+alt+right', screen.set_portrait_flipped, suppress=True)
-keyboard.add_hotkey('ctrl+alt+down', screen.set_landscape_flipped, suppress=True)
-keyboard.add_hotkey('ctrl+alt+left', screen.set_portrait, suppress=True)
-
-keyboard.wait()
-```
-
-## Example: ![Do A Barrel Roll](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/do-a-barrel-roll.py)
-This was a little joke script to show off some more of the modules functionality, due to the way windows rotates the display this is a pretty horrific looking, but entertaining. :)
-```python
-import rotatescreen
-import time
-
-screen = rotatescreen.get_primary_display()
-start_pos = screen.current_orientation
-
-for i in range(1, 5):
-    pos = abs((start_pos - i*90) % 360)
-    screen.rotate_to(pos)
-    time.sleep(1.5)
-```
+Metadata-Version: 2.1
+Name: rotate-screen
+Version: 0.1.5
+Summary: A small Python package for rotating the screen.
+Home-page: https://github.com/danny-burrows/rotate-screen
+Author: Danny Burrows
+Author-email: dannyburrows@protonmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Desktop Environment
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: shortcuts_example
+License-File: LICENSE
+
+<div align="center">
+  <img src="rotate-screen.svg" alt="Rotate Screen">
+</div>
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rotate-screen)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/rotate-screen)
+![GitHub](https://img.shields.io/github/license/danny-burrows/rotate-screen)
+
+## Platforms Supported
+Windows is currently the only platform supported.
+
+## Installation
+Clone the repo, download as a zip file, or use the following command...
+```sh
+pip install rotate-screen
+```
+
+## Documentation
+The package comes with some functions to get available displays in the form of \<rotatescreen Display\> objects. You can then use the \<rotatescreen Display\> object methods to change the orientation of the display. 
+
+#### Here are a few of the available package functions...
+
+| Function | Returns |
+|----------|---------|
+| `rotatescreen.get_displays()` | Returns a list of \<rotatescreen Display\> objects for each available display.  |
+| `rotatescreen.get_secondary_displays()` | Returns a list of \<rotatescreen Display\> objects for every display apart from the primary display. |
+| `rotatescreen.get_primary_display()` | Returns a \<rotatescreen Display\> object for the primary display. |
+
+#### Here are the available methods (no return value) for a \<rotatescreen Display\> object...
+
+| Procedure | Arguments | Result |
+|-----------|-----------|--------|
+| `.rotate_to(pos)`         | pos (int): Degrees to rotate the screen to. Must be one of 0, 90, 180, 270. | Rotates the screen to desired. |
+| `.set_landscape()`        || Rotates the screen to landscape. |
+| `.set_landscape_flipped()`|| Rotates the screen to upside down landscape.|
+| `.set_portrait()`         || Rotates the screen to portrait.|
+| `.set_portrait_flipped()` || Rotates the screen to upside down portrait.|
+
+#### Here are the available attributes for a \<rotatescreen Display\> object...
+
+| Attribute | Returns |
+|-----------|---------|
+| `.current_orientation` | Returns (int) the current orientation of the display, will be one of 0, 90, 180, 270. |
+| `.is_primary`          | Returns (bool) if the display is the primary monitor. |
+| `.info`                | Returns (dict) monitor info. |
+| `.device`              | Returns monitor device info. |
+| `.device_description`  | Returns (str) visable name for display device. |
+
+## Example: ![Ctrl+Alt+Arrow Shortcut](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/shortcuts.py)
+This is a simple example that implements the 'Ctrl+Alt+Arrow' keyboard shortcut for rotating the display. This is because some graphics cards don't come with this capability by default.
+
+This example requires the keyboard module...
+```sh
+pip install keyboard
+```
+Here is the code! It adds hotkeys to rotate the primary display in the desired direction upon the user entering Ctrl, Alt and an arrow key. It then waits until the script is exited.
+```python
+import rotatescreen
+import keyboard
+
+screen = rotatescreen.get_primary_display()
+
+keyboard.add_hotkey('ctrl+alt+up', screen.set_landscape, suppress=True)
+keyboard.add_hotkey('ctrl+alt+right', screen.set_portrait_flipped, suppress=True)
+keyboard.add_hotkey('ctrl+alt+down', screen.set_landscape_flipped, suppress=True)
+keyboard.add_hotkey('ctrl+alt+left', screen.set_portrait, suppress=True)
+
+keyboard.wait()
+```
+
+## Example: ![Do A Barrel Roll](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/do-a-barrel-roll.py)
+This was a little joke script to show off some more of the modules functionality, due to the way windows rotates the display this is a pretty horrific looking, but entertaining. :)
+```python
+import rotatescreen
+import time
+
+screen = rotatescreen.get_primary_display()
+start_pos = screen.current_orientation
+
+for i in range(1, 5):
+    pos = abs((start_pos - i*90) % 360)
+    screen.rotate_to(pos)
+    time.sleep(1.5)
+```
```

### Comparing `rotate-screen-0.1.4/README.md` & `rotate-screen-0.1.5/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-<div align="center">
-  <img src="rotate-screen.svg" alt="Rotate Screen">
-</div>
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rotate-screen)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/rotate-screen)
-![GitHub](https://img.shields.io/github/license/danny-burrows/rotate-screen)
-
-## Platforms Supported
-Windows is currently the only platform supported.
-
-## Installation
-Clone the repo, download as a zip file, or use the following command...
-```sh
-pip install rotate-screen
-```
-
-## Documentation
-The package comes with some functions to get available displays in the form of \<rotatescreen Display\> objects. You can then use the \<rotatescreen Display\> object methods to change the orientation of the display. 
-
-#### Here are a few of the available package functions...
-
-| Function | Returns |
-|----------|---------|
-| `rotatescreen.get_displays()` | Returns a list of \<rotatescreen Display\> objects for each available display.  |
-| `rotatescreen.get_secondary_displays()` | Returns a list of \<rotatescreen Display\> objects for every display apart from the primary display. |
-| `rotatescreen.get_primary_display()` | Returns a \<rotatescreen Display\> object for the primary display. |
-
-#### Here are the available methods (no return value) for a \<rotatescreen Display\> object...
-
-| Procedure | Arguments | Result |
-|-----------|-----------|--------|
-| `.rotate_to(pos)`         | pos (int): Degrees to rotate the screen to. Must be one of 0, 90, 180, 270. | Rotates the screen to desired. |
-| `.set_landscape()`        || Rotates the screen to landscape. |
-| `.set_landscape_flipped()`|| Rotates the screen to upside down landscape.|
-| `.set_portrait()`         || Rotates the screen to portrait.|
-| `.set_portrait_flipped()` || Rotates the screen to upside down portrait.|
-
-#### Here are the available attributes for a \<rotatescreen Display\> object...
-
-| Attribute | Returns |
-|-----------|---------|
-| `.current_orientation` | Returns (int) the current orientation of the display, will be one of 0, 90, 180, 270. |
-| `.is_primary`          | Returns (bool) if the display is the primary monitor. |
-| `.info`                | Returns (dict) monitor info. |
-| `.device`              | Returns monitor device info. |
-| `.device_description`  | Returns (str) visable name for display device. |
-
-## Example: ![Ctrl+Alt+Arrow Shortcut](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/shortcuts.py)
-This is a simple example that implements the 'Ctrl+Alt+Arrow' keyboard shortcut for rotating the display. This is because some graphics cards don't come with this capability by default.
-
-This example requires the keyboard module...
-```sh
-pip install keyboard
-```
-Here is the code! It adds hotkeys to rotate the primary display in the desired direction upon the user entering Ctrl, Alt and an arrow key. It then waits until the script is exited.
-```python
-import rotatescreen
-import keyboard
-
-screen = rotatescreen.get_primary_display()
-
-keyboard.add_hotkey('ctrl+alt+up', screen.set_landscape, suppress=True)
-keyboard.add_hotkey('ctrl+alt+right', screen.set_portrait_flipped, suppress=True)
-keyboard.add_hotkey('ctrl+alt+down', screen.set_landscape_flipped, suppress=True)
-keyboard.add_hotkey('ctrl+alt+left', screen.set_portrait, suppress=True)
-
-keyboard.wait()
-```
-
-## Example: ![Do A Barrel Roll](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/do-a-barrel-roll.py)
-This was a little joke script to show off some more of the modules functionality, due to the way windows rotates the display this is a pretty horrific looking, but entertaining. :)
-```python
-import rotatescreen
-import time
-
-screen = rotatescreen.get_primary_display()
-start_pos = screen.current_orientation
-
-for i in range(1, 5):
-    pos = abs((start_pos - i*90) % 360)
-    screen.rotate_to(pos)
-    time.sleep(1.5)
-```
+<div align="center">
+  <img src="rotate-screen.svg" alt="Rotate Screen">
+</div>
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rotate-screen)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/rotate-screen)
+![GitHub](https://img.shields.io/github/license/danny-burrows/rotate-screen)
+
+## Platforms Supported
+Windows is currently the only platform supported.
+
+## Installation
+Clone the repo, download as a zip file, or use the following command...
+```sh
+pip install rotate-screen
+```
+
+## Documentation
+The package comes with some functions to get available displays in the form of \<rotatescreen Display\> objects. You can then use the \<rotatescreen Display\> object methods to change the orientation of the display. 
+
+#### Here are a few of the available package functions...
+
+| Function | Returns |
+|----------|---------|
+| `rotatescreen.get_displays()` | Returns a list of \<rotatescreen Display\> objects for each available display.  |
+| `rotatescreen.get_secondary_displays()` | Returns a list of \<rotatescreen Display\> objects for every display apart from the primary display. |
+| `rotatescreen.get_primary_display()` | Returns a \<rotatescreen Display\> object for the primary display. |
+
+#### Here are the available methods (no return value) for a \<rotatescreen Display\> object...
+
+| Procedure | Arguments | Result |
+|-----------|-----------|--------|
+| `.rotate_to(pos)`         | pos (int): Degrees to rotate the screen to. Must be one of 0, 90, 180, 270. | Rotates the screen to desired. |
+| `.set_landscape()`        || Rotates the screen to landscape. |
+| `.set_landscape_flipped()`|| Rotates the screen to upside down landscape.|
+| `.set_portrait()`         || Rotates the screen to portrait.|
+| `.set_portrait_flipped()` || Rotates the screen to upside down portrait.|
+
+#### Here are the available attributes for a \<rotatescreen Display\> object...
+
+| Attribute | Returns |
+|-----------|---------|
+| `.current_orientation` | Returns (int) the current orientation of the display, will be one of 0, 90, 180, 270. |
+| `.is_primary`          | Returns (bool) if the display is the primary monitor. |
+| `.info`                | Returns (dict) monitor info. |
+| `.device`              | Returns monitor device info. |
+| `.device_description`  | Returns (str) visable name for display device. |
+
+## Example: ![Ctrl+Alt+Arrow Shortcut](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/shortcuts.py)
+This is a simple example that implements the 'Ctrl+Alt+Arrow' keyboard shortcut for rotating the display. This is because some graphics cards don't come with this capability by default.
+
+This example requires the keyboard module...
+```sh
+pip install keyboard
+```
+Here is the code! It adds hotkeys to rotate the primary display in the desired direction upon the user entering Ctrl, Alt and an arrow key. It then waits until the script is exited.
+```python
+import rotatescreen
+import keyboard
+
+screen = rotatescreen.get_primary_display()
+
+keyboard.add_hotkey('ctrl+alt+up', screen.set_landscape, suppress=True)
+keyboard.add_hotkey('ctrl+alt+right', screen.set_portrait_flipped, suppress=True)
+keyboard.add_hotkey('ctrl+alt+down', screen.set_landscape_flipped, suppress=True)
+keyboard.add_hotkey('ctrl+alt+left', screen.set_portrait, suppress=True)
+
+keyboard.wait()
+```
+
+## Example: ![Do A Barrel Roll](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/do-a-barrel-roll.py)
+This was a little joke script to show off some more of the modules functionality, due to the way windows rotates the display this is a pretty horrific looking, but entertaining. :)
+```python
+import rotatescreen
+import time
+
+screen = rotatescreen.get_primary_display()
+start_pos = screen.current_orientation
+
+for i in range(1, 5):
+    pos = abs((start_pos - i*90) % 360)
+    screen.rotate_to(pos)
+    time.sleep(1.5)
+```
```

### Comparing `rotate-screen-0.1.4/rotate_screen.egg-info/PKG-INFO` & `rotate-screen-0.1.5/rotate_screen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-Metadata-Version: 2.1
-Name: rotate-screen
-Version: 0.1.4
-Summary: A small Python package for rotating the screen.
-Home-page: https://github.com/danny-burrows/rotate-screen
-Author: Danny Burrows
-Author-email: dannyburrows@protonmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Desktop Environment
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: shortcuts_example
-License-File: LICENSE
-
-<div align="center">
-  <img src="rotate-screen.svg" alt="Rotate Screen">
-</div>
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rotate-screen)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/rotate-screen)
-![GitHub](https://img.shields.io/github/license/danny-burrows/rotate-screen)
-
-## Platforms Supported
-Windows is currently the only platform supported.
-
-## Installation
-Clone the repo, download as a zip file, or use the following command...
-```sh
-pip install rotate-screen
-```
-
-## Documentation
-The package comes with some functions to get available displays in the form of \<rotatescreen Display\> objects. You can then use the \<rotatescreen Display\> object methods to change the orientation of the display. 
-
-#### Here are a few of the available package functions...
-
-| Function | Returns |
-|----------|---------|
-| `rotatescreen.get_displays()` | Returns a list of \<rotatescreen Display\> objects for each available display.  |
-| `rotatescreen.get_secondary_displays()` | Returns a list of \<rotatescreen Display\> objects for every display apart from the primary display. |
-| `rotatescreen.get_primary_display()` | Returns a \<rotatescreen Display\> object for the primary display. |
-
-#### Here are the available methods (no return value) for a \<rotatescreen Display\> object...
-
-| Procedure | Arguments | Result |
-|-----------|-----------|--------|
-| `.rotate_to(pos)`         | pos (int): Degrees to rotate the screen to. Must be one of 0, 90, 180, 270. | Rotates the screen to desired. |
-| `.set_landscape()`        || Rotates the screen to landscape. |
-| `.set_landscape_flipped()`|| Rotates the screen to upside down landscape.|
-| `.set_portrait()`         || Rotates the screen to portrait.|
-| `.set_portrait_flipped()` || Rotates the screen to upside down portrait.|
-
-#### Here are the available attributes for a \<rotatescreen Display\> object...
-
-| Attribute | Returns |
-|-----------|---------|
-| `.current_orientation` | Returns (int) the current orientation of the display, will be one of 0, 90, 180, 270. |
-| `.is_primary`          | Returns (bool) if the display is the primary monitor. |
-| `.info`                | Returns (dict) monitor info. |
-| `.device`              | Returns monitor device info. |
-| `.device_description`  | Returns (str) visable name for display device. |
-
-## Example: ![Ctrl+Alt+Arrow Shortcut](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/shortcuts.py)
-This is a simple example that implements the 'Ctrl+Alt+Arrow' keyboard shortcut for rotating the display. This is because some graphics cards don't come with this capability by default.
-
-This example requires the keyboard module...
-```sh
-pip install keyboard
-```
-Here is the code! It adds hotkeys to rotate the primary display in the desired direction upon the user entering Ctrl, Alt and an arrow key. It then waits until the script is exited.
-```python
-import rotatescreen
-import keyboard
-
-screen = rotatescreen.get_primary_display()
-
-keyboard.add_hotkey('ctrl+alt+up', screen.set_landscape, suppress=True)
-keyboard.add_hotkey('ctrl+alt+right', screen.set_portrait_flipped, suppress=True)
-keyboard.add_hotkey('ctrl+alt+down', screen.set_landscape_flipped, suppress=True)
-keyboard.add_hotkey('ctrl+alt+left', screen.set_portrait, suppress=True)
-
-keyboard.wait()
-```
-
-## Example: ![Do A Barrel Roll](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/do-a-barrel-roll.py)
-This was a little joke script to show off some more of the modules functionality, due to the way windows rotates the display this is a pretty horrific looking, but entertaining. :)
-```python
-import rotatescreen
-import time
-
-screen = rotatescreen.get_primary_display()
-start_pos = screen.current_orientation
-
-for i in range(1, 5):
-    pos = abs((start_pos - i*90) % 360)
-    screen.rotate_to(pos)
-    time.sleep(1.5)
-```
+Metadata-Version: 2.1
+Name: rotate-screen
+Version: 0.1.5
+Summary: A small Python package for rotating the screen.
+Home-page: https://github.com/danny-burrows/rotate-screen
+Author: Danny Burrows
+Author-email: dannyburrows@protonmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Desktop Environment
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: shortcuts_example
+License-File: LICENSE
+
+<div align="center">
+  <img src="rotate-screen.svg" alt="Rotate Screen">
+</div>
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rotate-screen)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/rotate-screen)
+![GitHub](https://img.shields.io/github/license/danny-burrows/rotate-screen)
+
+## Platforms Supported
+Windows is currently the only platform supported.
+
+## Installation
+Clone the repo, download as a zip file, or use the following command...
+```sh
+pip install rotate-screen
+```
+
+## Documentation
+The package comes with some functions to get available displays in the form of \<rotatescreen Display\> objects. You can then use the \<rotatescreen Display\> object methods to change the orientation of the display. 
+
+#### Here are a few of the available package functions...
+
+| Function | Returns |
+|----------|---------|
+| `rotatescreen.get_displays()` | Returns a list of \<rotatescreen Display\> objects for each available display.  |
+| `rotatescreen.get_secondary_displays()` | Returns a list of \<rotatescreen Display\> objects for every display apart from the primary display. |
+| `rotatescreen.get_primary_display()` | Returns a \<rotatescreen Display\> object for the primary display. |
+
+#### Here are the available methods (no return value) for a \<rotatescreen Display\> object...
+
+| Procedure | Arguments | Result |
+|-----------|-----------|--------|
+| `.rotate_to(pos)`         | pos (int): Degrees to rotate the screen to. Must be one of 0, 90, 180, 270. | Rotates the screen to desired. |
+| `.set_landscape()`        || Rotates the screen to landscape. |
+| `.set_landscape_flipped()`|| Rotates the screen to upside down landscape.|
+| `.set_portrait()`         || Rotates the screen to portrait.|
+| `.set_portrait_flipped()` || Rotates the screen to upside down portrait.|
+
+#### Here are the available attributes for a \<rotatescreen Display\> object...
+
+| Attribute | Returns |
+|-----------|---------|
+| `.current_orientation` | Returns (int) the current orientation of the display, will be one of 0, 90, 180, 270. |
+| `.is_primary`          | Returns (bool) if the display is the primary monitor. |
+| `.info`                | Returns (dict) monitor info. |
+| `.device`              | Returns monitor device info. |
+| `.device_description`  | Returns (str) visable name for display device. |
+
+## Example: ![Ctrl+Alt+Arrow Shortcut](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/shortcuts.py)
+This is a simple example that implements the 'Ctrl+Alt+Arrow' keyboard shortcut for rotating the display. This is because some graphics cards don't come with this capability by default.
+
+This example requires the keyboard module...
+```sh
+pip install keyboard
+```
+Here is the code! It adds hotkeys to rotate the primary display in the desired direction upon the user entering Ctrl, Alt and an arrow key. It then waits until the script is exited.
+```python
+import rotatescreen
+import keyboard
+
+screen = rotatescreen.get_primary_display()
+
+keyboard.add_hotkey('ctrl+alt+up', screen.set_landscape, suppress=True)
+keyboard.add_hotkey('ctrl+alt+right', screen.set_portrait_flipped, suppress=True)
+keyboard.add_hotkey('ctrl+alt+down', screen.set_landscape_flipped, suppress=True)
+keyboard.add_hotkey('ctrl+alt+left', screen.set_portrait, suppress=True)
+
+keyboard.wait()
+```
+
+## Example: ![Do A Barrel Roll](https://github.com/TheBrokenEstate/rotate-screen/blob/master/examples/do-a-barrel-roll.py)
+This was a little joke script to show off some more of the modules functionality, due to the way windows rotates the display this is a pretty horrific looking, but entertaining. :)
+```python
+import rotatescreen
+import time
+
+screen = rotatescreen.get_primary_display()
+start_pos = screen.current_orientation
+
+for i in range(1, 5):
+    pos = abs((start_pos - i*90) % 360)
+    screen.rotate_to(pos)
+    time.sleep(1.5)
+```
```

### Comparing `rotate-screen-0.1.4/setup.py` & `rotate-screen-0.1.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import os
-from setuptools import find_packages, setup
-
-NAME = 'rotate-screen'
-DESCRIPTION = 'A small Python package for rotating the screen.'
-URL = 'https://github.com/danny-burrows/rotate-screen'
-EMAIL = 'dannyburrows@protonmail.com'
-AUTHOR = 'Danny Burrows'
-REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.1.4'
-
-INSTALL_REQUIRES = [
-    "pywin32;platform_system=='Windows'"
-]
-
-# Optional package for the examples...
-EXTRAS = {
-    'shortcuts_example': ['keyboard']
-}
-
-here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    install_requires=INSTALL_REQUIRES,
-    extras_require=EXTRAS,
-    license='MIT',
-    classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: Microsoft :: Windows',
-        'Topic :: Desktop Environment',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12'
-    ]
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import os
+from setuptools import find_packages, setup
+
+NAME = 'rotate-screen'
+DESCRIPTION = 'A small Python package for rotating the screen.'
+URL = 'https://github.com/danny-burrows/rotate-screen'
+EMAIL = 'dannyburrows@protonmail.com'
+AUTHOR = 'Danny Burrows'
+REQUIRES_PYTHON = '>=3.7.0'
+VERSION = '0.1.5'
+
+INSTALL_REQUIRES = [
+    "pywin32;platform_system=='Windows'"
+]
+
+# Optional package for the examples...
+EXTRAS = {
+    'shortcuts_example': ['keyboard']
+}
+
+here = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name=NAME,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    install_requires=INSTALL_REQUIRES,
+    extras_require=EXTRAS,
+    license='MIT',
+    classifiers=[
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: Microsoft :: Windows',
+        'Topic :: Desktop Environment',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12'
+    ]
+)
```

