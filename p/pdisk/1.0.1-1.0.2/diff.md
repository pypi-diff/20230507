# Comparing `tmp/pdisk-1.0.1.tar.gz` & `tmp/pdisk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdisk-1.0.1.tar", last modified: Sat May  6 20:17:17 2023, max compression
+gzip compressed data, was "pdisk-1.0.2.tar", last modified: Sun May  7 06:24:40 2023, max compression
```

## Comparing `pdisk-1.0.1.tar` & `pdisk-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 20:17:17.221432 pdisk-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-05-06 19:48:25.000000 pdisk-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2614 2023-05-06 20:17:17.217911 pdisk-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4295 2023-05-06 19:48:25.000000 pdisk-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 20:17:17.079201 pdisk-1.0.1/pdisk/
--rw-rw-rw-   0        0        0       26 2023-05-06 15:56:36.000000 pdisk-1.0.1/pdisk/__init__.py
--rw-rw-rw-   0        0        0    11319 2023-05-06 19:57:54.000000 pdisk-1.0.1/pdisk/pdisk.py
--rw-rw-rw-   0        0        0     2540 2023-05-06 18:03:15.000000 pdisk-1.0.1/pdisk/type.py
-drwxrwxrwx   0        0        0        0 2023-05-06 20:17:17.213192 pdisk-1.0.1/pdisk.egg-info/
--rw-rw-rw-   0        0        0     2614 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 20:17:17.223085 pdisk-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-05-06 20:16:55.000000 pdisk-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:24:40.504884 pdisk-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-05-06 19:48:25.000000 pdisk-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2614 2023-05-07 06:24:40.490801 pdisk-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4288 2023-05-06 21:59:58.000000 pdisk-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 06:24:40.472992 pdisk-1.0.2/pdisk/
+-rw-rw-rw-   0        0        0       26 2023-05-06 15:56:36.000000 pdisk-1.0.2/pdisk/__init__.py
+-rw-rw-rw-   0        0        0    11369 2023-05-06 21:23:35.000000 pdisk-1.0.2/pdisk/pdisk.py
+-rw-rw-rw-   0        0        0     2540 2023-05-06 18:03:15.000000 pdisk-1.0.2/pdisk/type.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:24:40.488801 pdisk-1.0.2/pdisk.egg-info/
+-rw-rw-rw-   0        0        0     2614 2023-05-07 06:24:39.000000 pdisk-1.0.2/pdisk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-07 06:24:39.000000 pdisk-1.0.2/pdisk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 06:24:39.000000 pdisk-1.0.2/pdisk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 06:24:39.000000 pdisk-1.0.2/pdisk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 06:24:39.000000 pdisk-1.0.2/pdisk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 06:24:40.504884 pdisk-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2023-05-06 21:59:12.000000 pdisk-1.0.2/setup.py
```

### Comparing `pdisk-1.0.1/LICENSE` & `pdisk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdisk-1.0.1/PKG-INFO` & `pdisk-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdisk
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Unofficial Asynchronous Python version of pdisk API wrapper
 Home-page: https://github.com/kalanakt/pdisk
 Author: kalanakt
 Author-email: kalanakt@uvew.xyz
 License: MIT
 Keywords: python,pdisk,earn money 
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pdisk-1.0.1/README.md` & `pdisk-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     <p align="center">
 <!-- <p align='center'>
   <img alt="GitHub Sparkline" src="https://github.com/gramscript/gramscript">
 </p> -->
         <a href=""><img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/kalanakt/pdisk?logo=files&logoColor=f72585"></a>
         <a href="https://github.com/kalanakt/pdisk" target="_blank"><img alt="GitHub issues" src="https://img.shields.io/github/issues-raw/kalanakt/pdisk?color=8eecf5&logo=anaconda&logoColor=06d6a0"></a>
         <a href="https://github.com/kalanakt/pdisk" target="_blank"><img alt="GitHub" src="https://img.shields.io/github/license/kalanakt/pdisk?logo=adguard&logoColor=390099"></a>
