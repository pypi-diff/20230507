# Comparing `tmp/pygit2-1.9.1.tar.gz` & `tmp/pygit2-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygit2-1.9.1.tar", last modified: Tue Mar 22 19:11:49 2022, max compression
+gzip compressed data, was "pygit2-1.9.2.tar", last modified: Tue May 24 20:01:01 2022, max compression
```

## Comparing `pygit2-1.9.1.tar` & `pygit2-1.9.2.tar`

### file list

```diff
@@ -1,259 +1,185 @@
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3305 2022-03-22 18:03:42.490198 pygit2-1.9.1/AUTHORS.rst
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    53747 2022-03-22 18:01:20.823864 pygit2-1.9.1/CHANGELOG.rst
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    19054 2021-09-17 11:25:19.987411 pygit2-1.9.1/COPYING
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      117 2022-03-06 08:31:44.306066 pygit2-1.9.1/Makefile
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3496 2022-03-22 19:11:49.092077 pygit2-1.9.1/PKG-INFO
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2363 2021-12-06 08:47:08.838489 pygit2-1.9.1/README.rst
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      253 2022-02-23 12:38:08.106666 pygit2-1.9.1/SPONSORS.rst
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     7742 2022-03-06 08:31:18.845079 pygit2-1.9.1/build.sh
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      156 2021-06-19 09:31:42.533738 pygit2-1.9.1/build_tag.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      461 2022-03-06 08:26:49.549038 pygit2-1.9.1/mypy-stubtest.ini
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.084077 pygit2-1.9.1/pygit2/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     8224 2021-09-17 11:25:19.987411 pygit2-1.9.1/pygit2/__init__.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2352 2022-03-22 18:18:03.074508 pygit2-1.9.1/pygit2/_build.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    20265 2022-03-06 08:26:49.549038 pygit2-1.9.1/pygit2/_pygit2.pyi
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2706 2022-03-19 10:40:15.425663 pygit2-1.9.1/pygit2/_run.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4107 2021-09-17 11:25:19.987411 pygit2-1.9.1/pygit2/blame.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    15783 2022-01-29 07:18:52.169225 pygit2-1.9.1/pygit2/callbacks.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    11092 2021-09-17 11:25:19.991411 pygit2-1.9.1/pygit2/config.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3938 2021-09-17 11:25:19.991411 pygit2-1.9.1/pygit2/credentials.py
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.085077 pygit2-1.9.1/pygit2/decl/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      451 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/attr.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1051 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/blame.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      112 2022-02-14 07:53:46.471747 pygit2-1.9.1/pygit2/decl/buffer.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      963 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/callbacks.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1826 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/checkout.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      952 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/clone.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      261 2021-10-20 07:44:38.815929 pygit2-1.9.1/pygit2/decl/commit.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      188 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/common.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2149 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/config.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1228 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/describe.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2114 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/diff.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      937 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/errors.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      128 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/graph.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2331 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/index.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      356 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/indexer.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2139 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/merge.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       84 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/net.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      309 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/oid.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      747 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/pack.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      411 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/proxy.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      615 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/refspec.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4855 2022-02-14 07:51:50.249861 pygit2-1.9.1/pygit2/decl/remote.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2135 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/repository.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      183 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/revert.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1688 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/stash.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      124 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/strarray.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1270 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/submodule.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1520 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/transport.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1554 2021-06-19 09:40:24.646733 pygit2-1.9.1/pygit2/decl/types.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2362 2021-09-17 11:25:19.991411 pygit2-1.9.1/pygit2/errors.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1246 2021-09-17 11:25:19.991411 pygit2-1.9.1/pygit2/ffi.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    14886 2021-09-17 11:25:19.991411 pygit2-1.9.1/pygit2/index.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2821 2021-09-17 11:25:19.991411 pygit2-1.9.1/pygit2/packbuilder.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3427 2021-09-17 11:25:19.991411 pygit2-1.9.1/pygit2/refspec.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    13276 2022-01-26 15:20:11.883729 pygit2-1.9.1/pygit2/remote.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    55966 2022-03-14 08:15:20.348721 pygit2-1.9.1/pygit2/repository.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6897 2021-09-17 11:25:19.995411 pygit2-1.9.1/pygit2/settings.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2635 2021-09-17 11:25:19.995411 pygit2-1.9.1/pygit2/submodule.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3664 2021-09-17 11:25:19.995411 pygit2-1.9.1/pygit2/utils.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       50 2020-03-11 08:34:41.877181 pygit2-1.9.1/pyproject.toml
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       64 2021-09-17 11:25:19.995411 pygit2-1.9.1/pytest.ini
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       18 2021-11-06 12:09:47.575052 pygit2-1.9.1/requirements-test.txt
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       52 2022-02-23 12:39:10.615412 pygit2-1.9.1/requirements.txt
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       89 2021-10-08 08:39:16.348105 pygit2-1.9.1/setup.cfg
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5605 2022-03-20 20:36:06.725472 pygit2-1.9.1/setup.py
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.087077 pygit2-1.9.1/src/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9210 2022-03-14 08:11:42.421751 pygit2-1.9.1/src/blob.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    10311 2022-03-14 08:11:42.422752 pygit2-1.9.1/src/branch.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1624 2022-01-26 17:46:27.227020 pygit2-1.9.1/src/branch.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    11661 2022-03-14 08:11:42.422752 pygit2-1.9.1/src/commit.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    39812 2022-03-14 08:11:42.426751 pygit2-1.9.1/src/diff.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1657 2022-01-26 17:46:27.227020 pygit2-1.9.1/src/diff.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4509 2022-03-14 08:11:42.427751 pygit2-1.9.1/src/error.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1674 2021-09-17 11:25:19.999411 pygit2-1.9.1/src/error.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9133 2022-03-14 08:11:42.430751 pygit2-1.9.1/src/mailmap.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1425 2022-01-26 17:53:30.098494 pygit2-1.9.1/src/mailmap.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9299 2022-03-14 08:11:42.430751 pygit2-1.9.1/src/note.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1470 2021-09-17 11:25:19.999411 pygit2-1.9.1/src/note.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    12056 2022-03-14 08:11:42.431751 pygit2-1.9.1/src/object.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1628 2022-01-26 17:46:27.227020 pygit2-1.9.1/src/object.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    12017 2022-03-14 08:11:42.431751 pygit2-1.9.1/src/odb.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1533 2021-09-17 11:25:19.999411 pygit2-1.9.1/src/odb.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    25493 2022-03-14 08:11:42.432751 pygit2-1.9.1/src/odb_backend.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1446 2021-09-17 11:25:19.999411 pygit2-1.9.1/src/odb_backend.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9046 2022-03-14 08:11:42.432751 pygit2-1.9.1/src/oid.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1620 2021-09-17 11:25:19.999411 pygit2-1.9.1/src/oid.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9842 2022-03-14 08:11:42.433751 pygit2-1.9.1/src/options.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1932 2021-09-17 11:25:20.003411 pygit2-1.9.1/src/options.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9858 2022-03-14 08:11:42.433751 pygit2-1.9.1/src/patch.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1425 2021-09-17 11:25:20.003411 pygit2-1.9.1/src/patch.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    22004 2022-03-14 08:11:42.434751 pygit2-1.9.1/src/pygit2.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6958 2022-03-14 08:11:42.434751 pygit2-1.9.1/src/refdb.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1416 2021-06-19 09:40:24.646733 pygit2-1.9.1/src/refdb.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    29161 2022-03-14 08:11:42.435751 pygit2-1.9.1/src/refdb_backend.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1456 2021-06-19 09:40:24.642733 pygit2-1.9.1/src/refdb_backend.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    23014 2022-03-14 08:11:42.435751 pygit2-1.9.1/src/reference.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1622 2022-01-26 17:46:27.227020 pygit2-1.9.1/src/reference.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    66673 2022-03-14 08:11:42.436751 pygit2-1.9.1/src/repository.c
--rwxr-xr-x   0 jdavid    (1001) jdavid    (1001)     3325 2022-01-26 17:46:27.228020 pygit2-1.9.1/src/repository.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5985 2022-03-14 08:11:42.436751 pygit2-1.9.1/src/revspec.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1442 2021-09-17 11:25:20.003411 pygit2-1.9.1/src/revspec.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    10093 2022-03-22 08:46:40.405650 pygit2-1.9.1/src/signature.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1492 2022-01-26 17:46:27.228020 pygit2-1.9.1/src/signature.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5967 2022-03-14 08:11:42.436751 pygit2-1.9.1/src/stash.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6681 2022-03-14 08:11:42.436751 pygit2-1.9.1/src/tag.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    18899 2022-03-14 08:11:42.436751 pygit2-1.9.1/src/tree.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1451 2022-01-26 17:46:27.228020 pygit2-1.9.1/src/tree.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     7413 2022-03-14 08:11:42.437751 pygit2-1.9.1/src/treebuilder.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1619 2021-09-17 11:25:20.007411 pygit2-1.9.1/src/treebuilder.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5507 2022-02-14 07:38:49.754672 pygit2-1.9.1/src/types.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6403 2022-03-14 08:11:42.437751 pygit2-1.9.1/src/utils.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5235 2021-09-17 11:25:20.007411 pygit2-1.9.1/src/utils.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6717 2022-03-14 08:11:42.437751 pygit2-1.9.1/src/walker.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1698 2021-09-17 11:25:20.007411 pygit2-1.9.1/src/walker.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9488 2022-03-14 08:11:42.437751 pygit2-1.9.1/src/wildmatch.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      501 2021-06-19 09:40:24.646733 pygit2-1.9.1/src/wildmatch.h
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6090 2022-03-14 08:11:42.438751 pygit2-1.9.1/src/worktree.c
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1449 2021-09-17 11:25:20.007411 pygit2-1.9.1/src/worktree.h
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.089077 pygit2-1.9.1/test/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1482 2022-03-22 17:53:02.953378 pygit2-1.9.1/test/__init__.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2196 2022-03-20 07:29:56.979253 pygit2-1.9.1/test/conftest.py
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    92160 2015-10-25 12:02:52.763826 pygit2-1.9.1/test/data/binaryfilerepo.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    71680 2021-09-17 11:25:20.007411 pygit2-1.9.1/test/data/blameflagsrepo.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    61440 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/dirtyrepo.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    30720 2015-01-26 17:11:50.327102 pygit2-1.9.1/test/data/emptyrepo.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    50176 2019-03-30 18:59:29.180037 pygit2-1.9.1/test/data/encoding.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    49152 2018-02-06 08:58:51.798514 pygit2-1.9.1/test/data/gpgsigned.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    61440 2020-04-19 15:11:42.206231 pygit2-1.9.1/test/data/submodulerepo.tar
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       23 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/HEAD
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       97 2015-01-26 17:11:50.327102 pygit2-1.9.1/test/data/testrepo.git/config
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.083077 pygit2-1.9.1/test/data/testrepo.git/objects/
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/05/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      154 2015-01-26 17:11:50.327102 pygit2-1.9.1/test/data/testrepo.git/objects/05/6e626e51b1fc1ee2182800e399ed8d84c8f082
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/10/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      209 2015-01-26 17:11:50.327102 pygit2-1.9.1/test/data/testrepo.git/objects/10/2374bdb1e8efca5e66cded18fd8f30571654a5
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/11/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      136 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/11/19926b06311143cab273f0af84eae77f5b3462
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/18/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       99 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/18/e2d2e9db075f9eb43bcb2daa65a2867d29a15e
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/19/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      136 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/19/bf31524643d743751b09cf719456914bbd8bd5
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/1a/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      107 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/1a/f81f24e48f92009ca02a874edb6151c71f60de
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/29/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       29 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/29/7efb891a47de80be0cfe9c639e4b8c9b450989
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/2a/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       99 2015-01-26 17:10:33.311656 pygit2-1.9.1/test/data/testrepo.git/objects/2a/d1d3456c5c4a1c9e40aeeddb9cd20b409623c8
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/2c/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      199 2015-01-26 17:10:33.311656 pygit2-1.9.1/test/data/testrepo.git/objects/2c/dae28389c059815e951d0bb9eed6533f61a46b
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/39/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      200 2015-01-26 17:10:33.311656 pygit2-1.9.1/test/data/testrepo.git/objects/39/a3001fcc2b9541fdcf4be2d662618a5d213f47
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/3d/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      136 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/3d/2962987c695a29f1f80b6c3aa4ec046ef44369
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/55/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      129 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/55/60f04f38a674decf34d16d7c7476642fa03794
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/5f/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      200 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/5f/e808e8953c12735680c257f56600cb0de44b10
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/61/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       46 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/61/4fd9a3094bf618ea938fffc00e7d1a54f89ad0
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/62/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       84 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/62/cc88a53cfb046fcf603b3aaeb73b8e18215442
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/63/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      150 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/63/59f8019b0954201a807b766547526173f3cc67
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/6a/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       29 2015-01-26 17:10:33.311656 pygit2-1.9.1/test/data/testrepo.git/objects/6a/270c81bc80b59591e0d2e3abd7d03450c0c395
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/72/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       99 2015-01-26 17:10:33.311656 pygit2-1.9.1/test/data/testrepo.git/objects/72/abb8755b2cc6c4e40fd9f50f54384d973a2f22
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.090077 pygit2-1.9.1/test/data/testrepo.git/objects/77/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       30 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/77/88019febe4f40259a64c529a9aed561e64ddbd
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/78/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      176 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/78/4855caf26449a1914d2cf62d12b9374d76ae78
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/7f/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       29 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/7f/129fd57e31e935c6d60a0c794efe4e6927664b
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/96/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       98 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/96/7fce8df97cc71722d3c2a5930ef3e6f1d27b12
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/97/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       29 2015-01-26 17:10:33.311656 pygit2-1.9.1/test/data/testrepo.git/objects/97/d615e1bc273c40c94a726814e7b93fdb5a1b36
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/a0/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      184 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/a0/75f5a7394b0838a9f54dfc511e1a3fbbb3b973
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/ab/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       34 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/ab/533997b80705767be3dae8cbb06a0740809f79
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/c2/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      149 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/c2/c2f6b06efdb6c1e4b1337811f0629fc0cadbd1
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/cc/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      178 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/cc/ca47fbb26183e71a7a46d165299b84e2e6c0b3
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/d8/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       37 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/d8/79714d880671ed84f8aaed8b27fca23ba01f27
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/f5/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      172 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/objects/f5/e5aa4e36ab0fe62ee1ccc6eb8f79b866863b87
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/info/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       54 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/info/packs
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/objects/pack/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1184 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/pack/pack-822653eb59791a6df714f8aa5fbf9f1c1951478e.idx
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      272 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/objects/pack/pack-822653eb59791a6df714f8aa5fbf9f1c1951478e.pack
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       85 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/packed-refs
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.083077 pygit2-1.9.1/test/data/testrepo.git/refs/
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/refs/heads/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       41 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/refs/heads/master
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/refs/notes/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       41 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepo.git/refs/notes/commits
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/data/testrepo.git/refs/tags/
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)       41 2013-03-02 10:50:05.000000 pygit2-1.9.1/test/data/testrepo.git/refs/tags/root
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    61440 2022-03-19 10:46:31.964542 pygit2-1.9.1/test/data/testrepo.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    92160 2015-01-26 17:11:50.330435 pygit2-1.9.1/test/data/testrepoformerging.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    61440 2020-11-28 15:06:42.105829 pygit2-1.9.1/test/data/testrepopacked.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    51200 2021-10-31 08:03:08.201437 pygit2-1.9.1/test/data/trailerrepo.tar
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    51200 2018-02-03 10:59:22.637729 pygit2-1.9.1/test/data/utf8branchrepo.tar
-drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-03-22 19:11:49.091077 pygit2-1.9.1/test/keys/
--rw-------   0 jdavid    (1001) jdavid    (1001)     2655 2020-05-02 09:23:03.664771 pygit2-1.9.1/test/keys/pygit2_empty
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)      566 2020-05-02 09:23:03.664771 pygit2-1.9.1/test/keys/pygit2_empty.pub
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4885 2022-03-20 08:43:45.006981 pygit2-1.9.1/test/test_apply_diff.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2396 2022-03-20 08:22:52.658377 pygit2-1.9.1/test/test_archive.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1915 2022-03-20 08:24:08.403258 pygit2-1.9.1/test/test_attributes.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4915 2021-09-17 11:25:20.007411 pygit2-1.9.1/test/test_blame.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5630 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_blob.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     8799 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_branch.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4173 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_branch_empty.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2348 2022-03-20 08:25:33.085441 pygit2-1.9.1/test/test_cherrypick.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    10090 2022-01-26 15:20:11.883729 pygit2-1.9.1/test/test_commit.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2871 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_commit_gpg.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1814 2021-10-31 08:03:08.201437 pygit2-1.9.1/test/test_commit_trailer.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5747 2022-03-20 08:49:27.825108 pygit2-1.9.1/test/test_config.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6427 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_credentials.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4133 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_describe.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    11541 2022-03-14 08:12:15.951593 pygit2-1.9.1/test/test_diff.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2198 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_diff_binary.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     8313 2022-03-20 08:26:12.830957 pygit2-1.9.1/test/test_index.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3520 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_mailmap.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9954 2022-03-20 08:27:29.597894 pygit2-1.9.1/test/test_merge.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2747 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_note.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4507 2021-09-17 11:25:20.011411 pygit2-1.9.1/test/test_object.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2694 2022-03-20 08:28:44.478738 pygit2-1.9.1/test/test_odb.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4287 2022-03-20 08:31:34.864454 pygit2-1.9.1/test/test_odb_backend.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2549 2021-09-17 11:25:20.015411 pygit2-1.9.1/test/test_oid.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4164 2021-09-17 11:25:20.015411 pygit2-1.9.1/test/test_options.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4122 2022-03-20 08:43:57.111059 pygit2-1.9.1/test/test_packbuilder.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6751 2021-09-17 11:25:20.015411 pygit2-1.9.1/test/test_patch.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2626 2021-09-17 11:25:20.015411 pygit2-1.9.1/test/test_patch_encoding.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4421 2022-03-20 08:35:53.082658 pygit2-1.9.1/test/test_refdb_backend.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    22428 2022-03-20 08:37:58.044605 pygit2-1.9.1/test/test_refs.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9330 2022-03-19 10:47:20.565374 pygit2-1.9.1/test/test_remote.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2523 2022-03-20 08:38:59.005046 pygit2-1.9.1/test/test_remote_prune.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1488 2021-09-17 11:25:20.015411 pygit2-1.9.1/test/test_remote_utf8.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)    21598 2022-03-20 20:45:43.136061 pygit2-1.9.1/test/test_repository.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     7278 2022-03-20 08:43:07.478738 pygit2-1.9.1/test/test_repository_bare.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2128 2022-03-20 08:40:03.038498 pygit2-1.9.1/test/test_repository_custom.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1418 2021-09-17 11:25:20.015411 pygit2-1.9.1/test/test_repository_empty.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3345 2021-09-17 11:25:20.019411 pygit2-1.9.1/test/test_revparse.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3922 2021-09-17 11:25:20.019411 pygit2-1.9.1/test/test_revwalk.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3182 2022-03-22 08:46:40.405650 pygit2-1.9.1/test/test_signature.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1470 2021-09-17 11:25:20.019411 pygit2-1.9.1/test/test_status.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3779 2022-03-20 07:43:53.770506 pygit2-1.9.1/test/test_submodule.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3190 2021-09-17 11:25:20.019411 pygit2-1.9.1/test/test_tag.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6926 2021-09-17 11:25:20.019411 pygit2-1.9.1/test/test_tree.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2092 2021-09-17 11:25:20.019411 pygit2-1.9.1/test/test_treebuilder.py
--rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4545 2022-03-20 07:27:15.959589 pygit2-1.9.1/test/utils.py
+drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-05-24 20:01:01.317232 pygit2-1.9.2/
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3341 2022-05-24 17:30:26.409273 pygit2-1.9.2/AUTHORS.rst
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    54088 2022-05-24 17:37:54.913962 pygit2-1.9.2/CHANGELOG.rst
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    19054 2021-09-17 11:25:19.987411 pygit2-1.9.2/COPYING
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      117 2022-04-14 06:24:00.331925 pygit2-1.9.2/Makefile
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3496 2022-05-24 20:01:01.317232 pygit2-1.9.2/PKG-INFO
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2363 2021-12-06 08:47:08.838489 pygit2-1.9.2/README.rst
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      253 2022-02-23 12:38:08.106666 pygit2-1.9.2/SPONSORS.rst
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     7742 2022-04-23 08:00:11.739299 pygit2-1.9.2/build.sh
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      156 2021-06-19 09:31:42.533738 pygit2-1.9.2/build_tag.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      461 2022-03-06 08:26:49.549038 pygit2-1.9.2/mypy-stubtest.ini
+drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-05-24 20:01:01.311232 pygit2-1.9.2/pygit2/
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     8224 2021-09-17 11:25:19.987411 pygit2-1.9.2/pygit2/__init__.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2352 2022-05-24 17:31:39.134028 pygit2-1.9.2/pygit2/_build.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    20561 2022-05-06 06:07:20.948192 pygit2-1.9.2/pygit2/_pygit2.pyi
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2706 2022-03-19 10:40:15.425663 pygit2-1.9.2/pygit2/_run.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4107 2021-09-17 11:25:19.987411 pygit2-1.9.2/pygit2/blame.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    15783 2022-01-29 07:18:52.169225 pygit2-1.9.2/pygit2/callbacks.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    11092 2021-09-17 11:25:19.991411 pygit2-1.9.2/pygit2/config.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3938 2021-09-17 11:25:19.991411 pygit2-1.9.2/pygit2/credentials.py
+drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-05-24 20:01:01.313232 pygit2-1.9.2/pygit2/decl/
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      451 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/attr.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1051 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/blame.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      112 2022-02-14 07:53:46.471747 pygit2-1.9.2/pygit2/decl/buffer.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      963 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/callbacks.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1826 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/checkout.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      952 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/clone.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      261 2021-10-20 07:44:38.815929 pygit2-1.9.2/pygit2/decl/commit.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      188 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/common.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2149 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/config.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1228 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/describe.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2114 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/diff.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      937 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/errors.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      128 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/graph.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2331 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/index.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      356 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/indexer.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2139 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/merge.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)       84 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/net.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      309 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/oid.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      747 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/pack.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      411 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/proxy.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      615 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/refspec.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4855 2022-02-14 07:51:50.249861 pygit2-1.9.2/pygit2/decl/remote.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2135 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/repository.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      183 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/revert.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1688 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/stash.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      124 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/strarray.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1270 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/submodule.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1520 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/transport.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1554 2021-06-19 09:40:24.646733 pygit2-1.9.2/pygit2/decl/types.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2362 2021-09-17 11:25:19.991411 pygit2-1.9.2/pygit2/errors.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1246 2021-09-17 11:25:19.991411 pygit2-1.9.2/pygit2/ffi.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    14886 2021-09-17 11:25:19.991411 pygit2-1.9.2/pygit2/index.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2821 2021-09-17 11:25:19.991411 pygit2-1.9.2/pygit2/packbuilder.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3427 2021-09-17 11:25:19.991411 pygit2-1.9.2/pygit2/refspec.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    13240 2022-04-26 18:55:32.101869 pygit2-1.9.2/pygit2/remote.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    55966 2022-03-14 08:15:20.348721 pygit2-1.9.2/pygit2/repository.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6897 2021-09-17 11:25:19.995411 pygit2-1.9.2/pygit2/settings.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2635 2021-09-17 11:25:19.995411 pygit2-1.9.2/pygit2/submodule.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3664 2021-09-17 11:25:19.995411 pygit2-1.9.2/pygit2/utils.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)       50 2020-03-11 08:34:41.877181 pygit2-1.9.2/pyproject.toml
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)       64 2021-09-17 11:25:19.995411 pygit2-1.9.2/pytest.ini
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)       18 2021-11-06 12:09:47.575052 pygit2-1.9.2/requirements-test.txt
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)       52 2022-02-23 12:39:10.615412 pygit2-1.9.2/requirements.txt
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)       89 2021-10-08 08:39:16.348105 pygit2-1.9.2/setup.cfg
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5605 2022-03-20 20:36:06.725472 pygit2-1.9.2/setup.py
+drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-05-24 20:01:01.314232 pygit2-1.9.2/src/
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9210 2022-03-14 08:11:42.421751 pygit2-1.9.2/src/blob.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    10311 2022-03-14 08:11:42.422752 pygit2-1.9.2/src/branch.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1624 2022-01-26 17:46:27.227020 pygit2-1.9.2/src/branch.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    11661 2022-03-14 08:11:42.422752 pygit2-1.9.2/src/commit.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    39812 2022-03-14 08:11:42.426751 pygit2-1.9.2/src/diff.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1657 2022-01-26 17:46:27.227020 pygit2-1.9.2/src/diff.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4509 2022-03-14 08:11:42.427751 pygit2-1.9.2/src/error.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1674 2021-09-17 11:25:19.999411 pygit2-1.9.2/src/error.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9133 2022-03-14 08:11:42.430751 pygit2-1.9.2/src/mailmap.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1425 2022-01-26 17:53:30.098494 pygit2-1.9.2/src/mailmap.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9299 2022-03-14 08:11:42.430751 pygit2-1.9.2/src/note.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1470 2021-09-17 11:25:19.999411 pygit2-1.9.2/src/note.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    12056 2022-03-14 08:11:42.431751 pygit2-1.9.2/src/object.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1628 2022-01-26 17:46:27.227020 pygit2-1.9.2/src/object.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    12017 2022-03-14 08:11:42.431751 pygit2-1.9.2/src/odb.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1533 2021-09-17 11:25:19.999411 pygit2-1.9.2/src/odb.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    25493 2022-03-14 08:11:42.432751 pygit2-1.9.2/src/odb_backend.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1446 2021-09-17 11:25:19.999411 pygit2-1.9.2/src/odb_backend.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9046 2022-03-14 08:11:42.432751 pygit2-1.9.2/src/oid.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1620 2021-09-17 11:25:19.999411 pygit2-1.9.2/src/oid.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9842 2022-03-14 08:11:42.433751 pygit2-1.9.2/src/options.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1932 2021-09-17 11:25:20.003411 pygit2-1.9.2/src/options.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9858 2022-03-14 08:11:42.433751 pygit2-1.9.2/src/patch.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1425 2021-09-17 11:25:20.003411 pygit2-1.9.2/src/patch.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    22004 2022-03-14 08:11:42.434751 pygit2-1.9.2/src/pygit2.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6958 2022-03-14 08:11:42.434751 pygit2-1.9.2/src/refdb.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1416 2021-06-19 09:40:24.646733 pygit2-1.9.2/src/refdb.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    29161 2022-03-14 08:11:42.435751 pygit2-1.9.2/src/refdb_backend.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1456 2021-06-19 09:40:24.642733 pygit2-1.9.2/src/refdb_backend.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    23014 2022-03-14 08:11:42.435751 pygit2-1.9.2/src/reference.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1622 2022-01-26 17:46:27.227020 pygit2-1.9.2/src/reference.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    70044 2022-05-06 06:07:20.948192 pygit2-1.9.2/src/repository.c
+-rwxr-xr-x   0 jdavid    (1001) jdavid    (1001)     3487 2022-05-06 06:07:20.948192 pygit2-1.9.2/src/repository.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5985 2022-03-14 08:11:42.436751 pygit2-1.9.2/src/revspec.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1442 2021-09-17 11:25:20.003411 pygit2-1.9.2/src/revspec.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    10093 2022-03-22 08:46:40.405650 pygit2-1.9.2/src/signature.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1492 2022-01-26 17:46:27.228020 pygit2-1.9.2/src/signature.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5967 2022-03-14 08:11:42.436751 pygit2-1.9.2/src/stash.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6681 2022-03-14 08:11:42.436751 pygit2-1.9.2/src/tag.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    18899 2022-03-14 08:11:42.436751 pygit2-1.9.2/src/tree.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1451 2022-01-26 17:46:27.228020 pygit2-1.9.2/src/tree.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     7413 2022-03-14 08:11:42.437751 pygit2-1.9.2/src/treebuilder.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1619 2021-09-17 11:25:20.007411 pygit2-1.9.2/src/treebuilder.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5507 2022-02-14 07:38:49.754672 pygit2-1.9.2/src/types.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6403 2022-03-14 08:11:42.437751 pygit2-1.9.2/src/utils.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5235 2021-09-17 11:25:20.007411 pygit2-1.9.2/src/utils.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6717 2022-03-14 08:11:42.437751 pygit2-1.9.2/src/walker.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1698 2021-09-17 11:25:20.007411 pygit2-1.9.2/src/walker.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9488 2022-03-14 08:11:42.437751 pygit2-1.9.2/src/wildmatch.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      501 2021-06-19 09:40:24.646733 pygit2-1.9.2/src/wildmatch.h
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6090 2022-03-14 08:11:42.438751 pygit2-1.9.2/src/worktree.c
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1449 2021-09-17 11:25:20.007411 pygit2-1.9.2/src/worktree.h
+drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-05-24 20:01:01.316232 pygit2-1.9.2/test/
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1482 2022-03-22 17:53:02.953378 pygit2-1.9.2/test/__init__.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2432 2022-05-24 17:39:04.882668 pygit2-1.9.2/test/conftest.py
+drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-05-24 20:01:01.317232 pygit2-1.9.2/test/data/
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    19195 2022-05-05 14:36:05.881153 pygit2-1.9.2/test/data/barerepo.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    16243 2022-04-23 16:14:30.408124 pygit2-1.9.2/test/data/binaryfilerepo.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    24164 2022-04-23 16:14:30.408124 pygit2-1.9.2/test/data/blameflagsrepo.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    18330 2022-04-23 16:14:30.408124 pygit2-1.9.2/test/data/dirtyrepo.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    10504 2022-05-05 14:36:05.881153 pygit2-1.9.2/test/data/emptyrepo.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    17199 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/data/encoding.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)   469796 2022-05-06 06:07:20.949192 pygit2-1.9.2/test/data/gpgsigned.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    19963 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/data/submodulerepo.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    19818 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/data/testrepo.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    29345 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/data/testrepoformerging.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    18105 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/data/testrepopacked.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    17433 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/data/trailerrepo.zip
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    17008 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/data/utf8branchrepo.zip
+drwxr-xr-x   0 jdavid    (1001) jdavid    (1001)        0 2022-05-24 20:01:01.317232 pygit2-1.9.2/test/keys/
+-rw-------   0 jdavid    (1001) jdavid    (1001)     2655 2020-05-02 09:23:03.664771 pygit2-1.9.2/test/keys/pygit2_empty
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)      566 2020-05-02 09:23:03.664771 pygit2-1.9.2/test/keys/pygit2_empty.pub
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4885 2022-03-20 08:43:45.006981 pygit2-1.9.2/test/test_apply_diff.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2396 2022-03-20 08:22:52.658377 pygit2-1.9.2/test/test_archive.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1915 2022-03-20 08:24:08.403258 pygit2-1.9.2/test/test_attributes.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4915 2021-09-17 11:25:20.007411 pygit2-1.9.2/test/test_blame.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5630 2021-09-17 11:25:20.011411 pygit2-1.9.2/test/test_blob.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     8799 2021-09-17 11:25:20.011411 pygit2-1.9.2/test/test_branch.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4173 2021-09-17 11:25:20.011411 pygit2-1.9.2/test/test_branch_empty.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2348 2022-03-20 08:25:33.085441 pygit2-1.9.2/test/test_cherrypick.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    10090 2022-01-26 15:20:11.883729 pygit2-1.9.2/test/test_commit.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5443 2022-05-06 06:07:20.950192 pygit2-1.9.2/test/test_commit_gpg.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1814 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/test_commit_trailer.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     5747 2022-03-20 08:49:27.825108 pygit2-1.9.2/test/test_config.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6427 2021-09-17 11:25:20.011411 pygit2-1.9.2/test/test_credentials.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4133 2021-09-17 11:25:20.011411 pygit2-1.9.2/test/test_describe.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    11541 2022-03-14 08:12:15.951593 pygit2-1.9.2/test/test_diff.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2198 2022-04-23 16:14:30.409124 pygit2-1.9.2/test/test_diff_binary.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     8313 2022-04-23 16:14:30.410124 pygit2-1.9.2/test/test_index.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3520 2021-09-17 11:25:20.011411 pygit2-1.9.2/test/test_mailmap.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9954 2022-03-20 08:27:29.597894 pygit2-1.9.2/test/test_merge.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2747 2021-09-17 11:25:20.011411 pygit2-1.9.2/test/test_note.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4507 2021-09-17 11:25:20.011411 pygit2-1.9.2/test/test_object.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2674 2022-05-05 14:36:05.882153 pygit2-1.9.2/test/test_odb.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4231 2022-05-05 14:36:05.882153 pygit2-1.9.2/test/test_odb_backend.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2549 2021-09-17 11:25:20.015411 pygit2-1.9.2/test/test_oid.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4164 2021-09-17 11:25:20.015411 pygit2-1.9.2/test/test_options.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4122 2022-04-23 16:14:30.410124 pygit2-1.9.2/test/test_packbuilder.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6751 2021-09-17 11:25:20.015411 pygit2-1.9.2/test/test_patch.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2626 2021-09-17 11:25:20.015411 pygit2-1.9.2/test/test_patch_encoding.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4421 2022-03-20 08:35:53.082658 pygit2-1.9.2/test/test_refdb_backend.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    22428 2022-03-20 08:37:58.044605 pygit2-1.9.2/test/test_refs.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     9330 2022-05-05 14:36:05.882153 pygit2-1.9.2/test/test_remote.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2523 2022-03-20 08:38:59.005046 pygit2-1.9.2/test/test_remote_prune.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1488 2022-04-23 16:14:30.410124 pygit2-1.9.2/test/test_remote_utf8.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)    21223 2022-05-05 14:36:05.882153 pygit2-1.9.2/test/test_repository.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     7278 2022-03-20 08:43:07.478738 pygit2-1.9.2/test/test_repository_bare.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2128 2022-03-20 08:40:03.038498 pygit2-1.9.2/test/test_repository_custom.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1418 2021-09-17 11:25:20.015411 pygit2-1.9.2/test/test_repository_empty.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3345 2021-09-17 11:25:20.019411 pygit2-1.9.2/test/test_revparse.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3922 2021-09-17 11:25:20.019411 pygit2-1.9.2/test/test_revwalk.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3182 2022-03-22 08:46:40.405650 pygit2-1.9.2/test/test_signature.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     1470 2021-09-17 11:25:20.019411 pygit2-1.9.2/test/test_status.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3779 2022-04-23 16:14:30.410124 pygit2-1.9.2/test/test_submodule.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     3190 2021-09-17 11:25:20.019411 pygit2-1.9.2/test/test_tag.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     6926 2021-09-17 11:25:20.019411 pygit2-1.9.2/test/test_tree.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     2092 2021-09-17 11:25:20.019411 pygit2-1.9.2/test/test_treebuilder.py
+-rw-r--r--   0 jdavid    (1001) jdavid    (1001)     4678 2022-04-23 16:14:30.410124 pygit2-1.9.2/test/utils.py
```

### Comparing `pygit2-1.9.1/AUTHORS.rst` & `pygit2-1.9.2/AUTHORS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,15 @@
   Huang Huang
   Ian P. McCullough
   Igor Gnatenko
   Insomnia
   Jack O'Connor
   Jared Flatow
   Jeremy Heiner
