# Comparing `tmp/redfin-scraper-0.1.5.tar.gz` & `tmp/redfin-scraper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfin-scraper-0.1.5.tar", last modified: Thu Apr  6 15:28:16 2023, max compression
+gzip compressed data, was "redfin-scraper-0.1.6.tar", last modified: Sun May  7 02:04:44 2023, max compression
```

## Comparing `redfin-scraper-0.1.5.tar` & `redfin-scraper-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 15:28:16.463302 redfin-scraper-0.1.5/
--rw-rw-rw-   0        0        0     1087 2023-03-18 00:15:21.000000 redfin-scraper-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     4020 2023-04-06 15:28:16.458304 redfin-scraper-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2154 2023-04-04 15:15:03.000000 redfin-scraper-0.1.5/README.md
--rw-rw-rw-   0        0        0      904 2023-04-06 15:25:40.000000 redfin-scraper-0.1.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-06 15:28:16.417199 redfin-scraper-0.1.5/redfin_scraper/
--rw-rw-rw-   0        0        0      120 2023-04-06 15:25:43.000000 redfin-scraper-0.1.5/redfin_scraper/__init__.py
--rw-rw-rw-   0        0        0      325 2023-03-18 17:58:54.000000 redfin-scraper-0.1.5/redfin_scraper/config.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:28:16.449300 redfin-scraper-0.1.5/redfin_scraper/core/
--rw-rw-rw-   0        0        0        0 2023-03-11 03:00:34.000000 redfin-scraper-0.1.5/redfin_scraper/core/__init__.py
--rw-rw-rw-   0        0        0    11730 2023-04-06 15:27:53.000000 redfin-scraper-0.1.5/redfin_scraper/core/redfin_scraper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:28:16.454300 redfin-scraper-0.1.5/redfin_scraper/resources/
--rw-rw-rw-   0        0        0        0 2023-02-25 20:03:01.000000 redfin-scraper-0.1.5/redfin_scraper/resources/__init__.py
--rw-rw-rw-   0        0        0     1116 2023-03-11 03:00:17.000000 redfin-scraper-0.1.5/redfin_scraper/resources/json_tools.py
--rw-rw-rw-   0        0        0     2462 2023-04-04 15:04:28.000000 redfin-scraper-0.1.5/redfin_scraper/resources/logging.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:28:16.445088 redfin-scraper-0.1.5/redfin_scraper.egg-info/
--rw-rw-rw-   0        0        0     4020 2023-04-06 15:28:16.000000 redfin-scraper-0.1.5/redfin_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-06 15:28:16.000000 redfin-scraper-0.1.5/redfin_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 15:28:16.000000 redfin-scraper-0.1.5/redfin_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-06 15:28:16.000000 redfin-scraper-0.1.5/redfin_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-06 15:28:16.000000 redfin-scraper-0.1.5/redfin_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 15:28:16.464301 redfin-scraper-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.696170 redfin-scraper-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-03-18 00:15:21.000000 redfin-scraper-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     4020 2023-05-07 02:04:44.693164 redfin-scraper-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2154 2023-04-04 15:15:03.000000 redfin-scraper-0.1.6/README.md
+-rw-rw-rw-   0        0        0      904 2023-05-07 02:02:00.000000 redfin-scraper-0.1.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.668989 redfin-scraper-0.1.6/redfin_scraper/
+-rw-rw-rw-   0        0        0      120 2023-05-07 02:02:53.000000 redfin-scraper-0.1.6/redfin_scraper/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-03-18 17:58:54.000000 redfin-scraper-0.1.6/redfin_scraper/config.py
+drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.688654 redfin-scraper-0.1.6/redfin_scraper/core/
+-rw-rw-rw-   0        0        0        0 2023-03-11 03:00:34.000000 redfin-scraper-0.1.6/redfin_scraper/core/__init__.py
+-rw-rw-rw-   0        0        0    11388 2023-05-07 01:57:33.000000 redfin-scraper-0.1.6/redfin_scraper/core/redfin_scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.692162 redfin-scraper-0.1.6/redfin_scraper/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-25 20:03:01.000000 redfin-scraper-0.1.6/redfin_scraper/resources/__init__.py
+-rw-rw-rw-   0        0        0     1116 2023-03-11 03:00:17.000000 redfin-scraper-0.1.6/redfin_scraper/resources/json_tools.py
+-rw-rw-rw-   0        0        0     2462 2023-04-04 15:04:28.000000 redfin-scraper-0.1.6/redfin_scraper/resources/logging.py
+drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.686656 redfin-scraper-0.1.6/redfin_scraper.egg-info/
+-rw-rw-rw-   0        0        0     4020 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 02:04:44.696170 redfin-scraper-0.1.6/setup.cfg
```

### Comparing `redfin-scraper-0.1.5/LICENSE.txt` & `redfin-scraper-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.1.5/PKG-INFO` & `redfin-scraper-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfin-scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library used to scrape data from Redfin.com using the unofficial Stringray API.
 Author-email: Ryan Sherby <ryan.m.sherby@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ryan Sherby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `redfin-scraper-0.1.5/README.md` & `redfin-scraper-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.1.5/pyproject.toml` & `redfin-scraper-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "redfin-scraper"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Python library used to scrape data from Redfin.com using the unofficial Stringray API."
 readme = "README.md"
 authors = [{ name = "Ryan Sherby", email = "ryan.m.sherby@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `redfin-scraper-0.1.5/redfin_scraper/core/redfin_scraper.py` & `redfin-scraper-0.1.6/redfin_scraper/core/redfin_scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import re
 import json
 import datetime as dt
 import time
 import itertools
 import multiprocessing
 import concurrent.futures
