# Comparing `tmp/NeuroRuler-1.0.1.tar.gz` & `tmp/NeuroRuler-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuroRuler-1.0.1.tar", last modified: Sun May  7 19:18:51 2023, max compression
+gzip compressed data, was "NeuroRuler-1.7.tar", last modified: Sat Apr 15 15:33:02 2023, max compression
```

## Comparing `NeuroRuler-1.0.1.tar` & `NeuroRuler-1.7.tar`

### file list

```diff
@@ -1,79 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.042351 NeuroRuler-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.026351 NeuroRuler-1.0.1/NeuroRuler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.026351 NeuroRuler-1.0.1/NeuroRuler/CLI/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/CLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/CLI/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.026351 NeuroRuler-1.0.1/NeuroRuler/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    49206 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    53000 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/mainwindow.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.026351 NeuroRuler-1.0.1/NeuroRuler/GUI/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/static/nr_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.026351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.030351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark/dark.json
--rw-r--r--   0 runner    (1001) docker     (123)   295673 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    61704 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark/stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.030351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-green/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-green/dark-green.json
--rw-r--r--   0 runner    (1001) docker     (123)   295809 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-green/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    62726 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-green/stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.030351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-nr/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-nr/dark-nr.json
--rw-r--r--   0 runner    (1001) docker     (123)   295739 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-nr/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    62210 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-nr/stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.030351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-purple/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-purple/dark-purple.json
--rw-r--r--   0 runner    (1001) docker     (123)   295869 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-purple/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    62908 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/dark-purple/stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.034351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light/light.json
--rw-r--r--   0 runner    (1001) docker     (123)   296029 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    62633 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light/stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.034351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-green/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-green/light-green.json
--rw-r--r--   0 runner    (1001) docker     (123)   296171 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-green/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    63613 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-green/stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.034351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-nr/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-nr/light-nr.json
--rw-r--r--   0 runner    (1001) docker     (123)   296097 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-nr/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    63097 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-nr/stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.038351 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-purple/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-purple/light-purple.json
--rw-r--r--   0 runner    (1001) docker     (123)   296221 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-purple/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    63835 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/GUI/themes/light-purple/stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.038351 NeuroRuler-1.0.1/NeuroRuler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/cli_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/gui_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/img_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/imgproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/NeuroRuler/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.026351 NeuroRuler-1.0.1/NeuroRuler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-07 19:18:51.000000 NeuroRuler-1.0.1/NeuroRuler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-07 19:18:51.000000 NeuroRuler-1.0.1/NeuroRuler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:18:51.000000 NeuroRuler-1.0.1/NeuroRuler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-07 19:18:51.000000 NeuroRuler-1.0.1/NeuroRuler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 19:18:51.000000 NeuroRuler-1.0.1/NeuroRuler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-07 19:18:51.038351 NeuroRuler-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-07 19:18:37.000000 NeuroRuler-1.0.1/cli_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/gui_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 19:18:51.042351 NeuroRuler-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:18:51.038351 NeuroRuler-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/tests/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/tests/test_algorithm_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/tests/test_img_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/tests/test_imgproc.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-07 19:18:40.000000 NeuroRuler-1.0.1/tests/test_unittest.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.396332 NeuroRuler-1.7/
+-rw-r--r--   0 jesse      (501) staff       (20)     1105 2023-04-03 23:13:14.000000 NeuroRuler-1.7/LICENSE
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.394270 NeuroRuler-1.7/NeuroRuler.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)     3910 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)      313 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)      142 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        4 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/top_level.txt
+-rw-r--r--   0 jesse      (501) staff       (20)     3910 2023-04-15 15:33:02.396123 NeuroRuler-1.7/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     2794 2023-04-15 13:56:33.000000 NeuroRuler-1.7/README.md
+-rw-r--r--   0 jesse      (501) staff       (20)     1445 2023-04-15 15:03:14.000000 NeuroRuler-1.7/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-04-15 15:33:02.396397 NeuroRuler-1.7/setup.cfg
+-rw-r--r--   0 jesse      (501) staff       (20)     2114 2023-04-15 15:26:51.000000 NeuroRuler-1.7/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.392259 NeuroRuler-1.7/src/
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.395072 NeuroRuler-1.7/src/GUI/
+-rw-r--r--   0 jesse      (501) staff       (20)     1622 2023-04-15 15:27:32.000000 NeuroRuler-1.7/src/GUI/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6001 2023-04-15 13:24:15.000000 NeuroRuler-1.7/src/GUI/helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)    39894 2023-04-15 13:38:34.000000 NeuroRuler-1.7/src/GUI/main.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.395671 NeuroRuler-1.7/tests/
+-rw-r--r--   0 jesse      (501) staff       (20)     2707 2023-04-15 13:24:15.000000 NeuroRuler-1.7/tests/test_img_helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)    12447 2023-04-15 13:38:34.000000 NeuroRuler-1.7/tests/test_imgproc.py
```

### Comparing `NeuroRuler-1.0.1/LICENSE` & `NeuroRuler-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `NeuroRuler-1.0.1/NeuroRuler/GUI/__init__.py` & `NeuroRuler-1.7/src/GUI/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """After installing NeuroRuler via pip, the functions here are importable like so
 
-from NeuroRuler import {function}
+from {package_name} import gui
 
-where NeuroRuler is the name of the package this __init__.py file is in."""
+Currently, the package name is GUI (TODO: Change this)"""
 
 import sys
 import os
-import shutil
-from pathlib import Path
-import pkg_resources
-import NeuroRuler.GUI.main as main
-import NeuroRuler.utils.parser as parser
-import NeuroRuler.utils.constants as constants
+import src.GUI.main as main
+import src.utils.parser as parser
 
+# TODO: Modify when refactoring
+__version__ = "1.7"
 
 def gui() -> None:
-    """Run GUI.
-
-    Will create ``gui_config.json`` using package's ``gui_config.json`` if it doesn't already exist.
-    """
+    """Start GUI."""
     # Source: https://stackoverflow.com/questions/5047734/in-osx-change-application-name-from-python
     if sys.platform.startswith("darwin"):
         # Set app name, if PyObjC is installed
         # Python 2 has PyObjC preinstalled
         # Python 3: pip3 install pyobjc-framework-Cocoa
         try:
             from Foundation import NSBundle
@@ -44,16 +39,15 @@
     try:
         # For Windows.
         # App icon works without this on macOS.
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
     except:
         pass
 
-    if not constants.JSON_GUI_CONFIG_PATH.exists():
-        json_gui_from_package: Path = Path(
-            pkg_resources.resource_filename(__name__, "../../gui_config.json")
-        )
-        shutil.copy(json_gui_from_package, constants.JSON_GUI_CONFIG_PATH)
-
-    parser.parse_gui_config()
+    parser.parse_config_json()
     parser.parse_gui_cli()
     main.main()
+
+
+def GUI() -> None:
+    """Alias for gui()."""
+    gui()
```

### Comparing `NeuroRuler-1.0.1/NeuroRuler/GUI/helpers.py` & `NeuroRuler-1.7/src/GUI/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""GUI helper functions."""
+"""GUI helper functions.
+
+Note, importing PyQt6 in any file that's imported by a test file will cause an error."""
 
 import platform
 import string
 from typing import Union
 
 import SimpleITK as sitk
 import numpy as np
@@ -21,56 +23,56 @@
     QMessageBox,
 )
 from PyQt6.QtCore import QSize
 from PyQt6.QtCore import Qt
 
 import qimage2ndarray
 
-import NeuroRuler.utils.exceptions as exceptions
-import NeuroRuler.utils.gui_settings as user_settings
-from NeuroRuler.utils.constants import deprecated
+import src.utils.exceptions as exceptions
+import src.utils.user_settings as user_settings
+from src.utils.constants import deprecated
 
 MACOS: bool = "macOS" in platform.platform()
 WINDOW_TITLE_PADDING: int = 12
 """Used in InformationDialog to add width to the dialog to prevent the window title from being truncated."""
 
 
 # tl;dr QColor can have alpha (e.g., if we wanted contour color to be transparent)
 # but we don't have a need for it so don't support it.
 # Call hasAlphaChannel() on many of the QImage's we're working with results in False.
 # qimage2ndarray supports scalar/gray + alpha and RGB + alpha, but perhaps the numpy arrays
 # we get from sitk.Image don't have alpha. We don't need to go to the effort of adding alpha.
 def string_to_QColor(name_or_hex: str) -> QColor:
-    """Convert a name (e.g. red) or 6-hexit rrggbb string to a ``QColor``.
+    """Convert a name (e.g. red) or 6-hexit rrggbb string to a `QColor`.
 
     :param name_or_hex: name of color (e.g. blue) or rrggbb (hexits)
     :type name_or_hex: str
     :return: QColor
     :rtype: QColor