+  Jesse P. Johnson
   Jiunn Haur Lim
   Jorge C. Leitao
   Jun Omae
   Kaarel Kitsemets
   Ken Dreyer
   Kevin KIN-FOO
   Marcel Waldvogel
@@ -109,14 +110,15 @@
   Sarath Lakshman
   Steve Kieffer
   Szucs Krisztian
   Vicent Marti
   Zbigniew Jędrzejewski-Szmek
   Zoran Zaric
   Adam Spiers
+  Alexandru Fikl
   Andrew Chin
   Andrey Trubachev
   András Veres-Szentkirályi
   Ash Berlin
   Benjamin Kircher
   Benjamin Pollack
   Benjamin Wohlwend
```

### Comparing `pygit2-1.9.1/CHANGELOG.rst` & `pygit2-1.9.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+1.9.2 (2022-05-24)
+-------------------------
+
+- New ``Repository.create_commit_string(...)`` and
+  ``Repository.create_commit_with_signature(...)``
+  `#1142 <https://github.com/libgit2/pygit2/pull/1142>`_
+
+- Linux and macOS wheels updated to libgit2 v1.4.3
+
+- Remove redundant line
+  `#1139 <https://github.com/libgit2/pygit2/pull/1139>`_
+
+
 1.9.1 (2022-03-22)
 -------------------------
 
 - Type hints: added to C code and Branches/References
   `#1121 <https://github.com/libgit2/pygit2/pull/1121>`_
   `#1132 <https://github.com/libgit2/pygit2/pull/1132>`_
