# Comparing `tmp/cyberdrop-dl-4.2.13.tar.gz` & `tmp/cyberdrop-dl-4.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.13.tar", last modified: Sun May  7 05:17:26 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.14.tar", last modified: Sun May  7 06:04:39 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.13.tar` & `cyberdrop-dl-4.2.14.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.978136 cyberdrop-dl-4.2.13/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.978136 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.978136 cyberdrop-dl-4.2.13/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17721 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.978136 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:39.779318 cyberdrop-dl-4.2.14/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-07 06:04:39.779318 cyberdrop-dl-4.2.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:39.775318 cyberdrop-dl-4.2.14/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:39.775318 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:39.775318 cyberdrop-dl-4.2.14/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:39.779318 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:39.779318 cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17721 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:39.779318 cyberdrop-dl-4.2.14/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:04:39.775318 cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-07 06:04:39.000000 cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-07 06:04:39.000000 cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:04:39.000000 cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 06:04:39.000000 cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-07 06:04:39.000000 cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 06:04:39.000000 cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-07 06:04:39.779318 cyberdrop-dl-4.2.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 06:04:30.000000 cyberdrop-dl-4.2.14/setup.py
```

### Comparing `cyberdrop-dl-4.2.13/LICENSE` & `cyberdrop-dl-4.2.14/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/PKG-INFO` & `cyberdrop-dl-4.2.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.13
+Version: 4.2.14
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.13 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.14 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.13/README.md` & `cyberdrop-dl-4.2.14/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class CyberFileCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.load_files = URL('https://cyberfile.me/account/ajax/load_files')
         self.file_details = URL('https://cyberfile.me/account/ajax/file_details')
-        self.limiter = AsyncLimiter(25, 10)
+        self.limiter = AsyncLimiter(10, 10)
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for cyberfile scraping"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         domain_obj = DomainItem("cyberfile", {})
 
         download_links = []
```

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.14/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.13
+Version: 4.2.14
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.13 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.14 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.14/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.13/setup.cfg` & `cyberdrop-dl-4.2.14/setup.cfg`

 * *Files identical despite different names*

