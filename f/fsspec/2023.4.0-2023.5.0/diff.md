# Comparing `tmp/fsspec-2023.4.0.tar.gz` & `tmp/fsspec-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsspec-2023.4.0.tar", last modified: Sat Apr  8 17:50:33 2023, max compression
+gzip compressed data, was "fsspec-2023.5.0.tar", last modified: Sun May  7 19:05:16 2023, max compression
```

## Comparing `fsspec-2023.4.0.tar` & `fsspec-2023.5.0.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 17:50:33.894985 fsspec-2023.4.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1513 2022-09-16 19:17:16.000000 fsspec-2023.4.0/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      110 2022-09-16 19:17:16.000000 fsspec-2023.4.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-04-08 17:50:33.895072 fsspec-2023.4.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     3464 2023-04-08 17:02:08.000000 fsspec-2023.4.0/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 17:50:33.895650 fsspec-2023.4.0/fsspec/
--rw-r--r--   0 mdurant    (502) staff       (20)     1800 2023-04-08 17:02:08.000000 fsspec-2023.4.0/fsspec/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-04-08 17:50:33.895702 fsspec-2023.4.0/fsspec/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2406 2023-01-20 20:07:35.000000 fsspec-2023.4.0/fsspec/archive.py
--rw-r--r--   0 mdurant    (502) staff       (20)    32277 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/asyn.py
--rw-r--r--   0 mdurant    (502) staff       (20)    26395 2023-04-08 17:02:08.000000 fsspec-2023.4.0/fsspec/caching.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6358 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/callbacks.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4856 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/compression.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4193 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/config.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1245 2022-09-21 20:03:17.000000 fsspec-2023.4.0/fsspec/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)    21507 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2717 2022-11-08 01:04:48.000000 fsspec-2023.4.0/fsspec/dircache.py
--rw-r--r--   0 mdurant    (502) staff       (20)      348 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/exceptions.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10187 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/fuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10211 2023-01-09 18:41:59.000000 fsspec-2023.4.0/fsspec/generic.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13766 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/gui.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 17:50:33.894748 fsspec-2023.4.0/fsspec/implementations/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/implementations/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8240 2023-03-12 01:59:42.000000 fsspec-2023.4.0/fsspec/implementations/arrow.py
--rw-r--r--   0 mdurant    (502) staff       (20)    30448 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/implementations/cached.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4466 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/implementations/dask.py
--rw-r--r--   0 mdurant    (502) staff       (20)    14648 2022-09-21 20:03:17.000000 fsspec-2023.4.0/fsspec/implementations/dbfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10826 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/implementations/dirfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10993 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/implementations/ftp.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4034 2022-11-28 20:11:28.000000 fsspec-2023.4.0/fsspec/implementations/git.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7328 2022-09-21 20:03:17.000000 fsspec-2023.4.0/fsspec/implementations/github.py
--rw-r--r--   0 mdurant    (502) staff       (20)    29225 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/implementations/http.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3816 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/implementations/jupyter.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7248 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/implementations/libarchive.py
--rw-r--r--   0 mdurant    (502) staff       (20)    12575 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/implementations/local.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9631 2023-01-09 15:22:42.000000 fsspec-2023.4.0/fsspec/implementations/memory.py
--rw-r--r--   0 mdurant    (502) staff       (20)    32532 2023-04-08 16:57:33.000000 fsspec-2023.4.0/fsspec/implementations/reference.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5464 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/implementations/sftp.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10023 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/implementations/smb.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4088 2023-01-09 15:00:42.000000 fsspec-2023.4.0/fsspec/implementations/tar.py
--rw-r--r--   0 mdurant    (502) staff       (20)    15391 2023-03-16 17:24:28.000000 fsspec-2023.4.0/fsspec/implementations/webhdfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4212 2023-01-20 20:07:35.000000 fsspec-2023.4.0/fsspec/implementations/zip.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7879 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)    19516 2022-11-04 01:13:55.000000 fsspec-2023.4.0/fsspec/parquet.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9900 2023-04-08 17:02:08.000000 fsspec-2023.4.0/fsspec/registry.py
--rw-r--r--   0 mdurant    (502) staff       (20)    60922 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/spec.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2195 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/transaction.py
--rw-r--r--   0 mdurant    (502) staff       (20)    16659 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 17:50:33.888389 fsspec-2023.4.0/fsspec.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1294 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-16 19:21:25.000000 fsspec-2023.4.0/fsspec.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      599 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        7 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      506 2023-04-08 17:02:08.000000 fsspec-2023.4.0/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.4.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      723 2023-04-08 17:50:33.895424 fsspec-2023.4.0/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     2427 2023-04-08 17:02:08.000000 fsspec-2023.4.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    78323 2023-03-12 01:59:42.000000 fsspec-2023.4.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.225273 fsspec-2023.5.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1513 2022-09-16 19:17:16.000000 fsspec-2023.5.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      110 2022-09-16 19:17:16.000000 fsspec-2023.5.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-05-07 19:05:16.225369 fsspec-2023.5.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     3464 2023-05-02 18:08:10.000000 fsspec-2023.5.0/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.226142 fsspec-2023.5.0/fsspec/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1800 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-05-07 19:05:16.226195 fsspec-2023.5.0/fsspec/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2406 2023-01-20 20:07:35.000000 fsspec-2023.5.0/fsspec/archive.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    32277 2023-04-01 20:24:09.000000 fsspec-2023.5.0/fsspec/asyn.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    26395 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/caching.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6358 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/callbacks.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4856 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/compression.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4193 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/config.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1245 2022-09-21 20:03:17.000000 fsspec-2023.5.0/fsspec/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    21507 2023-04-01 20:24:09.000000 fsspec-2023.5.0/fsspec/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2717 2022-11-08 01:04:48.000000 fsspec-2023.5.0/fsspec/dircache.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      348 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/exceptions.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10187 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/fuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10211 2023-01-09 18:41:59.000000 fsspec-2023.5.0/fsspec/generic.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13766 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/gui.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.224169 fsspec-2023.5.0/fsspec/implementations/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/implementations/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8240 2023-03-12 01:59:42.000000 fsspec-2023.5.0/fsspec/implementations/arrow.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    30448 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/implementations/cached.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4466 2023-04-01 20:24:09.000000 fsspec-2023.5.0/fsspec/implementations/dask.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    14648 2022-09-21 20:03:17.000000 fsspec-2023.5.0/fsspec/implementations/dbfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10826 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/implementations/dirfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10993 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/implementations/ftp.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4034 2022-11-28 20:11:28.000000 fsspec-2023.5.0/fsspec/implementations/git.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7328 2022-09-21 20:03:17.000000 fsspec-2023.5.0/fsspec/implementations/github.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    29225 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/implementations/http.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3816 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/implementations/jupyter.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7248 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/implementations/libarchive.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13672 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/implementations/local.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9631 2023-01-09 15:22:42.000000 fsspec-2023.5.0/fsspec/implementations/memory.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    41638 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/implementations/reference.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5464 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/implementations/sftp.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10023 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/implementations/smb.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4088 2023-01-09 15:00:42.000000 fsspec-2023.5.0/fsspec/implementations/tar.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    15391 2023-03-16 17:24:28.000000 fsspec-2023.5.0/fsspec/implementations/webhdfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4216 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/implementations/zip.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7879 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    19516 2022-11-04 01:13:55.000000 fsspec-2023.5.0/fsspec/parquet.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10079 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/registry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    62483 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/spec.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.208241 fsspec-2023.5.0/fsspec/tests/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.225102 fsspec-2023.5.0/fsspec/tests/abstract/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2179 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/tests/abstract/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10751 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/tests/abstract/copy.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1388 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/tests/abstract/get.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1338 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/tests/abstract/put.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2195 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/transaction.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    17103 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.217688 fsspec-2023.5.0/fsspec.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1416 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-16 19:21:25.000000 fsspec-2023.5.0/fsspec.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      599 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        7 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      506 2023-05-02 18:08:10.000000 fsspec-2023.5.0/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.5.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      723 2023-05-07 19:05:16.225771 fsspec-2023.5.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     2452 2023-05-02 18:08:10.000000 fsspec-2023.5.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    78323 2023-03-12 01:59:42.000000 fsspec-2023.5.0/versioneer.py
```

### Comparing `fsspec-2023.4.0/LICENSE` & `fsspec-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/PKG-INFO` & `fsspec-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: File-system specification
 Home-page: http://github.com/fsspec/filesystem_spec
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Project-URL: Changelog, https://filesystem-spec.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://filesystem-spec.readthedocs.io/en/latest/
```

### Comparing `fsspec-2023.4.0/README.md` & `fsspec-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/__init__.py` & `fsspec-2023.5.0/fsspec/__init__.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/archive.py` & `fsspec-2023.5.0/fsspec/archive.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/asyn.py` & `fsspec-2023.5.0/fsspec/asyn.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/caching.py` & `fsspec-2023.5.0/fsspec/caching.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/callbacks.py` & `fsspec-2023.5.0/fsspec/callbacks.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/compression.py` & `fsspec-2023.5.0/fsspec/compression.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/config.py` & `fsspec-2023.5.0/fsspec/config.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/conftest.py` & `fsspec-2023.5.0/fsspec/conftest.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/core.py` & `fsspec-2023.5.0/fsspec/core.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/dircache.py` & `fsspec-2023.5.0/fsspec/dircache.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/fuse.py` & `fsspec-2023.5.0/fsspec/fuse.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/generic.py` & `fsspec-2023.5.0/fsspec/generic.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/gui.py` & `fsspec-2023.5.0/fsspec/gui.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/arrow.py` & `fsspec-2023.5.0/fsspec/implementations/arrow.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/cached.py` & `fsspec-2023.5.0/fsspec/implementations/cached.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/dask.py` & `fsspec-2023.5.0/fsspec/implementations/dask.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/dbfs.py` & `fsspec-2023.5.0/fsspec/implementations/dbfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/dirfs.py` & `fsspec-2023.5.0/fsspec/implementations/dirfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/ftp.py` & `fsspec-2023.5.0/fsspec/implementations/ftp.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/git.py` & `fsspec-2023.5.0/fsspec/implementations/git.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/github.py` & `fsspec-2023.5.0/fsspec/implementations/github.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/http.py` & `fsspec-2023.5.0/fsspec/implementations/http.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/jupyter.py` & `fsspec-2023.5.0/fsspec/implementations/jupyter.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/libarchive.py` & `fsspec-2023.5.0/fsspec/implementations/libarchive.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/local.py` & `fsspec-2023.5.0/fsspec/implementations/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -268,14 +268,41 @@
         return path.lstrip("\\").replace("\\", "/").replace("//", "/")
     if path.startswith("\\"):
         # windows network path like "\\server\\path"
         return "/" + path.lstrip("\\").replace("\\", "/").replace("//", "/")
     return path
 
 
