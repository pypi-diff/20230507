# Comparing `tmp/nexus-utilities-0.1.7.tar.gz` & `tmp/nexus-utilities-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.1.7.tar", last modified: Tue May  2 15:41:01 2023, max compression
+gzip compressed data, was "nexus-utilities-0.1.8.tar", last modified: Tue May  2 15:49:36 2023, max compression
```

## Comparing `nexus-utilities-0.1.7.tar` & `nexus-utilities-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/src/package_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 15:49:16.000000 nexus-utilities-0.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-02 15:49:16.000000 nexus-utilities-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:49:35.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-02 15:49:36.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:49:35.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 15:49:35.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 15:49:35.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-02 15:49:16.000000 nexus-utilities-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:49:16.000000 nexus-utilities-0.1.8/src/__init__.py
```

### Comparing `nexus-utilities-0.1.7/LICENSE.txt` & `nexus-utilities-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.1.7/PKG-INFO` & `nexus-utilities-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.7
+Version: 0.1.8
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.1.7/README.md` & `nexus-utilities-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 Arguments:
  * None
 
 Programmatically determines the most likely root folder of the current running program, adds the parent folder to the system PATH, and returns the root folder name.  This can be helpful for resolving package-relative paths, particularly for programs with multiple possible entry points.  It achieves this by starting from the current working directory, and traversing upwards, counting the instances of the below files and folders:
 
 ```python
-["src", "tests", "templates", "docs", "readme.md", "license.txt", ".gitignore", "pyproject.toml", "requirements.txt", "poetry.lock", "setup.py", "manifest.in", ".editorconfig"]
+["src", "tests", "templates", "docs", "dist", "build", "readme.md", "license.txt", ".gitignore", "pyproject.toml", "requirements.txt", "poetry.lock", "setup.py", "manifest.in", ".editorconfig"]
 ```
 
 In the case of a tie, it takes the folder deeper into the path.  The returned "package_root_name" is meant to be used with the "import_relative()" function below.
 
 ### **import_relative(package_root_name, module_path, import_name, alias=None)**
 
 Example:
```

### Comparing `nexus-utilities-0.1.7/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.1.8/nexus_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.7
+Version: 0.1.8
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.1.7/setup.py` & `nexus-utilities-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.1.7',
+    version='0.1.8',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=find_packages(),
```

