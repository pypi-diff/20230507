# Comparing `tmp/pipkin-2.0b1.tar.gz` & `tmp/pipkin-2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipkin-2.0b1.tar", last modified: Mon May  1 05:02:01 2023, max compression
+gzip compressed data, was "pipkin-2.0b2.tar", last modified: Sun May  7 17:28:04 2023, max compression
```

## Comparing `pipkin-2.0b1.tar` & `pipkin-2.0b2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-01 05:02:01.486686 pipkin-2.0b1/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1070 2023-04-27 17:16:03.000000 pipkin-2.0b1/LICENSE
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       25 2023-04-27 17:16:03.000000 pipkin-2.0b1/MANIFEST.in
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    10700 2023-05-01 05:02:01.486524 pipkin-2.0b1/PKG-INFO
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     9404 2023-04-27 17:16:03.000000 pipkin-2.0b1/README.rst
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-01 05:02:01.482029 pipkin-2.0b1/pipkin/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     1738 2023-05-01 04:58:42.000000 pipkin-2.0b1/pipkin/__init__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2114 2023-04-27 17:16:03.000000 pipkin-2.0b1/pipkin/__main__.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    16912 2023-04-30 17:06:48.000000 pipkin-2.0b1/pipkin/adapters.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    33592 2023-04-30 06:24:37.000000 pipkin-2.0b1/pipkin/bare_metal.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      355 2023-04-27 17:16:03.000000 pipkin-2.0b1/pipkin/common.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6242 2023-04-30 06:23:56.000000 pipkin-2.0b1/pipkin/connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    10546 2023-04-27 17:16:03.000000 pipkin-2.0b1/pipkin/parser.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    23522 2023-04-30 07:11:11.000000 pipkin-2.0b1/pipkin/proxy.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     6597 2023-04-30 06:10:39.000000 pipkin-2.0b1/pipkin/serial_connection.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    27819 2023-04-30 06:10:39.000000 pipkin-2.0b1/pipkin/session.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     7156 2023-04-30 08:11:24.000000 pipkin-2.0b1/pipkin/util.py
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     4600 2023-04-30 06:25:03.000000 pipkin-2.0b1/pipkin/webrepl_connection.py
-drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-01 05:02:01.486312 pipkin-2.0b1/pipkin.egg-info/
--rw-r--r--   0 aivarannamaa   (502) staff       (20)    10700 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/PKG-INFO
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      492 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/SOURCES.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)        1 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/dependency_links.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       39 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/entry_points.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       34 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/requires.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)        7 2023-05-01 05:02:01.000000 pipkin-2.0b1/pipkin.egg-info/top_level.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)      155 2023-04-27 17:16:03.000000 pipkin-2.0b1/pyproject.toml
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       34 2023-05-01 05:01:05.000000 pipkin-2.0b1/requirements.txt
--rw-r--r--   0 aivarannamaa   (502) staff       (20)       38 2023-05-01 05:02:01.486732 pipkin-2.0b1/setup.cfg
--rw-r--r--   0 aivarannamaa   (502) staff       (20)     2105 2023-04-27 17:16:03.000000 pipkin-2.0b1/setup.py
+drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-07 17:28:04.066891 pipkin-2.0b2/
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     1070 2023-04-27 17:16:03.000000 pipkin-2.0b2/LICENSE
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       25 2023-04-27 17:16:03.000000 pipkin-2.0b2/MANIFEST.in
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    10712 2023-05-07 17:28:04.066569 pipkin-2.0b2/PKG-INFO
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     9416 2023-05-02 04:34:47.000000 pipkin-2.0b2/README.rst
+drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-07 17:28:04.063984 pipkin-2.0b2/pipkin/
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     1738 2023-05-07 17:23:27.000000 pipkin-2.0b2/pipkin/__init__.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     2114 2023-05-07 17:23:27.000000 pipkin-2.0b2/pipkin/__main__.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    16912 2023-04-30 17:06:48.000000 pipkin-2.0b2/pipkin/adapters.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    33592 2023-04-30 06:24:37.000000 pipkin-2.0b2/pipkin/bare_metal.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)      355 2023-04-27 17:16:03.000000 pipkin-2.0b2/pipkin/common.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     6242 2023-04-30 06:23:56.000000 pipkin-2.0b2/pipkin/connection.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    10546 2023-04-27 17:16:03.000000 pipkin-2.0b2/pipkin/parser.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    25889 2023-05-07 17:18:16.000000 pipkin-2.0b2/pipkin/proxy.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     6597 2023-04-30 06:10:39.000000 pipkin-2.0b2/pipkin/serial_connection.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    27819 2023-04-30 06:10:39.000000 pipkin-2.0b2/pipkin/session.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     7156 2023-04-30 08:11:24.000000 pipkin-2.0b2/pipkin/util.py
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     4600 2023-04-30 06:25:03.000000 pipkin-2.0b2/pipkin/webrepl_connection.py
+drwxr-xr-x   0 aivarannamaa   (502) staff       (20)        0 2023-05-07 17:28:04.066300 pipkin-2.0b2/pipkin.egg-info/
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)    10712 2023-05-07 17:28:03.000000 pipkin-2.0b2/pipkin.egg-info/PKG-INFO
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)      492 2023-05-07 17:28:03.000000 pipkin-2.0b2/pipkin.egg-info/SOURCES.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)        1 2023-05-07 17:28:03.000000 pipkin-2.0b2/pipkin.egg-info/dependency_links.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       39 2023-05-07 17:28:03.000000 pipkin-2.0b2/pipkin.egg-info/entry_points.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       34 2023-05-07 17:28:03.000000 pipkin-2.0b2/pipkin.egg-info/requires.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)        7 2023-05-07 17:28:03.000000 pipkin-2.0b2/pipkin.egg-info/top_level.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)      155 2023-04-27 17:16:03.000000 pipkin-2.0b2/pyproject.toml
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       34 2023-05-01 05:01:05.000000 pipkin-2.0b2/requirements.txt
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)       38 2023-05-07 17:28:04.066951 pipkin-2.0b2/setup.cfg
+-rw-r--r--   0 aivarannamaa   (502) staff       (20)     2105 2023-04-27 17:16:03.000000 pipkin-2.0b2/setup.py
```

### Comparing `pipkin-2.0b1/LICENSE` & `pipkin-2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/PKG-INFO` & `pipkin-2.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipkin
-Version: 2.0b1
+Version: 2.0b2
 Summary: Tool for installing packages for MicroPython and CircuitPython
 Home-page: https://github.com/aivarannamaa/pipkin
 Author: Aivar Annamaa
 License: MIT
 Project-URL: Source code, https://github.com/aivarannamaa/pipkin
 Project-URL: Bug tracker, https://github.com/aivarannamaa/pipkin/issues
 Keywords: MicroPython CircuitPython pip upip