+def trailing_sep(path):
+    """Return True if the path ends with a path separator.
+
+    A forward slash is always considered a path separator, even on Operating
+    Systems that normally use a backslash.
+    """
+    # TODO: if all incoming paths were posix-compliant then separator would
+    # always be a forward slash, simplifying this function.
+    # See https://github.com/fsspec/filesystem_spec/pull/1250
+    return path.endswith(os.sep) or (os.altsep is not None and path.endswith(os.altsep))
+
+
+def trailing_sep_maybe_asterisk(path):
+    """Return True if the path ends with a path separator and optionally an
+    asterisk.
+
+    A forward slash is always considered a path separator, even on Operating
+    Systems that normally use a backslash.
+    """
+    # TODO: if all incoming paths were posix-compliant then separator would
+    # always be a forward slash, simplifying this function.
+    # See https://github.com/fsspec/filesystem_spec/pull/1250
+    return path.endswith((os.sep, os.sep + "*")) or (
+        os.altsep is not None and path.endswith((os.altsep, os.altsep + "*"))
+    )
+
+
 class LocalFileOpener(io.IOBase):
     def __init__(
         self, path, mode, autocommit=True, fs=None, compression=None, **kwargs
     ):
         logger.debug("open file: %s", path)
         self.path = path
         self.mode = mode
