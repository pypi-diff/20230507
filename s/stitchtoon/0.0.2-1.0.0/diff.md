# Comparing `tmp/stitchtoon-0.0.2.tar.gz` & `tmp/stitchtoon-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stitchtoon-0.0.2.tar", last modified: Fri Apr 28 22:04:24 2023, max compression
+gzip compressed data, was "stitchtoon-1.0.0.tar", last modified: Sun May  7 16:43:52 2023, max compression
```

## Comparing `stitchtoon-0.0.2.tar` & `stitchtoon-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rwxr-xr-x   0        0        0      103 2023-04-28 10:31:49.403240 stitchtoon-0.0.2/.gitignore
--rwxr-xr-x   0        0        0     1073 2023-04-26 07:52:39.218719 stitchtoon-0.0.2/LICENSE
--rw-r--r--   0        0        0      603 2023-04-26 07:52:39.218719 stitchtoon-0.0.2/Makefile
--rwxr-xr-x   0        0        0      363 2023-04-28 10:36:15.659901 stitchtoon-0.0.2/Pipfile
--rw-r--r--   0        0        0    36902 2023-04-28 10:37:12.713234 stitchtoon-0.0.2/Pipfile.lock
--rwxr-xr-x   0        0        0     1510 2023-04-26 07:52:39.218719 stitchtoon-0.0.2/README.md
--rwxr-xr-x   0        0        0     1177 2023-04-28 10:46:07.089890 stitchtoon-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      102 2023-04-26 07:52:39.222054 stitchtoon-0.0.2/requirements.txt
--rwxr-xr-x   0        0        0      154 2023-04-26 07:52:39.272079 stitchtoon-0.0.2/scripts/formatter.py
--rwxr-xr-x   0        0        0      768 2023-04-26 07:52:39.232059 stitchtoon-0.0.2/setup.cfg
--rwxr-xr-x   0        0        0      117 2023-04-26 07:52:39.278749 stitchtoon-0.0.2/setup.py
--rwxr-xr-x   0        0        0     1673 2023-04-28 10:47:25.879888 stitchtoon-0.0.2/src/stitchtoon/__init__.py
--rwxr-xr-x   0        0        0     4807 2023-04-26 07:52:39.232059 stitchtoon-0.0.2/src/stitchtoon/__main__.py
--rwxr-xr-x   0        0        0      219 2023-04-26 07:52:39.232059 stitchtoon-0.0.2/src/stitchtoon/detectors/__init__.py
--rwxr-xr-x   0        0        0      687 2023-04-28 09:37:29.983305 stitchtoon-0.0.2/src/stitchtoon/detectors/direct_slicing.py
--rwxr-xr-x   0        0        0     2011 2023-04-26 12:43:33.252489 stitchtoon-0.0.2/src/stitchtoon/detectors/pixel_comparison.py
--rwxr-xr-x   0        0        0      523 2023-04-26 21:46:22.055454 stitchtoon-0.0.2/src/stitchtoon/detectors/selector.py
--rwxr-xr-x   0        0        0      384 2023-04-26 12:43:33.212489 stitchtoon-0.0.2/src/stitchtoon/services/__init__.py
--rwxr-xr-x   0        0        0     2333 2023-04-26 07:52:39.242064 stitchtoon-0.0.2/src/stitchtoon/services/global_logger.py
--rwxr-xr-x   0        0        0     1844 2023-04-28 09:58:01.109948 stitchtoon-0.0.2/src/stitchtoon/services/image_directory.py
--rwxr-xr-x   0        0        0     3195 2023-04-26 12:43:33.139156 stitchtoon-0.0.2/src/stitchtoon/services/image_handler.py
--rwxr-xr-x   0        0        0     3609 2023-04-28 09:55:08.669951 stitchtoon-0.0.2/src/stitchtoon/services/image_manipulator.py
--rwxr-xr-x   0        0        0      756 2023-04-26 07:52:39.255404 stitchtoon-0.0.2/src/stitchtoon/services/postprocess_runner.py
--rwxr-xr-x   0        0        0     7154 2023-04-28 10:05:17.899939 stitchtoon-0.0.2/src/stitchtoon/services/process.py
--rw-r--r--   0        0        0     1009 2023-04-26 07:54:58.167603 stitchtoon-0.0.2/src/stitchtoon/services/progressbar.py
--rwxr-xr-x   0        0        0     3037 2023-04-26 08:30:42.875031 stitchtoon-0.0.2/src/stitchtoon/services/scanner.py
--rwxr-xr-x   0        0        0        0 2023-04-28 21:57:52.553321 stitchtoon-0.0.2/src/stitchtoon/utils/__init__.py
--rwxr-xr-x   0        0        0     1108 2023-04-28 09:58:01.069948 stitchtoon-0.0.2/src/stitchtoon/utils/constants.py
--rwxr-xr-x   0        0        0      134 2023-04-28 09:58:00.606614 stitchtoon-0.0.2/src/stitchtoon/utils/errors.py
--rwxr-xr-x   0        0        0      451 2023-04-26 07:52:39.262074 stitchtoon-0.0.2/src/stitchtoon/utils/funcs.py
--rwxr-xr-x   0        0        0      823 2023-04-28 10:55:05.359879 stitchtoon-0.0.2/stitchtoon.spec
--rw-r--r--   0        0        0        0 2023-04-26 07:52:39.272079 stitchtoon-0.0.2/test/__init__.py
--rw-r--r--   0        0        0   138180 2023-04-26 07:48:14.598838 stitchtoon-0.0.2/test/data/01.jpeg
--rw-r--r--   0        0        0  1726886 2023-04-28 10:33:22.676571 stitchtoon-0.0.2/test/data/01.webp
--rw-r--r--   0        0        0   141943 2023-04-26 07:48:24.412171 stitchtoon-0.0.2/test/data/02.jpeg
--rw-r--r--   0        0        0   123745 2023-04-26 07:48:32.655504 stitchtoon-0.0.2/test/data/03.jpeg
--rw-r--r--   0        0        0   142053 2023-04-26 07:48:41.388838 stitchtoon-0.0.2/test/data/04.jpeg
--rw-r--r--   0        0        0     1117 2023-04-28 09:51:25.226622 stitchtoon-0.0.2/test/test_manipulator.py
--rw-r--r--   0        0        0     1101 2023-04-26 12:44:24.079155 stitchtoon-0.0.2/test/test_scan.py
--rw-r--r--   0        0        0      292 2023-04-26 07:52:39.272079 stitchtoon-0.0.2/tox.ini
--rw-r--r--   0        0        0     2452 1970-01-01 00:00:00.000000 stitchtoon-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      431 2023-05-07 16:26:35.828468 stitchtoon-1.0.0/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0      111 2023-04-28 22:49:08.769926 stitchtoon-1.0.0/.gitignore
+-rwxr-xr-x   0        0        0     1073 2023-04-26 07:52:39.218719 stitchtoon-1.0.0/LICENSE
+-rw-r--r--   0        0        0      603 2023-04-26 07:52:39.218719 stitchtoon-1.0.0/Makefile
+-rwxr-xr-x   0        0        0      363 2023-04-28 10:36:15.659901 stitchtoon-1.0.0/Pipfile
+-rw-r--r--   0        0        0    36902 2023-04-28 10:37:12.713234 stitchtoon-1.0.0/Pipfile.lock
+-rwxr-xr-x   0        0        0     3019 2023-05-05 16:29:36.234698 stitchtoon-1.0.0/README.md
+-rwxr-xr-x   0        0        0     1178 2023-05-07 16:42:27.643062 stitchtoon-1.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0      596 2023-05-07 16:33:56.675945 stitchtoon-1.0.0/requirements.txt
+-rwxr-xr-x   0        0        0      136 2023-05-05 16:29:36.234698 stitchtoon-1.0.0/scripts/formatter.py
+-rwxr-xr-x   0        0        0      768 2023-04-26 07:52:39.232059 stitchtoon-1.0.0/setup.cfg
+-rwxr-xr-x   0        0        0      117 2023-04-26 07:52:39.278749 stitchtoon-1.0.0/setup.py
+-rwxr-xr-x   0        0        0     1673 2023-05-07 16:42:35.893063 stitchtoon-1.0.0/src/stitchtoon/__init__.py
+-rwxr-xr-x   0        0        0     5611 2023-05-07 16:38:40.459716 stitchtoon-1.0.0/src/stitchtoon/__main__.py
+-rwxr-xr-x   0        0        0      219 2023-04-26 07:52:39.232059 stitchtoon-1.0.0/src/stitchtoon/detectors/__init__.py
+-rwxr-xr-x   0        0        0      687 2023-04-28 09:37:29.983305 stitchtoon-1.0.0/src/stitchtoon/detectors/direct_slicing.py
+-rwxr-xr-x   0        0        0     2011 2023-04-26 12:43:33.252489 stitchtoon-1.0.0/src/stitchtoon/detectors/pixel_comparison.py
+-rwxr-xr-x   0        0        0      523 2023-04-26 21:46:22.055454 stitchtoon-1.0.0/src/stitchtoon/detectors/selector.py
+-rwxr-xr-x   0        0        0      372 2023-05-07 16:28:37.948475 stitchtoon-1.0.0/src/stitchtoon/services/__init__.py
+-rwxr-xr-x   0        0        0     1588 2023-05-07 16:32:43.506041 stitchtoon-1.0.0/src/stitchtoon/services/global_logger.py
+-rwxr-xr-x   0        0        0     1861 2023-05-07 16:41:04.949725 stitchtoon-1.0.0/src/stitchtoon/services/image_directory.py
+-rwxr-xr-x   0        0        0     3464 2023-05-07 16:28:37.951808 stitchtoon-1.0.0/src/stitchtoon/services/image_handler.py
+-rwxr-xr-x   0        0        0     3563 2023-05-07 16:28:37.948475 stitchtoon-1.0.0/src/stitchtoon/services/image_manipulator.py
+-rwxr-xr-x   0        0        0      756 2023-04-26 07:52:39.255404 stitchtoon-1.0.0/src/stitchtoon/services/postprocess_runner.py
+-rwxr-xr-x   0        0        0     7440 2023-05-07 16:40:29.003056 stitchtoon-1.0.0/src/stitchtoon/services/process.py
+-rw-r--r--   0        0        0     1009 2023-05-07 16:10:22.120819 stitchtoon-1.0.0/src/stitchtoon/services/progressbar.py
+-rwxr-xr-x   0        0        0     3037 2023-04-26 08:30:42.875031 stitchtoon-1.0.0/src/stitchtoon/services/scanner.py
+-rwxr-xr-x   0        0        0        0 2023-04-28 21:57:52.553321 stitchtoon-1.0.0/src/stitchtoon/utils/__init__.py
+-rwxr-xr-x   0        0        0     1109 2023-04-28 23:16:20.733227 stitchtoon-1.0.0/src/stitchtoon/utils/constants.py
+-rwxr-xr-x   0        0        0      134 2023-04-28 09:58:00.606614 stitchtoon-1.0.0/src/stitchtoon/utils/errors.py
+-rwxr-xr-x   0        0        0      451 2023-04-26 07:52:39.262074 stitchtoon-1.0.0/src/stitchtoon/utils/funcs.py
+-rwxr-xr-x   0        0        0      823 2023-04-28 10:55:05.359879 stitchtoon-1.0.0/stitchtoon.spec
+-rw-r--r--   0        0        0        0 2023-04-26 07:52:39.272079 stitchtoon-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0   138180 2023-05-07 16:35:32.471442 stitchtoon-1.0.0/tests/test/data/01.jpeg
+-rw-r--r--   0        0        0  1726886 2023-05-07 16:35:32.528109 stitchtoon-1.0.0/tests/test/data/01.webp
+-rw-r--r--   0        0        0   141943 2023-05-07 16:35:32.488109 stitchtoon-1.0.0/tests/test/data/02.jpeg
+-rw-r--r--   0        0        0   123745 2023-05-07 16:35:32.494776 stitchtoon-1.0.0/tests/test/data/03.jpeg
+-rw-r--r--   0        0        0   142053 2023-05-07 16:35:32.498109 stitchtoon-1.0.0/tests/test/data/04.jpeg
+-rw-r--r--   0        0        0     1117 2023-05-07 16:35:32.494776 stitchtoon-1.0.0/tests/test/test_manipulator.py
+-rw-r--r--   0        0        0     1101 2023-05-07 16:35:32.494776 stitchtoon-1.0.0/tests/test/test_scan.py
+-rw-r--r--   0        0        0      284 2023-04-28 22:41:33.483269 stitchtoon-1.0.0/tox.ini
+-rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 stitchtoon-1.0.0/PKG-INFO
```

### Comparing `stitchtoon-0.0.2/LICENSE` & `stitchtoon-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/Makefile` & `stitchtoon-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/Pipfile.lock` & `stitchtoon-1.0.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/pyproject.toml` & `stitchtoon-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stitchtoon"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
   { name="Beshr Alghalil", email="beshrghalil@protonmail.com" },
 ]
 description = "A powerful program for stitching and cutting webtoons/manhwa/manhua raws."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["manga", "webtoon", "stitch", "slice", "combin"]