-    :raise: exceptions.InvalidColor if ``name_or_hex`` not in specified formats"""
+    :raise: exceptions.InvalidColor if `name_or_hex` not in specified formats"""
     if name_or_hex.isalpha():
         return QColor(name_or_hex)
     if not all(char in string.hexdigits for char in name_or_hex):
         raise exceptions.InvalidColor(name_or_hex)
 
     channels: bytes = bytes.fromhex(name_or_hex)
     if len(channels) == 3:
         return QColor(channels[0], channels[1], channels[2])
     else:
         raise exceptions.InvalidColor(name_or_hex)
 
 
 def mask_QImage(q_img: QImage, binary_mask: np.ndarray, color: QColor) -> None:
-    """Given 2D ``q_img`` and 2D ``binary_mask`` of the same shape, apply ``binary_mask`` on ``q_img``
-    to change ``q_img`` pixels corresponding to ``binary_mask``=1 to ``color``. Mutates ``q_img``.
+    """Given 2D `q_img` and 2D `binary_mask` of the same shape, apply `binary_mask` on `q_img`
+    to change `q_img` pixels corresponding to `binary_mask`=1 to `color`. Mutates `q_img`.
 
     QImage and numpy use [reversed w,h order](https://stackoverflow.com/a/68220805/18479243).
 
     This function checks that
-    ``q_img.size().width() == binary_mask.shape[0]`` and ``q_img.size().height() == binary_mask.shape[1]``.
+    `q_img.size().width() == binary_mask.shape[0]` and `q_img.size().height() == binary_mask.shape[1]`.
 
     :param q_img:
     :type q_img: QImage
     :param binary_mask: 0|1 elements
     :type binary_mask: np.ndarray
     :param color:
     :type color: QColor
```

### Comparing `NeuroRuler-1.0.1/NeuroRuler/GUI/main.py` & `NeuroRuler-1.7/src/GUI/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-"""Defines ``MainWindow`` and ``main()``, the entrypoint of the GUI.
+"""Defines MainWindow and main(), the entrypoint of the GUI.
 
-Loads ``NeuroRuler/GUI/mainwindow.ui``, made in QtDesigner.
+Loads `src/GUI/mainwindow.ui`, made in QtDesigner.
 
-Loads ``.qss`` stylesheets and ``resources.py`` (icons) files, generated
-by BreezeStyleSheets. Our fork of the repo: https://github.com/NIRALUser/BreezeStyleSheets.
+Loads `.qss` stylesheets and `resources.py` (icons) files, generated
+by BreezeStyleSheets. Our fork of the repo: https://github.com/COMP523TeamD/BreezeStyleSheets.
 
 If adding a new GUI element (in the GUI or in the menubar, whatever), you'll have to modify
 modify __init__ and settings_view_toggle.
 
 Edge cases: If this element should be disabled after enable_elements or enabled after disable_elements,
 then you will need to modify those."""
 
 
 import importlib
 import sys
 import os
-import json
-import re
 import webbrowser
 from pathlib import Path
 from typing import Union
 
 import SimpleITK as sitk
 import numpy as np
-from typing import Any
 
 from PyQt6 import QtGui, QtCore
 from PyQt6.QtGui import QPixmap, QAction, QImage, QIcon, QResizeEvent
 from PyQt6.QtWidgets import (
     QApplication,
     QDialog,
     QLabel,
@@ -38,84 +35,77 @@
     QWidget,
     QMessageBox,
 )
 from PyQt6.uic.load_ui import loadUi
 from PyQt6.QtCore import Qt, QSize
 
 import pprint
-import pkg_resources
-from NeuroRuler.utils.constants import View, ThresholdFilter
-import NeuroRuler.utils.constants as constants
+from src.utils.constants import View, ThresholdFilter
+import src.utils.constants as constants
 
 # Note, do not use imports like
-# from NeuroRuler.utils.global_vars import IMAGE_DICT
+# from src.utils.global_vars import IMAGE_DICT
 # This would make the global variables not work
-import NeuroRuler.utils.global_vars as global_vars
-import NeuroRuler.utils.imgproc as imgproc
-import NeuroRuler.utils.gui_settings as settings
-from NeuroRuler.GUI.helpers import (
+import src.utils.global_vars as global_vars
+import src.utils.imgproc as imgproc
+import src.utils.user_settings as user_settings
+from src.GUI.helpers import (
     string_to_QColor,
     mask_QImage,
     sitk_slice_to_qimage,
     ErrorMessageBox,
+    InformationMessageBox,
     InformationDialog,
 )
 
-from NeuroRuler.utils.img_helpers import (
+from src.utils.img_helpers import (
     initialize_globals,
     update_images,
     get_curr_image,
     get_curr_image_size,
     get_curr_rotated_slice,
     get_curr_smooth_slice,
     get_curr_metadata,
     get_curr_binary_thresholded_slice,
     get_curr_otsu_slice,
     get_curr_physical_units,
     get_curr_path,
-    get_all_paths,
     get_curr_properties_tuple,
     get_middle_dimension,
 )
 
-import NeuroRuler.utils.img_helpers as img_helpers
+import src.utils.img_helpers as img_helpers
 
 
-PATH_TO_UI_FILE: Path = Path("NeuroRuler") / "GUI" / "mainwindow.ui"
-if not PATH_TO_UI_FILE.exists():
-    PATH_TO_UI_FILE = Path(
-        pkg_resources.resource_filename("NeuroRuler.GUI", "mainwindow.ui")
-    )
-PATH_TO_NR_LOGO: Path = Path("NeuroRuler") / "GUI" / "static" / "nr_logo.png"
-if not PATH_TO_NR_LOGO.exists():
-    PATH_TO_NR_LOGO = Path(
-        pkg_resources.resource_filename("NeuroRuler.GUI", "static/nr_logo.png")
-    )
+PATH_TO_UI_FILE: Path = Path("src") / "GUI" / "mainwindow.ui"
+PATH_TO_HCT_LOGO: Path = Path("src") / "GUI" / "static" / "hct_logo.png"
 
 SETTINGS_VIEW_ENABLED: bool = True
 """Whether the user is able to adjust settings (settings screen) or not
 (circumference and contoured image screen)."""
 
 DEFAULT_CIRCUMFERENCE_LABEL_TEXT: str = "Calculated Circumference: N/A"
 DEFAULT_IMAGE_PATH_LABEL_TEXT: str = "Image path"
-GITHUB_LINK: str = "https://github.com/NIRALUser/NeuroRuler"
-DOCUMENTATION_LINK: str = "https://NeuroRuler.readthedocs.io/en/latest/"
+GITHUB_LINK: str = "https://github.com/COMP523TeamD/HeadCircumferenceTool"
+DOCUMENTATION_LINK: str = "https://headcircumferencetool.readthedocs.io/en/latest/"
 DEFAULT_IMAGE_TEXT: str = "Select images using File > Open!"
 DEFAULT_IMAGE_NUM_LABEL_TEXT: str = "Image 0 of 0"
 DEFAULT_IMAGE_STATUS_TEXT: str = "Image path is displayed here."
 
+# We assume units are millimeters if we can't find units in metadata
+MESSAGE_TO_SHOW_IF_UNITS_NOT_FOUND: str = "millimeters (mm)"
+
 UNSCALED_QPIXMAP: QPixmap
 """Unscaled QPixmap from which the scaled version is rendered in the GUI.
 
 When any slice (rotated, smoothed, previewed) is rendered from an unscaled QImage, this variable is set to the
 QPixmap generated from that unscaled QImage.
 
 This variable will not change on resizeEvent. resizeEvent will scale this. Otherwise, if scaling
 self.image's pixmap (which is already scaled), there would be loss of detail."""
-OUTPUT_SLICE_EXTENSION: str = "png"
 
 
 class MainWindow(QMainWindow):
     """Main window of the application.
 
     Settings mode and circumference mode."""
 
@@ -135,22 +125,23 @@
         self.action_github.triggered.connect(lambda: webbrowser.open(GITHUB_LINK))
         self.action_documentation.triggered.connect(
             lambda: webbrowser.open(DOCUMENTATION_LINK)
         )
         self.action_show_credits.triggered.connect(
             lambda: information_dialog(
                 "Credits",
-                'Credit to Jesse Wei, Madison Lester, Peifeng "Hank" He, Eric Schneider, and Martin Styner.\n\nUniversity of North Carolina at Chapel Hill, 2023. See the GitHub page for more info.',
+                'Credit to Jesse Wei, Madison Lester, Peifeng "Hank" He, Eric Schneider, and Martin Styner.',
             )
         )
-        self.action_show_dimensions.triggered.connect(display_dimensions)
-        self.action_show_properties.triggered.connect(display_properties)
-        self.action_show_direction.triggered.connect(display_direction)
-        self.action_show_spacing.triggered.connect(display_spacing)
-        self.action_export_json.triggered.connect(self.export_json)
+        self.action_test_stuff.triggered.connect(self.test_stuff)
+        self.action_print_metadata.triggered.connect(display_metadata)
+        self.action_print_dimensions.triggered.connect(display_dimensions)
+        self.action_print_properties.triggered.connect(display_properties)
+        self.action_print_direction.triggered.connect(display_direction)
+        self.action_print_spacing.triggered.connect(display_spacing)
         self.action_export_png.triggered.connect(
             lambda: self.export_curr_slice_as_img("png")
         )
         self.action_export_jpg.triggered.connect(
             lambda: self.export_curr_slice_as_img("jpg")
         )
         self.action_export_bmp.triggered.connect(
@@ -161,15 +152,14 @@
         )
         self.action_export_xbm.triggered.connect(
             lambda: self.export_curr_slice_as_img("xbm")
         )
         self.action_export_xpm.triggered.connect(
             lambda: self.export_curr_slice_as_img("xpm")
         )
-        self.action_import_image_settings.triggered.connect(self.import_json)
         self.next_button.clicked.connect(self.next_img)
         self.previous_button.clicked.connect(self.previous_img)
         self.apply_button.clicked.connect(self.settings_export_view_toggle)
         self.x_slider.valueChanged.connect(self.rotate_x)
         self.y_slider.valueChanged.connect(self.rotate_y)
         self.z_slider.valueChanged.connect(self.rotate_z)
         self.slice_slider.valueChanged.connect(self.slice_update)
@@ -178,16 +168,14 @@
         self.otsu_radio_button.clicked.connect(self.disable_binary_threshold_inputs)
         self.binary_radio_button.clicked.connect(self.enable_binary_threshold_inputs)
         self.threshold_preview_button.clicked.connect(self.render_threshold)
         self.x_view_radio_button.clicked.connect(self.update_view)
         self.y_view_radio_button.clicked.connect(self.update_view)
         self.z_view_radio_button.clicked.connect(self.update_view)
 
-        self.export_button.clicked.connect(self.export_json)
-
     def enable_elements(self) -> None:
         """Called after File > Open.
 
         Enables GUI elements. Explicitly disables some (e.g., Export CSV menu item and
         binary threshold inputs, since Otsu is default).
 
         :return: None
@@ -196,15 +184,15 @@
         for widget in self.findChildren(QWidget):
             widget.setEnabled(True)
 
         # Menu stuff
         for widget in self.findChildren(QAction):
             widget.setEnabled(True)
 
-        self.action_export_json.setEnabled(not SETTINGS_VIEW_ENABLED)
+        self.action_export_csv.setEnabled(not SETTINGS_VIEW_ENABLED)
         self.export_button.setEnabled(not SETTINGS_VIEW_ENABLED)
         self.disable_binary_threshold_inputs()
 
     def enable_binary_threshold_inputs(self) -> None:
         """Called when Binary filter button is clicked.
 
         Restore binary input box.
@@ -240,25 +228,25 @@
             # axial slice. For example, after clicking coronal and setting X rotation to 90,
             # clicking axial will not show an axial slice.
             # We could just not change the view and re-orient when clicking Apply if this is a valid use case (probably isn't).
             # TODO: Check with Styner
             self.set_view_z()
             self.orient_curr_image()
 
-            self.update_smoothing_settings(True)
-            self.update_binary_filter_settings(True)
+            self.update_smoothing_settings()
+            self.update_binary_filter_settings()
+            self.apply_button.setText("Adjust")
             # Ignore the type annotation warning here.
             # render_curr_slice() must return np.ndarray since not settings_view_enabled here
             binary_contour_slice: np.ndarray = self.render_curr_slice()
             self.render_circumference(binary_contour_slice)
 
-        # Open button is always enabled.
-        # If pressing it in circumference mode, then browse_files() will toggle to settings view.
-        self.action_open.setEnabled(True)
-        self.action_import_image_settings.setEnabled(settings_view_enabled)
+        # TODO: Call enable_elements and then a disable method (code another one, and it'd be short)
+        # If not settings_view_enabled
+        self.action_open.setEnabled(settings_view_enabled)
         self.action_add_images.setEnabled(settings_view_enabled)
         self.action_remove_image.setEnabled(settings_view_enabled)
         self.x_slider.setEnabled(settings_view_enabled)
         self.y_slider.setEnabled(settings_view_enabled)
         self.z_slider.setEnabled(settings_view_enabled)
         self.slice_slider.setEnabled(settings_view_enabled)
         self.x_rotation_label.setEnabled(settings_view_enabled)
@@ -270,15 +258,15 @@
         self.otsu_radio_button.setEnabled(settings_view_enabled)
         self.binary_radio_button.setEnabled(settings_view_enabled)
         self.lower_threshold.setEnabled(settings_view_enabled)
         self.lower_threshold_input.setEnabled(settings_view_enabled)
         self.upper_threshold.setEnabled(settings_view_enabled)
         self.upper_threshold_input.setEnabled(settings_view_enabled)
         self.threshold_preview_button.setEnabled(settings_view_enabled)
-        self.action_export_json.setEnabled(not settings_view_enabled)
+        self.action_export_csv.setEnabled(not settings_view_enabled)
         self.circumference_label.setEnabled(not settings_view_enabled)
         self.export_button.setEnabled(not settings_view_enabled)
         self.smoothing_preview_button.setEnabled(settings_view_enabled)
         self.conductance_parameter_label.setEnabled(settings_view_enabled)
         self.conductance_parameter_input.setEnabled(settings_view_enabled)
         self.smoothing_iterations_label.setEnabled(settings_view_enabled)
         self.smoothing_iterations_input.setEnabled(settings_view_enabled)
@@ -329,53 +317,41 @@
         self.image.setText(DEFAULT_IMAGE_TEXT)
         self.image.setStatusTip(DEFAULT_IMAGE_STATUS_TEXT)
         self.image_path_label.setText(DEFAULT_IMAGE_PATH_LABEL_TEXT)
         self.image_num_label.setText(DEFAULT_IMAGE_NUM_LABEL_TEXT)
         self.apply_button.setText("Apply")
         self.z_view_radio_button.setChecked(True)
 
-    def browse_files(self, extend: bool, path=None) -> None:
+    def browse_files(self, extend: bool) -> None:
         """Called after File > Open or File > Add Images.
 
-        If ``extend``, then ``IMAGE_DICT`` will be updated with new images.
+        If `extend`, then `IMAGE_DICT` will be updated with new images.
 
-        Else, ``IMAGE_DICT`` will be cleared and
+        Else, `IMAGE_DICT` will be cleared and
         (re)initialized (e.g. when choosing files for the first time or re-opening).
 
         Opens file menu.
 
-        Renders various elements depending on the value of ``extend``.
-
-        If called in circumference mode, then will toggle to settings mode.
+        Renders various elements depending on the value of `extend`.
 
         :param extend: Whether to clear IMAGE_DICT and (re)initialize or add images to it. Determines which GUI elements are rendered.
-        :param path: Used for unit testing, when only one path is imported. Normally, the path(s) are selected by user in a QFileDialog.
         :type extend: bool
         :return: None"""
-        # If called in circumference mode, then toggle to settings mode.
-        if not SETTINGS_VIEW_ENABLED:
-            self.settings_export_view_toggle()
+        file_filter: str = "MRI images " + str(constants.SUPPORTED_EXTENSIONS).replace(
+            "'", ""
+        ).replace(",", "")
 
-        if path is None:
-            file_filter: str = "MRI images " + str(
-                constants.SUPPORTED_IMAGE_EXTENSIONS
-            ).replace("'", "").replace(",", "")
-
-            files = QFileDialog.getOpenFileNames(
-                self,
-                "Open files",
-                str(settings.FILE_BROWSER_START_DIR),
-                file_filter,
-            )
-            # list[str]
-            path_list = files[0]
-            if len(path_list) == 0:
-                return
-        else:
-            path_list = [path]
+        files = QFileDialog.getOpenFileNames(
+            self, "Open files", str(user_settings.FILE_BROWSER_START_DIR), file_filter
+        )
+
+        # list[str]
+        path_list = files[0]
+        if len(path_list) == 0:
+            return
 
         # Convert to list[Path]. Slight inefficiency but worth.
         path_list = list(map(Path, path_list))
 
         differing_images: list[Path]
 
         if not extend:
@@ -437,98 +413,82 @@
         global_vars.VIEW = constants.View.Z
         # TODO: Uncheck x and y are technically unnecessary since these 3 buttons in the view_button_group have
         # autoExclusive=True
         self.x_view_radio_button.setChecked(False)
         self.y_view_radio_button.setChecked(False)
         self.z_view_radio_button.setChecked(True)
 
-    def update_smoothing_settings(self, set_global_vars_to_GUI_text: bool) -> None:
-        """Update smoothing text in the GUI and set SMOOTHING_FILTER parameters.
+    def update_smoothing_settings(self) -> None:
+        """Updates global smoothing settings.
 
-        :param set_global_vars_to_GUI_text: If True, will first try to modify global_vars variables to the text in the GUI before updating GUI text and filter parameters. If False, will not do so.
-        :type set_global_vars_to_GUI_text: bool
         :return: None
         """
-        if set_global_vars_to_GUI_text:
-            try:
-                global_vars.CONDUCTANCE_PARAMETER = float(
-                    self.conductance_parameter_input.displayText()
-                )
-            except ValueError:
-                if settings.DEBUG:
-                    print("Conductance must be a float!")
+        conductance: str = self.conductance_parameter_input.displayText()
+        try:
+            global_vars.CONDUCTANCE_PARAMETER = float(conductance)
+        except ValueError:
+            if user_settings.DEBUG:
+                print("Conductance must be a float!")
         self.conductance_parameter_input.setText(str(global_vars.CONDUCTANCE_PARAMETER))
         self.conductance_parameter_input.setPlaceholderText(
             str(global_vars.CONDUCTANCE_PARAMETER)
         )
         global_vars.SMOOTHING_FILTER.SetConductanceParameter(
             global_vars.CONDUCTANCE_PARAMETER
         )
 
-        if set_global_vars_to_GUI_text:
-            try:
-                global_vars.SMOOTHING_ITERATIONS = int(
-                    self.smoothing_iterations_input.displayText()
-                )
-            except ValueError:
-                if settings.DEBUG:
-                    print("Iterations must be an integer!")
+        iterations: str = self.smoothing_iterations_input.displayText()
+        try:
+            global_vars.SMOOTHING_ITERATIONS = int(iterations)
+        except ValueError:
+            if user_settings.DEBUG:
+                print("Iterations must be an integer!")
         self.smoothing_iterations_input.setText(str(global_vars.SMOOTHING_ITERATIONS))
         self.smoothing_iterations_input.setPlaceholderText(
             str(global_vars.SMOOTHING_ITERATIONS)
         )
         global_vars.SMOOTHING_FILTER.SetNumberOfIterations(
             global_vars.SMOOTHING_ITERATIONS
         )
 
-        if set_global_vars_to_GUI_text:
-            try:
-                global_vars.TIME_STEP = float(self.time_step_input.displayText())
-            except ValueError:
-                if settings.DEBUG:
-                    print("Time step must be a float!")
+        time_step: str = self.time_step_input.displayText()
+        try:
+            global_vars.TIME_STEP = float(time_step)
+        except ValueError:
+            if user_settings.DEBUG:
+                print("Time step must be a float!")
         self.time_step_input.setText(str(global_vars.TIME_STEP))
         self.time_step_input.setPlaceholderText(str(global_vars.TIME_STEP))
         global_vars.SMOOTHING_FILTER.SetTimeStep(global_vars.TIME_STEP)
 
-    def update_binary_filter_settings(self, set_global_vars_to_GUI_text: bool) -> None:
-        """Updates binary threshold filter text in the GUI and set BINARY_THRESHOLD_FILTER parameters.
+    def update_binary_filter_settings(self) -> None:
+        """Updates global binary filter settings.
 
-        :param set_global_vars_to_GUI_text: If True, will first try to modify global_vars variables to the text in the GUI before updating GUI text and filter parameters. If False, will not do so.
-        :type set_global_vars_to_GUI_text: bool
         :return: None
         """
-        if set_global_vars_to_GUI_text:
-            try:
-                global_vars.LOWER_BINARY_THRESHOLD = float(
-                    self.lower_threshold_input.displayText()
-                )
-            except ValueError:
-                pass
-        self.lower_threshold_input.setText(str(global_vars.LOWER_BINARY_THRESHOLD))
-        self.lower_threshold_input.setPlaceholderText(
-            str(global_vars.LOWER_BINARY_THRESHOLD)
-        )
+        lower_threshold: str = self.lower_threshold_input.displayText()
+        try:
+            global_vars.LOWER_THRESHOLD = float(lower_threshold)
+        except ValueError:
+            pass
+        self.lower_threshold_input.setText(str(global_vars.LOWER_THRESHOLD))
+        self.lower_threshold_input.setPlaceholderText(str(global_vars.LOWER_THRESHOLD))
         global_vars.BINARY_THRESHOLD_FILTER.SetLowerThreshold(
-            global_vars.LOWER_BINARY_THRESHOLD
+            global_vars.LOWER_THRESHOLD
         )
 
-        if set_global_vars_to_GUI_text:
-            try:
-                global_vars.UPPER_BINARY_THRESHOLD = float(
-                    self.upper_threshold_input.displayText()
-                )
-            except ValueError:
-                pass
-        self.upper_threshold_input.setText(str(global_vars.UPPER_BINARY_THRESHOLD))
-        self.upper_threshold_input.setPlaceholderText(
-            str(global_vars.UPPER_BINARY_THRESHOLD)
-        )
+        upper_threshold: str = self.upper_threshold_input.displayText()
+        try:
+            global_vars.UPPER_THRESHOLD = float(upper_threshold)
+        except ValueError:
+            pass
+        self.upper_threshold_input.setText(str(global_vars.UPPER_THRESHOLD))
+        self.upper_threshold_input.setPlaceholderText(str(global_vars.UPPER_THRESHOLD))
         global_vars.BINARY_THRESHOLD_FILTER.SetUpperThreshold(
-            global_vars.UPPER_BINARY_THRESHOLD
+            global_vars.UPPER_THRESHOLD
         )
 
     def render_scaled_qpixmap_from_qimage(self, q_img: QImage) -> None:
         """Convert q_img to QPixmap and set self.image's pixmap to that pixmap scaled to self.image's size.
 
         Sets UNSCALED_PIXMAP to the unscaled pixmap generated from the q_img.
 
@@ -563,23 +523,23 @@
             )
         QMainWindow.resizeEvent(self, event)
 
     def render_curr_slice(self) -> Union[np.ndarray, None]:
         """Resamples the currently selected image using its rotation and slice settings,
         then renders the resulting slice (scaled to the size of self.image) in the GUI.
 
-        DOES NOT set text for ``image_num_label`` and file path labels.
+        DOES NOT set text for `image_num_label` and file path labels.
 
-        If ``not SETTINGS_VIEW_ENABLED``, also calls ``imgproc.contour()`` and outlines
+        If `not SETTINGS_VIEW_ENABLED`, also calls `imgproc.contour()` and outlines
         the contour of the QImage (mutating it).
 
-        Additionally, also returns a view of the binary contoured slice if ``not SETTINGS_VIEW_ENABLED``.
+        Additionally, also returns a view of the binary contoured slice if `not SETTINGS_VIEW_ENABLED`.
         This saves work when computing circumference.
 
-        :return: np.ndarray if ``not SETTINGS_VIEW_ENABLED`` else None
+        :return: np.ndarray if `not SETTINGS_VIEW_ENABLED` else None
         :rtype: np.ndarray or None"""
 
         if not SETTINGS_VIEW_ENABLED:
             self.set_view_z()
 
         rotated_slice: sitk.Image = get_curr_rotated_slice()
         q_img: QImage = sitk_slice_to_qimage(rotated_slice)
@@ -594,38 +554,38 @@
                 binary_contour_slice: np.ndarray = imgproc.contour(
                     rotated_slice, ThresholdFilter.Binary
                 )
             rv_dummy_var = binary_contour_slice
             mask_QImage(
                 q_img,
                 np.transpose(binary_contour_slice),
-                string_to_QColor(settings.CONTOUR_COLOR),
+                string_to_QColor(user_settings.CONTOUR_COLOR),
             )
 
         elif global_vars.VIEW != constants.View.Z:
             z_indicator: np.ndarray = np.zeros(
                 (rotated_slice.GetSize()[1], rotated_slice.GetSize()[0])
             )
             z_indicator[get_curr_image_size()[2] - global_vars.SLICE - 1, :] = 1
             mask_QImage(
                 q_img,
                 np.transpose(z_indicator),
-                string_to_QColor(settings.CONTOUR_COLOR),
+                string_to_QColor(user_settings.CONTOUR_COLOR),
             )
 
         self.render_scaled_qpixmap_from_qimage(q_img)
 
         if not SETTINGS_VIEW_ENABLED:
             return rv_dummy_var
 
     def render_smooth_slice(self) -> None:
         """Renders smooth slice in GUI. Allows user to preview result of smoothing settings.
 
         :return: None"""
-        self.update_smoothing_settings(True)
+        self.update_smoothing_settings()
         # Preview should apply filter only on axial slice
         self.set_view_z()
         smooth_slice: sitk.Image = get_curr_smooth_slice()
         q_img: QImage = sitk_slice_to_qimage(smooth_slice)
         self.render_scaled_qpixmap_from_qimage(q_img)
 
     def render_threshold(self) -> None:
@@ -633,74 +593,38 @@
 
         :return: None"""
         # Preview should apply filter only on axial slice
         self.set_view_z()
         if self.otsu_radio_button.isChecked():
             filter_img: sitk.Image = get_curr_otsu_slice()
         else:
-            self.update_binary_filter_settings(True)
+            self.update_binary_filter_settings()
             filter_img: sitk.Image = get_curr_binary_thresholded_slice()
         q_img: QImage = sitk_slice_to_qimage(filter_img)
         self.render_scaled_qpixmap_from_qimage(q_img)
 
-    def render_circumference(self, binary_contour_slice: np.ndarray) -> float:
+    def render_circumference(self, binary_contour_slice: np.ndarray) -> None:
         """Called after pressing Apply or when
         (not SETTINGS_VIEW_ENABLED and (pressing Next or Previous or Remove Image))
 
         Computes circumference from binary_contour_slice and renders circumference label.
 
         binary_contour_slice is always the return value of render_curr_slice since render_curr_slice must have
         already been called. If calling this function, render_curr_slice must have been called first.
 
-        :param binary_contour_slice: Result of previously calling render_curr_slice when ``not SETTINGS_VIEW_ENABLED``
+        :param binary_contour_slice: Result of previously calling render_curr_slice when `not SETTINGS_VIEW_ENABLED`
         :type binary_contour_slice: np.ndarray
-        :return: circumference
-        :rtype: float"""
+        :return: None"""
         if SETTINGS_VIEW_ENABLED:
             raise Exception("Rendering circumference label when SETTINGS_VIEW_ENABLED")
         units: Union[str, None] = get_curr_physical_units()
-
-        # Euler3D rotation has no effect on spacing (see unit test). This is the correct spacing
-        # This is also the same as get_curr_rotated_slice().GetSpacing(), just without index [2]
-        spacing: tuple = get_curr_image().GetSpacing()
-
-        if settings.DEBUG:
-            print(f"Computing circumference, and this is the spacing: {spacing}")
-
-        # TODO
-        # binary_contour_slice is the transpose of the rotated_slice
-        # Thus, should pass spacing values in the reverse order?
-        circumference: float = imgproc.length_of_contour_with_spacing(
-            binary_contour_slice, spacing[0], spacing[1]
-        )
-        # circumference: float = imgproc.length_of_contour(binary_contour_slice)
+        circumference: float = imgproc.length_of_contour(binary_contour_slice)
         self.circumference_label.setText(
-            f"Calculated Circumference: {round(circumference, constants.NUM_DIGITS_TO_ROUND_TO)} {units if units is not None else constants.MESSAGE_TO_SHOW_IF_UNITS_NOT_FOUND}"
+            f"Calculated Circumference: {round(circumference, constants.NUM_DIGITS_TO_ROUND_TO)} {units if units is not None else MESSAGE_TO_SHOW_IF_UNITS_NOT_FOUND}"
         )
-        return circumference
-
-    def toggle_setting_to_false(self) -> None:
-        """Used in testing.
-
-        Flipping the SETTINGS_VIEW_ENABLED
-
-        :return: None"""
-        global SETTINGS_VIEW_ENABLED
-        if SETTINGS_VIEW_ENABLED:
-            SETTINGS_VIEW_ENABLED = not SETTINGS_VIEW_ENABLED
-
-    def toggle_setting_to_true(self) -> None:
-        """Used in testing.
-
-        Flipping the SETTINGS_VIEW_ENABLED
-
-        :return: None"""
-        global SETTINGS_VIEW_ENABLED
-        if not SETTINGS_VIEW_ENABLED:
-            SETTINGS_VIEW_ENABLED = not SETTINGS_VIEW_ENABLED
 
     def render_image_num_and_path(self) -> None:
         """Set image_num_label, image_path_label, and status tip of the image.
 
         Called when pressing Next or Previous (next_img, prev_img), and after File > Open (browse_files).
 
         Also called when removing an image.
@@ -733,59 +657,59 @@
         self.y_rotation_label.setText(f"Y rotation: {global_vars.THETA_Y}°")
         self.z_rotation_label.setText(f"Z rotation: {global_vars.THETA_Z}°")
         self.slice_num_label.setText(f"Slice: {global_vars.SLICE}")
 
     def rotate_x(self) -> None:
         """Called when the user updates the x slider.
 
-        Render image and set ``x_rotation_label``.
+        Render image and set `x_rotation_label`.
 
         :return: None"""
         x_slider_val: int = self.x_slider.value()
         global_vars.THETA_X = x_slider_val
         self.render_curr_slice()
         self.x_rotation_label.setText(f"X rotation: {x_slider_val}°")
 
     def rotate_y(self) -> None:
         """Called when the user updates the y slider.
 
-        Render image and set ``y_rotation_label``.
+        Render image and set `y_rotation_label`.
 
         :return: None"""
         y_slider_val: int = self.y_slider.value()
         global_vars.THETA_Y = y_slider_val
         self.render_curr_slice()
         self.y_rotation_label.setText(f"Y rotation: {y_slider_val}°")
 
     def rotate_z(self) -> None:
         """Called when the user updates the z slider.
 
-        Render image and set ``z_rotation_label``.
+        Render image and set `z_rotation_label`.
 
         :return: None"""
         z_slider_val: int = self.z_slider.value()
         global_vars.THETA_Z = z_slider_val
         self.render_curr_slice()
         self.z_rotation_label.setText(f"Z rotation: {z_slider_val}°")
 
     def slice_update(self) -> None:
         """Called when the user updates the slice slider.
 
-        Render image and set ``slice_num_label``.
+        Render image and set `slice_num_label`.
 
         :return: None"""
         slice_slider_val: int = self.slice_slider.value()
         global_vars.SLICE = slice_slider_val
         self.render_curr_slice()
         self.slice_num_label.setText(f"Slice: {slice_slider_val}")
 
     def reset_settings(self) -> None:
         """Called when Reset is clicked.
 
-        Resets rotation values to 0 and slice num to the default ``int((z-1)/2)``
+        Resets rotation values to 0 and slice num to the default `int((z-1)/2)`
         for the current image, then renders current image and sliders.
 
         :return: None"""
         global_vars.THETA_X = 0
         global_vars.THETA_Y = 0
         global_vars.THETA_Z = 0
         global_vars.SLICE = get_middle_dimension(get_curr_image(), View.Z)
@@ -825,16 +749,16 @@
             self.render_circumference(binary_contour_or_none)
 
     # TODO: Due to the images now being a dict, we can
     # easily let the user remove a range of images if they want
     def remove_curr_img(self) -> None:
         """Called after File > Remove File.
 
-        Removes current image from ``IMAGE_DICT``. Since ``IMAGE_DICT`` is a reference to an image dict
-        in ``IMAGE_GROUPS``, it's removed from ``IMAGE_GROUPS`` as well.
+        Removes current image from `IMAGE_DICT`. Since `IMAGE_DICT` is a reference to an image dict
+        in `IMAGE_GROUPS`, it's removed from `IMAGE_GROUPS` as well.
 
         :return: None"""
         img_helpers.del_curr_img()
 
         if len(global_vars.IMAGE_DICT) == 0:
             self.disable_elements()
             return
@@ -848,197 +772,48 @@
 
     def test_stuff(self) -> None:
         """Connected to Debug > Test stuff. Dummy button and function for easily testing stuff.
 
         Assume that anything you put here will be overwritten freely.
 
         :return: None"""
-        self.image.setPixmap(QPixmap(f":/{settings.THEME_NAME}/help.svg"))
+        self.image.setPixmap(QPixmap(f":/{user_settings.THEME_NAME}/help.svg"))
         self.image.setStatusTip(
             "This is intentional, if it's a question mark then that's good :), means we can display icons"
         )
 
     # TODO: File name should also include circumference when not SETTINGS_VIEW_ENABLED?
     def export_curr_slice_as_img(self, extension: str) -> None:
         """Called when an Export as image menu item is clicked.
 
-        Exports ``self.image`` to ``constants.OUTPUT_DIR/image_stem/``. Thus, calling this when ``SETTINGS_VIEW_ENABLED`` will
-        save a non-contoured image. Calling this when ``not SETTINGS_VIEW_ENABLED`` will save a contoured
+        Exports `self.image` to `settings.OUTPUT_DIR/img/`. Thus, calling this when `SETTINGS_VIEW_ENABLED` will
+        save a non-contoured image. Calling this when `not SETTINGS_VIEW_ENABLED` will save a contoured
         image.
 
-        Filename has format <file_name>[_contoured].<extension>
+        Filename has format <file_name>_[contoured_]<theta_x>_<theta_y>_<theta_z>_<slice_num>.<extension>
 
-        _contoured will be in the name if ``not SETTINGS_VIEW_ENABLED``.
+        contoured_ will be in the name if `not SETTINGS_VIEW_ENABLED`.
 
         Supported formats in this function are the ones supported by QPixmap,
         namely BMP, JPG, JPEG, PNG, PPM, XBM, XPM.
 
         :param extension: BMP, JPG, JPEG, PNG, PPM, XBM, XPM
         :type extension: str
-        :param path:
-        :type path: Path
-        :return: ``None``"""
-        file_stem: str = constants.get_path_stem(get_curr_path())
-        output_path: Path = constants.OUTPUT_DIR / file_stem
-
-        if not output_path.exists():
-            output_path.mkdir()
-
+        :return: `None`"""
+        file_name = (
+            global_vars.CURR_IMAGE_INDEX + 1
+            if user_settings.EXPORTED_FILE_NAMES_USE_INDEX
+            else get_curr_path().name
+        )
         path: str = str(
-            output_path
-            / f"{file_stem}{'_contoured' if not SETTINGS_VIEW_ENABLED else ''}.{extension}"
+            constants.IMG_DIR
+            / f"{file_name}_{'contoured_' if not SETTINGS_VIEW_ENABLED else ''}{global_vars.THETA_X}_{global_vars.THETA_Y}_{global_vars.THETA_Z}_{global_vars.SLICE}.{extension}"
         )
         self.image.pixmap().save(path, extension)
 
-    def import_json(self) -> None:
-        """Called when "import" button is clicked
-
-        Imported parameters include input_image_path, output_contoured_slice_path, x_rotation, y_rotation, z_rotation, slice,
-        smoothing_conductance, smoothing_iterations, smoothing_time_step, threshold_filter, upper_binary_threshold, lower_binary_threshold,
-        and circumference
-
-        input_image_path is the only mandatory field.
-
-        :return: `None`"""
-        file_filter: str = "NeuroRuler image settings JSON " + str(("*.json")).replace(
-            "'", ""
-        ).replace(",", "")
-
-        files, _ = QFileDialog.getOpenFileNames(
-            self, "Open file", str(settings.FILE_BROWSER_START_DIR), file_filter
-        )
-
-        # list[str]
-        path_list = files
-        if len(path_list) == 0:
-            return
-        elif "gui_config" in path_list[0]:
-            information_dialog(
-                "Invalid JSON",
-                "You selected a GUI configuration file. Please select an image settings JSON (fields circumference, x_rotation, y_rotation, etc.).",
-            )
-            return
-        elif len(path_list) > 1:
-            information_dialog(
-                "Multiple imports",
-                "Multiple JSON files were selected. Only the first will be imported.",
-            )
-
-        with open(path_list[0], "r") as file:
-            # Parse the JSON data into a dictionary
-            data = json.load(file)
-
-        image_path: str = data["input_image_path"]
-        self.browse_files(False, image_path)
-
-        if "x_rotation" in data:
-            global_vars.THETA_X = data["x_rotation"]
-            self.x_slider.setValue(global_vars.THETA_X)
-
-        if "y_rotation" in data:
-            global_vars.THETA_Y = data["y_rotation"]
-            self.y_slider.setValue(global_vars.THETA_Y)
-
-        if "z_rotation" in data:
-            global_vars.THETA_Z = data["z_rotation"]
-            self.z_slider.setValue(global_vars.THETA_Z)
-
-        self.update_view()
-
-        if "slice" in data:
-            global_vars.SLICE = data["slice"]
-            self.slice_slider.setValue(global_vars.SLICE)
-            self.slice_update()
-
-        if "smoothing_conductance" in data:
-            global_vars.CONDUCTANCE_PARAMETER = data["smoothing_conductance"]
-
-        if "smoothing_iterations" in data:
-            global_vars.SMOOTHING_ITERATIONS = data["smoothing_iterations"]
-
-        if "smoothing_time_step" in data:
-            global_vars.TIME_STEP = data["smoothing_time_step"]
-
-        self.update_smoothing_settings(False)
-
-        if "threshold_filter" in data:
-            if data["threshold_filter"] == "Binary":
-                if (
-                    not "upper_binary_threshold" in data
-                    or not "lower_binary_threshold" in data
-                ):
-                    print(
-                        "If the imported JSON has threshold_filter Binary, it must have upper_binary_threshold and lower_binary_threshold"
-                    )
-                    exit(1)
-                global_vars.UPPER_BINARY_THRESHOLD = data["upper_binary_threshold"]
-                global_vars.LOWER_BINARY_THRESHOLD = data["lower_binary_threshold"]
-                self.update_binary_filter_settings(False)
-                self.enable_binary_threshold_inputs()
-                self.binary_radio_button.click()
-            elif data["threshold_filter"] == "Otsu":
-                self.otsu_radio_button.click()
-                self.disable_binary_threshold_inputs()
-            else:
-                print("Invalid threshold_filter in imported JSON")
-                exit(1)
-
-    def export_json(self) -> None:
-        """Called when "export" button is clicked and when Menu > Export > JSON is clicked.
-
-        Exported parameters include: input_image_path, output_contoured_slice_path, x_rotation, y_rotation, z_rotation, slice,
-        smoothing_conductance, smoothing_iterations, smoothing_time_step, threshold_filter, upper_binary_threshold, lower_binary_threshold,
-        and circumference
-
-        :return: `None`"""
-
-        global_vars.CURR_IMAGE_INDEX = 0
-        self.render_image_num_and_path()
-        for image_num in range(len(global_vars.IMAGE_DICT)):
-            curr_path: Path = get_curr_path()
-            stem: str = constants.get_path_stem(curr_path)
-            binary_contour_slice: np.ndarray = self.render_curr_slice()
-            circumference: float = self.render_circumference(binary_contour_slice)
-            output_dir: Path = constants.OUTPUT_DIR / stem
-            if not output_dir.exists():
-                output_dir.mkdir()
-
-            self.export_curr_slice_as_img(OUTPUT_SLICE_EXTENSION)
-
-            data: dict[str, Any] = {
-                "input_image_path": str(curr_path),
-                "output_contoured_slice_path": str(
-                    Path.cwd()
-                    / output_dir
-                    / (stem + f"_contoured.{OUTPUT_SLICE_EXTENSION}")
-                ),
-                "circumference": circumference,
-                "x_rotation": global_vars.THETA_X,
-                "y_rotation": global_vars.THETA_Y,
-                "z_rotation": global_vars.THETA_Z,
-                "slice": global_vars.SLICE,
-                "smoothing_conductance": global_vars.CONDUCTANCE_PARAMETER,
-                "smoothing_iterations": global_vars.SMOOTHING_ITERATIONS,
-                "smoothing_time_step": global_vars.TIME_STEP,
-                "threshold_filter": "Otsu"
-                if self.otsu_radio_button.isChecked()
-                else "Binary",
-                "upper_binary_threshold": global_vars.UPPER_BINARY_THRESHOLD,
-                "lower_binary_threshold": global_vars.LOWER_BINARY_THRESHOLD,
-            }
-            # Otsu doesn't use the upper/lower binary thresholds set in the GUI
-            if data["threshold_filter"] == "Otsu":
-                data.pop("upper_binary_threshold")
-                data.pop("lower_binary_threshold")
-
-            with open(output_dir / (stem + "_settings.json"), "w") as outfile:
-                json.dump(data, outfile, indent=4)
-
-            self.next_img()
-
     def orient_curr_image(self) -> None:
         """Orient the current image for the current view (global_vars.VIEW) by applying ORIENT_FILTER on it.
 
         This mutates the image.
 
         :return: None"""
         img_helpers.orient_curr_image(global_vars.VIEW)
@@ -1072,29 +847,29 @@
     Typically, this returns less metadata for NRRD than for NIfTI.
 
     :return: None"""
     if not len(global_vars.IMAGE_DICT):
         print("Can't print metadata when there's no image!")
         return
     message: str = pprint.pformat(get_curr_metadata())
-    if settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
+    if user_settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
         print(message)
     else:
         information_dialog("Metadata", message)
 
 
 def display_dimensions() -> None:
     """Display current image's dimensions in window or terminal.
 
     :return: None"""
     if not len(global_vars.IMAGE_DICT):
         print("Can't print dimensions when there's no image!")
         return
     message: str = pprint.pformat(get_curr_image().GetSize())
-    if settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
+    if user_settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
         print(message)
     else:
         information_dialog("Dimensions", message)
 
 
 # TODO: If updating img_helpers.get_properties(), this needs to be slightly adjusted!
 def display_properties() -> None:
@@ -1108,102 +883,108 @@
     if not len(global_vars.IMAGE_DICT):
         print("No loaded image!")
         return
     curr_properties: tuple = get_curr_properties_tuple()
     fields: tuple = ("center of rotation", "dimensions", "spacing")
     if len(fields) != len(curr_properties):
         print(
-            "Update NeuroRuler/GUI/main.print_properties() !\nNumber of fields and number of properties don't match."
+            "Update src/GUI/main.print_properties() !\nNumber of fields and number of properties don't match."
         )
         exit(1)
     # Pretty sure the dict(zip(...)) goes through fields in alphabetical order
     message: str = pprint.pformat(dict(zip(fields, curr_properties)))
-    if settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
+    if user_settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
         print(message)
     else:
         information_dialog("Properties", message)
 
 
 def display_direction() -> None:
     """Display current image's direction in window or terminal.
 
     :return: None"""
     if not len(global_vars.IMAGE_DICT):
         print("Can't print direction when there's no image!")
         return
     message: str = pprint.pformat(get_curr_image().GetDirection())
-    if settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
+    if user_settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
         print(message)
     else:
         information_dialog("Direction", message)
 
 
 def display_spacing() -> None:
     """Display current image's spacing in window or terminal.
 
     :return: None"""
     if not len(global_vars.IMAGE_DICT):
         print("Can't print spacing when there's no image!")
         return
     message: str = pprint.pformat(get_curr_image().GetSpacing())
-    if settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
+    if user_settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
         print(message)
     else:
         information_dialog("Spacing", message)
 
 
 def main() -> None:
     """Main entrypoint of GUI."""
     # This import can't go at the top of the file
     # because gui.py.parse_gui_cli() has to set THEME_NAME before the import occurs
     # This imports globally
-    # For example, NeuroRuler/GUI/helpers.py can access resource files without having to import there
-    importlib.import_module(f"NeuroRuler.GUI.themes.{settings.THEME_NAME}.resources")
+    # For example, src/GUI/helpers.py can access resource files without having to import there
+    importlib.import_module(f"src.GUI.themes.{user_settings.THEME_NAME}.resources")
 
     app = QApplication(sys.argv)
 
     # On macOS, sets the application logo in the dock (but no window icon on macOS)
     # TODO
     # On Windows, sets the window icon at the top left of the window (but no dock icon on Windows)
-    app.setWindowIcon(QIcon(str(PATH_TO_NR_LOGO)))
+    app.setWindowIcon(QIcon(str(PATH_TO_HCT_LOGO)))
 
     # TODO: Put arrow buttons on the left and right endpoints of the sliders
     # These arrow buttons already show up if commenting in app.setStyle("Fusion")
     # And commenting out with open stylesheet and app.setStyleSheet
     # We should figure out how to get arrow buttons on sliders for (+, -) 1 precise adjustments.
     # Currently, the sliders allow this (left click on the left or right end), but the arrow buttons
     # are not in the GUI.
     # app.setStyle("Fusion")
 
     MAIN_WINDOW: MainWindow = MainWindow()
 
-    with open(constants.THEME_DIR / settings.THEME_NAME / "stylesheet.qss", "r") as f:
+    with open(
+        constants.THEME_DIR / user_settings.THEME_NAME / "stylesheet.qss", "r"
+    ) as f:
         MAIN_WINDOW.setStyleSheet(f.read())
 
     # Non-zero min width and height is needed to prevent
-    # this bug https://github.com/NIRALUser/NeuroRuler/issues/42
+    # this bug https://github.com/COMP523TeamD/HeadCircumferenceTool/issues/42
     # However, this also seems to affect startup GUI size or at least GUI element spacing
     MAIN_WINDOW.setMinimumSize(QSize(1, 1))
     MAIN_WINDOW.resize(
-        int(settings.STARTUP_WIDTH_RATIO * constants.PRIMARY_MONITOR_DIMENSIONS[0]),
-        int(settings.STARTUP_HEIGHT_RATIO * constants.PRIMARY_MONITOR_DIMENSIONS[1]),
+        int(
+            user_settings.STARTUP_WIDTH_RATIO * constants.PRIMARY_MONITOR_DIMENSIONS[0]
+        ),
+        int(
+            user_settings.STARTUP_HEIGHT_RATIO * constants.PRIMARY_MONITOR_DIMENSIONS[1]
+        ),
     )
 
     MAIN_WINDOW.show()
 
     try:
         # sys.exit will cause a bug when running from terminal
         # After importing the GUI runner function from __init__, clicking the close window button
         # (not the menu button) will not close the window
         # because the Python process wouldn't end
         os._exit(app.exec())
     except:
-        if settings.DEBUG:
+        if user_settings.DEBUG:
             print("Exiting")
 
 
 if __name__ == "__main__":
-    import NeuroRuler.utils.parser as parser
+    import src.utils.parser as parser
 
-    parser.parse_gui_config()
+    parser.parse_config_json()
     parser.parse_gui_cli()
     main()
```

### Comparing `NeuroRuler-1.0.1/pyproject.toml` & `NeuroRuler-1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -15,24 +15,35 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Multimedia :: Graphics",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
-# dependencies set in setup.py
-# version set in NeuroRuler/GUI/__init__.py
-# keywords set in setup.py
 dynamic = ["dependencies", "version", "keywords"]
 
 [project.urls]
-"Homepage" = "https://github.com/NIRALUser/NeuroRuler"
-"Bug Tracker" = "https://github.com/NIRALUser/NeuroRuler/issues"
+"Homepage" = "https://github.com/COMP523TeamD/HeadCircumferenceTool"
+"Bug Tracker" = "https://github.com/COMP523TeamD/HeadCircumferenceTool/issues"
 
 [build-system]
 requires = ["setuptools>=67.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
+
+[tool.mypy]
+mypy_path = "src"
+check_untyped_defs = true
+disallow_any_generics = true
+ignore_missing_imports = true
+no_implicit_optional = true
+show_error_codes = true
+strict_equality = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unreachable = true
+warn_unused_configs = true
+no_implicit_reexport = true
```

### Comparing `NeuroRuler-1.0.1/setup.py` & `NeuroRuler-1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,71 @@
 # Source: https://github.com/hmeine/qimage2ndarray/blob/master/setup.py
 
 try:
-    from setuptools import setup, find_packages
+    from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
+from pathlib import Path
+
+# TODO: Modify path when refactoring
+for line in open(Path("src") / "GUI" / "__init__.py"):
+    if line.startswith("__version__"):
+        exec(line)
+
+install_requires: list[str]
+
+print(f"cwd: {Path().cwd()}")
+
+# with open(Path("requirements.txt")) as f:
+#     install_requires = f.read().splitlines()
+
 install_requires: list[str] = [
     "setuptools",
+    "sphinx",
+    "sphinx_rtd_theme",
     "SimpleITK",
     "numpy",
     "argparse",
     "opencv-python",
     "pytest",
     "PyQt6",
     "qimage2ndarray",
     "screeninfo",
+    "black",
+    "pre-commit",
+    "build",
+    "twine",
 ]
-"""All required (i.e., for functionality) dependencies that are installed when running `pip install NeuroRuler`.
-
-Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="NeuroRuler",
-    # For current version number, see
-    # https://pypi.org/project/NeuroRuler/
-    version="1.0.1",
+    version=__version__,
     description="A program that calculates head circumference from MRI data (`.nii`, `.nii.gz`, `.nrrd`).",
     # Cannot use multiple authors
     # https://stackoverflow.com/questions/9999829/how-to-specify-multiple-authors-emails-in-setup-py
     author="COMP523 Team D",
     author_email="comp523d@gmail.com",
-    url="https://github.com/NIRALUser/NeuroRuler",
-    download_url="https://github.com/NIRALUser/NeuroRuler/releases",
+    url="https://github.com/COMP523TeamD/HeadCircumferenceTool",
+    download_url="https://github.com/COMP523TeamD/HeadCircumferenceTool/releases",
     keywords=[
         "MRI",
         "NIfTI",
         "NRRD",
         "brain",
         "circumference",
         "PyQt6",
     ],
     install_requires=install_requires,
-    tests_require=install_requires + ["tox", "pytest", "pytest-cov"],
-    # See https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
-    package_dir={"NeuroRuler": "NeuroRuler"},
-    packages=find_packages(),
-    package_data={
-        "NeuroRuler": ["GUI/*.ui", "GUI/static/*", "GUI/themes/*/*", "../*.json"]
-    },
+    # We don't need extras_require
+    # See https://stackoverflow.com/questions/41268863/what-is-the-difference-between-extras-require-and-install-requires-in-se
+    # extras_require=dict(),
+    tests_require="pytest",
+    # TODO: Change after refactoring
+    packages=["src.GUI"],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Topic :: Multimedia :: Graphics",
```

### Comparing `NeuroRuler-1.0.1/tests/test_img_helpers.py` & `NeuroRuler-1.7/tests/test_img_helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from NeuroRuler.utils.img_helpers import *
-import NeuroRuler.utils.global_vars as global_vars
+from src.utils.img_helpers import *
+import src.utils.global_vars as global_vars
 
 IMAGE_NAMES: list[str] = [
     "BCP_Dataset_2month_T1w.nrrd",
     "IBIS_Case1_V06_t1w_RAI.nrrd",
     "IBIS_Case2_V12_t1w_RAI.nrrd",
     "IBIS_Case3_V24_t1w_RAI.nrrd",
     "IBIS_Dataset_12month_T1w.nrrd",  # Group 1: 0-4
@@ -38,14 +38,29 @@
         hash(get_properties_from_sitk_image(img)) == first_group_hash for img in GROUP_1
     )
     assert second_group_hash != third_group_hash
     assert first_group_hash != second_group_hash
     assert first_group_hash != third_group_hash
 
 
+# TODO
+# def test_initialize_globals_and_update_image_groups():
+#    """This tests update_image_groups since initialize_globals calls update_image_groups."""
+#    clear_globals()
+#    assert len(global_vars.IMAGE_GROUPS) == 0
+#    initialize_globals(IMAGE_PATHS)
+#    assert len(global_vars.IMAGE_GROUPS) == 3
+#    clear_globals()
+#    initialize_globals(IMAGE_PATHS[:5])
+#    assert len(global_vars.IMAGE_GROUPS) == 1
+#    clear_globals()
+#    initialize_globals(IMAGE_PATHS[:6])
+#    assert len(global_vars.IMAGE_GROUPS) == 2
+
+
 def test_curr_path():
     clear_globals()
     initialize_globals(IMAGE_PATHS)
     for i in range(4):
         next_img()
     assert get_curr_path() == IMAGE_PATHS[4]
     for i in range(2):
```

### Comparing `NeuroRuler-1.0.1/tests/test_imgproc.py` & `NeuroRuler-1.7/tests/test_imgproc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-"""Test stuff in imgproc.py.
-
-A lot of tests here test behavior of libraries instead of our code. This was useful when learning how
-to use the libraries, not so useful anymore.
+"""Test stuff in Playground.imgproc.
 
 We use == for float comparison instead of |a-b|<epsilon when the numbers should be *exactly* the same."""
 
 import SimpleITK as sitk
 import numpy as np
 import cv2
 import pytest
 from pathlib import Path
-from NeuroRuler.utils.imgproc import contour, length_of_contour
-import NeuroRuler.utils.exceptions as exceptions
-from NeuroRuler.utils.constants import (
+from src.utils.imgproc import contour, length_of_contour
+import src.utils.exceptions as exceptions
+from src.utils.constants import (
     DATA_DIR,
-    SUPPORTED_IMAGE_EXTENSIONS,
-    degrees_to_radians,
-)
-from NeuroRuler.utils.global_vars import READER
-from NeuroRuler.utils.img_helpers import (
-    get_rotated_slice_hardcoded,
-    get_center_of_rotation,
+    NUM_CONTOURS_IN_INVALID_SLICE,
+    SUPPORTED_EXTENSIONS,
 )
+from src.utils.global_vars import READER
+from src.utils.img_helpers import get_rotated_slice_hardcoded
 
 EPSILON: float = 0.001
 """Used for `float` comparisons."""
 
 EXAMPLE_IMAGES: dict[Path, sitk.Image] = dict()
-for extension in SUPPORTED_IMAGE_EXTENSIONS:
+for extension in SUPPORTED_EXTENSIONS:
     for path in DATA_DIR.glob(extension):
         READER.SetFileName(str(path))
         EXAMPLE_IMAGES[path] = READER.Execute()
 
 
 @pytest.mark.skip(reason="Doesn't need to run again unless new images are added")
 def test_all_images_min_value_0_max_value_less_than_1600():
@@ -110,15 +104,15 @@
         for theta_x in range(0, 30, 15):
             for theta_y in range(0, 30, 15):
                 for theta_z in range(0, 30, 15):
                     for slice_num in range(img.GetSize()[2] // 3):
                         rotated_slice = get_rotated_slice_hardcoded(
                             img, theta_x, theta_y, theta_z, slice_num
                         )
-                        contour_slice: np.ndarray = contour(rotated_slice)
+                        contour_slice: np.ndarray = contour(rotated_slice, True)
                         assert (
                             contour_slice.shape[0] == img.GetSize()[0]
                             and contour_slice.shape[1] == img.GetSize()[1]
                         )
 
 
 @pytest.mark.skip(reason="This should be run again later")
@@ -181,47 +175,55 @@
                         assert length_of_not_copied == length_of_copied
 
 
 @pytest.mark.skip(
     reason="User can see in the GUI the contour generated to confirm its accuracy. Also, this won't matter except for edge cases where the slice is invalid"
 )
 def test_arc_length_of_transposed_matrix_is_same_except_for_invalid_slice():
-    """Per discussion here https://github.com/NIRALUser/NeuroRuler/commit/a230a6b57dc34ec433e311d760cc53841ddd6a49,
+    """Per discussion here https://github.com/COMP523TeamD/HeadCircumferenceTool/commit/a230a6b57dc34ec433e311d760cc53841ddd6a49,
 
     Test that the arc length of a contour and its transpose is the same in a specific case. It probably generalizes to the general case.
 
     Specifically, for a matrix and its transpose, cv2.findContours will return [ [[x0 y0]] [[x1 y1]] [[x2 y2]] ... ] and [ [[y0 x0]], [[y1 x1]] [[y2 x2]] ... ]
 
     But cv2.arcLength will apply the distance formula to these contours and that will return the same result.
 
     However, if pixel spacing is off (non-square pixels), then the distance formula would need a scaling factor for one of the dimensions. Then we'd have to account for this.
 
     But the pixel spacing of the underlying `np.ndarray` passed into cv2.findContours *seems* to be fine. See discussion in the GH link.
 
     TODO: Unit test with pre-computed circumferences to really confirm this."""
+    # Write settings of slices that cause ComputeCircumferenceOfInvalidSlice to a file to make sure they actually are just noise and not brain slices.
+    f = open(Path("tests") / "noise_vals.txt", "w")
+    f.write(
+        f"Write settings of slices that cause ComputeCircumferenceOfInvalidSlice (>= {NUM_CONTOURS_IN_INVALID_SLICE} contours detected)\nto this file to make sure they actually are invalid brain slices\n\n"
+    )
+    f.write("From test_arc_length_of_transposed_matrix_is_same\n\n")
+
     for img in EXAMPLE_IMAGES.values():
-        # f.write(f"{DATA_DIR.name}/{img.path.name}\n")
+        f.write(f"{DATA_DIR.name}/{img.path.name}\n")
         for theta_x in range(0, 31, 15):
             for theta_y in range(0, 31, 15):
                 for theta_z in range(0, 31, 15):
                     for slice_num in range(0, img.GetSize()[2]):
                         rotated_slice: sitk.Image = get_rotated_slice_hardcoded(
                             img, theta_x, theta_y, theta_z, slice_num
                         )
-                        contour_slice: np.ndarray = contour(rotated_slice)
+                        contour_slice: np.ndarray = contour(rotated_slice, True)
                         # .copy() probably isn't needed if above test passes
                         contour_slice_transposed: np.ndarray = np.transpose(
                             contour_slice
                         )
                         try:
                             length_1 = length_of_contour(contour_slice)
                             length_2 = length_of_contour(contour_slice_transposed)
                             assert length_1 == length_2
                         except exceptions.ComputeCircumferenceOfInvalidSlice:
-                            pass
+                            f.write(f"{theta_x, theta_y, theta_z, slice_num}\n")
+    f.close()
 
 
 @pytest.mark.skip(reason="")
 def test_contour_slice_retranspose_same_dimensions_as_original_slice():
     """Test that the np array generated after contouring has the same dimensions as the original
     sitk slice.
 
@@ -249,30 +251,12 @@
                 for theta_z in range(0, 31, 15):
                     for slice_num in range(
                         0, original_dimensions[2], original_dimensions[2] // 4
                     ):
                         rotated_slice: sitk.Image = get_rotated_slice_hardcoded(
                             img, theta_x, theta_y, theta_z, slice_num
                         )
-                        binary_contour = contour(rotated_slice)
+                        binary_contour = contour(rotated_slice, True)
                         assert (
                             original_dimensions[0] == binary_contour.shape[0]
                             and original_dimensions[1] == binary_contour.shape[1]
                         )
-
-
-@pytest.mark.skip(reason="Passed locally, doesn't need to run again")
-def test_rotation_doesnt_affect_spacing():
-    img = list(EXAMPLE_IMAGES.values())[0]
-    e3d = sitk.Euler3DTransform()
-    e3d.SetCenter(get_center_of_rotation(img))
-    spacing = img.GetSpacing()
-    for theta_x in range(0, 100, 25):
-        for theta_y in range(0, 100, 25):
-            for theta_z in range(0, 100, 25):
-                e3d.SetRotation(
-                    degrees_to_radians(theta_x),
-                    degrees_to_radians(theta_y),
-                    degrees_to_radians(theta_z),
-                )
-                new_img = sitk.Resample(img, e3d)
-                assert new_img.GetSpacing() == spacing
```