```

### Comparing `fsspec-2023.4.0/fsspec/implementations/memory.py` & `fsspec-2023.5.0/fsspec/implementations/memory.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/reference.py` & `fsspec-2023.5.0/fsspec/implementations/reference.py`

 * *Files 19% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 
         return pd
 
     def __init__(
         self,
         root,
         fs=None,
+        out_root=None,
         cache_size=128,
     ):
         """
         Parameters
         ----------
         root : str
             Root of parquet store
@@ -109,135 +110,355 @@
         self.dirs = None
         self.fs = fsspec.filesystem("file") if fs is None else fs
         with self.fs.open("/".join([self.root, ".zmetadata"]), "rb") as f:
             self._items[".zmetadata"] = f.read()
         met = json.loads(self._items[".zmetadata"])
         self.record_size = met["record_size"]
         self.zmetadata = met["metadata"]
-        if self.root:
-            self.url = self.root + "/{field}/refs.{record}.parq"
-        else:
-            self.url = "{field}/refs.{record}.parq"
+        self.url = self.root + "/{field}/refs.{record}.parq"
+        self.out_root = out_root or self.root
 
         # Define function to open and decompress refs
         @lru_cache(maxsize=cache_size)
         def open_refs(field, record):
+            """cached parquet file loader"""
             path = self.url.format(field=field, record=record)
             with self.fs.open(path) as f:
                 df = self.pd.read_parquet(f, engine="fastparquet")
             refs = {c: df[c].values for c in df.columns}
             # Return both df and dict of views because the former is
             # more convenient for iterating sequentially while the latter
             # is faster for random access.
             return df, refs
 
         self.open_refs = open_refs
 
+    @staticmethod
+    def create(record_size, root, fs, **kwargs):
+        met = {"metadata": {}, "record_size": record_size}
+        fs.pipe("/".join([root, ".zmetadata"]), json.dumps(met).encode())
+        return LazyReferenceMapper(root, fs, **kwargs)
+
     def listdir(self, basename=True):
+        """List top-level directories"""
         if self.dirs is None:
             dirs = [p.split("/", 1)[0] for p in self.zmetadata]
             self.dirs = set(sorted(p for p in dirs if p and not p.startswith(".")))
         listing = self.dirs
         if basename:
             listing = [os.path.basename(path) for path in listing]
         return listing
 
+    def ls(self, path="", detail=True):
+        """Shortcut file listings"""
+        if not path:
+            dirnames = self.listdir()
+            others = set(
+                [".zmetadata"]
+                + [name for name in self.zmetadata if "/" not in name]
+                + [name for name in self._items if "/" not in name]
+            )
+            if detail is False:
+                others.update(dirnames)
+                return sorted(others)
+            dirinfo = [
+                {"name": name, "type": "directory", "size": 0} for name in dirnames
+            ]
+            fileinfo = [
+                {
+                    "name": name,
+                    "type": "file",
+                    "size": len(
+                        json.dumps(self.zmetadata[name])
+                        if name in self.zmetadata
+                        else self._items[name]
+                    ),
+                }
+                for name in others
+            ]
+            return sorted(dirinfo + fileinfo, key=lambda s: s["name"])
+        parts = path.split("/", 1)
+        if len(parts) > 1:
+            raise FileNotFoundError("Cannot list within directories right now")
+        field = parts[0]
+        others = set(
+            [name for name in self.zmetadata if name.startswith(f"{path}/")]
+            + [name for name in self._items if name.startswith(f"{path}/")]
+        )
+        fileinfo = [
+            {
+                "name": name,
+                "type": "file",
+                "size": len(
+                    json.dumps(self.zmetadata[name])
+                    if name in self.zmetadata
+                    else self._items[name]
+                ),
+            }
+            for name in others
+        ]
+        keys = self._keys_in_field(field)
+
+        if detail is False:
+            return list(others) + list(keys)
+        recs = self._generate_all_records(field)
+        recinfo = [
+            {"name": name, "type": "file", "size": rec[-1]}
+            for name, rec in zip(keys, recs)
+            if rec[0]  # filters out path==None, deleted/missing
+        ]
+        return fileinfo + recinfo
+
     def _load_one_key(self, key):
+        """Get the reference for one key
+
+        Returns bytes, one-element list or three-element list.
+        """
         if key in self._items:
             return self._items[key]
         elif key in self.zmetadata:
             return json.dumps(self.zmetadata[key]).encode()
-        elif "/" not in key:
+        elif "/" not in key or self._is_meta(key):
             raise KeyError(key)
         field, sub_key = key.split("/")
+        record, _, _ = self._key_to_record(key)
+        maybe = self._items.get((field, key), {}).get(sub_key, False)
+        if maybe is None:
+            # explicitly deleted
+            raise KeyError
+        elif maybe:
+            return maybe
+
         # Chunk keys can be loaded from row group and cached in LRU cache
         try:
             record, ri, chunk_size = self._key_to_record(key)
             if chunk_size == 0:
                 return b""
             _, refs = self.open_refs(field, record)
         except (ValueError, TypeError, FileNotFoundError):
             raise KeyError(key)
         columns = ["path", "offset", "size", "raw"]
         selection = [refs[c][ri] if c in refs else None for c in columns]
         raw = selection[-1]
         if raw is not None:
             return raw
-        data = selection[:-1]
-        if data[1:] == [0, 0]:
-            data = data[:1]
-        return data
+        if selection[0] is None:
+            raise KeyError("This reference has been deleted")
+        if selection[1:3] == [0, 0]:
+            # URL only
+            return selection[:1]
+        # URL, offset, size
+        return selection[:3]
 
     def _key_to_record(self, key):
+        """Details needed to construct a reference for one key"""
         field, chunk = key.split("/")
         chunk_sizes = self._get_chunk_sizes(field)
         if chunk_sizes.size == 0:
             return 0, 0, 0
         chunk_idx = self.np.array([int(c) for c in chunk.split(".")])
         chunk_number = self.np.ravel_multi_index(chunk_idx, chunk_sizes)
         record = chunk_number // self.record_size
         ri = chunk_number % self.record_size
         return record, ri, chunk_sizes.size
 
     def _get_chunk_sizes(self, field):
+        """The number of chunks along each axis for a given field"""
         if field not in self.chunk_sizes:
             zarray = self.zmetadata[f"{field}/.zarray"]
             size_ratio = self.np.array(zarray["shape"]) / self.np.array(
                 zarray["chunks"]
             )
             self.chunk_sizes[field] = self.np.ceil(size_ratio).astype(int)
         return self.chunk_sizes[field]
 
     def _generate_record(self, field, record):
+        """The references for a given parquet file of a given field"""
         df, _ = self.open_refs(field, record)
         it = df.itertuples(name=None, index=False)
         if df.columns.size == 3:
             # All urls
             return (list(t) for t in it)
         elif df.columns.size == 1:
             # All raws
             return (t[0] for t in it)
         else:
             # Mix of urls and raws
             return (list(t[:3]) if not t[3] else t[3] for t in it)
 
     def _generate_all_records(self, field):
+        """Load all the references within a field by iterating over the parquet files"""
         chunk_size = self._get_chunk_sizes(field)
         nrec = int(self.np.ceil(self.np.product(chunk_size) / self.record_size))
         for record in range(nrec):
             yield from self._generate_record(field, record)
 
     def values(self):
         return RefsValuesView(self)
 
     def items(self):
         return RefsItemsView(self)
 
     def __getitem__(self, key):
-        if key in self._items:
-            val = self._items[key]
-            if val is None:
-                raise KeyError
-        if key in self.zmetadata:
-            # spec requires bytes even if we already decoded the metadata
-            return json.dumps(self.zmetadata[key]).encode()
         return self._load_one_key(key)
 
     def __setitem__(self, key, value):
-        self._items[key] = value
+        print(key, value)
+        if "/" in key and not self._is_meta(key):
+            field, chunk = key.split("/")
+            record, _, _ = self._key_to_record(key)
+            subdict = self._items.setdefault((field, record), {})
+            subdict[chunk] = value
+            if len(subdict) == self._output_size(field, record):
+                self.write(field, record)
+        else:
+            # metadata or top-level
+            self._items[key] = value
+            self.zmetadata[key] = json.loads(
+                value.decode() if isinstance(value, bytes) else value
+            )
+
+    @staticmethod
+    def _is_meta(key):
+        return key.startswith(".z") or "/.z" in key
 
     def __delitem__(self, key):
         if key in self._items:
             del self._items[key]
         elif key in self.zmetadata:
             del self.zmetadata[key]
         else:
-            # TODO: Add method to RefFs that tracks changes in _items
-            # and updates / copies appropriate parquet ref files.
-            self._items[key] = None
+            if "/" in key and not self._is_meta(key):
+                field, chunk = key.split("/")
+                record, _, _ = self._key_to_record(key)
+                subdict = self._items.setdefault((field, record), {})
+                subdict[chunk] = None
+                if len(subdict) == self._output_size(field, record):
+                    self.write(field, record)
+            else:
+                # metadata or top-level
+                self._items[key] = None
+
+    def _output_size(self, field, record):
+        np = self.np
+
+        zarray = json.loads(self[f"{field}/.zarray"])
+        chunk_sizes = np.ceil(np.array(zarray["shape"]) / np.array(zarray["chunks"]))
+        if chunk_sizes.size == 0:
+            chunk_sizes = np.array([0])
+        nchunks = int(np.product(chunk_sizes))
+        nrec = nchunks // self.record_size
+        rem = nchunks % self.record_size
+        if rem != 0:
+            nrec += 1
+        return self.record_size if record < nrec - 1 else rem
+
+    def write(self, field, record, base_url=None, storage_options=None):
+        # extra requirements if writing
+        import kerchunk.df
+        import numpy as np
+        import pandas as pd
+
+        # TODO: if the dict is incomplete, also load records and merge in
+        partition = self._items[(field, record)]
+        fn = f"{base_url or self.out_root}/{field}/refs.{record}.parq"
+        output_size = self._output_size(field, record)
+
+        ####
+        paths = np.full(self.record_size, np.nan, dtype="O")
+        offsets = np.zeros(self.record_size, dtype="int64")
+        sizes = np.zeros(self.record_size, dtype="int64")
+        raws = np.full(self.record_size, np.nan, dtype="O")
+        zarray = json.loads(self[f"{field}/.zarray"])
+        shape = np.array(zarray["shape"])
+        chunks = np.array(zarray["chunks"])
+        nraw = 0
+        npath = 0
+        for key, data in partition.items():
+            chunk_id = key.rsplit("/", 1)[-1]
+            chunk_ints = [int(ch) for ch in chunk_id.split(".")]
+            i = 0
+            mult = 1
+            for chunk_int, sh, ch in zip(chunk_ints[::-1], shape[::-1], chunks[::-1]):
+                i += chunk_int * mult
+                mult *= sh // ch
+            j = i % self.record_size
+            # Make note if expected number of chunks differs from actual
+            # number found in references
+            if isinstance(data, list):
+                npath += 1
+                paths[j] = data[0]
+                if len(data) > 1:
+                    offsets[j] = data[1]
+                    sizes[j] = data[2]
+            else:
+                nraw += 1
+                raws[j] = kerchunk.df._proc_raw(data)
+        # TODO: only save needed columns
+        df = pd.DataFrame(
+            dict(
+                path=paths,
+                offset=offsets,
+                size=sizes,
+                raw=raws,
+            ),
+            copy=False,
+        )[:output_size]
+        object_encoding = dict(raw="bytes", path="utf8")
+        has_nulls = ["path", "raw"]
+
+        self.fs.mkdirs(f"{base_url or self.out_root}/{field}", exist_ok=True)
+        df.to_parquet(
+            fn,
+            engine="fastparquet",
+            storage_options=storage_options
+            or getattr(self.fs, "storage_options", None),
+            compression="zstd",
+            index=False,
+            stats=False,
+            object_encoding=object_encoding,
+            has_nulls=has_nulls,
+            # **kwargs,
+        )
+        partition.clear()
+        self._items.pop((field, record))
+
+    def flush(self, base_url=None, storage_options=None):
+        """Output any modified or deleted keys
+
+        Parameters
+        ----------
+        base_url: str
+            Location of the output
+        """
+        # write what we have so far and clear sub chunks
+        for thing in self._items:
+            if isinstance(thing, tuple):
+                field, record = thing
+                if self._items.get((record, field)):
+                    self.write(
+                        field,
+                        record,
+                        base_url=base_url,
+                        storage_options=storage_options,
+                    )
+
+        # gather .zmetadata from self._items and write that too
+        for k in list(self._items):
+            if k != ".zmetadata" and ".z" in k:
+                self.zmetadata[k] = json.loads(self._items.pop(k))
+        met = {"metadata": self.zmetadata, "record_size": self.record_size}
+        self._items[".zmetadata"] = json.dumps(met).encode()
+        self.fs.pipe(
+            "/".join([base_url or self.out_root, ".zmetadata"]),
+            self._items[".zmetadata"],
+        )
+
+        # TODO: only clear those that we wrote to?
+        self.open_refs.cache_clear()
 
     def __len__(self):
         # Caveat: This counts expected references, not actual
         count = 0
         for field in self.listdir():
             if field.startswith("."):
                 count += 1
@@ -248,24 +469,41 @@
         count += len(self.zmetadata)  # all metadata keys
         count += len(self._items)  # the metadata file itself
         return count
 
     def __iter__(self):
         # Caveat: Note that this generates all expected keys, but does not
         # account for reference keys that are missing.
-        yield from self.zmetadata
-        yield from self._items
+        metas = set(self.zmetadata)
+        metas.update(self._items)
+        for bit in metas:
+            if isinstance(bit, str):
+                yield bit
         for field in self.listdir():
-            chunk_sizes = self._get_chunk_sizes(field)
-            if chunk_sizes.size == 0:
-                yield field + "/0"
-                continue
-            inds = self.np.ndindex(*chunk_sizes)
-            for ind in inds:
-                yield field + "/" + ".".join([str(c) for c in ind])
+            yield from self._keys_in_field(field)
+
+    def __contains__(self, item):
+        try:
+            self._load_one_key(item)
+            return True
+        except KeyError:
+            return False
+
+    def _keys_in_field(self, field):
+        """List key names in given field
+
+        Produces strings like "field/x.y" appropriate from the chunking of the array
+        """
+        chunk_sizes = self._get_chunk_sizes(field)
+        if chunk_sizes.size == 0:
+            yield field + "/0"
+            return
+        inds = self.np.ndindex(*chunk_sizes)
+        for ind in inds:
+            yield field + "/" + ".".join([str(c) for c in ind])
 
 
 class ReferenceFileSystem(AsyncFileSystem):
     """View byte ranges of some other file as a file system
     Initial version: single file system target, which must support
     async, and must allow start and end args in _cat_file. Later versions
     may allow multiple arbitrary URLs for the targets.
@@ -416,17 +654,19 @@
         if remote_protocol is None:
             # get single protocol from references
             for ref in self.references.values():
                 if callable(ref):
                     ref = ref()
                 if isinstance(ref, list) and ref[0]:
                     protocol, _ = fsspec.core.split_protocol(ref[0])
-                    if protocol and protocol not in self.fss:
+                    if protocol not in self.fss:
                         fs = filesystem(protocol, **(remote_options or {}))
                         self.fss[protocol] = fs
+                        # only use first remote URL
+                        break
 
         if remote_protocol and remote_protocol not in self.fss:
             fs = filesystem(remote_protocol, **(remote_options or {}))
             self.fss[remote_protocol] = fs
 
         self.fss[None] = fs or filesystem("file")  # default one
 
@@ -743,14 +983,20 @@
 
     def _open(self, path, mode="rb", block_size=None, cache_options=None, **kwargs):
         data = self.cat_file(path)  # load whole chunk into memory
         return io.BytesIO(data)
 
     def ls(self, path, detail=True, **kwargs):
         path = self._strip_protocol(path)
+        if isinstance(self.references, LazyReferenceMapper):
+            try:
+                return self.references.ls(path, detail)
+            except KeyError:
+                pass
+            raise FileNotFoundError(f"'{path}' is not a known key")
         if not self.dircache:
             self._dircache_from_items()
         out = self._ls_from_cache(path)
         if out is None:
             raise FileNotFoundError(path)
         if detail:
             return out
@@ -758,27 +1004,28 @@
 
     def exists(self, path, **kwargs):  # overwrite auto-sync version
         return self.isdir(path) or self.isfile(path)
 
     def isdir(self, path):  # overwrite auto-sync version
         if self.dircache:
             return path in self.dircache
+        elif isinstance(self.references, LazyReferenceMapper):
+            return path in self.references.listdir("")
         else:
             # this may be faster than building dircache for single calls, but
             # by looping will be slow for many calls; could cache it?
             return any(_.startswith(f"{path}/") for _ in self.references)
 
     def isfile(self, path):  # overwrite auto-sync version
         return path in self.references
 
     async def _ls(self, path, detail=True, **kwargs):  # calls fast sync code
         return self.ls(path, detail, **kwargs)
 
     def find(self, path, maxdepth=None, withdirs=False, detail=False, **kwargs):
-        # TODO: details
         if withdirs:
             return super().find(
                 path, maxdepth=maxdepth, withdirs=withdirs, detail=detail, **kwargs
             )
         if path:
             path = self._strip_protocol(path)
             r = sorted(k for k in self.references if k.startswith(path))
@@ -788,16 +1035,16 @@
             if not self.dircache:
                 self._dircache_from_items()
             return {k: self._ls_from_cache(k)[0] for k in r}
         else:
             return r
 
     def info(self, path, **kwargs):
-        if path in self.references:
-            out = self.references[path]
+        out = self.references.get(path)
+        if out is not None:
             if isinstance(out, (str, bytes)):
                 # decode base64 here
                 return {"name": path, "type": "file", "size": len(out)}
             elif len(out) > 1:
                 return {"name": path, "type": "file", "size": out[2]}
             else:
                 out0 = [{"name": path, "type": "file", "size": None}]
```

