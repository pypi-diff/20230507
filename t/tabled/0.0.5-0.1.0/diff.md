# Comparing `tmp/tabled-0.0.5.tar.gz` & `tmp/tabled-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tabled-0.0.5.tar", last modified: Tue Aug 31 18:00:24 2021, max compression
+gzip compressed data, was "tabled-0.1.0.tar", last modified: Sun May  7 12:55:40 2023, max compression
```

## Comparing `tabled-0.0.5.tar` & `tabled-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2021-08-31 18:00:24.801681 tabled-0.0.5/
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      487 2021-08-31 18:00:24.804221 tabled-0.0.5/PKG-INFO
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      140 2021-04-05 19:01:54.000000 tabled-0.0.5/README.md
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      571 2021-08-31 18:00:24.808563 tabled-0.0.5/setup.cfg
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)       91 2021-04-05 19:01:53.000000 tabled-0.0.5/setup.py
-drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2021-08-31 18:00:24.694946 tabled-0.0.5/tabled/
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)     2765 2021-08-31 00:28:37.000000 tabled-0.0.5/tabled/__init__.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)     4018 2021-08-31 00:30:04.000000 tabled-0.0.5/tabled/html.py
-drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2021-08-31 18:00:24.765807 tabled-0.0.5/tabled/tests/
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)        0 2021-04-05 19:05:15.000000 tabled-0.0.5/tabled/tests/__init__.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)     7371 2021-04-05 19:35:52.000000 tabled-0.0.5/tabled/tests/data.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)       32 2021-04-05 19:32:12.000000 tabled-0.0.5/tabled/tests/generate_data.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      508 2021-04-05 19:32:12.000000 tabled-0.0.5/tabled/tests/util.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)       14 2021-08-31 00:27:25.000000 tabled-0.0.5/tabled/util.py
-drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2021-08-31 18:00:24.723105 tabled-0.0.5/tabled.egg-info/
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      487 2021-08-31 18:00:23.000000 tabled-0.0.5/tabled.egg-info/PKG-INFO
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      352 2021-08-31 18:00:23.000000 tabled-0.0.5/tabled.egg-info/SOURCES.txt
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)        1 2021-08-31 18:00:23.000000 tabled-0.0.5/tabled.egg-info/dependency_links.txt
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)        1 2021-08-31 18:00:23.000000 tabled-0.0.5/tabled.egg-info/not-zip-safe
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)       16 2021-08-31 18:00:23.000000 tabled-0.0.5/tabled.egg-info/requires.txt
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)        7 2021-08-31 18:00:23.000000 tabled-0.0.5/tabled.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:55:39.993542 tabled-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 12:54:48.000000 tabled-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-07 12:55:39.993542 tabled-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 12:54:48.000000 tabled-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-07 12:55:39.993542 tabled-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-07 12:54:48.000000 tabled-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:55:39.993542 tabled-0.1.0/tabled/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-07 12:55:37.000000 tabled-0.1.0/tabled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-07 12:55:37.000000 tabled-0.1.0/tabled/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-07 12:55:37.000000 tabled-0.1.0/tabled/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:55:39.993542 tabled-0.1.0/tabled/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:54:48.000000 tabled-0.1.0/tabled/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-07 12:55:37.000000 tabled-0.1.0/tabled/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-07 12:55:37.000000 tabled-0.1.0/tabled/tests/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-07 12:54:48.000000 tabled-0.1.0/tabled/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-07 12:55:37.000000 tabled-0.1.0/tabled/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:55:39.993542 tabled-0.1.0/tabled.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-07 12:55:39.000000 tabled-0.1.0/tabled.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-07 12:55:39.000000 tabled-0.1.0/tabled.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:55:39.000000 tabled-0.1.0/tabled.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:55:39.000000 tabled-0.1.0/tabled.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 12:55:39.000000 tabled-0.1.0/tabled.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 12:55:39.000000 tabled-0.1.0/tabled.egg-info/top_level.txt
```

### Comparing `tabled-0.0.5/setup.cfg` & `tabled-0.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tabled
-version = 0.0.5
+version = 0.1.0
 url = https://github.com/i2mint/tabled
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = A (key-value) data-object-layer to get (pandas) tables from a variety of sources with ease
@@ -16,12 +16,13 @@
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
 	pandas
 	py2store
+	requests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tabled-0.0.5/tabled/html.py` & `tabled-0.1.0/tabled/html.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,94 @@
 """To work with html"""
 
 from typing import Callable, Union, Mapping
 import re
 import pandas as pd
 
 
