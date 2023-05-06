# Comparing `tmp/liccheck-0.9.0.tar.gz` & `tmp/liccheck-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liccheck-0.9.0.tar", last modified: Fri Apr 28 14:38:48 2023, max compression
+gzip compressed data, was "liccheck-0.9.1.tar", last modified: Sat May  6 22:05:15 2023, max compression
```

## Comparing `liccheck-0.9.0.tar` & `liccheck-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:38:48.173187 liccheck-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 14:38:46.000000 liccheck-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-28 14:38:48.173187 liccheck-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-04-28 14:38:46.000000 liccheck-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:38:48.173187 liccheck-0.9.0/liccheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:38:46.000000 liccheck-0.9.0/liccheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 14:38:46.000000 liccheck-0.9.0/liccheck/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-04-28 14:38:46.000000 liccheck-0.9.0/liccheck/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-28 14:38:46.000000 liccheck-0.9.0/liccheck/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:38:48.173187 liccheck-0.9.0/liccheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 14:38:48.173187 liccheck-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-28 14:38:46.000000 liccheck-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:05:15.076247 liccheck-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 22:05:12.000000 liccheck-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-06 22:05:15.076247 liccheck-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-06 22:05:12.000000 liccheck-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:05:15.076247 liccheck-0.9.1/liccheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 22:05:12.000000 liccheck-0.9.1/liccheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-06 22:05:12.000000 liccheck-0.9.1/liccheck/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-05-06 22:05:12.000000 liccheck-0.9.1/liccheck/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-06 22:05:12.000000 liccheck-0.9.1/liccheck/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:05:15.076247 liccheck-0.9.1/liccheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-06 22:05:15.000000 liccheck-0.9.1/liccheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-06 22:05:15.000000 liccheck-0.9.1/liccheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:05:15.000000 liccheck-0.9.1/liccheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 22:05:15.000000 liccheck-0.9.1/liccheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-06 22:05:15.000000 liccheck-0.9.1/liccheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 22:05:15.000000 liccheck-0.9.1/liccheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-06 22:05:15.076247 liccheck-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-06 22:05:12.000000 liccheck-0.9.1/setup.py
```

### Comparing `liccheck-0.9.0/LICENSE` & `liccheck-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liccheck-0.9.0/PKG-INFO` & `liccheck-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liccheck
-Version: 0.9.0
+Version: 0.9.1
 Summary: Check python packages from requirement.txt and report issues
 Home-page: https://github.com/dhatim/python-license-check
 Author: Dhatim
 Author-email: contact@dhatim.com
 License: Apache Software License
 Keywords: license check build tool
 Platform: UNKNOWN
```

### Comparing `liccheck-0.9.0/README.rst` & `liccheck-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `liccheck-0.9.0/liccheck/command_line.py` & `liccheck-0.9.1/liccheck/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,50 +219,57 @@
             return license_regex.search(license_str) is not None
         else:
             license_list = getattr(strategy, "{}_LICENSES".format(license_rule))
             return license_str in license_list
 
     at_least_one_unauthorized = False
     count_authorized = 0
-    for license in pkg["licenses"]:
-        lower = license.lower()
+    licenses = get_license_names(pkg["licenses"])
+    for license in licenses:
         if check_one(
-            lower,
+            license,
             license_rule="UNAUTHORIZED",
             as_regex=as_regex,
         ):
             at_least_one_unauthorized = True
         if check_one(
-            lower,
+            license,
             license_rule="AUTHORIZED",
             as_regex=as_regex,
         ):
             count_authorized += 1
 
     if (
         (count_authorized and level is Level.STANDARD)
         or (
             count_authorized
             and not at_least_one_unauthorized
             and level is Level.CAUTIOUS
         )
         or (
             count_authorized
-            and count_authorized == len(pkg["licenses"])
+            and count_authorized == len(licenses)
             and level is Level.PARANOID
         )
     ):
         return Reason.OK
 
     # if not OK and at least one unauthorized
     if at_least_one_unauthorized:
         return Reason.UNAUTHORIZED
 
     return Reason.UNKNOWN
 
+def get_license_names(licenses):
+    names = []
+    for license in licenses:
+        options = license.split(" OR ")
+        for option in options:
+            names.append(option.lower())
+    return names
 
 def find_parents(package, all, seen):
     if package in seen:
         return [package]
     seen.add(package)
     parents = [p["name"] for p in all if package in p["dependencies"]]
     if len(parents) == 0:
```

### Comparing `liccheck-0.9.0/liccheck/requirements.py` & `liccheck-0.9.1/liccheck/requirements.py`

 * *Files identical despite different names*

### Comparing `liccheck-0.9.0/liccheck.egg-info/PKG-INFO` & `liccheck-0.9.1/liccheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liccheck
-Version: 0.9.0
+Version: 0.9.1
 Summary: Check python packages from requirement.txt and report issues
 Home-page: https://github.com/dhatim/python-license-check
 Author: Dhatim
 Author-email: contact@dhatim.com
 License: Apache Software License
 Keywords: license check build tool
 Platform: UNKNOWN
```

### Comparing `liccheck-0.9.0/setup.py` & `liccheck-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name='liccheck',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.9.0',
+    version='0.9.1',
 
     description='Check python packages from requirement.txt and report issues',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/dhatim/python-license-check',
```

