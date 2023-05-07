# Comparing `tmp/cloud-files-4.9.0.tar.gz` & `tmp/cloud-files-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-files-4.9.0.tar", last modified: Fri Jul 15 02:44:23 2022, max compression
+gzip compressed data, was "cloud-files-4.9.1.tar", last modified: Sat Jul 16 05:39:39 2022, max compression
```

## Comparing `cloud-files-4.9.0.tar` & `cloud-files-4.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-15 02:44:23.066968 cloud-files-4.9.0/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-15 02:44:23.058512 cloud-files-4.9.0/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-15 02:44:23.060562 cloud-files-4.9.0/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      907 2022-07-15 02:34:59.000000 cloud-files-4.9.0/.github/workflows/test-suite.yml
--rw-r--r--   0 wms        (501) staff       (20)      129 2022-07-15 02:44:22.000000 cloud-files-4.9.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)    11950 2022-07-15 02:44:22.000000 cloud-files-4.9.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)     1538 2021-01-11 02:44:41.000000 cloud-files-4.9.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       46 2021-01-11 02:44:41.000000 cloud-files-4.9.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)    21881 2022-07-15 02:44:23.067099 cloud-files-4.9.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)    20989 2022-07-15 02:22:29.000000 cloud-files-4.9.0/README.md
--rw-r--r--   0 wms        (501) staff       (20)    32124 2022-07-15 02:29:19.000000 cloud-files-4.9.0/automated_test.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-15 02:44:23.062451 cloud-files-4.9.0/cloud_files.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    21881 2022-07-15 02:44:22.000000 cloud-files-4.9.0/cloud_files.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      781 2022-07-15 02:44:23.000000 cloud-files-4.9.0/cloud_files.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2022-07-15 02:44:22.000000 cloud-files-4.9.0/cloud_files.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       52 2022-07-15 02:44:22.000000 cloud-files-4.9.0/cloud_files.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-02-03 23:20:54.000000 cloud-files-4.9.0/cloud_files.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2022-07-15 02:44:22.000000 cloud-files-4.9.0/cloud_files.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)      326 2022-07-15 02:44:22.000000 cloud-files-4.9.0/cloud_files.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       26 2022-07-15 02:44:22.000000 cloud-files-4.9.0/cloud_files.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-15 02:44:23.065894 cloud-files-4.9.0/cloudfiles/
--rw-r--r--   0 wms        (501) staff       (20)      404 2022-04-14 01:16:15.000000 cloud-files-4.9.0/cloudfiles/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    31966 2022-06-23 02:11:54.000000 cloud-files-4.9.0/cloudfiles/cloudfiles.py
--rw-r--r--   0 wms        (501) staff       (20)     6150 2022-07-15 02:25:43.000000 cloud-files-4.9.0/cloudfiles/compression.py
--rw-r--r--   0 wms        (501) staff       (20)     4324 2021-12-01 19:53:50.000000 cloud-files-4.9.0/cloudfiles/connectionpools.py
--rw-r--r--   0 wms        (501) staff       (20)      770 2021-10-19 20:26:54.000000 cloud-files-4.9.0/cloudfiles/exceptions.py
--rw-r--r--   0 wms        (501) staff       (20)    28843 2022-07-15 02:21:47.000000 cloud-files-4.9.0/cloudfiles/interfaces.py
--rw-r--r--   0 wms        (501) staff       (20)     4994 2022-07-11 21:18:53.000000 cloud-files-4.9.0/cloudfiles/lib.py
--rw-r--r--   0 wms        (501) staff       (20)     9168 2022-04-14 03:30:00.000000 cloud-files-4.9.0/cloudfiles/paths.py
--rw-r--r--   0 wms        (501) staff       (20)     3412 2021-11-02 18:37:29.000000 cloud-files-4.9.0/cloudfiles/scheduler.py
--rw-r--r--   0 wms        (501) staff       (20)     4121 2021-12-01 19:55:19.000000 cloud-files-4.9.0/cloudfiles/secrets.py
--rw-r--r--   0 wms        (501) staff       (20)     7082 2021-10-19 20:33:35.000000 cloud-files-4.9.0/cloudfiles/threaded_queue.py
--rw-r--r--   0 wms        (501) staff       (20)      388 2021-11-02 18:35:49.000000 cloud-files-4.9.0/cloudfiles/typing.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-15 02:44:23.066621 cloud-files-4.9.0/cloudfiles_cli/
--rw-r--r--   0 wms        (501) staff       (20)     1538 2021-01-11 02:44:41.000000 cloud-files-4.9.0/cloudfiles_cli/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       89 2021-10-19 20:33:35.000000 cloud-files-4.9.0/cloudfiles_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    23350 2022-06-23 02:23:53.000000 cloud-files-4.9.0/cloudfiles_cli/cloudfiles_cli.py
--rw-r--r--   0 wms        (501) staff       (20)      291 2021-08-16 19:38:56.000000 cloud-files-4.9.0/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)      921 2022-07-15 02:44:23.067605 cloud-files-4.9.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      262 2021-10-19 20:33:35.000000 cloud-files-4.9.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-16 05:39:39.245259 cloud-files-4.9.1/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-16 05:39:39.237200 cloud-files-4.9.1/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-16 05:39:39.239498 cloud-files-4.9.1/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      907 2022-07-15 02:34:59.000000 cloud-files-4.9.1/.github/workflows/test-suite.yml
+-rw-r--r--   0 wms        (501) staff       (20)      129 2022-07-16 05:39:39.000000 cloud-files-4.9.1/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)    11998 2022-07-16 05:39:39.000000 cloud-files-4.9.1/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)     1538 2021-01-11 02:44:41.000000 cloud-files-4.9.1/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       46 2021-01-11 02:44:41.000000 cloud-files-4.9.1/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)    21881 2022-07-16 05:39:39.245401 cloud-files-4.9.1/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)    20989 2022-07-15 02:22:29.000000 cloud-files-4.9.1/README.md
+-rw-r--r--   0 wms        (501) staff       (20)    32124 2022-07-15 02:29:19.000000 cloud-files-4.9.1/automated_test.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-16 05:39:39.240773 cloud-files-4.9.1/cloud_files.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)    21881 2022-07-16 05:39:39.000000 cloud-files-4.9.1/cloud_files.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      781 2022-07-16 05:39:39.000000 cloud-files-4.9.1/cloud_files.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2022-07-16 05:39:39.000000 cloud-files-4.9.1/cloud_files.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       52 2022-07-16 05:39:39.000000 cloud-files-4.9.1/cloud_files.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-02-03 23:20:54.000000 cloud-files-4.9.1/cloud_files.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2022-07-16 05:39:39.000000 cloud-files-4.9.1/cloud_files.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)      326 2022-07-16 05:39:39.000000 cloud-files-4.9.1/cloud_files.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       26 2022-07-16 05:39:39.000000 cloud-files-4.9.1/cloud_files.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-16 05:39:39.244084 cloud-files-4.9.1/cloudfiles/
+-rw-r--r--   0 wms        (501) staff       (20)      404 2022-04-14 01:16:15.000000 cloud-files-4.9.1/cloudfiles/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    31966 2022-06-23 02:11:54.000000 cloud-files-4.9.1/cloudfiles/cloudfiles.py
+-rw-r--r--   0 wms        (501) staff       (20)     6150 2022-07-15 02:25:43.000000 cloud-files-4.9.1/cloudfiles/compression.py
+-rw-r--r--   0 wms        (501) staff       (20)     4324 2021-12-01 19:53:50.000000 cloud-files-4.9.1/cloudfiles/connectionpools.py
+-rw-r--r--   0 wms        (501) staff       (20)      770 2021-10-19 20:26:54.000000 cloud-files-4.9.1/cloudfiles/exceptions.py
+-rw-r--r--   0 wms        (501) staff       (20)    28843 2022-07-15 02:21:47.000000 cloud-files-4.9.1/cloudfiles/interfaces.py
+-rw-r--r--   0 wms        (501) staff       (20)     4994 2022-07-11 21:18:53.000000 cloud-files-4.9.1/cloudfiles/lib.py
+-rw-r--r--   0 wms        (501) staff       (20)     9174 2022-07-16 05:38:42.000000 cloud-files-4.9.1/cloudfiles/paths.py
+-rw-r--r--   0 wms        (501) staff       (20)     3412 2021-11-02 18:37:29.000000 cloud-files-4.9.1/cloudfiles/scheduler.py
+-rw-r--r--   0 wms        (501) staff       (20)     4121 2021-12-01 19:55:19.000000 cloud-files-4.9.1/cloudfiles/secrets.py
+-rw-r--r--   0 wms        (501) staff       (20)     7082 2021-10-19 20:33:35.000000 cloud-files-4.9.1/cloudfiles/threaded_queue.py
+-rw-r--r--   0 wms        (501) staff       (20)      388 2021-11-02 18:35:49.000000 cloud-files-4.9.1/cloudfiles/typing.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-07-16 05:39:39.244887 cloud-files-4.9.1/cloudfiles_cli/
+-rw-r--r--   0 wms        (501) staff       (20)     1538 2021-01-11 02:44:41.000000 cloud-files-4.9.1/cloudfiles_cli/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       89 2021-10-19 20:33:35.000000 cloud-files-4.9.1/cloudfiles_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    23350 2022-06-23 02:23:53.000000 cloud-files-4.9.1/cloudfiles_cli/cloudfiles_cli.py
+-rw-r--r--   0 wms        (501) staff       (20)      291 2021-08-16 19:38:56.000000 cloud-files-4.9.1/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)      921 2022-07-16 05:39:39.245937 cloud-files-4.9.1/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      262 2021-10-19 20:33:35.000000 cloud-files-4.9.1/setup.py
```

### Comparing `cloud-files-4.9.0/.github/workflows/test-suite.yml` & `cloud-files-4.9.1/.github/workflows/test-suite.yml`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/ChangeLog` & `cloud-files-4.9.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+4.9.1
+-----
+
+* feat: support n5 format parsing
+
 4.9.0
 -----
 
 * fixtest: python3.10 must be quoted
 * test: add python3.10 to CI
 * chore: update changelog
 * docs: state that bz2 and xz are supported
```

