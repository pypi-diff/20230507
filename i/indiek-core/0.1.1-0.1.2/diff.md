# Comparing `tmp/indiek-core-0.1.1.tar.gz` & `tmp/indiek-core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-or7b6s5q/indiek-core-0.1.1.tar", last modified: Mon Apr 17 01:36:04 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-vppkdjiq/indiek-core-0.1.2.tar", last modified: Sun May  7 13:33:53 2023, max compression
```

## Comparing `indiek-core-0.1.1.tar` & `indiek-core-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.626090 indiek-core-0.1.1/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.1/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1125 2023-04-17 01:36:04.626090 indiek-core-0.1.1/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      759 2023-04-17 01:35:55.000000 indiek-core-0.1.1/README.rst
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.622090 indiek-core-0.1.1/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.626090 indiek-core-0.1.1/indiek/core/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       13 2023-04-15 23:00:43.000000 indiek-core-0.1.1/indiek/core/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      420 2023-04-17 00:48:04.000000 indiek-core-0.1.1/indiek/core/items.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.626090 indiek-core-0.1.1/indiek_core.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1125 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      276 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       58 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-04-17 01:36:04.626090 indiek-core-0.1.1/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      840 2023-04-17 01:24:55.000000 indiek-core-0.1.1/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.626090 indiek-core-0.1.1/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      689 2023-04-16 01:50:53.000000 indiek-core-0.1.1/tests/test_items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.157884 indiek-core-0.1.2/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.2/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1210 2023-05-07 13:33:53.157884 indiek-core-0.1.2/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      759 2023-04-23 17:12:42.000000 indiek-core-0.1.2/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.141884 indiek-core-0.1.2/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.157884 indiek-core-0.1.2/indiek/core/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       13 2023-04-23 17:12:42.000000 indiek-core-0.1.2/indiek/core/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     2791 2023-05-07 13:27:55.000000 indiek-core-0.1.2/indiek/core/items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      280 2023-05-07 13:27:55.000000 indiek-core-0.1.2/indiek/core/search.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.157884 indiek-core-0.1.2/indiek_core.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1210 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      319 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       58 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-07 13:33:53.157884 indiek-core-0.1.2/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      924 2023-05-07 13:27:55.000000 indiek-core-0.1.2/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.157884 indiek-core-0.1.2/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1172 2023-05-07 13:27:55.000000 indiek-core-0.1.2/tests/test_items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      416 2023-05-07 13:27:55.000000 indiek-core-0.1.2/tests/test_search.py
```

### Comparing `indiek-core-0.1.1/LICENSE` & `indiek-core-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-core-0.1.1/PKG-INFO` & `indiek-core-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: indiek-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: core logic for indiek
 Home-page: https://pypi.org/project/indiek-core/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
-Project-URL: GitHub, https://github.com/indiek
+Project-URL: GitHub, https://github.com/indiek/indiek.core
+Project-URL: Documentation, https://indiekcore.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 Library that stores the core logic for the IndieK software suite.
 
 ============
```

### Comparing `indiek-core-0.1.1/README.rst` & `indiek-core-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `indiek-core-0.1.1/indiek_core.egg-info/PKG-INFO` & `indiek-core-0.1.2/indiek_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: indiek-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: core logic for indiek
 Home-page: https://pypi.org/project/indiek-core/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
-Project-URL: GitHub, https://github.com/indiek
+Project-URL: GitHub, https://github.com/indiek/indiek.core
+Project-URL: Documentation, https://indiekcore.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 Library that stores the core logic for the IndieK software suite.
 
 ============
```

### Comparing `indiek-core-0.1.1/setup.py` & `indiek-core-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.rst'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='indiek-core',
     python_requires='>=3.8',
-    version='0.1.1',
+    version='0.1.2',
     url='https://pypi.org/project/indiek-core/',
     description='core logic for indiek',
     long_description=long_description,
     author='Adrian Ernesto Radillo',
     author_email='adrian.radillo@gmail.com',
     license='GNU Affero General Public License v3.0',
     packages=['indiek.core'],
-    install_requires=['indiek-mockdb==0.1.1'],
+    install_requires=['indiek-mockdb==0.1.2'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov'
         ]
     },
     project_urls={
-        'GitHub': 'https://github.com/indiek',
+        'GitHub': 'https://github.com/indiek/indiek.core',
+        'Documentation': 'https://indiekcore.readthedocs.io/en/latest/'
     },
 )
```

