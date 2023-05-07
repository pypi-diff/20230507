# Comparing `tmp/django_tsp-3.14.5.tar.gz` & `tmp/django_tsp-3.14.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tsp-3.14.5.tar", last modified: Sun May  7 17:55:39 2023, max compression
+gzip compressed data, was "django_tsp-3.14.6.tar", last modified: Sun May  7 18:19:54 2023, max compression
```

## Comparing `django_tsp-3.14.5.tar` & `django_tsp-3.14.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 17:55:39.209621 django_tsp-3.14.5/
--rw-r--r--   0 abb       (1000) abb       (1000)    11813 2023-04-28 13:49:49.000000 django_tsp-3.14.5/CHANGELOG.rst
--rw-r--r--   0 abb       (1000) abb       (1000)     1078 2023-04-19 16:29:15.000000 django_tsp-3.14.5/LICENSE
--rw-r--r--   0 abb       (1000) abb       (1000)       78 2023-04-28 13:50:20.000000 django_tsp-3.14.5/MANIFEST.in
--rw-r--r--   0 abb       (1000) abb       (1000)     1462 2023-05-07 17:55:39.209621 django_tsp-3.14.5/PKG-INFO
--rw-r--r--   0 abb       (1000) abb       (1000)       44 2023-04-19 16:29:15.000000 django_tsp-3.14.5/README.md
--rw-r--r--   0 abb       (1000) abb       (1000)      499 2023-04-28 10:29:09.000000 django_tsp-3.14.5/pyproject.toml
--rw-r--r--   0 abb       (1000) abb       (1000)     1685 2023-05-07 17:55:39.212952 django_tsp-3.14.5/setup.cfg
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 17:55:39.202959 django_tsp-3.14.5/src/
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 17:55:39.206290 django_tsp-3.14.5/src/django_tsp/
--rw-r--r--   0 abb       (1000) abb       (1000)        0 2023-04-09 10:17:38.000000 django_tsp-3.14.5/src/django_tsp/__init__.py
--rw-r--r--   0 abb       (1000) abb       (1000)     1766 2023-05-07 17:51:34.000000 django_tsp-3.14.5/src/django_tsp/apis.py
--rw-r--r--   0 abb       (1000) abb       (1000)      429 2023-04-28 14:31:07.000000 django_tsp-3.14.5/src/django_tsp/apps.py
--rw-r--r--   0 abb       (1000) abb       (1000)     1141 2023-05-07 17:51:34.000000 django_tsp-3.14.5/src/django_tsp/checks.py
--rw-r--r--   0 abb       (1000) abb       (1000)      494 2023-05-07 17:51:34.000000 django_tsp-3.14.5/src/django_tsp/conf.py
--rw-r--r--   0 abb       (1000) abb       (1000)      590 2023-05-07 17:51:34.000000 django_tsp-3.14.5/src/django_tsp/consumer.py
--rw-r--r--   0 abb       (1000) abb       (1000)      132 2023-05-07 17:51:34.000000 django_tsp-3.14.5/src/django_tsp/routing.py
--rw-r--r--   0 abb       (1000) abb       (1000)      212 2023-05-07 17:51:34.000000 django_tsp-3.14.5/src/django_tsp/serializers.py
--rw-r--r--   0 abb       (1000) abb       (1000)      648 2023-05-07 17:51:34.000000 django_tsp-3.14.5/src/django_tsp/services.py
--rw-r--r--   0 abb       (1000) abb       (1000)      102 2023-05-07 17:51:34.000000 django_tsp-3.14.5/src/django_tsp/views.py
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 17:55:39.209621 django_tsp-3.14.5/src/django_tsp.egg-info/
--rw-r--r--   0 abb       (1000) abb       (1000)     1462 2023-05-07 17:55:39.000000 django_tsp-3.14.5/src/django_tsp.egg-info/PKG-INFO
--rw-r--r--   0 abb       (1000) abb       (1000)      549 2023-05-07 17:55:39.000000 django_tsp-3.14.5/src/django_tsp.egg-info/SOURCES.txt
--rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-05-07 17:55:39.000000 django_tsp-3.14.5/src/django_tsp.egg-info/dependency_links.txt
--rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-04-28 13:56:46.000000 django_tsp-3.14.5/src/django_tsp.egg-info/not-zip-safe
--rw-r--r--   0 abb       (1000) abb       (1000)       12 2023-05-07 17:55:39.000000 django_tsp-3.14.5/src/django_tsp.egg-info/requires.txt
--rw-r--r--   0 abb       (1000) abb       (1000)       11 2023-05-07 17:55:39.000000 django_tsp-3.14.5/src/django_tsp.egg-info/top_level.txt
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 18:19:54.309255 django_tsp-3.14.6/
+-rw-r--r--   0 abb       (1000) abb       (1000)    11813 2023-04-28 13:49:49.000000 django_tsp-3.14.6/CHANGELOG.rst
+-rw-r--r--   0 abb       (1000) abb       (1000)     1078 2023-04-19 16:29:15.000000 django_tsp-3.14.6/LICENSE
+-rw-r--r--   0 abb       (1000) abb       (1000)       78 2023-04-28 13:50:20.000000 django_tsp-3.14.6/MANIFEST.in
+-rw-r--r--   0 abb       (1000) abb       (1000)     1462 2023-05-07 18:19:54.309255 django_tsp-3.14.6/PKG-INFO
+-rw-r--r--   0 abb       (1000) abb       (1000)       44 2023-04-19 16:29:15.000000 django_tsp-3.14.6/README.md
+-rw-r--r--   0 abb       (1000) abb       (1000)      499 2023-04-28 10:29:09.000000 django_tsp-3.14.6/pyproject.toml
+-rw-r--r--   0 abb       (1000) abb       (1000)     1705 2023-05-07 18:19:54.309255 django_tsp-3.14.6/setup.cfg
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 18:19:54.305921 django_tsp-3.14.6/src/
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 18:19:54.309255 django_tsp-3.14.6/src/django_tsp/
+-rw-r--r--   0 abb       (1000) abb       (1000)        0 2023-04-09 10:17:38.000000 django_tsp-3.14.6/src/django_tsp/__init__.py
+-rw-r--r--   0 abb       (1000) abb       (1000)     1766 2023-05-07 17:51:34.000000 django_tsp-3.14.6/src/django_tsp/apis.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      429 2023-04-28 14:31:07.000000 django_tsp-3.14.6/src/django_tsp/apps.py
+-rw-r--r--   0 abb       (1000) abb       (1000)     1141 2023-05-07 17:51:34.000000 django_tsp-3.14.6/src/django_tsp/checks.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      448 2023-05-07 18:18:07.000000 django_tsp-3.14.6/src/django_tsp/conf.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      590 2023-05-07 17:51:34.000000 django_tsp-3.14.6/src/django_tsp/consumer.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      132 2023-05-07 17:51:34.000000 django_tsp-3.14.6/src/django_tsp/routing.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      212 2023-05-07 17:51:34.000000 django_tsp-3.14.6/src/django_tsp/serializers.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      648 2023-05-07 17:51:34.000000 django_tsp-3.14.6/src/django_tsp/services.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      102 2023-05-07 17:51:34.000000 django_tsp-3.14.6/src/django_tsp/views.py
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 18:19:54.309255 django_tsp-3.14.6/src/django_tsp.egg-info/
+-rw-r--r--   0 abb       (1000) abb       (1000)     1462 2023-05-07 18:19:54.000000 django_tsp-3.14.6/src/django_tsp.egg-info/PKG-INFO
+-rw-r--r--   0 abb       (1000) abb       (1000)      549 2023-05-07 18:19:54.000000 django_tsp-3.14.6/src/django_tsp.egg-info/SOURCES.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-05-07 18:19:54.000000 django_tsp-3.14.6/src/django_tsp.egg-info/dependency_links.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-04-28 13:56:46.000000 django_tsp-3.14.6/src/django_tsp.egg-info/not-zip-safe
+-rw-r--r--   0 abb       (1000) abb       (1000)       31 2023-05-07 18:19:54.000000 django_tsp-3.14.6/src/django_tsp.egg-info/requires.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)       11 2023-05-07 18:19:54.000000 django_tsp-3.14.6/src/django_tsp.egg-info/top_level.txt
```

### Comparing `django_tsp-3.14.5/CHANGELOG.rst` & `django_tsp-3.14.6/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.5/LICENSE` & `django_tsp-3.14.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.5/PKG-INFO` & `django_tsp-3.14.6/src/django_tsp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_tsp
-Version: 3.14.5
+Name: django-tsp
+Version: 3.14.6
 Summary: django-tsp is a django travel salesman problem.
 Home-page: https://github.com/TravelSalesmanProblem/django_tsp
 Author: AmirBahador Bahadori
 Author-email: amirbahador.pv@gmail.com
 Maintainer: AmirBahador Bahadori
 Maintainer-email: amirbahador.pv@gmail.com
 License: MIT
