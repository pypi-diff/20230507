# Comparing `tmp/fastapi-listing-0.0.5.tar.gz` & `tmp/fastapi-listing-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-listing-0.0.5.tar", last modified: Wed May  3 18:30:26 2023, max compression
+gzip compressed data, was "fastapi-listing-0.0.7.tar", last modified: Sun May  7 19:25:13 2023, max compression
```

## Comparing `fastapi-listing-0.0.5.tar` & `fastapi-listing-0.0.7.tar`

### file list

```diff
@@ -1,57 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.161166 fastapi-listing-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 18:30:26.161166 fastapi-listing-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.149164 fastapi-listing-0.0.5/fastapi_listing/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.153164 fastapi-listing-0.0.5/fastapi_listing/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/base_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.153164 fastapi-listing-0.0.5/fastapi_listing/dao/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/dao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/dao/generic_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.153164 fastapi-listing-0.0.5/fastapi_listing/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/factory/_generic_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/factory/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/factory/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.153164 fastapi-listing-0.0.5/fastapi_listing/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/filters/generic_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/interface/listing_meta_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/mechanics/iterative_filter_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/mechanics/singleton_sorter_mechanics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/paginator/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/paginator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/paginator/naive_page_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/service/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/service/listing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/sorter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/sorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/sorter/naive_page_sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.161166 fastapi-listing-0.0.5/fastapi_listing/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/strategies/query_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.149164 fastapi-listing-0.0.5/fastapi_listing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:30:26.161166 fastapi-listing-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.415625 fastapi-listing-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    21413 2023-05-07 19:25:13.415625 fastapi-listing-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.411625 fastapi-listing-0.0.7/fastapi_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.411625 fastapi-listing-0.0.7/fastapi_listing/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/abstracts/base_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/abstracts/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/abstracts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/abstracts/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/abstracts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/abstracts/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.411625 fastapi-listing-0.0.7/fastapi_listing/dao/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/dao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/dao/generic_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.411625 fastapi-listing-0.0.7/fastapi_listing/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/factory/_generic_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/factory/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/factory/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.411625 fastapi-listing-0.0.7/fastapi_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/filters/generic_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.411625 fastapi-listing-0.0.7/fastapi_listing/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/interface/listing_meta_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.411625 fastapi-listing-0.0.7/fastapi_listing/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/mechanics/iterative_filter_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/mechanics/singleton_sorter_mechanics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.415625 fastapi-listing-0.0.7/fastapi_listing/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/paginator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/paginator/naive_page_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.415625 fastapi-listing-0.0.7/fastapi_listing/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/service/listing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.415625 fastapi-listing-0.0.7/fastapi_listing/sorter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/sorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/sorter/naive_page_sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.415625 fastapi-listing-0.0.7/fastapi_listing/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/strategies/query_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/fastapi_listing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.411625 fastapi-listing-0.0.7/fastapi_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21413 2023-05-07 19:25:13.000000 fastapi-listing-0.0.7/fastapi_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-07 19:25:13.000000 fastapi-listing-0.0.7/fastapi_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:25:13.000000 fastapi-listing-0.0.7/fastapi_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-07 19:25:13.000000 fastapi-listing-0.0.7/fastapi_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 19:25:13.000000 fastapi-listing-0.0.7/fastapi_listing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 19:25:13.415625 fastapi-listing-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:13.415625 fastapi-listing-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/tests/fake_listing_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-07 19:25:04.000000 fastapi-listing-0.0.7/tests/test_main.py
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/__init__.py` & `fastapi-listing-0.0.7/fastapi_listing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi_listing.factory import strategy_factory
 from fastapi_listing.strategies import NaiveQueryStrategy, NaivePaginationStrategy, SortingOrderStrategy
 from fastapi_listing.service.listing_main import ListingService, FastapiListing
 from fastapi_listing.mechanics import IterativeFilterMechanics, SingletonSorterMechanics
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.7"
 
 strategy_factory.register_strategy("naive_paginator", NaivePaginationStrategy)
 strategy_factory.register_strategy("naive_sorter", SortingOrderStrategy)
 strategy_factory.register_strategy("naive_query", NaiveQueryStrategy)
 strategy_factory.register_strategy("iterative_filter_mechanics", IterativeFilterMechanics)
 strategy_factory.register_strategy("singleton_sorter_mechanics", SingletonSorterMechanics)
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/abstracts/listing.py` & `fastapi-listing-0.0.7/fastapi_listing/abstracts/listing.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.5/fastapi_listing/dao/generic_dao.py` & `fastapi-listing-0.0.7/fastapi_listing/dao/generic_dao.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fastapi_listing.abstracts import DaoAbstract
 from sqlalchemy.orm import Session