### Comparing `fsspec-2023.4.0/fsspec/implementations/sftp.py` & `fsspec-2023.5.0/fsspec/implementations/sftp.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/smb.py` & `fsspec-2023.5.0/fsspec/implementations/smb.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/tar.py` & `fsspec-2023.5.0/fsspec/implementations/tar.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/webhdfs.py` & `fsspec-2023.5.0/fsspec/implementations/webhdfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/implementations/zip.py` & `fsspec-2023.5.0/fsspec/implementations/zip.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def _strip_protocol(cls, path):
         # zip file paths are always relative to the archive root
         return super()._strip_protocol(path).lstrip("/")
 
     def __del__(self):
         if hasattr(self, "zip"):
             self.close()
-        del self.zip
+            del self.zip
 
     def close(self):
         """Commits any write changes to the file. Done on ``del`` too."""
         self.zip.close()
 
     def _get_dirs(self):
         if self.dir_cache is None or self.mode in set("wa"):
```

### Comparing `fsspec-2023.4.0/fsspec/mapping.py` & `fsspec-2023.5.0/fsspec/mapping.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/parquet.py` & `fsspec-2023.5.0/fsspec/parquet.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/registry.py` & `fsspec-2023.5.0/fsspec/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,29 +30,33 @@
         instead.
     errtxt: str (optional)
         If given, then a failure to import the given class will result in this
         text being given.
     """
     if isinstance(cls, str):
         if name in known_implementations and clobber is False:
-            raise ValueError(
-                "Name (%s) already in the known_implementations and clobber "
-                "is False" % name
-            )
-        known_implementations[name] = {
-            "class": cls,
-            "err": errtxt or "%s import failed for protocol %s" % (cls, name),
-        }
+            if cls != known_implementations[name]["class"]:
+                raise ValueError(
+                    "Name (%s) already in the known_implementations and clobber "
+                    "is False" % name
+                )
+        else:
+            known_implementations[name] = {
+                "class": cls,
+                "err": errtxt or "%s import failed for protocol %s" % (cls, name),
+            }
 
     else:
         if name in registry and clobber is False:
-            raise ValueError(
-                "Name (%s) already in the registry and clobber is False" % name
-            )
-        _registry[name] = cls
+            if _registry[name] is not cls:
+                raise ValueError(
+                    "Name (%s) already in the registry and clobber is False" % name
+                )
+        else:
+            _registry[name] = cls
 
 
 # protocols mapped to the class which implements them. This dict can
 # updated with register_implementation
 known_implementations = {
     "file": {"class": "fsspec.implementations.local.LocalFileSystem"},
     "memory": {"class": "fsspec.implementations.memory.MemoryFileSystem"},
```

### Comparing `fsspec-2023.4.0/fsspec/spec.py` & `fsspec-2023.5.0/fsspec/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -875,27 +875,40 @@
         Copies a specific file or tree of files (if recursive=True). If lpath
         ends with a "/", it will be assumed to be a directory, and target files
         will go within. Can submit a list of paths, which may be glob-patterns
         and will be expanded.
 
         Calls get_file for each source.
         """