```

### Comparing `pygit2-1.9.1/COPYING` & `pygit2-1.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/PKG-INFO` & `pygit2-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygit2
-Version: 1.9.1
+Version: 1.9.2
 Summary: Python bindings for libgit2.
 Home-page: https://github.com/libgit2/pygit2
 Maintainer: J. David Ibáñez
 Maintainer-email: jdavid.ibp@gmail.com
 License: GPLv2 with linking exception
 Project-URL: Documentation, https://www.pygit2.org/
 Project-URL: Changelog, https://github.com/libgit2/pygit2/blob/master/CHANGELOG.rst
```

### Comparing `pygit2-1.9.1/README.rst` & `pygit2-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/build.sh` & `pygit2-1.9.2/build.sh`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 #
 # Examples.
 #
 # Build inplace, libgit2 must be available in the path:
 #
 #   sh build.sh
 #
-# Build libgit2 1.4.2 (will use libssh2 if available), then build pygit2
+# Build libgit2 1.4.3 (will use libssh2 if available), then build pygit2
 # inplace:
 #
-#   LIBGIT2_VERSION=1.4.2 sh build.sh
+#   LIBGIT2_VERSION=1.4.3 sh build.sh
 #
-# Build libssh2 1.10.0 and libgit2 1.4.2, then build pygit2 inplace:
+# Build libssh2 1.10.0 and libgit2 1.4.3, then build pygit2 inplace:
 #
-#   LIBSSH2_VERSION=1.10.0 LIBGIT2_VERSION=1.4.2 sh build.sh
+#   LIBSSH2_VERSION=1.10.0 LIBGIT2_VERSION=1.4.3 sh build.sh
 #
-# Tell where libssh2 is installed, build libgit2 1.4.2, then build pygit2
+# Tell where libssh2 is installed, build libgit2 1.4.3, then build pygit2
 # inplace:
 #
-#   LIBSSH2_PREFIX=/usr/local LIBGIT2_VERSION=1.4.2 sh build.sh
+#   LIBSSH2_PREFIX=/usr/local LIBGIT2_VERSION=1.4.3 sh build.sh
 #
 # Build inplace and run the tests:
 #
 #   sh build.sh test
 #
 # Build a wheel:
 #
```