+from typing import Union, Dict, List
 
 from fastapi_listing.typing import SqlAlchemyModel
 
 
 class GenericDao(DaoAbstract):  # type:ignore # noqa
     """
     Dao stands for data access object.
@@ -36,16 +37,16 @@
         # considering that we are dealing with separate read and write dbs.
         # we must have two sessions one for read replica and one for master or write replica
         # we should define our reusable attributes here that we will use in each dao method definition
         # even if we are using single db still having two references for the same session won't hurt
         # for future expansion once we decide to move on to read/write replica architecure
         # we already have groundwork done and only need to push different connections
         # from request lifecycle layer.
-        self._read_db: Session = read_db #kwargs.get("read_db")
-        self._write_db: Session = write_db #kwargs.get("write_db")
+        self._read_db: Session = read_db  # kwargs.get("read_db")
+        self._write_db: Session = write_db  # kwargs.get("write_db")
         # if self.model is None:
         #     raise ValueError("model class is not set!")
 
     # def __setattr__(cls, name, value):
     #     if name == "model":
     #         raise AttributeError("Cannot modify .model")
     #     else:
@@ -53,34 +54,35 @@
     #
     # def __delattr__(cls, name):
     #     if name == "model":
     #         raise AttributeError("Cannot delete .model")
     #     else:
     #         return type.__delattr__(cls, name)
 
-    def create(self, values: dict[str, str | int]) -> SqlAlchemyModel:
+    def create(self, values: Dict[str, Union[str, int]]) -> SqlAlchemyModel:
         """
         A light method that enters values in primary model table.
         single value at a time receives a dict implementation could map the dict with model values and
         insert that mapping or single row into the table.
         :param values: dict of values where keys are columns of table and value should be row values
         :return: created object i.e., instrumented row object.
         """
         raise NotImplementedError
 
-    def update(self, identifier: dict[str, str | int | list], values: dict) -> bool:
+    def update(self, identifier: Dict[str, Union[str, int, list]], values: dict) -> bool:
         """
         Similar to create method this receives an identifier
         :param identifier:
         :param values:
         :return:
         """
         raise NotImplementedError
 
-    def read(self, identifier: dict[str, str | int | list], fields: list | str = "__all__") -> SqlAlchemyModel:
+    def read(self, identifier: Dict[str, Union[str, int, list]],
+             fields: Union[list, str] = "__all__") -> SqlAlchemyModel:
         raise NotImplementedError
 
-    def delete(self, ids: list[int]) -> bool:
+    def delete(self, ids: List[int]) -> bool:
         raise NotImplementedError
 
     def get_naive_read(self, fields_to_read: list):
         return self._read_db.query(*fields_to_read)
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/factory/_generic_factory.py` & `fastapi-listing-0.0.7/fastapi_listing/factory/_generic_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Factory for creating a game character."""
 
-from typing import Any, Callable
+from typing import Any, Callable, Dict
 
-object_creation_collector: dict[str, Callable[..., Any]] = {}
+object_creation_collector: Dict[str, Callable[..., Any]] = {}
 
 
 def register(key: str, creator: Callable[..., Any]) -> None:
     print(creator)
     """Register a new game character type."""
     if key in object_creation_collector:
         raise ValueError(f"Factory can not have duplicate builder key {key} for instance {creator.__name__}")
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/filters/__init__.py` & `fastapi-listing-0.0.7/fastapi_listing/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.5/fastapi_listing/filters/generic_filters.py` & `fastapi-listing-0.0.7/fastapi_listing/filters/generic_filters.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.5/fastapi_listing/interface/listing_meta_info.py` & `fastapi-listing-0.0.7/fastapi_listing/interface/listing_meta_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-from typing import Protocol, Type
-
+try:
+    from typing import Protocol
+except ImportError:
+    from typing_extensions import Protocol
+from typing import Dict
 from fastapi_listing.abstracts import TableDataSortingStrategy, TableDataPaginatingStrategy, QueryStrategy
 from fastapi_listing.sorter import SortingOrderStrategy
 
 
 class ListingMetaInfo(Protocol):
 
     @property