@@ -32,18 +32,18 @@
 Requires-Python: >=3.7
 License-File: LICENSE
 
 pipkin
 =======
 Tool for managing distribution packages for MicroPython and CircuitPython on target devices or in a local directory.
 
-Supports both `upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
+Supports `mip- and upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
 and regular pip-compatible packages.
 
-By default it prefers packages at micropython.org-s index. If the package or the required version is not
+By default it prefers micrpython-lib packages at https://micropython.org/pi/v2/index.json. If the package is not
 found there, then it turns to PyPI.
 
 Unlike some of the package managers for MicroPython and CircuitPython, pipkin keeps a minimal set of package
 metadata (trimmed .dist-info/METADATA and .dist-info/RECORD) next to the package itself, just like pip.
 This enables straigthforward approach for uninstalling, listing and freezing.
 
 When installing with ``--compile`` switch, pipkin uses suitable `mpy-cross` to compile the
```

### Comparing `pipkin-2.0b1/README.rst` & `pipkin-2.0b2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pipkin
 =======
 Tool for managing distribution packages for MicroPython and CircuitPython on target devices or in a local directory.
 
-Supports both `upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
+Supports `mip- and upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
 and regular pip-compatible packages.
 
-By default it prefers packages at micropython.org-s index. If the package or the required version is not
+By default it prefers micrpython-lib packages at https://micropython.org/pi/v2/index.json. If the package is not
 found there, then it turns to PyPI.
 
 Unlike some of the package managers for MicroPython and CircuitPython, pipkin keeps a minimal set of package
 metadata (trimmed .dist-info/METADATA and .dist-info/RECORD) next to the package itself, just like pip.
 This enables straigthforward approach for uninstalling, listing and freezing.
 
 When installing with ``--compile`` switch, pipkin uses suitable `mpy-cross` to compile the
