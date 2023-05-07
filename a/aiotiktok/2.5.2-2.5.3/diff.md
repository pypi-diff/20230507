# Comparing `tmp/aiotiktok-2.5.2.tar.gz` & `tmp/aiotiktok-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotiktok-2.5.2.tar", last modified: Thu Mar  2 14:52:34 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aiotiktok-2.5.2.tar` & `aiotiktok-2.5.3.tar`

### file list

```diff
@@ -1,17 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 14:52:34.126731 aiotiktok-2.5.2/
--rw-rw-rw-   0        0        0     1084 2022-09-13 07:38:59.000000 aiotiktok-2.5.2/LICENSE
--rw-rw-rw-   0        0        0     1058 2023-03-02 14:52:34.125729 aiotiktok-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      716 2023-01-22 17:11:45.000000 aiotiktok-2.5.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-02 14:52:34.102915 aiotiktok-2.5.2/aiotiktok/
--rw-rw-rw-   0        0        0       81 2023-03-02 14:52:23.000000 aiotiktok-2.5.2/aiotiktok/__init__.py
--rw-rw-rw-   0        0        0     3667 2023-03-02 14:51:56.000000 aiotiktok-2.5.2/aiotiktok/client.py
--rw-rw-rw-   0        0        0       94 2022-11-17 18:02:37.000000 aiotiktok-2.5.2/aiotiktok/exceptions.py
--rw-rw-rw-   0        0        0      724 2023-01-22 17:10:59.000000 aiotiktok-2.5.2/aiotiktok/types.py
-drwxrwxrwx   0        0        0        0 2023-03-02 14:52:34.124763 aiotiktok-2.5.2/aiotiktok.egg-info/
--rw-rw-rw-   0        0        0     1058 2023-03-02 14:52:33.000000 aiotiktok-2.5.2/aiotiktok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-03-02 14:52:34.000000 aiotiktok-2.5.2/aiotiktok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 14:52:33.000000 aiotiktok-2.5.2/aiotiktok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-02 14:52:33.000000 aiotiktok-2.5.2/aiotiktok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-02 14:52:33.000000 aiotiktok-2.5.2/aiotiktok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-02 14:52:34.126731 aiotiktok-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-03-02 14:52:19.000000 aiotiktok-2.5.2/setup.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/aiotiktok/__init__.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/aiotiktok/client.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/aiotiktok/exceptions.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/aiotiktok/types.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/LICENSE
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/PKG-INFO
```

### Comparing `aiotiktok-2.5.2/LICENSE` & `aiotiktok-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.5.2/PKG-INFO` & `aiotiktok-2.5.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-Metadata-Version: 2.1
-Name: aiotiktok
-Version: 2.5.2
-Summary: Tool for parse tiktok data
-Home-page: https://github.com/sheldygg/aiotiktok
-Author: sheldy
-License: MIT
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AIOtiktok
 
 [![PyPi Package Version](https://img.shields.io/pypi/v/aiotiktok?color=blue)](https://pypi.org/project/aiotiktok/)
 [![Downloads](https://img.shields.io/pypi/dm/aiotiktok?color=blue)](https://pypi.org/project/aiotiktok/)
 
-**aiotiktok** super simple and fast library to get all video data from tiktok
+**aiotiktok** super simple and fast library to get all video data from TikTok
 
 
 **One step before start.**
 - You must install library with pip `pip install aiotiktok`
 - or `pip install git+https://github.com/sheldygg/aiotiktok`
 
 ### Request
 
 ```python
 import asyncio
-from aiotiktok import TiktokClient
+from aiotiktok import Client
 
-tiktok = TiktokClient()
+tiktok = Client()
 
 async def main():
-    data = await tiktok.get_tiktok_data(original_url="some url")
+    data = await tiktok.get_data(url="some url")
     print(data)
     
 asyncio.run(main())
 ```
```

### Comparing `aiotiktok-2.5.2/aiotiktok/types.py` & `aiotiktok-2.5.3/aiotiktok/types.py`

 * *Files identical despite different names*

