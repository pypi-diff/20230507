# Comparing `tmp/cyberdrop-dl-4.2.12.tar.gz` & `tmp/cyberdrop-dl-4.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.12.tar", last modified: Fri May  5 19:58:42 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.13.tar", last modified: Sun May  7 05:17:26 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.12.tar` & `cyberdrop-dl-4.2.13.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.779605 cyberdrop-dl-4.2.12/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.783605 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.783605 cyberdrop-dl-4.2.12/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.779605 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.978136 cyberdrop-dl-4.2.13/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.978136 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.978136 cyberdrop-dl-4.2.13/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17721 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:17:26.978136 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 05:17:26.000000 cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-07 05:17:26.982137 cyberdrop-dl-4.2.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:17:17.000000 cyberdrop-dl-4.2.13/setup.py
```

### Comparing `cyberdrop-dl-4.2.12/LICENSE` & `cyberdrop-dl-4.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/PKG-INFO` & `cyberdrop-dl-4.2.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.12
+Version: 4.2.13
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.12 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.13 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.12/README.md` & `cyberdrop-dl-4.2.13/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import time
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Callable, Optional, Coroutine, Any, Tuple, Dict
 
 import aiofiles
 import aiohttp
 import certifi
+from aiolimiter import AsyncLimiter
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 from yarl import URL
 
 from ..base_functions.base_functions import logger
 from ..base_functions.error_classes import DownloadFailure, InvalidContentTypeFailure
 from ..downloader.downloader_utils import CustomHTTPStatus
 from ..downloader.progress_definitions import ProgressMaster, adjust_title
-from .rate_limiting import AsyncRateLimiter
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from rich.progress import TaskID
 
     from ..base_functions.data_classes import MediaItem
@@ -53,15 +53,15 @@
         self.cookies = aiohttp.CookieJar(quote_cookie=False)
 
 
 class ScrapeSession:
     """AIOHTTP operations for scraping"""
     def __init__(self, client: Client) -> None:
         self.client = client
-        self.rate_limiter = AsyncRateLimiter(self.client.ratelimit)
+        self.rate_limiter = AsyncLimiter(self.client.ratelimit, 1)
         self.headers = {"user-agent": client.user_agent}
         self.timeouts = aiohttp.ClientTimeout(total=self.client.connect_timeout + 45,
                                               connect=self.client.connect_timeout, sock_read=45)
         self.client_session = aiohttp.ClientSession(headers=self.headers, raise_for_status=True,
                                                     cookie_jar=self.client.cookies, timeout=self.timeouts)
 
     @scrape_limit
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING
 
+from aiolimiter import AsyncLimiter
 from yarl import URL
 
 from ..base_functions.base_functions import (
     FILE_FORMATS,
     get_filename_and_ext,
     log,
     logger,
@@ -21,14 +22,15 @@
 
 
 class BunkrCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper, remove_bunkr_id: bool):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.remove_bunkr_id = remove_bunkr_id
+        self.limiter = AsyncLimiter(20, 1)
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Scraper for Bunkr"""
         album_obj = AlbumItem("Loose Bunkr Files", [])
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if "v" in url.parts or "d" in url.parts:
@@ -95,15 +97,16 @@
     async def get_file(self, session: ScrapeSession, url: URL):
         """Gets the media item from the supplied url"""
 
         ### Temp Fix ###
         url = url.with_host("bunkr.la")
 
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             head = soup.select_one("head")
             scripts = head.select('script[type="text/javascript"]')
             link = None
 
             for script in scripts:
                 if script.text and "link.href" in script.text:
                     link = script.text.split('link.href = "')[-1].split('";')[0]
@@ -132,15 +135,16 @@
         """Iterates through an album and creates the media items"""
 
         ### Temp Fix ###
         url = url.with_host("bunkr.la")
 
         album = AlbumItem(url.name, [])
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             title = soup.select_one('h1[class="text-[24px] font-bold text-dark dark:text-white"]')
             for elem in title.find_all("span"):
                 elem.decompose()
             title = await make_title_safe(title.get_text())
             await album.set_new_title(title)
             for file in soup.select('a[class*="grid-images_box-link"]'):
                 link = file.get("href")
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Union, List
 
+from aiolimiter import AsyncLimiter
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import CascadeItem
 
 if TYPE_CHECKING:
@@ -36,14 +37,15 @@
 class CoomenoCrawler:
     def __init__(self, *, include_id=False, scraping_mapper, separate_posts=False, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.scraping_mapper = scraping_mapper
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
+        self.limiter = AsyncLimiter(15, 1)
 
     async def fetch(self, session: ScrapeSession, url: URL):
         """Director for Coomer/Kemono scraping"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
         title = None
         try:
@@ -91,15 +93,16 @@
         if tasks:
             await asyncio.wait(tasks)
 
     async def parse_profile(self, session: ScrapeSession, url: URL, spec: ParseSpec, cascade: CascadeItem) -> str:
         """Parses profiles with supplied selectors"""
         title = ""
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             title = await make_title_safe(soup.select_one("span[itemprop=name]").get_text())
             title = f"{title} ({url.host})"
 
             posts = []
             assert url.host is not None
             for posts_selector in spec.posts_selectors:
                 posts += soup.select(posts_selector)
@@ -124,15 +127,16 @@
 
     async def parse_post(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem,
                          title: str = "") -> str:
         """Parses posts with supplied selectors"""
         try:
             text = await self.SQL_Helper.get_blob(url)
             if not text:
-                text = await session.get_text(url)
+                async with self.limiter:
+                    text = await session.get_text(url)
                 assert text is not None
                 await self.SQL_Helper.insert_blob(text, url)
             soup = BeautifulSoup(text, 'html.parser')
 
             if self.separate_posts:
                 time_tag = soup.select_one("time[class*=timestamp]")
                 post_tag = soup.select_one("h1[class=post__title]")
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import contextlib
 from typing import TYPE_CHECKING, Optional, Tuple, List
 
+from aiolimiter import AsyncLimiter
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
 
@@ -17,14 +18,15 @@
 
 class CyberFileCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.load_files = URL('https://cyberfile.me/account/ajax/load_files')
         self.file_details = URL('https://cyberfile.me/account/ajax/file_details')
+        self.limiter = AsyncLimiter(25, 10)
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for cyberfile scraping"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         domain_obj = DomainItem("cyberfile", {})
 
         download_links = []