```

### Comparing `pipkin-2.0b1/pipkin/__init__.py` & `pipkin-2.0b2/pipkin/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pipkin.adapters import Adapter, DummyAdapter, create_adapter
 from pipkin.common import ManagementError, UserError
 from pipkin.session import Session
 
 logger = logging.getLogger("pipkin")
 
-__version__ = "2.0b1"
+__version__ = "2.0b2"
 
 
 def error(msg):
     msg = "ERROR: " + msg
     print(msg, file=sys.stderr)
 
     return 1
```

### Comparing `pipkin-2.0b1/pipkin/__main__.py` & `pipkin-2.0b2/pipkin/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 MIT License
 
-Copyright (c) 2022 Aivar Annamaa
+Copyright (c) 2023 Aivar Annamaa
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pipkin-2.0b1/pipkin/adapters.py` & `pipkin-2.0b2/pipkin/adapters.py`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/pipkin/bare_metal.py` & `pipkin-2.0b2/pipkin/bare_metal.py`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/pipkin/connection.py` & `pipkin-2.0b2/pipkin/connection.py`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/pipkin/parser.py` & `pipkin-2.0b2/pipkin/parser.py`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/pipkin/proxy.py` & `pipkin-2.0b2/pipkin/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import subprocess
 import sys
 import tarfile
 import tempfile
 import textwrap
 import threading
 import zipfile
-from abc import ABC
+from abc import ABC, abstractmethod
 from html.parser import HTMLParser
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from socketserver import BaseServer
 from textwrap import dedent
 from typing import Any, Dict, List, Optional, Tuple, Union
 from urllib.error import HTTPError
 from urllib.request import urlopen
@@ -51,14 +51,15 @@
 
 from pipkin.util import (
     create_dist_info_version_name,
     custom_normalize_dist_name,
     parse_dist_file_name,
 )
 