@@ -49,8 +49,8 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 120
 
 [tool.pylint.format]
-max-line-length = "120"
+max-line-length = "120"
```

### Comparing `stitchtoon-0.0.2/setup.cfg` & `stitchtoon-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/src/stitchtoon/__init__.py` & `stitchtoon-1.0.0/src/stitchtoon/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         except (OSError, subprocess.CalledProcessError, AttributeError):
             version_string = version_string.format(__version__)
     return version_string
 
 
 # Information
 __license__ = "MIT"
-__version__ = "0.0.2"
+__version__ = "1.0.0"
 __release__ = False
 __author__ = __maintainer__ = "Beshr Ghalil"
 __email__ = "beshrghalil@porotonmail.com"
 
 # Constants
 stitchtoon = os.path.dirname(__file__)
 DEFAULT_PAGER = "less"
```

### Comparing `stitchtoon-0.0.2/src/stitchtoon/__main__.py` & `stitchtoon-1.0.0/src/stitchtoon/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import argparse
 import math
 import sys
 
 from stitchtoon import __version__
+from stitchtoon.services.global_logger import DEFAULT_LOG_LEVEL, Logger, get_logger
 from stitchtoon.services.process import process
 
 
 def positive_int(value):
     if not value.isdigit() or int(value) <= 0:
         raise argparse.ArgumentTypeError("Not a valid integer value")
     return int(value)
 
 