+import io
+import csv
 
 import requests
 from bs4 import BeautifulSoup
 import numpy as np
 import pandas as pd
-import pyparsing as pp
 
 import redfin_scraper.config as rsc
 
 import redfin_scraper.resources.logging as rsrl
 import redfin_scraper.resources.json_tools as rsrj
 
 
@@ -228,26 +229,14 @@
         
         return user_agent
 
 
 
 
 
-    def _parse_listed_csv(self,listed_csv:list[str]) -> list[list]:
-        csv_contents_list=[]
-        
-        for li in listed_csv:
-            csv_contents_list.append(pp.common.comma_separated_list.parseString(li).asList())
-
-        return csv_contents_list
-
-
-
-
-
     def _sanitize_city_states(self,city_states):
 
         if city_states==None:
             return None
 
         cleaned_city_states=[]
 
@@ -407,31 +396,27 @@
 
 
     def _get_API_response(self,url):
         header=self._randomized_UA()
 
         req=requests.get(url,headers=header)
 
-        req_text=req.text
-
-        listed_req_text=req_text.splitlines()
-
-        parsed_response=self._parse_listed_csv(listed_req_text)
-
-        return parsed_response
+        return req
     
     
 
 
 
-    def _set_dataframe(self,api_responses:list[list[list]]):
+    def _set_dataframe(self,api_responses:list[requests.Response]):
         df_list=[]
 
         for response in api_responses:
-            df=pd.DataFrame(data=response[1:],columns=response[0])
+            csv_stream = io.StringIO(response.content.decode('utf-8'))
+            reader = csv.DictReader(csv_stream)
+            df=pd.DataFrame(reader)
             df_list.append(df)
 
         return df_list
```

### Comparing `redfin-scraper-0.1.5/redfin_scraper/resources/json_tools.py` & `redfin-scraper-0.1.6/redfin_scraper/resources/json_tools.py`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.1.5/redfin_scraper/resources/logging.py` & `redfin-scraper-0.1.6/redfin_scraper/resources/logging.py`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.1.5/redfin_scraper.egg-info/PKG-INFO` & `redfin-scraper-0.1.6/redfin_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfin-scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library used to scrape data from Redfin.com using the unofficial Stringray API.
 Author-email: Ryan Sherby <ryan.m.sherby@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ryan Sherby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

