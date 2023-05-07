# Comparing `tmp/wheeldiff-2023.5.7.tar.gz` & `tmp/wheeldiff-2023.5.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheeldiff-2023.5.7.tar", last modified: Sun May  7 04:38:59 2023, max compression
+gzip compressed data, was "wheeldiff-2023.5.7.5.tar", last modified: Sun May  7 05:12:53 2023, max compression
```

## Comparing `wheeldiff-2023.5.7.tar` & `wheeldiff-2023.5.7.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:38:59.916308 wheeldiff-2023.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 04:38:45.000000 wheeldiff-2023.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 04:38:45.000000 wheeldiff-2023.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46105 2023-05-07 04:38:59.916308 wheeldiff-2023.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-07 04:38:45.000000 wheeldiff-2023.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 04:38:45.000000 wheeldiff-2023.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 04:38:45.000000 wheeldiff-2023.5.7/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:38:59.916308 wheeldiff-2023.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:38:59.912308 wheeldiff-2023.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:38:59.912308 wheeldiff-2023.5.7/src/wheeldiff/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-07 04:38:59.000000 wheeldiff-2023.5.7/src/wheeldiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:38:59.912308 wheeldiff-2023.5.7/src/wheeldiff/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 04:38:45.000000 wheeldiff-2023.5.7/src/wheeldiff/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-07 04:38:45.000000 wheeldiff-2023.5.7/src/wheeldiff/_impl/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:38:59.912308 wheeldiff-2023.5.7/src/wheeldiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46105 2023-05-07 04:38:59.000000 wheeldiff-2023.5.7/src/wheeldiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 04:38:59.000000 wheeldiff-2023.5.7/src/wheeldiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:38:59.000000 wheeldiff-2023.5.7/src/wheeldiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 04:38:59.000000 wheeldiff-2023.5.7/src/wheeldiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 04:38:59.000000 wheeldiff-2023.5.7/src/wheeldiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 04:38:59.000000 wheeldiff-2023.5.7/src/wheeldiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:38:59.912308 wheeldiff-2023.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 04:38:45.000000 wheeldiff-2023.5.7/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:12:53.309315 wheeldiff-2023.5.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 05:12:41.000000 wheeldiff-2023.5.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 05:12:41.000000 wheeldiff-2023.5.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46107 2023-05-07 05:12:53.309315 wheeldiff-2023.5.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-07 05:12:41.000000 wheeldiff-2023.5.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 05:12:41.000000 wheeldiff-2023.5.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 05:12:41.000000 wheeldiff-2023.5.7.5/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:12:53.309315 wheeldiff-2023.5.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:12:53.305315 wheeldiff-2023.5.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:12:53.309315 wheeldiff-2023.5.7.5/src/wheeldiff/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 05:12:53.000000 wheeldiff-2023.5.7.5/src/wheeldiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:12:53.309315 wheeldiff-2023.5.7.5/src/wheeldiff/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 05:12:41.000000 wheeldiff-2023.5.7.5/src/wheeldiff/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-07 05:12:41.000000 wheeldiff-2023.5.7.5/src/wheeldiff/_impl/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:12:53.309315 wheeldiff-2023.5.7.5/src/wheeldiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46107 2023-05-07 05:12:53.000000 wheeldiff-2023.5.7.5/src/wheeldiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 05:12:53.000000 wheeldiff-2023.5.7.5/src/wheeldiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:12:53.000000 wheeldiff-2023.5.7.5/src/wheeldiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 05:12:53.000000 wheeldiff-2023.5.7.5/src/wheeldiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 05:12:53.000000 wheeldiff-2023.5.7.5/src/wheeldiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 05:12:53.000000 wheeldiff-2023.5.7.5/src/wheeldiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:12:53.309315 wheeldiff-2023.5.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 05:12:41.000000 wheeldiff-2023.5.7.5/tests/test_import.py
```

### Comparing `wheeldiff-2023.5.7/LICENSE` & `wheeldiff-2023.5.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7/PKG-INFO` & `wheeldiff-2023.5.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeldiff
-Version: 2023.5.7
+Version: 2023.5.7.5
 Summary: Diff two Python wheels
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `wheeldiff-2023.5.7/README.md` & `wheeldiff-2023.5.7.5/README.md`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7/pyproject.toml` & `wheeldiff-2023.5.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7/src/wheeldiff/_impl/cmd.py` & `wheeldiff-2023.5.7.5/src/wheeldiff/_impl/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
             LOG.debug("Renaming: %s => %s", entry.path, path)
             shutil.move(entry.path, path)
 
         if entry.is_dir():
             normalize(str(path), version, version_in_content)
         elif version_in_content:
             content = path.read_bytes()
+            # FIXME: this needs to be smarter, to ensure it only replaces
+            # versions which represent an entire word.
             new_content = content.replace(version.encode(), b"$VERSION")
             if content != new_content:
                 LOG.debug("Rewrote version in %s", path)
                 path.write_bytes(new_content)
 
 
 class UnpackedWheel:
```

### Comparing `wheeldiff-2023.5.7/src/wheeldiff.egg-info/PKG-INFO` & `wheeldiff-2023.5.7.5/src/wheeldiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeldiff
-Version: 2023.5.7
+Version: 2023.5.7.5
 Summary: Diff two Python wheels
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

