# Comparing `tmp/CrawlersTools-1.4.72.tar.gz` & `tmp/CrawlersTools-1.4.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrawlersTools-1.4.72.tar", last modified: Wed May  3 02:04:28 2023, max compression
+gzip compressed data, was "CrawlersTools-1.4.73.tar", last modified: Sun May  7 10:52:14 2023, max compression
```

## Comparing `CrawlersTools-1.4.72.tar` & `CrawlersTools-1.4.73.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.106403 CrawlersTools-1.4.72/CrawlersTools/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.106403 CrawlersTools-1.4.72/CrawlersTools/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/attachment_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/content_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/list_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.106403 CrawlersTools-1.4.72/CrawlersTools/extractors/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/schemas/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/time_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/title_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/js_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/js_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/js_crawler/font_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/js_crawler/transfer_js.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/logs/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/pipelines/mongo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/pipelines/mysql_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/pipelines/redis_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/preprocess/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/preprocess/time_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/projects/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/projects/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/projects/upload_oss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/CrawlersTools/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/requests/base_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/requests/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/requests/random_ua.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/CrawlersTools/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/schedules/auto_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.106403 CrawlersTools-1.4.72/CrawlersTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.622757 CrawlersTools-1.4.73/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.614756 CrawlersTools-1.4.73/CrawlersTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/attachment_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/content_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/list_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/extractors/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/schemas/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/time_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/title_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/extractors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/utils/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/extractors/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/js_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/js_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/js_crawler/font_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/js_crawler/transfer_js.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/logs/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/pipelines/mongo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/pipelines/mysql_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/pipelines/redis_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/preprocess/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/preprocess/time_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/projects/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/projects/upload_oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/requests/base_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/requests/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/requests/random_ua.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.618756 CrawlersTools-1.4.73/CrawlersTools/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/CrawlersTools/schedules/auto_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:52:14.614756 CrawlersTools-1.4.73/CrawlersTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-05-07 10:52:14.000000 CrawlersTools-1.4.73/CrawlersTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-07 10:52:14.000000 CrawlersTools-1.4.73/CrawlersTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:52:14.000000 CrawlersTools-1.4.73/CrawlersTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-07 10:52:14.000000 CrawlersTools-1.4.73/CrawlersTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 10:52:14.000000 CrawlersTools-1.4.73/CrawlersTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-05-07 10:52:14.622757 CrawlersTools-1.4.73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:52:14.622757 CrawlersTools-1.4.73/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-07 10:52:03.000000 CrawlersTools-1.4.73/setup.py
```

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/__init__.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/attachment_extractor.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/attachment_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/base.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/base.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/content_extractor.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/content_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/list_extractor.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/list_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/schemas/element.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/schemas/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/time_extractor.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/time_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/title_extractor.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/title_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/cluster.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/element.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/utils/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/preprocess.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/settings.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/utils/settings.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/similarity.py` & `CrawlersTools-1.4.73/CrawlersTools/extractors/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/js_crawler/font_decrypt.py` & `CrawlersTools-1.4.73/CrawlersTools/js_crawler/font_decrypt.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/js_crawler/transfer_js.py` & `CrawlersTools-1.4.73/CrawlersTools/js_crawler/transfer_js.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/logs/log.py` & `CrawlersTools-1.4.73/CrawlersTools/logs/log.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/pipelines/mongo_pipeline.py` & `CrawlersTools-1.4.73/CrawlersTools/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/pipelines/mysql_pipeline.py` & `CrawlersTools-1.4.73/CrawlersTools/pipelines/mysql_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/pipelines/redis_pipeline.py` & `CrawlersTools-1.4.73/CrawlersTools/pipelines/redis_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/preprocess/bloom_filter.py` & `CrawlersTools-1.4.73/CrawlersTools/preprocess/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/preprocess/time_process.py` & `CrawlersTools-1.4.73/CrawlersTools/preprocess/time_process.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/projects/filters.py` & `CrawlersTools-1.4.73/CrawlersTools/projects/filters.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/projects/upload_oss.py` & `CrawlersTools-1.4.73/CrawlersTools/projects/upload_oss.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/requests/base_requests.py` & `CrawlersTools-1.4.73/CrawlersTools/requests/base_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 
         js_text = js_text.split(';location.href=loc')[0].split('document.cookie=')[-1]
         r = execjs.eval(js_text).split(';')[0]
         return r
 
     @staticmethod
     def process_clearance(html):
+        import hashlib
 
         data = json.loads(re.findall(r'go\((.*?)\)', html)[1])
         chars_length = len(data.get('chars'))
         for i in range(chars_length):
             for j in range(chars_length):
                 result = data.get('bts')[0] + data.get('chars')[i] + data.get('chars')[j] + data.get('bts')[1]
                 b = eval('hashlib.{}()'.format(data.get('ha')))
```

### Comparing `CrawlersTools-1.4.72/CrawlersTools/requests/proxy.py` & `CrawlersTools-1.4.73/CrawlersTools/requests/proxy.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/requests/random_ua.py` & `CrawlersTools-1.4.73/CrawlersTools/requests/random_ua.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools/schedules/auto_thread.py` & `CrawlersTools-1.4.73/CrawlersTools/schedules/auto_thread.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/CrawlersTools.egg-info/PKG-INFO` & `CrawlersTools-1.4.73/CrawlersTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.72
+Version: 1.4.73
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.72/CrawlersTools.egg-info/SOURCES.txt` & `CrawlersTools-1.4.73/CrawlersTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/LICENSE` & `CrawlersTools-1.4.73/LICENSE`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/PKG-INFO` & `CrawlersTools-1.4.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.72
+Version: 1.4.73
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.72/README.md` & `CrawlersTools-1.4.73/README.md`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.72/setup.py` & `CrawlersTools-1.4.73/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='CrawlersTools',  # 包名
-    version='1.4.72',  # 版本号
+    version='1.4.73',  # 版本号
     description='Tools for Crawlers',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='MuggleK',
     author_email='peichangchuan@gmail.com',
     url='https://github.com/MuggleK/CrawlersTools',
     install_requires=[
```