### Comparing `pygit2-1.9.1/pygit2/__init__.py` & `pygit2-1.9.2/pygit2/__init__.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/_build.py` & `pygit2-1.9.2/pygit2/_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Import from the Standard Library
 import os
 from pathlib import Path
 
 #
 # The version number of pygit2
 #
-__version__ = '1.9.1'
+__version__ = '1.9.2'
 
 
 #
 # Utility functions to get the paths required for bulding extensions
 #
 def _get_libgit2_path():
     # LIBGIT2 environment variable takes precedence
```

### Comparing `pygit2-1.9.1/pygit2/_pygit2.pyi` & `pygit2-1.9.2/pygit2/_pygit2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterator
+from typing import Iterator, Optional
 from io import IOBase
 from . import Index, Submodule
 
 GIT_APPLY_LOCATION_BOTH: int
 GIT_APPLY_LOCATION_INDEX: int
 GIT_APPLY_LOCATION_WORKDIR: int
 GIT_BLAME_FIRST_PARENT: int
@@ -455,14 +455,16 @@
     def compress_references(self) -> None: ...
     def create_blob(self, data: bytes) -> Oid: ...
     def create_blob_fromdisk(self, path: str) -> Oid: ...
     def create_blob_fromiobase(self, iobase: IOBase) -> Oid: ...
     def create_blob_fromworkdir(self, path: str) -> Oid: ...
     def create_branch(self, name: str, commit: Commit, force = False) -> Branch: ...
     def create_commit(self, reference_name: str, author: Signature, committer: Signature, message: str, tree: _OidArg, parents: list[_OidArg], encoding: str = ...) -> Oid: ...