+def log_level(value):
+    import logging
+
+    return {"debug": logging.DEBUG, "info": logging.INFO, "error": logging.ERROR}.get(
+        value, DEFAULT_LOG_LEVEL
+    )
+
+
 def size_format(value):
     value = value.replace("x", "X")
     size = value.split("X")
     if len(size) > 2:
         raise argparse.ArgumentTypeError(
             "invalid size format. Supported formats `<height>X<width>` or `<height>`. ex: `5000X760`"
         )
@@ -98,20 +107,20 @@
         default="pixel",
         choices=["none", "pixel"],
         help="Sets the type of Slice Location Detection, Default=pixel (Pixel Comparison)",
     )
     advanced.add_argument(
         "-e",
         "--sensitivity",
-        dest="senstivity",
+        dest="sensitivity",
         type=int,
         default=90,
         choices=range(0, 101),
         metavar="[0-100]",
-        help="Sets the Object Detection Senstivity Percentage, Default=90 (10 percent tolerance)",
+        help="Sets the Object Detection sensitivity Percentage, Default=90 (10 percent tolerance)",
     )
     advanced.add_argument(
         "-q",
         "--quality",
         dest="lossy_quality",
         type=int,
         default=100,
@@ -133,23 +142,43 @@
         dest="line_steps",
         type=int,
         default=5,
         choices=range(1, 100),
         metavar="[1-100]",
         help="Sets the value of Scan Line Step, Default=5 (5px)",
     )
