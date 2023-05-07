# Comparing `tmp/dhapi-1.3.4.tar.gz` & `tmp/dhapi-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhapi-1.3.4.tar", last modified: Sun May  7 15:10:52 2023, max compression
+gzip compressed data, was "dhapi-1.3.5.tar", last modified: Sun May  7 15:13:47 2023, max compression
```

## Comparing `dhapi-1.3.4.tar` & `dhapi-1.3.5.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.227639 dhapi-1.3.4/
--rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-04-19 16:05:26.000000 dhapi-1.3.4/LICENSE.txt
--rw-r--r--   0 roeniss    (501) staff       (20)     1900 2023-05-07 15:10:52.227515 dhapi-1.3.4/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)     1245 2023-05-07 14:36:29.000000 dhapi-1.3.4/README.md
--rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-04-30 18:03:10.000000 dhapi-1.3.4/pyproject.toml
--rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-05-07 15:10:52.227670 dhapi-1.3.4/setup.cfg
--rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-05-07 15:06:57.000000 dhapi-1.3.4/setup.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.222521 dhapi-1.3.4/src/
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.223639 dhapi-1.3.4/src/dhapi/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/__init__.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.226194 dhapi-1.3.4/src/dhapi/client/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/client/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     4804 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/client/lottery_client.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.226405 dhapi-1.3.4/src/dhapi/domain_object/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/domain_object/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3313 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/domain_object/lotto645_buy_request.py
--rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/main.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.226598 dhapi-1.3.4/src/dhapi/purchase/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/purchase/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     2410 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/purchase/lotto645_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.227073 dhapi-1.3.4/src/dhapi/router/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/router/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     5132 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/router/arg_parser.py
--rw-r--r--   0 roeniss    (501) staff       (20)      518 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/router/router.py
--rw-r--r--   0 roeniss    (501) staff       (20)      953 2023-05-07 15:10:00.000000 dhapi-1.3.4/src/dhapi/router/version_checker.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.227306 dhapi-1.3.4/src/dhapi/user_info/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/user_info/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/user_info/user_info_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.225989 dhapi-1.3.4/src/dhapi.egg-info/
--rw-r--r--   0 roeniss    (501) staff       (20)     1900 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      705 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/SOURCES.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/dependency_links.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/entry_points.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       72 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/requires.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/top_level.txt
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.163349 dhapi-1.3.5/
+-rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-04-19 16:05:26.000000 dhapi-1.3.5/LICENSE.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)     1900 2023-05-07 15:13:47.163217 dhapi-1.3.5/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)     1245 2023-05-07 14:36:29.000000 dhapi-1.3.5/README.md
+-rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-04-30 18:03:10.000000 dhapi-1.3.5/pyproject.toml
+-rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-05-07 15:13:47.163387 dhapi-1.3.5/setup.cfg
+-rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-05-07 15:06:57.000000 dhapi-1.3.5/setup.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.157468 dhapi-1.3.5/src/
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.158573 dhapi-1.3.5/src/dhapi/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/__init__.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.161861 dhapi-1.3.5/src/dhapi/client/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/client/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     4804 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/client/lottery_client.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.162066 dhapi-1.3.5/src/dhapi/configuration/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-07 15:12:24.000000 dhapi-1.3.5/src/dhapi/configuration/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      862 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/configuration/logger.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.162249 dhapi-1.3.5/src/dhapi/domain_object/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/domain_object/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     3313 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/domain_object/lotto645_buy_request.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/main.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.162445 dhapi-1.3.5/src/dhapi/purchase/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/purchase/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     2410 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/purchase/lotto645_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.162839 dhapi-1.3.5/src/dhapi/router/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/router/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     5132 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/router/arg_parser.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      518 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/router/router.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      953 2023-05-07 15:10:00.000000 dhapi-1.3.5/src/dhapi/router/version_checker.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.163035 dhapi-1.3.5/src/dhapi/user_info/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/user_info/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/user_info/user_info_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.161670 dhapi-1.3.5/src/dhapi.egg-info/
+-rw-r--r--   0 roeniss    (501) staff       (20)     1900 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)      775 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/SOURCES.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/dependency_links.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/entry_points.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       72 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/requires.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/top_level.txt
```

### Comparing `dhapi-1.3.4/LICENSE.txt` & `dhapi-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/PKG-INFO` & `dhapi-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhapi
-Version: 1.3.4
+Version: 1.3.5
 Summary: 동행복권 비공식 API
 Home-page: https://github.com/roeniss/dhlottery-api
 Author: Roeniss Moon
 Author-email: roeniss2@gmail.com
 Project-URL: Bug Reports, https://github.com/roeniss/dhlottery-api/issues
 Project-URL: Source, https://github.com/roeniss/dhlottery-api/
 Keywords: donghaeng,lottery,lotto645,api,korean
```

### Comparing `dhapi-1.3.4/README.md` & `dhapi-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/setup.py` & `dhapi-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/src/dhapi/client/lottery_client.py` & `dhapi-1.3.5/src/dhapi/client/lottery_client.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/src/dhapi/domain_object/lotto645_buy_request.py` & `dhapi-1.3.5/src/dhapi/domain_object/lotto645_buy_request.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/src/dhapi/purchase/lotto645_controller.py` & `dhapi-1.3.5/src/dhapi/purchase/lotto645_controller.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/src/dhapi/router/arg_parser.py` & `dhapi-1.3.5/src/dhapi/router/arg_parser.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/src/dhapi/router/router.py` & `dhapi-1.3.5/src/dhapi/router/router.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/src/dhapi/router/version_checker.py` & `dhapi-1.3.5/src/dhapi/router/version_checker.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.4/src/dhapi.egg-info/PKG-INFO` & `dhapi-1.3.5/src/dhapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhapi
-Version: 1.3.4
+Version: 1.3.5
 Summary: 동행복권 비공식 API
 Home-page: https://github.com/roeniss/dhlottery-api
 Author: Roeniss Moon
 Author-email: roeniss2@gmail.com
 Project-URL: Bug Reports, https://github.com/roeniss/dhlottery-api/issues
 Project-URL: Source, https://github.com/roeniss/dhlottery-api/
 Keywords: donghaeng,lottery,lotto645,api,korean
```

### Comparing `dhapi-1.3.4/src/dhapi.egg-info/SOURCES.txt` & `dhapi-1.3.5/src/dhapi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 src/dhapi.egg-info/SOURCES.txt
 src/dhapi.egg-info/dependency_links.txt
 src/dhapi.egg-info/entry_points.txt
 src/dhapi.egg-info/requires.txt
 src/dhapi.egg-info/top_level.txt
 src/dhapi/client/__init__.py
 src/dhapi/client/lottery_client.py
+src/dhapi/configuration/__init__.py
+src/dhapi/configuration/logger.py
 src/dhapi/domain_object/__init__.py
 src/dhapi/domain_object/lotto645_buy_request.py
 src/dhapi/purchase/__init__.py
 src/dhapi/purchase/lotto645_controller.py
 src/dhapi/router/__init__.py
 src/dhapi/router/arg_parser.py
 src/dhapi/router/router.py
```