-        from .implementations.local import LocalFileSystem, make_path_posix
+        from .implementations.local import (
+            LocalFileSystem,
+            make_path_posix,
+            trailing_sep,
+            trailing_sep_maybe_asterisk,
+        )
+
+        source_is_str = isinstance(rpath, str)
+        rpaths = self.expand_path(rpath, recursive=recursive)
+        if source_is_str and not recursive:
+            # Non-recursive glob does not copy directories
+            rpaths = [p for p in rpaths if not (trailing_sep(p) or self.isdir(p))]
+            if not rpaths:
+                return
 
         if isinstance(lpath, str):
             lpath = make_path_posix(lpath)
-        rpaths = self.expand_path(rpath, recursive=recursive)
         isdir = isinstance(lpath, str) and (
-            lpath.endswith("/") or LocalFileSystem().isdir(lpath)
+            trailing_sep(lpath) or LocalFileSystem().isdir(lpath)
         )
         lpaths = other_paths(
             rpaths,
             lpath,
-            exists=isdir and isinstance(rpath, str) and not rpath.endswith("/"),
+            exists=isdir and source_is_str and not trailing_sep_maybe_asterisk(rpath),
             is_dir=isdir,
+            flatten=not source_is_str,
         )
 
         callback.set_size(len(lpaths))
         for lpath, rpath in callback.wrap(zip(lpaths, rpaths)):
             callback.branch(rpath, lpath, kwargs)
             self.get_file(rpath, lpath, **kwargs)
 