+    def create_commit_string(self, author: Signature, committer: Signature, message: str, tree: _OidArg, parents: list[_OidArg], encoding: str = ...) -> Oid: ...
+    def create_commit_with_signature(self, content: str, signature: str, signature_field: Optional[str] = None) -> Oid: ...
     def create_note(self, message: str, author: Signature, committer: Signature, annotated_id: str, ref: str = "refs/notes/commits", force: bool = False) -> Oid: ...
     def create_reference_direct(self, name: str, target: _OidArg, force: bool, message: str = None) -> Reference: ...
     def create_reference_symbolic(self, name: str, target: str, force: bool, message: str = None) -> Reference: ...
     def create_tag(self, name: str, oid: _OidArg, type: int, tagger: Signature, message: str) -> Oid: ...
     def descendant_of(self, oid1: _OidArg, oid2: _OidArg) -> bool: ...
     def expand_id(self, hex: str) -> Oid: ...
     def free(self) -> None: ...
```

### Comparing `pygit2-1.9.1/pygit2/_run.py` & `pygit2-1.9.2/pygit2/_run.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/blame.py` & `pygit2-1.9.2/pygit2/blame.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/callbacks.py` & `pygit2-1.9.2/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/config.py` & `pygit2-1.9.2/pygit2/config.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/credentials.py` & `pygit2-1.9.2/pygit2/credentials.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/blame.h` & `pygit2-1.9.2/pygit2/decl/blame.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/callbacks.h` & `pygit2-1.9.2/pygit2/decl/callbacks.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/checkout.h` & `pygit2-1.9.2/pygit2/decl/checkout.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/clone.h` & `pygit2-1.9.2/pygit2/decl/clone.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/config.h` & `pygit2-1.9.2/pygit2/decl/config.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/describe.h` & `pygit2-1.9.2/pygit2/decl/describe.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/diff.h` & `pygit2-1.9.2/pygit2/decl/diff.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/errors.h` & `pygit2-1.9.2/pygit2/decl/errors.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/index.h` & `pygit2-1.9.2/pygit2/decl/index.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/merge.h` & `pygit2-1.9.2/pygit2/decl/merge.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/pack.h` & `pygit2-1.9.2/pygit2/decl/pack.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/refspec.h` & `pygit2-1.9.2/pygit2/decl/refspec.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/remote.h` & `pygit2-1.9.2/pygit2/decl/remote.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/repository.h` & `pygit2-1.9.2/pygit2/decl/repository.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/stash.h` & `pygit2-1.9.2/pygit2/decl/stash.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/submodule.h` & `pygit2-1.9.2/pygit2/decl/submodule.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/transport.h` & `pygit2-1.9.2/pygit2/decl/transport.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/decl/types.h` & `pygit2-1.9.2/pygit2/decl/types.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/errors.py` & `pygit2-1.9.2/pygit2/errors.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/ffi.py` & `pygit2-1.9.2/pygit2/ffi.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/index.py` & `pygit2-1.9.2/pygit2/index.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/packbuilder.py` & `pygit2-1.9.2/pygit2/packbuilder.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/refspec.py` & `pygit2-1.9.2/pygit2/refspec.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/remote.py` & `pygit2-1.9.2/pygit2/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,14 @@
         proxy : None or True or str
             Proxy configuration. Can be one of:
 
             * `None` (the default) to disable proxy usage
             * `True` to enable automatic proxy detection
             * an url to a proxy (`http://proxy.example.org:3128/`)
         """
-        message = to_bytes(message)
         with git_fetch_options(callbacks) as payload:
             opts = payload.fetch_options
             opts.prune = prune
             self.__set_proxy(opts.proxy_opts, proxy)
             with StrArray(refspecs) as arr:
                 err = C.git_remote_fetch(self._remote, arr, opts, to_bytes(message))
                 payload.check_error(err)
```

### Comparing `pygit2-1.9.1/pygit2/repository.py` & `pygit2-1.9.2/pygit2/repository.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/settings.py` & `pygit2-1.9.2/pygit2/settings.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/submodule.py` & `pygit2-1.9.2/pygit2/submodule.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/pygit2/utils.py` & `pygit2-1.9.2/pygit2/utils.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/setup.py` & `pygit2-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/blob.c` & `pygit2-1.9.2/src/blob.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/branch.c` & `pygit2-1.9.2/src/branch.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/branch.h` & `pygit2-1.9.2/src/branch.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/commit.c` & `pygit2-1.9.2/src/commit.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/diff.c` & `pygit2-1.9.2/src/diff.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/diff.h` & `pygit2-1.9.2/src/diff.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/error.c` & `pygit2-1.9.2/src/error.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/error.h` & `pygit2-1.9.2/src/error.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/mailmap.c` & `pygit2-1.9.2/src/mailmap.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/mailmap.h` & `pygit2-1.9.2/src/mailmap.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/note.c` & `pygit2-1.9.2/src/note.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/note.h` & `pygit2-1.9.2/src/note.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/object.c` & `pygit2-1.9.2/src/object.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/object.h` & `pygit2-1.9.2/src/object.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/odb.c` & `pygit2-1.9.2/src/odb.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/odb.h` & `pygit2-1.9.2/src/odb.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/odb_backend.c` & `pygit2-1.9.2/src/odb_backend.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/odb_backend.h` & `pygit2-1.9.2/src/odb_backend.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/oid.c` & `pygit2-1.9.2/src/oid.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/oid.h` & `pygit2-1.9.2/src/oid.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/options.c` & `pygit2-1.9.2/src/options.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/options.h` & `pygit2-1.9.2/src/options.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/patch.c` & `pygit2-1.9.2/src/patch.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/patch.h` & `pygit2-1.9.2/src/patch.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/pygit2.c` & `pygit2-1.9.2/src/pygit2.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/refdb.c` & `pygit2-1.9.2/src/refdb.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/refdb.h` & `pygit2-1.9.2/src/refdb.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/refdb_backend.c` & `pygit2-1.9.2/src/refdb_backend.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/refdb_backend.h` & `pygit2-1.9.2/src/refdb_backend.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/reference.c` & `pygit2-1.9.2/src/reference.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/reference.h` & `pygit2-1.9.2/src/reference.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/repository.c` & `pygit2-1.9.2/src/repository.c`

 * *Files 2% similar despite different names*

```diff
@@ -1106,14 +1106,123 @@
         i--;
         git_commit_free(parents[i]);
     }
     free(parents);
     return py_result;
 }
 
+PyDoc_STRVAR(Repository_create_commit_string__doc__,
+  "create_commit_string(author: Signature, committer: Signature, message: bytes | str, tree: Oid, parents: list[Oid][, encoding: str]) -> str\n"
+  "\n"
+  "Create a new commit but return it as a string.");
+
+PyObject *
+Repository_create_commit_string(Repository *self, PyObject *args)
+{
+    Signature *py_author, *py_committer;
+    PyObject *py_oid, *py_message, *py_parents, *py_parent;
+    PyObject *str;
+    char *encoding = NULL;
+    git_oid oid;
+    git_tree *tree = NULL;
+    int parent_count;
+    git_commit **parents = NULL;
+    git_buf buf = { 0 };
+    int i = 0;
+
+    if (!PyArg_ParseTuple(args, "O!O!OOO!|s",
+                          &SignatureType, &py_author,
+                          &SignatureType, &py_committer,
+                          &py_message,
+                          &py_oid,
+                          &PyList_Type, &py_parents,
+                          &encoding))
+        return NULL;
+
+    size_t len = py_oid_to_git_oid(py_oid, &oid);
+    if (len == 0)
+        return NULL;
+
+    PyObject *tmessage;
+    const char *message = pgit_borrow_encoding(py_message, encoding, NULL, &tmessage);
+    if (message == NULL)
+        return NULL;
+
+    int err = git_tree_lookup_prefix(&tree, self->repo, &oid, len);
+    if (err < 0) {
+        Error_set(err);
+        goto out;
+    }
+
+    parent_count = (int)PyList_Size(py_parents);
+    parents = malloc(parent_count * sizeof(git_commit*));
+    if (parents == NULL) {
+        PyErr_SetNone(PyExc_MemoryError);
+        goto out;
+    }
+    for (; i < parent_count; i++) {
+        py_parent = PyList_GET_ITEM(py_parents, i);
+        len = py_oid_to_git_oid(py_parent, &oid);
+        if (len == 0)
+            goto out;
+        err = git_commit_lookup_prefix(&parents[i], self->repo, &oid, len);
+        if (err < 0) {
+            Error_set(err);
+            goto out;
+        }
+    }
+
+    err = git_commit_create_buffer(&buf, self->repo,
+                                   py_author->signature, py_committer->signature,
+                                   encoding, message, tree, parent_count,
+                                   (const git_commit**)parents);
+    if (err < 0) {
+        Error_set(err);
+        goto out;
+    }
+
+    str = to_unicode_n(buf.ptr, buf.size, NULL, NULL);
+    git_buf_dispose(&buf);
+
+out:
+    Py_DECREF(tmessage);
+    git_tree_free(tree);
+    while (i > 0) {
+        i--;
+        git_commit_free(parents[i]);
+    }
+    free(parents);
+    return str;
+}
+
+PyDoc_STRVAR(Repository_create_commit_with_signature__doc__,
+  "create_commit_with_signature(content: str, signature: str, field_name: str) -> Oid\n"
+  "\n"
+  "Create a new signed commit object, return its oid.");
+
+PyObject *
+Repository_create_commit_with_signature(Repository *self, PyObject *args)
+{
+    git_oid oid;
+    char *content, *signature;
+    char *signature_field = NULL;
+
+    if (!PyArg_ParseTuple(args, "ss|s", &content, &signature, &signature_field))
+        return NULL;
+
+    int err = git_commit_create_with_signature(&oid, self->repo, content,
+                                               signature, signature_field);
+
+    if (err < 0) {
+        Error_set(err);
+        return NULL;
+    }
+
+    return git_oid_to_python(&oid);
+}
 
 PyDoc_STRVAR(Repository_create_tag__doc__,
   "create_tag(name: str, oid: Oid, type: int, tagger: Signature[, message: str]) -> Oid\n"
   "\n"
   "Create a new tag object, return its oid.");
 
 PyObject *
@@ -2273,14 +2382,16 @@
 
 PyMethodDef Repository_methods[] = {
     METHOD(Repository, create_blob, METH_VARARGS),
     METHOD(Repository, create_blob_fromworkdir, METH_O),
     METHOD(Repository, create_blob_fromdisk, METH_VARARGS),
     METHOD(Repository, create_blob_fromiobase, METH_O),
     METHOD(Repository, create_commit, METH_VARARGS),
+    METHOD(Repository, create_commit_string, METH_VARARGS),
+    METHOD(Repository, create_commit_with_signature, METH_VARARGS),
     METHOD(Repository, create_tag, METH_VARARGS),
     METHOD(Repository, TreeBuilder, METH_VARARGS),
     METHOD(Repository, walk, METH_VARARGS),
     METHOD(Repository, descendant_of, METH_VARARGS),
     METHOD(Repository, merge_base, METH_VARARGS),
     METHOD(Repository, merge_base_many, METH_VARARGS),
     METHOD(Repository, merge_base_octopus, METH_VARARGS),
```

### Comparing `pygit2-1.9.1/src/repository.h` & `pygit2-1.9.2/src/repository.h`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 int  Repository_traverse(Repository *self, visitproc visit, void *arg);
 int  Repository_clear(Repository *self);
 
 PyObject* Repository_walk(Repository *self, PyObject *args);
 PyObject* Repository_create_blob(Repository *self, PyObject *args);
 PyObject* Repository_create_blob_fromdisk(Repository *self, PyObject *args);
 PyObject* Repository_create_commit(Repository *self, PyObject *args);
+PyObject* Repository_create_commit_string(Repository *self, PyObject *args);
+PyObject* Repository_create_commit_with_signature(Repository *self, PyObject *args);
 PyObject* Repository_create_tag(Repository *self, PyObject *args);
 PyObject* Repository_create_branch(Repository *self, PyObject *args);
 PyObject* Repository_listall_references(Repository *self, PyObject *args);
 PyObject* Repository_listall_reference_objects(Repository *self,
                                                PyObject *args);
 PyObject* Repository_listall_branches(Repository *self, PyObject *args);
 PyObject* Repository_lookup_reference(Repository *self, PyObject *py_name);
```

### Comparing `pygit2-1.9.1/src/revspec.c` & `pygit2-1.9.2/src/revspec.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/revspec.h` & `pygit2-1.9.2/src/revspec.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/signature.c` & `pygit2-1.9.2/src/signature.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/signature.h` & `pygit2-1.9.2/src/signature.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/stash.c` & `pygit2-1.9.2/src/stash.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/tag.c` & `pygit2-1.9.2/src/tag.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/tree.c` & `pygit2-1.9.2/src/tree.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/tree.h` & `pygit2-1.9.2/src/tree.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/treebuilder.c` & `pygit2-1.9.2/src/treebuilder.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/treebuilder.h` & `pygit2-1.9.2/src/treebuilder.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/types.h` & `pygit2-1.9.2/src/types.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/utils.c` & `pygit2-1.9.2/src/utils.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/utils.h` & `pygit2-1.9.2/src/utils.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/walker.c` & `pygit2-1.9.2/src/walker.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/walker.h` & `pygit2-1.9.2/src/walker.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/wildmatch.c` & `pygit2-1.9.2/src/wildmatch.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/worktree.c` & `pygit2-1.9.2/src/worktree.c`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/src/worktree.h` & `pygit2-1.9.2/src/worktree.h`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/__init__.py` & `pygit2-1.9.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/conftest.py` & `pygit2-1.9.2/test/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,62 +22,71 @@
 def pygit2_empty_key():
     path = Path(__file__).parent / 'keys' / 'pygit2_empty'
     return path, f'{path}.pub', 'empty'
 
 
 @pytest.fixture
 def barerepo(tmp_path):
-    with utils.TemporaryRepository('testrepo.git', tmp_path) as path:
+    with utils.TemporaryRepository('barerepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 @pytest.fixture
 def barerepo_path(tmp_path):
-    with utils.TemporaryRepository('testrepo.git', tmp_path) as path:
+    with utils.TemporaryRepository('barerepo.zip', tmp_path) as path:
         yield pygit2.Repository(path), path
 
 
 @pytest.fixture
 def blameflagsrepo(tmp_path):
-    with utils.TemporaryRepository('blameflagsrepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('blameflagsrepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 @pytest.fixture
 def dirtyrepo(tmp_path):
-    with utils.TemporaryRepository('dirtyrepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('dirtyrepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 @pytest.fixture
-def emptyrepo(tmp_path):
-    with utils.TemporaryRepository('emptyrepo.tar', tmp_path) as path:
-        yield pygit2.Repository(path)
+def emptyrepo(barerepo, tmp_path):
+    with utils.TemporaryRepository('emptyrepo.zip', tmp_path) as path:
+        repo = pygit2.Repository(path)
+        repo.remotes.create('origin', barerepo.path)
+        yield repo
+
 
 @pytest.fixture
 def encodingrepo(tmp_path):
-    with utils.TemporaryRepository('encoding.tar', tmp_path) as path:
+    with utils.TemporaryRepository('encoding.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 @pytest.fixture
 def mergerepo(tmp_path):
-    with utils.TemporaryRepository('testrepoformerging.tar', tmp_path) as path:
+    with utils.TemporaryRepository('testrepoformerging.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 @pytest.fixture
 def testrepo(tmp_path):
-    with utils.TemporaryRepository('testrepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('testrepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 @pytest.fixture
 def testrepo_path(tmp_path):
-    with utils.TemporaryRepository('testrepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('testrepo.zip', tmp_path) as path:
         yield pygit2.Repository(path), path
 
 
 @pytest.fixture
 def testrepopacked(tmp_path):
-    with utils.TemporaryRepository('testrepopacked.tar', tmp_path) as path:
+    with utils.TemporaryRepository('testrepopacked.zip', tmp_path) as path:
+        yield pygit2.Repository(path)
+
+
+@pytest.fixture
+def gpgsigned(tmp_path):
+    with utils.TemporaryRepository('gpgsigned.zip', tmp_path) as path:
         yield pygit2.Repository(path)
```

### Comparing `pygit2-1.9.1/test/keys/pygit2_empty` & `pygit2-1.9.2/test/keys/pygit2_empty`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/keys/pygit2_empty.pub` & `pygit2-1.9.2/test/keys/pygit2_empty.pub`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_apply_diff.py` & `pygit2-1.9.2/test/test_apply_diff.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_archive.py` & `pygit2-1.9.2/test/test_archive.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_attributes.py` & `pygit2-1.9.2/test/test_attributes.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_blame.py` & `pygit2-1.9.2/test/test_blame.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_blob.py` & `pygit2-1.9.2/test/test_blob.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_branch.py` & `pygit2-1.9.2/test/test_branch.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_branch_empty.py` & `pygit2-1.9.2/test/test_branch_empty.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_cherrypick.py` & `pygit2-1.9.2/test/test_cherrypick.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_commit.py` & `pygit2-1.9.2/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_commit_trailer.py` & `pygit2-1.9.2/test/test_commit_trailer.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import pytest
 
 from . import utils
 
 
 @pytest.fixture
 def repo(tmp_path):
-    with utils.TemporaryRepository('trailerrepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('trailerrepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 def test_get_trailers_array(repo):
     commit_hash = '010231b2fdaee6b21da4f06058cf6c6a3392dd12'
     expected_trailers = {
         'Bug': '1234',
```

### Comparing `pygit2-1.9.1/test/test_config.py` & `pygit2-1.9.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_credentials.py` & `pygit2-1.9.2/test/test_credentials.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_describe.py` & `pygit2-1.9.2/test/test_describe.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_diff.py` & `pygit2-1.9.2/test/test_diff.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_diff_binary.py` & `pygit2-1.9.2/test/test_diff_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import pytest
 
 from . import utils
 
 
 @pytest.fixture
 def repo(tmp_path):
-    with utils.TemporaryRepository('binaryfilerepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('binaryfilerepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 PATCH_BINARY = """diff --git a/binary_file b/binary_file
 index 86e5c10..b835d73 100644
 Binary files a/binary_file and b/binary_file differ
 """
```

### Comparing `pygit2-1.9.1/test/test_index.py` & `pygit2-1.9.2/test/test_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     entry.mode = pygit2.GIT_FILEMODE_BLOB_EXECUTABLE
     assert 'foo.txt' == entry.path
     assert ign_entry.id == entry.id
     assert pygit2.GIT_FILEMODE_BLOB_EXECUTABLE == entry.mode
 
 def test_write_tree_to(testrepo, tmp_path):
     pygit2.option(pygit2.GIT_OPT_ENABLE_STRICT_OBJECT_CREATION, False)
-    with utils.TemporaryRepository('emptyrepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('emptyrepo.zip', tmp_path) as path:
         nrepo = Repository(path)
         id = testrepo.index.write_tree(nrepo)
         assert nrepo[id] is not None
 
 
 def test_create_entry(testrepo):
     index = testrepo.index
```

### Comparing `pygit2-1.9.1/test/test_mailmap.py` & `pygit2-1.9.2/test/test_mailmap.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_merge.py` & `pygit2-1.9.2/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_note.py` & `pygit2-1.9.2/test/test_note.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_object.py` & `pygit2-1.9.2/test/test_object.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_odb.py` & `pygit2-1.9.2/test/test_odb.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 
 
 BLOB_HEX = 'af431f20fc541ed6d5afede3e2dc7160f6f01f16'
 BLOB_RAW = binascii.unhexlify(BLOB_HEX.encode('ascii'))
 BLOB_OID = Oid(raw=BLOB_RAW)
 
 
-def test_emptyodb():
+def test_emptyodb(barerepo):
     odb = Odb()
 
     assert len([str(o) for o in odb]) == 0
     assert BLOB_HEX not in odb
-    path = Path(__file__).parent / 'data' / 'testrepo.git' / 'objects'
+    path = Path(barerepo.path) / 'objects'
     odb.add_disk_alternate(path)
     assert BLOB_HEX in odb
 
 
 @pytest.fixture
 def odb(barerepo):
     odb = barerepo.odb
```

### Comparing `pygit2-1.9.1/test/test_odb_backend.py` & `pygit2-1.9.2/test/test_odb_backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 BLOB_HEX = 'af431f20fc541ed6d5afede3e2dc7160f6f01f16'
 BLOB_RAW = binascii.unhexlify(BLOB_HEX.encode('ascii'))
 BLOB_OID = pygit2.Oid(raw=BLOB_RAW)
 
 
 @pytest.fixture
 def odb(barerepo):
-    yield barerepo.odb, Path(__file__).parent / 'data' / 'testrepo.git' / 'objects'
+    yield barerepo.odb, Path(barerepo.path) / 'objects'
 
 
 def test_pack(odb):
     odb, path = odb
 
     pack = pygit2.OdbBackendPack(path)
     assert len(list(pack)) > 0
@@ -94,15 +94,15 @@
 #
 # Test a custom object backend alone (without adding it to an ODB)
 # This doesn't make much sense, but it's possible.
 #
 
 @pytest.fixture
 def proxy(barerepo):
-    path = Path(__file__).parent / 'data' / 'testrepo.git' / 'objects'
+    path = Path(barerepo.path) / 'objects'
     yield ProxyBackend(pygit2.OdbBackendPack(path))
 
 
 def test_iterable(proxy):
     assert BLOB_HEX in [str(o) for o in proxy]
 
 def test_read(proxy):
```

### Comparing `pygit2-1.9.1/test/test_oid.py` & `pygit2-1.9.2/test/test_oid.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_options.py` & `pygit2-1.9.2/test/test_options.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_packbuilder.py` & `pygit2-1.9.2/test/test_packbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 pb.add_recur(commit.oid_new)
     confirm_same_repo_after_packing(testrepo, tmp_path, pack_delegate)
 
 
 def setup_second_repo(tmp_path):
     # helper method to set up a second repo for comparison
     tmp_path_2 = tmp_path / 'test_repo2'
-    with utils.TemporaryRepository('testrepo.tar', tmp_path_2) as path:
+    with utils.TemporaryRepository('testrepo.zip', tmp_path_2) as path:
         testrepo = pygit2.Repository(path)
     return testrepo
 
 def confirm_same_repo_after_packing(testrepo, tmp_path, pack_delegate):
     # Helper method to confirm the contents of two repos before and after packing
     pack_repo = setup_second_repo(tmp_path)
     pack_repo_path = Path(pack_repo.path)
```

### Comparing `pygit2-1.9.1/test/test_patch.py` & `pygit2-1.9.2/test/test_patch.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_patch_encoding.py` & `pygit2-1.9.2/test/test_patch_encoding.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_refdb_backend.py` & `pygit2-1.9.2/test/test_refdb_backend.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_refs.py` & `pygit2-1.9.2/test/test_refs.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_remote.py` & `pygit2-1.9.2/test/test_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,22 +236,22 @@
     callbacks = MyCallbacks(tips)
     remote.fetch(callbacks=callbacks)
     assert callbacks.i > 0
 
 
 @pytest.fixture
 def origin(tmp_path):
-    with utils.TemporaryRepository('testrepo.git', tmp_path) as path:
+    with utils.TemporaryRepository('barerepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 @pytest.fixture
 def clone(tmp_path):
     clone = tmp_path / 'clone'
     clone.mkdir()
-    with utils.TemporaryRepository('testrepo.git', clone) as path:
+    with utils.TemporaryRepository('barerepo.zip', clone) as path:
         yield pygit2.Repository(path)
 
 @pytest.fixture
 def remote(origin, clone):
     yield clone.remotes.create('origin', origin.path)
```

### Comparing `pygit2-1.9.1/test/test_remote_prune.py` & `pygit2-1.9.2/test/test_remote_prune.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_remote_utf8.py` & `pygit2-1.9.2/test/test_remote_utf8.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 import pygit2
 import pytest
 from . import utils
 
 
 @pytest.fixture
 def repo(tmp_path):
-    with utils.TemporaryRepository('utf8branchrepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('utf8branchrepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 def test_fetch(repo):
     remote = repo.remotes.create('origin', repo.workdir)
     remote.fetch()
```

### Comparing `pygit2-1.9.1/test/test_repository.py` & `pygit2-1.9.2/test/test_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,50 +352,38 @@
     subdir.mkdir(parents=True)
     assert repo.path == discover_repository(subdir)
 
 def test_discover_repo_not_found():
     assert discover_repository(tempfile.tempdir) is None
 
 
-def test_bytes_string():
-    repo_path = b'./test/data/testrepo.git/'
-    pygit2.Repository(repo_path)
-
-def test_unicode_string():
-    # String is unicode because of unicode_literals
-    repo_path = './test/data/testrepo.git/'
-    pygit2.Repository(repo_path)
-
-def test_aspath():
-    repo_path = Path('./test/data/testrepo.git/')
-    pygit2.Repository(repo_path)
-
-
-def test_clone_repository(tmp_path):
-    repo_path = "./test/data/testrepo.git/"
-    repo = clone_repository(repo_path, tmp_path)
+def test_repository_init(barerepo_path):
+    barerepo, path = barerepo_path
+    assert isinstance(path, Path)
+    pygit2.Repository(path)
+    pygit2.Repository(str(path))
+    pygit2.Repository(bytes(path))
+
+def test_clone_repository(barerepo, tmp_path):
+    assert barerepo.is_bare
+    repo = clone_repository(Path(barerepo.path), tmp_path / 'clonepath')
     assert not repo.is_empty
     assert not repo.is_bare
-
-def test_clone_repository_aspath(tmp_path):
-    repo_path = Path("./test/data/testrepo.git/")
-    repo = clone_repository(repo_path, Path(tmp_path))
+    repo = clone_repository(str(barerepo.path), str(tmp_path / 'clonestr'))
     assert not repo.is_empty
     assert not repo.is_bare
 
-def test_clone_bare_repository(tmp_path):
-    repo_path = "./test/data/testrepo.git/"
-    repo = clone_repository(repo_path, tmp_path, bare=True)
+def test_clone_bare_repository(barerepo, tmp_path):
+    repo = clone_repository(barerepo.path, tmp_path / 'clone', bare=True)
     assert not repo.is_empty
     assert repo.is_bare
 
-def test_clone_repository_and_remote_callbacks(tmp_path):
-    src_repo_relpath = Path('./test/data/testrepo.git/').resolve()
+def test_clone_repository_and_remote_callbacks(barerepo, tmp_path):
+    url = Path(barerepo.path).resolve().as_uri()
     repo_path = tmp_path / 'clone-into'
-    url = src_repo_relpath.as_uri()
 
     def create_repository(path, bare):
         return init_repository(path, bare)
 
     # here we override the name
     def create_remote(repo, name, url):
         return repo.remotes.create("custom_remote", url)
@@ -423,22 +411,19 @@
             raise RuntimeError('Unexpected error')
 
     url = "https://github.com/github/github"
     with pytest.raises(RuntimeError) as exc:
         clone_repository(url, tmp_path, callbacks=MyCallbacks())
     assert str(exc.value) == 'Unexpected error'
 
-def test_clone_with_checkout_branch(tmp_path):
+def test_clone_with_checkout_branch(barerepo, tmp_path):
     # create a test case which isolates the remote
-    test_repo = clone_repository('./test/data/testrepo.git',
-                                 tmp_path / 'testrepo-orig.git',
-                                 bare=True)
+    test_repo = clone_repository(barerepo.path, tmp_path / 'testrepo-orig.git', bare=True)
     test_repo.create_branch('test', test_repo[test_repo.head.target])
-    repo = clone_repository(test_repo.path,
-                            tmp_path / 'testrepo.git',
+    repo = clone_repository(test_repo.path, tmp_path / 'testrepo.git',
                             checkout_branch='test', bare=True)
     assert repo.lookup_reference('HEAD').target == 'refs/heads/test'
 
 # FIXME The tests below are commented because they are broken:
 #
 # - test_clone_push_url: Passes, but does nothing useful.
 #
@@ -560,15 +545,15 @@
     # The ref is no longer checked out
     assert worktree_ref.is_checked_out() == False
 
     # The branch still exists
     assert branch_name in testrepo.branches
 
 def test_open_extended(tmp_path):
-    with utils.TemporaryRepository('dirtyrepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('dirtyrepo.zip', tmp_path) as path:
         orig_repo = pygit2.Repository(path)
         assert not orig_repo.is_bare
         assert orig_repo.path
         assert orig_repo.workdir
 
         # GIT_REPOSITORY_OPEN_NO_SEARCH
         subdir_path = path / "subdir"
```

### Comparing `pygit2-1.9.1/test/test_repository_bare.py` & `pygit2-1.9.2/test/test_repository_bare.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_repository_custom.py` & `pygit2-1.9.2/test/test_repository_custom.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_repository_empty.py` & `pygit2-1.9.2/test/test_repository_empty.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_revparse.py` & `pygit2-1.9.2/test/test_revparse.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_revwalk.py` & `pygit2-1.9.2/test/test_revwalk.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_signature.py` & `pygit2-1.9.2/test/test_signature.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_status.py` & `pygit2-1.9.2/test/test_status.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_submodule.py` & `pygit2-1.9.2/test/test_submodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 SUBM_PATH = 'TestGitRepository'
 SUBM_URL = 'https://github.com/libgit2/TestGitRepository'
 SUBM_HEAD_SHA = '49322bb17d3acc9146f98c97d078513228bbf3c0'
 
 
 @pytest.fixture
 def repo(tmp_path):
-    with utils.TemporaryRepository('submodulerepo.tar', tmp_path) as path:
+    with utils.TemporaryRepository('submodulerepo.zip', tmp_path) as path:
         yield pygit2.Repository(path)
 
 
 def test_lookup_submodule(repo):
     s = repo.lookup_submodule(SUBM_PATH)
     assert s is not None
```

### Comparing `pygit2-1.9.1/test/test_tag.py` & `pygit2-1.9.2/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_tree.py` & `pygit2-1.9.2/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/test_treebuilder.py` & `pygit2-1.9.2/test/test_treebuilder.py`

 * *Files identical despite different names*

### Comparing `pygit2-1.9.1/test/utils.py` & `pygit2-1.9.2/test/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import hashlib
 from pathlib import Path
 import shutil
 import socket
 import stat
 import sys
 import tarfile
+import zipfile
 
 # Requirements
 import pytest
 
 # Pygit2
 import pygit2
 
@@ -104,18 +105,20 @@
     def __init__(self, name, tmp_path):
         self.name = name
         self.tmp_path = tmp_path
 
     def __enter__(self):
         path = Path(__file__).parent / 'data' / self.name
         temp_repo_path = Path(self.tmp_path) / path.stem
-        if path.suffix == '.tar':
-            tar = tarfile.open(path)
-            tar.extractall(self.tmp_path)
-            tar.close()
+        if path.suffix == '.zip':
+            with zipfile.ZipFile(path) as zipf:
+                zipf.extractall(self.tmp_path)
+        elif path.suffix == '.tar':
+            with tarfile.open(path) as tar:
+                tar.extractall(self.tmp_path)
         elif path.suffix == '.git':
             shutil.copytree(path, temp_repo_path)
         else:
             raise ValueError(f'Unexpected {path.suffix} extension')
 
         return temp_repo_path
```

