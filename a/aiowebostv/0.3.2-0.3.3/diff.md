# Comparing `tmp/aiowebostv-0.3.2.tar.gz` & `tmp/aiowebostv-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiowebostv-0.3.2.tar", last modified: Mon Jan 16 17:34:01 2023, max compression
+gzip compressed data, was "aiowebostv-0.3.3.tar", last modified: Sun May  7 05:52:54 2023, max compression
```

## Comparing `aiowebostv-0.3.2.tar` & `aiowebostv-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:34:01.833587 aiowebostv-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-01-16 17:34:01.833587 aiowebostv-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:34:01.833587 aiowebostv-0.3.2/aiowebostv/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/aiowebostv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/aiowebostv/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/aiowebostv/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/aiowebostv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/aiowebostv/handshake.py
--rw-r--r--   0 runner    (1001) docker     (123)    33270 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/aiowebostv/webos_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:34:01.833587 aiowebostv-0.3.2/aiowebostv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-01-16 17:34:01.000000 aiowebostv-0.3.2/aiowebostv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-16 17:34:01.000000 aiowebostv-0.3.2/aiowebostv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 17:34:01.000000 aiowebostv-0.3.2/aiowebostv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 17:34:01.000000 aiowebostv-0.3.2/aiowebostv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-16 17:34:01.000000 aiowebostv-0.3.2/aiowebostv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-16 17:34:01.000000 aiowebostv-0.3.2/aiowebostv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-16 17:34:01.833587 aiowebostv-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-01-16 17:33:59.000000 aiowebostv-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:52:54.756175 aiowebostv-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-07 05:52:54.756175 aiowebostv-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:52:54.756175 aiowebostv-0.3.3/aiowebostv/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/aiowebostv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/aiowebostv/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/aiowebostv/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/aiowebostv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/aiowebostv/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/aiowebostv/webos_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:52:54.756175 aiowebostv-0.3.3/aiowebostv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-07 05:52:54.000000 aiowebostv-0.3.3/aiowebostv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-07 05:52:54.000000 aiowebostv-0.3.3/aiowebostv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:52:54.000000 aiowebostv-0.3.3/aiowebostv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:52:54.000000 aiowebostv-0.3.3/aiowebostv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 05:52:54.000000 aiowebostv-0.3.3/aiowebostv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 05:52:54.000000 aiowebostv-0.3.3/aiowebostv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 05:52:54.756175 aiowebostv-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-07 05:52:51.000000 aiowebostv-0.3.3/setup.py
```

### Comparing `aiowebostv-0.3.2/LICENSE` & `aiowebostv-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiowebostv-0.3.2/PKG-INFO` & `aiowebostv-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aiowebostv
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to control webOS based LG TV devices
 Home-page: https://github.com/home-assistant-libs/aiowebostv
 Author: Home Assistant Team
 Author-email: hello@home-assistant.io
 License: UNKNOWN
 Download-URL: https://github.com/home-assistant-libs/aiowebostv
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiowebostv
 Python library to control LG webOS based TV devices.
```

### Comparing `aiowebostv-0.3.2/README.md` & `aiowebostv-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `aiowebostv-0.3.2/aiowebostv/buttons.py` & `aiowebostv-0.3.3/aiowebostv/buttons.py`

 * *Files identical despite different names*

### Comparing `aiowebostv-0.3.2/aiowebostv/endpoints.py` & `aiowebostv-0.3.3/aiowebostv/endpoints.py`

 * *Files identical despite different names*

### Comparing `aiowebostv-0.3.2/aiowebostv/handshake.py` & `aiowebostv-0.3.3/aiowebostv/handshake.py`

 * *Files identical despite different names*

### Comparing `aiowebostv-0.3.2/aiowebostv/webos_client.py` & `aiowebostv-0.3.3/aiowebostv/webos_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
             self._extinputs = {}
             self._system_info = None
             self._software_info = None
             self._hello_info = None
             self._sound_output = None
 
             for callback in self.state_update_callbacks:
-                closeout.add(callback(self))
+                closeout.add(asyncio.create_task(callback(self)))
 
             if closeout:
                 closeout_task = asyncio.create_task(asyncio.wait(closeout))
 
                 while not closeout_task.done():
                     try:
                         await asyncio.shield(closeout_task)
```

### Comparing `aiowebostv-0.3.2/aiowebostv.egg-info/PKG-INFO` & `aiowebostv-0.3.3/aiowebostv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aiowebostv
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to control webOS based LG TV devices
 Home-page: https://github.com/home-assistant-libs/aiowebostv
 Author: Home Assistant Team
 Author-email: hello@home-assistant.io
 License: UNKNOWN
 Download-URL: https://github.com/home-assistant-libs/aiowebostv
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiowebostv
 Python library to control LG webOS based TV devices.
```

### Comparing `aiowebostv-0.3.2/setup.py` & `aiowebostv-0.3.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for aiowebostv."""
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.3.2"
+VERSION = "0.3.3"
 
 
 setup(
     name="aiowebostv",
     version=VERSION,
     url="https://github.com/home-assistant-libs/aiowebostv",
     download_url="https://github.com/home-assistant-libs/aiowebostv",
@@ -26,10 +26,11 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Home Automation",
     ],
 )
```

