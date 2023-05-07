# Comparing `tmp/papis-0.8.2.tar.gz` & `tmp/papis-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/papis-0.8.2.tar", last modified: Thu Feb 28 19:26:34 2019, max compression
+gzip compressed data, was "dist/papis-0.9.tar", last modified: Mon Oct 21 09:42:47 2019, max compression
```

## Comparing `papis-0.8.2.tar` & `papis-0.9.tar`

### file list

```diff
@@ -1,108 +1,119 @@
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/contrib/
--rw-r--r--   0 gallo     (1004) cqc       (1001)      237 2018-08-03 17:06:42.000000 papis-0.8.2/contrib/papis.desktop
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/doc/
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/
--rw-r--r--   0 gallo     (1004) cqc       (1001)     7093 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-add.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1836 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-addto.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1854 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-browse.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2248 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-config.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2612 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-default.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1529 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-edit.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)    12580 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-explore.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3028 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-export.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1428 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-git.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3138 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-list.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1238 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-mv.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3624 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-open.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1234 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-rename.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1323 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-rm.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1708 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-run.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3818 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis-update.1
--rw-r--r--   0 gallo     (1004) cqc       (1001)   105767 2019-02-28 19:26:34.000000 papis-0.8.2/doc/build/man/papis.1
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/papis/
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/papis/commands/
--rw-r--r--   0 gallo     (1004) cqc       (1001)        0 2019-02-21 11:04:40.000000 papis-0.8.2/papis/commands/__init__.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    20244 2019-02-28 19:24:39.000000 papis-0.8.2/papis/commands/add.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3029 2019-02-26 16:30:45.000000 papis-0.8.2/papis/commands/addto.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1426 2019-02-22 10:19:10.000000 papis-0.8.2/papis/commands/browse.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1647 2019-02-22 10:19:10.000000 papis-0.8.2/papis/commands/config.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3753 2019-02-21 11:04:40.000000 papis-0.8.2/papis/commands/default.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2169 2019-02-22 10:19:10.000000 papis-0.8.2/papis/commands/edit.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    18234 2019-02-26 16:30:45.000000 papis-0.8.2/papis/commands/explore.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     5849 2019-02-22 10:19:10.000000 papis-0.8.2/papis/commands/export.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1236 2019-02-22 10:20:15.000000 papis-0.8.2/papis/commands/external.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      896 2019-02-22 10:19:42.000000 papis-0.8.2/papis/commands/git.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     5345 2019-02-26 16:30:45.000000 papis-0.8.2/papis/commands/list.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2389 2019-02-22 10:19:10.000000 papis-0.8.2/papis/commands/mv.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     4964 2019-02-22 10:19:10.000000 papis-0.8.2/papis/commands/open.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1453 2019-02-22 10:19:10.000000 papis-0.8.2/papis/commands/rename.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2172 2019-02-26 16:30:45.000000 papis-0.8.2/papis/commands/rm.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1354 2019-02-22 10:19:28.000000 papis-0.8.2/papis/commands/run.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     8406 2019-02-22 10:19:10.000000 papis-0.8.2/papis/commands/update.py
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/papis/database/
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1173 2018-09-03 09:17:37.000000 papis-0.8.2/papis/database/__init__.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1778 2018-09-03 09:17:37.000000 papis-0.8.2/papis/database/base.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    12359 2019-02-21 14:25:53.000000 papis-0.8.2/papis/database/cache.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    10236 2018-09-03 09:17:37.000000 papis-0.8.2/papis/database/whoosh.py
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/papis/downloaders/
--rw-r--r--   0 gallo     (1004) cqc       (1001)        0 2018-08-03 17:06:42.000000 papis-0.8.2/papis/downloaders/__init__.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1335 2018-09-03 09:17:38.000000 papis-0.8.2/papis/downloaders/acs.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1350 2018-09-03 09:17:38.000000 papis-0.8.2/papis/downloaders/annualreviews.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1491 2018-09-03 09:17:38.000000 papis-0.8.2/papis/downloaders/aps.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1588 2019-02-21 10:17:38.000000 papis-0.8.2/papis/downloaders/arxiv.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     6120 2019-02-21 10:10:26.000000 papis-0.8.2/papis/downloaders/base.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1197 2018-12-10 16:14:20.000000 papis-0.8.2/papis/downloaders/frontiersin.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      872 2018-09-03 09:17:38.000000 papis-0.8.2/papis/downloaders/get.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1457 2019-02-07 13:36:19.000000 papis-0.8.2/papis/downloaders/hal.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2180 2018-09-03 09:17:38.000000 papis-0.8.2/papis/downloaders/ieee.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1938 2018-09-03 09:17:38.000000 papis-0.8.2/papis/downloaders/iopscience.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      963 2018-09-10 09:34:28.000000 papis-0.8.2/papis/downloaders/libgen.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1226 2018-09-03 09:17:38.000000 papis-0.8.2/papis/downloaders/scitationaip.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2291 2018-09-10 12:36:11.000000 papis-0.8.2/papis/downloaders/thesesfr.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3010 2019-02-07 13:36:19.000000 papis-0.8.2/papis/downloaders/utils.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1426 2018-10-22 12:44:16.000000 papis-0.8.2/papis/downloaders/worldscientific.py
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/papis/tui/
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/papis/tui/widgets/
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3177 2019-02-26 16:30:45.000000 papis-0.8.2/papis/tui/widgets/__init__.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2760 2019-02-26 16:30:45.000000 papis-0.8.2/papis/tui/widgets/command_line_prompt.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     7759 2019-02-26 16:30:45.000000 papis-0.8.2/papis/tui/widgets/list.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      974 2019-02-26 16:30:45.000000 papis-0.8.2/papis/tui/__init__.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    12173 2019-02-26 16:30:45.000000 papis-0.8.2/papis/tui/app.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:22:07.000000 papis-0.8.2/papis/tui/utils.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      141 2019-02-28 19:25:47.000000 papis-0.8.2/papis/__init__.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     6949 2019-01-10 17:50:51.000000 papis-0.8.2/papis/api.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2559 2018-09-04 00:52:37.000000 papis-0.8.2/papis/arxiv.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2356 2019-02-07 14:37:35.000000 papis-0.8.2/papis/base.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    93928 2019-01-10 19:24:23.000000 papis-0.8.2/papis/bibtex.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     4307 2019-02-22 10:32:03.000000 papis-0.8.2/papis/cli.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    34684 2019-02-27 18:39:06.000000 papis-0.8.2/papis/config.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     9785 2019-02-07 13:36:19.000000 papis-0.8.2/papis/crossref.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2133 2018-09-03 09:17:37.000000 papis-0.8.2/papis/dissemin.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     4791 2019-02-21 14:34:42.000000 papis-0.8.2/papis/docmatcher.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    16608 2019-01-17 16:50:33.000000 papis-0.8.2/papis/document.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      792 2018-09-03 09:17:37.000000 papis-0.8.2/papis/exceptions.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      804 2018-09-17 09:25:40.000000 papis-0.8.2/papis/isbn.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     4320 2018-09-17 09:25:40.000000 papis-0.8.2/papis/isbnplus.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      152 2019-02-21 10:22:28.000000 papis-0.8.2/papis/main.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)      502 2019-02-26 16:30:45.000000 papis-0.8.2/papis/pick.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)    13165 2019-02-28 19:22:09.000000 papis-0.8.2/papis/utils.py
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/papis.egg-info/
--rw-r--r--   0 gallo     (1004) cqc       (1001)     6830 2019-02-28 19:26:34.000000 papis-0.8.2/papis.egg-info/PKG-INFO
--rw-r--r--   0 gallo     (1004) cqc       (1001)     2189 2019-02-28 19:26:34.000000 papis-0.8.2/papis.egg-info/SOURCES.txt
--rw-r--r--   0 gallo     (1004) cqc       (1001)        1 2019-02-28 19:26:34.000000 papis-0.8.2/papis.egg-info/dependency_links.txt
--rw-r--r--   0 gallo     (1004) cqc       (1001)       43 2019-02-28 19:26:34.000000 papis-0.8.2/papis.egg-info/entry_points.txt
--rw-r--r--   0 gallo     (1004) cqc       (1001)      410 2019-02-28 19:26:34.000000 papis-0.8.2/papis.egg-info/requires.txt
--rw-r--r--   0 gallo     (1004) cqc       (1001)        6 2019-02-28 19:26:34.000000 papis-0.8.2/papis.egg-info/top_level.txt
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/scripts/
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/scripts/shell_completion/
-drwxr-xr-x   0 gallo     (1004) cqc       (1001)        0 2019-02-28 19:26:34.000000 papis-0.8.2/scripts/shell_completion/click/
--rw-r--r--   0 gallo     (1004) cqc       (1001)      630 2019-02-18 10:07:04.000000 papis-0.8.2/scripts/shell_completion/click/papis.sh
--rw-r--r--   0 gallo     (1004) cqc       (1001)      701 2019-02-26 16:36:45.000000 papis-0.8.2/AUTHORS
--rw-r--r--   0 gallo     (1004) cqc       (1001)     1384 2019-02-27 19:38:00.000000 papis-0.8.2/CHANGELOG.md
--rw-r--r--   0 gallo     (1004) cqc       (1001)      674 2018-08-03 17:06:42.000000 papis-0.8.2/LICENSE.txt
--rw-r--r--   0 gallo     (1004) cqc       (1001)     4506 2018-09-14 13:57:16.000000 papis-0.8.2/README.rst
--rw-r--r--   0 gallo     (1004) cqc       (1001)      230 2019-02-28 19:26:34.000000 papis-0.8.2/setup.cfg
--rw-r--r--   0 gallo     (1004) cqc       (1001)     3906 2019-02-27 18:37:08.000000 papis-0.8.2/setup.py
--rw-r--r--   0 gallo     (1004) cqc       (1001)     6830 2019-02-28 19:26:34.000000 papis-0.8.2/PKG-INFO
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      732 2019-10-21 09:42:47.000000 papis-0.9/setup.cfg
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5013 2019-09-14 22:00:24.000000 papis-0.9/README.rst
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/papis.egg-info/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2420 2019-10-21 09:42:47.000000 papis-0.9/papis.egg-info/SOURCES.txt
+-rw-r--r--   0 gallo     (1000) gallo     (1000)        1 2019-10-21 09:42:47.000000 papis-0.9/papis.egg-info/dependency_links.txt
+-rw-r--r--   0 gallo     (1000) gallo     (1000)        6 2019-10-21 09:42:47.000000 papis-0.9/papis.egg-info/top_level.txt
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     7455 2019-10-21 09:42:47.000000 papis-0.9/papis.egg-info/PKG-INFO
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      436 2019-10-21 09:42:47.000000 papis-0.9/papis.egg-info/requires.txt
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2482 2019-10-21 09:42:47.000000 papis-0.9/papis.egg-info/entry_points.txt
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      674 2018-08-04 00:26:27.000000 papis-0.9/LICENSE.txt
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     7214 2019-10-21 09:35:54.000000 papis-0.9/setup.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     7455 2019-10-21 09:42:47.000000 papis-0.9/PKG-INFO
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      701 2019-02-26 21:37:11.000000 papis-0.9/AUTHORS
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/doc/
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/doc/build/
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/doc/build/man/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1244 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-rename.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1718 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-run.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1623 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-edit.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     3256 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-update.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    12949 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-explore.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2736 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-default.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1917 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-addto.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1446 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-rm.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1931 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-browse.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2258 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-config.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2814 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-list.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1428 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-git.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2746 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-export.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     3724 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-open.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     6936 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-add.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1248 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis-mv.1
+-rw-r--r--   0 gallo     (1000) gallo     (1000)   109005 2019-10-21 09:42:46.000000 papis-0.9/doc/build/man/papis.1
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/scripts/
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/scripts/shell_completion/
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/scripts/shell_completion/click/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      630 2019-02-17 16:12:30.000000 papis-0.9/scripts/shell_completion/click/papis.sh
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/scripts/shell_completion/click/zsh/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      802 2019-03-23 02:52:33.000000 papis-0.9/scripts/shell_completion/click/zsh/_papis
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/contrib/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      237 2018-08-04 00:26:27.000000 papis-0.9/contrib/papis.desktop
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5051 2019-10-21 09:13:24.000000 papis-0.9/CHANGELOG.md
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/papis/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      639 2019-06-08 11:55:33.000000 papis-0.9/papis/json.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      558 2019-03-30 13:23:06.000000 papis-0.9/papis/exceptions.py
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/papis/tui/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      974 2019-02-26 21:37:11.000000 papis-0.9/papis/tui/__init__.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    12344 2019-06-08 11:55:33.000000 papis-0.9/papis/tui/app.py
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/papis/tui/widgets/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2512 2019-03-17 21:06:48.000000 papis-0.9/papis/tui/widgets/__init__.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     6297 2019-10-16 21:55:35.000000 papis-0.9/papis/tui/widgets/diff.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     8934 2019-06-08 11:55:33.000000 papis-0.9/papis/tui/widgets/list.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2633 2019-03-23 02:52:33.000000 papis-0.9/papis/tui/widgets/command_line_prompt.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)       58 2019-03-30 13:23:06.000000 papis-0.9/papis/strings.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      423 2019-09-14 22:28:51.000000 papis-0.9/papis/__init__.py
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/papis/downloaders/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5511 2019-10-20 20:18:20.000000 papis-0.9/papis/downloaders/sciencedirect.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2290 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/thesesfr.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     3044 2019-10-20 20:18:20.000000 papis-0.9/papis/downloaders/tandfonline.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2132 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/ieee.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1024 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/get.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2632 2019-10-20 20:18:20.000000 papis-0.9/papis/downloaders/annualreviews.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      684 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/hal.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     3856 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/__init__.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     3586 2019-10-20 20:18:20.000000 papis-0.9/papis/downloaders/acs.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    12796 2019-10-20 20:18:20.000000 papis-0.9/papis/downloaders/base.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1191 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/frontiersin.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1421 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/worldscientific.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      914 2019-10-20 20:18:20.000000 papis-0.9/papis/downloaders/fallback.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      671 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/aps.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1962 2019-10-20 20:18:20.000000 papis-0.9/papis/downloaders/iopscience.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1222 2019-09-14 22:00:24.000000 papis-0.9/papis/downloaders/scitationaip.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2719 2019-10-20 20:18:20.000000 papis-0.9/papis/downloaders/springer.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2994 2019-06-08 11:55:33.000000 papis-0.9/papis/base.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1924 2019-10-20 20:47:02.000000 papis-0.9/papis/git.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     9401 2019-10-20 20:18:20.000000 papis-0.9/papis/arxiv.py
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/papis/database/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1266 2019-03-23 02:52:33.000000 papis-0.9/papis/database/__init__.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1869 2019-03-23 02:52:33.000000 papis-0.9/papis/database/base.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     8882 2019-10-20 23:14:01.000000 papis-0.9/papis/database/cache.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    10860 2019-09-14 22:00:24.000000 papis-0.9/papis/database/whoosh.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2873 2019-10-16 01:47:39.000000 papis-0.9/papis/cli.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      544 2019-03-30 13:23:06.000000 papis-0.9/papis/library.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    18581 2019-10-21 08:52:23.000000 papis-0.9/papis/config.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     3545 2019-10-17 21:52:00.000000 papis-0.9/papis/importer.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     4733 2019-10-21 08:52:23.000000 papis-0.9/papis/docmatcher.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    13142 2019-10-20 20:18:20.000000 papis-0.9/papis/document.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      862 2019-09-14 22:00:24.000000 papis-0.9/papis/pubmed.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    13046 2019-10-17 21:30:00.000000 papis-0.9/papis/crossref.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5158 2019-06-08 11:55:33.000000 papis-0.9/papis/isbnplus.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    95802 2019-09-14 22:00:24.000000 papis-0.9/papis/bibtex.py
+drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:42:47.000000 papis-0.9/papis/commands/
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1254 2019-03-30 13:23:12.000000 papis-0.9/papis/commands/external.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2384 2019-10-20 20:18:20.000000 papis-0.9/papis/commands/mv.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    17370 2019-10-21 09:24:38.000000 papis-0.9/papis/commands/add.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1409 2019-09-14 22:00:24.000000 papis-0.9/papis/commands/__init__.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5857 2019-10-16 01:47:39.000000 papis-0.9/papis/commands/default.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     3301 2019-10-16 01:47:39.000000 papis-0.9/papis/commands/rm.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      913 2019-03-30 13:23:12.000000 papis-0.9/papis/commands/git.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2662 2019-06-08 11:55:33.000000 papis-0.9/papis/commands/browse.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1613 2019-06-08 11:55:33.000000 papis-0.9/papis/commands/rename.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1361 2019-03-30 13:23:12.000000 papis-0.9/papis/commands/run.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1647 2019-03-30 13:23:12.000000 papis-0.9/papis/commands/config.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5347 2019-10-16 01:47:39.000000 papis-0.9/papis/commands/list.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5726 2019-09-14 22:00:24.000000 papis-0.9/papis/commands/export.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    10877 2019-10-16 01:47:39.000000 papis-0.9/papis/commands/explore.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     8325 2019-10-20 20:18:20.000000 papis-0.9/papis/commands/bibtex.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5207 2019-06-08 11:55:33.000000 papis-0.9/papis/commands/open.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     3606 2019-10-16 01:47:39.000000 papis-0.9/papis/commands/addto.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5839 2019-10-16 21:55:42.000000 papis-0.9/papis/commands/update.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2911 2019-10-16 01:47:39.000000 papis-0.9/papis/commands/edit.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)    15114 2019-10-21 08:52:23.000000 papis-0.9/papis/utils.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     1574 2019-06-08 11:55:33.000000 papis-0.9/papis/isbn.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     5356 2019-09-14 22:00:24.000000 papis-0.9/papis/api.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2641 2019-06-08 11:55:33.000000 papis-0.9/papis/dissemin.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2211 2019-09-14 22:00:24.000000 papis-0.9/papis/pick.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)     2482 2019-09-14 22:00:24.000000 papis-0.9/papis/yaml.py
+-rw-r--r--   0 gallo     (1000) gallo     (1000)      213 2019-09-14 22:00:24.000000 papis-0.9/papis/plugin.py
```

### Comparing `papis-0.8.2/doc/build/man/papis-add.1` & `papis-0.9/doc/build/man/papis-add.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-ADD" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-ADD" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-add \- add command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -44,15 +44,16 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis add ~/Documents/interesting.pdf \-\-name interesting\-paper\-2021
+papis add ~/Documents/interesting.pdf \e
+    \-\-folder\-name interesting\-paper\-2021
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
@@ -62,15 +63,15 @@
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis add ~/Documents/interesting.pdf \e
-    \-\-name interesting\-paper\-2021 \e
+    \-\-folder\-name interesting\-paper\-2021 \e
     \-\-set author \(aqJohn Smith\(aq \e
     \-\-set title \(aqThe interesting life of bees\(aq \e
     \-\-set year 1985 \e
     \-\-set tags \(aqbiology interesting bees\(aq
 .ft P
 .fi
 .UNINDENT
@@ -84,15 +85,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis add ~/Documents/interesting.pdf \-\-from\-doi 10.10763/1.3237134
+papis add ~/Documents/interesting.pdf \-\-from doi 10.10763/1.3237134
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -101,15 +102,15 @@
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis \-l machine\-learning add \e
-    \-\-from\-url https://arxiv.org/abs/1712.03134
+    \-\-from url https://arxiv.org/abs/1712.03134
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -119,65 +120,96 @@
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis add \-\-link ~/Documents/interesting.pdf \e
-    \-\-from\-doi 10.10763/1.3237134
+    \-\-from doi 10.10763/1.3237134
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
 will add an entry into the papis library, but the pdf document will remain
 at \fB~/Documents/interesting.pdf\fP, and in the document\(aqs folder
 there will be a link to \fB~/Documents/interesting.pdf\fP instead of the
 file itself. Of course you always have to be sure that the
 document at \fB~/Documents/interesting.pdf\fP does not disappear, otherwise
 you will end up without a document to open.
+.IP \(bu 2
+Papis also tries to make sense of the inputs that you have passed
+to the command, for instance you could provide only a \fBdoi\fP and
+papis will try to know if this is indeed a \fBdoi\fP
+.INDENT 2.0
+.INDENT 3.5
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis add 10.1103/PhysRevLett.123.156401
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.sp
+or from a \fBurl\fP
+.INDENT 2.0
+.INDENT 3.5
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis add https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.123.156401
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
 .UNINDENT
 .SH EXAMPLES IN PYTHON
 .sp
 There is a python function in the add module that can be used to interact
 in a more effective way in python scripts,
 .INDENT 0.0
 .TP
-.B papis.commands.add.run(paths, data={}, name=None, file_name=None, subfolder=None, interactive=False, confirm=False, open_file=False, edit=False, commit=False, link=False)
+.B papis.commands.add.run(paths, data={}, folder_name=None, file_name=None, subfolder=None, confirm=False, open_file=False, edit=False, git=False, link=False)
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpaths\fP (\fI[\fP\fI]\fP) \-\- Paths to the documents to be added
 .IP \(bu 2
 \fBdata\fP (\fIdict\fP) \-\- Data for the document to be added.
 If more data is to be retrieved from other sources, the data dictionary
 will be updated from these sources.
 .IP \(bu 2
-\fBname\fP (\fIstr\fP) \-\- Name of the folder where the document will be stored
+\fBfolder_name\fP (\fIstr\fP) \-\- Name of the folder where the document will be stored
 .IP \(bu 2
 \fBfile_name\fP (\fIstr\fP) \-\- File name of the document\(aqs files to be stored.
 .IP \(bu 2
 \fBsubfolder\fP (\fIstr\fP) \-\- Folder within the library where the document\(aqs folder
 should be stored.
 .IP \(bu 2
-\fBinteractive\fP (\fIbool\fP) \-\- Wether or not interactive functionality of this command
-should be activated.
-.IP \(bu 2
 \fBconfirm\fP (\fIbool\fP) \-\- Wether or not to ask user for confirmation before adding.
 .IP \(bu 2
 \fBopen_file\fP (\fIbool\fP) \-\- Wether or not to ask user for opening file before adding.
 .IP \(bu 2
 \fBedit\fP (\fIbool\fP) \-\- Wether or not to ask user for editing the infor file
 before adding.
 .IP \(bu 2
-\fBcommit\fP (\fIbool\fP) \-\- Wether or not to ask user for committing before adding,
+\fBgit\fP (\fIbool\fP) \-\- Wether or not to ask user for committing before adding,
 in the case of course that the library is a git repository.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SH CLI
 .SS papis add
 .sp
@@ -188,78 +220,50 @@
 .nf
 .ft C
 papis add [OPTIONS] [FILES]...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-s, \-\-set <set_list>
 Set some information before
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-d, \-\-dir <directory>
+.B \-d, \-\-subfolder <subfolder>
 Subfolder in the library
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-i, \-\-interactive, \-\-no\-interactive
-Do some of the actions interactively
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-name <name>
+.B \-\-folder\-name <folder_name>
 Name for the document\(aqs folder (papis format)
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-file\-name <file_name>
 File name for the document (papis format)
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-from\-bibtex <from_bibtex>
-Parse information from a bibtex file
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-yaml <from_yaml>
-Parse information from a yaml file
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-folder <from_folder>
-Add document from folder being a valid papis document (containing info.yaml)
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-url <from_url>
-Get document and information from agiven url, a parser must be implemented
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-doi <from_doi>
-Doi to try to get information from
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-pmid <from_pmid>
-PMID to try to get information from
+.B \-\-from <from_importer>
+Add document from a specific importer (pdf2doi, yaml, crossref, folder, pmid, arxiv, lib, bibtex, doi, pdf2arxivid)
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-from\-lib <from_lib>
-Add document from another library
+.B \-b, \-\-batch
+Batch mode, do not prompt or otherwise
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-confirm, \-\-no\-confirm
 Ask to confirm before adding to the collection
 .UNINDENT
 .INDENT 0.0
@@ -270,28 +274,30 @@
 .INDENT 0.0
 .TP
 .B \-\-edit, \-\-no\-edit
 Edit info file before adding document
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-commit, \-\-no\-commit
-Commit document if library is a git repository
+.B \-\-link, \-\-no\-link
+Instead of copying the file to the library, create a link toits original location
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-link, \-\-no\-link
-Instead of copying the file to the library, create a link toits original location
+.B \-\-git, \-\-no\-git
+Git add and commit the new document
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-no\-document
-DEPRECATION NOTICE: This option is no longer valid, it will be removed in future releases
+.B \-\-list\-importers, \-\-li
+List all available papis importers
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B FILES
 Optional argument(s)
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-addto.1` & `papis-0.9/doc/build/man/papis-addto.1`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-ADDTO" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-ADDTO" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-addto \- addto command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -58,30 +58,39 @@
 .nf
 .ft C
 papis addto [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-git, \-\-no\-git
+Add and commit files
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-f, \-\-files <files>
 File fullpaths to documents
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-file\-name <file_name>
 File name for the document (papis format)
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-browse.1` & `papis-0.9/doc/build/man/papis-browse.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-BROWSE" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-BROWSE" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-browse \- browse command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -51,25 +51,34 @@
 .nf
 .ft C
 papis browse [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-k, \-\-key <key>
 Use the value of the document\(aqs key to open in the browser, e.g.doi, url, doc_url ...
 .UNINDENT
-Arguments.INDENT 0.0
+.INDENT 0.0
+.TP
+.B \-\-all
+Browse all selected documents
+.UNINDENT
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-config.1` & `papis-0.9/doc/build/man/papis-config.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-CONFIG" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-CONFIG" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-config \- config command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -89,20 +89,24 @@
 .nf
 .ft C
 papis config [OPTIONS] OPTION
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B OPTION
 Required argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-default.1` & `papis-0.9/doc/build/man/papis-default.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-DEFAULT" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-DEFAULT" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-default \- default command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -77,15 +77,17 @@
 .nf
 .ft C
 papis [OPTIONS] COMMAND [ARGS]...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-version
@@ -106,14 +108,19 @@
 .B \-c, \-\-config <config>
 Configuration file to use
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-log <log>
 Logging level
+.INDENT 7.0
+.TP
+.B Options
+INFO|DEBUG|WARNING|ERROR|CRITICAL
+.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-pick\-lib
 Pick library to use
 .UNINDENT
 .INDENT 0.0
@@ -124,16 +131,21 @@
 .INDENT 0.0
 .TP
 .B \-s, \-\-set <set_list>
 Set key value, e.g., \-\-set info\-name information.yaml  \-\-set opentool evince
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-nc, \-\-no\-color
+.B \-\-color <color>
 Prevent the output from having color
+.INDENT 7.0
+.TP
+.B Options
+always|auto|no
+.UNINDENT
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
 2017, Alejandro Gallo
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `papis-0.8.2/doc/build/man/papis-edit.1` & `papis-0.9/doc/build/man/papis-edit.1`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-EDIT" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-EDIT" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-edit \- edit command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -43,35 +43,44 @@
 .nf
 .ft C
 papis edit [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-git, \-\-no\-git
+Add changes made to the info file
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-n, \-\-notes
 Edit notes associated to the document
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-all
 Edit all matching documents
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-e, \-\-editor <editor>
 Editor to be used
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-explore.1` & `papis-0.9/doc/build/man/papis-explore.1`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-EXPLORE" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-EXPLORE" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-explore \- explore command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -65,21 +65,21 @@
 .UNINDENT
 .UNINDENT
 .sp
 will tell you which commands are available.
 Let us suppose that you want to look for some documents on crossref,
 say some papers of Schroedinger, and you want to store them into a bibtex
 file called \fBlib.bib\fP, then you could concatenate the commands
-\fBcrossref\fP and \fBexport \-\-bibtex\fP as such
+\fBcrossref\fP and \fBexport \-\-format bibtex\fP as such
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis explore crossref \-a \(aqSchrodinger\(aq export \-\-bibtex lib.bib
+papis explore crossref \-a \(aqSchrodinger\(aq export \-\-format bibtex lib.bib
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 This will store everything that you got from crossref in the file \fBlib.bib\fP
 and store in bibtex format. \fBexplore\fP is much more flexible than that,
@@ -87,15 +87,15 @@
 you don\(aqt want to store all retrieved documents but only one that you pick,
 the \fBpick\fP command will take care of it
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis explore crossref \-a \(aqSchrodinger\(aq pick export \-\-bibtex lib.bib
+papis explore crossref \-a \(aqSchrodinger\(aq pick export \-\-format bibtex lib.bib
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 notice how the \fBpick\fP command is situated before the \fBexport\fP\&.
 More generally you could write something like
@@ -104,17 +104,17 @@
 .sp
 .nf
 .ft C
 papis explore \e
     crossref \-a Schroedinger \e
     crossref \-a Einstein \e
     arxiv \-a \(aqFelix Hummel\(aq \e
-    export \-\-yaml docs.yaml \e
+    export \-\-format yaml docs.yaml \e
     pick  \e
-    export \-\-bibtex specially\-picked\-document.bib
+    export \-\-format bibtex specially\-picked\-document.bib
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 The upper command will look in crossref for documents authored by Schrodinger,
 then also by Einstein, and will look on the arxiv for papers authored by Felix
@@ -156,15 +156,17 @@
 .nf
 .ft C
 papis explore [OPTIONS] COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .SS arxiv
 .sp
 Look for documents on ArXiV.org.
@@ -189,15 +191,17 @@
 .nf
 .ft C
 papis explore arxiv [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
@@ -255,15 +259,17 @@
 .nf
 .ft C
 papis explore base [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
@@ -281,47 +287,58 @@
 .nf
 .ft C
 papis explore bibtex [OPTIONS] BIBFILE
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B BIBFILE
 Required argument
 .UNINDENT
 .SS citations
 .sp
 Query the citations of a paper
 .sp
 Example:
 .sp
 Go through the citations of a paper and export it in a yaml file
 .INDENT 0.0
 .INDENT 3.5
-papis explore citations \(aqeinstein\(aq export \-\-yaml einstein.yaml
+papis explore citations \(aqeinstein\(aq export \-\-format yaml einstein.yaml
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis explore citations [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
+.TP
+.B \-\-doc\-folder <doc_folder>
+Apply action to a document path
+.UNINDENT
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-s, \-\-save
@@ -333,15 +350,17 @@
 Remove the stored citations file
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-m, \-\-max\-citations <max_citations>
 Number of citations to be retrieved
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS cmd
 .sp
 Run a general command on the document list
@@ -360,20 +379,24 @@
 .nf
 .ft C
 papis explore cmd [OPTIONS] COMMAND
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B COMMAND
 Required argument
 .UNINDENT
 .SS crossref
 .sp
 Look for documents on crossref.org.
@@ -387,34 +410,65 @@
 .nf
 .ft C
 papis explore crossref [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
+General query
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-a, \-\-author <author>
+Author of the query
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-t, \-\-title <title>
+Title of the query
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-m, \-\-max <max>
+Maximum number of results
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-f, \-\-filter <filter>
+Filters to apply
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-o, \-\-order <order>
+Order of appearance according to sorting  [default: desc]
+.INDENT 7.0
+.TP
+.B Options
+asc|desc
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-s, \-\-sort <sort>
+Sorting parameter  [default: score]
+.INDENT 7.0
+.TP
+.B Options
+relevance|score|updated|deposited|indexed|published|published\-print|published\-online|issued|is\-referenced\-by\-count|references\-count
+.UNINDENT
 .UNINDENT
 .SS dissemin
 .sp
 Look for documents on dissem.in
 .sp
 Examples of its usage are
 .sp
@@ -425,15 +479,17 @@
 .nf
 .ft C
 papis explore dissemin [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
@@ -451,33 +507,35 @@
 .nf
 .ft C
 papis explore export [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-bibtex <bibtex>
-Export list of documents retrieved to a bibtex file
-.UNINDENT
-.INDENT 0.0
+.B \-f, \-\-format <format>
+Format for the document
+.INDENT 7.0
 .TP
-.B \-\-yaml <yaml>
-Export list of documents retrieved to a yaml file
+.B Options
+json|bibtex|yaml
+.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-json <json>
-Export list of documents retrieved to a json file
+.B \-o, \-\-out <out>
+Outfile to write information to
 .UNINDENT
 .SS isbn
 .sp
 Look for documents using isbnlib
 .sp
 Examples of its usage are
 .sp
@@ -488,26 +546,33 @@
 .nf
 .ft C
 papis explore isbn [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-s, \-\-service <service>
+.INDENT 7.0
+.TP
+.B Options
+wcat|goob|openl
+.UNINDENT
 .UNINDENT
 .SS isbnplus
 .sp
 Look for documents on isbnplus.com
 .sp
 Examples of its usage are
 .sp
@@ -518,15 +583,17 @@
 .nf
 .ft C
 papis explore isbnplus [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
@@ -552,20 +619,24 @@
 .nf
 .ft C
 papis explore json [OPTIONS] JSONFILE
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B JSONFILE
 Required argument
 .UNINDENT
 .SS lib
 .sp
 Query for documents in your library
@@ -582,62 +653,37 @@
 .nf
 .ft C
 papis explore lib [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
-.TP
-.B \-h, \-\-help
-Show this message and exit.
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-l, \-\-library <library>
-Papis library to look
-.UNINDENT
-Arguments.INDENT 0.0
-.TP
-.B QUERY
-Optional argument
-.UNINDENT
-.SS libgen
 .sp
-Look for documents on library genesis
-.sp
-Examples of its usage are
-.sp
-papis explore libgen \-a \(aqAlbert einstein\(aq export \-\-yaml einstein.yaml
+Options
 .INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-papis explore libgen [OPTIONS]
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-Options.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-a, \-\-author <author>
+.B \-\-doc\-folder <doc_folder>
+Apply action to a document path
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-t, \-\-title <title>
+.B \-l, \-\-library <library>
+Papis library to look
 .UNINDENT
+.sp
+Arguments
 .INDENT 0.0
 .TP
-.B \-i, \-\-isbn <isbn>
+.B QUERY
+Optional argument
 .UNINDENT
 .SS pick
 .sp
 Pick a document from the retrieved documents
 .sp
 Examples of its usage are
 .sp
@@ -648,15 +694,17 @@
 .nf
 .ft C
 papis explore pick [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-n, \-\-number <number>
@@ -675,20 +723,24 @@
 .nf
 .ft C
 papis explore yaml [OPTIONS] YAMLFILE
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B YAMLFILE
 Required argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-export.1` & `papis-0.9/doc/build/man/papis-export.1`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-EXPORT" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-EXPORT" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-export \- export command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -39,41 +39,41 @@
 Export one of the documents matching the author with einstein to bibtex:
 .UNINDENT
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis export \-\-bibtex \(aqauthor = einstein\(aq
+papis export \-\-format bibtex \(aqauthor : einstein\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 or export all of them
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis export \-\-bibtex \-\-all \(aqauthor = einstein\(aq
+papis export \-\-format bibtex \-\-all \(aqauthor : einstein\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 Export all documents to bibtex and save them into a \fBlib.bib\fP file
 .UNINDENT
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis export \-\-all \-\-bibtex \-\-out lib.bib
+papis export \-\-all \-\-format bibtex \-\-out lib.bib
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 Export a folder of one of the documents matching the word \fBkrebs\fP
@@ -85,26 +85,14 @@
 .nf
 .ft C
   papis export \-\-folder \-\-out interesting\-document krebs
 
 this will create the folder \(ga\(gainteresting\-document\(ga\(ga containing the
 \(ga\(gainfo.yaml\(ga\(ga file, the linked documents and a \(ga\(gabibtex\(ga\(ga file for
 sharing with other people.
-
-You can also just export its associated document:
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-papis export \-\-file krebs
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SH CLI
 .SS papis export
 .sp
@@ -115,61 +103,50 @@
 .nf
 .ft C
 papis export [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-yaml
-Export into yaml
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-bibtex
-Export into bibtex
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-json
-Export into json
-.UNINDENT
-.INDENT 0.0
-.TP
 .B \-\-folder
 Export document folder to share
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-o, \-\-out <out>
 Outfile or outdir
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-t, \-\-text
-Text formated reference
+.B \-f, \-\-format <format>
+Format for the document
+.INDENT 7.0
+.TP
+.B Options
+json|bibtex|yaml
+.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-a, \-\-all
 Export all without picking
 .UNINDENT
+.sp
+Arguments
 .INDENT 0.0
 .TP
-.B \-\-file
-Export a copy of a file
-.UNINDENT
-Arguments.INDENT 0.0
-.TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
 2017, Alejandro Gallo
```

### Comparing `papis-0.8.2/doc/build/man/papis-git.1` & `papis-0.9/doc/build/man/papis-git.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-GIT" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-GIT" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-git \- git command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `papis-0.8.2/doc/build/man/papis-list.1` & `papis-0.9/doc/build/man/papis-list.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-LIST" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-LIST" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-list \- list command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -39,15 +39,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis list \-\-file
+papis list \-\-all \-\-file
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -55,15 +55,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis list \-\-format \(aq{doc[year]} {doc[title]}\(aq
+papis list \-\-all \-\-format \(aq{doc[year]} {doc[title]}\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -72,60 +72,39 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis list \-\-template bibitem.template
+papis list \-\-all \-\-template bibitem.template
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
-.SH PYTHON EXAMPLES
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-# Import the run function from the list command
-
-from papis.commands.list import run as papis_list
-
-documents = papis_list(query=\(aqeinstein\(aq, library=\(aqpapis\(aq)
-
-for doc in documents:
-    print(doc["url"])
-
-# etc...
-info_files = list(query=\(aqeinstein\(aq, library=\(aqpapis\(aq, info_files=True)
-
-# do something with the info file paths...
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
 .SH CLI
 .SS papis list
 .sp
 List documents\(aq properties
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis list [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-i, \-\-info
@@ -139,38 +118,45 @@
 .INDENT 0.0
 .TP
 .B \-d, \-\-dir
 Show the folder name associated with the document
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-format <format>
-List entries using a custom papis format, e.g. \(aq{doc[year] {doc[title]}
+.B \-n, \-\-notes
+List notes files, if any
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-template <template>
-Template file containing a papis format to list entries
+.B \-\-format <_format>
+List entries using a custom papis format, e.g. \(aq{doc[year] {doc[title]}
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-p, \-\-pick
-Pick the document instead of listing everything
+.B \-\-template <template>
+Template file containing a papis format to list entries
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-downloaders
 List available downloaders
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-libraries
 List defined libraries
 .UNINDENT
-Arguments.INDENT 0.0
+.INDENT 0.0
+.TP
+.B \-a, \-\-all
+Process all documents matching a query, if a query is given
+.UNINDENT
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-mv.1` & `papis-0.9/doc/build/man/papis-run.1`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-MV" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-RUN" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
-papis-mv \- mv command
+papis-run \- run command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,42 +26,77 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.sp
+This command is useful to issue commands in the directory of your library.
+.SH CLI EXAMPLES
+.INDENT 0.0
+.INDENT 3.5
+.INDENT 0.0
+.IP \(bu 2
+List files in your directory
+.UNINDENT
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis run ls
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.IP \(bu 2
+Find a file in your directory using the \fBfind\fP command
+.UNINDENT
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis run find \-name \(aqdocument.pdf\(aq
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.SH PYTHON EXAMPLES
 .SH CLI
-.SS papis mv
+.SS papis run
 .sp
-Move a document into some other path
+Run an arbitrary shell command in the library folder
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis mv [OPTIONS] [QUERY]
+papis run [OPTIONS] [RUN_COMMAND]...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
+.sp
+Arguments
 .INDENT 0.0
 .TP
-.B \-\-git, \-\-no\-git
-Add git interoperability
-.UNINDENT
-Arguments.INDENT 0.0
-.TP
-.B QUERY
-Optional argument
+.B RUN_COMMAND
+Optional argument(s)
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
 2017, Alejandro Gallo
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `papis-0.8.2/doc/build/man/papis-open.1` & `papis-0.9/doc/build/man/papis-open.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-OPEN" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-OPEN" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-open \- open command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -140,21 +140,28 @@
 .nf
 .ft C
 papis open [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-doc\-folder <doc_folder>
+Apply action to a document path
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-\-tool <tool>
 Tool for opening the file (opentool)
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-d, \-\-dir
 Open directory
@@ -165,15 +172,17 @@
 Open all matching documents
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-m, \-\-mark, \-\-no\-mark
 Open mark
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-rename.1` & `papis-0.9/doc/build/man/papis-mv.1`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-RENAME" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-MV" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
-papis-rename \- rename command
+papis-mv \- mv command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -27,38 +27,42 @@
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
 .SH CLI
-.SS papis rename
+.SS papis mv
 .sp
-Rename entry
+Move a document into some other path
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis rename [OPTIONS] [QUERY]
+papis mv [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-git, \-\-no\-git
 Add git interoperability
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-rm.1` & `papis-0.9/doc/build/man/papis-rm.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-RM" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-RM" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-rm \- rm command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -29,41 +29,55 @@
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
 .SH CLI
 .SS papis rm
 .sp
-Delete command for several objects
+Delete a document or a file
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis rm [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-git, \-\-no\-git
+Remove in git
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-\-file
 Remove files from a document instead of the whole folder
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-f, \-\-force
 Do not confirm removal
 .UNINDENT
-Arguments.INDENT 0.0
+.INDENT 0.0
+.TP
+.B \-\-all
+Remove all matches
+.UNINDENT
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis-run.1` & `papis-0.9/doc/build/man/papis-rename.1`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-RUN" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-RENAME" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
-papis-run \- run command
+papis-rename \- rename command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,73 +26,46 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.SH CLI
+.SS papis rename
 .sp
-This command is useful to issue commands in the directory of your library.
-.SH CLI EXAMPLES
-.INDENT 0.0
-.INDENT 3.5
-.INDENT 0.0
-.IP \(bu 2
-List files in your directory
-.UNINDENT
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-papis run ls
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.IP \(bu 2
-Find a file in your directory using the \fBfind\fP command
-.UNINDENT
+Rename entry
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis run find \-name \(aqdocument.pdf\(aq
+papis rename [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-.UNINDENT
-.UNINDENT
-.SH PYTHON EXAMPLES
-.SH CLI
-.SS papis run
 .sp
-Run an arbitrary shell command in the library folder
+Options
 .INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-papis run [OPTIONS] [RUN_COMMAND]...
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-Options.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.INDENT 0.0
+.TP
+.B \-\-git, \-\-no\-git
+Add git interoperability
+.UNINDENT
+.sp
+Arguments
+.INDENT 0.0
 .TP
-.B RUN_COMMAND
-Optional argument(s)
+.B QUERY
+Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
 2017, Alejandro Gallo
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `papis-0.8.2/doc/build/man/papis-update.1` & `papis-0.9/doc/build/man/papis-update.1`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS-UPDATE" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS-UPDATE" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis-update \- update command
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -41,15 +41,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis update \-\-auto \-i "author = dyson"
+papis update \-\-auto \-i "author : dyson"
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -61,15 +61,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis update \-\-from\-bibtex libraryfile.bib \-i
+papis update \-\-from bibtex libraryfile.bib \-i
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -115,85 +115,54 @@
 .nf
 .ft C
 papis update [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-i, \-\-interactive, \-b, \-\-no\-interactive
-Interactively update
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-f, \-\-force
-Force update, overwrite conflicting information
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-crossref <from_crossref>
-Update info from crossref.org
+.B \-\-git, \-\-no\-git
+Add git interoperability
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-from\-isbn <from_isbn>
-Update info from isbn
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-isbnplus <from_isbnplus>
-Update info from isbnplus.org
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-base <from_base>
-Update info from Bielefeld Academic Search Engine
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-yaml <from_yaml>
-Update info from yaml file
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-bibtex <from_bibtex>
-Update info from bibtex file
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-url <from_url>
-Get document or information from url
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-doi <from_doi>
-Doi to try to get information from
+.B \-\-doc\-folder <doc_folder>
+Apply action to a document path
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-auto
 Try to parse information from different sources
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-all
 Update all entries in library
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-s, \-\-set <set>
+.B \-\-from <from_importer>
+Add document from a specific importer (pdf2doi, yaml, crossref, folder, pmid, arxiv, lib, bibtex, doi, pdf2arxivid)
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-s, \-\-set <set_tuples>
 Update document\(aqs information with key value.The value can be a papis format.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH AUTHOR
 Alejandro Gallo
 .SH COPYRIGHT
```

### Comparing `papis-0.8.2/doc/build/man/papis.1` & `papis-0.9/doc/build/man/papis.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PAPIS" "1" "Feb 28, 2019" "0.8" "papis"
+.TH "PAPIS" "1" "Oct 21, 2019" "0.9" "papis"
 .SH NAME
 papis \- Papis Documentation
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -38,20 +38,20 @@
 .sp
 This is a tutorial that should be enough to get you started using papis.  Papis
 tries to be as simple and lightweight as possible, therefore its database
 structure is ridiculously simple.
 .sp
 But before taking a look at its database structure let us see how is the daily
 usage of papis for a regular user. This tutorial is command\-line based, so you
-should be familiar with opening a terminal window in your system.
+should be familiar with opening a terminal window on your system.
 .SS Creating a new library
 .sp
 We will illustrate the process by creating a first library with a couple of
 \fB\(gapdf\(ga\fP documents in it. Papis can be highly configured using configuration
-files. Many programs use configuration files without you maybe being aware of
+files. Many programs use configuration files maybe without you being aware of
 it. Papis\(aq configuration files are stored together inside the folder
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 ~/.config/papis
@@ -69,21 +69,21 @@
 .ft C
 ~/.config/papis/config
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-Right now we will open this file to edit and we will create a library.  In
+Right now we will open this file for editing and we will create a library.  In
 papis everything should be human\-readable and human\-editable. So adding a
 library is as easy as adding two lines to this configuration file.
 .sp
 Say that you want to create a "papers" library, where you can finally order
-all those pdf\(aqs hanging around in your computer. We can create this library
-by putting inside the config file the two lines:
+all those pdf\(aqs hanging around on your computer. We create this library
+by putting these two lines inside the config file:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 [papers]
 dir = ~/Documents/mypapers
@@ -92,28 +92,28 @@
 .UNINDENT
 .UNINDENT
 .sp
 In the above lines we have created a library with the name \fBpapers\fP which is
 located in the directory \fB~/Documents/mypapers\fP\&.  So all the documents that
 we will be adding to the library will be located inside
 \fB~/Documents/mypapers\fP, and nowhere else. Everything that papis needs to take
-care of your papers library is inside the \fB~/Documents/mypapers\fP directory,
+care of your \fBpapers\fP library is inside the \fB~/Documents/mypapers\fP directory,
 self\-contained.
 .sp
-So now add the two lines to the \fB~/.config/papis/config\fP file and save it, and we will
+If you have not already, add the two lines to the \fB~/.config/papis/config\fP file and save it, and we will
 proceed to add some documents.
 .SS Adding the first document
 .sp
 If you don\(aqt have any special pdf lying around let me choose one for you:
 \fI\%link\fP\&.
 You can download this document and we are going to add it into the \fBpapers\fP
 library.
 .sp
-Supposing that you have the document in the current directory and you have renamed
-the document to \fBdocument.pdf\fP, you can do the following to add this into your
+Assuming that you have the document in the current directory and you have renamed
+the document to \fBdocument.pdf\fP, do the following to add the pdf into your
 library:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis add document.pdf \-\-set author "Newton" \-\-set title "Principia Mathematica"
@@ -121,15 +121,15 @@
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 And it\(aqs done! We have added our first book to the library.
 .sp
 Let us see how this works exactly. Papis consists of many commands, and one of
-these commands is \fBadd\fP\&. \fBAdd\fP itself has many flags, which are options for the
+these commands is \fBadd\fP\&. \fBadd\fP itself has many flags, which are options for the
 given command. In the example above we have used the flags \fBauthor\fP and
 \fBtitle\fP to tell papis to use \fBNewton\fP as the author\(aqs name and \fBPrincipia
 Mathematica\fP as the document\(aqs title. You can see all the possible flags
 for the command \fBadd\fP if you use the \fBhelp\fP flag, i.e., if you issue the
 following command
 .INDENT 0.0
 .INDENT 3.5
@@ -138,18 +138,18 @@
 .ft C
 papis add \-\-help
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-Now you are asking yourself, what happened to the pdf file? Where it is
+Now you are asking yourself, what happened to the pdf\-file? Where is it
 stored?  Is it stored in an obscure database somewhere in my computer? No,
 papis just copied the \fBdocument.pdf\fP file into a folder inside the library
-folder \fB~/Documents/papers/\fP\&. If you go now there, you will see that a folder
+folder \fB~/Documents/papers/\fP\&. If you now go there, you will see that a folder
 with a weird name has been created. Inside of the folder there is the
 \fBdocument.pdf\fP file and another file, \fBinfo.yaml\fP\&.
 .sp
 If you open the \fBinfo.yaml\fP file you will see the following contents:
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -176,23 +176,23 @@
 .ft C
 papis open
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-and the document should just open in your default pdf viewer.
-You can change the default pdf viewer in your configuration file
+and the document should open in your default pdf\-viewer.
+You can change the default pdf\-viewer in your configuration file
 (see section on configuration\-file).
 .sp
-Now you can try to repeat the same process with another pdf file lying around.
+Now you can try to repeat the same process with another pdf\-file lying around.
 When you hit \fBpapis open\fP again, it will ask you which one you want.
 If you input parts of the title or the author\(aqs name it will try to match
 what you typed with the paper you are looking for, so that you can get the
-paper that you are looking for very easily.
+desired paper very easily.
 .SH INSTALLATION
 \fI\%\fP\fI\%\fP.SS Using pip
 .sp
 The easiest way of installing papis is using the \fBPyPi\fP repositories and
 the package manager \fBpip3\fP, just open a terminal and type in
 .INDENT 0.0
 .INDENT 3.5
@@ -213,15 +213,15 @@
 .ft C
 sudo pip3 install papis
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-of if you prefer installing it locally then simply type
+or if you prefer installing it locally then simply type
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 pip3 install \-\-user papis
 .ft P
@@ -303,15 +303,15 @@
 or download the
 \fI\%zip file\fP\&.
 .sp
 Go inside of the \fBpapis\fP source folder and you can either use the \fBMakefile\fP
 or install it with \fBpython3\fP\&.
 .SS Using the Makefile
 .sp
-Now you have to initialise the submodules, just type
+Now you have to initialize the submodules, just type
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 make submodules
 .ft P
@@ -373,50 +373,50 @@
 .sp
 The general command that you have to hit is by using the \fBsetup.py\fP script:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-python3 setup\&.py install
+python3 setup.py install
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 Again, if you want to install it locally because you don\(aqt have administrative
-rights in your computer you can just simply type
+rights on your computer you simply type
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-python3 setup\&.py install \-\-user
+python3 setup.py install \-\-user
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-If you want to develop on the code, you can also alternatively hit
+If you want to work on the code, you can alternatively hit
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-python3 setup\&.py develop \-\-user
+python3 setup.py develop \-\-user
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 \fBWARNING:\fP
 .INDENT 0.0
 .INDENT 3.5
 If you install the package locally, the program \fBpapis\fP will be installed
-by default into your \fB~/.local/bin\fP direcrtory, so that you will have to
+by default into your \fB~/.local/bin\fP directory, so that you will have to
 set your \fBPATH\fP accordingly.
 .sp
 One way of doing this in \fBbash\fP shells (\fBLinux\fP and the like, also
 \fBUbuntu\fP on Windows or \fBcygwin\fP) is by adding the following line to your
 \fB~/.bashrc\fP file
 .INDENT 0.0
 .INDENT 3.5
@@ -475,32 +475,43 @@
 .sp
 A more complete example of a configuration file is the following
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
+#
+# This is a general section, the settings set here will be set for
+# all libraries
+#
 [settings]
-# Open file with rifle, a nice python program
+#
+# General file opener program, rifle is a nice python program
+# If you\(aqre on macOS, you can write "open", if you\(aqre on linux
+# you can also write "xdg\-open", on windows\-cygwin, you can set it to
+# "cygstart"
+#
 opentool = rifle
-# Use ranger as a file browser, too a  nice python package
+# Use ranger as a file browser, a nice python program
 file\-browser = ranger
-# Ask for confirmation when doing papis add ...
+# Ask for confirmation when doing papis add
 add\-confirm = True
 # Edit the info.yaml file before adding a doc into the library
 # papis add \-\-edit
 add\-edit = True
 # Open the files before adding a document into the library
 # papis add \-\-open
 add\-open = True
-
+#
 # Define custom default match and header formats
+#
 match\-format = {doc[tags]}{doc.subfolder}{doc[title]}{doc[author]}{doc[year]}
-
+#
 # Define header format with colors and multiline support
+#
 header\-format = <red>{doc.html_escape[title]}</red>
   <span color=\(aq#ff00ff\(aq>  {doc.html_escape[author]}</span>
   <yellow>   ({doc.html_escape[year]})</yellow>
 
 [tui]
 editmode = vi
 options_list.selected_margin_style = bg:ansigreen fg:ansired
@@ -508,16 +519,22 @@
 
 
 
 # Define a lib
 [papers]
 dir = ~/Documents/papers
 
+# override settings from the section tui only for the papers library
+# you have to prepend "tui\-" to the settings
 tui\-editmode = emacs
 tui\-options_list.unselected_margin_style = bg:blue
+# use whoosh as a database for papers
+database\-backend = whoosh
+# rename files added by author and title
+add\-file\-name = {doc[author]}{doc[title]}
 
 # Define a lib for books
 [books]
 dir = ~/Documents/books
 database\-backend = whoosh
 
 # Define a lib for Videos
@@ -530,23 +547,14 @@
 dir = ~/contacts/general
 database\-backend = papis
 mode = contact
 header\-format = {doc[first_name]} {doc[last_name]}
 match\-format = {doc[org]} {doc[first_name]} {doc[last_name]}
 browse\-query\-format = {doc[first_name]} {doc[last_name]}
 add\-open = False
-
-rofi\-gui\-gui\-eh = 2
-rofi\-gui\-header\-format = %(header\-format)s
-                     {doc[tel][cell]}
-tk\-gui\-header\-format = %(rofi\-gui\-header\-format)s
-vim\-gui\-header\-format = Title: %(header\-format)s
-                        Tel  : {doc[tel]}
-                        Mail : {doc[email]}
-                     {doc[empty]}
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Local configuration files
 .sp
 Papis also offers the possibility of creating local configuration files.
@@ -572,33 +580,33 @@
 .ft C
 ~/Documents/papers/.papis.config
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-then everytime that you use this library also papis will source this
+then every time that you use this library papis will also source this
 configuration file.
-.SS Default settings
+.SS General settings
 .INDENT 0.0
 .TP
 \fBlocal\-config\-file\fP (\fI\%config\-settings\-local\-config\-file\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fB\&.papis.config\fP
 .UNINDENT
 .UNINDENT
 .sp
 Name AND relative path of the local configuration file that papis
 will additionally read if the file is present in the current
 directory or in the base directory of a given library.
 .sp
-This is useful for instance if you have a library somewhere
-for which you want special configuration settings to be set
-but you do not want these settings to cluster in your configuration
+This is useful, for instance, if you have a library somewhere
+for which you want special configuration settings
+but do not want these settings to cluster in your configuration
 file. It is also useful if you\(aqre sharing a library with someone
 else and you want them to have the same settings in that library as
 you. Imagine you\(aqre sharing a library of datasheets with your friend
 Fulano. You have your library at
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -705,40 +713,30 @@
 \fBdoc\-url\-key\-name\fP (\fI\%config\-settings\-doc\-url\-key\-name\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBdoc_url\fP
 .UNINDENT
 .UNINDENT
 .sp
-Some documents might have associated apart from an url also a file url,
-the key name appearing in the information file is defined by
+Some documents might have, apart from an url, also a file url associated with them.
+The key name appearing in the information file is defined by
 this setting.
 .INDENT 0.0
 .TP
 \fBdefault\-library\fP (\fI\%config\-settings\-default\-library\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBpapers\fP
 .UNINDENT
 .UNINDENT
 .sp
 The name of the library that is to be searched when \fBpapis\fP
 is run without library arguments.
 .INDENT 0.0
 .TP
-\fBexport\-text\-format\fP (\fI\%config\-settings\-export\-text\-format\fP)
-.INDENT 7.0
-.IP \(bu 2
-\fBDefault\fP: \fB{doc[author]}. {doc[title]}. {doc[journal]} {doc[pages]} {doc[month]} {doc[year]}\fP
-.UNINDENT
-.UNINDENT
-.sp
-The default output papis format for \fBpapis export \-\-text\fP\&.
-.INDENT 0.0
-.TP
 \fBformat\-doc\-name\fP (\fI\%config\-settings\-format\-doc\-name\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBdoc\fP
 .UNINDENT
 .UNINDENT
 .sp
@@ -754,76 +752,43 @@
 .IP \(bu 2
 \fBDefault\fP: \fB{doc[tags]}{doc.subfolder}{doc[title]}{doc[author]}{doc[year]}\fP
 .UNINDENT
 .UNINDENT
 .sp
 Default format that is used to match a document against in order to select
 it. For example if the \fBmatch\-format\fP is equal to
-\fB{doc[year]} {doc[author]}\fP then title of a document will not work
+\fB{doc[year]} {doc[author]}\fP then the title of a document will not work
 to match a document, only the year and author.
 .INDENT 0.0
 .TP
 \fBheader\-format\fP (\fI\%config\-settings\-header\-format\fP)
 .INDENT 7.0
 .IP \(bu 2
 .INDENT 2.0
 .TP
 \fBDefault\fP: 
 .INDENT 7.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-<red>{doc.html_escape[title]}</red>
- <span color=\(aq#00ff00\(aq>{doc.html_escape[author]}</span>
-  <span color=\(aq#00ffaa\(aq>({doc.html_escape[year]})</span> [<yellow>{doc.html_escape[tags]}</yellow>]
+<ansired>{doc.html_escape[title]}</ansired>
+ <ansigreen>{doc.html_escape[author]}</ansigreen>
+  <blue>({doc.html_escape[year]})</blue> [<ansiyellow>{doc.html_escape[tags]}</ansiyellow>]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
 Default format that is used to show a document in order to select it.
 .INDENT 0.0
 .TP
-\fBformat\-jinja2\-enable\fP (\fI\%config\-settings\-format\-jinja2\-enable\fP)
-.INDENT 7.0
-.IP \(bu 2
-\fBDefault\fP: \fBFalse\fP
-.UNINDENT
-.UNINDENT
-.sp
-This setting is to enable the \fI\%jinja2\fP template
-engine to render the papis templates being used, as \fBheader\-format\fP,
-\fBmatch\-format\fP etc...
-.sp
-For instance you could set the option \fBheader\-format\fP to
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-<span color=\(aq#ff00ff\(aq>{{doc.html_escape["title"]}}</span>
-<span color=\(aq#00ff00\(aq>  {{doc.html_escape["author"]}}</span>
-<span color=\(aq#00ffaa\(aq>   ({{doc.html_escape["year"]}}) </span>
-{%\- if doc.has(\(aqtags\(aq) %}<span>[<yellow>{{doc[\(aqtags\(aq]}}</yellow>] </span>{%\- endif %}
-{%\- if doc.has(\(aqcitations\(aq) %}<red>{{doc[\(aqcitations\(aq]|length}}</red>{%\- endif %}
-{%\- if doc.has(\(aqurl\(aq) %}
-<span>    {{doc.html_escape["url"]}}</span>
-{%\- endif %}
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.sp
-To use it, just install jinja2.
-.INDENT 0.0
-.TP
 \fBheader\-format\-file\fP (\fI\%config\-settings\-header\-format\-file\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBNone\fP
 .UNINDENT
 .UNINDENT
 .sp
@@ -865,17 +830,17 @@
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBxdg\-open\fP
 .UNINDENT
 .UNINDENT
 .sp
 This is the general program that will be used to open documents.
-As for now papis is not intended to detect the type of document to be open
-and decide upon it how to open the document. You should set this
-to the right program for the tool. If you are in linux you might want
+As for now papis is not intended to detect the type of document to be opened
+and decide upon how to open the document. You should set this
+to the right program for the tool. If you are on linux you might want
 to take a look at \fI\%ranger\fP or let
 the default handle it in your system.
 For mac users you might set this to \fBopen\fP\&.
 .INDENT 0.0
 .TP
 \fBbrowser\fP (\fI\%config\-settings\-browser\fP)
 .INDENT 7.0
@@ -887,53 +852,53 @@
 Program to be used for opening websites, the default is the environment
 variable \fB$BROWSER\fP\&.
 .INDENT 0.0
 .TP
 \fBpicktool\fP (\fI\%config\-settings\-picktool\fP)
 .INDENT 7.0
 .IP \(bu 2
-\fBDefault\fP: \fBpapis.pick\fP
+\fBDefault\fP: \fBpapis\fP
 .UNINDENT
 .UNINDENT
 .sp
 This is the program used whenever papis asks you to pick a document
 or options in general.
 .INDENT 0.0
 .TP
-.B Possible options are:
+.B Only option is:
 .INDENT 7.0
 .IP \(bu 2
-papis.pick
+papis
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 \fBeditor\fP (\fI\%config\-settings\-editor\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fB$EDITOR\fP
 .UNINDENT
 .UNINDENT
 .sp
-Editor used to edit files in papis, for instance for the \fBpapis edit\fP
+Editor used to edit files in papis, e.g., for the \fBpapis edit\fP
 command. It defaults to the \fB$EDITOR\fP environment variable, if this is
 not set then it will default to the \fB$VISUAL\fP environment variable.
 Otherwise the default editor in your system will be used.
 .INDENT 0.0
 .TP
 \fBfile\-browser\fP (\fI\%config\-settings\-file\-browser\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBxdg\-open\fP
 .UNINDENT
 .UNINDENT
 .sp
-File browser to be used when opening a directory, it defaults to the
-default file browser in your system, however you can set it to different
-file browsers such as \fBdolphin\fP, \fBthunar\fP, \fBranger\fP to name a few.
+File browser to be used when opening a directory. It defaults to the
+default file browser in your system, however, you can set it to different
+file browsers such as \fBdolphin\fP, \fBthunar\fP or \fBranger\fP just to name a few.
 .SS Bibtex options
 .INDENT 0.0
 .TP
 \fBbibtex\-journal\-key\fP (\fI\%config\-settings\-bibtex\-journal\-key\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBjournal\fP
@@ -947,58 +912,63 @@
 Set as \fBfull_journal_title\fP or \fBabbrev_journal_title\fP for
 whichever style required. Default is \fBjournal\fP\&.
 .INDENT 0.0
 .TP
 \fBextra\-bibtex\-keys\fP (\fI\%config\-settings\-extra\-bibtex\-keys\fP)
 .INDENT 7.0
 .IP \(bu 2
-\fBDefault\fP: 
-.nf
-\(ga\(ga
-.fi
-
-.nf
-\(ga\(ga
-.fi
-
+\fBDefault\fP: \fB[]\fP
 .UNINDENT
 .UNINDENT
 .sp
 When exporting documents in bibtex format, you might want to add
-non\-standard bibtex keys such as \fBdoc_url\fP or \fBtags\fP, you can add
-these here as comma separated values, for example
-\fBextra\-bibtex\-keys = tags, doc_url\fP\&.
+non\-standard bibtex keys such as \fBdoc_url\fP or \fBtags\fP\&. You can add
+these as a valid python list of strings, for instance:
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+[mylib]
+extra\-bibtex\-keys = ["tags", "doc_url"]
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
 .INDENT 0.0
 .TP
 \fBextra\-bibtex\-types\fP (\fI\%config\-settings\-extra\-bibtex\-types\fP)
 .INDENT 7.0
 .IP \(bu 2
-\fBDefault\fP: 
-.nf
-\(ga\(ga
-.fi
-
+\fBDefault\fP: \fB[]\fP
+.UNINDENT
+.UNINDENT
+.sp
+Allow non\-standard bibtex types to be recognized, e.g,
+.INDENT 0.0
+.INDENT 3.5
+.sp
 .nf
-\(ga\(ga
+.ft C
+[mylib]
+extra\-bibtex\-types = ["wikipedia", "video", "song"]
+.ft P
 .fi
-
 .UNINDENT
 .UNINDENT
 .sp
-Allow non\-standard bibtex types to be recognized, e.g,
-\fBextra\-bibtex\-types = wikipedia, video, song\fP\&.
 See
 \fI\%bibtex
 reference\fP\&.
 .INDENT 0.0
 .TP
 \fBmultiple\-authors\-format\fP (\fI\%config\-settings\-multiple\-authors\-format\fP)
 .INDENT 7.0
 .IP \(bu 2
-\fBDefault\fP: \fB{au[surname]}, {au[given_name]}\fP
+\fBDefault\fP: \fB{au[family]}, {au[given]}\fP
 .UNINDENT
 .UNINDENT
 .sp
 When retrieving automatic author information from services like
 crossref.org, papis usually builds the \fBauthor\fP field for the
 given document. The format how every single author name is built
 is given by this setting, for instance you could customize it
@@ -1034,15 +1004,15 @@
 \fBbibtex\-unicode\fP (\fI\%config\-settings\-bibtex\-unicode\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBFalse\fP
 .UNINDENT
 .UNINDENT
 .sp
-Wether or not to allow direct unicode characters in the document
+Whether or not to allow direct unicode characters in the document
 fields to be exported into the bibtex text.
 .SS \fBpapis add\fP options
 .INDENT 0.0
 .TP
 \fBref\-format\fP (\fI\%config\-settings\-ref\-format\fP)
 .INDENT 7.0
 .IP \(bu 2
@@ -1071,100 +1041,100 @@
 \fBadd\-confirm\fP (\fI\%config\-settings\-add\-confirm\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBFalse\fP
 .UNINDENT
 .UNINDENT
 .sp
-If set to \fBTrue\fP, everytime you run \fBpapis add\fP
+If set to \fBTrue\fP, every time you run \fBpapis add\fP
 the flag \fB\-\-confirm\fP will be added automatically. If is set to \fBTrue\fP
 and you add it, i.e., you run \fBpapis add \-\-confirm\fP, then it will
 fave the contrary effect, i.e., it will not ask for confirmation.
 .INDENT 0.0
 .TP
-\fBadd\-name\fP (\fI\%config\-settings\-add\-name\fP)
+\fBadd\-folder\-name\fP (\fI\%config\-settings\-add\-folder\-name\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBempty string\fP
 .UNINDENT
 .UNINDENT
 .sp
-Default name for the folder of newly added documents. For example, if you
+Default name for the folder of newly added documents. For example, if you want
 the folder of your documents to be named after the format
 \fBauthor\-title\fP then you should set it to
 the papis format: \fB{doc[author]}\-{doc[title]}\fP\&.
 Per default a hash followed by the author name is created.
 .INDENT 0.0
 .TP
-\fBfile\-name\fP (\fI\%config\-settings\-file\-name\fP)
+\fBadd\-file\-name\fP (\fI\%config\-settings\-add\-file\-name\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBNone\fP
 .UNINDENT
 .UNINDENT
 .sp
-Same as \fBadd\-name\fP, but for files, not folders. If it is not set,
+Same as \fBadd\-folder\-name\fP, but for files, not folders. If it is not set,
 the names of the files will be cleaned and taken \fIas\-is\fP\&.
 .INDENT 0.0
 .TP
 \fBadd\-interactive\fP (\fI\%config\-settings\-add\-interactive\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBFalse\fP
 .UNINDENT
 .UNINDENT
 .sp
-If set to \fBTrue\fP, everytime you run \fBpapis add\fP
+If set to \fBTrue\fP, every time you run \fBpapis add\fP
 the flag \fB\-\-interactive\fP will be added automatically. If is set to
 \fBTrue\fP and you add it, i.e., you run \fBpapis add \-\-interactive\fP, then it
 will fave the contrary effect, i.e., it will not run in interactive mode.
 .INDENT 0.0
 .TP
 \fBadd\-edit\fP (\fI\%config\-settings\-add\-edit\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBFalse\fP
 .UNINDENT
 .UNINDENT
 .sp
-If set to \fBTrue\fP, everytime you run \fBpapis add\fP
-the flag \fB\-\-edit\fP will be added automatically. If is set to
-\fBTrue\fP and you add it, i.e., you run \fBpapis add \-\-edit\fP, then it
-will fave the contrary effect, i.e., it will not prompt to edit the info
+If set to \fBTrue\fP, every time you run \fBpapis add\fP
+the flag \fB\-\-edit\fP will be added automatically. If it is set to
+\fBTrue\fP and you add something, i.e., you run \fBpapis add \-\-edit\fP, then it
+will have the contrary effect, i.e., it will not prompt to edit the info
 file.
 .INDENT 0.0
 .TP
 \fBadd\-open\fP (\fI\%config\-settings\-add\-open\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBFalse\fP
 .UNINDENT
 .UNINDENT
 .sp
-If set to \fBTrue\fP, everytime you run \fBpapis add\fP
-the flag \fB\-\-open\fP will be added automatically. If is set to
-\fBTrue\fP and you add it, i.e., you run \fBpapis add \-\-open\fP, then it
-will fave the contrary effect, i.e., it will not open the attached files
+If set to \fBTrue\fP, every time you run \fBpapis add\fP
+the flag \fB\-\-open\fP will be added automatically. If it is set to
+\fBTrue\fP and you add something, i.e., you run \fBpapis add \-\-open\fP, then it
+will have the contrary effect, i.e., it will not open the attached files
 before adding the document to the library.
 .SS \fBpapis browse\fP options
 .INDENT 0.0
 .TP
 \fBbrowse\-key\fP (\fI\%config\-settings\-browse\-key\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBurl\fP
 .UNINDENT
 .UNINDENT
 .sp
 This command provides the key that is used to generate the
-url. For users that \fBpapis add \-\-from\-doi\fP, setting browse\-key
+url. For users that run \fBpapis add \-\-from\-doi\fP, setting browse\-key
 to \fBdoi\fP constructs the url from dx.doi.org/DOI, providing a
 much more accurate url.
 .sp
-Default value is set to \fBurl\fP\&. If the user needs functionality
+Default value is set to \fBurl\fP\&. If you need functionality
 with the \fBsearch\-engine\fP option, set the option to an empty
 string e.g.
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
@@ -1192,15 +1162,15 @@
 \fBopen\-mark\fP (\fI\%config\-settings\-open\-mark\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBFalse\fP
 .UNINDENT
 .UNINDENT
 .sp
-If this option is set to \fBTrue\fP, then every time that papis opens
+If this option is set to \fBTrue\fP, every time papis opens
 a document it will ask to open a mark first.
 If it is set to \fBFalse\fP, then doing
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
@@ -1216,16 +1186,16 @@
 \fBmark\-key\-name\fP (\fI\%config\-settings\-mark\-key\-name\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBmarks\fP
 .UNINDENT
 .UNINDENT
 .sp
-This is the default key name for the marks in the info file, for
-example if you set \fBmark\-key\-name = bookmarks\fP then you would have
+This is the default key name for the marks in the info file. For
+example, if you set \fBmark\-key\-name = bookmarks\fP then you would have
 in your \fBinfo.yaml\fP file
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 author: J. Krishnamurti
@@ -1254,17 +1224,17 @@
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fB{mark[name]} \- {mark[value]}\fP
 .UNINDENT
 .UNINDENT
 .sp
 This is the format in which the mark will appear whenever the user
-has to pick one, you can change this in order to make \fBmarks\fP work
+has to pick one. You can change this in order to make \fBmarks\fP work
 in the way you like. Per default it is assumed that every mark
-has a \fBname\fP and a \fBvalue\fP key, but this you can change.
+has a \fBname\fP and a \fBvalue\fP key.
 .INDENT 0.0
 .TP
 \fBmark\-match\-format\fP (\fI\%config\-settings\-mark\-match\-format\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fB{mark[name]} \- {mark[value]}\fP
 .UNINDENT
@@ -1355,42 +1325,42 @@
 .IP \(bu 2
 \fBDefault\fP: \fB\&.\fP
 .UNINDENT
 .UNINDENT
 .sp
 This is the default query that a command will take if no
 query string is typed in the command line. For example this is
-the query that is passed to the command open whenever no search
+the query that is passed to the command \fBopen\fP whenever no search
 string is typed:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis open
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-Imagine you want to have all your papers whenever you do not
-specify an input query string, then you would set
+Imagine you want to open all papers authored by \fBJohn Smith\fP whenever you do not
+specify an input query string, i.e., \fBpapis open\fP\&. Then setting
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-default\-query\-string = author="John Smith"
+default\-query\-string = author:"John Smith"
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-and whenever you typed \fBpapis open\fP, onlye the \fBJohn Smith\fP authored
-papers would appear. Notice that the current example has been
+would do the trick.
+Notice that the current example has been
 done assuming the \fBdatabase\-backend = papis\fP\&.
 .INDENT 0.0
 .TP
 \fBdatabase\-backend\fP (\fI\%config\-settings\-database\-backend\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fBpapis\fP
@@ -1413,28 +1383,28 @@
 for the given library. This is only effective if you\(aqre using the
 \fBpapis\fP database\-backend.
 .INDENT 0.0
 .TP
 \fBcache\-dir\fP (\fI\%config\-settings\-cache\-dir\fP)
 .INDENT 7.0
 .IP \(bu 2
-\fBDefault\fP: \fBNone\fP
+\fBDefault\fP: \fB$XDG_CACHE_HOME\fP
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 \fBwhoosh\-schema\-fields\fP (\fI\%config\-settings\-whoosh\-schema\-fields\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fB[\(aqdoi\(aq]\fP
 .UNINDENT
 .UNINDENT
 .sp
 Python list with the \fBTEXT\fP fields that should be included in the
-whoosh database schema. For instance say that you want to be able
+whoosh database schema. For instance, say that you want to be able
 to search for the \fBdoi\fP and \fBref\fP of the documents, then you could
 include
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
@@ -1473,15 +1443,15 @@
 This is the model for the whoosh schema, check
 \fI\%the documentation\fP
 for more information.
 .SS Terminal user interface (picker)
 .sp
 These options are for the terminal user interface (tui).
 They are defined in the section \fBtui\fP which means that you can set them
-in your configuration file globaly like
+in your configuration file globally like
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 [tui]
 status_line_format = "F1: Help"
@@ -1494,15 +1464,15 @@
 or inside the library sections prepending a \fBtui\-\fP,
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 [papers]
-tui\-status_line_format = "Library papers"
+tui\-status_line_format = "Library papers**
 \&...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
@@ -1513,17 +1483,16 @@
 .nf
 \(ga\(ga
 .fi
 {selected_index}/{number_of_documents}  F1:help  c\-l:redraw  \(ga\(ga
 .UNINDENT
 .UNINDENT
 .sp
-This is the format of the string that appears on the bottom line in the
-status line.
-Right now there are only two variables defined:
+This is the format of the string that appears at the bottom in the
+status line.  Right now there are only two variables defined:
 .INDENT 0.0
 .IP \(bu 2
 \fBselected_index\fP
 .IP \(bu 2
 \fBnumber_of_documents\fP
 .UNINDENT
 .sp
@@ -1694,27 +1663,14 @@
 .IP \(bu 2
 \fBDefault\fP: \fBend\fP
 .UNINDENT
 .UNINDENT
 .SS Other
 .INDENT 0.0
 .TP
-\fBcitation\-string\fP (\fI\%config\-settings\-citation\-string\fP)
-.INDENT 7.0
-.IP \(bu 2
-\fBDefault\fP: \fB*\fP
-.UNINDENT
-.UNINDENT
-.sp
-string that can be displayed in header if the reference has a
-citation
-.sp
-Default set to \(aq*\(aq
-.INDENT 0.0
-.TP
 \fBunique\-document\-keys\fP (\fI\%config\-settings\-unique\-document\-keys\fP)
 .INDENT 7.0
 .IP \(bu 2
 \fBDefault\fP: \fB[\(aqdoi\(aq,\(aqref\(aq,\(aqisbn\(aq,\(aqisbn10\(aq,\(aqurl\(aq,\(aqdoc_url\(aq]\fP
 .UNINDENT
 .UNINDENT
 .sp
@@ -1724,25 +1680,65 @@
 Which keys are checked against is decided by this option, which
 should be formatted as a python list, just as in the default value.
 .sp
 For instance, if you add a paper with a given \fBdoi\fP, and then you
 add another document with the same \fBdoi\fP, then papis will notify
 you that there is already another document with this \fBdoi\fP because
 the \fBdoi\fP key is part of the \fBunique\-document\-keys\fP option.
+.INDENT 0.0
+.TP
+\fBdocument\-description\-format\fP (\fI\%config\-settings\-document\-description\-format\fP)
+.INDENT 7.0
+.IP \(bu 2
+\fBDefault\fP: \fB{doc[title]} \- {doc[author]}\fP
+.UNINDENT
+.UNINDENT
+.sp
+\fBpapis\fP sometimes will have to tell you which document it is processing
+through text, for instance, imagine you are updating a document
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+author: Albert Einstein
+title: General Relativity
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+and papis is doing something with it. Then if your
+\fBdocument\-description\-format\fP is set to
+\fB{doc[title]} \- {doc[author]}\fP, you will see that papis tells you
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+\&.....
+Updating \(aqGeneral Relativity \- Albert Einstein\(aq
+\&...
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+so you will know exactly what is going on.
 .SH THE INFO.YAML FILE
 .sp
-At the heart of papis there is the information file.  The info file contains
+At the heart of papis there is the information file. The info file contains
 all information about the documents.
 .sp
 It uses the \fI\%yaml\fP syntax to store
-information, which is a very human readable language. It is quite format free,
+information, which is a very human\-readable language. It is quite format\-free:
 \fIpapis\fP does not assume that any special information should be there.
 .sp
 If you are storing papers with papis, then you most probably would like to
-store author and title in there,
+store author and title in there like this:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 author: Isaac Newton
 title: Opticks, or a treatise of the reflections refractions, inflections and
@@ -1796,83 +1792,131 @@
  \ \      ├── notes.tex
  \ \      └── output.pdf
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-The first thing that you might notice is that there are really many folders of
-course. Just to check that you undeerstand exactly what is a document, just
+The first thing that you might notice is that there are many folders.
+Just to check that you understand exactly what is a document,
 please think about which of these pdfs is not a valid papis document... That\(aqs
 right!, \fBfolder1/paper.pdf\fP is not a valid document since the folder1 does not
 contain any \fBinfo.yaml\fP file. You see also that it does not matter how deep the
-folder structure is, you can have in your library a \fBphysics\fP folder, where you
-have a \fBnewton\fP folder, where also you have a folder containing the actual book
+folder structure is in your library: you can have a \fBphysics\fP folder in which you
+have a \fBnewton\fP folder in which you have a folder containing the actual book
 \fBdocument.pdf\fP plus some supplementary information \fBsupplements.pdf\fP\&.  In this
-case inside the \fBinfo.yaml\fP you would have the following \fBfile\fP section
+case, inside the \fBinfo.yaml\fP you would have the following \fBfile\fP section
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 files:
 \- document.pdf
 \- supplements.pdf
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-so that you are telling papis that in this folder there are two relevant files.
+which tells papis that this folder contains two relevant files.
 .SH THE DATABASE
 .sp
 One of the things that makes papis interesting is the fact that
 there can be many backends for the database system, including no database.
 .sp
-Right now there are three types of database in that the user can use:
+Right now there are three types of databases that the user can use:
 .INDENT 0.0
 .IP \(bu 2
-No database
+.INDENT 2.0
+.TP
+.B No database
+.INDENT 7.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+database\-backend = papis
+use\-cache = False
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.UNINDENT
 .IP \(bu 2
 Simple cache based database
+\- Configuration option
+.INDENT 2.0
+.INDENT 3.5
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+database\-backend = papis
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
 .IP \(bu 2
-\fI\%Whoosh\fP  based database.
+.INDENT 2.0
+.TP
+.B \fI\%Whoosh\fP  based database.
+.INDENT 7.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+database\-backend = whoosh
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.UNINDENT
 .UNINDENT
 .sp
-If you just plan to have or have few dozen of documents in your library,
-probably you\(aqll have ample performance with the two first options.
-However if you\(aqre reaching higher numbers, 500, 1000, 2000 documents,
+If you just plan to have up to 3000 documents in your library,
+you will have ample performance with the two first options.
+However if you\(aqre reaching higher numbers,
 you\(aqll probably want to use the \fBWhoosh\fP backend for very good performance.
 .sp
-You can select the databases using the flag
+You can select a database by using the flag
 database\-backend\&.
 .SS Papis database
 .sp
 The fact that there is no database means that papis should crawl through
 the library folder and see which folders have an \fBinfo.yaml\fP file, which
-is for slow computers quite bad.
+is for slow computers (and harddrives) quite bad.
 .sp
 Papis implements a very rudimentary caching system. A cache is created for
-every library. Inside the cache only the paths to the different valid papis
-documents are stored.
+every library. Inside the cache the whole information already converted
+into python is stored.
 .sp
 These cache files are stored per default in
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 ~/.cache/papis/
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-Some papis commands update the cache automatically, for example the \fBadd\fP and
-\fBrm\fP command clear the cache when something is changed.
+Notice that most papis commands will update the cache if it has to be the case.
+For instance the \fBedit\fP command will let you edit your document\(aqs information
+and after you are done editing it will update the information for the given
+document in the cache.
+If you go directly to the document and edit the info file without
+passing through the papis edit command, the cache will not be updated and
+therefore papis will not know of these changes, although they will be there.
+In such cases you will have to \fIclear the cache\fP\&.
 .SS Clearing the cache
 .sp
 To clear the cache for a given library you can use the flag
 \fB\-\-clear\-cache\fP, e.g.
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1883,63 +1927,63 @@
 .fi
 .UNINDENT
 .UNINDENT
 .SS Query language
 .sp
 Since version \fI0.3\fP there is a query language in place for the searching
 of documents.
-The queries can contain any field of the info file, i.e.,
-\fBauthor=einstein publisher = review\fP will match documents that have
-a matching \fBauthor\fP with \fBeinstein\fP AND having a \fBpublisher\fP
+The queries can contain any field of the info file, e.g.,
+\fBauthor:einstein publisher : review\fP will match documents that have
+a matching \fBauthor\fP with \fBeinstein\fP AND have a \fBpublisher\fP
 matching \fBreview\fP\&.
 The AND part here is important, since
 only the \fBAND\fP filter is implemented in this simple query
-language, at the moment it is not possible to do an \fBOR\fP\&.
+language. At the moment it is not possible to do an \fBOR\fP\&.
 If you need this, you should consider using the
 \fI\%Whoosh database\fP\&.
 .sp
-To illustrate it here are some examples:
+For illustration, here are some examples:
 .INDENT 0.0
 .INDENT 3.5
 .INDENT 0.0
 .IP \(bu 2
-Open documents where the author key matches \(aqalbert\(aq (ignoring case),
+Open documents where the author key matches \(aqalbert\(aq (ignoring case) and
 year matches \(aq19\(aq (i.e., 1990, 2019, 1920):
 .INDENT 2.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis open \(aqauthor = albert year = 05\(aq
+papis open \(aqauthor : albert year : 05\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
 Add the restriction to the previous search that the usual matching matches
 the substring \(aqlicht\(aq in addition to the previously selected
 .INDENT 2.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis open \(aqauthor = albert year = 05 licht\(aq
+papis open \(aqauthor : albert year : 05 licht\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 This is not to be mixed with the restriction that the key \fIyear\fP matches
 \fI\(aq05 licht\(aq\fP, which will not match any year, i.e.
 .INDENT 2.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis open \(aqauthor = albert year = "05 licht"\(aq
+papis open \(aqauthor : albert year : "05 licht"\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
@@ -1982,15 +2026,15 @@
 .INDENT 0.0
 .IP \(bu 2
 whoosh\-schema\-fields
 .IP \(bu 2
 whoosh\-schema\-prototype
 .UNINDENT
 .sp
-The prototype is for advanced users. If you just want to say, include
+The prototype is for advanced users. If you just want to, say, include
 the publisher to the fields that you can search in, then you can put
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 whoosh\-schema\-fields = [\(aqpublisher\(aq]
@@ -2051,15 +2095,16 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis add ~/Documents/interesting.pdf \-\-name interesting\-paper\-2021
+papis add ~/Documents/interesting.pdf \e
+    \-\-folder\-name interesting\-paper\-2021
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
@@ -2069,15 +2114,15 @@
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis add ~/Documents/interesting.pdf \e
-    \-\-name interesting\-paper\-2021 \e
+    \-\-folder\-name interesting\-paper\-2021 \e
     \-\-set author \(aqJohn Smith\(aq \e
     \-\-set title \(aqThe interesting life of bees\(aq \e
     \-\-set year 1985 \e
     \-\-set tags \(aqbiology interesting bees\(aq
 .ft P
 .fi
 .UNINDENT
@@ -2091,15 +2136,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis add ~/Documents/interesting.pdf \-\-from\-doi 10.10763/1.3237134
+papis add ~/Documents/interesting.pdf \-\-from doi 10.10763/1.3237134
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -2108,15 +2153,15 @@
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis \-l machine\-learning add \e
-    \-\-from\-url https://arxiv.org/abs/1712.03134
+    \-\-from url https://arxiv.org/abs/1712.03134
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -2126,65 +2171,96 @@
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis add \-\-link ~/Documents/interesting.pdf \e
-    \-\-from\-doi 10.10763/1.3237134
+    \-\-from doi 10.10763/1.3237134
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
 will add an entry into the papis library, but the pdf document will remain
 at \fB~/Documents/interesting.pdf\fP, and in the document\(aqs folder
 there will be a link to \fB~/Documents/interesting.pdf\fP instead of the
 file itself. Of course you always have to be sure that the
 document at \fB~/Documents/interesting.pdf\fP does not disappear, otherwise
 you will end up without a document to open.
+.IP \(bu 2
+Papis also tries to make sense of the inputs that you have passed
+to the command, for instance you could provide only a \fBdoi\fP and
+papis will try to know if this is indeed a \fBdoi\fP
+.INDENT 2.0
+.INDENT 3.5
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis add 10.1103/PhysRevLett.123.156401
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.sp
+or from a \fBurl\fP
+.INDENT 2.0
+.INDENT 3.5
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis add https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.123.156401
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
 .UNINDENT
 .SS Examples in python
 .sp
 There is a python function in the add module that can be used to interact
 in a more effective way in python scripts,
 .INDENT 0.0
 .TP
-.B papis.commands.add.run(paths, data={}, name=None, file_name=None, subfolder=None, interactive=False, confirm=False, open_file=False, edit=False, commit=False, link=False)
+.B papis.commands.add.run(paths, data={}, folder_name=None, file_name=None, subfolder=None, confirm=False, open_file=False, edit=False, git=False, link=False)
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
 \fBpaths\fP (\fI[\fP\fI]\fP) \-\- Paths to the documents to be added
 .IP \(bu 2
 \fBdata\fP (\fIdict\fP) \-\- Data for the document to be added.
 If more data is to be retrieved from other sources, the data dictionary
 will be updated from these sources.
 .IP \(bu 2
-\fBname\fP (\fIstr\fP) \-\- Name of the folder where the document will be stored
+\fBfolder_name\fP (\fIstr\fP) \-\- Name of the folder where the document will be stored
 .IP \(bu 2
 \fBfile_name\fP (\fIstr\fP) \-\- File name of the document\(aqs files to be stored.
 .IP \(bu 2
 \fBsubfolder\fP (\fIstr\fP) \-\- Folder within the library where the document\(aqs folder
 should be stored.
 .IP \(bu 2
-\fBinteractive\fP (\fIbool\fP) \-\- Wether or not interactive functionality of this command
-should be activated.
-.IP \(bu 2
 \fBconfirm\fP (\fIbool\fP) \-\- Wether or not to ask user for confirmation before adding.
 .IP \(bu 2
 \fBopen_file\fP (\fIbool\fP) \-\- Wether or not to ask user for opening file before adding.
 .IP \(bu 2
 \fBedit\fP (\fIbool\fP) \-\- Wether or not to ask user for editing the infor file
 before adding.
 .IP \(bu 2
-\fBcommit\fP (\fIbool\fP) \-\- Wether or not to ask user for committing before adding,
+\fBgit\fP (\fIbool\fP) \-\- Wether or not to ask user for committing before adding,
 in the case of course that the library is a git repository.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS Cli
 .SS papis add
 .sp
@@ -2195,78 +2271,50 @@
 .nf
 .ft C
 papis add [OPTIONS] [FILES]...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-s, \-\-set <set_list>
 Set some information before
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-d, \-\-dir <directory>
+.B \-d, \-\-subfolder <subfolder>
 Subfolder in the library
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-i, \-\-interactive, \-\-no\-interactive
-Do some of the actions interactively
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-name <name>
+.B \-\-folder\-name <folder_name>
 Name for the document\(aqs folder (papis format)
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-file\-name <file_name>
 File name for the document (papis format)
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-from\-bibtex <from_bibtex>
-Parse information from a bibtex file
+.B \-\-from <from_importer>
+Add document from a specific importer (pdf2doi, yaml, crossref, folder, pmid, arxiv, lib, bibtex, doi, pdf2arxivid)
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-from\-yaml <from_yaml>
-Parse information from a yaml file
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-folder <from_folder>
-Add document from folder being a valid papis document (containing info.yaml)
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-url <from_url>
-Get document and information from agiven url, a parser must be implemented
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-doi <from_doi>
-Doi to try to get information from
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-pmid <from_pmid>
-PMID to try to get information from
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-lib <from_lib>
-Add document from another library
+.B \-b, \-\-batch
+Batch mode, do not prompt or otherwise
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-confirm, \-\-no\-confirm
 Ask to confirm before adding to the collection
 .UNINDENT
 .INDENT 0.0
@@ -2277,28 +2325,30 @@
 .INDENT 0.0
 .TP
 .B \-\-edit, \-\-no\-edit
 Edit info file before adding document
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-commit, \-\-no\-commit
-Commit document if library is a git repository
+.B \-\-link, \-\-no\-link
+Instead of copying the file to the library, create a link toits original location
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-link, \-\-no\-link
-Instead of copying the file to the library, create a link toits original location
+.B \-\-git, \-\-no\-git
+Git add and commit the new document
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-no\-document
-DEPRECATION NOTICE: This option is no longer valid, it will be removed in future releases
+.B \-\-list\-importers, \-\-li
+List all available papis importers
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B FILES
 Optional argument(s)
 .UNINDENT
 .SS Addto
 .sp
 This command adds files to existing papis documents in some library.
@@ -2328,30 +2378,39 @@
 .nf
 .ft C
 papis addto [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-git, \-\-no\-git
+Add and commit files
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-f, \-\-files <files>
 File fullpaths to documents
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-file\-name <file_name>
 File name for the document (papis format)
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS Browse
 .sp
 This command will try its best to find a source in the internet for the
@@ -2374,29 +2433,211 @@
 .nf
 .ft C
 papis browse [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-k, \-\-key <key>
 Use the value of the document\(aqs key to open in the browser, e.g.doi, url, doc_url ...
 .UNINDENT
-Arguments.INDENT 0.0
+.INDENT 0.0
+.TP
+.B \-\-all
+Browse all selected documents
+.UNINDENT
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
+.SS Bibtex
+.sp
+This command helps to interact with \fIbib\fP files in your LaTeX projects.
+.SS Examples
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis bibtex                                  read new_papers.bib                   \e # Read bib file
+  cmd \(aqpapis add \-\-from\-doi {doc[doi]}\(aq   # For every entry run the command
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+I use it for opening some papers for instance
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis bibtex read new_papers.bib open
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+or to add papers to the bib
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis bibtex                read new_papers.bib \e # Read bib file
+  add einstein        \e # Pick a document with query \(aqeinstein\(aq from library
+  add heisenberg      \e # Pick a document with query \(aqheisenberg\(aq from library
+  save new_papers.bib   # Save in new_papers.bib
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+or if I update some information in my papis \fByaml\fP files then I can do
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis bibtex                read new_papers.bib \e # Read bib file
+  update \-f           \e # Update what has been read from papis library
+  save new_papers.bib   # save everything to new_papers.bib, overwriting
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+Maybe this is also interesting for you guys!
+.SS Vim integration
+.sp
+Right now, you can easily use it from vim with these simple lines
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+function! PapisBibtexRef()
+  let l:temp = tempname()
+  echom l:temp
+  silent exec "!papis bibtex ref \-o ".l:temp
+  let l:olda = @a
+  let @a = join(readfile(l:temp), \(aq,\(aq)
+  normal! "ap
+  redraw!
+  let @a = l:olda
+endfunction
+
+command! \-nargs=0 BibRef call PapisBibtexRef()
+command! \-nargs=0 BibOpen exec "!papis bibtex open"
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+And use like such: \fI\%asciicast\fP
+.SS Cli
+.SS papis add
+.sp
+Add a document into a given library
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+papis add [OPTIONS] [FILES]...
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+Options
+.INDENT 0.0
+.TP
+.B \-h, \-\-help
+Show this message and exit.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-s, \-\-set <set_list>
+Set some information before
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-d, \-\-subfolder <subfolder>
+Subfolder in the library
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-folder\-name <folder_name>
+Name for the document\(aqs folder (papis format)
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-file\-name <file_name>
+File name for the document (papis format)
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-from <from_importer>
+Add document from a specific importer (pdf2doi, yaml, crossref, folder, pmid, arxiv, lib, bibtex, doi, pdf2arxivid)
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-b, \-\-batch
+Batch mode, do not prompt or otherwise
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-confirm, \-\-no\-confirm
+Ask to confirm before adding to the collection
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-open, \-\-no\-open
+Open file before adding document
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-edit, \-\-no\-edit
+Edit info file before adding document
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-link, \-\-no\-link
+Instead of copying the file to the library, create a link toits original location
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-git, \-\-no\-git
+Git add and commit the new document
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-list\-importers, \-\-li
+List all available papis importers
+.UNINDENT
+.sp
+Arguments
+.INDENT 0.0
+.TP
+.B FILES
+Optional argument(s)
+.UNINDENT
 .SS Config
 .sp
 The command config is a useful command because it allows you to check
 the configuration settings\(aq values that your current \fIpapis\fP session
 is using.
 .sp
 For example let\(aqs say that you want to see which \fBdir\fP setting your
@@ -2453,20 +2694,24 @@
 .nf
 .ft C
 papis config [OPTIONS] OPTION
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B OPTION
 Required argument
 .UNINDENT
 .SS Main
 .SS Examples
 .INDENT 0.0
@@ -2515,15 +2760,17 @@
 .nf
 .ft C
 papis [OPTIONS] COMMAND [ARGS]...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-version
@@ -2544,14 +2791,19 @@
 .B \-c, \-\-config <config>
 Configuration file to use
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-log <log>
 Logging level
+.INDENT 7.0
+.TP
+.B Options
+INFO|DEBUG|WARNING|ERROR|CRITICAL
+.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-pick\-lib
 Pick library to use
 .UNINDENT
 .INDENT 0.0
@@ -2562,16 +2814,21 @@
 .INDENT 0.0
 .TP
 .B \-s, \-\-set <set_list>
 Set key value, e.g., \-\-set info\-name information.yaml  \-\-set opentool evince
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-nc, \-\-no\-color
+.B \-\-color <color>
 Prevent the output from having color
+.INDENT 7.0
+.TP
+.B Options
+always|auto|no
+.UNINDENT
 .UNINDENT
 .SS Edit
 .sp
 This command edits the information of the documents.
 The editor used is defined by the \fBeditor\fP configuration setting.
 .SS Cli
 .SS papis edit
@@ -2583,35 +2840,44 @@
 .nf
 .ft C
 papis edit [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-git, \-\-no\-git
+Add changes made to the info file
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-n, \-\-notes
 Edit notes associated to the document
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-all
 Edit all matching documents
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-e, \-\-editor <editor>
 Editor to be used
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS Explore
 .sp
 This command is in an experimental stage but it might be useful for many
@@ -2648,21 +2914,21 @@
 .UNINDENT
 .UNINDENT
 .sp
 will tell you which commands are available.
 Let us suppose that you want to look for some documents on crossref,
 say some papers of Schroedinger, and you want to store them into a bibtex
 file called \fBlib.bib\fP, then you could concatenate the commands
-\fBcrossref\fP and \fBexport \-\-bibtex\fP as such
+\fBcrossref\fP and \fBexport \-\-format bibtex\fP as such
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis explore crossref \-a \(aqSchrodinger\(aq export \-\-bibtex lib.bib
+papis explore crossref \-a \(aqSchrodinger\(aq export \-\-format bibtex lib.bib
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 This will store everything that you got from crossref in the file \fBlib.bib\fP
 and store in bibtex format. \fBexplore\fP is much more flexible than that,
@@ -2670,15 +2936,15 @@
 you don\(aqt want to store all retrieved documents but only one that you pick,
 the \fBpick\fP command will take care of it
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis explore crossref \-a \(aqSchrodinger\(aq pick export \-\-bibtex lib.bib
+papis explore crossref \-a \(aqSchrodinger\(aq pick export \-\-format bibtex lib.bib
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 notice how the \fBpick\fP command is situated before the \fBexport\fP\&.
 More generally you could write something like
@@ -2687,17 +2953,17 @@
 .sp
 .nf
 .ft C
 papis explore \e
     crossref \-a Schroedinger \e
     crossref \-a Einstein \e
     arxiv \-a \(aqFelix Hummel\(aq \e
-    export \-\-yaml docs.yaml \e
+    export \-\-format yaml docs.yaml \e
     pick  \e
-    export \-\-bibtex specially\-picked\-document.bib
+    export \-\-format bibtex specially\-picked\-document.bib
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 The upper command will look in crossref for documents authored by Schrodinger,
 then also by Einstein, and will look on the arxiv for papers authored by Felix
@@ -2739,15 +3005,17 @@
 .nf
 .ft C
 papis explore [OPTIONS] COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .SS arxiv
 .sp
 Look for documents on ArXiV.org.
@@ -2772,15 +3040,17 @@
 .nf
 .ft C
 papis explore arxiv [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
@@ -2838,15 +3108,17 @@
 .nf
 .ft C
 papis explore base [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
@@ -2864,47 +3136,58 @@
 .nf
 .ft C
 papis explore bibtex [OPTIONS] BIBFILE
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B BIBFILE
 Required argument
 .UNINDENT
 .SS citations
 .sp
 Query the citations of a paper
 .sp
 Example:
 .sp
 Go through the citations of a paper and export it in a yaml file
 .INDENT 0.0
 .INDENT 3.5
-papis explore citations \(aqeinstein\(aq export \-\-yaml einstein.yaml
+papis explore citations \(aqeinstein\(aq export \-\-format yaml einstein.yaml
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis explore citations [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
+.TP
+.B \-\-doc\-folder <doc_folder>
+Apply action to a document path
+.UNINDENT
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-s, \-\-save
@@ -2916,15 +3199,17 @@
 Remove the stored citations file
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-m, \-\-max\-citations <max_citations>
 Number of citations to be retrieved
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS cmd
 .sp
 Run a general command on the document list
@@ -2943,20 +3228,24 @@
 .nf
 .ft C
 papis explore cmd [OPTIONS] COMMAND
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B COMMAND
 Required argument
 .UNINDENT
 .SS crossref
 .sp
 Look for documents on crossref.org.
@@ -2970,34 +3259,65 @@
 .nf
 .ft C
 papis explore crossref [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
+General query
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-a, \-\-author <author>
+Author of the query
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-t, \-\-title <title>
+Title of the query
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-m, \-\-max <max>
+Maximum number of results
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-f, \-\-filter <filter>
+Filters to apply
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-o, \-\-order <order>
+Order of appearance according to sorting  [default: desc]
+.INDENT 7.0
+.TP
+.B Options
+asc|desc
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-s, \-\-sort <sort>
+Sorting parameter  [default: score]
+.INDENT 7.0
+.TP
+.B Options
+relevance|score|updated|deposited|indexed|published|published\-print|published\-online|issued|is\-referenced\-by\-count|references\-count
+.UNINDENT
 .UNINDENT
 .SS dissemin
 .sp
 Look for documents on dissem.in
 .sp
 Examples of its usage are
 .sp
@@ -3008,15 +3328,17 @@
 .nf
 .ft C
 papis explore dissemin [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
@@ -3034,33 +3356,35 @@
 .nf
 .ft C
 papis explore export [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-bibtex <bibtex>
-Export list of documents retrieved to a bibtex file
-.UNINDENT
-.INDENT 0.0
+.B \-f, \-\-format <format>
+Format for the document
+.INDENT 7.0
 .TP
-.B \-\-yaml <yaml>
-Export list of documents retrieved to a yaml file
+.B Options
+json|bibtex|yaml
+.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-json <json>
-Export list of documents retrieved to a json file
+.B \-o, \-\-out <out>
+Outfile to write information to
 .UNINDENT
 .SS isbn
 .sp
 Look for documents using isbnlib
 .sp
 Examples of its usage are
 .sp
@@ -3071,26 +3395,33 @@
 .nf
 .ft C
 papis explore isbn [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-s, \-\-service <service>
+.INDENT 7.0
+.TP
+.B Options
+wcat|goob|openl
+.UNINDENT
 .UNINDENT
 .SS isbnplus
 .sp
 Look for documents on isbnplus.com
 .sp
 Examples of its usage are
 .sp
@@ -3101,15 +3432,17 @@
 .nf
 .ft C
 papis explore isbnplus [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-q, \-\-query <query>
@@ -3135,20 +3468,24 @@
 .nf
 .ft C
 papis explore json [OPTIONS] JSONFILE
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B JSONFILE
 Required argument
 .UNINDENT
 .SS lib
 .sp
 Query for documents in your library
@@ -3165,62 +3502,37 @@
 .nf
 .ft C
 papis explore lib [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
-.TP
-.B \-h, \-\-help
-Show this message and exit.
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-l, \-\-library <library>
-Papis library to look
-.UNINDENT
-Arguments.INDENT 0.0
-.TP
-.B QUERY
-Optional argument
-.UNINDENT
-.SS libgen
-.sp
-Look for documents on library genesis
-.sp
-Examples of its usage are
 .sp
-papis explore libgen \-a \(aqAlbert einstein\(aq export \-\-yaml einstein.yaml
+Options
 .INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-papis explore libgen [OPTIONS]
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-Options.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-a, \-\-author <author>
+.B \-\-doc\-folder <doc_folder>
+Apply action to a document path
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-t, \-\-title <title>
+.B \-l, \-\-library <library>
+Papis library to look
 .UNINDENT
+.sp
+Arguments
 .INDENT 0.0
 .TP
-.B \-i, \-\-isbn <isbn>
+.B QUERY
+Optional argument
 .UNINDENT
 .SS pick
 .sp
 Pick a document from the retrieved documents
 .sp
 Examples of its usage are
 .sp
@@ -3231,15 +3543,17 @@
 .nf
 .ft C
 papis explore pick [OPTIONS]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-n, \-\-number <number>
@@ -3258,20 +3572,24 @@
 .nf
 .ft C
 papis explore yaml [OPTIONS] YAMLFILE
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B YAMLFILE
 Required argument
 .UNINDENT
 .SS Export
 .sp
 The export command is useful to work with other programs such as bibtex.
@@ -3282,41 +3600,41 @@
 Export one of the documents matching the author with einstein to bibtex:
 .UNINDENT
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis export \-\-bibtex \(aqauthor = einstein\(aq
+papis export \-\-format bibtex \(aqauthor : einstein\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 or export all of them
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis export \-\-bibtex \-\-all \(aqauthor = einstein\(aq
+papis export \-\-format bibtex \-\-all \(aqauthor : einstein\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 Export all documents to bibtex and save them into a \fBlib.bib\fP file
 .UNINDENT
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis export \-\-all \-\-bibtex \-\-out lib.bib
+papis export \-\-all \-\-format bibtex \-\-out lib.bib
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 Export a folder of one of the documents matching the word \fBkrebs\fP
@@ -3328,26 +3646,14 @@
 .nf
 .ft C
   papis export \-\-folder \-\-out interesting\-document krebs
 
 this will create the folder \(ga\(gainteresting\-document\(ga\(ga containing the
 \(ga\(gainfo.yaml\(ga\(ga file, the linked documents and a \(ga\(gabibtex\(ga\(ga file for
 sharing with other people.
-
-You can also just export its associated document:
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-papis export \-\-file krebs
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Cli
 .SS papis export
 .sp
@@ -3358,61 +3664,50 @@
 .nf
 .ft C
 papis export [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-yaml
-Export into yaml
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-bibtex
-Export into bibtex
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-json
-Export into json
-.UNINDENT
-.INDENT 0.0
-.TP
 .B \-\-folder
 Export document folder to share
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-o, \-\-out <out>
 Outfile or outdir
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-t, \-\-text
-Text formated reference
+.B \-f, \-\-format <format>
+Format for the document
+.INDENT 7.0
+.TP
+.B Options
+json|bibtex|yaml
+.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-a, \-\-all
 Export all without picking
 .UNINDENT
+.sp
+Arguments
 .INDENT 0.0
 .TP
-.B \-\-file
-Export a copy of a file
-.UNINDENT
-Arguments.INDENT 0.0
-.TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS Git
 .sp
 This command is useful if your library is itself a git repository.
 You can use this command to issue git commands in your library
@@ -3460,15 +3755,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis list \-\-file
+papis list \-\-all \-\-file
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -3476,15 +3771,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis list \-\-format \(aq{doc[year]} {doc[title]}\(aq
+papis list \-\-all \-\-format \(aq{doc[year]} {doc[title]}\(aq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -3493,60 +3788,39 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis list \-\-template bibitem.template
+papis list \-\-all \-\-template bibitem.template
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
-.SS Python examples
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-# Import the run function from the list command
-
-from papis.commands.list import run as papis_list
-
-documents = papis_list(query=\(aqeinstein\(aq, library=\(aqpapis\(aq)
-
-for doc in documents:
-    print(doc["url"])
-
-# etc...
-info_files = list(query=\(aqeinstein\(aq, library=\(aqpapis\(aq, info_files=True)
-
-# do something with the info file paths...
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
 .SS Cli
 .SS papis list
 .sp
 List documents\(aq properties
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis list [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-i, \-\-info
@@ -3560,38 +3834,45 @@
 .INDENT 0.0
 .TP
 .B \-d, \-\-dir
 Show the folder name associated with the document
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-format <format>
-List entries using a custom papis format, e.g. \(aq{doc[year] {doc[title]}
+.B \-n, \-\-notes
+List notes files, if any
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-template <template>
-Template file containing a papis format to list entries
+.B \-\-format <_format>
+List entries using a custom papis format, e.g. \(aq{doc[year] {doc[title]}
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-p, \-\-pick
-Pick the document instead of listing everything
+.B \-\-template <template>
+Template file containing a papis format to list entries
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-downloaders
 List available downloaders
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-libraries
 List defined libraries
 .UNINDENT
-Arguments.INDENT 0.0
+.INDENT 0.0
+.TP
+.B \-a, \-\-all
+Process all documents matching a query, if a query is given
+.UNINDENT
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS Mv
 .SS Cli
 .SS papis mv
@@ -3603,25 +3884,29 @@
 .nf
 .ft C
 papis mv [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-git, \-\-no\-git
 Add git interoperability
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS Open
 .sp
 The open command is a very important command in the papis workflow.
@@ -3733,21 +4018,28 @@
 .nf
 .ft C
 papis open [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-doc\-folder <doc_folder>
+Apply action to a document path
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-\-tool <tool>
 Tool for opening the file (opentool)
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-d, \-\-dir
 Open directory
@@ -3758,15 +4050,17 @@
 Open all matching documents
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-m, \-\-mark, \-\-no\-mark
 Open mark
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS Rename
 .SS Cli
 .SS papis rename
@@ -3778,60 +4072,78 @@
 .nf
 .ft C
 papis rename [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-git, \-\-no\-git
 Add git interoperability
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS Rm
 .SS Cli
 .SS papis rm
 .sp
-Delete command for several objects
+Delete a document or a file
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis rm [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
+.B \-\-git, \-\-no\-git
+Remove in git
+.UNINDENT
+.INDENT 0.0
+.TP
 .B \-\-file
 Remove files from a document instead of the whole folder
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-f, \-\-force
 Do not confirm removal
 .UNINDENT
-Arguments.INDENT 0.0
+.INDENT 0.0
+.TP
+.B \-\-all
+Remove all matches
+.UNINDENT
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SS Run
 .sp
 This command is useful to issue commands in the directory of your library.
@@ -3879,20 +4191,24 @@
 .nf
 .ft C
 papis run [OPTIONS] [RUN_COMMAND]...
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B RUN_COMMAND
 Optional argument(s)
 .UNINDENT
 .SS Update
 .sp
 This command is to update the information of the documents.
@@ -3905,15 +4221,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis update \-\-auto \-i "author = dyson"
+papis update \-\-auto \-i "author : dyson"
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -3925,15 +4241,15 @@
 .INDENT 2.0
 .INDENT 3.5
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis update \-\-from\-bibtex libraryfile.bib \-i
+papis update \-\-from bibtex libraryfile.bib \-i
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
@@ -3979,92 +4295,61 @@
 .nf
 .ft C
 papis update [OPTIONS] [QUERY]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-Options.INDENT 0.0
+.sp
+Options
+.INDENT 0.0
 .TP
 .B \-h, \-\-help
 Show this message and exit.
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-i, \-\-interactive, \-b, \-\-no\-interactive
-Interactively update
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-f, \-\-force
-Force update, overwrite conflicting information
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-crossref <from_crossref>
-Update info from crossref.org
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-isbn <from_isbn>
-Update info from isbn
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-isbnplus <from_isbnplus>
-Update info from isbnplus.org
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-base <from_base>
-Update info from Bielefeld Academic Search Engine
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-yaml <from_yaml>
-Update info from yaml file
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-bibtex <from_bibtex>
-Update info from bibtex file
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-from\-url <from_url>
-Get document or information from url
+.B \-\-git, \-\-no\-git
+Add git interoperability
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-\-from\-doi <from_doi>
-Doi to try to get information from
+.B \-\-doc\-folder <doc_folder>
+Apply action to a document path
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-auto
 Try to parse information from different sources
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-all
 Update all entries in library
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-s, \-\-set <set>
+.B \-\-from <from_importer>
+Add document from a specific importer (pdf2doi, yaml, crossref, folder, pmid, arxiv, lib, bibtex, doi, pdf2arxivid)
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-s, \-\-set <set_tuples>
 Update document\(aqs information with key value.The value can be a papis format.
 .UNINDENT
-Arguments.INDENT 0.0
+.sp
+Arguments
+.INDENT 0.0
 .TP
 .B QUERY
 Optional argument
 .UNINDENT
 .SH GUI
 .sp
-Papis is a program mainly intended for the command line, however
+Papis is a program mainly intended for the command line, however,
 some experimental frontends have been conceived for it and are
 already downloadable from pip.
 .sp
 See for instance
 .INDENT 0.0
 .IP \(bu 2
 \fI\%papis\-rofi\fP
@@ -4087,15 +4372,15 @@
 .sp
 .nf
 .ft C
 #! /usr/bin/env bash
 # papis\-short\-help: Email a paper to my friend
 
 folder_name=$1
-zip_name="${folder_name}\&.zip"
+zip_name="${folder_name}.zip"
 
 papis \-l ${PAPIS_LIB} export \-\-folder \-\-out ${folder_name}
 zip \-r ${zip_name} ${folder_name}
 
 mutt \-a ${zip_name}
 .ft P
 .fi
@@ -4115,15 +4400,15 @@
 papis \-h
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 and you will see that there is another command besides the default
-called \fBmail\fP\&. You will see in fact
+called \fBmail\fP\&. In fact, you will see
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 positional arguments:
   command               For further information for every command, type in \(aqpapis <command> \-h\(aq
@@ -4139,28 +4424,28 @@
 .UNINDENT
 .UNINDENT
 .sp
 where the description \fBEmail a paper to my friend\fP is there because
 we have defined the comment \fB# papis\-short\-help: Email a paper to my friend\fP
 in the header of the script.
 .sp
-Then if you type
+Then, if you type
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis \-l mylib mail this_paper
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 this will create a folder called \fBthis_paper\fP with a selection of a
-document, zip it, and send it to whoever you choose to.
+document, zip it and send it to whoever you choose to.
 .SS Example: Accessing papis from within mutt
 .sp
 You may want to pick documents to attach to your email in \fBmutt\fP
 from the papis interface.
 .sp
 Add this code to your \fBmuttrc\fP
 .INDENT 0.0
@@ -4240,14 +4525,31 @@
 .ft C
 >>> clear_lib_cache()
 .ft P
 .fi
 .UNINDENT
 .INDENT 0.0
 .TP
+.B papis.api.doi_to_data(doi)
+Try to get from a DOI expression a dictionary with the document\(aqs data
+using the crossref module.
+.INDENT 7.0
+.TP
+.B Parameters
+\fBdoi\fP (\fIstr\fP) \-\- DOI expression.
+.TP
+.B Returns
+Document\(aqs data
+.TP
+.B Return type
+dict
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
 .B papis.api.edit_file(file_path, wait=True)
 Edit file using the \fBeditor\fP key value as a program to
 handle file_path.
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
@@ -4274,15 +4576,15 @@
 list
 .UNINDENT
 .sp
 .nf
 .ft C
 >>> import tempfile
 >>> folder = tempfile.mkdtemp()
->>> set_lib(folder)
+>>> set_lib_from_name(folder)
 >>> docs = get_all_documents_in_lib(folder)
 >>> len(docs)
 0
 .ft P
 .fi
 .UNINDENT
 .INDENT 0.0
@@ -4336,39 +4638,39 @@
 .TP
 .B Return type
 list
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B papis.api.get_lib()
+.B papis.api.get_lib_name()
 Get current library, it either retrieves the library from
 the environment PAPIS_LIB variable or from the command line
 args passed by the user.
 .INDENT 7.0
 .TP
 .B Returns
 Library name
 .TP
 .B Return type
 str
 .UNINDENT
 .sp
 .nf
 .ft C
->>> get_lib() is not None
+>>> get_lib_name() is not None
 True
 .ft P
 .fi
 .UNINDENT
 .INDENT 0.0
 .TP
 .B papis.api.get_libraries()
 Get all libraries declared in the configuration. A library is discovered
-if the \fBdir\fP key defined in the library section.
+if the \fBdir\fP or \fBdirs\fP key defined in the library section.
 .INDENT 7.0
 .TP
 .B Returns
 List of library names
 .TP
 .B Return type
 list
@@ -4411,15 +4713,15 @@
 .IP \(bu 2
 \fBwait\fP (\fIbool\fP) \-\- Wait for the completion of the opener program to continue
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B papis.api.pick(options: list, pick_config={})
+.B papis.api.pick(options, pick_config={})
 This is a wrapper for the various pickers that are supported.
 Depending on the configuration different selectors or \(aqpickers\(aq
 are used.
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
@@ -4434,63 +4736,48 @@
 .TP
 .B Returns
 Returns elements of \fBoptions\fP\&.
 .TP
 .B Return type
 Element(s) of \fBoptions\fP
 .UNINDENT
-.sp
-.nf
-.ft C
->>> papis.config.set(\(aqpicktool\(aq, \(aqpapis.pick\(aq)
->>> pick([\(aqsomething\(aq])
-\(aqsomething\(aq
->>> papis.config.set(\(aqpicktool\(aq, \(aqnonexistent\(aq)
->>> pick([\(aqsomething\(aq])
-Traceback (most recent call last):
-\&...
-Exception: I don\(aqt know how to use the picker \(aqnonexistent\(aq
->>> papis.config.set(\(aqpicktool\(aq, \(aqpapis.pick\(aq)
-.ft P
-.fi
 .UNINDENT
 .INDENT 0.0
 .TP
-.B papis.api.pick_doc(documents: list)
+.B papis.api.pick_doc(documents)
 Pick a document from documents with the correct formatting
 .INDENT 7.0
 .TP
 .B Documents
 List of documents
 .TP
 .B Returns
 Document
 .UNINDENT
-.sp
-.nf
-.ft C
->>> from papis.document import from_data
->>> doc = from_data({\(aqtitle\(aq: \(aqHello World\(aq})
->>> pick_doc([doc]).dump()
-\(aqtitle:   Hello World\en\(aq
-.ft P
-.fi
 .UNINDENT
 .INDENT 0.0
 .TP
-.B papis.api.set_lib(library)
+.B papis.api.set_lib_from_name(library)
 Set current library, it either sets the library in
 the environment PAPIS_LIB variable or in the command line
 args passed by the user.
 .INDENT 7.0
 .TP
 .B Parameters
 \fBlibrary\fP (\fIstr\fP) \-\- Name of library or path to a given library
 .UNINDENT
 .UNINDENT
+.SH PLUGIN ARCHITECTURE
+.sp
+\fBNOTE:\fP
+.INDENT 0.0
+.INDENT 3.5
+TODO
+.UNINDENT
+.UNINDENT
 .SH GIT
 .sp
 Papis is conceived to work well with the tool \fIgit\fP, this would also work with
 \fI\%mercurial\fP
 or \fI\%subversion\fP\&.
 .sp
 Here you will find a description of a possible workflow using git with papis.
@@ -4536,15 +4823,15 @@
 .UNINDENT
 .UNINDENT
 .sp
 if you want to do it using the \fIpapis\fP\(aq \fBgit\fP command.
 .SS Interplay with other commands
 .sp
 Some papis commands give you the opportunity of using \fBgit\fP to manage
-changes. For instance if you are adding a new document, you could use
+changes. For instance, if you are adding a new document, you could use
 the \fB\-\-commit\fP flag to also add a commit into your library, so if you do
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis add \-\-set author "Pedrito" \-\-set title "Super book" book.pdf \-\-commit
@@ -4552,20 +4839,20 @@
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 then also papis will do an automatic commit for the book, so that you can
 push your library afterwards to a remote repository.
 .sp
-You can imagine that papis command like \fBrename\fP and \fBmv\fP should also
+You can imagine that papis commands like \fBrename\fP and \fBmv\fP should also
 offer such functionality, and they indeed do through the \fB\-\-git\fP flag.
 Go to their documentation for more information.
 .SS Updating the libray
 .sp
-You can use the papis\(aq simple \fBgit\fP wrapper,
+You can use papis\(aq simple \fBgit\fP wrapper,
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis git pull
 .ft P
@@ -4626,15 +4913,15 @@
 .UNINDENT
 .sp
 When editing a document\(aqs info file:
 .INDENT 0.0
 .INDENT 3.5
 .INDENT 0.0
 .IP \(bu 2
-Edit the file and then take a look at the \fBdiff\fP maybe
+Edit the file and then take a look at the \fBdiff\fP
 .INDENT 2.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis git diff
 .ft P
@@ -4644,15 +4931,15 @@
 .IP \(bu 2
 Add the changes
 .INDENT 2.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis git add \-a
+papis git add \-\-all
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
 Commit
 .INDENT 2.0
@@ -4678,16 +4965,16 @@
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
-Of course these workflows are just very basic examples, you can imagine
-that your workflow would look completely different.
+Of course these workflows are just very basic examples.
+Your optimal workflow could look completely different.
 .SH SCIHUB SUPPORT
 \fI\%\fP
 .sp
 Papis has a script that uses the scihub platform to download scientific
 papers. Due to legal caution the script is not included directly
 as a papis command, and it has its own PyPi repository.
 .sp
@@ -4724,27 +5011,29 @@
 .IP \(bu 2
 Download via the doi number:
 .INDENT 2.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis scihub 10\&.1002/andp.19053220607 add \-d einstein_papers \-\-name photon_definition
+papis scihub 10.1002/andp.19053220607 \e\e
+  add \-d einstein_papers \-\-folder\-name photon_definition
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
 Download via a url that contains the doi number in the format \fB\&.*/doi/<doinumber>\fP
 .INDENT 2.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-papis scihub http://physicstoday.scitation.org/doi/10.1063/1.881498 add \-\-name important_paper
+papis scihub http://physicstoday.scitation.org/doi/10.1063/1.881498 \e\e
+  add \-\-folder\-name important_paper
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .IP \(bu 2
 Download via the \fBdoi.org\fP url:
 .INDENT 2.0
@@ -4764,16 +5053,16 @@
 .sp
 Many users will want to import a library from a bibtex file
 that another program such as \fBzotero\fP, \fBmendeley\fP or
 \fBjabref\fP will have exported. These programs usually have a
 field called \fBFILE\fP or \fBfile\fP that points to a path
 where the document file can be found.
 .sp
-To import such a library you can use a script originally
-intended for \fBzotero\fP but that is general enought to work
+To import such a library you can use a provided script originally
+intended for \fBzotero\fP which is, however, general enough to work
 for other programs too.
 .sp
 To install this script you can copy the file \fBpapis\-zotero\fP in the
 repository\(aqs example directory to your papis \fBconfig/scripts\fP directory.
 .sp
 You can do this automatically issuing the following commands
 .INDENT 0.0
@@ -4811,15 +5100,15 @@
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 \fBWARNING:\fP
 .INDENT 0.0
 .INDENT 3.5
-Note that if your bibtex file has some pdf entries, i.e., looks like:
+Note that if your bibtex file has some pdf entries, i.e., it looks like:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 @article{Einstein1905Photon,
   author = { A. Einstein },
@@ -4833,26 +5122,26 @@
 }
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 then \fBpapis\-zotero\fP will interpret the path of the \fBFILE\fP entry
-as a relative path, so you should run the command where this relative path
+as a relative path, so you should run the command from where this relative path
 makes sense.
 .UNINDENT
 .UNINDENT
 .SH IMPORTING FROM ZOTERO SQLITE FILE
 .sp
 There is also a script that decodes the
 \fBzotero.sqlite\fP sqlite file that \fBzotero\fP uses to manage documents
 and creates papis Documents out of it.
 .sp
 This script will retrieve the documents from zotero (be it \fBpdf\fP documents
-or else) and important information like tags.
+or something else) and important information like tags.
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 wget \-O ~/.config/papis/scripts/papis\-zotero\-sql https://raw.githubusercontent.com/alejandrogallo/papis/master/examples/scripts/papis\-zotero\-sql
 chmod +x ~/.config/papis/scripts/papis\-zotero\-sql
@@ -4870,21 +5159,21 @@
 .ft C
 cd ~/.mozilla/firefox/zqb7ju1q.default/zotero
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-Maybe the path is slightly different, it may vary from version to version from
+Maybe the path is slightly different. It may vary from version to version from
 zotero.  In the zotero data directory there should be a file called
 \fBzotero.sqlite\fP and there might be a \fBstorage\fP directory with
 document data inside. These will be used by \fBzotero\-sql\fP to
 retrieve information and files from.
 .sp
-Now you can use the script as
+Now you can use the script through
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 papis zotero\-sql
 .ft P
@@ -4914,15 +5203,15 @@
 .ft C
 papis add \-\-from\-folder Documents/ZOTERO_ID
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-or write a \fBbash\fP for loop to do it with all the converted documents
+or write a \fBbash\fP for\-loop to do it with all the converted documents
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 for folder in Documents/* ; do papis add \-\-from\-folder $folder ; done
 .ft P
@@ -4935,17 +5224,17 @@
 .INDENT 3.5
 Please be aware that the database structure of zotero is version dependent
 and this script \fBmight\fP not work fully with your version.
 You can check \fI\%issue #18\fP
 for more information.
 .UNINDENT
 .UNINDENT
-.SH SHELL AUTOCOMPLETION
+.SH SHELL AUTO-COMPLETION
 .sp
-Papis has a bash autocompletion script that comes installed
+Papis has a bash auto\-completion script that comes installed
 when you install papis with \fBpip3\fP\&.
 .sp
 It should be installed in a relative path
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -4969,15 +5258,15 @@
 .UNINDENT
 .UNINDENT
 .sp
 or get the bash script from
 \fI\%here\fP\&.
 .SS Zsh
 .sp
-There is also a way for \fBzsh\fP users to autocomplete. Either downloading the
+There is also a way for \fBzsh\fP users to auto\-complete. Either downloading the
 script
 \fI\%here\fP\&.
 or adding the following line int the \fB\&.zshrc\fP configuration file
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -4985,19 +5274,19 @@
 eval "$(_PAPIS_COMPLETE=source_zsh papis)"
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SH FAQ
 .sp
-Here are some problems that users have come accross with often:
+Here are some problems that users have come across often:
 .INDENT 0.0
 .IP \(bu 2
-When I remove a folder manually in a library or I synchronize manually
-the library I do not see the new papers in the library.
+When I remove a folder manually in a library or I synchronize
+the library manually, I do not see the new papers in the library.
 \fBAnswer\fP: You probably need to update the cache because papis did not
 know anything about your changes in the library since you did it by yourself.
 .INDENT 2.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
```

### Comparing `papis-0.8.2/papis/commands/add.py` & `papis-0.9/papis/commands/add.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,58 +9,73 @@
 ^^^^^^^^
 
 - Add a document located in ``~/Documents/interesting.pdf`` and name the
   folder where it will be stored in the database ``interesting-paper-2021``
 
     .. code::
 
-        papis add ~/Documents/interesting.pdf --name interesting-paper-2021
+        papis add ~/Documents/interesting.pdf \\
+            --folder-name interesting-paper-2021
 
   if you want to add directly some key values, like ``author``, ``title``
   and ``tags``, you can also run the following:
 
     .. code::
 
         papis add ~/Documents/interesting.pdf \\
-            --name interesting-paper-2021 \\
+            --folder-name interesting-paper-2021 \\
             --set author 'John Smith' \\
             --set title 'The interesting life of bees' \\
             --set year 1985 \\
             --set tags 'biology interesting bees'
 
 - Add a paper that you have locally in a file and get the paper information
   through its ``doi`` identifier (in this case ``10.10763/1.3237134`` as an
   example):
 
     .. code::
 
-        papis add ~/Documents/interesting.pdf --from-doi 10.10763/1.3237134
+        papis add ~/Documents/interesting.pdf --from doi 10.10763/1.3237134
 
 - Add paper to a library named ``machine-learning`` from ``arxiv.org``
 
     .. code::
 
         papis -l machine-learning add \\
-            --from-url https://arxiv.org/abs/1712.03134
+            --from url https://arxiv.org/abs/1712.03134
 
 - If you do not want copy the original pdfs into the library, you can
   also tell papis to just create a link to them, for example
 
     .. code::
 
         papis add --link ~/Documents/interesting.pdf \\
-            --from-doi 10.10763/1.3237134
+            --from doi 10.10763/1.3237134
 
   will add an entry into the papis library, but the pdf document will remain
   at ``~/Documents/interesting.pdf``, and in the document's folder
   there will be a link to ``~/Documents/interesting.pdf`` instead of the
   file itself. Of course you always have to be sure that the
   document at ``~/Documents/interesting.pdf`` does not disappear, otherwise
   you will end up without a document to open.
 
+- Papis also tries to make sense of the inputs that you have passed
+  to the command, for instance you could provide only a ``doi`` and
+  papis will try to know if this is indeed a ``doi``
+
+    .. code::
+
+        papis add 10.1103/PhysRevLett.123.156401
+
+  or from a ``url``
+
+    .. code::
+
+        papis add https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.123.156401
+
 
 Examples in python
 ^^^^^^^^^^^^^^^^^^
 
 There is a python function in the add module that can be used to interact
 in a more effective way in python scripts,
 
@@ -69,37 +84,78 @@
 Cli
 ^^^
 .. click:: papis.commands.add:cli
     :prog: papis add
 
 """
 import logging
-import papis
 from string import ascii_lowercase
 import os
 import re
 import tempfile
 import hashlib
 import shutil
-import subprocess
 import papis.api
-from papis.api import status
+import papis.pick
 import papis.utils
 import papis.config
-import papis.bibtex
 import papis.document
-import papis.downloaders.utils
+import papis.importer
 import papis.cli
 import click
-import builtins
 import colorama
+import papis.downloaders
+import papis.git
 
 logger = logging.getLogger('add')
 
 
+class FromFolderImporter(papis.importer.Importer):
+
+    """Importer that gets files and data from a valid papis folder"""
+
+    def __init__(self, **kwargs):
+        papis.importer.Importer.__init__(self, name='folder', **kwargs)
+
+    @classmethod
+    def match(cls, uri):
+        return FromFolderImporter(uri=uri) if os.path.isdir(uri) else None
+
+    def fetch(self):
+        doc = papis.document.from_folder(self.uri)
+        self.logger.info('importing from folder {0}'.format(self.uri))
+        self.ctx.data = papis.document.to_dict(doc)
+        self.ctx.files = doc.get_files()
+
+
+class FromLibImporter(papis.importer.Importer):
+
+    """Importer that queries a valid papis library (also paths) and adds files
+    and data
+    """
+
+    def __init__(self, **kwargs):
+        papis.importer.Importer.__init__(self, name='lib', **kwargs)
+
+    @classmethod
+    def match(cls, uri):
+        try:
+            papis.config.get_lib_from_name(uri)
+        except Exception:
+            return None
+        else:
+            return FromLibImporter(uri=uri)
+
+    def fetch(self):
+        doc = papis.pick.pick_doc(papis.api.get_all_documents_in_lib(self.uri))
+        importer = FromFolderImporter(uri=doc.get_main_folder())
+        importer.fetch()
+        self.ctx = importer.ctx
+
+
 def get_file_name(data, original_filepath, suffix=""):
     """Generates file name for the document
 
     :param data: Data parsed for the actual document
     :type  data: dict
     :param original_filepath: The full path to the original file
     :type  original_filepath: str
@@ -108,43 +164,49 @@
     :type  suffix: str
     :returns: New file name
     :rtype:  str
 
     """
 
     basename_limit = 150
-    file_name_opt = papis.config.get('file-name')
+    file_name_opt = papis.config.get('add-file-name')
+    ext = papis.utils.get_document_extension(original_filepath)
 
     if file_name_opt is None:
         file_name_opt = os.path.basename(original_filepath)
 
+    # Get a file name from the format `add-file-name`
     file_name_base = papis.utils.format_doc(
         file_name_opt,
         papis.document.from_data(data)
     )
 
     if len(file_name_base) > basename_limit:
         logger.warning(
-            'Shortening the documents\' {} name for portability'.format(
-                original_filepath
-            )
+            "Shortening the name {0} for portability".format(file_name_base)
         )
         file_name_base = file_name_base[0:basename_limit]
 
+    # Remove extension from file_name_base, if any
+    file_name_base = re.sub(
+        r"([.]{0})?$".format(ext),
+        '',
+        file_name_base
+    )
+
+    # Adding some extra suffixes, if any, and cleaning up document name
     filename_basename = papis.utils.clean_document_name(
         "{}{}".format(
             file_name_base,
             "-" + suffix if len(suffix) > 0 else ""
         )
     )
 
-    filename = "{}.{}".format(
-        filename_basename,
-        papis.utils.get_document_extension(original_filepath)
-    )
+    # Adding the recognised extension
+    filename = filename_basename + '.' + ext
 
     return filename
 
 
 def get_hash_folder(data, document_paths):
     """Folder name where the document will be stored.
 
@@ -170,94 +232,50 @@
 
     result = md5 + author
     result = papis.utils.clean_document_name(result)
 
     return result
 
 
-def get_default_title(data, document_path, interactive=False):
-    """
-    >>> get_default_title({'title': 'hello world'}, 'whatever.pdf')
-    'hello world'
-    >>> open('Luces-de-bohemia.pdf', 'w+').close()
-    >>> get_default_title(dict(), 'Luces-de-bohemia.pdf')
-    'Luces de bohemia'
-    """
-    if "title" in data.keys():
-        return data["title"]
-    extension = papis.utils.get_document_extension(document_path)
-    title = (os.path.basename(document_path)
-        .replace("."+extension, "")
-        .replace("_", " ")
-        .replace("-", " ")
-    )
-    if interactive:
-        title = papis.utils.input(
-            'Title?', title
-        )
-    return title
-
-
-def get_default_author(data, document_path, interactive=False):
-    """
-    >>> get_default_author({'author': 'Garcilaso de la vega'}, 'whatever.pdf')
-    'Garcilaso de la vega'
-    >>> get_default_author(dict(), 'Luces-de-bohemia.pdf')
-    'Unknown'
-    """
-    if "author" in data.keys():
-        return data["author"]
-    author = "Unknown"
-    if interactive:
-        author = papis.utils.input(
-            'Author?', author
-        )
-    return author
-
-
 def run(
         paths,
         data=dict(),
-        name=None,
+        folder_name=None,
         file_name=None,
         subfolder=None,
-        interactive=False,
         confirm=False,
         open_file=False,
         edit=False,
-        commit=False,
+        git=False,
         link=False
         ):
     """
     :param paths: Paths to the documents to be added
     :type  paths: []
     :param data: Data for the document to be added.
         If more data is to be retrieved from other sources, the data dictionary
         will be updated from these sources.
     :type  data: dict
-    :param name: Name of the folder where the document will be stored
-    :type  name: str
+    :param folder_name: Name of the folder where the document will be stored
+    :type  folder_name: str
     :param file_name: File name of the document's files to be stored.
     :type  file_name: str
     :param subfolder: Folder within the library where the document's folder
         should be stored.
     :type  subfolder: str
-    :param interactive: Wether or not interactive functionality of this command
-        should be activated.
-    :type  interactive: bool
     :param confirm: Wether or not to ask user for confirmation before adding.
     :type  confirm: bool
     :param open_file: Wether or not to ask user for opening file before adding.
     :type  open_file: bool
     :param edit: Wether or not to ask user for editing the infor file
         before adding.
     :type  edit: bool
-    :param commit: Wether or not to ask user for committing before adding,
+    :param git: Wether or not to ask user for committing before adding,
         in the case of course that the library is a git repository.
-    :type  commit: bool
+    :type  git: bool
     """
 
     logger = logging.getLogger('add:run')
     # The folder name of the new document that will be created
     out_folder_name = None
     # The real paths of the documents to be added
     in_documents_paths = paths
@@ -273,401 +291,264 @@
     in_documents_names = [
         papis.utils.clean_document_name(doc_path)
         for doc_path in in_documents_paths
     ]
 
     tmp_document = papis.document.Document(temp_dir)
 
-    if not name:
-        logger.info("Getting an automatic name")
+    if not folder_name:
         out_folder_name = get_hash_folder(data, in_documents_paths)
+        logger.info("Got an automatic folder name")
     else:
         temp_doc = papis.document.Document(data=data)
-        out_folder_name = papis.utils.format_doc(name, temp_doc)
+        out_folder_name = papis.utils.format_doc(folder_name, temp_doc)
         out_folder_name = papis.utils.clean_document_name(out_folder_name)
         del temp_doc
 
     data["files"] = in_documents_names
-    out_folder_path = os.path.expanduser(os.path.join(
-        papis.config.get('dir'), subfolder or '',  out_folder_name
-    ))
+    out_folder_path = os.path.expanduser(
+        os.path.join(
+            papis.config.get_lib_dirs()[0],
+            subfolder or '',
+            out_folder_name))
 
-    logger.info("The document will be saved in {0}".format(out_folder_name))
+    logger.info("The folder name is {0}".format(out_folder_name))
     logger.debug("Folder path: {0}".format(out_folder_path))
     logger.debug("File(s): {0}".format(in_documents_paths))
 
     # First prepare everything in the temporary directory
     g = papis.utils.create_identifier(ascii_lowercase)
     string_append = ''
     if file_name is not None:  # Use args if set
-        papis.config.set("file-name", file_name)
+        papis.config.set("add-file-name", file_name)
     new_file_list = []
 
     for in_file_path in in_documents_paths:
 
         # Rename the file in the staging area
         new_filename = papis.utils.clean_document_name(
             get_file_name(
                 data,
                 in_file_path,
-                suffix=string_append
-            )
-        )
+                suffix=string_append))
         new_file_list.append(new_filename)
 
         tmp_end_filepath = os.path.join(
             tmp_document.get_main_folder(),
-            new_filename
-        )
+            new_filename)
         string_append = next(g)
 
         if link:
             in_file_abspath = os.path.abspath(in_file_path)
             logger.debug(
                 "[SYMLINK] '%s' to '%s'" %
-                (in_file_abspath, tmp_end_filepath)
-            )
+                (in_file_abspath, tmp_end_filepath))
             os.symlink(in_file_abspath, tmp_end_filepath)
         else:
             logger.debug(
                 "[CP] '%s' to '%s'" %
-                (in_file_path, tmp_end_filepath)
-            )
+                (in_file_path, tmp_end_filepath))
             shutil.copy(in_file_path, tmp_end_filepath)
 
     data['files'] = new_file_list
-    tmp_document.update(data, force=True)
+    tmp_document.update(data)
     tmp_document.save()
 
     # Check if the user wants to edit before submitting the doc
     # to the library
     if edit:
         logger.info("Editing file before adding it")
         papis.api.edit_file(tmp_document.get_info_file(), wait=True)
         logger.info("Loading the changes made by editing")
         tmp_document.load()
-        data = papis.document.to_dict(tmp_document)
 
     # Duplication checking
     logger.info("Checking if this document is already in the library")
     try:
         found_document = papis.utils.locate_document_in_lib(tmp_document)
     except IndexError:
-        logger.info("I did not found anything matching")
+        logger.info("No document matching found already in the library")
     else:
         logger.warning(
             colorama.Fore.RED +
             "DUPLICATION WARNING" +
-            colorama.Style.RESET_ALL
-        )
+            colorama.Style.RESET_ALL)
         logger.warning(
-            "The document beneath is in your library and it seems to match"
-        )
+            "The document beneath is in your library and it seems to match")
         logger.warning(
             "the one that you're trying to add, "
-            "I will prompt you for confirmation"
-        )
+            "I will prompt you for confirmation")
         logger.warning(
             "(Hint) Use the update command if you just want to update"
-            " the info."
-        )
+            " the info.")
         papis.utils.text_area(
             'The following document is already in your library',
             papis.document.dump(found_document),
             lexer_name='yaml',
-            height=20
-        )
+            height=20)
         confirm = True
 
     if open_file:
         for d_path in tmp_document.get_files():
-            papis.api.open_file(d_path)
+            papis.utils.open_file(d_path)
     if confirm:
         if not papis.utils.confirm('Really add?'):
-            return status.success
+            return
 
     logger.info(
         "[MV] '%s' to '%s'" %
         (tmp_document.get_main_folder(), out_folder_path)
     )
     # This also sets the folder of tmp_document
     papis.document.move(tmp_document, out_folder_path)
     papis.database.get().add(tmp_document)
-    if commit:
-        subprocess.call(["git", "-C", out_folder_path, "add", "."])
-        subprocess.call(
-            ["git", "-C", out_folder_path, "commit", "-m", "Add document"]
-        )
-    return status.success
+    if git:
+        papis.git.add_and_commit_resource(
+            tmp_document.get_main_folder(), '.',
+            "Add document '{0}'".format(papis.document.describe(tmp_document)))
 
 
 @click.command(
     "add",
     help="Add a document into a given library"
 )
 @click.help_option('--help', '-h')
-@click.argument("files", type=click.Path(exists=True), nargs=-1)
+@click.argument("files", type=str, nargs=-1)
 @click.option(
     "-s", "--set", "set_list",
     help="Set some information before",
     multiple=True,
-    type=(str, str)
-)
+    type=(str, str))
 @click.option(
-    "-d", "--dir", "directory",
+    "-d", "--subfolder",
     help="Subfolder in the library",
-    default=""
-)
+    default="")
 @click.option(
-    "-i", "--interactive/--no-interactive",
-    help="Do some of the actions interactively",
-    default=lambda: True if papis.config.get('add-interactive') else False
-)
-@click.option(
-    "--name",
+    "--folder-name",
     help="Name for the document's folder (papis format)",
-    default=lambda: papis.config.get('add-name')
-)
+    default=lambda: papis.config.get('add-folder-name'))
 @click.option(
     "--file-name",
     help="File name for the document (papis format)",
-    default=None
-)
-@click.option(
-    "--from-bibtex",
-    help="Parse information from a bibtex file",
-    default=""
-)
-@click.option(
-    "--from-yaml",
-    help="Parse information from a yaml file",
-    default=""
-)
-@click.option(
-    "--from-folder",
-    help="Add document from folder being a valid papis document"
-         " (containing info.yaml)",
-    default=""
-)
-@click.option(
-    "--from-url",
-    help="Get document and information from a"
-    "given url, a parser must be implemented",
-    default=""
-)
+    default=None)
 @click.option(
-    "--from-doi",
-    help="Doi to try to get information from",
-    default=None
-)
-@click.option(
-    "--from-pmid",
-    help="PMID to try to get information from",
-    default=None
-)
+    "--from", "from_importer",
+    help="Add document from a specific importer ({0})".format(
+        ", ".join(papis.importer.available_importers())
+    ),
+    type=(click.Choice(papis.importer.available_importers()), str),
+    nargs=2,
+    multiple=True,
+    default=(),)
 @click.option(
-    "--from-lib",
-    help="Add document from another library",
-    default=""
-)
+    "-b", "--batch",
+    help="Batch mode, do not prompt or otherwise",
+    default=False, is_flag=True)
 @click.option(
     "--confirm/--no-confirm",
     help="Ask to confirm before adding to the collection",
-    default=lambda: True if papis.config.get('add-confirm') else False
-)
+    default=lambda: True if papis.config.get('add-confirm') else False)
 @click.option(
     "--open/--no-open", "open_file",
     help="Open file before adding document",
-    default=lambda: True if papis.config.get('add-open') else False
-)
+    default=lambda: True if papis.config.get('add-open') else False)
 @click.option(
     "--edit/--no-edit",
     help="Edit info file before adding document",
-    default=lambda: True if papis.config.get('add-edit') else False
-)
-@click.option(
-    "--commit/--no-commit",
-    help="Commit document if library is a git repository",
-    default=False
-)
+    default=lambda: True if papis.config.get('add-edit') else False)
 @click.option(
     "--link/--no-link",
     help="Instead of copying the file to the library, create a link to"
          "its original location",
-    default=False
-)
+    default=False)
+@papis.cli.git_option(help="Git add and commit the new document")
 @click.option(
-    #TODO: REMOVE IT AT SOME POINT
-    "--no-document",
+    "--list-importers", "--li", "list_importers",
+    help="List all available papis importers",
     default=False,
-    is_flag=True,
-    help="DEPRECATION NOTICE: This option is no longer valid, "
-         "it will be removed in future releases"
-)
-def cli(
-        files,
-        set_list,
-        directory,
-        interactive,
-        name,
-        file_name,
-        from_bibtex,
-        from_yaml,
-        from_folder,
-        from_url,
-        from_doi,
-        from_pmid,
-        from_lib,
-        confirm,
-        open_file,
-        edit,
-        commit,
-        link,
-        no_document
-        ):
-    """
-    :param from_folder: Filepath where to find a papis document (folder +
-        info file) to be added to the library.
-    :type  from_folder: str
-    :param from_doi: doi number to try to download information from.
-    :type  from_doi: str
-    :param from_pmid: pmid number to try to download information from.
-    :type  from_pmid: str
-    :param from_url: Url to try to download information and files from.
-    :type  from_url: str
-    :param from_bibtex: Filepath where to find a file containing bibtex info.
-    :type  from_bibtex: str
-    :param from_yaml: Filepath where to find a file containing yaml info.
-    :type  from_yaml: str
-    """
-    data = dict()
-    files = list(files)
-
-    for data_set in set_list:
-        data[data_set[0]] = data_set[1]
+    is_flag=True)
+def cli(files, set_list, subfolder, folder_name, file_name, from_importer,
+        batch, confirm, open_file, edit, git, link, list_importers):
+
+    if list_importers:
+        import_mgr = papis.importer.get_import_mgr()
+        for n in import_mgr.names():
+            print("{name}\n\t{text}".format(
+                name=n,
+                text=re.sub(r"[ \n]+", " ", import_mgr[n].plugin.__doc__)))
+        return
 
+    from_importer = list(from_importer)
     logger = logging.getLogger('cli:add')
 
-    if from_lib:
-        doc = papis.api.pick_doc(
-            papis.api.get_all_documents_in_lib(from_lib)
-        )
-        if doc:
-            from_folder = doc.get_main_folder()
-
-    try:
-        # Try getting title if title is an argument of add
-        data["title"] = data.get('title') or get_default_title(
-            data,
-            files[0],
-            interactive
-        )
-        logger.info("Title = % s" % data["title"])
-    except:
-        pass
-
-    try:
-        # Try getting author if author is an argument of add
-        data["author"] = data.get('author') or get_default_author(
-            data,
-            files[0],
-            interactive
-        )
-        logger.info("Author = % s" % data["author"])
-    except:
-        pass
-
-    if from_folder:
-        original_document = papis.document.Document(from_folder)
-        from_yaml = original_document.get_info_file()
-        files.extend(original_document.get_files())
-
-    if from_url:
-        logger.info("Attempting to retrieve from url")
-        url_data = papis.downloaders.utils.get(from_url)
-        data.update(url_data["data"])
-        files.extend(url_data["documents_paths"])
-        # If no data was retrieved and doi was found, try to get
-        # information with the document's doi
-        if not data and url_data["doi"] is not None and not from_doi:
-            logger.warning(
-                "I could not get any data from {0}".format(from_url)
-            )
-            from_doi = url_data["doi"]
-            logger.info(
-                "But I found a doi ({0}), I'll try my luck there".format(
-                    from_doi
-                )
-            )
-
-    if from_pmid:
-        logger.info("Using PMID %s via HubMed" % from_pmid)
-        hubmed_url = "http://pubmed.macropus.org/articles/"\
-                     "?format=text%%2Fbibtex&id=%s" % from_pmid
-        bibtex_data = papis.downloaders.utils.get_downloader(
-            hubmed_url,
-            "get"
-        ).get_document_data().decode("utf-8")
-        bibtex_data = papis.bibtex.bibtex_to_dict(bibtex_data)
-        if len(bibtex_data):
-            data.update(bibtex_data[0])
-            if "doi" in data and not from_doi:
-                from_doi = data["doi"]
-        else:
-            logger.error("PMID %s not found or invalid" % from_pmid)
-
-    if from_doi:
-        logger.info("using doi {0}".format(from_doi))
-        data.update(papis.utils.doi_to_data(from_doi))
-        if len(files) == 0 and \
-                papis.config.get('doc-url-key-name') in data.keys():
-
-            doc_url = data[papis.config.get('doc-url-key-name')]
-            logger.info(
-                'You did not provide any files, but I found a possible '
-                'url where the file might be'
-            )
-            logger.info(
-                'I am trying to download the document from %s' % doc_url
-            )
-            down = papis.downloaders.utils.get_downloader(doc_url, 'get')
-            assert(down is not None)
-            tmp_filepath = tempfile.mktemp()
-            logger.debug("Saving in %s" % tmp_filepath)
-
-            with builtins.open(tmp_filepath, 'wb+') as fd:
-                fd.write(down.get_document_data())
-
-            logger.info('Opening the file')
-            papis.api.open_file(tmp_filepath)
-            if papis.utils.confirm('Do you want to use this file?'):
-                files.append(tmp_filepath)
-
-    if from_yaml:
-        logger.info("Reading yaml input file = %s" % from_yaml)
-        data.update(papis.utils.yaml_to_data(from_yaml))
-
-    if from_bibtex:
-        logger.info("Reading bibtex input file = %s" % from_bibtex)
-        bib_data = papis.bibtex.bibtex_to_dict(from_bibtex)
-        if len(bib_data) > 1:
-            logger.warning(
-                'Your bibtex file contains more than one entry,'
-                ' I will be taking the first entry'
-            )
-        data.update(bib_data[0])
+    data = dict()
+    for data_set in set_list:
+        data[data_set[0]] = data_set[1]
 
-    assert(isinstance(data, dict))
+    files = list(files)
+    ctx = papis.importer.Context()
+    ctx.files = [f for f in files if os.path.exists(f)]
+    ctx.data.update(data)
+
+    if batch:
+        edit = False
+        confirm = False
+        open_file = False
+
+    import_mgr = papis.importer.get_import_mgr()
+    matching_importers = []
+
+    if not from_importer and not batch and files:
+        matching_importers = sum((
+            papis.utils.get_matching_importer_or_downloader(f)
+            for f in files), [])
+
+    for importer_tuple in from_importer:
+        try:
+            importer_name = importer_tuple[0]
+            resource = importer_tuple[1]
+            importer = import_mgr[importer_name].plugin(uri=resource)
+            importer.fetch()
+            if importer.ctx:
+                matching_importers.append(importer)
+        except Exception as e:
+            logger.exception(e)
+
+    if matching_importers:
+        logger.info(
+            'There are {0} possible matchings'.format(len(matching_importers)))
+
+        for importer in matching_importers:
+            if importer.ctx.data:
+                logger.info(
+                    'Merging data from importer {0}'.format(importer.name))
+                if batch:
+                    ctx.data.update(importer.ctx.data)
+                else:
+                    papis.utils.update_doc_from_data_interactively(
+                        ctx.data,
+                        importer.ctx.data,
+                        str(importer))
+            if importer.ctx.files:
+                logger.info(
+                    'Got files {0} from importer {1}'
+                    .format(importer.ctx.files, importer.name))
+                for f in importer.ctx.files:
+                    papis.utils.open_file(f)
+                    if batch or papis.utils.confirm("Use this file?"):
+                        ctx.files.append(f)
+
+    if not ctx:
+        logger.error('there is nothing to be added')
+        return
 
     return run(
-        list(files),
-        data=data,
-        name=name,
+        ctx.files,
+        data=ctx.data,
+        folder_name=folder_name,
         file_name=file_name,
-        subfolder=directory,
-        interactive=interactive,
+        subfolder=subfolder,
         confirm=confirm,
         open_file=open_file,
         edit=edit,
-        commit=commit,
-        link=link
-    )
+        git=git,
+        link=link)
```

### Comparing `papis-0.8.2/papis/commands/addto.py` & `papis-0.9/papis/commands/addto.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 ^^^
 .. click:: papis.commands.addto:cli
     :prog: papis addto
 """
 from string import ascii_lowercase
 import os
 import shutil
-import papis.api
-from papis.api import status
+import papis.pick
 import papis.utils
 import papis.document
+import papis.git
 import papis.config
 import papis.commands.add
 import logging
 import papis.cli
 import click
+import papis.strings
 
 
-def run(document, filepaths):
+def run(document, filepaths, git=False):
     logger = logging.getLogger('addto')
     g = papis.utils.create_identifier(ascii_lowercase)
     string_append = ''
     for i in range(len(document.get_files())):
         string_append = next(g)
 
     new_file_list = []
@@ -68,43 +69,54 @@
             )
 
         if os.path.exists(endDocumentPath):
             logger.warning(
                 "%s already exists, ignoring..." % endDocumentPath
             )
             continue
-        logger.debug(
+        logger.info(
             "[CP] '%s' to '%s'" %
             (in_file_path, endDocumentPath)
         )
         shutil.copy(in_file_path, endDocumentPath)
 
+    if not "files" in document.keys():
+        document["files"] = []
     document['files'] += new_file_list
     document.save()
-    return status.success
+    papis.database.get().update(document)
+    if git:
+        for r in new_file_list + [document.get_info_file()]:
+            papis.git.add(document.get_main_folder(), r)
+        papis.git.commit(
+            document.get_main_folder(),
+            "Add new files to '{}'".format(papis.document.describe(document)))
 
 
 @click.command("addto")
 @click.help_option('--help', '-h')
 @papis.cli.query_option()
+@papis.cli.git_option(help="Add and commit files")
 @click.option(
     "-f", "--files",
     help="File fullpaths to documents",
     multiple=True,
-    type=click.Path(exists=True)
-)
+    type=click.Path(exists=True))
 @click.option(
     "--file-name",
     help="File name for the document (papis format)",
-    default=None
-)
-def cli(query, files, file_name):
+    default=None)
+def cli(query, git, files, file_name):
     """Add files to an existing document"""
     documents = papis.database.get().query(query)
-    document = papis.api.pick_doc(documents)
+    logger = logging.getLogger('cli:addto')
+    if not documents:
+        logger.warning(papis.strings.no_documents_retrieved_message)
+        return
+    document = papis.pick.pick_doc(documents)
     if not document:
-        return status.file_not_found
+        return
 
     if file_name is not None:  # Use args if set
-        papis.config.set("file-name", file_name)
+        papis.config.set("add-file-name", file_name)
 
-    return run(document, files)
+    return run(document, files, git=git)
```

### Comparing `papis-0.8.2/papis/commands/config.py` & `papis-0.9/papis/commands/config.py`

 * *Files identical despite different names*

### Comparing `papis-0.8.2/papis/commands/default.py` & `papis-0.9/papis/commands/default.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,26 +23,87 @@
 ^^^
 .. click:: papis.commands.default:run
     :prog: papis
     :commands: []
 
 """
 import os
+import difflib
+import sys
 import papis
 import papis.api
 import papis.config
 import papis.commands
+import papis.database
 import colorama
 import logging
 import click
 import papis.cli
 
 
+class MultiCommand(click.MultiCommand):
+
+    scripts = papis.commands.get_scripts()
+    scripts.update(papis.commands.get_external_scripts())
+    logger = logging.getLogger('multicommand')
+
+    def list_commands(self, ctx):
+        """List all matched commands in the command folder and in path
+
+        >>> mc = MultiCommand()
+        >>> rv = mc.list_commands(None)
+        >>> len(rv) > 0
+        True
+        """
+        rv = [s for s in self.scripts.keys()]
+        rv.sort()
+        return rv
+
+    def get_command(self, ctx, name):
+        """Get the command to be run
+
+        >>> mc = MultiCommand()
+        >>> cmd = mc.get_command(None, 'add')
+        >>> cmd.name, cmd.help
+        ('add', 'Add...')
+        >>> mc.get_command(None, 'this command does not exist')
+        """
+        try:
+            script = self.scripts[name]
+        except KeyError:
+            matches = difflib.get_close_matches(name, self.scripts, n=2)
+            self.logger.error(
+                '{c.Fore.RED}{c.Style.BRIGHT}{c.Back.BLACK}'
+                'did you mean {0}?'
+                '{c.Style.RESET_ALL}'
+                .format(
+                    ' or '.join(matches),
+                    c=colorama
+                ))
+            # return the match if there was only one match
+            if len(matches) == 1:
+                self.logger.warning("I suppose you meant {0}".format(*matches))
+                script = self.scripts[matches[0]]
+            else:
+                return None
+
+        if script['plugin']:
+            return script['plugin']
+        # If it gets here, it means that it is an external script
+        from papis.commands.external import external_cli as cli
+        from papis.commands.external import get_command_help
+        cli.context_settings['obj'] = script
+        cli.help = get_command_help(script['path'])
+        cli.name = script["command_name"]
+        cli.short_help = cli.help
+        return cli
+
+
 @click.group(
-    cls=papis.cli.MultiCommand,
+    cls=MultiCommand,
     invoke_without_command=True
 )
 @click.help_option('--help', '-h')
 @click.version_option(version=papis.__version__)
 @click.option(
     "-v",
     "--verbose",
@@ -56,14 +117,15 @@
     help="Choose a library name or library path (unamed library)",
     default=lambda: papis.config.get("default-library")
 )
 @click.option(
     "-c",
     "--config",
     help="Configuration file to use",
+    type=click.Path(exists=True),
     default=None,
 )
 @click.option(
     "--log",
     help="Logging level",
     type=click.Choice(["INFO", "DEBUG", "WARNING", "ERROR", "CRITICAL"]),
     default="INFO"
@@ -84,31 +146,31 @@
     "-s", "--set", "set_list",
     type=(str, str),
     multiple=True,
     help="Set key value, e.g., "
          "--set info-name information.yaml  --set opentool evince",
 )
 @click.option(
-    "--nc", "--no-color", "no_color",
-    default=False,
-    is_flag=True,
+    "--color",
+    type=click.Choice(["always", "auto", "no"]),
+    default="auto",
     help="Prevent the output from having color"
 )
 def run(
         verbose,
         config,
         lib,
         log,
         pick_lib,
         clear_cache,
         set_list,
-        no_color
+        color
         ):
 
-    if no_color:
+    if color == "no" or (color == "auto" and not sys.stdout.isatty()):
         # Turn off colorama (strip escape sequences from the output)
         colorama.init(strip=True)
     else:
         colorama.init()
 
     log_format = (
         colorama.Fore.YELLOW +
@@ -134,30 +196,29 @@
         papis.config.set(pair[0], pair[1])
 
     if config:
         papis.config.set_config_file(config)
         papis.config.reset_configuration()
 
     if pick_lib:
-        lib = papis.api.pick(
-            papis.api.get_libraries(),
-            pick_config=dict(header_filter=lambda x: x)
-        )
+        lib = papis.pick.pick(papis.api.get_libraries())
 
-    papis.config.set_lib(lib)
+    papis.config.set_lib_from_name(lib)
+    library = papis.config.get_lib()
 
-    # Now the library should be set, let us check if there is a
-    # local configuration file there, and if there is one, then
-    # merge its contents
-    local_config_file = os.path.expanduser(
-        os.path.join(
-            papis.config.get("dir"),
-            papis.config.get("local-config-file")
+    for path in library.paths:
+        # Now the library should be set, let us check if there is a
+        # local configuration file there, and if there is one, then
+        # merge its contents
+        local_config_file = os.path.expanduser(
+            os.path.join(
+                path,
+                papis.config.get("local-config-file")
+            )
+        )
+        papis.config.merge_configuration_from_path(
+            local_config_file,
+            papis.config.get_configuration()
         )
-    )
-    papis.config.merge_configuration_from_path(
-        local_config_file,
-        papis.config.get_configuration()
-    )
 
     if clear_cache:
-        papis.api.clear_lib_cache(lib)
+        papis.database.get().clear()
```

### Comparing `papis-0.8.2/papis/commands/edit.py` & `papis-0.9/papis/commands/edit.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,70 +6,79 @@
 ^^^
 .. click:: papis.commands.edit:cli
     :prog: papis edit
 """
 import papis
 import os
 import papis.api
+import papis.pick
 import papis.utils
 import papis.config
 import papis.database
 import papis.cli
 import click
 import logging
+import papis.strings
+import papis.git
 
 
-def run(document, wait=True):
+def run(document, wait=True, git=False):
     database = papis.database.get()
     papis.utils.general_open(document.get_info_file(), "editor", wait=wait)
     document.load()
     database.update(document)
+    if git:
+        papis.git.add_and_commit_resource(
+            document.get_main_folder(),
+            document.get_info_file(),
+            "Update information for '{0}'".format(
+                papis.document.describe(document)))
 
 
 @click.command("edit")
 @click.help_option('-h', '--help')
 @papis.cli.query_option()
+@papis.cli.git_option(help="Add changes made to the info file")
 @click.option(
     "-n",
     "--notes",
     help="Edit notes associated to the document",
     default=False,
-    is_flag=True
-)
+    is_flag=True)
 @click.option(
     "--all",
     help="Edit all matching documents",
     default=False,
-    is_flag=True
-)
+    is_flag=True)
 @click.option(
     "-e",
     "--editor",
     help="Editor to be used",
-    default=None
-)
+    default=None)
 def cli(
         query,
+        git,
         notes,
         all,
         editor
         ):
     """Edit document information from a given library"""
 
     logger = logging.getLogger('cli:edit')
     documents = papis.database.get().query(query)
 
     if editor is not None:
         papis.config.set('editor', editor)
 
     if not all:
-        document = papis.api.pick_doc(documents)
+        document = papis.pick.pick_doc(documents)
         documents = [document] if document else []
 
     if len(documents) == 0:
+        logger.warning(papis.strings.no_documents_retrieved_message)
         return 0
 
     for document in documents:
         if notes:
             logger.debug("Editing notes")
             if not document.has("notes"):
                 logger.warning(
@@ -80,13 +89,21 @@
                 document.save()
             notesPath = os.path.join(
                 document.get_main_folder(),
                 document["notes"]
             )
 
             if not os.path.exists(notesPath):
-                logger.debug("Creating %s" % notesPath)
+                logger.info("Creating {0}".format(notesPath))
                 open(notesPath, "w+").close()
 
             papis.api.edit_file(notesPath)
+            if git:
+                papis.git.add_and_commit_resource(
+                    document.get_main_folder(),
+                    document.get_info_file(),
+                    "Update notes for '{0}'".format(
+                        papis.document.describe(document)))
+
+
         else:
-            run(document)
+            run(document, git=git)
```

### Comparing `papis-0.8.2/papis/commands/export.py` & `papis-0.9/papis/commands/list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,249 +1,210 @@
 """
-The export command is useful to work with other programs such as bibtex.
+This command is to list contents of a library.
 
-Some examples of its usage are:
+CLI Examples
+^^^^^^^^^^^^
 
-- Export one of the documents matching the author with einstein to bibtex:
+- List all document files associated will all entries:
 
-.. code::
+    .. code:: bash
 
-    papis export --bibtex 'author = einstein'
+        papis list --all --file
 
-or export all of them
+    .. raw:: HTML
 
-.. code::
+        <script type="text/javascript"
+        src="https://asciinema.org/a/XwD0ZaUORoOonwDw4rXoQDkjZ.js"
+        id="asciicast-XwD0ZaUORoOonwDw4rXoQDkjZ" async></script>
 
-    papis export --bibtex --all 'author = einstein'
+- List all document year and title with custom formatting:
 
-- Export all documents to bibtex and save them into a ``lib.bib`` file
+    .. code:: bash
 
-.. code::
+        papis list --all --format '{doc[year]} {doc[title]}'
 
-    papis export --all --bibtex --out lib.bib
+    .. raw:: HTML
 
-- Export a folder of one of the documents matching the word ``krebs``
-  into a folder named, ``interesting-document``
+        <script type="text/javascript"
+        src="https://asciinema.org/a/NZ8Ii1wWYPo477CIL4vZhUqOy.js"
+        id="asciicast-NZ8Ii1wWYPo477CIL4vZhUqOy" async></script>
 
-.. code::
+- List all documents according to the bibitem formatting (stored in a template
+  file ``bibitem.template``):
 
-    papis export --folder --out interesting-document krebs
+    .. code:: bash
 
-  this will create the folder ``interesting-document`` containing the
-  ``info.yaml`` file, the linked documents and a ``bibtex`` file for
-  sharing with other people.
+        papis list --all --template bibitem.template
 
-  You can also just export its associated document:
-
-.. code::
-
-    papis export --file krebs
+    .. raw:: HTML
 
+        <script type="text/javascript"
+        src="https://asciinema.org/a/QZTBZ3tFfyk9WQuJ9WWB2UpSw.js"
+        id="asciicast-QZTBZ3tFfyk9WQuJ9WWB2UpSw" async></script>
 
 Cli
 ^^^
-.. click:: papis.commands.export:cli
-    :prog: papis export
+.. click:: papis.commands.list:cli
+    :prog: papis list
 """
+
+import logging
 import papis
 import os
-import sys
-import shutil
 import papis.utils
-import papis.document
-import click
-import papis.cli
-import papis.api
+import papis.strings
+import papis.config
 import papis.database
-import logging
+import papis.downloaders
+import papis.cli
+import papis.pick
+import click
+
+logger = logging.getLogger('list')
 
 
 def run(
-    documents,
-    yaml=False,
-    bibtex=False,
-    json=False,
-    text=False
-):
-    """
-    Exports several documents into something else.
+        documents,
+        libraries=False,
+        downloaders=False,
+        pick=False,
+        files=False,
+        folders=False,
+        info_files=False,
+        notes=False,
+        fmt="",
+        template=None
+        ):
+    """Main method to the list command
 
-    :param document: A ist of papis document
-    :type  document: [papis.document.Document]
-    :param yaml: Wether to return a yaml string
-    :type  yaml: bool
-    :param bibtex: Wether to return a bibtex string
-    :type  bibtex: bool
-    :param json: Wether to return a json string
-    :type  json: bool
-    :param text: Wether to return a text string representing the document
-    :type  text: bool
+    :returns: List different objects
+    :rtype:  list
     """
-    if json:
-        import json
-        return json.dumps(
-            [
-                papis.document.to_dict(document) for document in documents
-            ]
-        )
-
-    if yaml:
-        import yaml
-        return yaml.dump_all(
-            [
-                papis.document.to_dict(document) for document in documents
-            ],
-            allow_unicode=True
-        )
-
-    if bibtex:
-        return '\n'.join([
-            papis.document.to_bibtex(document) for document in documents
-        ])
-
-    if text:
-        text_format = papis.config.get('export-text-format')
-        return '\n'.join([
-            papis.utils.format_doc(text_format, document)
-            for document in documents
-        ])
+    if downloaders:
+        return papis.downloaders.get_available_downloaders()
 
-    return None
+    if template is not None:
+        if not os.path.exists(template):
+            logger.error("Template file %s not found".format(template))
+            return
+        with open(template) as fd:
+            fmt = fd.read()
+
+    if libraries:
+        config = papis.config.get_configuration()
+        return [
+            section + ' ' + config[section]['dir']
+            for section in config
+            if 'dir' in config[section] ]
+
+    if files:
+        return [
+            doc_file for files in [
+                document.get_files() for document in documents
+            ] for doc_file in files
+        ]
+    elif notes:
+        return [
+            os.path.join(d.get_main_folder(), d["notes"])
+            for d in documents
+            if d.has("notes") and isinstance(d["notes"], str)
+                and os.path.exists(
+                        os.path.join(d.get_main_folder(), d["notes"]))]
+    elif info_files:
+        return [
+            os.path.join(
+                document.get_main_folder(),
+                document.get_info_file()
+            ) for document in documents
+        ]
+    elif fmt:
+        return [
+            papis.utils.format_doc(fmt, document)
+            for document in documents
+        ]
+    elif folders:
+        return [
+            document.get_main_folder() for document in documents
+        ]
+    else:
+        return documents
 
 
-@click.command("export")
+@click.command("list")
 @click.help_option('--help', '-h')
 @papis.cli.query_option()
 @click.option(
-    "--yaml",
-    help="Export into yaml",
+    "-i",
+    "--info",
+    help="Show the info file name associated with the document",
     default=False,
-    is_flag=True
-)
+    is_flag=True)
 @click.option(
-    "--bibtex",
-    help="Export into bibtex",
+    "-f", "--file", "_file",
+    help="Show the file name associated with the document",
     default=False,
-    is_flag=True
-)
-@click.option(
-    "--json",
-    help="Export into json",
-    default=False,
-    is_flag=True
-)
-@click.option(
-    "--folder",
-    help="Export document folder to share",
-    default=False,
-    is_flag=True
-)
-@click.option(
-    "-o",
-    "--out",
-    help="Outfile or outdir",
-    default=None
-)
-@click.option(
-    "-t",
-    "--text",
-    help="Text formated reference",
-    default=False,
-    is_flag=True
-)
-@click.option(
-    "-a", "--all",
-    help="Export all without picking",
-    default=False,
-    is_flag=True
-)
-@click.option(
-    "--file",
-    help="Export a copy of a file",
-    default=False,
-    is_flag=True
-)
-def cli(
-        query,
-        yaml,
-        bibtex,
-        json,
-        folder,
-        out,
-        text,
-        all,
-        file
-        ):
-    """Export a document from a given library"""
+    is_flag=True)
+@click.option(
+    "-d", "--dir", "_dir",
+    help="Show the folder name associated with the document",
+    default=False,
+    is_flag=True)
+@click.option(
+    "-n", "--notes",
+    help="List notes files, if any",
+    default=False,
+    is_flag=True)
+@click.option(
+    "--format", "_format",
+    help="List entries using a custom papis format, e.g."
+    " '{doc[year] {doc[title]}",
+    default=None)
+@click.option(
+    "--template",
+    help="Template file containing a papis format to list entries",
+    default=None)
+@click.option(
+    "--downloaders",
+    help="List available downloaders",
+    default=False,
+    is_flag=True)
+@click.option(
+    "--libraries",
+    help="List defined libraries",
+    default=False,
+    is_flag=True)
+@click.option(
+    "-a", "--all", "_all",
+    help="Process all documents matching a query, if a query is given",
+    default=False,
+    is_flag=True)
+def cli(query, info, _file, notes, _dir, _format,
+        template, _all, downloaders, libraries,):
+    """List documents' properties"""
 
-    logger = logging.getLogger('cli:export')
-    documents = papis.database.get().query(query)
+    logger = logging.getLogger('cli:list')
+    documents = []
 
-    if json and folder or yaml and folder:
-        logger.warning("Only --folder flag will be considered")
+    if not libraries and not downloaders and not _file and not info and not _dir:
+        _dir = True
 
-    if not all:
-        document = papis.api.pick_doc(documents)
-        if not document:
-            return 0
-        documents = [document]
+    if not libraries and not downloaders:
+        db = papis.database.get()
+        documents = db.query(query)
+        if not documents:
+            logger.warning(papis.strings.no_documents_retrieved_message)
+        if not _all:
+            documents = filter(lambda x: x, [papis.pick.pick_doc(documents)])
 
-    ret_string = run(
+    objects = run(
         documents,
-        yaml=yaml,
-        bibtex=bibtex,
-        json=json,
-        text=text
-    )
-
-    if ret_string is not None:
-        if out is not None:
-            logger.info("Dumping to {0}".format(out))
-            with open(out, 'a+') as fd:
-                fd.write(ret_string)
-        else:
-            logger.info("Dumping to stdout")
-            print(ret_string)
-        return 0
-
-    for document in documents:
-        if folder:
-            folder = document.get_main_folder()
-            outdir = out or document.get_main_folder_name()
-            if not len(documents) == 1:
-                outdir = os.path.join(
-                    outdir, document.get_main_folder_name()
-                )
-            shutil.copytree(folder, outdir)
-        elif file:
-            logger.info("Exporting file")
-            files = document.get_files()
-            assert(isinstance(files, list))
-            if not files:
-                logger.error('No files found for doc in {0}'.format(
-                    document.get_main_folder()
-                ))
-                continue
-            files_to_open = [papis.api.pick(
-                files,
-                pick_config=dict(
-                    header_filter=lambda x: x.replace(
-                        document.get_main_folder(), ""
-                    )
-                )
-            )]
-            files_to_copy = list(filter(lambda x: x, files_to_open))
-            for file_to_open in files_to_copy:
-
-                if out is not None and len(files_to_open) == 1:
-                    out_file = out
-                else:
-                    out_file = os.path.basename(file_to_open)
-
-                logger.info("copy {0} to {1}".format(
-                    file_to_open,
-                    out_file
-                ))
-                shutil.copyfile(
-                    file_to_open,
-                    out_file
-                )
+        libraries=libraries,
+        downloaders=downloaders,
+        notes=notes,
+        files=_file,
+        folders=_dir,
+        info_files=info,
+        fmt=_format,
+        template=template)
+
+    for o in objects:
+        click.echo(o)
```

### Comparing `papis-0.8.2/papis/commands/external.py` & `papis-0.9/papis/commands/external.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     return "No help message available"
 
 
 def export_variables():
     """Export environment variables so that external script can access to
     the information
     """
-    os.environ["PAPIS_LIB"] = papis.config.get_lib()
-    os.environ["PAPIS_LIB_PATH"] = papis.config.get('dir')
+    os.environ["PAPIS_LIB"] = papis.config.get_lib().name
+    os.environ["PAPIS_LIB_PATH"] = papis.config.get_lib().path_format()
     os.environ["PAPIS_CONFIG_PATH"] = papis.config.get_config_folder()
     os.environ["PAPIS_CONFIG_FILE"] = papis.config.get_config_file()
     os.environ["PAPIS_SCRIPTS_PATH"] = papis.config.get_scripts_folder()
 
 
 @click.command(
     context_settings=dict(
```

### Comparing `papis-0.8.2/papis/commands/git.py` & `papis-0.9/papis/commands/git.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,8 +34,9 @@
 
 
 @click.command("git", context_settings=dict(ignore_unknown_options=True))
 @click.help_option('--help', '-h')
 @click.argument("command", nargs=-1)
 def cli(command):
     "Run a git command in the library folder"
-    return run(papis.config.get("dir"), command=list(command))
+    for d in papis.config.get_lib_dirs():
+        run(d, command=list(command))
```

### Comparing `papis-0.8.2/papis/commands/list.py` & `papis-0.9/papis/commands/open.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,241 +1,184 @@
 """
-This command is to list contents of a library.
+The open command is a very important command in the papis workflow.
+With it you can open documents, folders or marks.
 
-CLI Examples
-^^^^^^^^^^^^
+Marks
+^^^^^
 
-- List all document files associated will all entries:
+One of special things about this command is the possibility of
+creating marks for documents. As you would imagine, it is in general
+difficult to create marks for any kind of data. For instance,
+if our library consists of pdf files and epub files for instance,
+we would like to define bookmarks in order to go back to them at
+some later point.
 
-    .. code:: bash
+How you define marks can be customized through the marks configuration
+settings :ref:`here <marks-options>`.
+The default way of doing it is just by defining a ``marks`` list in a document.
+Let us look at a concrete example:
 
-        papis list --file
+.. code:: yaml
 
-    .. raw:: HTML
+    author: Isaiah Shavitt, Rodney J. Bartlett
+    edition: '1'
+    files: [book.pdf]
+    isbn: 052181832X,9780521818322
 
-        <script type="text/javascript"
-        src="https://asciinema.org/a/XwD0ZaUORoOonwDw4rXoQDkjZ.js"
-        id="asciicast-XwD0ZaUORoOonwDw4rXoQDkjZ" async></script>
+    marks:
+    - {name: Intermediates definition, value: 344}
+    - {name: EOM equations, value: 455}
 
-- List all document year and title with custom formatting:
+    publisher: Cambridge University Press
+    ref: book:293288
+    series: Cambridge Molecular Science
+    title: 'Many-Body Methods in Chemistry and Physics'
+    type: book
+    year: '2009'
 
-    .. code:: bash
+This book has defined two marks. Each mark has a name and a value.
+If you tell the open command to open marks, then it will look for
+the marks and open the value (page number). This is the default behaviour,
+however if you go to the :ref:`configuration <marks-options>`
+you'll see that you can change the convention to what it suits you.
 
-        papis list --format '{doc[year]} {doc[title]}'
 
-    .. raw:: HTML
+Examples
+^^^^^^^^
+- Open a pdf file linked to a document matching the string ``bohm``
 
-        <script type="text/javascript"
-        src="https://asciinema.org/a/NZ8Ii1wWYPo477CIL4vZhUqOy.js"
-        id="asciicast-NZ8Ii1wWYPo477CIL4vZhUqOy" async></script>
+    ::
 
-- List all documents according to the bibitem formatting (stored in a template
-  file ``bibitem.template``):
+        papis open bohm
 
-    .. code:: bash
+- Open the folder where this last document is stored
 
-        papis list --template bibitem.template
+    ::
 
-    .. raw:: HTML
+        papis open -d bohm
 
-        <script type="text/javascript"
-        src="https://asciinema.org/a/QZTBZ3tFfyk9WQuJ9WWB2UpSw.js"
-        id="asciicast-QZTBZ3tFfyk9WQuJ9WWB2UpSw" async></script>
+  Please notice that the file browser used will be also related to
+  the :ref:`file-browser setting <config-settings-file-browser>`.
 
-Python examples
-^^^^^^^^^^^^^^^
+- Open a mark defined in the info file
 
-.. code:: python
+    ::
 
-    # Import the run function from the list command
+        papis open --mark bohm
 
-    from papis.commands.list import run as papis_list
-
-    documents = papis_list(query='einstein', library='papis')
-
-    for doc in documents:
-        print(doc["url"])
-
-    # etc...
-    info_files = list(query='einstein', library='papis', info_files=True)
-
-    # do something with the info file paths...
 
 Cli
 ^^^
-.. click:: papis.commands.list:cli
-    :prog: papis list
+.. click:: papis.commands.open:cli
+    :prog: papis open
 """
-
-import logging
 import papis
-from papis.api import status
-import os
+import papis.api
+import papis.pick
 import papis.utils
 import papis.config
-import papis.database
-import papis.downloaders.utils
 import papis.cli
+import papis.database
 import click
-
-logger = logging.getLogger('list')
+import logging
+from papis.document import from_folder
+import papis.strings
 
 
-def run(
-        query="",
-        library=None,
-        libraries=False,
-        downloaders=False,
-        pick=False,
-        files=False,
-        folders=False,
-        info_files=False,
-        fmt="",
-        template=None
-        ):
-    """Main method to the list command
-
-    :returns: List different objects
-    :rtype:  list
-    """
-    if library is None:
-        library = papis.config.get_lib()
-    config = papis.config.get_configuration()
-    db = papis.database.get(library)
-    if template is not None:
-        if not os.path.exists(template):
-            logger.error(
-                "Template file %s not found" % template
-            )
-            return status.file_not_found
-        fd = open(template)
-        fmt = fd.read()
-        fd.close()
-
-    if downloaders:
-        return papis.downloaders.utils.get_available_downloaders()
-
-    if libraries:
-        return [
-            config[section]['dir']
-            for section in config
-            if 'dir' in config[section]
-        ]
-
-    documents = db.query(query)
-
-    if pick:
-        documents = filter(lambda x: x, [papis.api.pick_doc(documents)])
-
-    if files:
-        return [
-            doc_file for files in [
-                document.get_files() for document in documents
-            ] for doc_file in files
-        ]
-    elif info_files:
-        return [
-            os.path.join(
-                document.get_main_folder(),
-                document.get_info_file()
-            ) for document in documents
-        ]
-    elif fmt:
-        return [
-            papis.utils.format_doc(fmt, document)
-            for document in documents
-        ]
-    elif folders:
-        return [
-            document.get_main_folder() for document in documents
-        ]
+def run(document, opener=None, folder=False, mark=False):
+    logger = logging.getLogger('open:run')
+    if opener is not None:
+        papis.config.set("opentool", opener)
+
+    if folder:
+        # Open directory
+        papis.api.open_dir(document.get_main_folder())
     else:
-        return documents
+        if mark:
+            logger.debug("Getting document's marks")
+            marks = document[papis.config.get("mark-key-name")]
+            if marks:
+                logger.info("Picking marks")
+                mark = papis.api.pick(
+                    marks,
+                    dict(
+                        header_filter=lambda x: papis.utils.format_doc(
+                            papis.config.get("mark-header-format"),
+                            x, key=papis.config.get("mark-format-name")
+                        ),
+                        match_filter=lambda x: papis.utils.format_doc(
+                            papis.config.get("mark-header-format"),
+                            x, key=papis.config.get("mark-format-name")
+                        )
+                    )
+                )
+                if mark:
+                    opener = papis.utils.format_doc(
+                        papis.config.get("mark-opener-format"),
+                        mark, key=papis.config.get("mark-format-name")
+                    )
+                    papis.config.set("opentool", opener)
+        files = document.get_files()
+        if len(files) == 0:
+            logger.error("The document chosen has no files attached")
+            return 1
+        file_to_open = papis.api.pick(
+            files,
+            pick_config=dict(
+                header_filter=lambda x: x.replace(
+                    document.get_main_folder(), ""
+                )
+            )
+        )
+        papis.api.open_file(file_to_open, wait=False)
 
 
-@click.command("list")
-@click.help_option('--help', '-h')
+@click.command("open")
+@click.help_option('-h', '--help')
 @papis.cli.query_option()
+@papis.cli.doc_folder_option()
 @click.option(
-    "-i",
-    "--info",
-    help="Show the info file name associated with the document",
-    default=False,
-    is_flag=True
-)
-@click.option(
-    "-f",
-    "--file",
-    help="Show the file name associated with the document",
-    default=False,
-    is_flag=True
+    "--tool",
+    help="Tool for opening the file (opentool)",
+    default=""
 )
 @click.option(
     "-d",
     "--dir",
-    help="Show the folder name associated with the document",
-    default=False,
-    is_flag=True
-)
-@click.option(
-    "--format",
-    help="List entries using a custom papis format, e.g."
-    " '{doc[year] {doc[title]}",
-    default=None
-)
-@click.option(
-    "--template",
-    help="Template file containing a papis format to list entries",
-    default=None
-)
-@click.option(
-    "-p",
-    "--pick",
-    help="Pick the document instead of listing everything",
+    "folder",
+    help="Open directory",
     default=False,
     is_flag=True
 )
 @click.option(
-    "--downloaders",
-    help="List available downloaders",
+    "--all",
+    help="Open all matching documents",
     default=False,
     is_flag=True
 )
 @click.option(
-    "--libraries",
-    help="List defined libraries",
-    default=False,
-    is_flag=True
+    "-m",
+    "--mark/--no-mark",
+    help="Open mark",
+    default=lambda: True if papis.config.get('open-mark') else False
 )
-def cli(
-        query,
-        info,
-        file,
-        dir,
-        format,
-        template,
-        pick,
-        downloaders,
-        libraries
-        ):
-    """List documents' properties"""
-
-    if not libraries and not downloaders and not file and not info and not dir:
-        dir = True
-
-    lib = papis.config.get_lib()
-
-    objects = run(
-        query=query,
-        library=lib,
-        libraries=libraries,
-        downloaders=downloaders,
-        pick=pick,
-        files=file,
-        folders=dir,
-        info_files=info,
-        fmt=format,
-        template=template
-    )
-    for o in objects:
-        click.echo(o)
-    return status.success
+def cli(query, doc_folder, tool, folder, all, mark):
+    """Open document from a given library"""
+    if tool:
+        papis.config.set("opentool", tool)
+    logger = logging.getLogger('cli:run')
+
+    documents = papis.database.get().query(query)
+
+    if doc_folder:
+        documents = [from_folder(doc_folder)]
+
+    if not documents:
+        logger.warning(papis.strings.no_documents_retrieved_message)
+        return 0
+
+    if not all:
+        documents = [papis.pick.pick_doc(documents)]
+        documents = [d for d in documents if d]
+
+    for document in documents:
+        run(document, folder=folder, mark=mark)
```

### Comparing `papis-0.8.2/papis/commands/mv.py` & `papis-0.9/papis/commands/mv.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,37 +3,25 @@
 Cli
 ^^^
 .. click:: papis.commands.mv:cli
     :prog: papis mv
 """
 import papis
 import os
-import re
 import papis.config
 import papis.utils
 import papis.database
 import subprocess
 import logging
 import papis.cli
-import papis.api
+import papis.pick
+import papis.strings
 import click
 
 
-def get_dirs(main):
-    directories = []
-    p = ""
-    for root, dirs, files in os.walk(main):
-        for di in dirs:
-            p = os.path.join(root, di, papis.utils.get_info_file_name())
-            if not os.path.exists(p) \
-               and not re.match(r".*[.]git.*", os.path.join(root, di)):
-                directories.append(di)
-    return directories
-
-
 def run(document, new_folder_path, git=False):
     logger = logging.getLogger('mv:run')
     folder = document.get_main_folder()
     cmd = ['git', '-C', folder] if git else []
     cmd += ['mv', folder, new_folder_path]
     db = papis.database.get()
     logger.debug(cmd)
@@ -57,38 +45,45 @@
     # Leave this imports here for performance
     import prompt_toolkit
     import prompt_toolkit.completion
 
     logger = logging.getLogger('cli:mv')
 
     documents = papis.database.get().query(query)
+    if not documents:
+        logger.warning(papis.strings.no_documents_retrieved_message)
+        return
 
-    document = papis.api.pick_doc(documents)
+    document = papis.pick.pick_doc(documents)
     if not document:
         return 0
 
-    lib_dir = os.path.expanduser(papis.config.get('dir'))
-
-    directories = get_dirs(lib_dir)
+    lib_dir = os.path.expanduser(papis.config.get_lib_dirs()[0])
 
-    completer = prompt_toolkit.completion.WordCompleter(
-        directories
+    completer = prompt_toolkit.completion.PathCompleter(
+        only_directories=True,
+        get_paths=lambda: [lib_dir]
     )
 
     try:
         new_folder = os.path.join(
             lib_dir,
             prompt_toolkit.prompt(
-                "Enter directory: (Tab completion enabled)\n"
-                ">  ",
+                message=(
+                    "Enter directory  : (Tab completion enabled)\n"
+                    "Current directory: ({dir})\n".format(
+                        dir=document.get_main_folder_name()
+                    ) +
+                    ">  "
+                ),
                 completer=completer,
                 complete_while_typing=True
-            )
-        )
-    except:
+            ))
+    except Exception as e:
+        logger.error(e)
         return 0
 
     logger.info(new_folder)
 
     if not os.path.exists(new_folder):
         logger.info("Creating path %s" % new_folder)
         os.makedirs(new_folder, mode=papis.config.getint('dir-umask'))
```

### Comparing `papis-0.8.2/papis/commands/rename.py` & `papis-0.9/papis/commands/rename.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 Cli
 ^^^
 .. click:: papis.commands.rename:cli
     :prog: papis rename
 """
 import papis
 import os
-import papis.api
+import papis.pick
 import papis.utils
 import subprocess
 import logging
 import click
 import papis.cli
 import papis.database
+import papis.strings
 
 
 def run(document, new_name, git=False):
     db = papis.database.get()
     logger = logging.getLogger('rename:run')
     folder = document.get_main_folder()
     subfolder = os.path.dirname(folder)
@@ -48,15 +49,19 @@
 @click.help_option('--help', '-h')
 @papis.cli.query_option()
 @papis.cli.git_option()
 def cli(query, git):
     """Rename entry"""
 
     documents = papis.database.get().query(query)
-    document = papis.api.pick_doc(documents)
+    logger = logging.getLogger('cli:rename')
+
+    if not documents:
+        logger.warning(papis.strings.no_documents_retrieved_message)
+    document = papis.pick.pick_doc(documents)
     if not document:
         return 0
 
     new_name = papis.utils.input(
         "Enter new folder name:\n"
         ">",
         default=document.get_main_folder_name()
```

### Comparing `papis-0.8.2/papis/commands/run.py` & `papis-0.9/papis/commands/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,9 +53,9 @@
 
 
 @click.command("run", context_settings=dict(ignore_unknown_options=True))
 @click.help_option('--help', '-h')
 @click.argument("run_command", nargs=-1)
 def cli(run_command):
     """Run an arbitrary shell command in the library folder"""
-    folder = papis.config.get("dir")
-    return run(folder, command=run_command)
+    for folder in papis.config.get_lib_dirs():
+        run(folder, command=run_command)
```

### Comparing `papis-0.8.2/papis/database/__init__.py` & `papis-0.9/papis/database/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 DATABASES = dict()
 
 
 def get(library=None):
     global DATABASES
     import papis.config
-    backend = papis.config.get('database-backend')
     if library is None:
         library = papis.config.get_lib()
+    elif isinstance(library, str):
+        library = papis.config.get_lib_from_name(library)
+    backend = papis.config.get('database-backend')
     database = DATABASES.get(library)
     # if there is already a database and the backend of the database
     # is the same as the config backend, then return that library
     # else we will (re)define the database in the dictionary DATABASES
     if database is not None and database.get_backend_name() == backend:
         return DATABASES.get(library)
     if backend == "papis":
```

### Comparing `papis-0.8.2/papis/database/base.py` & `papis-0.9/papis/database/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """
 Here the database abstraction for the libraries is defined.
 """
 
-import os
 import papis.utils
 import papis.config
+import papis.library
 
 
 class Database(object):
     """Abstract class for the database backends
     """
 
-    def __init__(self, library=papis.config.get_lib()):
-        self.lib = library
+    def __init__(self, library=None):
+        self.lib = library or papis.config.get_lib()
+        assert(isinstance(self.lib, papis.library.Library))
 
     def initialize(self):
-        pass
+        raise NotImplementedError('Initialize not implemented')
 
     def get_backend_name(self):
         raise NotImplementedError('Get backend name not implemented')
 
     def get_lib(self):
         """Get library name
         """
-        return self.lib
+        return self.lib.name
 
-    def get_dir(self):
-        """Get directory of the library
+    def get_dirs(self):
+        """Get directories of the library
         """
-        return os.path.expanduser(papis.config.get('dir', section=self.lib))
+        return self.lib.paths
 
     def match(self, document, query_string):
         """Wether or not document matches query_string
 
         :param document: Document to be matched
         :type  document: papis.document.Document
         :param query_string: Query string
```

### Comparing `papis-0.8.2/papis/database/whoosh.py` & `papis-0.9/papis/database/whoosh.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,35 +46,42 @@
 import whoosh.index
 import whoosh.qparser
 
 import papis.config
 import papis.document
 import papis.database.base
 import papis.database.cache
+from papis.utils import get_cache_home, get_folders, folders_to_documents
 
 
 class Database(papis.database.base.Database):
 
     def __init__(self, library=None):
         papis.database.base.Database.__init__(self, library)
         self.logger = logging.getLogger('db:whoosh')
+        self.cache_dir = os.path.join(get_cache_home(), 'database', 'whoosh')
+        self.index_dir = os.path.expanduser(
+            os.path.join(
+                self.cache_dir,
+                papis.database.cache.get_cache_file_name(
+                    self.lib.path_format()
+                )
+            )
+        )
+
         self.initialize()
 
     def get_backend_name(self):
         return 'whoosh'
 
     def clear(self):
         import shutil
         if self.index_exists():
             self.logger.warning('Clearing the database')
-            shutil.rmtree(self.get_index_dir())
-        else:
-            self.logger.warning(
-                'Trying to clear database, but no database found'
-            )
+            shutil.rmtree(self.index_dir)
 
 #   TODO
     def match(self, document, query_string):
         pass
 
     def add(self, document):
         schema_keys = self.get_schema_init_fields().keys()
@@ -151,24 +158,23 @@
         return document.get_main_folder()
 
     def create_index(self):
         """Create a brand new index, notice that if an index already
         exists it will delete it and create a new one.
         """
         self.logger.debug('Creating index...')
-        index_dir = self.get_index_dir()
-        if not os.path.exists(index_dir):
-            self.logger.debug('Creating dir %s' % index_dir)
-            os.makedirs(index_dir)
-        whoosh.index.create_in(self.get_index_dir(), self.create_schema())
+        if not os.path.exists(self.index_dir):
+            self.logger.debug('Creating dir %s' % self.index_dir)
+            os.makedirs(self.index_dir)
+        whoosh.index.create_in(self.index_dir, self.create_schema())
 
     def index_exists(self):
-        """Check if index already exists in get_index_dir()
+        """Check if index already exists in index_dir()
         """
-        return whoosh.index.exists_in(self.get_index_dir())
+        return whoosh.index.exists_in(self.index_dir)
 
     def add_document_with_writer(self, document, writer, schema_keys):
         """Helper function that takes a writer and a dictionary
         containing the keys of the schema and adds the document to the writer.
         Notice that this function does only two things, creating a suitable
         dictionary to be added to the database and adding it to the writer.
         It DOES NOT commit the change to the writer, this has to be done
@@ -196,40 +202,74 @@
         """This function initializes the database. Basically it goes through
         all folders from the library (that contain an `info.yaml` file)
         and adds the documents to the database index. This function is
         expensive and will be called only if no index is present, so
         at the time of building a brand new index.
         """
         self.logger.debug('Indexing the library, this might take a while...')
-        folders = papis.utils.get_folders(self.get_dir())
-        documents = papis.database.cache.folders_to_documents(folders)
+        folders = sum([get_folders(d) for d in self.get_dirs()], [])
+        documents = folders_to_documents(folders)
         schema_keys = self.get_schema_init_fields().keys()
         writer = self.get_writer()
         for doc in documents:
             self.add_document_with_writer(doc, writer, schema_keys)
         writer.commit()
 
     def initialize(self):
         """Function to be called everytime a database object is created.
         It checks if an index exists, if not, it creates one and
         indexes the library.
+
+        If the schema fields have been changed, it updates the database.
         """
         if self.index_exists():
-            self.logger.debug('Initialized index found for library')
-            return True
+            user_fields = self.get_schema_init_fields()
+            db_fields = self.get_schema()
+
+            user_field_names = sorted(list(user_fields))
+            db_field_names = sorted(db_fields.names())
+
+            # If the user fields and the fields in the DB
+            # aren't the same, then we have to rebuild the
+            # database.
+            if user_field_names != db_field_names:
+                self.rebuild()
+                self.logger.debug("Rebuilt database because field names"
+                                  "don't match")
+            else:
+                # Otherwise, verify that the fields are
+                # all the same and rebuild if any have
+                # changed at all.
+                rebuilt_db = False
+                for field in user_field_names:
+                    if user_fields[field] != db_fields[field]:
+                        self.rebuild()
+                        self.logger.debug("Rebuilt DB because field types"
+                                          " don't match")
+                        rebuilt_db = True
+                        break
+
+                if not rebuilt_db:
+                    self.logger.debug('Initialized index found for library')
+                    return True
+        self.create_index()
+        self.do_indexing()
+
+    def rebuild(self):
+        self.clear()
         self.create_index()
         self.do_indexing()
 
     def get_index(self):
         """Gets the index for the current library
 
         :returns: Index
         :rtype:  whoosh.index
         """
-        return whoosh.index.open_dir(self.get_index_dir())
+        return whoosh.index.open_dir(self.index_dir)
 
     def get_writer(self):
         """Gets the writer for the current library
 
         :returns: Writer
         :rtype:  whoosh.writer
         """
@@ -262,41 +302,12 @@
         from whoosh.fields import TEXT, ID, KEYWORD, STORED
         # This part is non-negotiable
         fields = {self.get_id_key(): ID(stored=True, unique=True)}
         user_prototype = eval(
             papis.config.get('whoosh-schema-prototype')
         )
         fields.update(user_prototype)
-        fields_list = eval(papis.config.get('whoosh-schema-fields'))
-        if not isinstance(fields_list, list):
-            raise Exception('whoosh-schema-fields should be a python list')
+        fields_list = papis.config.getlist('whoosh-schema-fields')
         for field in fields_list:
             fields.update({field: TEXT(stored=True)})
         # self.logger.debug('Schema prototype: {}'.format(fields))
         return fields
-
-    def get_cache_dir(self):
-        """Get general directory to store whoosh indexes.
-
-        :returns: Full path to whoosh cache home directory
-        :rtype:  str
-        """
-        path = os.path.join(
-            papis.database.cache.get_cache_home(),
-            'whoosh'
-        )
-        # self.logger.debug('Cache dir %s' % path)
-        return path
-
-    def get_index_dir(self):
-        """Get the directory inside `get_cache_dir` to store the index.
-        :returns: Full path to index dir
-        :rtype:  str
-        """
-        path = os.path.expanduser(
-            os.path.join(
-                self.get_cache_dir(),
-                papis.database.cache.get_name(self.get_dir())
-            )
-        )
-        # self.logger.debug('Index dir %s' % path)
-        return path
```

### Comparing `papis-0.8.2/papis/downloaders/acs.py` & `papis-0.9/papis/downloaders/worldscientific.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 import re
 import papis.downloaders.base
 
 
 class Downloader(papis.downloaders.base.Downloader):
 
     def __init__(self, url):
-        papis.downloaders.base.Downloader.__init__(self, url, name="acs")
+        papis.downloaders.base.Downloader.__init__(
+            self, url, name="worldscientific"
+        )
         self.expected_document_extension = 'pdf'
-        # It seems to be necessary so that acs lets us download the bibtex
         self.cookies = {
             'gdpr': 'true',
         }
 
     @classmethod
     def match(cls, url):
-        if re.match(r".*acs.org.*", url):
+        if re.match(r".*worldscientific.com.*", url):
             return Downloader(url)
         else:
             return False
 
     def get_doi(self):
-        # .../pubs.acs.org/doi/whatever/10.1021/acs.jchemed.6b00559?blah=2
-        mdoi = re.match(r'.*acs.org/doi/[^/]+/([^?]*)', self.get_url())
+        url = self.uri
+        self.logger.debug('Parsing doi from {0}'.format(url))
+        mdoi = re.match(r'.*/doi/(.*/[^?&%^$]*).*', url)
         if mdoi:
             doi = mdoi.group(1).replace("abs/", "").replace("full/", "")
-            self.logger.debug("[doi] = %s" % doi)
             return doi
-        else:
-            self.logger.error("Doi not found!!")
+
+        mdoi = re.match(r'.*/worldscibooks/(.*/[^?&%^$]*).*', url)
+        if mdoi:
+            doi = mdoi.group(1).replace("abs/", "").replace("full/", "")
+            return doi
+
+        return None
 
     def get_document_url(self):
-        # http://pubs.acs.org/doi/pdf/10.1021/acs.jchemed.6b00559
-        return "http://pubs.acs.org/doi/pdf/" + self.get_doi()
+        durl = "https://www.worldscientific.com/doi/pdf/%s" % self.get_doi()
+        self.logger.debug("[doc url] = %s" % durl)
+        return durl
 
     def get_bibtex_url(self):
-        url = "http://pubs.acs.org/action/downloadCitation"\
+        url = "https://www.worldscientific.com/action/downloadCitation"\
               "?format=bibtex&cookieSet=1&doi=%s" % self.get_doi()
         self.logger.debug("[bibtex url] = %s" % url)
         return url
```

### Comparing `papis-0.8.2/papis/downloaders/arxiv.py` & `papis-0.9/papis/downloaders/ieee.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,66 @@
 import re
-import os
+import urllib.parse
+import urllib.request
 import papis.downloaders.base
-import arxiv2bib
 
 
 class Downloader(papis.downloaders.base.Downloader):
 
     def __init__(self, url):
-        papis.downloaders.base.Downloader.__init__(self, url, name="arxiv")
+        papis.downloaders.base.Downloader.__init__(self, url, name="ieee")
         self.expected_document_extension = 'pdf'
 
     @classmethod
     def match(cls, url):
-        m = re.match(r"^arxiv:(.*)", url, re.IGNORECASE)
+        m = re.match(r"^ieee:(.*)", url, re.IGNORECASE)
         if m:
-            url = "https://arxiv.org/abs/{m}".format(m=m.group(1))
-        if re.match(r".*arxiv.org.*", url):
-            # https://arxiv.org/pdf/1707.09820|.pdf?blahslas=sdfad|
+            url = "http://ieeexplore.ieee.org/document/{m}".format(
+                m=m.group(1))
+            return Downloader(url)
+        if re.match(r".*ieee.org.*", url):
             url = re.sub(r"\.pdf.*$", "", url)
             return Downloader(url)
         else:
             return False
 
     def get_identifier(self):
-        """Get arxiv identifier
-        :returns: Identifier
-        """
-        url = self.get_url()
-        return re.sub(r'^.*arxiv.org/(abs|pdf)/(.*)\/?$', r'\2', url)
+        url = self.uri
+        return re.sub(r'^.*ieeexplore\.ieee\.org/document/(.*)\/', r'\1', url)
 
     def get_bibtex_url(self):
         identifier = self.get_identifier()
-        return identifier
+        bibtex_url = \
+            'http://ieeexplore.ieee.org/xpl/downloadCitations?reload=true'
+        data = {
+            'recordIds': identifier,
+            'citations-format': 'citation-and-abstract',
+            'download-format': 'download-bibtex',
+            'x': '0',
+            'y': '0'
+        }
+        return bibtex_url, data
 
     def download_bibtex(self):
-        bib_url = self.get_bibtex_url()
-        bibtexCli = arxiv2bib.Cli([bib_url])
-        bibtexCli.run()
+        bib_url, values = self.get_bibtex_url()
+        post_data = urllib.parse.urlencode(values)
+        post_data = post_data.encode('ascii')
+
         self.logger.debug("[bibtex url] = %s" % bib_url)
-        data = os.linesep.join(bibtexCli.output)
-        self.bibtex_data = data
+
+        req = urllib.request.Request(bib_url, post_data)
+        with urllib.request.urlopen(req) as response:
+            data = response.read()
+            text = data.decode('utf-8')
+            text = text.replace('<br>', '')
+            self.bibtex_data = text
 
     def get_document_url(self):
-        # https://arxiv.org/pdf/1702.01590
         identifier = self.get_identifier()
         self.logger.debug("[paper id] = %s" % identifier)
-        pdf_url = "https://arxiv.org/pdf/"+identifier+".pdf"
+        pdf_url = "{}{}".format(
+            "http://ieeexplore.ieee.org/"
+            "stampPDF/getPDF.jsp?tp=&isnumber=&arnumber=",
+            identifier
+        )
         self.logger.debug("[pdf url] = %s" % pdf_url)
         return pdf_url
```

### Comparing `papis-0.8.2/papis/downloaders/frontiersin.py` & `papis-0.9/papis/downloaders/frontiersin.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def match(cls, url):
         if re.match(r".*frontiersin.org.*", url):
             return Downloader(url)
         else:
             return False
 
     def get_doi(self):
-        url = self.get_url()
+        url = self.uri
         self.logger.info('Parsing doi from {0}'.format(url))
         mdoi = re.match(r'.*/articles/([^/]+/[^/?&%^$]+).*', url)
         if mdoi:
             doi = mdoi.group(1)
             return doi
         return None
```

### Comparing `papis-0.8.2/papis/downloaders/get.py` & `papis-0.9/papis/downloaders/get.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import papis.downloaders.base
 
 
 class Downloader(papis.downloaders.base.Downloader):
     def __init__(self, url):
         papis.downloaders.base.Downloader.__init__(self, url, name="get")
+        self.priority = 0
 
     @classmethod
     def match(cls, url):
         """
         >>> Downloader.match('http://wha2341!@#!@$%!@#file.pdf') is False
         False
         >>> Downloader.match('https://whateverpt?is?therefile.epub') is False
@@ -16,14 +17,17 @@
         >>> not Downloader.match('http://whatever?path?is?therefile')
         True
         """
         endings = "pdf|djvu|epub|mobi|jpg|png|md"
         m = re.match(r"^http.*\.(%s)$" % endings, url, re.IGNORECASE)
         if m:
             d = Downloader(url)
-            d.expected_document_extension = m.group(1)
+            extension = m.group(1)
+            d.logger.info(
+                'Expecting a document of type "{0}"'.format(extension))
+            d.expected_document_extension = extension
             return d
         else:
-            return False
+            return None
 
     def get_document_url(self):
-        return self.get_url()
+        return self.uri
```

### Comparing `papis-0.8.2/papis/downloaders/scitationaip.py` & `papis-0.9/papis/downloaders/scitationaip.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
             self, url, name="scitationaip"
         )
         self.expected_document_extension = 'pdf'
 
     @classmethod
     def match(cls, url):
         # http://aip.scitation.org/doi/10.1063/1.4873138
-        if re.match(r".*(aip|aapt).scitation.org.*", url):
+        if re.match(r".*(aip|aapt)\.scitation\.org.*", url):
             return Downloader(url)
         else:
             return False
 
     def get_doi(self):
-        mdoi = re.match(r'.*/doi/(.*/[^?&%^$]*).*', self.get_url())
+        mdoi = re.match(r'.*/doi/(.*/[^?&%^$]*).*', self.uri)
         if mdoi:
             doi = mdoi.group(1).replace("abs/", "").replace("full/", "")
             return doi
         else:
             return None
 
     def get_document_url(self):
```

### Comparing `papis-0.8.2/papis/downloaders/thesesfr.py` & `papis-0.9/papis/downloaders/thesesfr.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,26 @@
         >>> d = Downloader("http://www.theses.fr/2014TOU30305")
         >>> d.get_identifier()
         '2014TOU30305'
         >>> d = Downloader("http://www.theses.fr/2014TOU30305.bib/?asdf=2")
         >>> d.get_identifier()
         '2014TOU30305'
         """
-        m = re.match(r".*theses.fr/([^/?.&]+).*", self.url)
+        m = re.match(r".*theses.fr/([^/?.&]+).*", self.uri)
         return m.group(1) if m is not None else None
 
     def get_document_url(self):
         """
         >>> d = Downloader("http://www.theses.fr/2014TOU30305")
         >>> d.get_document_url()
         'http://thesesups.ups-tlse.fr/2722/1/2014TOU30305.pdf'
         >>> d = Downloader("http://theses.fr/1998ENPC9815")
         >>> d.get_document_url()
         """
-        raw_data = self.session.get(self.url).content.decode('utf-8')
+        raw_data = self.session.get(self.uri).content.decode('utf-8')
         soup = bs4.BeautifulSoup(raw_data, "html.parser")
         a = list(filter(
             lambda t: re.match(r'.*en ligne.*', t.text),
             soup.find_all('a')
         ))
 
         if not a:
@@ -66,8 +66,7 @@
         >>> d = Downloader("http://www.theses.fr/2014TOU30305")
         >>> d.get_bibtex_url()
         'http://www.theses.fr/2014TOU30305.bib'
         """
         url = "http://www.theses.fr/{id}.bib".format(id=self.get_identifier())
         self.logger.debug("[bibtex url] = %s" % url)
         return url
-
```

### Comparing `papis-0.8.2/papis/tui/widgets/command_line_prompt.py` & `papis-0.9/papis/tui/widgets/command_line_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from prompt_toolkit.filters import has_focus, Condition
 from prompt_toolkit.layout.processors import BeforeInput
 from prompt_toolkit.buffer import Buffer
-from prompt_toolkit.completion import WordCompleter, Completer, Completion
+from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.layout.containers import (
-    HSplit, Window, WindowAlign, ConditionalContainer
+    Window, ConditionalContainer
 )
 from prompt_toolkit.layout.controls import (
     BufferControl,
-    FormattedTextControl
 )
 from prompt_toolkit.application.current import get_app
-from prompt_toolkit.utils import Event
+from prompt_toolkit.filters import has_focus
 import shlex
 
 
-class Command(Event):
+class Command:
     """
     :param name: Name of the command
     :type  name: parameter_type
     :param run: A callable object where the first argument is the cmd itself.
     :type  run: callable
     """
     def __init__(self, name, run, aliases=[]):
@@ -89,8 +87,7 @@
     @property
     def text(self):
         return self.buf.text
 
     @text.setter
     def text(self, text):
         self.buf.text = text
-
```

### Comparing `papis-0.8.2/papis/tui/widgets/list.py` & `papis-0.9/papis/tui/widgets/list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 import re
-from prompt_toolkit.application.current import get_app
-from prompt_toolkit.formatted_text.html import HTML, html_escape
-from prompt_toolkit.filters import Condition
+from prompt_toolkit.formatted_text.html import HTML
 from prompt_toolkit.layout.screen import Point
 from prompt_toolkit.buffer import Buffer
-from prompt_toolkit.layout.controls import (
-    FormattedTextControl, BufferControl
-)
-from prompt_toolkit.widgets import HorizontalLine
+from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.containers import (
-    HSplit, Window, ConditionalContainer, WindowAlign, ScrollOffsets
+    Window, ConditionalContainer, WindowAlign, ScrollOffsets
 )
 from prompt_toolkit.filters import has_focus
-from prompt_toolkit.layout import NumberedMargin
 import multiprocessing
 
 import logging
 
 logger = logging.getLogger('tui:widget:list')
 
 
+def match_against_regex(regex, line, index):
+    return index if regex.match(line) else None
+
+
 class OptionsList(ConditionalContainer):
 
     def __init__(
             self,
             options,
             default_index=0,
             header_filter=lambda x: x,
             match_filter=lambda x: x,
             custom_filter=None,
-            search_buffer=Buffer(multiline=False)
+            search_buffer=Buffer(multiline=False),
+            cpu_count=multiprocessing.cpu_count()
             ):
 
         assert(isinstance(options, list))
         assert(callable(header_filter))
         assert(callable(match_filter))
         assert(isinstance(default_index, int))
 
         self.search_buffer = search_buffer
+        self.last_query_text = ''
         self.search_buffer.on_text_changed += self.update
 
         self.header_filter = header_filter
         self.match_filter = match_filter
         self.current_index = default_index
         self.entries_left_offset = 0
-        self.pool = multiprocessing.Pool(multiprocessing.cpu_count())
+        self.pool = multiprocessing.Pool(cpu_count)
+
+        self.options_headers_linecount = []
+        self._indices_to_lines = []
 
         self._options = []
+        self.marks = []
         self.max_entry_height = 1
         # Options are processed here also through the setter
         self.options = options
         self.cursor = Point(0, 0)
 
         self.content = FormattedTextControl(
             text=self.get_tokens,
@@ -61,20 +65,20 @@
         self.content_window = Window(
             content=self.content,
             wrap_lines=False,
             allow_scroll_beyond_bottom=True,
             scroll_offsets=ScrollOffsets(bottom=self.max_entry_height),
             cursorline=False,
             cursorcolumn=False,
-            #right_margins=[NumberedMargin()],
-            #left_margins=[NumberedMargin()],
+            # right_margins=[NumberedMargin()],
+            # left_margins=[NumberedMargin()],
             align=WindowAlign.LEFT,
             height=None,
             get_line_prefix=self.get_line_prefix
-            #get_line_prefix=lambda line, b: [('bg:red', '  ')]
+            # get_line_prefix=lambda line, b: [('bg:red', '  ')]
         )
 
         self.update()
 
         super(OptionsList, self).__init__(
             content=self.content_window,
             filter=(
@@ -86,30 +90,35 @@
 
     def __del__(self):
         # Clean initialized pool upon deleting of the object
         self.pool.close()
         self.pool.join()
 
     def get_line_prefix(self, line, blih):
-        try:
-            index = self.indices.index(self.current_index)
-            cline = sum(
-                self.options_headers_linecount[i]
-                for i in self.indices[0:index]
-            )
-            cline = sum(
-                self.options_headers_linecount[i]
-                for i in self.indices[0:index]
-            )
-            if line == cline:
-                return [('class:options_list.selected_margin', '>')]
+        if self.current_index is None:
+            return
+        current_line = self.index_to_line(self.current_index)
+        if (0 <= line - current_line
+                < self.options_headers_linecount[self.current_index]):
+            return [('class:options_list.selected_margin', '|')]
+        else:
+            marked_clines = [self.index_to_line(i) for i in self.marks]
+            if line in marked_clines:
+                return [('class:options_list.marked_margin', '#')]
             else:
                 return [('class:options_list.unselected_margin', ' ')]
-        except:
-            return
+
+    def toggle_mark_current_selection(self):
+        if self.current_index in self.marks:
+            self.marks.pop(self.marks.index(self.current_index))
+        else:
+            self.mark_current_selection()
+
+    def mark_current_selection(self):
+        self.marks.append(self.current_index)
 
     @property
     def options(self):
         return self._options
 
     @options.setter
     def options(self, new_options):
@@ -138,55 +147,69 @@
         except ValueError:
             pass
 
     def go_top(self):
         if len(self.indices) > 0:
             self.current_index = self.indices[0]
 
+    def deselect(self):
+        self.current_index = None
+
     def go_bottom(self):
         if len(self.indices) > 0:
             self.current_index = self.indices[-1]
 
     @property
+    def query_text(self):
+        return self.search_buffer.text
+
+    @property
     def search_regex(self):
         cleaned_search = (
-            self.search_buffer.text
+            self.query_text
             .replace('(', '\\(')
             .replace(')', '\\)')
             .replace('+', '\\+')
             .replace('[', '\\[')
             .replace(']', '\\]')
         )
         return re.compile(r".*"+re.sub(r"\s+", ".*", cleaned_search), re.I)
 
-    @staticmethod
-    def match_against_regex(regex, line, index):
-        return index if regex.match(line, re.I) else None
-
     def update(self, *args):
         self.filter_options()
+        self._indices_to_lines = []
 
     def filter_options(self, *args):
         indices = []
         regex = self.search_regex
 
+        if self.query_text == self.last_query_text:
+            return
+
+        if self.query_text.startswith(self.last_query_text):
+            search_indices = self.indices
+        else:
+            search_indices = range(len(self.options_matchers))
+
+        self.last_query_text = self.query_text
+
         result = [
             self.pool.apply_async(
-                OptionsList.match_against_regex,
+                match_against_regex,
                 args=(regex, opt, i,)
-            ) for i, opt in enumerate(self.options_matchers)
+            )
+            for i, opt in enumerate(self.options_matchers)
+            if i in search_indices
         ]
 
-        indices =  [d.get() for d in result if d.get() is not None]
+        indices = [d.get() for d in result if d.get() is not None]
 
         self.indices = indices
         if len(self.indices) and self.current_index not in self.indices:
-            if self.current_index < min(self.indices):
-                self.current_index = self.indices[0]
-            elif self.current_index > max(self.indices):
+            if self.current_index > max(self.indices):
                 self.current_index = max(self.indices)
             else:
                 self.current_index = self.indices[0]
 
     def get_selection(self):
         if len(self.indices) and self.current_index is not None:
             return self.options[self.current_index]
@@ -198,42 +221,57 @@
         try:
             index = self.indices.index(self.current_index)
             line = sum(
                 self.options_headers_linecount[i]
                 for i in self.indices[0:index]
             )
             self.cursor = Point(0, line)
-        except Exception as e:
+        except Exception:
             self.cursor = Point(0, 0)
 
     def get_tokens(self):
         self.update_cursor()
         result = sum(
             [self.options_headers[i] for i in self.indices],
             []
         )
         return result
 
+    def index_to_line(self, index):
+        if not self._indices_to_lines:
+            options_headers_linecount = [
+                self.options_headers_linecount[i] if i in self.indices else 0
+                for i in range(len(self.options_headers_linecount))
+            ]
+            self._indices_to_lines = [
+                sum(options_headers_linecount[0:i])
+                for i in range(len(options_headers_linecount))
+            ]
+        return self._indices_to_lines[index]
+
     def process_options(self):
         logger.debug('processing {0} options'.format(len(self.options)))
+        self.marks = []
         self.options_headers_linecount = [
             len(self.header_filter(o).split('\n'))
             for o in self.options
         ]
         self.max_entry_height = max(self.options_headers_linecount)
         logger.debug('processing headers')
         self.options_headers = []
         for o in self.options:
             prestring = self.header_filter(o) + '\n'
             try:
                 htmlobject = HTML(prestring).formatted_text
-            except:
+            except Exception as e:
                 logger.error(
-                    'Error processing html for \n {0}'.format(prestring)
+                    'Error processing html for \n {0} \n {1}'.format(
+                        prestring, e
+                    )
                 )
-                htmlobject = [ ('fg:red', prestring) ]
+                htmlobject = [('fg:red', prestring)]
             self.options_headers += [htmlobject]
         logger.debug('got {0} headers'.format(len(self.options_headers)))
         logger.debug('processing matchers')
         self.options_matchers = [self.match_filter(o) for o in self.options]
         self.indices = range(len(self.options))
         logger.debug('got {0} matchers'.format(len(self.options_matchers)))
```

### Comparing `papis-0.8.2/papis/tui/__init__.py` & `papis-0.9/papis/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `papis-0.8.2/papis/tui/app.py` & `papis-0.9/papis/tui/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-import os
-import re
 from prompt_toolkit.application import Application
 from prompt_toolkit.formatted_text.html import HTML
-from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.enums import EditingMode
 from prompt_toolkit.layout.processors import BeforeInput
 from prompt_toolkit.key_binding import KeyBindings, merge_key_bindings
-from prompt_toolkit.layout.screen import Point
 from prompt_toolkit.filters import has_focus, Condition
 from prompt_toolkit.styles import Style
 from prompt_toolkit.layout.containers import (
-    HSplit, Window, ConditionalContainer
+    HSplit, Window
 )
 from prompt_toolkit.layout.controls import (
     BufferControl,
 )
 from prompt_toolkit.layout.layout import Layout
 import papis.config as config
+import papis.document
 import logging
 
 from .widgets.command_line_prompt import Command
 from .widgets import (
     InfoWindow, CommandLinePrompt, HelpWindow, OptionsList,
     MessageToolbar
 )
 
 logger = logging.getLogger('pick')
 
 _keys_info = None
+
+
 def get_keys_info():
     global _keys_info
     if not _keys_info:
         _keys_info = {
             "move_down_key": {
                 'key': config.get('move_down_key', section='tui'),
                 'help': 'Move cursor down in the list',
             },
             "move_up_key": {
                 'key': config.get('move_up_key', section='tui'),
                 'help': 'Move cursor up in the list',
             },
             "move_down_while_info_window_active_key": {
-                'key': config.get('move_down_while_info_window_active_key', section='tui'),
+                'key': config.get(
+                    'move_down_while_info_window_active_key', section='tui'
+                ),
                 'help': 'Move cursor down while info window is active',
             },
             "move_up_while_info_window_active_key": {
-                'key': config.get('move_up_while_info_window_active_key', section='tui'),
+                'key': config.get(
+                    'move_up_while_info_window_active_key', section='tui'
+                ),
                 'help': 'Move cursor up while info window is active',
             },
             "focus_command_line_key": {
                 'key': config.get('focus_command_line_key', section='tui'),
                 'help': 'Focus command line prompt',
             },
             "edit_document_key": {
@@ -85,34 +88,38 @@
     kb = KeyBindings()
 
     @kb.add('escape', filter=Condition(lambda: app.message_toolbar.text))
     def _(event):
         event.app.message_toolbar.text = None
 
     @kb.add('escape', filter=Condition(lambda: app.error_toolbar.text))
-    def _(event):
+    def _escape(event):
         event.app.error_toolbar.text = None
 
     @kb.add('c-n', filter=~has_focus(app.info_window))
-    @kb.add(keys_info["move_down_key"]["key"], filter=~has_focus(app.info_window))
+    @kb.add(
+        keys_info["move_down_key"]["key"], filter=~has_focus(app.info_window)
+    )
     def down_(event):
         event.app.options_list.move_down()
         event.app.refresh()
         event.app.update()
 
     @kb.add(
         keys_info["move_down_while_info_window_active_key"]["key"],
         filter=has_focus(app.info_window)
     )
     def down_info(event):
         down_(event)
         event.app.update_info_window()
 
     @kb.add('c-p', filter=~has_focus(app.info_window))
-    @kb.add(keys_info["move_up_key"]["key"], filter=~has_focus(app.info_window))
+    @kb.add(
+        keys_info["move_up_key"]["key"], filter=~has_focus(app.info_window)
+    )
     def up_(event):
         event.app.options_list.move_up()
         event.app.refresh()
         event.app.update()
 
     @kb.add(
         keys_info["move_up_while_info_window_active_key"]["key"],
@@ -150,18 +157,22 @@
         try:
             event.app.command_line_prompt.trigger()
         except Exception as e:
             event.app.error_toolbar.text = str(e)
         event.app.command_line_prompt.clear()
 
     @kb.add('escape', filter=has_focus(app.command_line_prompt))
-    def _(event):
+    def _escape_when_commandline_has_focus(event):
         event.app.layout.focus(event.app.options_list.search_buffer)
         event.app.command_line_prompt.clear()
 
+    @kb.add('c-t')
+    def _toggle_mark_(event):
+        event.app.options_list.toggle_mark_current_selection()
+
     return kb
 
 
 def get_commands(app):
 
     kb = KeyBindings()
     keys_info = get_keys_info()
@@ -256,15 +267,14 @@
             self,
             options,
             default_index=0,
             header_filter=lambda x: x,
             match_filter=lambda x: x
             ):
 
-
         self.info_window = InfoWindow()
         self.help_window = HelpWindow()
         self.message_toolbar = MessageToolbar(style="class:message_toolbar")
         self.error_toolbar = MessageToolbar(style="class:error_toolbar")
         self.status_line = MessageToolbar(style="class:status_line")
         self.status_line_format = config.get(
             'status_line_format', section="tui"
@@ -273,14 +283,15 @@
         self.options_list = OptionsList(
             options,
             default_index,
             header_filter,
             match_filter,
             custom_filter=~has_focus(self.help_window)
         )
+        self.options_list.search_buffer.on_text_changed += self.update
 
         commands, commands_kb = get_commands(self)
         self.command_line_prompt = CommandLinePrompt(commands=commands)
         kb = merge_key_bindings([create_keybindings(self), commands_kb])
 
         _root_container = HSplit([
             HSplit([
@@ -296,16 +307,14 @@
             self.help_window,
             self.error_toolbar,
             self.message_toolbar,
             self.status_line,
             self.command_line_prompt.window,
         ])
 
-        regex = re.compile(r'.*\.([^ ]+) +at.*')
-
         help_text = ""
         keys_info = get_keys_info()
         for k in keys_info:
             help_text += (
                 "<ansired>{k[key]}</ansired>: {k[help]}\n".format(
                     k=keys_info[k]
                 )
@@ -342,15 +351,15 @@
             include_default_pygments_style=False,
             full_screen=True,
             enable_page_navigation_bindings=True
         )
         self.update()
 
     def deselect(self):
-        self.options_list.current_index = None
+        self.options_list.deselect()
 
     def refresh_status_line(self):
         self.status_line.text = self.status_line_format.format(
             selected_index=int(self.options_list.current_index) + 1,
             number_of_documents=len(self.options_list.options),
         )
 
@@ -362,8 +371,8 @@
         self.refresh_status_line()
 
     def get_selection(self):
         return self.options_list.get_selection()
 
     def update_info_window(self):
         doc = self.options_list.get_selection()
-        self.info_window.set_text(doc.dump())
+        self.info_window.text = papis.document.dump(doc)
```

### Comparing `papis-0.8.2/papis/api.py` & `papis-0.9/papis/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,78 @@
 """This module describes which functions are intended to be used by users to
 create papis scripts.
 """
 
 import logging
-
-logger = logging.getLogger("api")
-logger.debug("importing")
-
-import os
 import papis.utils
 import papis.commands
 import papis.config
+import papis.pick
 import papis.database
 
-
-class status():
-    success = 0
-    generic_fail = 1
-    file_not_found = 2
+logger = logging.getLogger("api")
+logger.debug("importing")
 
 
-def get_lib():
+def get_lib_name():
     """Get current library, it either retrieves the library from
     the environment PAPIS_LIB variable or from the command line
     args passed by the user.
 
     :returns: Library name
     :rtype:  str
 
-    >>> get_lib() is not None
+    >>> get_lib_name() is not None
     True
     """
-    return papis.config.get_lib()
+    return papis.config.get_lib_name()
 
 
-def set_lib(library):
+def set_lib_from_name(library):
     """Set current library, it either sets the library in
     the environment PAPIS_LIB variable or in the command line
     args passed by the user.
 
     :param library: Name of library or path to a given library
     :type  library: str
 
     """
-    return papis.config.set_lib(library)
-
-
-def get_arg(arg, default=None):
-    try:
-        val = getattr(papis.commands.get_args(), arg)
-    except AttributeError:
-        try:
-            val = os.environ["PAPIS_"+arg.upper()]
-        except KeyError:
-            val = default
-    return val
+    return papis.config.set_lib_from_name(library)
 
 
 def get_libraries():
     """Get all libraries declared in the configuration. A library is discovered
-    if the ``dir`` key defined in the library section.
+    if the ``dir`` or ``dirs`` key defined in the library section.
 
     :returns: List of library names
     :rtype: list
 
     >>> len(get_libraries()) >= 1
     True
 
     """
     libs = []
     config = papis.config.get_configuration()
     for key in config.keys():
-        if "dir" in config[key]:
+        if "dir" in config[key] or "dirs" in config[key]:
             libs.append(key)
     return libs
 
 
-def pick_doc(documents: list):
+def pick_doc(documents):
     """Pick a document from documents with the correct formatting
 
     :documents: List of documents
     :returns: Document
 
-    >>> from papis.document import from_data
-    >>> doc = from_data({'title': 'Hello World'})
-    >>> pick_doc([doc]).dump()
-    'title:   Hello World\\n'
-
-    """
-    header_format_path = papis.config.get('header-format-file')
-    if header_format_path is not None:
-        with open(os.path.expanduser(header_format_path)) as fd:
-            header_format = fd.read()
-    else:
-        header_format = papis.config.get("header-format")
-    match_format = papis.config.get("match-format")
-    pick_config = dict(
-        header_filter=lambda x: papis.utils.format_doc(header_format, x),
-        match_filter=lambda x: papis.utils.format_doc(match_format, x)
-    )
-    return papis.api.pick(
-        documents,
-        pick_config
-    )
+    """
+    return papis.pick.pick_doc(documents)
 
 
-def pick(options: list, pick_config={}):
+def pick(options, pick_config={}):
     """This is a wrapper for the various pickers that are supported.
     Depending on the configuration different selectors or 'pickers'
     are used.
 
     :param options: List of different objects. The type of the objects within
         the list must be supported by the pickers. This is the reason why this
         function is difficult to generalize for external picker programs.
@@ -118,51 +81,29 @@
     :param pick_config: Dictionary with additional configuration for the used
         picker. This depends on the picker.
     :type  pick_config: dict
 
     :returns: Returns elements of ``options``.
     :rtype: Element(s) of ``options``
 
-    >>> papis.config.set('picktool', 'papis.pick')
-    >>> pick(['something'])
-    'something'
-    >>> papis.config.set('picktool', 'nonexistent')
-    >>> pick(['something'])
-    Traceback (most recent call last):
-    ...
-    Exception: I don\'t know how to use the picker \'nonexistent\'
-    >>> papis.config.set('picktool', 'papis.pick')
-
-    """
-    # Leave this import here
-    import papis.config
-    logger.debug("Parsing picktool")
-    external_picker = papis.config.get_external_picker()
-    picker = external_picker or papis.config.get("picktool")
-    if picker == "papis.pick":
-        import papis.pick
-        logger.debug("Using papis.pick picker")
-        return papis.pick.pick(options, **pick_config)
-    elif papis.config.get_external_picker() is not None:
-        return papis.config.get_external_picker()(options, **pick_config)
-    else:
-        raise Exception("I don't know how to use the picker '%s'" % picker)
+    """
+    return papis.pick.pick(options, **pick_config)
 
 
 def open_file(file_path, wait=True):
     """Open file using the ``opentool`` key value as a program to
     handle file_path.
 
     :param file_path: File path to be handled.
     :type  file_path: str
     :param wait: Wait for the completion of the opener program to continue
     :type  wait: bool
 
     """
-    papis.utils.general_open(file_path, "opentool", wait=wait)
+    papis.utils.open_file(file_path, wait=wait)
 
 
 def open_dir(dir_path, wait=True):
     """Open dir using the ``file-browser`` key value as a program to
     open dir_path.
 
     :param dir_path: Folder path to be handled.
@@ -194,15 +135,15 @@
     :type  library: str
 
     :returns: List of all documents.
     :rtype: list
 
     >>> import tempfile
     >>> folder = tempfile.mkdtemp()
-    >>> set_lib(folder)
+    >>> set_lib_from_name(folder)
     >>> docs = get_all_documents_in_lib(folder)
     >>> len(docs)
     0
 
     """
     return papis.database.get(library=library).get_all_documents()
 
@@ -222,15 +163,15 @@
 
     >>> import tempfile
     >>> docs = get_documents_in_dir(tempfile.mkdtemp())
     >>> len(docs)
     0
 
     """
-    set_lib(directory)
+    set_lib_from_name(directory)
     return get_documents_in_lib(directory, search)
 
 
 def get_documents_in_lib(library=None, search=""):
     """Get documents contained in the given library with possibly a search
     string.
 
@@ -253,9 +194,20 @@
 
     :param lib: Library name.
     :type  lib: str
 
     >>> clear_lib_cache()
 
     """
-    lib = papis.api.get_lib() if lib is None else lib
     papis.database.get(lib).clear()
+
+
+def doi_to_data(doi):
+    """Try to get from a DOI expression a dictionary with the document's data
+    using the crossref module.
+
+    :param doi: DOI expression.
+    :type  doi: str
+    :returns: Document's data
+    :rtype: dict
+    """
+    return papis.crossref.doi_to_data(doi)
```

### Comparing `papis-0.8.2/papis/bibtex.py` & `papis-0.9/papis/bibtex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,141 +1,146 @@
 from __future__ import unicode_literals
 from __future__ import absolute_import, division, print_function
-import re
+
 import logging
 import os
+import re
+
 import papis.config
+import click
+import papis.document
+import papis.importer
+import papis.utils
 
 logger = logging.getLogger("bibtex")
 
 bibtex_types = [
-  "article",
-  "book",
-  "booklet",
-  "conference",
-  "inbook",
-  "incollection",
-  "inproceedings",
-  "manual",
-  "mastersthesis",
-  "misc",
-  "phdthesis",
-  "proceedings",
-  "techreport",
-  "unpublished"
-] + re.sub(r" *", "", papis.config.get('extra-bibtex-types')).split(',')
+  "article", "book", "booklet", "conference", "inbook", "incollection",
+  "inproceedings", "manual", "mastersthesis", "misc", "phdthesis",
+  "proceedings", "techreport", "unpublished"
+] + papis.config.getlist('extra-bibtex-types')
 
 bibtex_type_converter = {
-  "conferencePaper" : "inproceedings",
-  "journalArticle" : "article",
-  "journal" : "article"
+  "conferencePaper": "inproceedings",
+  "journalArticle": "article",
+  "journal": "article"
 }
 
 bibtex_keys = [
-    "addendum",
-    "address",
-    "afterword",
-    "annotator",
-    "annote",
-    "author",
-    "bookauthor",
-    "booksubtitle",
-    "booktitle",
-    "booktitleaddon",
-    "chapter",
-    "commentator",
-    "crossref",
-    "date",
-    "doi",
-    "edition",
-    "editor",
-    "editora",
-    "editorb",
-    "editorc",
-    "eid",
-    "eprint",
-    "eprintclass",
-    "eprinttype",
-    "eventdate",
-    "eventtitle",
-    "eventtitleaddon",
-    "foreword",
-    "holder",
-    "howpublished",
-    "institution",
-    "introduction",
-    "isbn",
-    "isrn",
-    "issn",
-    "issue",
-    "issuesubtitle",
-    "issuetitle",
-    "journal",
-    "journalsubtitle",
-    "journaltitle",
-    "key",
-    "language",
-    "location",
-    "mainsubtitle",
-    "maintitle",
-    "maintitleaddon",
-    "month",
-    "note",
-    "number",
-    "organization",
-    "origlanguage",
-    "pages",
-    "pagetotal",
-    "part",
-    "publisher",
-    "pubstate",
-    "school",
-    "series",
-    "subtitle",
-    "title",
-    "translator",
-    "type",
-    "titleaddon",
-    "url",
-    "urldate",
-    "venue",
-    "version",
-    "volume",
-    "volumes",
-    "year",
-  ] + re.sub(r" *", "", papis.config.get('extra-bibtex-keys')).split(',')
+    "addendum", "address", "afterword", "annotator", "annote", "author",
+    "bookauthor", "booksubtitle", "booktitle", "booktitleaddon", "chapter",
+    "commentator", "crossref", "date", "doi", "edition", "editor", "editora",
+    "editorb", "editorc", "eid", "eprint", "eprintclass", "eprinttype",
+    "eventdate", "eventtitle", "eventtitleaddon", "foreword", "holder",
+    "howpublished", "institution", "introduction", "isbn", "isrn",
+    "issn", "issue", "issuesubtitle", "issuetitle", "journal",
+    "journalsubtitle", "journaltitle", "key", "language", "location",
+    "mainsubtitle", "maintitle", "maintitleaddon", "month", "note",
+    "number", "organization", "origlanguage", "pages", "pagetotal", "part",
+    "publisher", "pubstate", "school", "series", "subtitle", "title",
+    "translator", "type", "titleaddon", "url", "urldate", "venue", "version",
+    "volume", "volumes", "year",
+] + papis.config.getlist('extra-bibtex-keys')
 
 bibtex_key_converter = {
-    "abstractNote" : "abstract",
-    "university" : "school",
-    "conferenceName" : "eventtitle",
-    "place" : "location",
-    "publicationTitle" : "journal",
-    "proceedingsTitle" : "booktitle"
+    "abstractNote": "abstract",
+    "university": "school",
+    "conferenceName": "eventtitle",
+    "place": "location",
+    "publicationTitle": "journal",
+    "proceedingsTitle": "booktitle"
 }
 
+
+class Importer(papis.importer.Importer):
+
+    """Importer that parses a bibtex files"""
+
+    def __init__(self, **kwargs):
+        papis.importer.Importer.__init__(self, name='bibtex', **kwargs)
+
+    @classmethod
+    def match(cls, uri):
+        if (not os.path.exists(uri) or os.path.isdir(uri) or
+                papis.utils.get_document_extension(uri) == 'pdf'):
+            return None
+        importer = Importer(uri=uri)
+        importer.fetch()
+        return importer if importer.ctx else None
+
+    @papis.importer.cache
+    def fetch(self):
+        self.logger.info("Reading input file = %s" % self.uri)
+        try:
+            bib_data = bibtex_to_dict(self.uri)
+            if len(bib_data) > 1:
+                self.logger.warning(
+                    'Your bibtex file contains more than one entry,'
+                    ' I will be taking the first entry')
+            if bib_data:
+                self.ctx.data = bib_data[0]
+        except Exception as e:
+            self.logger.debug(e)
+
+
+@click.command('bibtex')
+@click.pass_context
+@click.argument('bibfile', type=click.Path(exists=True))
+@click.help_option('--help', '-h')
+def explorer(ctx, bibfile):
+    """
+    Import documents from a bibtex file
+
+    Examples of its usage are
+
+    papis explore bibtex lib.bib pick
+
+    """
+    logger = logging.getLogger('explore:bibtex')
+    logger.info('Reading in bibtex file {}'.format(bibfile))
+    docs = [
+        papis.document.from_data(d)
+        for d in bibtex_to_dict(bibfile)
+    ]
+    ctx.obj['documents'] += docs
+    logger.info('{} documents found'.format(len(docs)))
+
+
 def bibtexparser_entry_to_papis(entry):
     """Convert keys of a bib entry in bibtexparser format to papis compatible
     format.
 
     :param entry: Dictionary with keys of bibtexparser format.
     :type  entry: dict
     :returns: Dictionary with keys of papis format.
 
     """
-    result = dict()
-    for key in entry.keys():
-        if key == 'ID':
-            result['ref'] = entry[key]
-        elif key == 'ENTRYTYPE':
-            result['type'] = entry[key]
-        elif key == 'link':
-            result['url'] = entry[key]
-        else:
-            result[key] = entry[key]
+    from bibtexparser.customization import splitname
+    def to_author_list(authors):
+        author_list = []
+        for author in re.split(r"\s+and\s+", authors):
+            parts = splitname(author)
+            given = " ".join(parts["first"])
+            family = " ".join(parts["von"] + parts["last"] + parts["jr"])
+
+            author_list.append(dict(family=family, given=given))
+
+        return author_list
+
+    from collections import OrderedDict
+    key_conversion = OrderedDict({
+        "ID": {"key": "ref"},
+        "ENTRYTYPE": {"key": "type"},
+        "link": {"key": "url"},
+        "author": {"key": "author_list", "action": to_author_list},
+    })
+
+    result = papis.document.keyconversion_to_data(key_conversion, entry,
+            keep_unknown_keys=True)
+
     return result
 
 
 def bibtex_to_dict(bibtex):
     """
     Convert bibtex file to dict
 
@@ -145,29 +150,31 @@
 
     :param bibtex: Bibtex file path or bibtex information in string format.
     :type  bibtex: str
     :returns: Dictionary with bibtex information with keys that bibtex
         formally recognizes.
     :rtype:  list
     """
-    import bibtexparser
+    from bibtexparser.bparser import BibTexParser
+
+    parser = BibTexParser(common_strings=True,
+            ignore_nonstandard_types=False,
+            homogenize_fields=False,
+            interpolate_strings=True)
+
     # bibtexparser has too many debug messages to be useful
     logging.getLogger("bibtexparser.bparser").setLevel(logging.WARNING)
     global logger
     if os.path.exists(bibtex):
         with open(bibtex) as fd:
             logger.debug("Reading in file %s" % bibtex)
             text = fd.read()
     else:
         text = bibtex
-    logger.debug("Removing comments...")
-    text = re.sub(r" +%.*", "", text)
-    logger.debug("Removing empty lines...")
-    text = re.sub(r"^\s*$", "", text)
-    entries = bibtexparser.loads(text).entries
+    entries = parser.parse(text, partial=True).entries
     # Clean entries
     return [bibtexparser_entry_to_papis(entry) for entry in entries]
 
 
 def unicode_to_latex(text):
     """
     unicode_to_latex - what it says
```

### Comparing `papis-0.8.2/papis/dissemin.py` & `papis-0.9/papis/dissemin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 import urllib.request  # urlopen, Request
 import urllib.parse  # import urlencode
 import papis.config
 import json
+import click
+import papis.document
 
 
 logger = logging.getLogger('dissemin')
 
 
 def dissemin_authors_to_papis_authors(data):
     new_data = dict()
     if 'authors' in data.keys():
         authors = []
         for author in data['authors']:
-            keys = ('first', 'last')
+            # keys = ('first', 'last')
             authors.append(
                 dict(
                     given_name=author['name']['first'],
                     surname=author['name']['last']
                 )
             )
         new_data["author_list"] = authors
@@ -47,24 +49,42 @@
 
 
 def get_data(query=None):
     """
     Get data using the dissemin API
     https://dissem.in/api/search/?q=pregroup
     """
-    dict_params = { "q": query, }
-    result = []
-    clean_params = {x: dict_params[x] for x in dict_params if dict_params[x]}
+    dict_params = {"q": query}
     params = urllib.parse.urlencode(dict_params)
     main_url = "https://dissem.in/api/search/?"
     req_url = main_url + params
     logger.debug("url = " + req_url)
     url = urllib.request.Request(
         req_url,
         headers={
             'User-Agent': papis.config.get('user-agent')
         }
     )
     jsondoc = urllib.request.urlopen(url).read().decode()
     paperlist = json.loads(jsondoc)
-    docs = sum([dissemindoc_to_papis(d) for d in paperlist['papers']], [])
-    return docs
+    return sum([dissemindoc_to_papis(d) for d in paperlist['papers']], [])
+
+
+@click.command('dissemin')
+@click.pass_context
+@click.help_option('--help', '-h')
+@click.option('--query', '-q', default=None)
+def explorer(ctx, query):
+    """
+    Look for documents on dissem.in
+
+    Examples of its usage are
+
+    papis explore dissemin -q 'Albert einstein' pick cmd 'firefox {doc[url]}'
+
+    """
+    logger = logging.getLogger('explore:dissemin')
+    logger.info('Looking up...')
+    data = get_data(query=query)
+    docs = [papis.document.from_data(data=d) for d in data]
+    ctx.obj['documents'] += docs
+    logger.info('{} documents found'.format(len(docs)))
```

### Comparing `papis-0.8.2/papis/docmatcher.py` & `papis-0.9/papis/docmatcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,18 +15,15 @@
         DocMatcher.parse()
     Now the DocMatcher is ready to match documents with the input query
     via the `return_if_match` method, which is used to parallelize the
     matching.
     """
     search = ""
     parsed_search = None
-    if papis.config.get('format-jinja2-enable'):
-        doc_format = '{{' + papis.config.get('format-doc-name') + '["DOC_KEY"]}}' 
-    else:
-        doc_format = '{' + papis.config.get('format-doc-name') + '[DOC_KEY]}'
+    doc_format = '{' + papis.config.get('format-doc-name') + '[DOC_KEY]}'
     logger = logging.getLogger('DocMatcher')
     matcher = None
 
     @classmethod
     def return_if_match(cls, doc):
         """Use the attribute `cls.parsed_search` to match the `doc` document
         to the previously parsed query.
@@ -43,16 +40,16 @@
         ([(['einste'], {})], {})
         >>> DocMatcher.return_if_match(doc) is not None
         True
         >>> DocMatcher.parse('heisenberg')
         ([(['heisenberg'], {})], {})
         >>> DocMatcher.return_if_match(doc) is not None
         False
-        >>> DocMatcher.parse('title = ein')
-        ([(['title', '=', 'ein'], {})], {})
+        >>> DocMatcher.parse('title : ein')
+        ([(['title', ':', 'ein'], {})], {})
         >>> DocMatcher.return_if_match(doc) is not None
         True
 
         """
         match = None
         for parsed in cls.parsed_search:
             if len(parsed) == 1:
@@ -91,53 +88,55 @@
         :param cls: The class object, since it is a static method
         :type  cls: object
         :param search: Search text string if a custom search string is to be
             used. False if the `cls.search` class attribute is to be used.
         :type  search: str
         :returns: Parsed query
         :rtype:  list
-        >>> print(DocMatcher.parse('hello author = einstein'))
-        [['hello'], ['author', '=', 'einstein']]
+        >>> print(DocMatcher.parse('hello author : einstein'))
+        [['hello'], ['author', ':', 'einstein']]
         >>> print(DocMatcher.parse(''))
         []
         >>> print(\
             DocMatcher.parse(\
-                '"hello world whatever =" tags = \\\'hello ====\\\''))
-        [['hello world whatever ='], ['tags', '=', 'hello ====']]
+                '"hello world whatever :" tags : \\\'hello ::::\\\''))
+        [['hello world whatever :'], ['tags', ':', 'hello ::::']]
         >>> print(DocMatcher.parse('hello'))
         [['hello']]
         """
         if search is None:
             search = cls.search
         cls.parsed_search = parse_query(search)
         return cls.parsed_search
 
 
 def parse_query(query_string):
     import pyparsing
     logger = logging.getLogger('query_parser')
     logger.debug('Parsing search')
 
-    papis_key = pyparsing.Word(pyparsing.alphanums + '-._/')
+    papis_key_word = pyparsing.Word(pyparsing.alphanums + '-._/')
+    papis_value_word = pyparsing.Word(pyparsing.alphanums + '-._/()')
 
     papis_value = pyparsing.QuotedString(
         quoteChar='"', escChar='\\', escQuote='\\'
     ) ^ pyparsing.QuotedString(
         quoteChar="'", escChar='\\', escQuote='\\'
-    ) ^ papis_key
+    ) ^ papis_value_word
 
     equal = (
         pyparsing.ZeroOrMore(" ") +
-        pyparsing.Literal('=') +
+        pyparsing.Literal(':') +
         pyparsing.ZeroOrMore(" ")
     )
 
     papis_query = pyparsing.ZeroOrMore(
         pyparsing.Group(
             pyparsing.ZeroOrMore(
-                papis_key + equal
+                papis_key_word + equal
             ) + papis_value
         )
     )
     parsed = papis_query.parseString(query_string)
+
     logger.debug('Parsed query = %s' % parsed)
     return parsed
```

### Comparing `papis-0.8.2/papis/document.py` & `papis-0.9/papis/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,532 +1,603 @@
+import sys
 import os
-import shutil
-import papis.utils
-import papis.config
-import papis.bibtex
+from os.path import expanduser
+import configparser
+import papis.exceptions
+import papis.library
+from collections import OrderedDict
 import logging
-import re
 
+logger = logging.getLogger("config")
+logger.debug("importing")
 
-logger = logging.getLogger("document")
+_CURRENT_LIBRARY = None  #: Current library in use
+_CONFIGURATION = None  #: Global configuration object variable.
+_DEFAULT_SETTINGS = None  #: Default settings for the whole papis.
+_OVERRIDE_VARS = {
+    "folder": None,
+    "file": None,
+    "scripts": None
+}
+
+
+def get_default_opener():
+    """Get the default file opener for the current system
+    """
+    if sys.platform.startswith('darwin'):
+        return "open"
+    elif os.name == 'nt':
+        return "start"
+    elif os.name == 'posix':
+        return "xdg-open"
+
+
+general_settings = {
+    "local-config-file": ".papis.config",
+    "database-backend": "papis",
+    "default-query-string": ".",
+
+    "opentool": get_default_opener(),
+    "dir-umask": 0o755,
+    "browser": os.environ.get('BROWSER') or get_default_opener(),
+    "picktool": "papis",
+    "mvtool": "mv",
+    "editor": os.environ.get('EDITOR')
+                        or os.environ.get('VISUAL')
+                        or get_default_opener(),
+    "notes-name": "notes.tex",
+    "use-cache": True,
+    "cache-dir": None,
+    "use-git": False,
+
+    "add-confirm": False,
+    "add-folder-name": "",
+    "add-file-name": None,
+    "add-interactive": False,
+    "add-edit": False,
+    "add-open": False,
+
+    "browse-key": 'url',
+    "browse-query-format": "{doc[title]} {doc[author]}",
+    "search-engine": "https://duckduckgo.com",
+    "user-agent": 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3)',
+    "scripts-short-help-regex": ".*papis-short-help: *(.*)",
+    "info-name": "info.yaml",
+    "doc-url-key-name": "doc_url",
+
+    "open-mark": False,
+    "mark-key-name": "marks",
+    "mark-format-name": "mark",
+    "mark-header-format": "{mark[name]} - {mark[value]}",
+    "mark-match-format": "{mark[name]} - {mark[value]}",
+    "mark-opener-format": get_default_opener(),
+
+    "file-browser": get_default_opener(),
+    "bibtex-journal-key": 'journal',
+    "extra-bibtex-keys": "[]",
+    "extra-bibtex-types": "[]",
+    "default-library": "papers",
+    "format-doc-name": "doc",
+    "match-format":
+        "{doc[tags]}{doc.subfolder}{doc[title]}{doc[author]}{doc[year]}",
+    "header-format-file": None,
+    "header-format": (
+        "<ansired>{doc.html_escape[title]}</ansired>\n"
+        " <ansigreen>{doc.html_escape[author]}</ansigreen>\n"
+        "  <blue>({doc.html_escape[year]})</blue> "
+        "[<ansiyellow>{doc.html_escape[tags]}</ansiyellow>]"
+    ),
+
+    "info-allow-unicode": True,
+    "ref-format": "{doc[doi]}",
+    "multiple-authors-separator": " and ",
+    "multiple-authors-format": "{au[family]}, {au[given]}",
+
+    "whoosh-schema-fields": "['doi']",
+    "whoosh-schema-prototype":
+    '{\n'
+    '"author": TEXT(stored=True),\n'
+    '"title": TEXT(stored=True),\n'
+    '"year": TEXT(stored=True),\n'
+    '"tags": TEXT(stored=True),\n'
+    '}',
+
+    'unique-document-keys': "['doi','ref','isbn','isbn10','url','doc_url']",
+
+    "downloader-proxy": None,
+    "bibtex-unicode": False,
+
+    "document-description-format": '{doc[title]} - {doc[author]}',
+
+}
+
+
+def get_general_settings_name():
+    """Get the section name of the general settings
+    :returns: Section's name
+    :rtype:  str
+    >>> get_general_settings_name()
+    'settings'
+    """
+    return "settings"
 
 
-def open_in_browser(document):
-    """Browse document's url whenever possible.
+def get_default_settings(section="", key=""):
+    """Get the default settings for all non-user variables
+    in papis.
 
-    :document: Document object
-    :returns: Returns the url that is composed from the document
-    :rtype:  str
+    If section and key are given, then the setting
+    for the given section and the given key are returned.
+
+    If only ``key`` is given, then the setting
+    for the ``general`` section is returned.
+
+    :param section: Particular section of the default settings
+    :type  section: str
+    :param key: Setting's name to be queried for.
+    :type  key: str
+
+    """
+    global _DEFAULT_SETTINGS
+    # We use an OrderedDict so that the first entry will always be the general
+    # settings, also good for automatic documentation
+    if _DEFAULT_SETTINGS is None:
+        _DEFAULT_SETTINGS = OrderedDict()
+        _DEFAULT_SETTINGS.update({
+            get_general_settings_name(): general_settings,
+        })
+        import papis.tui
+        _DEFAULT_SETTINGS.update(papis.tui.get_default_settings())
+    if not section and not key:
+        return _DEFAULT_SETTINGS
+    elif not section:
+        return _DEFAULT_SETTINGS[get_general_settings_name()][key]
+    else:
+        return _DEFAULT_SETTINGS[section][key]
+
+
+def register_default_settings(settings_dictionary):
+    """Register configuration settings into the global configuration registry.
+
+    Notice that you can define sections or global options. For instance,
+    let us suppose that a script called ``hubation`` defines some
+    configuration options. In the script there could be the following defined
+
+    ::
 
-    >>> import papis.config; papis.config.set('browser', 'echo')
-    >>> papis.config.set('browse-key', 'url')
-    >>> open_in_browser( from_data({'url': 'hello.com'}) )
-    'hello.com'
-    >>> papis.config.set('browse-key', 'doi')
-    >>> open_in_browser( from_data({'doi': '12312/1231'}) )
-    'https://doi.org/12312/1231'
-    >>> papis.config.set('browse-key', 'nonexistentkey')
-    >>> open_in_browser( from_data({'title': 'blih', 'author': 'me'}) )
-    'https://duckduckgo.com/?q=blih+me'
-    """
-    global logger
-    url = None
-    key = papis.config.get("browse-key")
-
-    if document.has(key):
-        if "doi" == key:
-            url = 'https://doi.org/{}'.format(document['doi'])
-        elif "isbn" == key:
-            url = 'https://isbnsearch.org/isbn/{}'.format(document['isbn'])
+        import papis.config
+        options = {'hubation': { 'command': 'open'}}
+        papis.config.register_default_settings(options)
+
+    and later on the script can use these options as:
+
+    ::
+
+        papis.config.get('command', section='hubation')
+
+    :param settings_dictionary: A dictionary with settings
+    :type  settings_dictionary: dict
+    """
+    default_settings = get_default_settings()
+    # we do a for loop because apparently the OrderedDict removes all
+    # key-val fields after updating, so we have to do it by hand
+    for section in settings_dictionary.keys():
+        if section in default_settings.keys():
+            default_settings[section].update(settings_dictionary[section])
         else:
-            url = document[key]
+            default_settings[section] = settings_dictionary[section]
 
-    if url is None or key == 'search-engine':
-        from urllib.parse import urlencode
-        params = {
-            'q': papis.utils.format_doc(
-                papis.config.get('browse-query-format'),
-                document
-            )
-        }
-        url = papis.config.get('search-engine') + '/?' + urlencode(params)
 
-    logger.debug("Opening url %s:" % url)
-    papis.utils.general_open(
-        url, "browser", wait=False
+def get_config_home():
+    """Returns the base directory relative to which user specific configuration
+    files should be stored.
+
+    :returns: Configuration base directory
+    :rtype:  str
+    """
+    xdg_home = os.environ.get('XDG_CONFIG_HOME')
+    if xdg_home:
+        return expanduser(xdg_home)
+    else:
+        return os.path.join(expanduser('~'), '.config')
+
+
+def get_config_dirs():
+    """Get papis configuration directories where the configuration
+    files might be stored
+    """
+    dirs = []
+    if os.environ.get('XDG_CONFIG_DIRS'):
+        # get_config_home should also be included on top of XDG_CONFIG_DIRS
+        dirs += [
+            os.path.join(d, 'papis') for d in
+            os.environ.get('XDG_CONFIG_DIRS').split(':')
+        ]
+    # Take XDG_CONFIG_HOME and $HOME/.papis for backwards
+    # compatibility
+    dirs += [
+        os.path.join(get_config_home(), 'papis'),
+        os.path.join(expanduser('~'), '.papis')
+    ]
+    return dirs
+
+
+def get_config_folder():
+    """Get folder where the configuration files are stored,
+    e.g. ``/home/user/.papis``. It is XDG compatible, which means that if the
+    environment variable ``XDG_CONFIG_HOME`` is defined it will use the
+    configuration folder ``XDG_CONFIG_HOME/papis`` instead.
+
+    """
+    config_dirs = get_config_dirs()
+    for config_dir in config_dirs:
+        if os.path.exists(config_dir):
+            return config_dir
+    # If no folder is found, then get the config home
+    return os.path.join(get_config_home(), 'papis')
+
+
+def get_config_file():
+    """Get the path of the main configuration file,
+    e.g. /home/user/.papis/config
+    """
+    global _OVERRIDE_VARS
+    if _OVERRIDE_VARS["file"] is not None:
+        config_file = _OVERRIDE_VARS["file"]
+    else:
+        config_file = os.path.join(
+            get_config_folder(), "config"
+        )
+    logger.debug("Getting config file %s" % config_file)
+    return config_file
+
+
+def get_configpy_file():
+    """Get the path of the main python configuration file,
+    e.g. /home/user/config/.papis/config.py
+    """
+    return os.path.join(get_config_folder(), "config.py")
+
+
+def set_config_file(filepath):
+    """Override the main configuration file path
+    """
+    global _OVERRIDE_VARS
+    logger.debug("Setting config file to %s" % filepath)
+    _OVERRIDE_VARS["file"] = filepath
+
+
+def get_scripts_folder():
+    """Get folder where the scripts are stored,
+    e.g. /home/user/.papis/scripts
+    """
+    return os.path.join(
+        get_config_folder(), "scripts"
     )
-    return url
 
 
-def from_folder(folder_path):
-    """Construct a document object from a folder
+def set(key, val, section=None):
+    """Set a key to val in some section and make these changes available
+    everywhere.
+    """
+    config = get_configuration()
+    if not config.has_section(section or "settings"):
+        config.add_section(section or "settings")
+    config[section or get_general_settings_name()][key] = str(val)
+
+
+def general_get(key, section=None, data_type=None):
+    """General getter method that will be specialized for different modules.
+
+    :param data_type: The data type that should be expected for the value of
+        the variable.
+    :type  data_type: DataType, e.g. int, src ...
+    :param default: Default value for the configuration variable if it is not
+        set.
+    :type  default: It should be the same that ``data_type``
+    :param extras: List of tuples containing section and prefixes
+    """
+    # Init main variables
+    method = None
+    value = None
+    config = get_configuration()
+    libname = get_lib_name()
+    global_section = get_general_settings_name()
+    specialized_key = section + "-" + key if section is not None else key
+    extras = [(section, key)] if section is not None else []
+    sections = [(global_section, specialized_key)] +\
+        extras + [(libname, specialized_key)]
+    default_settings = get_default_settings()
+
+    # Check data type for setting getter method
+    if data_type == int:
+        method = config.getint
+    elif data_type == float:
+        method = config.getfloat
+    elif data_type == bool:
+        method = config.getboolean
+    else:
+        method = config.get
+
+    # Try to get key's value from configuration
+    for extra in sections:
+        sec = extra[0]
+        whole_key = extra[1]
+        if sec not in config.keys():
+            continue
+        if whole_key in config[sec].keys():
+            value = method(sec, whole_key)
+
+    if value is None:
+        try:
+            default = default_settings[
+                section or global_section
+            ][
+                specialized_key if section is None else key
+            ]
+        except KeyError:
+            raise papis.exceptions.DefaultSettingValueMissing(key)
+        else:
+            return default
+    return value
 
-    :param folder_path: Full path to a valid papis folder
-    :type  folder_path: str
-    :returns: A papis document
-    :rtype:  papis.document.Document
+
+def get(*args, **kwargs):
+    """String getter
     """
-    return papis.document.Document(folder=folder_path)
+    return general_get(*args, **kwargs)
+
 
+def getint(*args, **kwargs):
+    """Integer getter
+    >>> set('something', 42)
+    >>> getint('something')
+    42
+    """
+    return general_get(*args, data_type=int, **kwargs)
 
-def from_data(data):
-    """Construct a document object from a data dictionary.
 
-    :param data: Data to be copied to a new document
-    :type  data: dict
-    :returns: A papis document
-    :rtype:  papis.document.Document
+def getfloat(*args, **kwargs):
+    """Float getter
+    >>> set('something', 0.42)
+    >>> getfloat('something')
+    0.42
     """
-    return papis.document.Document(data=data)
+    return general_get(*args, data_type=float, **kwargs)
 
 
-def to_bibtex(document):
-    """Create a bibtex string from document's information
+def getboolean(*args, **kwargs):
+    """Bool getter
+    >>> set('add-open', True)
+    >>> getboolean('add-open')
+    True
+    """
+    return general_get(*args, data_type=bool, **kwargs)
 
-    :param document: Papis document
-    :type  document: Document
-    :returns: String containing bibtex formating
-    :rtype:  str
 
-    >>> import papis.config
-    >>> papis.config.set('bibtex-journal-key', 'journal_abbrev')
-    >>> doc = from_data({'title': 'Hello', 'type': 'book', 'journal': 'jcp'})
-    >>> import tempfile; doc.set_folder('path/to/superfolder')
-    >>> to_bibtex(doc)
-    '@book{superfolder,\\n  journal = {jcp},\\n  title = {Hello},\\n  type = {book},\\n}\\n'
-    >>> doc['journal_abbrev'] = 'j'
-    >>> to_bibtex(doc)
-    '@book{superfolder,\\n  journal = {j},\\n  title = {Hello},\\n  type = {book},\\n}\\n'
-    >>> del doc['title']
-    >>> doc['ref'] = 'hello1992'
-    >>> to_bibtex(doc)
-    '@book{hello1992,\\n  journal = {j},\\n  type = {book},\\n}\\n'
-    """
-    bibtexString = ""
-    bibtexType = ""
-
-    # First the type, article ....
-    if "type" in document.keys():
-        if document["type"] in papis.bibtex.bibtex_types:
-            bibtexType = document["type"]
-        elif document["type"] in papis.bibtex.bibtex_type_converter.keys():
-            bibtexType = papis.bibtex.bibtex_type_converter[document["type"]]
-    if not bibtexType:
-        bibtexType = "article"
+def getlist(key, **kwargs):
+    """Bool getter
 
-    ref = document["ref"]
-    if not ref:
-        try:
-            ref = os.path.basename(document.get_main_folder())
-        except:
-            if document.has('doi'):
-                ref = document['doi']
-            else:
-                ref = 'noreference'
-
-    ref = re.sub(r'[;,()\/{}\[\]]', '', ref)
-
-    bibtexString += "@%s{%s,\n" % (bibtexType, ref)
-    for bibKey in sorted(document.keys()):
-        logger.debug('%s : %s' % (bibKey, document[bibKey]))
-        if bibKey in papis.bibtex.bibtex_key_converter:
-            newBibKey = papis.bibtex.bibtex_key_converter[bibKey]
-            document[newBibKey] = document[bibKey]
-            continue
-        if bibKey in papis.bibtex.bibtex_keys:
-            value = str(document[bibKey])
-            if not papis.config.get('bibtex-unicode'):
-                value = papis.bibtex.unicode_to_latex(value)
-            if bibKey == 'journal':
-                bibtex_journal_key = papis.config.get('bibtex-journal-key')
-                if bibtex_journal_key in document.keys():
-                    bibtexString += "  %s = {%s},\n" % (
-                        'journal',
-                        papis.bibtex.unicode_to_latex(
-                            str(
-                              document[papis.config.get('bibtex-journal-key')]
-                            )
-                        )
-                    )
-                elif bibtex_journal_key not in document.keys():
-                    logger.warning(
-                        "Key '%s' is not present for ref=%s" % (
-                            papis.config.get('bibtex-journal-key'),
-                            document["ref"]
-                        )
-                    )
-                    bibtexString += "  %s = {%s},\n" % (
-                        'journal',
-                        value
-                    )
-            else:
-                bibtexString += "  %s = {%s},\n" % (
-                    bibKey,
-                    value
-                )
-    bibtexString += "}\n"
-    return bibtexString
+    :returns: A python list
+    :rtype:  list
+    :raises SyntaxError: Whenever the parsed syntax is either not a valid
+        python object or a valid python list.
+    """
+    rawvalue = general_get(key, **kwargs)
+    if isinstance(rawvalue, list):
+        return rawvalue
+    try:
+        value = eval(rawvalue)
+    except Exception as e:
+        raise SyntaxError(
+            "The key '{0}' must be a valid python object\n\t{1}".format(key, e)
+        )
+    else:
+        if not isinstance(value, list):
+            raise SyntaxError(
+                "The key '{0}' must be a valid python list".format(key)
+            )
+        return value
 
 
-def to_json(document):
-    """Export information into a json string
-    :param document: Papis document
-    :type  document: Document
-    :returns: Json formatted info file
-    :rtype:  str
+def get_configuration():
+    """Get the configuration object, if no papis configuration has ever been
+    initialized, it initializes one. Only one configuration per process should
+    ever be configured.
+
+    :returns: Configuration object
+    :rtype:  papis.config.Configuration
+    """
+    global _CONFIGURATION
+    if _CONFIGURATION is None:
+        logger.debug("Creating configuration")
+        _CONFIGURATION = Configuration()
+        # Handle local configuration file, and merge it if it exists
+        local_config_file = papis.config.get("local-config-file")
+        merge_configuration_from_path(local_config_file, _CONFIGURATION)
+    return _CONFIGURATION
 
-    >>> doc = from_data({'title': 'Hello World'})
-    >>> to_json(doc)
-    '{"title": "Hello World"}'
-    """
-    import json
-    return json.dumps(to_dict(document))
-
-
-def to_dict(document):
-    """Gets a python dictionary with the information of the document
-    :param document: Papis document
-    :type  document: Document
-    :returns: Python dictionary
-    :rtype:  dict
-    """
-    result = dict()
-    for key in document.keys():
-        result[key] = document[key]
-    return result
-
-
-def dump(document):
-    """Return information string without any obvious format
-    :param document: Papis document
-    :type  document: Document
-    :returns: String with document's information
-    :rtype:  str
 
-    >>> doc = from_data({'title': 'Hello World'})
-    >>> dump(doc)
-    'title:   Hello World\\n'
-    """
-    string = ""
-    for i in document.keys():
-        string += str(i)+":   "+str(document[i])+"\n"
-    return string
-
-
-def delete(document):
-    """This function deletes a document from disk.
-    :param document: Papis document
-    :type  document: papis.document.Document
-    """
-    import shutil
-    folder = document.get_main_folder()
-    shutil.rmtree(folder)
-
-
-def move(document, path):
-    """This function moves a document to path, it supposes that
-    the document exists in the location ``document.get_main_folder()``.
-    Warning: This method will change the folder in the document object too.
-    :param document: Papis document
-    :type  document: papis.document.Document
-    :param path: Full path where the document will be moved to
+def merge_configuration_from_path(path, configuration):
+    """
+    Merge information of a configuration file found in `path`
+    to the information of the configuration object stored in `configuration`.
+
+    :param path: Path to the configuration file
     :type  path: str
+    :param configuration: Configuration object
+    :type  configuration: papis.config.Configuration
+    """
+    if not os.path.exists(path):
+        return
+    logger.debug("Merging configuration from " + path)
+    configuration.read(path)
+    configuration.handle_includes()
+
+
+def set_lib(library):
+    """Set library
+
+    :param library: Library object
+    :type  library: papis.library.Library
+
+    """
+    global _CURRENT_LIBRARY
+    assert(isinstance(library, papis.library.Library))
+    config = get_configuration()
+    if library.name not in config.keys():
+        config[library.name] = dict(dirs=library.paths)
+    _CURRENT_LIBRARY = library
 
-    >>> doc = from_data({'title': 'Hello World'})
-    >>> doc.set_folder('path/to/folder')
-    >>> import tempfile; newfolder = tempfile.mkdtemp()
-    >>> move(doc, newfolder)
-    Traceback (most recent call last):
-    ...
-    Exception: There is already...
-    """
-    import shutil
-    path = os.path.expanduser(path)
-    if os.path.exists(path):
-        raise Exception(
-            "There is already a document in {0}, please check it,\n"
-            "a temporary papis document has been stored in {1}".format(
-                path, document.get_main_folder()
+
+def set_lib_from_name(libname):
+    """Set library, notice that in principle library can be a full path.
+
+    :param libname: Name of the library or some path to a folder
+    :type  libname: str
+    """
+    assert(isinstance(libname, str))
+    set_lib(get_lib_from_name(libname))
+
+
+def get_lib_from_name(libname):
+    assert(isinstance(libname, str))
+    config = get_configuration()
+    if libname not in config.keys():
+        if os.path.isdir(libname):
+            # Check if the path exists, then use this path as a new library
+            logger.warning(
+                "Since {0} exists, interpreting it as a library".format(
+                    libname
+                )
             )
-        )
-    shutil.move(document.get_main_folder(), path)
-    # Let us chmod it because it might come from a temp folder
-    # and temp folders are per default 0o600
-    os.chmod(path, papis.config.getint('dir-umask'))
-    document.set_folder(path)
-
-
-class DocHtmlEscaped(dict):
-    """
-    Small helper class to escape html elements.
-
-    >>> DocHtmlEscaped(from_data(dict(title='> >< int & "" "')))['title']
-    '&gt; &gt;&lt; int &amp; &quot;&quot; &quot;'
-    """
-
-    def __init__(self, doc):
-        self.doc = doc
-
-    def __getitem__(self, key):
-        return str(self.doc[key]).replace('&', '&amp;')\
-                                .replace('<', '&lt;')\
-                                .replace('>', '&gt;')\
-                                .replace('"', '&quot;')
-
-
-class Document(object):
-
-    """Class implementing the entry abstraction of a document in a library.
-    It is basically a python dictionary with more methods.
-    """
-
-    subfolder = ""
-    _infoFilePath = ""
-
-    def __init__(self, folder=None, data=None):
-        self._keys = []
-        self._folder = None
-
-        if folder is not None:
-            self.set_folder(folder)
-            self.load()
-
-        if data is not None:
-            self.update(data)
-
-    def __delitem__(self, key):
-        """Deletes property from document, e.g. ``del doc['url']``.
-        :param key: Name of the property.
-        :type  key: str
-
-        >>> doc = from_data({'title': 'Hello', 'type': 'book'})
-        >>> del doc['title']
-        >>> doc.has('title')
-        False
-        """
-        self._keys.pop(self._keys.index(key))
-        delattr(self, key)
-
-    def __setitem__(self, key, value):
-        """Sets property to value from document, e.g. ``doc['url'] =
-        'www.gnu.org'``.
-        :param key: Name of the property.
-        :type  key: str
-        :param value: Value of the parameter
-        :type  value: str,int,float,list
-        """
-        self._keys.append(key)
-        setattr(self, key, value)
-
-    def __getitem__(self, key):
-        """Gets property to value from document, e.g. ``a = doc['url']``.
-        If the property `key` does not exist, then the empy string is returned.
-
-        :param key: Name of the property.
-        :type  key: str
-        :returns: Value of the property
-        :rtype:  str,int,float,list
-        """
-        return getattr(self, key) if hasattr(self, key) else ""
-
-    @property
-    def html_escape(self):
-        return DocHtmlEscaped(self)
-
-    def get_main_folder(self):
-        """Get full path for the folder where the document and the information
-        is stored.
-        :returns: Folder path
-        """
-        return self._folder
-
-    def set_folder(self, folder):
-        """Set document's folder. The info_file path will be accordingly set.
-
-        :param folder: Folder where the document will be stored, full path.
-        :type  folder: str
-        """
-        self._folder = folder
-        self._infoFilePath = os.path.join(
-            folder,
-            papis.utils.get_info_file_name()
-        )
-        self.subfolder = self.get_main_folder().replace(
-            os.environ["HOME"], ""
-        ).replace(
-            "/", " "
-        )
+            library_obj = papis.library.from_paths([libname])
+            name = library_obj.path_format()
+            config[name] = dict(dirs=library_obj.paths)
+        else:
+            raise Exception(
+                "Path or library '%s' does not seem to exist" % libname
+            )
+    else:
+        name = libname
+        if name not in config.keys():
+            raise Exception('Library {0} not defined'.format(libname))
+        try:
+            paths = [expanduser(config[name]['dir'])]
+        except KeyError:
+            try:
+                paths = eval(expanduser(config[name].get('dirs')))
+            except SyntaxError as e:
+                raise Exception(
+                    "To define a library you have to set either dir or dirs"
+                    " in the configuration file.\n"
+                    "Error: ({0})".format(e)
+                )
+        library_obj = papis.library.Library(libname, paths)
+    return library_obj
 
-    def get_main_folder_name(self):
-        """Get main folder name where the document and the information is
-        stored.
-        :returns: Folder name
-        """
-        return os.path.basename(self._folder)
-
-    def has(self, key):
-        """Check if the information file has some key defined.
-
-        :param key: Key name to be checked
-        :returns: True/False
-
-        >>> doc = from_data({'title': 'Hello World'})
-        >>> doc.has('title')
-        True
-        >>> doc.has('author')
-        False
-        """
-        return key in self.keys()
-
-    def rm_file(self, filepath):
-        """Remove file from document, it also removes the entry in `files`
-
-        :filepath: Full file path for file
-
-        >>> doc = from_data({'title': 'Hello', 'files': ['a.pdf']})
-        >>> doc.rm_file('b.pdf')
-        Traceback (most recent call last):
-        ...
-        Exception: File b.pdf not tracked by document
-        """
-        basename = os.path.basename(filepath)
-        if basename not in self['files']:
-            raise Exception("File %s not tracked by document" % basename)
-        os.remove(filepath)
-        self['files'].pop(self['files'].index(basename))
-
-    def rm(self):
-        """Removes document's folder, effectively removing it from the library.
-
-        >>> doc = from_data({'title': 'Hello World'})
-        >>> import tempfile; doc.set_folder(tempfile.mkdtemp())
-        >>> doc.rm()
-        """
-        shutil.rmtree(self.get_main_folder())
-
-    def save(self):
-        """Saves the current document's information into the info file.
-        """
-        import yaml
-        fd = open(self._infoFilePath, "w+")
-        structure = dict()
-        for key in self.keys():
-            structure[key] = self[key]
-        # self.logger.debug("Saving %s " % self.get_info_file())
-        yaml.dump(
-            structure,
-            fd,
-            allow_unicode=papis.config.getboolean("info-allow-unicode"),
-            default_flow_style=False
-        )
-        fd.close()
 
-    def update(self, data, force=False, interactive=False):
-        """Update document's information from an info dictionary.
+def get_lib_dirs():
+    """Get the directories of the current library
 
-        :param data: Dictionary with key and values to be updated
-        :type  data: dict
-        :param force: If True, the update turns into a replace, i.e., it
-            replaces the old value by the new value stored in data.
-        :type  force: bool
-        :param interactive: If True, it will ask for user's input every time
-            that the values differ.
-        :type  interactive: bool
-
-        """
-        for key in data.keys():
-            if self[key] != data[key]:
-                if force:
-                    self[key] = data[key]
-                elif interactive:
-                    confirmation = papis.utils.confirm(
-                        "(%s conflict) Replace '%s' by '%s'?" % (
-                            key, self[key], data[key]
+    :returns: A list of paths
+    :rtype:  list
+    """
+    return get_lib().paths
+
+
+def get_lib_name():
+    return get_lib().name
+
+
+def get_lib():
+    """Get current library, if there is no library set before,
+    the default library will be retrieved.
+    If the `PAPIS_LIB` environment variable is defined, this is the
+    library name (or path) that will be taken as a default.
+
+    :returns: Current library
+    :rtype:  papis.library.Library
+    """
+    global _CURRENT_LIBRARY
+    if os.environ.get('PAPIS_LIB'):
+        set_lib_from_name(os.environ['PAPIS_LIB'])
+    if _CURRENT_LIBRARY is None:
+        # Do not put papis.config.get because get is a special function
+        # that also needs the library to see if some key was overridden!
+        lib = papis.config.get_default_settings(key="default-library")
+        set_lib_from_name(lib)
+    assert(isinstance(_CURRENT_LIBRARY, papis.library.Library))
+    return _CURRENT_LIBRARY
+
+
+def reset_configuration():
+    """Destroys existing configuration and returns a new one.
+
+    :returns: Configuration object
+    :rtype:  papis.config.Configuration
+    """
+    global _CONFIGURATION
+    _CONFIGURATION = None
+    logger.debug("Resetting configuration")
+    return get_configuration()
+
+
+class Configuration(configparser.ConfigParser):
+
+    default_info = {
+      "papers": {
+        'dir': '~/Documents/papers'
+      },
+      get_general_settings_name(): {
+        'default-library': 'papers'
+      }
+    }
+
+    def __init__(self):
+        configparser.ConfigParser.__init__(self)
+        self.dir_location = get_config_folder()
+        self.scripts_location = get_scripts_folder()
+        self.file_location = get_config_file()
+        self.logger = logging.getLogger("Configuration")
+        self.initialize()
+
+    def handle_includes(self):
+        if "include" in self.keys():
+            for name in self["include"]:
+                self.logger.debug("including %s" % name)
+                fullpath = os.path.expanduser(self.get("include", name))
+                if os.path.exists(fullpath):
+                    self.read(fullpath)
+                else:
+                    self.logger.warn(
+                        "{0} not included because it does not exist".format(
+                            fullpath
                         )
                     )
-                    if confirmation:
-                        self[key] = data[key]
-                elif self[key] is None or self[key] == '':
-                    self[key] = data[key]
-
-    def get_info_file(self):
-        """Get full path for the info file
-        :returns: Full path for the info file
-        :rtype: str
-        """
-        return self._infoFilePath
-
-    def get_files(self):
-        """Get the files linked to the document, if any.
-
-        :returns: List of full file paths
-        :rtype:  list
-        """
-        files = self["files"] if isinstance(self["files"], list) \
-            else [self["files"]]
-        result = []
-        for f in files:
-            result.append(os.path.join(self.get_main_folder(), f))
-        return result
-
-    def keys(self):
-        """Returns the keys defined for the document.
-
-        :returns: Keys for the document
-        :rtype:  list
-        """
-        return self._keys
-
-    @property
-    def has_citations(self):
-        """Returns string defined in config if keys contains citations
-        else returns None.
-
-        :returns: String or None
-        :rtype: str OR None
-
-        >>> import papis.config
-        >>> doc = from_data({'title': 'Hello World'})
-        >>> doc.has_citations
-        ''
-        >>> doc.update(dict(citations=[]))
-        >>> doc.has_citations == papis.config.get('citation-string')
-        True
-        """
-
-        if 'citations' in self.keys():
-            return papis.config.get('citation-string')
-        else:
-            return ''
 
-    def dump(self):
-        """Return information string without any obvious format
-        :returns: String with document's information
-        :rtype:  str
-
-        >>> doc = from_data({'title': 'Hello World'})
-        >>> doc.dump()
-        'title:   Hello World\\n'
-        """
-        return dump(self)
-
-    def load(self):
-        """Load information from info file
-        """
-        import yaml
-        # TODO: think about if it's better to raise an exception here
-        # TODO: if no info file is found
-        try:
-            fd = open(self.get_info_file(), "r")
-        except:
-            return False
-        try:
-            structure = yaml.load(fd)
-            for key in structure:
-                self[key] = structure[key]
-            fd.close()
-        except Exception as e:
-            logging.error(
-                'Error reading yaml file in {0}'.format(self.get_info_file()) +
-                '\nPlease check it!\n\n{0}'.format(str(e))
+    def initialize(self):
+        if not os.path.exists(self.dir_location):
+            self.logger.warning(
+                'Creating configuration folder in %s' % self.dir_location
             )
-            fd.close()
+            os.makedirs(self.dir_location)
+        if not os.path.exists(self.scripts_location):
+            os.makedirs(self.scripts_location)
+        if os.path.exists(self.file_location):
+            self.logger.debug(
+                'Reading configuration from {0}'.format(self.file_location)
+            )
+            self.read(self.file_location)
+            self.handle_includes()
+        else:
+            for section in self.default_info:
+                self[section] = {}
+                for field in self.default_info[section]:
+                    self[section][field] = self.default_info[section][field]
+            with open(self.file_location, "w") as configfile:
+                self.write(configfile)
+        configpy = get_configpy_file()
+        if os.path.exists(configpy):
+            self.logger.debug('Executing {0}'.format(configpy))
+            with open(configpy) as fd:
+                exec(fd.read())
```

### Comparing `papis-0.8.2/papis/exceptions.py` & `papis-0.9/papis/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 """This module implements custom exceptions used to make the code more
 readable.
 """
 
 
-class SettingNotRegistered(Exception):
-    """This exception is when a setting is to be retrieved that has not been
-    considered beforehand in the code and registered accordingly, thus giving a
-    default value to it"""
-    pass
-
-
 class DefaultSettingValueMissing(Exception):
     """This exception is when a setting's value has no default value.
     """
 
     def __init__(self, key):
         message = """
```

### Comparing `papis-0.8.2/papis/isbn.py` & `papis-0.9/papis/isbn.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 import isbnlib
+import click
+import papis.document
 # See https://github.com/xlcnd/isbnlib for details
 
 logger = logging.getLogger('papis:isbnlib')
 
 
 def get_data(query="", service=None):
     global logger
@@ -26,7 +28,37 @@
     :param data: Dictionary with data
     :type  data: dict
     :returns: Dictionary with papis keynames
 
     """
     data = {k.lower(): data[k] for k in data}
     return data
+
+
+@click.command('isbn')
+@click.pass_context
+@click.help_option('--help', '-h')
+@click.option('--query', '-q', default=None)
+@click.option(
+    '--service',
+    '-s',
+    default='goob',
+    type=click.Choice(['wcat', 'goob', 'openl'])
+)
+def explorer(ctx, query, service):
+    """
+    Look for documents using isbnlib
+
+    Examples of its usage are
+
+    papis explore isbn -q 'Albert einstein' pick cmd 'firefox {doc[url]}'
+
+    """
+    logger = logging.getLogger('explore:isbn')
+    logger.info('Looking up...')
+    data = get_data(
+        query=query,
+        service=service,
+    )
+    docs = [papis.document.from_data(data=d) for d in data]
+    logger.info('{} documents found'.format(len(docs)))
+    ctx.obj['documents'] += docs
```

### Comparing `papis-0.8.2/papis/utils.py` & `papis-0.9/papis/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # -*- coding: utf-8 -*-
-from subprocess import call
-import logging
+import subprocess
+import multiprocessing
+import time
+import copy
 from itertools import count, product
-
-logger = logging.getLogger("utils")
-logger.debug("importing")
-
 import os
 import re
-import papis.api
+import papis.pick
 import papis.config
 import papis.commands
 import papis.document
-import papis.crossref
 import papis.bibtex
 import papis.exceptions
+import logging
+import papis.importer
+import papis.downloaders
+import colorama
+
+logger = logging.getLogger("utils")
+logger.debug("importing")
 
 
 def general_open(fileName, key, default_opener=None, wait=True):
     """Wraper for openers
 
 
     >>> import tempfile; path = tempfile.mktemp()
@@ -39,17 +43,16 @@
     try:
         opener = papis.config.get(key)
     except papis.exceptions.DefaultSettingValueMissing:
         if default_opener is None:
             default_opener = papis.config.get_default_opener()
         opener = default_opener
     if isinstance(fileName, list):
-        fileName = papis.api.pick(fileName)
+        fileName = papis.pick.pick(fileName)
     if isinstance(opener, str):
-        import subprocess
         import shlex
         cmd = shlex.split("{0} '{1}'".format(opener, fileName))
         logger.debug("cmd:  %s" % cmd)
         if wait:
             logger.debug("Waiting for process to finsih")
             return subprocess.call(cmd)
         else:
@@ -60,59 +63,65 @@
             )
     elif hasattr(opener, '__call__'):
         return opener(fileName)
     else:
         raise Warning("How should I use the opener %s?" % opener)
 
 
+def open_file(file_path, wait=True):
+    """Open file using the ``opentool`` key value as a program to
+    handle file_path.
+
+    :param file_path: File path to be handled.
+    :type  file_path: str
+    :param wait: Wait for the completion of the opener program to continue
+    :type  wait: bool
+
+    """
+    general_open(fileName=file_path, key="opentool", wait=wait)
+
+
 def format_doc(python_format, document, key=""):
     """Construct a string using a pythonic format string and a document.
 
     :param python_format: Python-like format string.
         (`see <
             https://docs.python.org/2/library/string.html#format-string-syntax
         >`_)
     :type  python_format: str
     :param document: Papis document
     :type  document: papis.document.Document
     :returns: Formated string
     :rtype: str
     """
     doc = key or papis.config.get("format-doc-name")
-    if papis.config.getboolean('format-jinja2-enable') is True:
-        try:
-            import jinja2
-        except ImportError:
-            logger.error("""
-            You're trying to format strings using jinja2
-            Jinja2 is not installed by default, so just install it
-
-                pip3 install jinja2
-
-            """)
-        else:
-            return jinja2.Template(python_format).render(**{doc: document})
-    return python_format.format(**{doc: document})
+    fdoc = papis.document.Document()
+    fdoc.update(document)
+    try:
+        return python_format.format(**{doc: fdoc})
+    except Exception as e:
+        return str(e)
 
 
 def get_folders(folder):
     """This is the main indexing routine. It looks inside ``folder`` and crawls
     the whole directory structure in search for subfolders containing an info
     file.
 
     :param folder: Folder to look into.
     :type  folder: str
     :returns: List of folders containing an info file.
     :rtype: list
     """
-    logger.debug("Indexing folders")
+    logger.debug("Indexing folders in '{0}'".format(folder))
     folders = list()
     for root, dirnames, filenames in os.walk(folder):
-        if os.path.exists(os.path.join(root, get_info_file_name())):
+        if os.path.exists(os.path.join(root, papis.config.get('info-name'))):
             folders.append(root)
+    logger.debug("{0} valid folders retrieved".format(len(folders)))
     return folders
 
 
 def create_identifier(input_list):
     """This creates a generator object capable of iterating over lists to
     create combinations of that list that result in unique strings.
     Ideally for use in modifying an existing string to make it unique.
@@ -132,47 +141,14 @@
 
     """
     for n in count(1):
         for s in product(input_list, repeat=n):
             yield ''.join(s)
 
 
-def get_info_file_name():
-    """Get the name of the general info file for any document
-
-    :returns: Name of the file.
-    :rtype: str
-    """
-    return papis.config.get("info-name")
-
-
-def doi_to_data(doi):
-    """Try to get from a DOI expression a dictionary with the document's data
-    using the crossref module.
-
-    :param doi: DOI expression.
-    :type  doi: str
-    :returns: Document's data
-    :rtype: dict
-    """
-    return papis.crossref.doi_to_data(doi)
-
-
-def yaml_to_data(yaml_path):
-    """Convert a yaml file into a dictionary using the yaml module.
-
-    :param yaml_path: Path to a yaml file
-    :type  yaml_path: str
-    :returns: Dictionary containing the info of the yaml file
-    :rtype:  dict
-    """
-    import yaml
-    return yaml.load(open(yaml_path))
-
-
 def confirm(prompt, yes=True, bottom_toolbar=None):
     """Confirm with user input
 
     :param prompt: Question or text that the user gets.
     :type  prompt: str
     :param yes: If yes should be the default.
     :type  yes: bool
@@ -186,15 +162,15 @@
         default='Y/n' if yes else 'y/N',
         validator_function=lambda x: x in 'YyNn',
         dirty_message='Please, write either "y" or "n" to confirm'
     )
     if yes:
         return result not in 'Nn'
     else:
-        return result not in 'Yy'
+        return result in 'Yy'
 
 
 def text_area(title, text, lexer_name="", height=10, full_screen=False):
     """
     Small implementation of an editor/pager for small pieces of text.
 
     :param title: Title of the text_area
@@ -209,15 +185,17 @@
     :param full_screen: Wether or not the text area should be full screen.
     :type  full_screen: bool
     """
     from prompt_toolkit import Application
     from prompt_toolkit.enums import EditingMode
     from prompt_toolkit.buffer import Buffer
     from prompt_toolkit.layout.containers import HSplit, Window, WindowAlign
-    from prompt_toolkit.layout.controls import BufferControl, FormattedTextControl
+    from prompt_toolkit.layout.controls import (
+        BufferControl, FormattedTextControl
+    )
     from prompt_toolkit.layout.layout import Layout
     from prompt_toolkit.layout import Dimension
     from prompt_toolkit.key_binding import KeyBindings
     from prompt_toolkit.lexers import PygmentsLexer
     from pygments.lexers import find_lexer_class_by_name
     assert(type(title) == str)
     assert(type(text) == str)
@@ -242,35 +220,36 @@
 
     text_height = Dimension(min=0, max=height) if height is not None else None
 
     pygment_lexer = find_lexer_class_by_name(lexer_name)
     lexer = PygmentsLexer(pygment_lexer)
     text_window = Window(
         height=text_height,
+        style='bg:black fg:ansiwhite',
         content=BufferControl(buffer=buffer1, lexer=lexer)
     )
 
     root_container = HSplit([
         Window(
-            char='-',
-            align=WindowAlign.CENTER,
+            align=WindowAlign.LEFT,
+            style='bg:ansiwhite',
             height=1,
             content=FormattedTextControl(
                 text=[('fg:ansiblack bg:ansiwhite', title)]
             ),
             always_hide_cursor=True
         ),
 
         text_window,
 
         Window(
             height=1,
             width=None,
-            align=WindowAlign.CENTER,
-            char='-',
+            align=WindowAlign.LEFT,
+            style='bg:ansiwhite',
             content=FormattedTextControl(
                 text=[(
                     'fg:ansiblack bg:ansiwhite',
                     "Quit [Ctrl-q]  Save [Ctrl-s]"
                 )]
             )
         ),
@@ -288,15 +267,14 @@
         ), layout=layout, key_bindings=kb, full_screen=full_screen
     )
     app.run()
     return app.return_text
 
 
 def yes_no_dialog(title, text):
-    from prompt_toolkit.formatted_text import HTML
     from prompt_toolkit.shortcuts import yes_no_dialog
     from prompt_toolkit.styles import Style
 
     example_style = Style.from_dict({
         'dialog': 'bg:#88ff88',
         'dialog frame-label': 'bg:#ffffff #000000',
         'dialog.body': 'bg:#000000 #00ff00',
@@ -306,54 +284,70 @@
     return yes_no_dialog(
         title=title,
         text=text,
         style=example_style
     )
 
 
-def input(prompt, default="", bottom_toolbar=None, multiline=False, 
+def input(
+        prompt, default="", bottom_toolbar=None, multiline=False,
         validator_function=None, dirty_message=""):
     """Prompt user for input
 
     :param prompt: Question or text that the user gets.
     :type  prompt: str
     :param default: Default value to give if the user does not input anything
     :type  default: str
     :returns: User input or default
     :rtype:  bool
 
     """
     import prompt_toolkit
-    from prompt_toolkit.validation import Validator
+    import prompt_toolkit.validation
     if validator_function is not None:
-        validator = Validator.from_callable(
+        validator = prompt_toolkit.validation.Validator.from_callable(
             validator_function,
             error_message=dirty_message,
             move_cursor_to_end=True
         )
     else:
         validator = None
-
-    fragments = [
-        ('', prompt),
-        ('fg:red', ' ({0})'.format(default)),
-        ('', ': '),
-    ]
+    if isinstance(prompt, str):
+        fragments = [
+            ('', prompt),
+            ('fg:red', ' ({0})'.format(default)),
+            ('', ': '),
+        ]
+    else:
+        fragments = prompt
 
     result = prompt_toolkit.prompt(
         fragments,
         validator=validator,
         multiline=multiline,
         bottom_toolbar=bottom_toolbar,
         validate_while_typing=True
     )
 
     return result if result else default
 
 
+def update_doc_from_data_interactively(document, data, data_name):
+    import papis.tui.widgets.diff
+    docdata = copy.copy(document)
+    # do not compare some entries
+    docdata.pop('files', None)
+    docdata.pop('tags', None)
+    document.update(
+        papis.tui.widgets.diff.diffdict(
+            docdata,
+            data,
+            namea=papis.document.describe(document), nameb=data_name))
+
+
 def clean_document_name(doc_path):
     """Get a file path and return the basename of the path cleaned.
 
     It will also turn chinese, french, russian etc into ascii characters.
 
     :param doc_path: Path of a document.
     :type  doc_path: str
@@ -366,34 +360,14 @@
     return slugify.slugify(
         os.path.basename(doc_path),
         word_boundary=True,
         regex_pattern=regex_pattern
     )
 
 
-def git_commit(path="", message=""):
-    """Commits changes in the path with a message.
-    If the path is not given, then the lib path is used.
-
-    :param path: Folder where a git repo exists.
-    :type  path: str
-    :param message: Commit message
-    :type  message: str
-    :returns: None
-
-    """
-    logger.debug('Commiting...')
-    path = path or os.path.expanduser(papis.config.get('dir'))
-    message = '-m "%s"' % message if len(message) > 0 else ''
-    cmd = ['git', '-C', path, 'commit', message]
-    logger.debug(cmd)
-    message = '-m "%s"' % message if len(message) > 0 else ''
-    call(cmd)
-
-
 def locate_document_in_lib(document, library=None):
     """Try to figure out if a document is already in a library
 
     :param document: Document to be searched for
     :type  document: papis.document.Document
     :param library: Name of a valid papis library
     :type  library: str
@@ -445,7 +419,86 @@
     filetype.guess(document_path)
     kind = filetype.guess(document_path)
     if kind is None:
         m = re.match(r"^.*\.([^.]+)$", os.path.basename(document_path))
         return m.group(1) if m else 'data'
     else:
         return kind.extension
+
+
+def folders_to_documents(folders):
+    """Turn folders into documents, this is done in a multiprocessing way, this
+    step is quite critical for performance.
+
+    :param folders: List of folder paths.
+    :type  folders: list
+    :returns: List of document objects.
+    :rtype:  list
+    """
+    logger = logging.getLogger("utils:dir2doc")
+    np = multiprocessing.cpu_count()
+    logger.debug("converting folder into documents on {0} cores".format(np))
+    pool = multiprocessing.Pool(np)
+    begin_t = time.time()
+    result = pool.map(papis.document.from_folder, folders)
+    pool.close()
+    pool.join()
+    logger.debug("done in %.1f ms" % (1000*time.time()-1000*begin_t))
+    return result
+
+
+def get_cache_home():
+    """Get folder where the cache files are stored, it retrieves the
+    ``cache-dir`` configuration setting. It is ``XDG`` standard compatible.
+
+    :returns: Full path for cache main folder
+    :rtype:  str
+
+    """
+    user_defined = papis.config.get('cache-dir')
+    if user_defined is not None:
+        path = os.path.expanduser(user_defined)
+    else:
+        path = os.path.expanduser(
+            os.path.join(os.environ.get('XDG_CACHE_HOME'), 'papis')
+        ) if os.environ.get(
+            'XDG_CACHE_HOME'
+        ) else os.path.expanduser(
+            os.path.join('~', '.cache', 'papis')
+        )
+    if not os.path.exists(path):
+        os.makedirs(path)
+    return path
+
+
+def geturl(url):
+    """Quick and dirty file get request utility.
+    """
+    assert(isinstance(url, str))
+    import requests
+    session = requests.Session()
+    session.headers = {'User-Agent': papis.config.get('user-agent')}
+    return session.get(url).content
+
+
+def get_matching_importer_or_downloader(matching_string):
+    importers = []
+    logger = logging.getLogger("utils:matcher")
+    for importer_cls in (papis.importer.get_importers() +
+                         papis.downloaders.get_downloaders()):
+        importer = importer_cls.match(matching_string)
+        logger.debug(
+            "trying with importer {c.Back.BLACK}{c.Fore.YELLOW}{name}"
+            "{c.Style.RESET_ALL}".format(
+                c=colorama, name=importer_cls))
+        if importer:
+            logger.info(
+                "{f} {c.Back.BLACK}{c.Fore.GREEN}matches {name}"
+                "{c.Style.RESET_ALL}".format(
+                    f=matching_string, c=colorama, name=importer.name))
+            try:
+                importer.fetch()
+            except Exception as e:
+                logger.error(e)
+            else:
+                importers.append(importer)
+    return importers
```

### Comparing `papis-0.8.2/papis.egg-info/PKG-INFO` & `papis-0.9/papis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: papis
-Version: 0.8.2
+Version: 0.9
 Summary: Powerful and highly extensible command-line based document and bibliography manager
 Home-page: https://github.com/papis/papis
 Author: Alejandro Gallo
 Author-email: aamsgallo@gmail.com
 Maintainer: Alejandro Gallo
 Maintainer-email: aamsgallo@gmail.com
 License: GPLv3
-Description: Papis |Build_Status| |Coveralls| |RTD| |Pypi| |Code_Quality| |zenodo_badge|
+Description: Papis
         =====
         
+        |PyPI-Versions| |Build_Status| |Coveralls| |RTD| |Pypi|
+        |Code_Quality| |zenodo_badge| |PyPI-Downloads|
+        
         |Packaging_status|
         
         Description
         -----------
         
         Papis is a powerful and highly extensible command-line based document
         and bibliography manager.
@@ -40,17 +43,16 @@
            account, nowhere, never.
         -  Download directly paper information from *DOI* number via *Crossref*.
         -  (optional) **scihub** support, use the example papis script
            ``examples/scripts/papis-scihub`` to download papers from scihub and
            add them to your library with all the relevant information, in a
            matter of seconds, also you can check the documentation
            `here <http://papis.readthedocs.io/en/latest/scihub.html>`__.
-        -  Import from Zotero and other managers using the script in
-           ``examples/scripts/papis-zotero``
-           (`doc <http://papis.readthedocs.io/en/latest/importing.html>`__).
+        -  Import from Zotero and other managers using
+           `papis-zotero <https://github.com/papis/papis-zotero>_`.
         -  Create custom scripts to help you achieve great tasks easily
            (`doc <http://papis.readthedocs.io/en/latest/scripting.html>`__).
         -  Export documents into many formats (bibtex, yaml..)
         -  Command-line granularity, all the power of a library at the tip of
            your fingers.
         
         Contributing
@@ -132,14 +134,27 @@
            :target: https://travis-ci.org/papis/papis
         .. |Packaging_status| image:: https://repology.org/badge/vertical-allrepos/papis.svg
            :target: https://repology.org/metapackage/papis
         .. |asciicast_help| image:: https://asciinema.org/a/3otatlbqXIsI102uAywMhT4fP.png
            :target: https://asciinema.org/a/3otatlbqXIsI102uAywMhT4fP
         .. |Code_Quality| image:: https://img.shields.io/lgtm/grade/python/g/papis/papis.svg?logo=lgtm&logoWidth=18
            :target: https://lgtm.com/projects/g/papis/papis/context:python
+        .. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/papis.svg?label=pypi%20downloads&logo=python&logoColor=white
+           :target: https://pypi.org/project/papis
+        .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/papis.svg?logo=python&logoColor=white
+           :target: https://pypi.org/project/papis
+        
+        Related software
+        ----------------
+        
+        Here is a list of similar software:
+        
+        - `Mendeley <https://www.mendeley.com/>`__ Proprietary.
+        - `Zotero <https://www.zotero.org/>`__ FOSS
+        - `Xapers <https://finestructure.net/xapers/>`__.
         
 Keywords: document,crossref,libgen,scihub,physics,mathematics,books,papers,science,research,bibtex,latex,command-line,tui,biblatex,pubmed,ieee,reference manager,mendeley,zotero,elsevier,cli,biliography,datasheets
 Platform: linux
 Platform: osx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `papis-0.8.2/papis.egg-info/SOURCES.txt` & `papis-0.9/papis.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -30,28 +30,36 @@
 papis/cli.py
 papis/config.py
 papis/crossref.py
 papis/dissemin.py
 papis/docmatcher.py
 papis/document.py
 papis/exceptions.py
+papis/git.py
+papis/importer.py
 papis/isbn.py
 papis/isbnplus.py
-papis/main.py
+papis/json.py
+papis/library.py
 papis/pick.py
+papis/plugin.py
+papis/pubmed.py
+papis/strings.py
 papis/utils.py
+papis/yaml.py
 papis.egg-info/PKG-INFO
 papis.egg-info/SOURCES.txt
 papis.egg-info/dependency_links.txt
 papis.egg-info/entry_points.txt
 papis.egg-info/requires.txt
 papis.egg-info/top_level.txt
 papis/commands/__init__.py
 papis/commands/add.py
 papis/commands/addto.py
+papis/commands/bibtex.py
 papis/commands/browse.py
 papis/commands/config.py
 papis/commands/default.py
 papis/commands/edit.py
 papis/commands/explore.py
 papis/commands/export.py
 papis/commands/external.py
@@ -67,26 +75,28 @@
 papis/database/base.py
 papis/database/cache.py
 papis/database/whoosh.py
 papis/downloaders/__init__.py
 papis/downloaders/acs.py
 papis/downloaders/annualreviews.py
 papis/downloaders/aps.py
-papis/downloaders/arxiv.py
 papis/downloaders/base.py
+papis/downloaders/fallback.py
 papis/downloaders/frontiersin.py
 papis/downloaders/get.py
 papis/downloaders/hal.py
 papis/downloaders/ieee.py
 papis/downloaders/iopscience.py
-papis/downloaders/libgen.py
+papis/downloaders/sciencedirect.py
 papis/downloaders/scitationaip.py
+papis/downloaders/springer.py
+papis/downloaders/tandfonline.py
 papis/downloaders/thesesfr.py
-papis/downloaders/utils.py
 papis/downloaders/worldscientific.py
 papis/tui/__init__.py
 papis/tui/app.py
-papis/tui/utils.py
 papis/tui/widgets/__init__.py
 papis/tui/widgets/command_line_prompt.py
+papis/tui/widgets/diff.py
 papis/tui/widgets/list.py
-scripts/shell_completion/click/papis.sh
+scripts/shell_completion/click/papis.sh
+scripts/shell_completion/click/zsh/_papis
```

### Comparing `papis-0.8.2/scripts/shell_completion/click/papis.sh` & `papis-0.9/scripts/shell_completion/click/papis.sh`

 * *Files identical despite different names*

### Comparing `papis-0.8.2/AUTHORS` & `papis-0.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `papis-0.8.2/LICENSE.txt` & `papis-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `papis-0.8.2/README.rst` & `papis-0.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-Papis |Build_Status| |Coveralls| |RTD| |Pypi| |Code_Quality| |zenodo_badge|
+Papis
 =====
 
+|PyPI-Versions| |Build_Status| |Coveralls| |RTD| |Pypi|
+|Code_Quality| |zenodo_badge| |PyPI-Downloads|
+
 |Packaging_status|
 
 Description
 -----------
 
 Papis is a powerful and highly extensible command-line based document
 and bibliography manager.
@@ -30,17 +33,16 @@
    account, nowhere, never.
 -  Download directly paper information from *DOI* number via *Crossref*.
 -  (optional) **scihub** support, use the example papis script
    ``examples/scripts/papis-scihub`` to download papers from scihub and
    add them to your library with all the relevant information, in a
    matter of seconds, also you can check the documentation
    `here <http://papis.readthedocs.io/en/latest/scihub.html>`__.
--  Import from Zotero and other managers using the script in
-   ``examples/scripts/papis-zotero``
-   (`doc <http://papis.readthedocs.io/en/latest/importing.html>`__).
+-  Import from Zotero and other managers using
+   `papis-zotero <https://github.com/papis/papis-zotero>_`.
 -  Create custom scripts to help you achieve great tasks easily
    (`doc <http://papis.readthedocs.io/en/latest/scripting.html>`__).
 -  Export documents into many formats (bibtex, yaml..)
 -  Command-line granularity, all the power of a library at the tip of
    your fingers.
 
 Contributing
@@ -122,7 +124,20 @@
    :target: https://travis-ci.org/papis/papis
 .. |Packaging_status| image:: https://repology.org/badge/vertical-allrepos/papis.svg
    :target: https://repology.org/metapackage/papis
 .. |asciicast_help| image:: https://asciinema.org/a/3otatlbqXIsI102uAywMhT4fP.png
    :target: https://asciinema.org/a/3otatlbqXIsI102uAywMhT4fP
 .. |Code_Quality| image:: https://img.shields.io/lgtm/grade/python/g/papis/papis.svg?logo=lgtm&logoWidth=18
    :target: https://lgtm.com/projects/g/papis/papis/context:python
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/papis.svg?label=pypi%20downloads&logo=python&logoColor=white
+   :target: https://pypi.org/project/papis
+.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/papis.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/papis
+
+Related software
+----------------
+
+Here is a list of similar software:
+
+- `Mendeley <https://www.mendeley.com/>`__ Proprietary.
+- `Zotero <https://www.zotero.org/>`__ FOSS
+- `Xapers <https://finestructure.net/xapers/>`__.
```

### Comparing `papis-0.8.2/PKG-INFO` & `papis-0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: papis
-Version: 0.8.2
+Version: 0.9
 Summary: Powerful and highly extensible command-line based document and bibliography manager
 Home-page: https://github.com/papis/papis
 Author: Alejandro Gallo
 Author-email: aamsgallo@gmail.com
 Maintainer: Alejandro Gallo
 Maintainer-email: aamsgallo@gmail.com
 License: GPLv3
-Description: Papis |Build_Status| |Coveralls| |RTD| |Pypi| |Code_Quality| |zenodo_badge|
+Description: Papis
         =====
         
+        |PyPI-Versions| |Build_Status| |Coveralls| |RTD| |Pypi|
+        |Code_Quality| |zenodo_badge| |PyPI-Downloads|
+        
         |Packaging_status|
         
         Description
         -----------
         
         Papis is a powerful and highly extensible command-line based document
         and bibliography manager.
@@ -40,17 +43,16 @@
            account, nowhere, never.
         -  Download directly paper information from *DOI* number via *Crossref*.
         -  (optional) **scihub** support, use the example papis script
            ``examples/scripts/papis-scihub`` to download papers from scihub and
            add them to your library with all the relevant information, in a
            matter of seconds, also you can check the documentation
            `here <http://papis.readthedocs.io/en/latest/scihub.html>`__.
-        -  Import from Zotero and other managers using the script in
-           ``examples/scripts/papis-zotero``
-           (`doc <http://papis.readthedocs.io/en/latest/importing.html>`__).
+        -  Import from Zotero and other managers using
+           `papis-zotero <https://github.com/papis/papis-zotero>_`.
         -  Create custom scripts to help you achieve great tasks easily
            (`doc <http://papis.readthedocs.io/en/latest/scripting.html>`__).
         -  Export documents into many formats (bibtex, yaml..)
         -  Command-line granularity, all the power of a library at the tip of
            your fingers.
         
         Contributing
@@ -132,14 +134,27 @@
            :target: https://travis-ci.org/papis/papis
         .. |Packaging_status| image:: https://repology.org/badge/vertical-allrepos/papis.svg
            :target: https://repology.org/metapackage/papis
         .. |asciicast_help| image:: https://asciinema.org/a/3otatlbqXIsI102uAywMhT4fP.png
            :target: https://asciinema.org/a/3otatlbqXIsI102uAywMhT4fP
         .. |Code_Quality| image:: https://img.shields.io/lgtm/grade/python/g/papis/papis.svg?logo=lgtm&logoWidth=18
            :target: https://lgtm.com/projects/g/papis/papis/context:python
+        .. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/papis.svg?label=pypi%20downloads&logo=python&logoColor=white
+           :target: https://pypi.org/project/papis
+        .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/papis.svg?logo=python&logoColor=white
+           :target: https://pypi.org/project/papis
+        
+        Related software
+        ----------------
+        
+        Here is a list of similar software:
+        
+        - `Mendeley <https://www.mendeley.com/>`__ Proprietary.
+        - `Zotero <https://www.zotero.org/>`__ FOSS
+        - `Xapers <https://finestructure.net/xapers/>`__.
         
 Keywords: document,crossref,libgen,scihub,physics,mathematics,books,papers,science,research,bibtex,latex,command-line,tui,biblatex,pubmed,ieee,reference manager,mendeley,zotero,elsevier,cli,biliography,datasheets
 Platform: linux
 Platform: osx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