@@ -23,15 +26,15 @@
         ...
 
     @property
     def sorting_strategy() -> TableDataSortingStrategy:  # type:ignore # noqa
         ...
 
     @property
-    def default_sort_val() -> dict[str, str]:  # type:ignore # noqa
+    def default_sort_val() -> Dict[str, str]:  # type:ignore # noqa
         ...
 
     @property
     def sorter_mechanic() -> str:  # type:ignore # noqa
         ...
 
     @property
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/loader.py` & `fastapi-listing-0.0.7/fastapi_listing/loader.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.5/fastapi_listing/mechanics/iterative_filter_mechanics.py` & `fastapi-listing-0.0.7/fastapi_listing/mechanics/iterative_filter_mechanics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import List, Dict
 from fastapi_listing.factory import filter_factory, _generic_factory
 from fastapi_listing.filters import CommonFilterImpl
 from fastapi_listing.typing import SqlAlchemyQuery, FastapiRequest
 
 
 class IterativeFilterMechanics:
 
@@ -16,15 +17,15 @@
     to give a real world example
     if user has applied city, pincode, region filter then
     pincode is the most atomic unit here region and city filters are just extra burden on query and db as well.
     one can tackle this situation by having a mechanic which will check if specific filter is applied
     with other relative filters then don't apply other relative filters...
     """
 
-    def apply(self, *, query: SqlAlchemyQuery = None, filter_params: list[dict[str, str]], dao=None,
+    def apply(self, *, query: SqlAlchemyQuery = None, filter_params: List[Dict[str, str]], dao=None,
               request: FastapiRequest = None, extra_context: dict = None) -> SqlAlchemyQuery:
         for applied_filter in filter_params:
             filter_obj: CommonFilterImpl = filter_factory.create(applied_filter.get("field"),
                                                                  dao=dao,
                                                                  request=request,
                                                                  extra_context=extra_context)
             query = filter_obj.filter(field=applied_filter.get("field"),
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/mechanics/singleton_sorter_mechanics.py` & `fastapi-listing-0.0.7/fastapi_listing/mechanics/singleton_sorter_mechanics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fastapi_listing.factory import _generic_factory
+from typing import List, Dict
 from fastapi_listing.abstracts import TableDataSortingStrategy
 from fastapi_listing.typing import SqlAlchemyQuery
 
 
 class SingletonSorterMechanics:
     """
     Singleton Sorter mechanic.