+    general = parser.add_argument_group("General")
+    general.add_argument(
+        "--log-level",
+        dest="log_level",
+        default="error",
+        choices=["error", "debug", "info"],
+        help="Sets log level",
+    )
+    general.add_argument(
+        "--log-file",
+        dest="log_file",
+        default=sys.stdout,
+        help="Sets the log file, this supports providing datatime format.",
+    )
     return parser.parse_args()
 
 
 def main():
     kwargs = get_args()
 
+    global Logger
+    Logger = get_logger(
+        log_level=log_level(kwargs.log_level),
+        filename=kwargs.log_file,
+    )
+
     stitch_params = {
         "detection_type": kwargs.detection_type,
-        "senstivity": kwargs.senstivity,
+        "sensitivity": kwargs.sensitivity,
         "width_enforce": kwargs.width_enforcement,
         "custom_width": kwargs.size[1],
         "line_steps": kwargs.line_steps,
         "ignorable_pixels": kwargs.ignorable_pixels,
     }
 
     try:
```

### Comparing `stitchtoon-0.0.2/src/stitchtoon/detectors/direct_slicing.py` & `stitchtoon-1.0.0/src/stitchtoon/detectors/direct_slicing.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/src/stitchtoon/detectors/pixel_comparison.py` & `stitchtoon-1.0.0/src/stitchtoon/detectors/pixel_comparison.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/src/stitchtoon/detectors/selector.py` & `stitchtoon-1.0.0/src/stitchtoon/detectors/selector.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/src/stitchtoon/services/global_logger.py` & `stitchtoon-1.0.0/src/stitchtoon/services/global_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,52 @@
 import functools
 import logging
 import os