```

### Comparing `django_tsp-3.14.5/setup.cfg` & `django_tsp-3.14.6/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_tsp
-version = 3.14.5
+version = 3.14.6
 description = django-tsp is a django travel salesman problem.
 long_description = file: README.md
 long_description_content_type = text/x-rst
 url = https://github.com/TravelSalesmanProblem/django_tsp
 author = AmirBahador Bahadori
 author_email = amirbahador.pv@gmail.com
 maintainer = AmirBahador Bahadori
@@ -38,14 +38,15 @@
 project_urls = 
 	Twitter = https://twitter.com/AmirBahadordev
 
 [options]
 packages = find:
 install_requires = 
 	Django>=3.2
+	tsp-wrapper>=1.0.5
 python_requires = >=3.7
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
```

### Comparing `django_tsp-3.14.5/src/django_tsp/apis.py` & `django_tsp-3.14.6/src/django_tsp/apis.py`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.5/src/django_tsp/checks.py` & `django_tsp-3.14.6/src/django_tsp/checks.py`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.5/src/django_tsp/consumer.py` & `django_tsp-3.14.6/src/django_tsp/consumer.py`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.5/src/django_tsp/services.py` & `django_tsp-3.14.6/src/django_tsp/services.py`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.5/src/django_tsp.egg-info/PKG-INFO` & `django_tsp-3.14.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-tsp
-Version: 3.14.5
+Name: django_tsp
+Version: 3.14.6
 Summary: django-tsp is a django travel salesman problem.
 Home-page: https://github.com/TravelSalesmanProblem/django_tsp
 Author: AmirBahador Bahadori
 Author-email: amirbahador.pv@gmail.com
 Maintainer: AmirBahador Bahadori
 Maintainer-email: amirbahador.pv@gmail.com
 License: MIT
```

### Comparing `django_tsp-3.14.5/src/django_tsp.egg-info/SOURCES.txt` & `django_tsp-3.14.6/src/django_tsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