@@ -924,31 +937,44 @@
 
         Copies a specific file or tree of files (if recursive=True). If rpath
         ends with a "/", it will be assumed to be a directory, and target files
         will go within.
 
         Calls put_file for each source.
         """
-        from .implementations.local import LocalFileSystem, make_path_posix
+        from .implementations.local import (
+            LocalFileSystem,
+            make_path_posix,
+            trailing_sep,
+            trailing_sep_maybe_asterisk,
+        )
+
+        if isinstance(lpath, str):
+            lpath = make_path_posix(lpath)
+        fs = LocalFileSystem()
+        source_is_str = isinstance(lpath, str)
+        lpaths = fs.expand_path(lpath, recursive=recursive)
+        if source_is_str and not recursive:
+            # Non-recursive glob does not copy directories
+            lpaths = [p for p in lpaths if not (trailing_sep(p) or self.isdir(p))]
+            if not lpaths:
+                return
 
         rpath = (
             self._strip_protocol(rpath)
             if isinstance(rpath, str)
             else [self._strip_protocol(p) for p in rpath]
         )
-        if isinstance(lpath, str):
-            lpath = make_path_posix(lpath)
-        fs = LocalFileSystem()
-        lpaths = fs.expand_path(lpath, recursive=recursive)
-        isdir = isinstance(rpath, str) and (rpath.endswith("/") or self.isdir(rpath))
+        isdir = isinstance(rpath, str) and (trailing_sep(rpath) or self.isdir(rpath))
         rpaths = other_paths(
             lpaths,
             rpath,
-            exists=isdir and isinstance(lpath, str) and not lpath.endswith("/"),
+            exists=isdir and source_is_str and not trailing_sep_maybe_asterisk(lpath),
             is_dir=isdir,
+            flatten=not source_is_str,
         )
 
         callback.set_size(len(rpaths))
         for lpath, rpath in callback.wrap(zip(lpaths, rpaths)):
             callback.branch(lpath, rpath, kwargs)
             self.put_file(lpath, rpath, **kwargs)
 
@@ -970,60 +996,79 @@
         """Copy within two locations in the filesystem
 
         on_error : "raise", "ignore"
             If raise, any not-found exceptions will be raised; if ignore any
             not-found exceptions will cause the path to be skipped; defaults to
             raise unless recursive is true, where the default is ignore
         """
+        from .implementations.local import trailing_sep, trailing_sep_maybe_asterisk
+
         if on_error is None and recursive:
             on_error = "ignore"
         elif on_error is None:
             on_error = "raise"
 
+        source_is_str = isinstance(path1, str)
         paths = self.expand_path(path1, recursive=recursive)
-        isdir = isinstance(path2, str) and (path2.endswith("/") or self.isdir(path2))
+        if source_is_str and not recursive:
+            # Non-recursive glob does not copy directories
+            paths = [p for p in paths if not (trailing_sep(p) or self.isdir(p))]
+            if not paths:
+                return
+
+        isdir = isinstance(path2, str) and (trailing_sep(path2) or self.isdir(path2))
         path2 = other_paths(
             paths,
             path2,
-            exists=isdir and isinstance(path1, str) and not path1.endswith("/"),
+            exists=isdir and source_is_str and not trailing_sep_maybe_asterisk(path1),
             is_dir=isdir,
+            flatten=not source_is_str,
         )
 
         for p1, p2 in zip(paths, path2):
             try:
                 self.cp_file(p1, p2, **kwargs)
             except FileNotFoundError:
                 if on_error == "raise":
                     raise
 
-    def expand_path(self, path, recursive=False, maxdepth=None):
+    def expand_path(self, path, recursive=False, maxdepth=None, **kwargs):
         """Turn one or more globs or directories into a list of all matching paths