@@ -50,15 +52,16 @@
         await self.SQL_Helper.insert_domain("cyberfile", url, domain_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return domain_obj
 
     async def get_folder_id(self, session: ScrapeSession, url: URL) -> int:
         """Gets the internal ID for a folder"""
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             script_func = soup.select_one('div[class="page-container horizontal-menu with-sidebar fit-logo-with-sidebar logged-out clear-adblock"] script').text
             script_func = script_func.split('loadImages(')[-1]
             script_func = script_func.split(';')[0]
             nodeId = int(script_func.split(',')[1].replace("'", ""))
             return nodeId
 
         except Exception as e:
@@ -69,15 +72,16 @@
 
     async def get_folder_content(self, session: ScrapeSession, url: URL, nodeId: int, page: int, title=None):
         """Gets the content id's encased in a folder"""
         data = {"pageType": "folder", "nodeId": nodeId, "pageStart": page, "perPage": 0, "filterOrderBy": ""}
         nodes = []
         contents = []
         try:
-            content = await session.post(self.load_files, data)
+            async with self.limiter:
+                content = await session.post(self.load_files, data)
             text = content['html']
             original_title = title
             if title:
                 title = title + "/" + await make_title_safe(content['page_title'])
             else:
                 title = content['page_title']
                 title = await make_title_safe(title)
@@ -115,15 +119,16 @@
             log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
 
     async def get_single_contentId(self, session: ScrapeSession, url: URL) -> int:
         """Gets an individual content id"""
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             script_funcs = soup.select('script')
             for script in script_funcs:
                 script_text = script.text
                 if script_text and "showFileInformation" in script_text:
                     part_a = script_text.split("showFileInformation(")
                     part_a = [x for x in part_a if x[0].isdigit()][0]
                     part_b = part_a.split(");")[0]
@@ -137,22 +142,24 @@
             logger.debug(e)
             return 0
 
     async def get_shared_ids_and_content(self, session: ScrapeSession, url: URL, page: int) -> Tuple[List, List]:
         """Gets folder id's and content id's from shared links"""
         try:
             # Initial page load to tell server, this is what we want.
-            await session.get_no_resp(url, {'referer': str(url), "user-agent": session.client.user_agent})
+            async with self.limiter:
+                await session.get_no_resp(url, {'referer': str(url), "user-agent": session.client.user_agent})
 
             # get the content listings
             data = {"pageType": "nonaccountshared", "nodeId": '', "pageStart": page, "perPage": 0, "filterOrderBy": ""}
             nodes = []
             contents = []
 
-            content = await session.post(self.load_files, data)
+            async with self.limiter:
+                content = await session.post(self.load_files, data)
             text = content['html']
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
             page_tag = soup.select_one('input[id=rspTotalPages]')
             assert page_tag is not None
             page_str = page_tag.get('value')
             assert isinstance(page_str, str)
             total_pages = int()
@@ -189,39 +196,41 @@
     async def get_shared_content(self, session, url: URL, nodeId: int, page: int, title=None) -> List:
         """Gets content from shared folders"""
         try:
             nodes = []
             contents = []
             data = {"pageType": "nonaccountshared", "nodeId": nodeId, "pageStart": page, "perPage": 0, "filterOrderBy": ""}
 
-            content = await session.post(self.load_files, data)
+            async with self.limiter:
+                content = await session.post(self.load_files, data)
             text = content['html']
-
             title = title if title else content['page_title']
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
 
             page_ref = soup.select("a[onclick*=loadImages]")[-1].get('onclick')
             assert isinstance(page_ref, str)
             total_pages = int(page_ref.split(',')[2])
 
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
                 with contextlib.suppress(TypeError, AttributeError):
                     filename = listing.select_one('span[class=filename]')
-                    assert filename is not None
-                    temp_title = title + '/' + await make_title_safe(filename.text)
+                    if filename:
+                        temp_title = title + '/' + await make_title_safe(filename.text)
 
                     folder_id = listing.get('folderid')
-                    assert isinstance(folder_id, str)
-                    nodes.append((temp_title, int(folder_id)))
+                    if folder_id:
+                        assert isinstance(folder_id, str)
+                        nodes.append((temp_title, int(folder_id)))
 
                 with contextlib.suppress(TypeError):
                     file_id = listing.get('fileid')
-                    assert isinstance(file_id, str)
-                    contents.append((title, int(file_id)))
+                    if file_id:
+                        assert isinstance(file_id, str)
+                        contents.append((title, int(file_id)))
 
             if page < total_pages:
                 contents.extend(await self.get_shared_content(session, url, nodeId, page + 1, title))
             for title, node in nodes:
                 contents.extend(await self.get_shared_content(session, url, node, 1, title))
             return contents
 
@@ -233,15 +242,16 @@
 
     async def get_download_links(self, session: ScrapeSession, url: URL, contentIds: List) -> List:
         """Obtains download links from content ids"""
         download_links = []
         try:
             for title, contentId in contentIds:
                 data = {"u": contentId}
-                content = await session.post(self.file_details, data)
+                async with self.limiter:
+                    content = await session.post(self.file_details, data)
                 text = content['html']
                 soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
                 menu = soup.select_one('ul[class="dropdown-menu dropdown-info account-dropdown-resize-menu"] li a')
                 button = soup.select_one('div[class="btn-group responsiveMobileMargin"] button')
 
                 if menu:
                     html_download_text = menu.get("onclick")
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import http
 from typing import TYPE_CHECKING, Union, List, Dict
 
+from aiolimiter import AsyncLimiter
 from yarl import URL
 
 from ..base_functions.base_functions import log, logger, make_title_safe, get_filename_and_ext
 from ..base_functions.data_classes import DomainItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
@@ -14,14 +15,15 @@
     from ..client.client import ScrapeSession
 
 
 class GoFileCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
+        self.limiter = AsyncLimiter(1, 1)
 
         self.api_address = URL("https://api.gofile.io")
         self.token = ""
 
     async def get_token(self, session: ScrapeSession, api_token=None):
         """Creates an anon gofile account to use."""
         if self.token:
@@ -29,15 +31,16 @@
 
         if api_token:
             self.token = api_token
             await self.set_cookie(session)
             return
 
         try:
-            json_obj = await session.get_json(self.api_address / "createAccount")
+            async with self.limiter:
+                json_obj = await session.get_json(self.api_address / "createAccount")
             if json_obj["status"] == "ok":
                 self.token = json_obj["data"]["token"]
                 await self.set_cookie(session)
             else:
                 raise
         except Exception as e:
             logger.debug("Error encountered while getting GoFile token", exc_info=True)
@@ -75,15 +78,18 @@
         """Gets links from the given url, creates media_items"""
         results: List[List] = []
         params = {
             "token": self.token,
             "contentId": content_id,
             "websiteToken": "12345",
         }
-        content = await session.get_json(self.api_address / "getContent", params)
+
+        async with self.limiter:
+            content = await session.get_json(self.api_address / "getContent", params)
+
         if content["status"] != "ok":
             logger.debug("Error encountered while handling %s", url)
             log(f"Error: {url}", quiet=self.quiet, style="red")
             return results
 
         content = content['data']
         if title:
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import re
 from typing import TYPE_CHECKING
 
+from aiolimiter import AsyncLimiter
 from yarl import URL
 
 from ..base_functions.base_functions import (
     check_direct,
     create_media_item,
     log,
     logger,
@@ -22,14 +23,15 @@
 
 
 class ShareXCrawler:
     def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
+        self.limiter = AsyncLimiter(20, 1)
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for ShareX scraper"""
         assert url.host is not None
         domain_obj = DomainItem(url.host.lower(), {})
 
         log(f"Starting: {url}", quiet=self.quiet, style="green")
@@ -55,15 +57,16 @@
     async def jpg_fish_from_church(self, url: URL) -> URL:
         pattern2 = r"simp([1-5])\.jpg\.church/"
         return URL(re.sub(pattern2, r'simp\1.jpg.fish/', str(url)))
 
     async def get_albums(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for Albums"""
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             albums = soup.select("a[class='image-container --media']")
             for album in albums:
                 album_url = URL(album.get('href'))
                 await self.parse(session=session, url=album_url, domain_obj=domain_obj)
 
             next_page = soup.select_one('li.pagination-next a')
             if not next_page:
@@ -79,45 +82,48 @@
             log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_singular(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for singular files"""
         await asyncio.sleep(1)
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             link = URL(soup.select_one("input[id=embed-code-2]").get('value'))
             link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
             link = await self.jpg_fish_from_church(link)
 
             media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
             log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_sub_album_links(self, session: ScrapeSession, url: URL, og_title: str,
                                   domain_obj: DomainItem) -> None:
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             albums = soup.select("div[class=pad-content-listing] div")
             for album in albums:
                 album_url = album.get('data-url-short')
                 if album_url is not None:
                     album_url = URL(album_url)
                     await self.parse(session=session, url=album_url, og_title=og_title, domain_obj=domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
             log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def parse_profile(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for profiles"""
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             title = soup.select_one("div[class=header] h1 strong").get_text()
             if title is None:
                 title = url.name
             elif self.include_id:
                 titlep2 = url.name
                 title = title + " - " + titlep2
             title = await make_title_safe(title.replace(r"\n", "").strip())
@@ -127,15 +133,16 @@
             logger.debug("Error encountered while handling %s", url, exc_info=True)
             log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_list_links(self, session: ScrapeSession, url: URL, title: str, domain_obj: DomainItem) -> None:
         """Gets final links and adds to domain_obj"""
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
             assert url.host is not None
             if 'jpg.fish' in url.host or 'jpg.church' in url.host:
                 links = soup.select("a[href*=img] img")
             else:
                 links = soup.select("a[href*=image] img")
             for link in links:
                 link = URL(link.get('src'))
@@ -160,15 +167,16 @@
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
             log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def parse(self, *, session: ScrapeSession, url: URL, og_title=None, domain_obj: DomainItem) -> None:
         try:
-            soup = await session.get_BS4(url)
+            async with self.limiter:
+                soup = await session.get_BS4(url)
 
             title = soup.select_one("a[data-text=album-name]").get_text()
             if title is None:
                 title = url.name
             elif self.include_id:
                 titlep2 = url.name
                 title = title + " - " + titlep2
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 import asyncio
 import re
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Dict, List, Tuple
 
 import aiofiles
-import bs4
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import (
     get_filename_and_ext,
     log,
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import CascadeItem, MediaItem
 from ..base_functions.error_classes import FailedLoginFailure, NoExtensionFailure
 
 if TYPE_CHECKING:
+    import bs4
+
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 @dataclass
 class ParseSpec:
     """Class for specific selectors of supported domains"""
@@ -259,23 +260,19 @@
         soup = await session.get_BS4(url)
 
         assert url.host is not None
         domain = URL("https://" + url.host)
         post_num_str = ""
         content_links = []
 
-        title_block = soup.select_one(spec.title_block_tag)
-        for elem in title_block.find_all(spec.title_clutter_tag):
-            elem.decompose()
-
-        if title:
-            pass
-        else:
-            title = title_block.text
-            title = await make_title_safe(title.replace("\n", "").strip())
+        if not title:
+            title_block = soup.select_one(spec.title_block_tag)
+            for elem in title_block.find_all(spec.title_clutter_tag):
+                elem.decompose()
+            title = await make_title_safe(title_block.text.replace("\n", "").strip())
 
         posts = soup.select(spec.posts_block_tag)
 
         for post in posts:
             post_num_str = post.select_one(spec.posts_number_tag).get(spec.posts_number_attribute).split('/')[-1]
             post_num_int = int(post_num_str.split('post-')[-1])
             if post_number > post_num_int:
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,17 +68,16 @@
     async def wrapper(self, *args, **kwargs):
         while True:
             try:
                 return await f(self, *args, **kwargs)
             except DownloadFailure as e:
                 media = args[1]
                 url_path = args[2]
-                if not self.disable_attempt_limit and self.current_attempt[url_path] >= self.allowed_attempts - 1:
-                    await self.output_failed(media, e)
+                if not self.can_retry(url_path):
                     logger.debug('Skipping %s...', media.url, exc_info=True)
-                    self.files.add_failed()
+                    await self.handle_failed(media, e)
                     return None
                 logger.debug(e.message)
                 logger.debug(f'Retrying ({self.current_attempt[url_path]}) {media.url}...')
                 self.current_attempt[url_path] += 1
 
     return wrapper
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import itertools
 import logging
 from http import HTTPStatus
-from pathlib import Path
 from random import gauss
-from typing import TYPE_CHECKING, Dict, Any, Tuple, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Tuple
 
 import aiofiles
 import aiohttp.client_exceptions
 from rich.live import Live
 
 from cyberdrop_dl.base_functions.base_functions import (
     clear,
@@ -36,18 +35,21 @@
     basic_auth,
     check_free_space,
     get_threads_number,
     is_4xx_client_error,
     retry,
 )
 from .progress_definitions import (
-    ProgressMaster, OverallFileProgress
+    OverallFileProgress,
+    ProgressMaster,
 )
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from rich.progress import TaskID
 
 
 class CDLHelper:
     def __init__(self, args: Dict, client: Client, files: OverallFileProgress, SQL_Helper: SQLHelper):
         self.args = args
 
@@ -100,18 +102,15 @@
         max_workers = get_threads_number(CDL_Helper.args, domain)
         self._semaphore = asyncio.Semaphore(max_workers)
         self.current_attempt: Dict[str, int] = {}
 
         self.download_session = DownloadSession(CDL_Helper.client)
 
         self.CDL_Helper = CDL_Helper
-        self.files = CDL_Helper.files
         self.Progress_Master = Progress_Master
-        self.disable_attempt_limit = CDL_Helper.disable_attempt_limit
-        self.allowed_attempts = CDL_Helper.allowed_attempts
 
     async def download(self, album: str, media: MediaItem, url_path: str, album_task: TaskID) -> None:
         async with self._semaphore:
             await self.download_file(album, media, url_path, album_task)
 
     @retry
     async def download_file(self, album: str, media: MediaItem, url_path: str, album_task: TaskID) -> None:
@@ -207,38 +206,40 @@
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", e.code)
                     log(f"Failed Download: {media.filename}", quiet=True)
-                    self.CDL_Helper.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
-                    await self.output_failed(media, e)
+                    await self.handle_failed(media, e)
                     return
 
                 if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == HTTPStatus.BAD_GATEWAY \
                         or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
                     if hasattr(e, "message"):
                         if not e.message:
                             e.message = "Web server is down"
                         logging.debug(f"\n{media.url} ({e.message})")
                     log(f"Failed Download: {media.filename}", quiet=True)
-                    self.CDL_Helper.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
-                    await self.output_failed(media, e)
+                    await self.handle_failed(media, e)
                     return
 
                 logger.debug("Error status code: %s", e.code)
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
-    async def output_failed(self, media: MediaItem, e: Any) -> None:
+    def can_retry(self, url_path: str) -> bool:
+        return self.CDL_Helper.disable_attempt_limit or self.current_attempt[url_path] < self.CDL_Helper.allowed_attempts - 1
+
+    async def handle_failed(self, media: MediaItem, e: Any) -> None:
+        self.CDL_Helper.files.add_failed()
         if self.CDL_Helper.errored_output:
             async with aiofiles.open(self.CDL_Helper.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
 
     async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
                                 url_path: str, original_filename: str, current_throttle: float):
         """Complicated checker for if a file already exists, and was already downloaded"""
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,35 +206,37 @@
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", e.code)
                     log(f"Failed Download: {media.filename}", quiet=True)
-                    self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
-                    await self.output_failed(media, e)
+                    await self.handle_failed(media, e)
                     return
                 if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
                     if hasattr(e, "message"):
                         if not e.message:
                             e.message = "Web server is down"
                         logging.debug(f"\n{media.url} ({e.message})")
                     log(f"Failed Download: {media.filename}", quiet=True)
-                    self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
-                    await self.output_failed(media, e)
+                    await self.handle_failed(media, e)
                     return
                 logger.debug("Error status code: %s", e.code)
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
-    async def output_failed(self, media: MediaItem, e: Any) -> None:
+    def can_retry(self, url_path: str) -> bool:
+        return self.disable_attempt_limit or self.current_attempt[url_path] < self.allowed_attempts - 1
+
+    async def handle_failed(self, media: MediaItem, e: Any) -> None:
+        self.files.add_failed()
         if self.errored_output:
             async with aiofiles.open(self.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
 
     async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
                                 url_path: str, original_filename: str,
                                 current_throttle: float) -> tuple[Path, Path, bool]:
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.13/cyberdrop_dl/scraper/Scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Optional, Dict
 
 import aiofiles
+from aiolimiter import AsyncLimiter
 from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.data_classes import AlbumItem, CascadeItem, DomainItem, ForumItem, SkipData
 from cyberdrop_dl.client.client import Client, ScrapeSession
-from cyberdrop_dl.client.rate_limiting import AsyncRateLimiter
 from cyberdrop_dl.crawlers.Anonfiles_Spider import AnonfilesCrawler
 from cyberdrop_dl.crawlers.Bunkr_Spider import BunkrCrawler
 from cyberdrop_dl.crawlers.Coomeno_Spider import CoomenoCrawler
 from cyberdrop_dl.crawlers.CyberFile_Spider import CyberFileCrawler
 from cyberdrop_dl.crawlers.Cyberdrop_Spider import CyberdropCrawler
 from cyberdrop_dl.crawlers.EHentai_Spider import EHentaiCrawler
 from cyberdrop_dl.crawlers.Erome_Spider import EromeCrawler
@@ -75,26 +75,14 @@
 
         self.include_id = args['Runtime']['include_id']
         self.remove_bunkr_id = args['Runtime']['remove_bunkr_identifier']
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.quiet = quiet
         self.jdownloader = JDownloader(args['JDownloader'], quiet)
 
-        self.bunkr_limiter = AsyncRateLimiter(max_calls=1, period=1)
-        self.coomer_limiter = AsyncRateLimiter(8)
-        self.gofile_limiter = AsyncRateLimiter(max_calls=1, period=3)
-        self.jpgfish_limiter = AsyncRateLimiter(10)
-        self.kemono_limiter = AsyncRateLimiter(8)
-
-        self.bunkr_semaphore = asyncio.Semaphore(2)
-        self.coomer_semaphore = asyncio.Semaphore(1)
-        self.cyberfile_semaphore = asyncio.Semaphore(2)
-        self.gofile_semaphore = asyncio.Semaphore(1)
-        self.jpgfish_semaphore = asyncio.Semaphore(5)
-        self.kemono_semaphore = asyncio.Semaphore(1)
         self.nudostar_semaphore = asyncio.Semaphore(1)
         self.simpcity_semaphore = asyncio.Semaphore(1)
         self.socialmediagirls_semaphore = asyncio.Semaphore(1)
         self.xbunker_semaphore = asyncio.Semaphore(1)
 
         self.mapping = {"anonfiles": self.Anonfiles, "bayfiles": self.Anonfiles, "xbunkr": self.XBunkr,
                         "bunkr": self.Bunkr, "cyberdrop": self.Cyberdrop, "cyberfile": self.CyberFile,
@@ -140,17 +128,16 @@
         await anonfiles_session.exit_handler()
 
     async def Bunkr(self, url: URL, title=None):
         bunkr_session = ScrapeSession(self.client)
         if not self.bunkr_crawler:
             self.bunkr_crawler = BunkrCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
                                               remove_bunkr_id=self.remove_bunkr_id)
-        async with self.bunkr_semaphore:
-            async with self.bunkr_limiter:
-                album_obj = await self.bunkr_crawler.fetch(bunkr_session, url)
+
+        album_obj = await self.bunkr_crawler.fetch(bunkr_session, url)
         if not await album_obj.is_empty():
             await self._handle_album_additions("bunkr", album_obj, title)
         await bunkr_session.exit_handler()
 
     async def Cyberdrop(self, url: URL, title=None):
         cyberdrop_session = ScrapeSession(self.client)
         if not self.cyberdrop_crawler:
@@ -159,16 +146,16 @@
         await self._handle_album_additions("cyberdrop", album_obj, title)
         await cyberdrop_session.exit_handler()
 
     async def CyberFile(self, url, title=None):
         cyberfile_session = ScrapeSession(self.client)
         if not self.cyberfile_crawler:
             self.cyberfile_crawler = CyberFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
-        async with self.cyberfile_semaphore:
-            domain_obj = await self.cyberfile_crawler.fetch(cyberfile_session, url)
+
+        domain_obj = await self.cyberfile_crawler.fetch(cyberfile_session, url)
         await self._handle_domain_additions("cyberfile", domain_obj, title)
         await cyberfile_session.exit_handler()
 
     async def EHentai(self, url, title=None):
         ehentai_session = ScrapeSession(self.client)
         if not self.ehentai_crawler:
             self.ehentai_crawler = EHentaiCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
@@ -192,19 +179,18 @@
         await self._handle_album_additions("gfycat", album_obj, title)
         await gfycat_session.exit_handler()
 
     async def GoFile(self, url, title=None):
         gofile_session = ScrapeSession(self.client)
         if not self.gofile_crawler:
             self.gofile_crawler = GoFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
-        async with self.gofile_limiter:
-            async with self.gofile_semaphore:
-                await self.gofile_crawler.get_token(session=gofile_session,
-                                                    api_token=self.args['Authentication']['gofile_api_key'])
-            domain_obj = await self.gofile_crawler.fetch(gofile_session, url)
+
+        await self.gofile_crawler.get_token(session=gofile_session,
+                                            api_token=self.args['Authentication']['gofile_api_key'])
+        domain_obj = await self.gofile_crawler.fetch(gofile_session, url)
         await self._handle_domain_additions("gofile", domain_obj, title)
         await gofile_session.exit_handler()
 
     async def HGameCG(self, url, title=None):
         hgamecg_session = ScrapeSession(self.client)
         if not self.hgamecg_crawler:
             self.hgamecg_crawler = HGameCGCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
@@ -260,20 +246,16 @@
         await self._handle_album_additions("saint", album_obj, title)
         await saint_session.exit_handler()
 
     async def ShareX(self, url, title=None):
         sharex_session = ScrapeSession(self.client)
         if not self.sharex_crawler:
             self.sharex_crawler = ShareXCrawler(include_id=self.include_id, quiet=self.quiet, SQL_Helper=self.SQL_Helper)
-        if ("jpg.fish" in url.host or "jpg.church" in url.host or "img.kiwi" in url.host) and sharex_session.client.ratelimit > 19:
-            async with self.jpgfish_semaphore:
-                async with self.jpgfish_limiter:
-                    domain_obj = await self.sharex_crawler.fetch(sharex_session, url)
-        else:
-            domain_obj = await self.sharex_crawler.fetch(sharex_session, url)
+
+        domain_obj = await self.sharex_crawler.fetch(sharex_session, url)
         await self._handle_domain_additions("sharex", domain_obj, title)
         await sharex_session.exit_handler()
 
     async def XBunkr(self, url, title=None):
         xbunkr_session = ScrapeSession(self.client)
         if not self.xbunkr_crawler:
             self.xbunkr_crawler = XBunkrCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
@@ -303,22 +285,16 @@
     async def Coomeno(self, url: URL, title=None):
         coomeno_session = ScrapeSession(self.client)
         if not self.coomeno_crawler:
             self.coomeno_crawler = CoomenoCrawler(include_id=self.include_id, scraping_mapper=self,
                                                   separate_posts=self.separate_posts, SQL_Helper=self.SQL_Helper,
                                                   quiet=self.quiet)
         assert url.host is not None
-        if "coomer" in url.host:
-            async with self.coomer_semaphore:
-                async with self.coomer_limiter:
-                    cascade, new_title = await self.coomeno_crawler.fetch(coomeno_session, url)
-        elif "kemono" in url.host:
-            async with self.kemono_semaphore:
-                async with self.kemono_limiter:
-                    cascade, new_title = await self.coomeno_crawler.fetch(coomeno_session, url)
+        cascade, new_title = await self.coomeno_crawler.fetch(coomeno_session, url)
+
         if not new_title or await cascade.is_empty():
             await coomeno_session.exit_handler()
             return
         if title:
             await cascade.append_title(title)
             await self.Forums.extend_thread(title, cascade)
         else:
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.12
+Version: 4.2.13
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.12 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.13 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.13/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 cyberdrop_dl/base_functions/config_schema.py
 cyberdrop_dl/base_functions/data_classes.py
 cyberdrop_dl/base_functions/error_classes.py
 cyberdrop_dl/base_functions/sorting_functions.py
 cyberdrop_dl/base_functions/sql_helper.py
 cyberdrop_dl/client/__init__.py
 cyberdrop_dl/client/client.py
-cyberdrop_dl/client/rate_limiting.py
 cyberdrop_dl/crawlers/Anonfiles_Spider.py
 cyberdrop_dl/crawlers/Bunkr_Spider.py
 cyberdrop_dl/crawlers/Coomeno_Spider.py
 cyberdrop_dl/crawlers/CyberFile_Spider.py
 cyberdrop_dl/crawlers/Cyberdrop_Spider.py
 cyberdrop_dl/crawlers/EHentai_Spider.py
 cyberdrop_dl/crawlers/Erome_Spider.py
```

### Comparing `cyberdrop-dl-4.2.12/setup.cfg` & `cyberdrop-dl-4.2.13/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 [options]
 python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires = 
 	aiofiles>=23.1.0
 	aiohttp>=3.8.4
+	aiolimiter>=1.0.0
 	beautifulsoup4>=4.12.2
 	certifi>=2022.12.7
 	myjdapi>=1.1.6
 	PyYAML>=6.0
 	rich>=13.3.4
 	setuptools>=67.7.2
 	yarl==1.8.2
```

