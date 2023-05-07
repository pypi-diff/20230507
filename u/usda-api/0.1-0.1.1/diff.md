# Comparing `tmp/usda_api-0.1.tar.gz` & `tmp/usda_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usda_api-0.1.tar", last modified: Sat May  6 09:56:49 2023, max compression
+gzip compressed data, was "usda_api-0.1.1.tar", last modified: Sun May  7 03:42:07 2023, max compression
```

## Comparing `usda_api-0.1.tar` & `usda_api-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.635925 usda_api-0.1/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      182 2023-05-06 09:56:49.635448 usda_api-0.1/PKG-INFO
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:32:11.000000 usda_api-0.1/README.md
--rw-r--r--   0 lohyikuang   (501) staff       (20)       38 2023-05-06 09:56:49.636065 usda_api-0.1/setup.cfg
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1850 2023-05-06 09:43:55.000000 usda_api-0.1/setup.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.620395 usda_api-0.1/src/
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.623014 usda_api-0.1/src/usda_api/
--rw-r--r--   0 lohyikuang   (501) staff       (20)       20 2023-05-06 08:30:26.000000 usda_api-0.1/src/usda_api/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.628272 usda_api-0.1/src/usda_api/scrapers/
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 08:30:22.000000 usda_api-0.1/src/usda_api/scrapers/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.629583 usda_api-0.1/src/usda_api/scrapers/esr/
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:25.000000 usda_api-0.1/src/usda_api/scrapers/esr/__init__.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     6552 2023-05-06 09:43:55.000000 usda_api-0.1/src/usda_api/scrapers/esr/main.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.632675 usda_api-0.1/src/usda_api/scrapers/esr/schemas/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      470 2023-05-06 09:43:55.000000 usda_api-0.1/src/usda_api/scrapers/esr/schemas/__init__.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     2019 2023-05-06 09:36:01.000000 usda_api-0.1/src/usda_api/scrapers/esr/schemas/response.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.634024 usda_api-0.1/src/usda_api/scrapers/gats/
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:42.000000 usda_api-0.1/src/usda_api/scrapers/gats/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.634711 usda_api-0.1/src/usda_api/scrapers/psd/
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:44.000000 usda_api-0.1/src/usda_api/scrapers/psd/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-06 09:56:49.627314 usda_api-0.1/src/usda_api.egg-info/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      182 2023-05-06 09:56:49.000000 usda_api-0.1/src/usda_api.egg-info/PKG-INFO
--rw-r--r--   0 lohyikuang   (501) staff       (20)      536 2023-05-06 09:56:49.000000 usda_api-0.1/src/usda_api.egg-info/SOURCES.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)        1 2023-05-06 09:56:49.000000 usda_api-0.1/src/usda_api.egg-info/dependency_links.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)       55 2023-05-06 09:56:49.000000 usda_api-0.1/src/usda_api.egg-info/entry_points.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)      404 2023-05-06 09:56:49.000000 usda_api-0.1/src/usda_api.egg-info/requires.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)        9 2023-05-06 09:56:49.000000 usda_api-0.1/src/usda_api.egg-info/top_level.txt
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.348842 usda_api-0.1.1/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      184 2023-05-07 03:42:07.348022 usda_api-0.1.1/PKG-INFO
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:32:11.000000 usda_api-0.1.1/README.md
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       38 2023-05-07 03:42:07.349077 usda_api-0.1.1/setup.cfg
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1850 2023-05-06 09:43:55.000000 usda_api-0.1.1/setup.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.329935 usda_api-0.1.1/src/
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.333858 usda_api-0.1.1/src/usda_api/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       22 2023-05-06 14:37:07.000000 usda_api-0.1.1/src/usda_api/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.339325 usda_api-0.1.1/src/usda_api/scrapers/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 08:30:22.000000 usda_api-0.1.1/src/usda_api/scrapers/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.340938 usda_api-0.1.1/src/usda_api/scrapers/esr/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      201 2023-05-06 14:35:52.000000 usda_api-0.1.1/src/usda_api/scrapers/esr/__init__.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     6552 2023-05-06 09:43:55.000000 usda_api-0.1.1/src/usda_api/scrapers/esr/main.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.344606 usda_api-0.1.1/src/usda_api/scrapers/esr/schemas/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      470 2023-05-06 09:43:55.000000 usda_api-0.1.1/src/usda_api/scrapers/esr/schemas/__init__.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     2019 2023-05-06 09:36:01.000000 usda_api-0.1.1/src/usda_api/scrapers/esr/schemas/response.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.346161 usda_api-0.1.1/src/usda_api/scrapers/gats/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:42.000000 usda_api-0.1.1/src/usda_api/scrapers/gats/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.346896 usda_api-0.1.1/src/usda_api/scrapers/psd/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:44.000000 usda_api-0.1.1/src/usda_api/scrapers/psd/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.338128 usda_api-0.1.1/src/usda_api.egg-info/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      184 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/PKG-INFO
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      536 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        1 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       55 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/entry_points.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      404 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/requires.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        9 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/top_level.txt
```

### Comparing `usda_api-0.1/setup.py` & `usda_api-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `usda_api-0.1/src/usda_api/scrapers/esr/main.py` & `usda_api-0.1.1/src/usda_api/scrapers/esr/main.py`

 * *Files identical despite different names*

### Comparing `usda_api-0.1/src/usda_api/scrapers/esr/schemas/response.py` & `usda_api-0.1.1/src/usda_api/scrapers/esr/schemas/response.py`

 * *Files identical despite different names*

### Comparing `usda_api-0.1/src/usda_api.egg-info/SOURCES.txt` & `usda_api-0.1.1/src/usda_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