@@ -13,15 +13,15 @@
         # the latest one which is last column that client requested to sort on.
         # if user want they can implement their own asc or dsc sorting order strategy and
         # decide how they really want to apply sorting params maybe all maybe none or maybe
         # conditional sorting where if one param is applied then don't apply another specific one, etc.
     """
 
     def apply(self, *, query: SqlAlchemyQuery = None, strategy: TableDataSortingStrategy = None,
-              sorting_params: list[dict[str, str]] = None, extra_context: dict = None) -> SqlAlchemyQuery:
+              sorting_params: List[Dict[str, str]] = None, extra_context: dict = None) -> SqlAlchemyQuery:
         latest = sorting_params[-1]
         query = strategy.sort(query=query, value=latest, extra_context=extra_context)
         return query
 
 
 # def register() -> None:
 #     generic_factory.register("singleton_sorter_mechanics", SingletonSorterMechanics)
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/paginator/naive_page_builder.py` & `fastapi-listing-0.0.7/fastapi_listing/paginator/naive_page_builder.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.5/fastapi_listing/service/listing_main.py` & `fastapi-listing-0.0.7/fastapi_listing/service/listing_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from fastapi import Request
 from sqlalchemy.orm import Query
 from json import JSONDecodeError
-from typing import Type, Optional
+from typing import Type, Optional, Dict, List
 
 from fastapi_listing import utils
 from fastapi_listing.abstracts import TableDataPaginatingStrategy
 from fastapi_listing.typing import ListingResponseType
 from fastapi_listing.abstracts import ListingBase, ListingServiceBase
 from fastapi_listing.factory import strategy_factory
-from fastapi_listing.errors import ListingFilterError, ListingSorterError
+from fastapi_listing.errors import ListingFilterError, ListingSorterError, FastapiListingRequestSemanticApiException,\
+    NotRegisteredApiException
 from fastapi_listing.dao.generic_dao import GenericDao
 from fastapi_listing.interface.listing_meta_info import ListingMetaInfo
 from fastapi_listing import constants
 import os
+from fastapi import HTTPException
 
 try:
     from pydantic import BaseModel
 
     HAS_PYDANTIC = True
 except ImportError:
     HAS_PYDANTIC = False
@@ -31,29 +33,30 @@
         self.dao = dao
         if HAS_PYDANTIC and pydantic_serializer:
             self.fields_to_fetch = list(pydantic_serializer.__fields__.keys())
         else:
             self.fields_to_fetch = []
         self.custom_fields = custom_fields
 
-    def _replace_aliases(self, mapper: dict[str, str], req_params: list[dict[str, str]]) -> list[dict[str, str]]:
+    def _replace_aliases(self, mapper: Dict[str, str], req_params: List[Dict[str, str]]) -> List[Dict[str, str]]:
         req_prms_cpy = req_params.copy()
         for param in req_prms_cpy:
             param["field"] = mapper[param["field"]]
         return req_prms_cpy
 
     def _apply_sorting(self, query: Query, listing_meta_info: ListingMetaInfo) -> Query:
         try:
             sorting_params: list[dict] = utils.jsonify_query_params(self.request.query_params.get("sort"))
         except JSONDecodeError:
-            raise ListingSorterError("sorter param is not a valid json!")
-
-        if temp := set(item.get("field") for item in sorting_params) - set(
-                listing_meta_info.sorting_column_mapper.keys()):
-            raise ListingSorterError(f"Sorter'(s) not registered with listing: {temp}, Did you forget to do it?")
+            raise FastapiListingRequestSemanticApiException(status_code=422, detail="sorter param is not a valid json!")
+        temp = set(item.get("field") for item in sorting_params) - set(
+            listing_meta_info.sorting_column_mapper.keys())
+        if temp:
+            raise NotRegisteredApiException(
+                status_code=409, detail=f"Sorter'(s) not registered with listing: {temp}, Did you forget to do it?")
         if sorting_params:
             sorting_params = self._replace_aliases(listing_meta_info.sorting_column_mapper, sorting_params)
         else:
             sorting_params = [listing_meta_info.default_sort_val]
 
         # ideally sorting should only happen on one field multi field sorting puts
         # unwanted strain on table when the size is big and not really popular
@@ -94,18 +97,19 @@
     # we can leave multi sorting for later release for now only allow sort on a singular field.
     # this class name is not looking to good think of a different name if possible.
     # FilterApplicationEngine
     def _apply_filters(self, query: Query, listing_meta_info: ListingMetaInfo) -> Query:
         try:
             fltrs: list[dict] = utils.jsonify_query_params(self.request.query_params.get("filter"))
         except JSONDecodeError:
-            raise ListingFilterError(f"filter param is not a valid json!")
-
-        if temp := set(item.get("field") for item in fltrs) - set(listing_meta_info.filter_column_mapper.keys()):
-            raise ListingFilterError(f"Filter'(s) not registered with listing: {temp}, Did you forget to do it?")
+            raise FastapiListingRequestSemanticApiException(status_code=422, detail=f"filter param is not a valid json!")
+        temp = set(item.get("field") for item in fltrs) - set(listing_meta_info.filter_column_mapper.keys())
+        if temp:
+            raise NotRegisteredApiException(
+                status_code=409, detail=f"Filter'(s) not registered with listing: {temp}, Did you forget to do it?")
 
         fltrs = self._replace_aliases(listing_meta_info.filter_column_mapper, fltrs)
 
         def launch_mechanics(qry):
             mecha_obj = strategy_factory.create(listing_meta_info.filter_mechanic)
             qry = mecha_obj.apply(query=qry, filter_params=fltrs, dao=self.dao,
                                   request=self.request, extra_context=listing_meta_info.extra_context)
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/sorter/naive_page_sorter.py` & `fastapi-listing-0.0.7/fastapi_listing/sorter/naive_page_sorter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Dict
 from fastapi_listing.abstracts import TableDataSortingStrategy
 from fastapi_listing.typing import SqlAlchemyModel, FastapiRequest, SqlAlchemyQuery, AnySqlAlchemyColumn
 
 
 class SortingOrderStrategy(TableDataSortingStrategy):
 
     def __init__(self, model: SqlAlchemyModel = None, request: FastapiRequest = None):
@@ -14,19 +15,19 @@
         return query
 
     @staticmethod
     def sort_dsc_util(query: SqlAlchemyQuery, inst_field: AnySqlAlchemyColumn) -> SqlAlchemyQuery:
         query = query.order_by(inst_field.desc())
         return query
 
-    def sort(self, *, query: SqlAlchemyQuery = None, value: dict[str, str] = None,
+    def sort(self, *, query: SqlAlchemyQuery = None, value: Dict[str, str] = None,
              extra_context: dict = None) -> SqlAlchemyQuery:
-        assert value["type"] in ["asc", "dsc"]
         if value is None:
             raise ValueError("sort expects value with structure [type, field], none provided")
+        assert value["type"] in ["asc", "dsc"], "invalid sorting style!"
         inst_field: AnySqlAlchemyColumn = self.validate_srt_field(self.model, value["field"])
         if value["type"] == "asc":
             query = self.sort_asc_util(query, inst_field)
         else:
             query = self.sort_dsc_util(query, inst_field)
         return query
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing/strategies/__init__.py` & `fastapi-listing-0.0.7/fastapi_listing/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.5/fastapi_listing/strategies/query_strategy.py` & `fastapi-listing-0.0.7/fastapi_listing/strategies/query_strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.5/fastapi_listing/typing.py` & `fastapi-listing-0.0.7/fastapi_listing/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, List, Dict
+from typing import TypeVar, List, Dict, Union
 from typing_extensions import TypedDict
 from fastapi import Request
 
 # will support future imports as well like pymongo and other orm tools
 
 try:
     from sqlalchemy.orm.decl_api import DeclarativeMeta
@@ -14,15 +14,15 @@
     DeclarativeMeta = None
     Query = None
     Session = None
     Column = None
 
 
 class ListingResponseType(TypedDict):
-    data: List[Dict[str, int | str | list | dict]]
+    data: List[Dict[str, Union[int, str, list, dict]]]
     currentPageNumber: int
     currentPageSize: int
     totalCount: int
     hasNext: bool
 
 
 SqlAlchemyQuery = TypeVar("SqlAlchemyQuery", bound=Query)
```

### Comparing `fastapi-listing-0.0.5/fastapi_listing.egg-info/SOURCES.txt` & `fastapi-listing-0.0.7/fastapi_listing.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -35,8 +35,11 @@
 fastapi_listing/paginator/__init__.py
 fastapi_listing/paginator/naive_page_builder.py
 fastapi_listing/service/__init__.py
 fastapi_listing/service/listing_main.py
 fastapi_listing/sorter/__init__.py
 fastapi_listing/sorter/naive_page_sorter.py
 fastapi_listing/strategies/__init__.py
-fastapi_listing/strategies/query_strategy.py
+fastapi_listing/strategies/query_strategy.py
+tests/__init__.py
+tests/fake_listing_setup.py
+tests/test_main.py
```

### Comparing `fastapi-listing-0.0.5/setup.py` & `fastapi-listing-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,22 +37,28 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.7",
-    keywords=["starlette", "fastapi", "starlite", "pydantic"],
+    keywords=["starlette", "fastapi", "pydantic", "sqlalchemy"],
     extras_require={
         "test": [
             "requests",
+            "pytest>=6.2.4",
             "mypy>=0.971",
+            "pytest-env>=0.6.2",
             "flake8>=3.9.2",
             "isort>=5.10.1",
             "pydantic>=1.5.0",
             "starlette>=0.21.0",
             "sqlalchemy>=2.0.7",
             "starlite>=1.38.0",
             "httpx>=0.23.0",
+            "pytest-mock>=3.6.1",
+            "fastapi>=0.92.0",
+            "mypy>=0.971",
+            "pytest-mypy>=0.9.1",
         ],
     },
 )
```