+import sys
 from datetime import datetime
 
-from ..utils.constants import LOG_REL_DIR
+DEFAULT_LOG_LEVEL = logging.ERROR
 
 
-class GlobalLogger:
-    @classmethod
-    def configureGlobalLogger(self):
-        """Initializes and Configures Logging Service"""
-        if not os.path.exists(LOG_REL_DIR):
-            os.makedirs(LOG_REL_DIR)
+def get_logger(log_level=logging.ERROR, filename=sys.stdout):
+    logger = logging.getLogger("STITCHTOON")
+    logger.setLevel(log_level)
+    log_format = "%(name)s:%(levelname)s:%(asctime)s:%(message)s"
+    logging.basicConfig(format=log_format)
+    if isinstance(filename, str):
         current_date = datetime.now()
-        log_filename = current_date.strftime("log-%Y-%m-%d.log")
-        log_filename = os.path.join(LOG_REL_DIR, log_filename)
+        filename = current_date.strftime(filename)
+        handler = logging.FileHandler(filename, mode="w")
+        logger.addHandler(handler)
 
-        log_level = logging.DEBUG
-        log_format = "%(levelname)s:%(asctime)s:%(message)s"
-        logging.basicConfig(format=log_format, filename=log_filename, level=log_level)
-        logging.debug("GlobalLogger:Logger Initialized")
-        # Removes the pil logging from polluting the Debug Level.
-        pil_logger = logging.getLogger("PIL")
-        pil_logger.setLevel(logging.INFO)
-
-    @classmethod
-    def log_warning(self, message, caller="GlobalLogger", *args, **kwargs):
-        log_msg = f"{caller}:{message}"
-        logging.warning(log_msg, *args, **kwargs)
-
-    @classmethod
-    def log_debug(self, message, caller="GlobalLogger", *args, **kwargs):
-        log = f"{caller}:{message}"
-        logging.debug(log, *args, **kwargs)
-
-    @classmethod
-    def log_info(self, message, caller="GlobalLogger", *args, **kwargs):
-        log = f"{caller}:{message}"
-        logging.info(log, *args, **kwargs)
+    logger.debug("Logger Initialized")
+    # Removes the pil logging from polluting the Debug Level.
+    pil_logger = logging.getLogger("PIL")
+    pil_logger.setLevel(logging.INFO)
+    return logger
 
 
-def logFunc(func=None, inclass=False):
+Logger = get_logger()
+
+
+def logFunc(func=None, inclass=False, logger=Logger):
     if func is None:
         return functools.partial(logFunc, inclass=inclass)
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        caller_class = "GlobalLogger"
         args_repr = [repr(a) for a in args]
         if inclass:
-            caller_class = type(args[0]).__name__
             args_repr = [repr(args[i]) for i in range(1, len(args))]
         kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]
         signature = ", ".join(args_repr + kwargs_repr)
-        GlobalLogger.log_debug(f"{func.__name__}:args:{signature}", caller_class)
+        logger.debug(f"{func.__name__}:args:{signature}")
         try:
             result = func(*args, **kwargs)
             return result
         except Exception as e:
-            logging.exception(
+            logger.exception(
                 f"Exception raised in {func.__name__}. exception: {str(e)}"
             )
             raise e
 
     return wrapper
-
-
-GlobalLogger.configureGlobalLogger()
```

### Comparing `stitchtoon-0.0.2/src/stitchtoon/services/image_directory.py` & `stitchtoon-1.0.0/src/stitchtoon/services/image_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import os
 from dataclasses import dataclass, field
 
 from PIL import Image as pilImage
 from psd_tools import PSDImage
 
-from ..utils.constants import FORMAT_NAME_MAPPER, PHOTOSHOP_FILE_TYPES, SUPPORTED_IMG_TYPES
+from ..utils.constants import (
+    FORMAT_NAME_MAPPER,
+    PHOTOSHOP_FILE_TYPES,
+    SUPPORTED_IMG_TYPES,
+)
 from ..utils.errors import ImageNotOpenedError
 
 
 @dataclass
 class Image:
     path: os.PathLike
     name: str
```

### Comparing `stitchtoon-0.0.2/src/stitchtoon/services/image_handler.py` & `stitchtoon-1.0.0/src/stitchtoon/services/image_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,21 +21,30 @@
         if not osp.splitext(filename)[1]:
             filename = f"{filename}.{format}"
         else:
             filename = f"{osp.splitext(filename)[0]}.{format}"
 
         return filename
 
+    # TODOO: Load images from ao zip/cbz archive.
     @logFunc(inclass=True)
-    def load_zip(self, path):
+    def load_zip(
+        self,
+        path: os.PathLike,
+        progress: ProgressHandler = ProgressHandler(),
+        increament: int = 0,
+    ) -> list[Image]:
         pass
 
     @logFunc(inclass=True)
     def load(
-        self, images: list[Image], progress=ProgressHandler(), increament=0
+        self,
+        images: list[Image],
+        progress: ProgressHandler = ProgressHandler(),
+        increament: int = 0,
     ) -> list[Image]:
         """Loads all image files into a list of PIL image objects."""
         images_len = len(images)
         for idx, image in enumerate(images, 1):
             if image.format not in PHOTOSHOP_FILE_TYPES:
                 image.pil = pilImage.open(image.path)
             else:
@@ -50,42 +59,43 @@
         self,
         output,
         images: list[pilImage.Image],
         img_format: str,
         quality=100,
         progress=ProgressHandler(),
         increament=0,
-    ):
+    ) -> os.PathLike:
         if img_format in PHOTOSHOP_FILE_TYPES:
             # FIXMEE: support archiving psd files
             raise Exception("Can't make PSD archive")
 
         zf = zipfile.ZipFile(output, mode="w")
         images_len = len(images)
         for idx, image in enumerate(images, 1):
             img_byte_arr = io.BytesIO()
             image.pil.save(img_byte_arr, img_format, quality=quality)
             img_byte_arr = img_byte_arr.getvalue()
             zf.writestr(self.filename_handler(f"{idx:02}", img_format), img_byte_arr)
             progress.update(progress.value + increament, f"Archive {idx}/{images_len}")
 
