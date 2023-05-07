# Comparing `tmp/league-shop-base-1.0.8.tar.gz` & `tmp/league-shop-base-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "league-shop-base-1.0.8.tar", last modified: Thu Jan 26 05:37:44 2023, max compression
+gzip compressed data, was "league-shop-base-1.0.9.tar", last modified: Thu Feb 16 07:45:53 2023, max compression
```

## Comparing `league-shop-base-1.0.8.tar` & `league-shop-base-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 05:37:44.991344 league-shop-base-1.0.8/
--rw-rw-rw-   0        0        0     1093 2022-06-29 07:43:58.000000 league-shop-base-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       70 2023-01-01 09:05:57.000000 league-shop-base-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1529 2023-01-26 05:37:44.991344 league-shop-base-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-01-10 12:18:24.000000 league-shop-base-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-26 05:37:44.806243 league-shop-base-1.0.8/league_shop_base.egg-info/
--rw-rw-rw-   0        0        0     1529 2023-01-26 05:37:44.000000 league-shop-base-1.0.8/league_shop_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      814 2023-01-26 05:37:44.000000 league-shop-base-1.0.8/league_shop_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 05:37:44.000000 league-shop-base-1.0.8/league_shop_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-01-26 05:37:44.000000 league-shop-base-1.0.8/league_shop_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-01-26 05:37:44.000000 league-shop-base-1.0.8/league_shop_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-26 05:37:44.938965 league-shop-base-1.0.8/lsb/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:31:26.000000 league-shop-base-1.0.8/lsb/__init__.py
--rw-rw-rw-   0        0        0     2528 2023-01-26 05:36:23.000000 league-shop-base-1.0.8/lsb/admin.py
--rw-rw-rw-   0        0        0      144 2023-01-03 09:04:47.000000 league-shop-base-1.0.8/lsb/apps.py
--rw-rw-rw-   0        0        0      779 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/crypto.py
-drwxrwxrwx   0        0        0        0 2023-01-26 05:37:44.941961 league-shop-base-1.0.8/lsb/ddragon/
--rw-rw-rw-   0        0        0       89 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/ddragon/__init__.py
--rw-rw-rw-   0        0        0     2503 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/ddragon/_ddragon.py
--rw-rw-rw-   0        0        0     2930 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/ddragon/_skins.py
-drwxrwxrwx   0        0        0        0 2023-01-26 05:37:44.968408 league-shop-base-1.0.8/lsb/migrations/
--rw-rw-rw-   0        0        0     3686 2023-01-01 08:34:51.000000 league-shop-base-1.0.8/lsb/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      426 2023-01-16 04:53:14.000000 league-shop-base-1.0.8/lsb/migrations/0002_product_country.py
--rw-rw-rw-   0        0        0      441 2023-01-25 08:33:29.000000 league-shop-base-1.0.8/lsb/migrations/0003_product_summoner_name.py
--rw-rw-rw-   0        0        0        0 2023-01-01 08:31:26.000000 league-shop-base-1.0.8/lsb/migrations/__init__.py
--rw-rw-rw-   0        0        0     4615 2023-01-25 08:32:23.000000 league-shop-base-1.0.8/lsb/models.py
--rw-rw-rw-   0        0        0     3185 2023-01-25 08:34:58.000000 league-shop-base-1.0.8/lsb/serializers.py
-drwxrwxrwx   0        0        0        0 2023-01-26 05:37:44.720530 league-shop-base-1.0.8/lsb/templates/
-drwxrwxrwx   0        0        0        0 2023-01-26 05:37:44.985434 league-shop-base-1.0.8/lsb/templates/shop/
--rw-rw-rw-   0        0        0      191 2023-01-01 08:35:58.000000 league-shop-base-1.0.8/lsb/templates/shop/skins_change_list.html
--rw-rw-rw-   0        0        0      218 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/templates/shop/skins_download_failure.html
--rw-rw-rw-   0        0        0      233 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/templates/shop/skins_download_success.html
--rw-rw-rw-   0        0        0       63 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/tests.py
-drwxrwxrwx   0        0        0        0 2023-01-26 05:37:44.990348 league-shop-base-1.0.8/lsb/utils/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/utils/__init__.py
--rw-rw-rw-   0        0        0      456 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/utils/champion_rates.py
--rw-rw-rw-   0        0        0      674 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/utils/product.py
--rw-rw-rw-   0        0        0      288 2023-01-01 08:30:40.000000 league-shop-base-1.0.8/lsb/utils/skins.py
--rw-rw-rw-   0        0        0     4598 2023-01-10 12:14:25.000000 league-shop-base-1.0.8/lsb/views.py
--rw-rw-rw-   0        0        0      110 2023-01-01 04:52:22.000000 league-shop-base-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1001 2023-01-26 05:37:44.993339 league-shop-base-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-01-01 04:56:58.000000 league-shop-base-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-16 07:45:53.348770 league-shop-base-1.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-06-29 07:43:58.000000 league-shop-base-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       70 2023-01-01 09:05:57.000000 league-shop-base-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1529 2023-02-16 07:45:53.349770 league-shop-base-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-01-10 12:18:24.000000 league-shop-base-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-16 07:45:53.207399 league-shop-base-1.0.9/league_shop_base.egg-info/
+-rw-rw-rw-   0        0        0     1529 2023-02-16 07:45:53.000000 league-shop-base-1.0.9/league_shop_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2023-02-16 07:45:53.000000 league-shop-base-1.0.9/league_shop_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-16 07:45:53.000000 league-shop-base-1.0.9/league_shop_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-02-16 07:45:53.000000 league-shop-base-1.0.9/league_shop_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-02-16 07:45:53.000000 league-shop-base-1.0.9/league_shop_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-16 07:45:53.315858 league-shop-base-1.0.9/lsb/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:31:26.000000 league-shop-base-1.0.9/lsb/__init__.py
+-rw-rw-rw-   0        0        0     2528 2023-01-26 05:36:23.000000 league-shop-base-1.0.9/lsb/admin.py
+-rw-rw-rw-   0        0        0      144 2023-01-03 09:04:47.000000 league-shop-base-1.0.9/lsb/apps.py
+-rw-rw-rw-   0        0        0      779 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/crypto.py
+drwxrwxrwx   0        0        0        0 2023-02-16 07:45:53.321842 league-shop-base-1.0.9/lsb/ddragon/
+-rw-rw-rw-   0        0        0       89 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/ddragon/__init__.py
+-rw-rw-rw-   0        0        0     2503 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/ddragon/_ddragon.py
+-rw-rw-rw-   0        0        0     2930 2023-02-16 07:37:51.000000 league-shop-base-1.0.9/lsb/ddragon/_skins.py
+drwxrwxrwx   0        0        0        0 2023-02-16 07:45:53.327826 league-shop-base-1.0.9/lsb/migrations/
+-rw-rw-rw-   0        0        0     3686 2023-01-01 08:34:51.000000 league-shop-base-1.0.9/lsb/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      426 2023-01-16 04:53:14.000000 league-shop-base-1.0.9/lsb/migrations/0002_product_country.py
+-rw-rw-rw-   0        0        0      441 2023-01-25 08:33:29.000000 league-shop-base-1.0.9/lsb/migrations/0003_product_summoner_name.py
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:31:26.000000 league-shop-base-1.0.9/lsb/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4615 2023-01-25 08:32:23.000000 league-shop-base-1.0.9/lsb/models.py
+-rw-rw-rw-   0        0        0     3185 2023-01-25 08:34:58.000000 league-shop-base-1.0.9/lsb/serializers.py
+drwxrwxrwx   0        0        0        0 2023-02-16 07:45:53.172978 league-shop-base-1.0.9/lsb/templates/
+drwxrwxrwx   0        0        0        0 2023-02-16 07:45:53.332813 league-shop-base-1.0.9/lsb/templates/shop/
+-rw-rw-rw-   0        0        0      191 2023-01-01 08:35:58.000000 league-shop-base-1.0.9/lsb/templates/shop/skins_change_list.html
+-rw-rw-rw-   0        0        0      218 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/templates/shop/skins_download_failure.html
+-rw-rw-rw-   0        0        0      233 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/templates/shop/skins_download_success.html
+-rw-rw-rw-   0        0        0       63 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/tests.py
+drwxrwxrwx   0        0        0        0 2023-02-16 07:45:53.347775 league-shop-base-1.0.9/lsb/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/utils/__init__.py
+-rw-rw-rw-   0        0        0      456 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/utils/champion_rates.py
+-rw-rw-rw-   0        0        0      674 2023-01-01 08:30:40.000000 league-shop-base-1.0.9/lsb/utils/product.py
+-rw-rw-rw-   0        0        0     2482 2023-02-16 07:43:47.000000 league-shop-base-1.0.9/lsb/utils/skins.py
+-rw-rw-rw-   0        0        0     4598 2023-02-16 07:26:21.000000 league-shop-base-1.0.9/lsb/views.py
+-rw-rw-rw-   0        0        0      110 2023-01-01 04:52:22.000000 league-shop-base-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1001 2023-02-16 07:45:53.356750 league-shop-base-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-01-01 04:56:58.000000 league-shop-base-1.0.9/setup.py
```

### Comparing `league-shop-base-1.0.8/LICENSE` & `league-shop-base-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/PKG-INFO` & `league-shop-base-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: league-shop-base
-Version: 1.0.8
+Version: 1.0.9
 Summary: A reusable Django app for league shop.
 Home-page: https://github.com/sandbox-pokhara/league-shop-base.git
 Author: Anchal Gurung
 Author-email: anchalghale@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `league-shop-base-1.0.8/README.md` & `league-shop-base-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/league_shop_base.egg-info/PKG-INFO` & `league-shop-base-1.0.9/league_shop_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: league-shop-base
-Version: 1.0.8
+Version: 1.0.9
 Summary: A reusable Django app for league shop.
 Home-page: https://github.com/sandbox-pokhara/league-shop-base.git
 Author: Anchal Gurung
 Author-email: anchalghale@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `league-shop-base-1.0.8/league_shop_base.egg-info/SOURCES.txt` & `league-shop-base-1.0.9/league_shop_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/admin.py` & `league-shop-base-1.0.9/lsb/admin.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/crypto.py` & `league-shop-base-1.0.9/lsb/crypto.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/ddragon/_ddragon.py` & `league-shop-base-1.0.9/lsb/ddragon/_ddragon.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/ddragon/_skins.py` & `league-shop-base-1.0.9/lsb/ddragon/_skins.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/migrations/0001_initial.py` & `league-shop-base-1.0.9/lsb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/models.py` & `league-shop-base-1.0.9/lsb/models.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/serializers.py` & `league-shop-base-1.0.9/lsb/serializers.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/utils/product.py` & `league-shop-base-1.0.9/lsb/utils/product.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/lsb/views.py` & `league-shop-base-1.0.9/lsb/views.py`

 * *Files identical despite different names*

### Comparing `league-shop-base-1.0.8/setup.cfg` & `league-shop-base-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 6561 6775 652d 7368 6f70 2d62   = league-shop-b
 00000020: 6173 650d 0a76 6572 7369 6f6e 203d 2031  ase..version = 1
-00000030: 2e30 2e38 0d0a 6465 7363 7269 7074 696f  .0.8..descriptio
+00000030: 2e30 2e39 0d0a 6465 7363 7269 7074 696f  .0.9..descriptio
 00000040: 6e20 3d20 4120 7265 7573 6162 6c65 2044  n = A reusable D
 00000050: 6a61 6e67 6f20 6170 7020 666f 7220 6c65  jango app for le
 00000060: 6167 7565 2073 686f 702e 0d0a 6c6f 6e67  ague shop...long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

