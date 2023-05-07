# Comparing `tmp/automation-common-test-1.2.0.tar.gz` & `tmp/automation-common-test-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-common-test-1.2.0.tar", last modified: Sun May  7 06:25:08 2023, max compression
+gzip compressed data, was "automation-common-test-1.3.0.tar", last modified: Sun May  7 06:33:41 2023, max compression
```

## Comparing `automation-common-test-1.2.0.tar` & `automation-common-test-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-07 06:25:08.480666 automation-common-test-1.2.0/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-07 06:25:08.480459 automation-common-test-1.2.0/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-1.2.0/README.md
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-07 06:25:08.478603 automation-common-test-1.2.0/automation_common_test.egg-info/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-07 06:25:08.000000 automation-common-test-1.2.0/automation_common_test.egg-info/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      420 2023-05-07 06:25:08.000000 automation-common-test-1.2.0/automation_common_test.egg-info/SOURCES.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-05-07 06:25:08.000000 automation-common-test-1.2.0/automation_common_test.egg-info/dependency_links.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-05-07 06:25:08.000000 automation-common-test-1.2.0/automation_common_test.egg-info/top_level.txt
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-07 06:25:08.479457 automation-common-test-1.2.0/helpers/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-1.2.0/helpers/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-1.2.0/helpers/base_locator.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     5694 2023-04-27 06:23:19.000000 automation-common-test-1.2.0/helpers/driver_manager.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-1.2.0/helpers/soft_check.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)    66006 2023-04-27 06:59:19.000000 automation-common-test-1.2.0/helpers/web_operations.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-05-07 06:25:08.480714 automation-common-test-1.2.0/setup.cfg
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-05-07 06:23:34.000000 automation-common-test-1.2.0/setup.py
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-07 06:25:08.480215 automation-common-test-1.2.0/utils/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-1.2.0/utils/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-1.2.0/utils/config_parser.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-1.2.0/utils/encryption_decryption.py
--rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4591 2023-05-07 05:57:59.000000 automation-common-test-1.2.0/utils/post_results_teams.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-07 06:33:41.108408 automation-common-test-1.3.0/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-07 06:33:41.108204 automation-common-test-1.3.0/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-1.3.0/README.md
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-07 06:33:41.105073 automation-common-test-1.3.0/automation_common_test.egg-info/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-07 06:33:41.000000 automation-common-test-1.3.0/automation_common_test.egg-info/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      420 2023-05-07 06:33:41.000000 automation-common-test-1.3.0/automation_common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-05-07 06:33:41.000000 automation-common-test-1.3.0/automation_common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-05-07 06:33:41.000000 automation-common-test-1.3.0/automation_common_test.egg-info/top_level.txt
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-07 06:33:41.106681 automation-common-test-1.3.0/helpers/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-1.3.0/helpers/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-1.3.0/helpers/base_locator.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     5694 2023-04-27 06:23:19.000000 automation-common-test-1.3.0/helpers/driver_manager.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-1.3.0/helpers/soft_check.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)    66006 2023-04-27 06:59:19.000000 automation-common-test-1.3.0/helpers/web_operations.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-05-07 06:33:41.108457 automation-common-test-1.3.0/setup.cfg
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-05-07 06:33:21.000000 automation-common-test-1.3.0/setup.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-07 06:33:41.107814 automation-common-test-1.3.0/utils/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-1.3.0/utils/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-1.3.0/utils/config_parser.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-1.3.0/utils/encryption_decryption.py
+-rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4591 2023-05-07 05:57:59.000000 automation-common-test-1.3.0/utils/post_results_teams.py
```

### Comparing `automation-common-test-1.2.0/README.md` & `automation-common-test-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.2.0/helpers/driver_manager.py` & `automation-common-test-1.3.0/helpers/driver_manager.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.2.0/helpers/soft_check.py` & `automation-common-test-1.3.0/helpers/soft_check.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.2.0/helpers/web_operations.py` & `automation-common-test-1.3.0/helpers/web_operations.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.2.0/utils/encryption_decryption.py` & `automation-common-test-1.3.0/utils/encryption_decryption.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.2.0/utils/post_results_teams.py` & `automation-common-test-1.3.0/utils/post_results_teams.py`

 * *Files identical despite different names*

