# Comparing `tmp/indiek-mockdb-0.1.1.tar.gz` & `tmp/indiek-mockdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-mockdb/dist/.tmp-tj_6ca4n/indiek-mockdb-0.1.1.tar", last modified: Mon Apr 17 01:22:01 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-mockdb/dist/.tmp-nnicdprj/indiek-mockdb-0.1.2.tar", last modified: Sun May  7 13:31:15 2023, max compression
```

## Comparing `indiek-mockdb-0.1.1.tar` & `indiek-mockdb-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:22:01.423993 indiek-mockdb-0.1.1/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-16 01:06:17.000000 indiek-mockdb-0.1.1/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-04-17 01:22:01.423993 indiek-mockdb-0.1.1/PKG-INFO
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:22:01.399993 indiek-mockdb-0.1.1/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:22:01.419993 indiek-mockdb-0.1.1/indiek/mockdb/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-04-16 01:07:43.000000 indiek-mockdb-0.1.1/indiek/mockdb/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      719 2023-04-17 00:57:30.000000 indiek-mockdb-0.1.1/indiek/mockdb/items.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:22:01.423993 indiek-mockdb-0.1.1/indiek_mockdb.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-04-17 01:22:01.000000 indiek-mockdb-0.1.1/indiek_mockdb.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      279 2023-04-17 01:22:01.000000 indiek-mockdb-0.1.1/indiek_mockdb.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-04-17 01:22:01.000000 indiek-mockdb-0.1.1/indiek_mockdb.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       37 2023-04-17 01:22:01.000000 indiek-mockdb-0.1.1/indiek_mockdb.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-04-17 01:22:01.000000 indiek-mockdb-0.1.1/indiek_mockdb.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-04-17 01:22:01.423993 indiek-mockdb-0.1.1/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      618 2023-04-17 01:01:29.000000 indiek-mockdb-0.1.1/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:22:01.423993 indiek-mockdb-0.1.1/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      372 2023-04-16 01:15:46.000000 indiek-mockdb-0.1.1/tests/test_items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-16 01:06:17.000000 indiek-mockdb-0.1.2/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/PKG-INFO
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.081183 indiek-mockdb-0.1.2/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/indiek/mockdb/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-04-16 01:07:43.000000 indiek-mockdb-0.1.2/indiek/mockdb/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3460 2023-05-06 13:46:41.000000 indiek-mockdb-0.1.2/indiek/mockdb/items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      279 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       37 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      618 2023-05-05 21:52:52.000000 indiek-mockdb-0.1.2/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1292 2023-05-06 13:44:24.000000 indiek-mockdb-0.1.2/tests/test_items.py
```

### Comparing `indiek-mockdb-0.1.1/LICENSE` & `indiek-mockdb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-mockdb-0.1.1/setup.py` & `indiek-mockdb-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(name='indiek-mockdb',
       python_requires='>=3.8',
-      version='0.1.1',
+      version='0.1.2',
       description='mock database for indiek',
       long_description='''This is an on-the-fly in-memory mock Database used by indiek-core
       for development and testing purposes. The versioning of this library is locked with that
       of indiek-core.''',
       author='Adrian Ernesto Radillo',
       author_email='adrian.radillo@gmail.com',
       license='GNU Affero General Public License v3.0',
```