+        return output
+
+    @logFunc(inclass=True)
     def save_all(
         self,
-        output,
+        output: os.PathLike,
         images: list[Image],
         format: str = "png",
         as_archive: bool = False,
-        quality=100,
+        quality: int = 100,
         progress=ProgressHandler(),
-        increament=0,
-    ) -> str:
+        increament: int = 0,
+    ) -> os.PathLike:
+        progress.update(progress.value, "Saving, Please wait...")
         if as_archive:
-            if osp.splitext(output)[1] != ".zip":
-                output = osp.join(output, dt.now().strftime("%d%m%Y_%H%M%S.zip"))
-
             os.makedirs(osp.dirname(output), exist_ok=True)
             self.save_archive(output, images, format, quality, progress, increament)
         else:
             os.makedirs(output, exist_ok=True)
             images_len = len(images)
             for idx, img in enumerate(images, 1):
                 filename = self.filename_handler(f"{idx:02}", format)
```

### Comparing `stitchtoon-0.0.2/src/stitchtoon/services/image_manipulator.py` & `stitchtoon-1.0.0/src/stitchtoon/services/image_manipulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,36 +23,36 @@
 
         Returns:
             list[Image]
         """
 
         if enforce_setting == WIDTH_ENFORCEMENT.NONE.value and not custom_width:
             return img_objs
-        # Resizing Image Logic depending on enforcement settings
+
         new_img_width = 0
         if enforce_setting == WIDTH_ENFORCEMENT.AUTO.value:
             widths, heights = zip(*(img.size for img in img_objs))
             new_img_width = min(widths)
         elif enforce_setting == WIDTH_ENFORCEMENT.FIXED.value or custom_width:
             new_img_width = custom_width
         for img in img_objs:
             if img.width == new_img_width:
                 continue
             img_ratio = float(img.height / img.width)
             new_img_height = int(img_ratio * new_img_width)
             if new_img_height > 0:
                 img.pil = img.pil.resize(
-                    (new_img_width, new_img_height), pilImage.LANCZOS
+                    (new_img_width, new_img_height), pilImage.Resampling.LANCZOS
                 )
         return img_objs
 
     @logFunc(inclass=True)
     @staticmethod
     def combine(
-        img_objs: list[Image], progress: ProgressHandler = None, increament=0
+        img_objs: list[Image], progress: ProgressHandler = None, increament: int = 0
     ) -> Image:
         """Combines given image objs to a single vertically stacked single image obj.
 
         Args:
             img_objs (list[Image])
             progress (_type_, optional)
             increament (int, optional). Defaults to 0.
```

### Comparing `stitchtoon-0.0.2/src/stitchtoon/services/postprocess_runner.py` & `stitchtoon-1.0.0/src/stitchtoon/services/postprocess_runner.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/src/stitchtoon/services/process.py` & `stitchtoon-1.0.0/src/stitchtoon/services/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,16 +93,22 @@
             split_height,
             progress=progress,
             increament=per_dir_percentage / images_len,
             **params,
         )
         images_len = len(images)
         sub_output = output
+
         if recursive:
             sub_output = osp.join(output, osp.basename(image_dir.path))