-        <a href="https://github.com/kalanakt/pdisk" target="_blank"><img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/gramscript/gramscript?color=90e0ef&logoColor=ff4d6d"></a>
+        <a href="https://github.com/kalanakt/pdisk" target="_blank"><img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/kalanakt/pdisk?color=90e0ef&logoColor=ff4d6d"></a>
         <a href="https://github.com/kalanakt/pdisk"><img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/kalanakt/pdisk?logo=electron&logoColor=89fc00"></a>
         <a href="https://pypi.org/project/pdisk/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pdisk?logo=adguard&logoColor=89fc00"></a>
         <a href="https://github.com/kalanakt/pdisk"><img alt="GitHub" src="https://img.shields.io/github/license/kalanakt/pdisk?logo=adguard&logoColor=89fc00"></a>
         <a href="https://pypi.org/project/pdisk"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/pdisk?color=06d6a0&logo=adguard&logoColor=89fc00"></a>
         <a href="https://github.com/kalanakt/pdisk"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/kalanakt/pdisk?color=06d6a0&logo=adguard&logoColor=89fc00"></a>
         <a href="https://pypi.org/project/pdisk/"><img alt="PyPI - Format" src="https://img.shields.io/pypi/format/pdisk"></a>
         <a href="https://github.com/kalanakt/pdisk"><img alt="Sourcegraph for Repo Reference Count" src="https://img.shields.io/sourcegraph/rrc/https://github.com/kalanakt/pdisk"></a>
```

### Comparing `pdisk-1.0.1/pdisk/pdisk.py` & `pdisk-1.0.2/pdisk/pdisk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,96 @@
-#Copyright (c) 2023. kalanakt
+# Copyright (c) 2023. kalanakt
 
 import re
 import asyncio
 from typing import List
 import requests
 from urllib.parse import urlparse
 
 from .type import AccountInfo, AccountStat, ClonFile, DeletedFile, File, FileInfo, Folder, FolderList, UploadResponse
 
 
 class Pdisk:
-
     "Unofficial PDisk.pro API Wrapper By Kalanakt"
-    def __init__(self, api_key:str):
+
+    def __init__(self, api_key: str):
         self.__api_key = api_key
         self.__base_url = 'https://pdisk.pro/api'
 
         if not self.__api_key:
             raise Exception("API key not provided")
 
     ###################### ACCOUNT ######################
 
     async def account_info(self) -> AccountInfo:
         url = f"{self.__base_url}/account/info?key={self.__api_key}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
-            raise Exception(f"Failed to retrieve account info: {response.text}")
+            raise Exception(
+                f"Failed to retrieve account info: {response.text}")
         data = response.json()
         if data["status"] != 200:
             raise Exception(f"Failed to retrieve account info: {data['msg']}")
         result = data["result"]
         return AccountInfo(result["email"], float(result["balance"]), result["storage_used"])
-    
+
     async def account_stats(self) -> List[AccountStat]:
         url = f"{self.__base_url}/account/stats?key={self.__api_key}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
-            raise Exception(f"Failed to retrieve account stats: {response.text}")
+            raise Exception(
+                f"Failed to retrieve account stats: {response.text}")
         data = response.json()
         if data["status"] != 200:
             raise Exception(f"Failed to retrieve account stats: {data['msg']}")
         result = data["result"]
         return [AccountStat(int(r["downloads"]), int(r["refs"]), float(r["profit_total"])) for r in result]
-    
 
     ###################### UPLOAD ######################
 
     async def upload_server(self) -> str:
         url = f"{self.__base_url}/upload/server?key={self.__api_key}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
-            raise Exception(f"Failed to retrieve upload server: {response.text}")
+            raise Exception(
+                f"Failed to retrieve upload server: {response.text}")
         data = response.json()
         if data["status"] != 200:
             raise Exception(f"Failed to retrieve upload server: {data['msg']}")
         return data["result"]
 
     async def upload_file(self, file_path: str) -> List[UploadResponse]:
-        server_url = await self.get_upload_server()
+        server_url = await self.upload_server()
         files = {"file_0": open(file_path, "rb")}
         data = {"sess_id": "", "utype": "prem"}
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.post(server_url, files=files, data=data))
         if response.status_code != 200:
             raise Exception(f"Failed to upload file: {response.text}")
         data = response.json()
         return [UploadResponse(file["file_code"], file["file_status"]) for file in data]
-    
+
     async def upload_remote_file(self, url: str, folder_id: int) -> List[UploadResponse]:
         upload_url = f"{self.__base_url}/upload/url?key={self.__api_key}&url={url}&fld_id={folder_id}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(upload_url))
         if response.status_code != 200:
             raise Exception(f"Failed to upload remote file: {response.text}")
         data = response.json()
         return [UploadResponse(file["file_code"], None) for file in data]
-    
+
     async def check_upload_status(self, file_code: str) -> str:
         isLink = await self.is_pdisk_link(file_code)
         if isLink:
             file_code = await self.extract_file_code(file_code)
 
         url = f"{self.__base_url}/upload/url?key={self.__api_key}&file_code={file_code}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
             raise Exception(f"Failed to check upload status: {response.text}")
         data = response.json()
         return data[0]["file_code"]
-            
 
     ###################### FILE MANAGEMENT ######################
 
     async def file_info(self, file_code: str) -> List[FileInfo]:
         isLink = await self.is_pdisk_link(file_code)
         if isLink:
             file_code = await self.extract_file_code(file_code)
@@ -99,17 +100,18 @@
         if response.status_code != 200:
             raise Exception(f"Failed to retrieve file info: {response.text}")
         data = response.json()
         if data["status"] != 200:
             raise Exception(f"Failed to retrieve file info: {data['msg']}")
         result = data["result"]
         return [FileInfo(
-            f["filecode"], f["name"], f["status"], int(f["size"]), f["uploaded"], int(f["downloads"])
+            f["filecode"], f["name"], f["status"], int(
+                f["size"]), f["uploaded"], int(f["downloads"])
         ) for f in result]
-    
+
     async def get_file_list(self, page: int = 1, per_page: int = 20, fld_id: int = None, public: int = None, created: str = None, name: str = None) -> List[File]:
         url = f"{self.__base_url}/file/list?key={self.__api_key}&page={page}&per_page={per_page}"
         if fld_id is not None:
             url += f"&fld_id={fld_id}"
         if public is not None:
             url += f"&public={public}"
         if created is not None:
@@ -135,101 +137,102 @@
                 file_data["size"],
                 file_data["link"],
                 file_data["fld_id"],
                 file_data["uploaded"],
             )
             for file_data in data["result"]["files"]
         ]
-    
+
     async def rename_file(self, file_code: str, new_name: str) -> bool:
         isLink = await self.is_pdisk_link(file_code)
         if isLink:
             file_code = await self.extract_file_code(file_code)
 
         url = f"{self.__base_url}/file/rename?key={self.__api_key}&file_code={file_code}&name={new_name}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
             raise Exception(f"Failed to rename file: {response.text}")
         data = response.json()
         return data["result"]
-    
+
     async def clone_file(self, file_code: str) -> ClonFile:
         isLink = await self.is_pdisk_link(file_code)
         if isLink:
             file_code = await self.extract_file_code(file_code)
 
         url = f"{self.__base_url}/file/clone?key={self.__api_key}&file_code={file_code}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
             raise Exception(f"Failed to clone file: {response.text}")
         data = response.json()
         result = data["result"]
         return ClonFile(result["filecode"], result["url"])
-    
+
     async def set_file_folder(self, file_code: str, folder_id: int):
         isLink = await self.is_pdisk_link(file_code)
         if isLink:
             file_code = await self.extract_file_code(file_code)
 
         url = f"{self.__base_url}/file/set_folder?file_code={file_code}&fld_id={folder_id}&key={self.__api_key}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
             raise Exception(f"Failed to clone file: {response.text}")
