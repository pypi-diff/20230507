# Comparing `tmp/silobuster-0.1.4.tar.gz` & `tmp/silobuster-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silobuster-0.1.4.tar", last modified: Sun May  7 04:41:42 2023, max compression
+gzip compressed data, was "silobuster-0.1.5.tar", last modified: Sun May  7 04:51:54 2023, max compression
```

## Comparing `silobuster-0.1.4.tar` & `silobuster-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:41:42.666149 silobuster-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:41:42.666149 silobuster-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 04:41:35.000000 silobuster-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:41:42.666149 silobuster-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 04:41:37.000000 silobuster-0.1.4/setup_pypi_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:41:42.666149 silobuster-0.1.4/silobuster/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-07 04:41:37.000000 silobuster-0.1.4/silobuster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:41:42.666149 silobuster-0.1.4/silobuster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:41:42.000000 silobuster-0.1.4/silobuster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 04:41:42.000000 silobuster-0.1.4/silobuster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:41:42.000000 silobuster-0.1.4/silobuster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 04:41:42.000000 silobuster-0.1.4/silobuster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 04:41:42.000000 silobuster-0.1.4/silobuster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:51:54.481650 silobuster-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:51:54.481650 silobuster-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 04:51:47.000000 silobuster-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:51:54.481650 silobuster-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 04:51:49.000000 silobuster-0.1.5/setup_pypi_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:51:54.481650 silobuster-0.1.5/silobuster/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-07 04:51:49.000000 silobuster-0.1.5/silobuster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:51:54.481650 silobuster-0.1.5/silobuster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/top_level.txt
```

### Comparing `silobuster-0.1.4/README.md` & `silobuster-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `silobuster-0.1.4/silobuster/__init__.py` & `silobuster-0.1.5/silobuster/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import os
+# import os
 
-# Retrieve the package directory
-package_dir = os.path.dirname(__file__)
+# # Retrieve the package directory
+# package_dir = os.path.dirname(__file__)
 
-# Get a list of subfolders within the package directory
-subfolders = [f for f in os.listdir(package_dir) if os.path.isdir(os.path.join(package_dir, f))]
+# # Get a list of subfolders within the package directory
+# subfolders = [f for f in os.listdir(package_dir) if os.path.isdir(os.path.join(package_dir, f))]
 
-# Loop through the subfolders and dynamically import the modules
-for subfolder in subfolders:
-    try:
-        module_name = subfolder
-        module = __import__(f"{__name__}.{module_name}", fromlist=["*"])
-        globals().update(vars(module))
-    except ImportError:
-        pass
+# # Loop through the subfolders and dynamically import the modules
+# for subfolder in subfolders:
+#     try:
+#         module_name = subfolder
+#         module = __import__(f"{__name__}.{module_name}", fromlist=["*"])
+#         globals().update(vars(module))
+#     except ImportError:
+#         pass
```