+            if as_archive and osp.splitext(output)[1] != ".zip":
+                sub_output += ".zip"
+        else:
+            if as_archive and osp.splitext(output)[1] != ".zip":
+                sub_output = osp.join(output, f"{osp.basename(image_dir.path)}.zip")
 
         per_dir_percentage = PROGRESS_PERCENTAGE["save"] / working_dirs_len
         handler.save_all(
             output=sub_output,
             images=images,
             format=format,
             as_archive=as_archive,
@@ -119,46 +125,48 @@
 def stitch(
     images: list[Image],
     split_height: int,
     *,
     progress: ProgressHandler = None,
     increament: int = StitchDefaults.INCREAMENT,
     detection_type: str = StitchDefaults.DETECTION_TYPE,
-    senstivity: int = StitchDefaults.SENSTIVITY,
+    sensitivity: int = StitchDefaults.SENSITIVITY,
     width_enforce: str = StitchDefaults.WIDTH_ENFORCE,
     custom_width: int = StitchDefaults.CUSTOM_WIDTH,
     line_steps: int = StitchDefaults.LINE_STEPS,
     ignorable_pixels: int = StitchDefaults.IGNORABLE_PIXELS,
 ) -> list[Image]:
     """Stitchs images to specified heigh
 
     Args:
         images (list[Image])
         split_height (int)
         progress (ProgressHandler, optional): progressbar handler. Defaults to None.
         increament (int, optional): progressbar increament factor. Defaults to StitchDefaults.INCREAMENT.
         detection_type (str, optional): Defaults to StitchDefaults.DETECTION_TYPE.
-        senstivity (int, optional): Defaults to StitchDefaults.SENSTIVITY.
+        sensitivity (int, optional): Defaults to StitchDefaults.SENSITIVITY.
         width_enforce (str, optional): Defaults to StitchDefaults.WIDTH_ENFORCE.
         custom_width (int, optional): Defaults to StitchDefaults.CUSTOM_WIDTH.
         line_steps (int, optional): Defaults to StitchDefaults.LINE_STEPS.
         ignorable_pixels (int, optional): Defaults to StitchDefaults.IGNORABLE_PIXELS.
 
     Returns:
         list[Images]: stitched images
     """
     if not progress:
         progress = _get_progressbar()
     detector = select_detector(detection_type=detection_type)
     images = ImageManipulator.resize(images, width_enforce, custom_width)
-    combined_img = ImageManipulator.combine(images, progress=progress, increament=increament)
+    combined_img = ImageManipulator.combine(
+        images, progress=progress, increament=increament
+    )
     slice_points = detector.run(
         combined_img,
         split_height,
-        sensitivity=senstivity,
+        sensitivity=sensitivity,
         ignorable_pixels=ignorable_pixels,
         scan_step=line_steps,
     )
     images = ImageManipulator.slice(combined_img, slice_points)
 
     return images
```

### Comparing `stitchtoon-0.0.2/src/stitchtoon/services/progressbar.py` & `stitchtoon-1.0.0/src/stitchtoon/services/progressbar.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/src/stitchtoon/services/scanner.py` & `stitchtoon-1.0.0/src/stitchtoon/services/scanner.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/src/stitchtoon/utils/constants.py` & `stitchtoon-1.0.0/src/stitchtoon/utils/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,12 +52,12 @@
     LOSSY_QUALITY: int = 90
     SHOW_PROGRESS: bool = False
 
 
 class StitchDefaults:
     INCREAMENT: int = 0
     DETECTION_TYPE: str = DETECTION_TYPE.NO_DETECTION.value
-    SENSTIVITY: int = 90
+    SENSITIVITY: int = 90
     WIDTH_ENFORCE: str = "none"
     CUSTOM_WIDTH: int = -1
     LINE_STEPS: int = 5
     IGNORABLE_PIXELS: int = 5
```

### Comparing `stitchtoon-0.0.2/stitchtoon.spec` & `stitchtoon-1.0.0/stitchtoon.spec`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/test/data/01.jpeg` & `stitchtoon-1.0.0/tests/test/data/01.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/test/data/01.webp` & `stitchtoon-1.0.0/tests/test/data/01.webp`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/test/data/02.jpeg` & `stitchtoon-1.0.0/tests/test/data/02.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/test/data/03.jpeg` & `stitchtoon-1.0.0/tests/test/data/03.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/test/data/04.jpeg` & `stitchtoon-1.0.0/tests/test/data/04.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/test/test_manipulator.py` & `stitchtoon-1.0.0/tests/test/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-0.0.2/test/test_scan.py` & `stitchtoon-1.0.0/tests/test/test_scan.py`

 * *Files identical despite different names*