-def url_to_html_func(kind="requests") -> Callable:
+def url_to_html_func(kind='requests') -> Callable:
     """Get a url_to_html function of a given kind."""
     url_to_html = None
-    if kind == "requests":
+    if kind == 'requests':
         import requests
 
         def url_to_html(url):
             r = requests.get(url)
             if r.status_code != 200:
                 print(
-                    f"An error occured. Returning the response object for you to analyze: {r}"
+                    f'An error occured. Returning the response object for you to analyze: {r}'
                 )
                 return r
             return r.content
 
-    elif kind == "chrome":
+    elif kind == 'chrome' or kind == 'selenium':
 
         from selenium import webdriver
         from time import sleep
 
         def url_to_html(url, wait=2):
             b = webdriver.Chrome()
             b.get(url)
             if isinstance(wait, (int, float)):
                 sleep(wait)
             html = b.page_source
             b.close()
             return html
 
     else:
-        raise ValueError(f"Unknown url_to_html value: {url_to_html}")
+        raise ValueError(f'Unknown url_to_html value: {url_to_html}')
     assert callable(url_to_html), "Couldn't make a url_to_html function"
 
     return url_to_html
 
 
-def get_tables_from_url(url, url_to_html: Union[Callable, str] = "requests"):
+get_tables_from_html = pd.read_html
+
+
+def get_tables_from_url(
+    url, *, url_to_html: Union[Callable, str] = 'requests', **tables_from_html_kwargs
+):
     """Get's a list of pandas dataframes from tables scraped from a url.
     Note that this will only work with static pages. If the html needs to be rendered dynamically,
     you'll have to get your needed html otherwise (like with selenium).
 
     >>> url = 'https://en.wikipedia.org/wiki/List_of_musical_instruments'
-    >>> tables = get_tables_from_url(url)
+    >>> tables = get_tables_from_url(url)  # doctest: +SKIP
 
     If you install selenium and download a chromedriver,
     you can even use your browser to render dynamic html.
     Say, to get updated coronavirus stats without a need to figure out the API
     (I mean, why have to figure out the language of an API, when someone already did that
     for you in their webpage!!):
 
     ```python
     url = 'https://www.worldometers.info/coronavirus/?utm_campaign=homeAdvegas1?'
-    tables = get_tables_from_url(url, url_to_html='chrome')
+    tables = get_tables_from_url(url, url_to_html='chrome')  # doctest: +SKIP
     ```
 
     To make selenium work:
     ```
         pip install selenium
         Download seleniumdriver here: https://chromedriver.chromium.org/
         Uzip and put in a place that's on you PATH (run command `echo $PATH` for a list of those places)
     ```
     """
     if not callable(url_to_html):
         url_to_html = url_to_html_func(url_to_html)
-    return pd.read_html(url_to_html(url))
+    try:
+        return get_tables_from_html(url_to_html(url), **tables_from_html_kwargs)
+    except ValueError as e:
+        if len(e.args) > 0:
+            msg, *_ = e.args
+            if 'No tables found' in msg:
+                return []
+        raise
 
 
-HTML_TEMPLATE1 = """
+HTML_TEMPLATE1 = '''
 <html>
 <head>
 <style>
   h2 {
     text-align: center;
     font-family: Helvetica, Arial, sans-serif;
   }
@@ -99,34 +111,34 @@
   }
   .wide {
     width: 90%; 
   }
 </style>
 </head>
 <body>
-"""
+'''
 
-HTML_TEMPLATE2 = """
+HTML_TEMPLATE2 = '''
 </body>
 </html>
-"""
+'''
 
 
 def df_to_html(df, title=None):
-    ht = ""
+    ht = ''
     if title is not None:
-        ht += f"<h2> {title} </h2>\n"
-    ht += df.to_html(classes="wide", escape=False)
+        ht += f'<h2> {title} </h2>\n'
+    ht += df.to_html(classes='wide', escape=False)
     return ht
 
 
-def df_store_to_html(df_store, sep="\n<br>\n"):
-    ht = ""
+def df_store_to_html(df_store, sep='\n<br>\n'):
+    ht = ''
     for k, df in df_store.items():
-        title = re.match(r"[^\d]+", k).group(0)
+        title = re.match(r'[^\d]+', k).group(0)
         ht += df_to_html(df, title)
         ht += sep
     return ht
 
 
 def dfs_to_html_pretty(dfs, title=None):
     """
```

