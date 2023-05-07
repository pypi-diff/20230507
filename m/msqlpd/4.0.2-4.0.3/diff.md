# Comparing `tmp/msqlpd-4.0.2.tar.gz` & `tmp/msqlpd-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msqlpd-4.0.2.tar", last modified: Sun May  7 10:59:50 2023, max compression
+gzip compressed data, was "msqlpd-4.0.3.tar", last modified: Sun May  7 11:20:45 2023, max compression
```

## Comparing `msqlpd-4.0.2.tar` & `msqlpd-4.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 10:59:50.036565 msqlpd-4.0.2/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2023-05-07 10:45:43.000000 msqlpd-4.0.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-07 10:59:50.034992 msqlpd-4.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      107 2023-05-07 10:59:48.000000 msqlpd-4.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 10:59:50.026114 msqlpd-4.0.2/msqlpd/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-05-07 10:45:43.000000 msqlpd-4.0.2/msqlpd/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 10:59:50.032804 msqlpd-4.0.2/msqlpd/src/
--rwxrwxrwx   0 root         (0) root         (0)    13819 2023-05-07 10:45:43.000000 msqlpd-4.0.2/msqlpd/src/connection.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 10:59:50.032068 msqlpd-4.0.2/msqlpd.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      219 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-07 10:59:50.036981 msqlpd-4.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      512 2023-05-07 10:49:24.000000 msqlpd-4.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 11:20:45.656129 msqlpd-4.0.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2023-05-07 10:45:43.000000 msqlpd-4.0.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-07 11:20:45.655703 msqlpd-4.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-05-07 11:20:44.000000 msqlpd-4.0.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 11:20:45.651814 msqlpd-4.0.3/msqlpd/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-05-07 10:45:43.000000 msqlpd-4.0.3/msqlpd/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 11:20:45.655145 msqlpd-4.0.3/msqlpd/src/
+-rwxrwxrwx   0 root         (0) root         (0)    13819 2023-05-07 10:45:43.000000 msqlpd-4.0.3/msqlpd/src/connection.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 11:20:45.654677 msqlpd-4.0.3/msqlpd.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      219 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-07 11:20:45.656432 msqlpd-4.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      530 2023-05-07 11:20:09.000000 msqlpd-4.0.3/setup.py
```

### Comparing `msqlpd-4.0.2/LICENSE` & `msqlpd-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msqlpd-4.0.2/msqlpd/src/connection.py` & `msqlpd-4.0.3/msqlpd/src/connection.py`

 * *Files identical despite different names*

### Comparing `msqlpd-4.0.2/setup.py` & `msqlpd-4.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="msqlpd",
-    version="4.0.2",
+    version="4.0.3",
     author="Moses Dastmard",
     description="return a path information",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'sqlalchemy',
         'pandas',
         'mysql-connector-python',
+        'joblib',
     ]
 )
```