-        to files or directories."""
+        to files or directories.
+
+        kwargs are passed to ``glob`` or ``find``, which may in turn call ``ls``
+        """
+
         if maxdepth is not None and maxdepth < 1:
             raise ValueError("maxdepth must be at least 1")
 
         if isinstance(path, str):
             out = self.expand_path([path], recursive, maxdepth)
         else:
             out = set()
             path = [self._strip_protocol(p) for p in path]
             for p in path:
                 if has_magic(p):
-                    bit = set(self.glob(p))
+                    bit = set(self.glob(p, **kwargs))
                     out |= bit
                     if recursive:
                         out |= set(
                             self.expand_path(
-                                list(bit), recursive=recursive, maxdepth=maxdepth
+                                list(bit),
+                                recursive=recursive,
+                                maxdepth=maxdepth,
+                                **kwargs,
                             )
                         )
                     continue
                 elif recursive:
                     rec = set(
-                        self.find(p, maxdepth=maxdepth, withdirs=True, detail=False)
+                        self.find(
+                            p, maxdepth=maxdepth, withdirs=True, detail=False, **kwargs
+                        )
                     )
                     out |= rec
                 if p not in out and (recursive is False or self.exists(p)):
                     # should only check once, for the root
                     out.add(p)
         if not out:
             raise FileNotFoundError(path)