### Comparing `cloud-files-4.9.0/LICENSE` & `cloud-files-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/PKG-INFO` & `cloud-files-4.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-files
-Version: 4.9.0
+Version: 4.9.1
 Summary: Fast access to cloud storage and local FS.
 Home-page: https://github.com/seung-lab/cloud-files/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: BSD License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cloud-files-4.9.0/README.md` & `cloud-files-4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/automated_test.py` & `cloud-files-4.9.1/automated_test.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloud_files.egg-info/PKG-INFO` & `cloud-files-4.9.1/cloud_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-files
-Version: 4.9.0
+Version: 4.9.1
 Summary: Fast access to cloud storage and local FS.
 Home-page: https://github.com/seung-lab/cloud-files/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: BSD License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cloud-files-4.9.0/cloud_files.egg-info/SOURCES.txt` & `cloud-files-4.9.1/cloud_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/cloudfiles.py` & `cloud-files-4.9.1/cloudfiles/cloudfiles.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/compression.py` & `cloud-files-4.9.1/cloudfiles/compression.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/connectionpools.py` & `cloud-files-4.9.1/cloudfiles/connectionpools.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/exceptions.py` & `cloud-files-4.9.1/cloudfiles/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/interfaces.py` & `cloud-files-4.9.1/cloudfiles/interfaces.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/lib.py` & `cloud-files-4.9.1/cloudfiles/lib.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/paths.py` & `cloud-files-4.9.1/cloudfiles/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ALIASES_FROM_FILE = None
 ALIASES = {}
 BASE_ALLOWED_PROTOCOLS = [ 
   'gs', 'file', 's3', 
   'http', 'https', 'mem' 
 ]
 ALLOWED_PROTOCOLS = list(BASE_ALLOWED_PROTOCOLS)
-ALLOWED_FORMATS = [ 'graphene', 'precomputed', 'boss' ] 
+ALLOWED_FORMATS = [ 'graphene', 'precomputed', 'boss', 'n5' ] 
 
 def update_aliases_from_file():
   global ALIASES_FROM_FILE
   global ALIAS_FILE
   if ALIASES_FROM_FILE is not None:
     return
```

### Comparing `cloud-files-4.9.0/cloudfiles/scheduler.py` & `cloud-files-4.9.1/cloudfiles/scheduler.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/secrets.py` & `cloud-files-4.9.1/cloudfiles/secrets.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles/threaded_queue.py` & `cloud-files-4.9.1/cloudfiles/threaded_queue.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles_cli/LICENSE` & `cloud-files-4.9.1/cloudfiles_cli/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/cloudfiles_cli/cloudfiles_cli.py` & `cloud-files-4.9.1/cloudfiles_cli/cloudfiles_cli.py`

 * *Files identical despite different names*

### Comparing `cloud-files-4.9.0/setup.cfg` & `cloud-files-4.9.1/setup.cfg`

 * *Files identical despite different names*