-    
+
     async def deleted_files(self, file_code: str) -> List[DeletedFile]:
         isLink = await self.is_pdisk_link(file_code)
         if isLink:
             file_code = await self.extract_file_code(file_code)
 
         url = f"{self.__base_url}/files/deleted?key={self.__api_key}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
             raise Exception(f"Failed to clone file: {response.text}")
         data = response.json()
         result = data["result"]
-        return [DeletedFile(f["deleted_ago_sec"], f["deleted"], f["file_code"], f["name"] ) for f in result]
-
-    ###################### FOLDER MANAGEMENT ####################### 
+        return [DeletedFile(f["deleted_ago_sec"], f["deleted"], f["file_code"], f["name"]) for f in result]
 
+    ###################### FOLDER MANAGEMENT #######################
 
     async def get_folder_list(self, folder_id: int = 0) -> FolderList:
         url = f"{self.__base_url}/folder/list?key={self.__api_key}&fld_id={folder_id}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
             raise Exception(f"Failed to retrieve folder list: {response.text}")
         data = response.json()
         if data["status"] != 200:
             raise Exception(f"Failed to retrieve folder list: {data['msg']}")
         result = data["result"]
-        folders = [Folder(fld["fld_id"], fld["name"], fld["code"]) for fld in result["folders"]]
-        files = [File(f["file_id"], f["name"], f["file_code"], f["uploaded"], f["fld_id"]) for f in result["files"]]
-        return FolderList(folders, files) 
+        folders = [Folder(fld["fld_id"], fld["name"], fld["code"])
+                   for fld in result["folders"]]
+        files = [File(f["file_id"], f["name"], f["file_code"],
+                      f["uploaded"], f["fld_id"]) for f in result["files"]]
+        return FolderList(folders, files)
 
     async def create_folder(self, parent_id: int, name: str) -> int:
         url = f"{self.__base_url}/folder/create?key={self.__api_key}&parent_id={parent_id}&name={name}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
             raise Exception(f"Failed to create folder: {response.text}")
         data = response.json()
         if data["status"] != 200:
             raise Exception(f"Failed to create folder: {data['msg']}")
         result = data["result"]
         return int(result["fld_id"])
-    
+
     async def rename_folder(self, folder_id: int, new_name: str) -> bool:
         url = f"{self.__base_url}/folder/rename?fld_id={folder_id}&name={new_name}&key={self.__api_key}"
         response = await asyncio.get_event_loop().run_in_executor(None, lambda: requests.get(url))
         if response.status_code != 200:
             raise Exception(f"Failed to rename folder: {response.text}")
         data = response.json()
         if data["status"] != 200:
             raise Exception(f"Failed to rename folder: {data['msg']}")
         return data["result"] == "true"
 
     @staticmethod
-    async def is_pdisk_link(link:str) -> bool:
+    async def is_pdisk_link(link: str) -> bool:
         domain = urlparse(link).netloc
         return 'pdisk.pro' in domain
-    
+
     @staticmethod
-    async def extract_file_code(link:str) -> bool:
+    async def extract_file_code(link: str) -> bool:
         return link.replace('https://pdisk.pro/', '')
```

### Comparing `pdisk-1.0.1/pdisk/type.py` & `pdisk-1.0.2/pdisk/type.py`

 * *Files identical despite different names*

### Comparing `pdisk-1.0.1/pdisk.egg-info/PKG-INFO` & `pdisk-1.0.2/pdisk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdisk
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Unofficial Asynchronous Python version of pdisk API wrapper
 Home-page: https://github.com/kalanakt/pdisk
 Author: kalanakt
 Author-email: kalanakt@uvew.xyz
 License: MIT
 Keywords: python,pdisk,earn money 
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pdisk-1.0.1/setup.py` & `pdisk-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "package.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'An Unofficial Asynchronous Python version of pdisk API wrapper'
 
 # Setting up
 setup(
     name="pdisk",
     version=VERSION,
     author="kalanakt",
```