```

### Comparing `fsspec-2023.4.0/fsspec/transaction.py` & `fsspec-2023.5.0/fsspec/transaction.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/fsspec/utils.py` & `fsspec-2023.5.0/fsspec/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         end = all(p[i] == parts[0][i] for p in parts)
         if not end:
             break
     i += end
     return "/".join(parts[0][:i])
 
 
-def other_paths(paths, path2, is_dir=None, exists=False):
+def other_paths(paths, path2, is_dir=None, exists=False, flatten=False):
     """In bulk file operations, construct a new file tree from a list of files
 
     Parameters
     ----------
     paths: list of str
         The input file tree
     path2: str or list of str
@@ -354,26 +354,37 @@
     is_dir: bool (optional)
         For the special case where the input in one element, whether to regard the value
         as the target path, or as a directory to put a file path within. If None, a
         directory is inferred if the path ends in '/'
     exists: bool (optional)
         For a str destination, it is already exists (and is a dir), files should
         end up inside.
+    flatten: bool (optional)
+        Whether to flatten the input directory tree structure so that the output files
+        are in the same directory.
 
     Returns
     -------
     list of str
     """
+
     if isinstance(path2, str):
         is_dir = is_dir or path2.endswith("/")
         path2 = path2.rstrip("/")
-        cp = common_prefix(paths)
-        if exists:
-            cp = cp.rsplit("/", 1)[0]
-        path2 = [p.replace(cp, path2, 1) for p in paths]
+
+        if flatten:
+            path2 = ["/".join((path2, p.split("/")[-1])) for p in paths]
+        else:
+            cp = common_prefix(paths)
+            if exists:
+                cp = cp.rsplit("/", 1)[0]
+            if not cp and all(not s.startswith("/") for s in paths):
+                path2 = ["/".join([path2, p]) for p in paths]
+            else:
+                path2 = [p.replace(cp, path2, 1) for p in paths]
     else:
         assert len(paths) == len(path2)
     return path2
 
 
 def is_exception(obj):
     return isinstance(obj, BaseException)
```

### Comparing `fsspec-2023.4.0/fsspec.egg-info/PKG-INFO` & `fsspec-2023.5.0/fsspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: File-system specification
 Home-page: http://github.com/fsspec/filesystem_spec
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Project-URL: Changelog, https://filesystem-spec.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://filesystem-spec.readthedocs.io/en/latest/
```

### Comparing `fsspec-2023.4.0/fsspec.egg-info/SOURCES.txt` & `fsspec-2023.5.0/fsspec.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -48,8 +48,12 @@
 fsspec/implementations/local.py
 fsspec/implementations/memory.py
 fsspec/implementations/reference.py
 fsspec/implementations/sftp.py
 fsspec/implementations/smb.py
 fsspec/implementations/tar.py
 fsspec/implementations/webhdfs.py
-fsspec/implementations/zip.py
+fsspec/implementations/zip.py
+fsspec/tests/abstract/__init__.py
+fsspec/tests/abstract/copy.py
+fsspec/tests/abstract/get.py
+fsspec/tests/abstract/put.py
```

### Comparing `fsspec-2023.4.0/fsspec.egg-info/requires.txt` & `fsspec-2023.5.0/fsspec.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/setup.cfg` & `fsspec-2023.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fsspec-2023.4.0/setup.py` & `fsspec-2023.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,13 +66,13 @@
         "Changelog": "https://filesystem-spec.readthedocs.io/en/latest/changelog.html",
         "Documentation": "https://filesystem-spec.readthedocs.io/en/latest/",
     },
     maintainer="Martin Durant",
     maintainer_email="mdurant@anaconda.com",
     license="BSD",
     keywords="file",
-    packages=["fsspec", "fsspec.implementations"],
+    packages=["fsspec", "fsspec.implementations", "fsspec.tests.abstract"],
     python_requires=">=3.8",
     install_requires=open("requirements.txt").read().strip().split("\n"),
     extras_require=extras_require,
     zip_safe=False,
 )
```

### Comparing `fsspec-2023.4.0/versioneer.py` & `fsspec-2023.5.0/versioneer.py`

 * *Files identical despite different names*