+MP_ORG_INDEX_V1 = "https://micropython.org/pi"
 MP_ORG_INDEX_V2 = "https://micropython.org/pi/v2"
 PYPI_SIMPLE_INDEX = "https://pypi.org/simple"
 SERVER_ENCODING = "utf-8"
 
 # https://github.com/adafruit/circuitpython-build-tools/blob/de44a709f6287d2759df14c89707f2d8f5a026f5/circuitpython_build_tools/scripts/build_bundles.py#L42
 NORMALIZED_IRRELEVANT_PACKAGE_NAMES = {
     "adafruit_blinka",
@@ -108,62 +109,53 @@
         pass
 
 
 class BaseIndexDownloader(ABC):
     def __init__(self, index_url: str):
         self._index_url = index_url.rstrip("/")
 
+    @abstractmethod
     def get_dist_file_names(self, dist_name: str) -> Optional[List[str]]:
         raise NotImplementedError()
 
+    @abstractmethod
     def get_file_content(self, dist_name: str, file_name: str) -> bytes:
         raise NotImplementedError()
 
 
-class SimpleIndexDownloader(BaseIndexDownloader):
+class RegularIndexDownloader(BaseIndexDownloader, ABC):
     def __init__(self, index_url: str):
         super().__init__(index_url)
         self._dist_urls_cache: Dict[str, Dict[str, str]] = {}
 
     def get_dist_file_names(self, dist_name: str) -> Optional[List[str]]:
         urls = self._get_dist_urls(dist_name)
         if urls is None:
             return None
         return list(urls.keys())
 
+    def get_file_content(self, dist_name: str, file_name: str) -> bytes:
+        if self._should_return_dummy(dist_name):
+            return create_dummy_dist(dist_name, file_name)
+        else:
+            original_bytes = self._download_file(dist_name, file_name)
+            return self._tweak_file(dist_name, file_name, original_bytes)
+
     def _get_dist_urls(self, dist_name: str) -> Optional[Dict[str, str]]:
         """
         Returns file names and url-s for constructing the dist index page.
         """
         if dist_name not in self._dist_urls_cache:
             self._dist_urls_cache[dist_name] = self._download_file_urls(dist_name)
 
         return self._dist_urls_cache[dist_name]
 
+    @abstractmethod
     def _download_file_urls(self, dist_name) -> Optional[Dict[str, str]]:
-        url = f"{self._index_url}/{dist_name}"
-        logger.info("Downloading file urls from simple index %s", url)
-
-        try:
-            with urlopen(url) as fp:
-                parser = SimpleUrlsParser()
-                parser.feed(fp.read().decode("utf-8"))
-                return parser.file_urls
-        except HTTPError as e:
-            if e.code == 404:
-                return None
-            else:
-                raise e
-
-    def get_file_content(self, dist_name: str, file_name: str) -> bytes:
-        if self._should_return_dummy(dist_name):
-            return create_dummy_dist(dist_name, file_name)
-        else:
-            original_bytes = self._download_file(dist_name, file_name)
-            return self._tweak_file(dist_name, file_name, original_bytes)
+        raise NotImplementedError()
 
     def _download_file(self, dist_name: str, file_name: str) -> bytes:
         urls = self._get_dist_urls(dist_name)
         assert urls
 
         assert file_name in urls
         url = urls[file_name]
@@ -356,14 +348,71 @@
         # include all other files as package data
         src += "    package_data={'*': ['*', '*/*', '*/*/*', '*/*/*/*', '*/*/*/*/*', '*/*/*/*/*/*', '*/*/*/*/*/*/*', '*/*/*/*/*/*/*/*']}\n"
 
         src += ")\n"
         return src
 
 
+class SimpleIndexDownloader(RegularIndexDownloader):
+    def _download_file_urls(self, dist_name) -> Optional[Dict[str, str]]:
+        url = f"{self._index_url}/{dist_name}"
+        logger.info("Downloading file urls from simple index %s", url)
+
+        try:
+            with urlopen(url) as fp:
+                parser = SimpleUrlsParser()
+                parser.feed(fp.read().decode("utf-8"))
+                return parser.file_urls
+        except HTTPError as e:
+            if e.code == 404:
+                return None
+            else:
+                raise e
+
+
+class JsonIndexDownloader(RegularIndexDownloader):
+    def _download_file_urls(self, dist_name) -> Optional[Dict[str, str]]:
+        metadata_url = f"{self._index_url}/{dist_name}/json"
+        logger.info("Downloading file urls from json index at %s", metadata_url)
+
+        result = {}
+        try:
+            with urlopen(metadata_url) as fp:
+                data = json.load(fp)
+                releases = data["releases"]
+                for ver in releases:
+                    for file in releases[ver]:
+                        file_url = file["url"]
+                        if "filename" in file:
+                            file_name = file["filename"]
+                        else:
+                            # micropython.org/pi doesn't have it
+                            file_name = file_url.split("/")[-1]
+                            # may be missing micropython prefix
+                            if not file_name.startswith(dist_name):
+                                # Let's hope version part doesn't contain dashes
+                                _, suffix = file_name.split("-")
+                                file_name = dist_name + "-" + suffix
+                        result[file_name] = file_url
+        except HTTPError as e:
+            if e.code == 404:
+                return None
+            else:
+                raise e
+        return result
+
+
+class MpOrgV1IndexDownloader(JsonIndexDownloader):
+    def _download_file_urls(self, dist_name) -> Optional[Dict[str, str]]:
+        if not custom_normalize_dist_name(dist_name).startswith("micropython_"):
+            return None
+
+        return super()._download_file_urls(dist_name)
+
+
 class MpOrgV2IndexDownloader(BaseIndexDownloader):
     def __init__(self, index_url):
         self._packages = None
         super().__init__(index_url)
 
     def get_dist_file_names(self, dist_name: str) -> Optional[List[str]]:
         # there is no per-package, all-versions metadata resource. Need to use the global index
@@ -492,14 +541,16 @@
 class PipkinProxy(HTTPServer):
     def __init__(
         self, no_mp_org: bool, index_url: Optional[str], extra_index_urls: List[str], port: int
     ):
         self._downloaders: List[BaseIndexDownloader] = []
         self._downloaders_by_dist_name: Dict[str, Optional[BaseIndexDownloader]] = {}
         if not no_mp_org:
+            # V1 first, because it only considers packages with "micropython-"-prefix
+            self._downloaders.append(MpOrgV1IndexDownloader(MP_ORG_INDEX_V1))
             self._downloaders.append(MpOrgV2IndexDownloader(MP_ORG_INDEX_V2))
         self._downloaders.append(SimpleIndexDownloader(index_url or PYPI_SIMPLE_INDEX))
         for url in extra_index_urls:
             self._downloaders.append(SimpleIndexDownloader(url))
         super().__init__(("127.0.0.1", port), PipkinProxyHandler)
 
     def get_downloader_for_dist(self, dist_name: str) -> Optional[BaseIndexDownloader]:
@@ -585,18 +636,24 @@
 
 
 def start_proxy(
     no_mp_org: bool,
     index_url: Optional[str],
     extra_index_urls: List[str],
 ) -> PipkinProxy:
+    port = PREFERRED_PORT
+    if no_mp_org:
+        # Use different port for different set of source indexes, otherwise
+        # pip may use wrong cached wheel.
+        port += 7
     try:
-        proxy = PipkinProxy(no_mp_org, index_url, extra_index_urls, PREFERRED_PORT)
+        proxy = PipkinProxy(no_mp_org, index_url, extra_index_urls, port)
     except OSError as e:
         if e.errno == errno.EADDRINUSE:
+            logger.warning("Port %s was in use. Letting OS choose.", port)
             proxy = PipkinProxy(no_mp_org, index_url, extra_index_urls, 0)
         else:
             raise e
 
     server_thread = threading.Thread(target=proxy.serve_forever)
     server_thread.start()
```

### Comparing `pipkin-2.0b1/pipkin/serial_connection.py` & `pipkin-2.0b2/pipkin/serial_connection.py`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/pipkin/session.py` & `pipkin-2.0b2/pipkin/session.py`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/pipkin/util.py` & `pipkin-2.0b2/pipkin/util.py`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/pipkin/webrepl_connection.py` & `pipkin-2.0b2/pipkin/webrepl_connection.py`

 * *Files identical despite different names*

### Comparing `pipkin-2.0b1/pipkin.egg-info/PKG-INFO` & `pipkin-2.0b2/pipkin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipkin
-Version: 2.0b1
+Version: 2.0b2
 Summary: Tool for installing packages for MicroPython and CircuitPython
 Home-page: https://github.com/aivarannamaa/pipkin
 Author: Aivar Annamaa
 License: MIT
 Project-URL: Source code, https://github.com/aivarannamaa/pipkin
 Project-URL: Bug tracker, https://github.com/aivarannamaa/pipkin/issues
 Keywords: MicroPython CircuitPython pip upip
@@ -32,18 +32,18 @@
 Requires-Python: >=3.7
 License-File: LICENSE
 
 pipkin
 =======
 Tool for managing distribution packages for MicroPython and CircuitPython on target devices or in a local directory.
 
-Supports both `upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
+Supports `mip- and upip-compatible packages <https://docs.micropython.org/en/latest/reference/packages.html>`_,
 and regular pip-compatible packages.
 
-By default it prefers packages at micropython.org-s index. If the package or the required version is not
+By default it prefers micrpython-lib packages at https://micropython.org/pi/v2/index.json. If the package is not
 found there, then it turns to PyPI.
 
 Unlike some of the package managers for MicroPython and CircuitPython, pipkin keeps a minimal set of package
 metadata (trimmed .dist-info/METADATA and .dist-info/RECORD) next to the package itself, just like pip.
 This enables straigthforward approach for uninstalling, listing and freezing.
 
 When installing with ``--compile`` switch, pipkin uses suitable `mpy-cross` to compile the
```

### Comparing `pipkin-2.0b1/setup.py` & `pipkin-2.0b2/setup.py`

 * *Files identical despite different names*

