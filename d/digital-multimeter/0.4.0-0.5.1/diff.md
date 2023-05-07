# Comparing `tmp/digital-multimeter-0.4.0.tar.gz` & `tmp/digital_multimeter-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-multimeter-0.4.0.tar", last modified: Tue Jul  5 10:02:19 2022, max compression
+gzip compressed data, was "digital_multimeter-0.5.1.tar", max compression
```

## Comparing `digital-multimeter-0.4.0.tar` & `digital_multimeter-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,18 @@
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.562468 digital-multimeter-0.4.0/
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     1268 2022-07-05 10:00:02.000000 digital-multimeter-0.4.0/LICENSE
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)      114 2022-07-05 10:00:02.000000 digital-multimeter-0.4.0/MANIFEST.in
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     3624 2022-07-05 10:02:19.561468 digital-multimeter-0.4.0/PKG-INFO
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     2723 2022-07-05 09:49:03.000000 digital-multimeter-0.4.0/README.md
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)      920 2022-07-05 10:00:02.000000 digital-multimeter-0.4.0/package.yml
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)       38 2022-07-05 10:02:19.563468 digital-multimeter-0.4.0/setup.cfg
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     1846 2022-07-05 10:00:02.000000 digital-multimeter-0.4.0/setup.py
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.501467 digital-multimeter-0.4.0/src/
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.513467 digital-multimeter-0.4.0/src/digital_multimeter/
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     2015 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/DigitalMultimeter.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)      404 2022-07-05 10:00:02.000000 digital-multimeter-0.4.0/src/digital_multimeter/__init__.py
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.535467 digital-multimeter-0.4.0/src/digital_multimeter/cli/
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)        0 2020-11-08 01:13:49.000000 digital-multimeter-0.4.0/src/digital_multimeter/cli/__init__.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     3661 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/cli/click.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     3583 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/cli/config.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)      517 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/cli/entrypoints.py
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.539467 digital-multimeter-0.4.0/src/digital_multimeter/exceptions/
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)       47 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/exceptions/MultimeterException.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)        0 2020-11-08 01:13:49.000000 digital-multimeter-0.4.0/src/digital_multimeter/exceptions/__init__.py
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.550468 digital-multimeter-0.4.0/src/digital_multimeter/multimeters/
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)      246 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/multimeters/MultimeterBase.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     6805 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/multimeters/MultimeterEDI9604.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     8734 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)    13923 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)      906 2022-07-05 09:43:29.000000 digital-multimeter-0.4.0/src/digital_multimeter/multimeters/__init__.py
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.553468 digital-multimeter-0.4.0/src/digital_multimeter/utils/
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)        0 2020-11-08 01:13:49.000000 digital-multimeter-0.4.0/src/digital_multimeter/utils/__init__.py
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     2342 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/digital_multimeter/utils/cli_output.py
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.528467 digital-multimeter-0.4.0/src/digital_multimeter.egg-info/
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     3624 2022-07-05 10:02:19.000000 digital-multimeter-0.4.0/src/digital_multimeter.egg-info/PKG-INFO
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)     1136 2022-07-05 10:02:19.000000 digital-multimeter-0.4.0/src/digital_multimeter.egg-info/SOURCES.txt
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)        1 2022-07-05 10:02:19.000000 digital-multimeter-0.4.0/src/digital_multimeter.egg-info/dependency_links.txt
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)       64 2022-07-05 10:02:19.000000 digital-multimeter-0.4.0/src/digital_multimeter.egg-info/entry_points.txt
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)       15 2022-07-05 10:02:19.000000 digital-multimeter-0.4.0/src/digital_multimeter.egg-info/requires.txt
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)       19 2022-07-05 10:02:19.000000 digital-multimeter-0.4.0/src/digital_multimeter.egg-info/top_level.txt
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)        1 2020-11-30 11:45:18.000000 digital-multimeter-0.4.0/src/digital_multimeter.egg-info/zip-safe
-drwxrwxr-x   0 ndejong   (1000) ndejong   (1000)        0 2022-07-05 10:02:19.559468 digital-multimeter-0.4.0/src/test/
--rw-rw-r--   0 ndejong   (1000) ndejong   (1000)      107 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/test/__init__.py
--rwxrwxr-x   0 ndejong   (1000) ndejong   (1000)      588 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/test/test_basic.py
--rwxrwxr-x   0 ndejong   (1000) ndejong   (1000)      429 2022-07-05 09:31:28.000000 digital-multimeter-0.4.0/src/test/test_trivial.py
+-rw-r--r--   0        0        0     1273 2023-05-06 02:11:48.657947 digital_multimeter-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3155 2023-05-07 01:42:21.389047 digital_multimeter-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2617 2023-05-06 13:52:36.944084 digital_multimeter-0.5.1/readme.md
+-rw-r--r--   0        0        0      404 2023-05-07 01:42:21.391047 digital_multimeter-0.5.1/src/digital_multimeter/__init__.py
+-rw-r--r--   0        0        0        0 2020-11-08 01:13:49.217434 digital_multimeter-0.5.1/src/digital_multimeter/cli/__init__.py
+-rw-r--r--   0        0        0     3582 2023-05-06 13:58:12.436781 digital_multimeter-0.5.1/src/digital_multimeter/cli/click.py
+-rw-r--r--   0        0        0     3462 2023-05-06 02:27:22.944278 digital_multimeter-0.5.1/src/digital_multimeter/cli/config.py
+-rw-r--r--   0        0        0      442 2023-05-07 00:51:28.258205 digital_multimeter-0.5.1/src/digital_multimeter/cli/entrypoints.py
+-rw-r--r--   0        0        0       47 2023-05-06 02:27:22.925278 digital_multimeter-0.5.1/src/digital_multimeter/exceptions.py
+-rw-r--r--   0        0        0     2087 2023-05-06 14:21:55.093427 digital_multimeter-0.5.1/src/digital_multimeter/main.py
+-rw-r--r--   0        0        0      245 2023-05-06 02:12:07.448155 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterBase.py
+-rw-r--r--   0        0        0     6727 2023-05-06 02:50:14.875375 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterEDI9604.py
+-rw-r--r--   0        0        0     8680 2023-05-06 02:50:14.889375 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py
+-rw-r--r--   0        0        0    13869 2023-05-06 02:50:21.414447 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py
+-rw-r--r--   0        0        0     1076 2023-05-06 02:40:10.689751 digital_multimeter-0.5.1/src/digital_multimeter/multimeters/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-06 02:44:08.655364 digital_multimeter-0.5.1/src/digital_multimeter/utils/__init__.py
+-rw-r--r--   0        0        0     2323 2023-05-06 02:27:22.934278 digital_multimeter-0.5.1/src/digital_multimeter/utils/cli_output.py
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 digital_multimeter-0.5.1/PKG-INFO
```

### Comparing `digital-multimeter-0.4.0/LICENSE` & `digital_multimeter-0.5.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 Nicholas de Jong
+Copyright 2021-2023 Nicholas de Jong
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer.
```

### Comparing `digital-multimeter-0.4.0/PKG-INFO` & `digital_multimeter-0.5.1/readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,36 @@
-Metadata-Version: 2.1
-Name: digital-multimeter
-Version: 0.4.0
-Summary: Digital Multimeter provides both a CLI interface and a Python3 library interface to receive data from a variety of digital multimeters.
-Home-page: https://digital-multimeter.readthedocs.io/
-Author: Nicholas de Jong
-Author-email: contact@nicholasdejong.com
-License: BSD2
-Keywords: multimeter,digital multimeter,dmm,Fortune FS9721
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.5.0,<4.0.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Digital Multimeter
 [![PyPi](https://img.shields.io/pypi/v/digital-multimeter.svg)](https://pypi.python.org/pypi/digital-multimeter/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/digital-multimeter.svg)](https://github.com/ndejong/digital-multimeter/)
 [![Read the Docs](https://img.shields.io/readthedocs/digital-multimeter)](https://digital-multimeter.readthedocs.io)
 ![License](https://img.shields.io/github/license/ndejong/digital-multimeter.svg)
 
-Digital Multimeter provides both a command-line interface and a Python module interface to receive data from a 
-variety of digital multimeters.  Checkout the [list of supported multimeters](https://digital-multimeter.readthedocs.io/en/latest/docs/supported-multimeters).
+Digital Multimeter provides both a CLI and Python API interface to receive data 
+from a variety of digital multimeters.  
+
+See the list of supported multimeters [here](https://digital-multimeter.readthedocs.io/en/latest/docs/supported-multimeters).
 
 ## Features
 * Command line and Python module interface to digital multimeters
 * Continuous live data readings (using `--count 0`)
 * Output in **json** or **csv** formats
 * Output to console or file, allowing other tools to pickup and use the data
 * Configuration via config-file or environment-variables
 * Easy to expand for new digital-multimeter protocols
 * Easy installation using PyPI `pip`
-* Plenty of documentation and examples - https://digital-multimeter.readthedocs.io
+* Documentation and examples at [digital-multimeter.readthedocs.io](https://digital-multimeter.readthedocs.io)
 
 ## Installation
 ```shell
-user@computer:~$ pip3 install digital-multimeter
+user@computer:~$ pip install [--upgrade] digital-multimeter
 ```
 
-## Command Line Usage
-Continuously read the digital-multimeter and pipe the JSON output through `jq` making it look prettier.
+## CLI Usage Example
+Continuously read the digital-multimeter and pipe the JSON output through `jq` to 
+make the JSON output look prettier.
 ```shell
 user@computer:~$ dmm read --connect /dev/ttyUSB0 --count 0 | jq .
 {
   "reading": {
     "value": 156.70000000000002,
     "unit_name": "volts",
     "unit_symbol": "V",
@@ -71,21 +52,17 @@
     "timestamp": 1605936374.7694516,
     "unit_name": "second",
     "unit_symbol": "s"
   }
 }
 ```
 
-Plenty more command-line examples [available here](https://digital-multimeter.readthedocs.io/en/latest/docs/command-line/examples/).
-
-## Python Module Usage
-Python-module documentation is [available here](https://digital-multimeter.readthedocs.io/en/latest/docs/python-module/).
+## Python API Usage
+Python-module documentation is available [here](https://digital-multimeter.readthedocs.io/en/latest/docs/python-module/).
 
 ## Project
 * Github - [github.com/ndejong/digital-multimeter](https://github.com/ndejong/digital-multimeter)
 * PyPI - [pypi.python.org/pypi/digital-multimeter](https://pypi.python.org/pypi/digital-multimeter/)
 * ReadTheDocs - [digital-multimeter.readthedocs.io](https://digital-multimeter.readthedocs.io)
 
 ---
-Copyright &copy; 2021-2022 [Nicholas de Jong](https://www.nicholasdejong.com)
-
-
+Copyright &copy; 2021-2023 [Nicholas de Jong](https://www.nicholasdejong.com)
```

### Comparing `digital-multimeter-0.4.0/src/digital_multimeter/cli/click.py` & `digital_multimeter-0.5.1/src/digital_multimeter/cli/click.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import sys
-import click
 import logging
+import sys
 import warnings
 
-from digital_multimeter import __version__ as VERSION
-from digital_multimeter import __env_connect__ as ENV_CONNECT
-from digital_multimeter.exceptions.MultimeterException import MultimeterException
+import click
+
+from digital_multimeter import __env_connect__ as ENV_CONNECT, __version__ as VERSION
 from digital_multimeter.cli.config import Config
-from digital_multimeter.utils.cli_output import cli_output
-from digital_multimeter.DigitalMultimeter import DigitalMultimeter
+from digital_multimeter.exceptions import MultimeterException
+from digital_multimeter.main import DigitalMultimeter
+from digital_multimeter.utils import cli_output
 
 
 @click.group()
 @click.option("-q", "--quiet", is_flag=True, help="Quiet mode; priority over --verbose")
 @click.option("-v", "--verbose", is_flag=True, help="Verbose logging; debug level.")
 @click.option("-W", "--disable-warnings", is_flag=True, help="Disable Python warnings.")
 @click.version_option(VERSION)
 def dmm(quiet, verbose, disable_warnings):
     """
-    Digital multimeter CLI tool utilizing the Python3 DigitalMultimeter module.
+    Digital multimeter CLI tool utilizing the DigitalMultimeter() module.
 
     Configuration can be achieved through command arguments, environment values or config file.
 
     Documentation available https://digital-multimeter.readthedocs.io
     """
 
     if quiet:
```

### Comparing `digital-multimeter-0.4.0/src/digital_multimeter/cli/config.py` & `digital_multimeter-0.5.1/src/digital_multimeter/cli/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-import os
-import logging
-import functools
 import configparser
+import functools
+import logging
+import os
 
-from digital_multimeter import __env_model__ as ENV_MODEL
-from digital_multimeter import __env_connect__ as ENV_CONNECT
-from digital_multimeter import __config_file_user__ as CONFIG_FILE_USER
-from digital_multimeter import __config_file_system__ as CONFIG_FILE_SYSTEM
-from digital_multimeter import __config_section_name__ as CONFIG_SECTION_NAME
-from digital_multimeter.exceptions.MultimeterException import MultimeterException
-
+from digital_multimeter import (
+    __config_file_system__ as CONFIG_FILE_SYSTEM,
+    __config_file_user__ as CONFIG_FILE_USER,
+    __config_section_name__ as CONFIG_SECTION_NAME,
+    __env_connect__ as ENV_CONNECT,
+    __env_model__ as ENV_MODEL,
+)
+from digital_multimeter.exceptions import MultimeterException
 
 logger = logging.getLogger(__name__)
 
 
 class ConfigException(MultimeterException):
     pass
 
 
 class Config:
-
     session_config_file = None
 
     def __init__(self, session_config_file=None):
         self.session_config_file = session_config_file
 
     def __getattr__(self, item):
         return self.get(item)
 
     @functools.lru_cache()
     def get(self, item):
-
         if not self.session_config_file:
             if item == "connect":  # serial port
                 env_name = ENV_CONNECT
             elif item == "model":  # dmm model
                 env_name = ENV_MODEL
             else:
                 raise ConfigException("Unknown configuration attribute requested.", item)
@@ -45,15 +44,14 @@
                 return os.environ.get(env_name)
 
         # Configuration file based config setting
         return self.__get_config_from_file(item)
 
     @functools.lru_cache()
     def __get_config_from_file(self, item):
-
         config = None
 
         if self.session_config_file and not os.path.isfile(os.path.expanduser(self.session_config_file)):
             raise ConfigException("Unable to find the configuration filename supplied.", self.session_config_file)
 
         config_files = [self.session_config_file, CONFIG_FILE_USER, CONFIG_FILE_SYSTEM]
 
@@ -72,18 +70,16 @@
             return None
 
         logger.debug('"{}" returned from the configuration file.'.format(item))
         return config[_item]
 
     @functools.lru_cache()
     def __load_config_file(self, filename, section=CONFIG_SECTION_NAME):
-
         filename = os.path.expanduser(filename)
         if os.path.isfile(filename):
-
             cp = configparser.ConfigParser()
 
             try:
                 cp.read(filename)
             except Exception as e:
                 raise ConfigException("Unable to correctly parse the configuration file provided.", e)
```

### Comparing `digital-multimeter-0.4.0/src/digital_multimeter/multimeters/MultimeterEDI9604.py` & `digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterEDI9604.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from struct import pack
-import time
-import serial
 import logging
+import time
 
+import serial
 from serial import SerialException
-from digital_multimeter.exceptions.MultimeterException import MultimeterException
-from digital_multimeter.multimeters.MultimeterBase import MultimeterBase
+
+from ..exceptions import MultimeterException
+from ..multimeters.MultimeterBase import MultimeterBase
 
 SERIAL_BAUD = 2400
 SERIAL_PARITY = "N"
 SERIAL_STOPBITS = 1
 PACKET_RETRY_LIMIT = 3
 
 logger = logging.getLogger(__name__)
 
 
 class MultimeterEDI9604Exception(MultimeterException):
     pass
 
 
 class MultimeterEDI9604(MultimeterBase):
-
     serial = None
 
     def __init__(self, connect):
         super().__init__()
         try:
             self.serial = serial.Serial(
                 port=connect, baudrate=SERIAL_BAUD, parity=SERIAL_PARITY, stopbits=SERIAL_STOPBITS
```

### Comparing `digital-multimeter-0.4.0/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py` & `digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import time
-import serial
 import logging
+import time
 
+import serial
 from serial import SerialException
-from digital_multimeter.exceptions.MultimeterException import MultimeterException
-from digital_multimeter.multimeters.MultimeterBase import MultimeterBase
+
+from ..exceptions import MultimeterException
+from ..multimeters.MultimeterBase import MultimeterBase
 
 SERIAL_BAUD = 2400
 SERIAL_PARITY = "N"
 SERIAL_STOPBITS = 1
 PACKET_RETRY_LIMIT = 3
 
 logger = logging.getLogger(__name__)
 
 
 class MultimeterFortuneFS9721Exception(MultimeterException):
     pass
 
 
 class MultimeterFortuneFS9721(MultimeterBase):
-
     serial = None
 
     def __init__(self, connect):
         super().__init__()
         try:
             self.serial = serial.Serial(
                 port=connect, baudrate=SERIAL_BAUD, parity=SERIAL_PARITY, stopbits=SERIAL_STOPBITS
```

### Comparing `digital-multimeter-0.4.0/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py` & `digital_multimeter-0.5.1/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,24 @@
     Thanks to the following projects (which knowledge is partially used here):
     - sigrok (https://github.com/martinling/libsigrok/blob/master/src/dmm/vc870.c)
     - https://github.com/jsyk/VC870_USB_Datalog
     - http://erste.de/UT61/index.html
     - https://github.com/pklaus/ut61e_python
 """
 
-import time
 import logging
-import re
 import math
+import re
+import time
+
 import usb.core
 import usb.util
 
-from digital_multimeter.exceptions.MultimeterException import MultimeterException
-from digital_multimeter.multimeters.MultimeterBase import MultimeterBase
+from ..exceptions import MultimeterException
+from ..multimeters.MultimeterBase import MultimeterBase
 
 UART_SPEED = 9600
 
 PACKET_RETRY_LIMIT = 3
 PACKET_SIZE = 23
 PACKET_TERMINATOR = "\r\n"
 ALLOWED_DATA = range(0x30, 0x40)
@@ -55,15 +56,14 @@
 
 
 class MultimeterVC870USBHIDException(MultimeterException):
     pass
 
 
 class MultimeterVC870USBHID(MultimeterBase):
-
     dev = None
     ep = None
     buffer = ""
 
     def __init__(self, connect):
         super().__init__()
         self.interface_open(connect)
@@ -283,15 +283,15 @@
             "81": ("ACA", "A", 1e-3),
             "90": ("Act+Apar_Power", "W", 0.1, "VA", 0.1),
             "91": ("PowFactor+Freq", "cos_fi", 1e-3, "Hz", 0.1),
             "92": ("VoltEff+CurrEff", "V", 0.1, "A", 0.1),
         }
 
         operation_mode = id_to_op_mode.get(operation_id)
-        if operation_mode == None:
+        if operation_mode is None:
             raise MultimeterVC870USBHIDException("Unsupported digital multimeter mode from packet")
 
         return operation_mode
 
     def _parse_packet_display_value(self, packet):
         value = int(packet[3:8])
         aux_value = int(packet[8:13])
```

### Comparing `digital-multimeter-0.4.0/src/digital_multimeter/multimeters/__init__.py` & `digital_multimeter-0.5.1/src/digital_multimeter/multimeters/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #
 # Digital Multimeter models
 #
+# The __multimeter_models__ dict maps DMM product-models to their chipset implementations as
+# code, thus making it possible to map multiple products to the same chipsets
+#
+# References:
+#  - MultimeterFortuneFS9721 https://www.ic-fortune.com/upload/Download/FS9721_LP3-DS-21_EN.pdf
+#  - MultimeterVC870USBHID ??
+#  - MultimeterEDI9604 ??
+#
 
-multimeter_models = {
-    # MultimeterFortuneFS9721
-    # Models that use the Fortune FS9721 chipset - search for "site:ic-fortune.com FS9721"
+__multimeter_models__ = {
     "Default": "MultimeterFortuneFS9721",
+    "Digitec_DT9604": "MultimeterEDI9604",
     "Digitech_QM1538": "MultimeterFortuneFS9721",
     "Digitek_DT4000ZC": "MultimeterFortuneFS9721",
+    "Editronic_EDI9604": "MultimeterEDI9604",
     "PCE_PCEDM32": "MultimeterFortuneFS9721",
     "Tecpel_DMM8062": "MultimeterFortuneFS9721",
     "TekPower_TP4000ZC": "MultimeterFortuneFS9721",
     "UniTrend_UT30A": "MultimeterFortuneFS9721",
     "UniTrend_UT30E": "MultimeterFortuneFS9721",
     "UniTrend_UT60E": "MultimeterFortuneFS9721",
     "Voltcraft_VC820": "MultimeterFortuneFS9721",
     "Voltcraft_VC840": "MultimeterFortuneFS9721",
-
-    # MultimeterVC870USBHID
     "Voltcraft_VC870": "MultimeterVC870USBHID",
-
-    # MultimeterEDI9604
-    "Editronic_EDI9604": "MultimeterEDI9604",
-    "Digitec_DT9604": "MultimeterEDI9604",
 }
```

### Comparing `digital-multimeter-0.4.0/src/digital_multimeter/utils/cli_output.py` & `digital_multimeter-0.5.1/src/digital_multimeter/utils/cli_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import sys
 import json
-from digital_multimeter.exceptions.MultimeterException import MultimeterException
+import sys
+
+from digital_multimeter.exceptions import MultimeterException
 
 
 def cli_output(data, format="json", output="stdout", count=0):
     if format.lower() == "json":
         out = _json_format(data)
     elif format.lower() == "csv":
         out = _csv_format(data, delimiter="_", row=count)
```

### Comparing `digital-multimeter-0.4.0/src/digital_multimeter.egg-info/PKG-INFO` & `digital_multimeter-0.5.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,67 @@
 Metadata-Version: 2.1
 Name: digital-multimeter
-Version: 0.4.0
-Summary: Digital Multimeter provides both a CLI interface and a Python3 library interface to receive data from a variety of digital multimeters.
-Home-page: https://digital-multimeter.readthedocs.io/
+Version: 0.5.1
+Summary: Digital Multimeter provides both a CLI interface and a Python API interface to receive data from a variety of digital multimeters.
+License: BSD-2-Clause
+Keywords: multimeter,digital multimeter,dmm,Digitech,Digitek,TekPower,UniTrend,Voltcraft
 Author: Nicholas de Jong
 Author-email: contact@nicholasdejong.com
-License: BSD2
-Keywords: multimeter,digital multimeter,dmm,Fortune FS9721
-Platform: UNKNOWN
+Requires-Python: >=3.5,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.5.0,<4.0.0
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: click (>=7.0.0,<9.0.0)
+Requires-Dist: pyserial (>=3.0.0,<4.0.0)
+Requires-Dist: pyusb (>=1.0.0,<2.0.0)
+Project-URL: Bug Tracker, https://github.com/ndejong/digital-multimeter/issues
+Project-URL: Documentation, https://digital-multimeter.readthedocs.io/en/latest/
+Project-URL: Homepage, https://digital-multimeter.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/ndejong/digital-multimeter.git
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Digital Multimeter
 [![PyPi](https://img.shields.io/pypi/v/digital-multimeter.svg)](https://pypi.python.org/pypi/digital-multimeter/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/digital-multimeter.svg)](https://github.com/ndejong/digital-multimeter/)
 [![Read the Docs](https://img.shields.io/readthedocs/digital-multimeter)](https://digital-multimeter.readthedocs.io)
 ![License](https://img.shields.io/github/license/ndejong/digital-multimeter.svg)
 
-Digital Multimeter provides both a command-line interface and a Python module interface to receive data from a 
-variety of digital multimeters.  Checkout the [list of supported multimeters](https://digital-multimeter.readthedocs.io/en/latest/docs/supported-multimeters).
+Digital Multimeter provides both a CLI and Python API interface to receive data 
+from a variety of digital multimeters.  
+
+See the list of supported multimeters [here](https://digital-multimeter.readthedocs.io/en/latest/docs/supported-multimeters).
 
 ## Features
 * Command line and Python module interface to digital multimeters
 * Continuous live data readings (using `--count 0`)
 * Output in **json** or **csv** formats
 * Output to console or file, allowing other tools to pickup and use the data
 * Configuration via config-file or environment-variables
 * Easy to expand for new digital-multimeter protocols
 * Easy installation using PyPI `pip`
-* Plenty of documentation and examples - https://digital-multimeter.readthedocs.io
+* Documentation and examples at [digital-multimeter.readthedocs.io](https://digital-multimeter.readthedocs.io)
 
 ## Installation
 ```shell
-user@computer:~$ pip3 install digital-multimeter
+user@computer:~$ pip install [--upgrade] digital-multimeter
 ```
 
-## Command Line Usage
-Continuously read the digital-multimeter and pipe the JSON output through `jq` making it look prettier.
+## CLI Usage Example
+Continuously read the digital-multimeter and pipe the JSON output through `jq` to 
+make the JSON output look prettier.
 ```shell
 user@computer:~$ dmm read --connect /dev/ttyUSB0 --count 0 | jq .
 {
   "reading": {
     "value": 156.70000000000002,
     "unit_name": "volts",
     "unit_symbol": "V",
@@ -71,21 +83,18 @@
     "timestamp": 1605936374.7694516,
     "unit_name": "second",
     "unit_symbol": "s"
   }
 }
 ```
 
-Plenty more command-line examples [available here](https://digital-multimeter.readthedocs.io/en/latest/docs/command-line/examples/).
-
-## Python Module Usage
-Python-module documentation is [available here](https://digital-multimeter.readthedocs.io/en/latest/docs/python-module/).
+## Python API Usage
+Python-module documentation is available [here](https://digital-multimeter.readthedocs.io/en/latest/docs/python-module/).
 
 ## Project
 * Github - [github.com/ndejong/digital-multimeter](https://github.com/ndejong/digital-multimeter)
 * PyPI - [pypi.python.org/pypi/digital-multimeter](https://pypi.python.org/pypi/digital-multimeter/)
 * ReadTheDocs - [digital-multimeter.readthedocs.io](https://digital-multimeter.readthedocs.io)
 
 ---
-Copyright &copy; 2021-2022 [Nicholas de Jong](https://www.nicholasdejong.com)
-
+Copyright &copy; 2021-2023 [Nicholas de Jong](https://www.nicholasdejong.com)
```

