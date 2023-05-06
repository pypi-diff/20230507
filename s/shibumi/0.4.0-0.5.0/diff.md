# Comparing `tmp/shibumi-0.4.0.tar.gz` & `tmp/shibumi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shibumi-0.4.0.tar", last modified: Sun Nov 15 23:19:33 2020, max compression
+gzip compressed data, was "shibumi-0.5.0.tar", last modified: Sat May  6 22:59:16 2023, max compression
```

## Comparing `shibumi-0.4.0.tar` & `shibumi-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,65 @@
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.998347 shibumi-0.4.0/
--rw-rw-r--   0 don       (1000) don       (1000)     4786 2020-11-15 23:19:32.998347 shibumi-0.4.0/PKG-INFO
--rw-rw-r--   0 don       (1000) don       (1000)     3391 2020-10-07 00:02:59.000000 shibumi-0.4.0/README.md
--rw-rw-r--   0 don       (1000) don       (1000)       38 2020-11-15 23:19:32.998347 shibumi-0.4.0/setup.cfg
--rw-rw-r--   0 don       (1000) don       (1000)     2154 2020-11-13 06:09:47.000000 shibumi-0.4.0/setup.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.686318 shibumi-0.4.0/shibumi/
--rw-rw-r--   0 don       (1000) don       (1000)       22 2020-11-15 23:18:46.000000 shibumi-0.4.0/shibumi/__init__.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.710320 shibumi-0.4.0/shibumi/margo/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-09-10 05:22:12.000000 shibumi-0.4.0/shibumi/margo/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)      326 2020-10-22 01:45:36.000000 shibumi-0.4.0/shibumi/margo/display.py
--rw-rw-r--   0 don       (1000) don       (1000)      351 2020-11-15 16:12:44.000000 shibumi-0.4.0/shibumi/margo/state.py
--rw-rw-r--   0 don       (1000) don       (1000)       46 2020-08-13 05:51:36.000000 shibumi-0.4.0/shibumi/play_shibumi.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.742323 shibumi-0.4.0/shibumi/sandbox/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-10-05 01:01:40.000000 shibumi-0.4.0/shibumi/sandbox/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)      323 2020-10-19 19:54:19.000000 shibumi-0.4.0/shibumi/sandbox/display.py
--rw-rw-r--   0 don       (1000) don       (1000)     2795 2020-11-13 04:15:51.000000 shibumi-0.4.0/shibumi/sandbox/game.py
--rw-rw-r--   0 don       (1000) don       (1000)      900 2020-09-27 15:24:27.000000 shibumi-0.4.0/shibumi/shibumi.py
--rw-rw-r--   0 don       (1000) don       (1000)    22397 2020-11-14 18:36:33.000000 shibumi-0.4.0/shibumi/shibumi_display.py
--rw-rw-r--   0 don       (1000) don       (1000)     8911 2020-11-15 03:29:06.000000 shibumi-0.4.0/shibumi/shibumi_display_ui.py
--rw-rw-r--   0 don       (1000) don       (1000)    16902 2020-11-14 05:37:35.000000 shibumi-0.4.0/shibumi/shibumi_game_state.py
--rw-rw-r--   0 don       (1000) don       (1000)   889093 2020-10-18 19:37:14.000000 shibumi-0.4.0/shibumi/shibumi_images_rc.py
--rw-rw-r--   0 don       (1000) don       (1000)     7923 2020-11-15 23:07:29.000000 shibumi-0.4.0/shibumi/shibumi_rules_rc.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.802328 shibumi-0.4.0/shibumi/spaiji/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-10-20 04:14:31.000000 shibumi-0.4.0/shibumi/spaiji/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)     1352 2020-10-22 01:42:17.000000 shibumi-0.4.0/shibumi/spaiji/display.py
--rw-rw-r--   0 don       (1000) don       (1000)     7980 2020-10-23 02:54:26.000000 shibumi-0.4.0/shibumi/spaiji/game.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.830331 shibumi-0.4.0/shibumi/spargo/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-09-10 05:22:12.000000 shibumi-0.4.0/shibumi/spargo/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)      610 2020-10-29 04:26:07.000000 shibumi-0.4.0/shibumi/spargo/display.py
--rw-rw-r--   0 don       (1000) don       (1000)     6386 2020-10-29 04:31:44.000000 shibumi-0.4.0/shibumi/spargo/game.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.894337 shibumi-0.4.0/shibumi/spire/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-10-31 15:44:57.000000 shibumi-0.4.0/shibumi/spire/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)     1031 2020-11-01 22:14:43.000000 shibumi-0.4.0/shibumi/spire/display.py
--rw-rw-r--   0 don       (1000) don       (1000)     6897 2020-11-03 02:07:58.000000 shibumi-0.4.0/shibumi/spire/state.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.934341 shibumi-0.4.0/shibumi/spline/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-08-13 05:51:36.000000 shibumi-0.4.0/shibumi/spline/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)      537 2020-10-23 20:44:20.000000 shibumi-0.4.0/shibumi/spline/display.py
--rw-rw-r--   0 don       (1000) don       (1000)     1672 2020-09-27 03:05:31.000000 shibumi-0.4.0/shibumi/spline/game.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.958343 shibumi-0.4.0/shibumi/spook/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-11-13 04:22:16.000000 shibumi-0.4.0/shibumi/spook/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)     1009 2020-11-15 23:07:27.000000 shibumi-0.4.0/shibumi/spook/display.py
--rw-rw-r--   0 don       (1000) don       (1000)    10901 2020-11-15 01:31:46.000000 shibumi-0.4.0/shibumi/spook/state.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.978345 shibumi-0.4.0/shibumi/utils/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-08-13 05:51:36.000000 shibumi-0.4.0/shibumi/utils/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)     1216 2020-09-13 22:54:17.000000 shibumi-0.4.0/shibumi/utils/headcount.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 23:19:32.686318 shibumi-0.4.0/shibumi.egg-info/
--rwxrwxrwx   0 don       (1000) don       (1000)     4786 2020-11-15 23:19:31.000000 shibumi-0.4.0/shibumi.egg-info/PKG-INFO
--rwxrwxrwx   0 don       (1000) don       (1000)      995 2020-11-15 23:19:31.000000 shibumi-0.4.0/shibumi.egg-info/SOURCES.txt
--rwxrwxrwx   0 don       (1000) don       (1000)        1 2020-11-15 23:19:31.000000 shibumi-0.4.0/shibumi.egg-info/dependency_links.txt
--rwxrwxrwx   0 don       (1000) don       (1000)      388 2020-11-15 23:19:31.000000 shibumi-0.4.0/shibumi.egg-info/entry_points.txt
--rwxrwxrwx   0 don       (1000) don       (1000)       79 2020-11-15 23:19:31.000000 shibumi-0.4.0/shibumi.egg-info/requires.txt
--rwxrwxrwx   0 don       (1000) don       (1000)        8 2020-11-15 23:19:31.000000 shibumi-0.4.0/shibumi.egg-info/top_level.txt
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.311577 shibumi-0.5.0/
+-rw-rw-r--   0 don       (1000) don       (1000)      329 2022-04-06 22:49:25.000000 shibumi-0.5.0/LICENSE
+-rw-rw-r--   0 don       (1000) don       (1000)     4188 2023-05-06 22:59:16.311577 shibumi-0.5.0/PKG-INFO
+-rw-rw-r--   0 don       (1000) don       (1000)     3467 2023-04-13 03:25:44.000000 shibumi-0.5.0/README.md
+-rw-rw-r--   0 don       (1000) don       (1000)       38 2023-05-06 22:59:16.311577 shibumi-0.5.0/setup.cfg
+-rw-rw-r--   0 don       (1000) don       (1000)     2258 2023-05-01 18:49:00.000000 shibumi-0.5.0/setup.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.303577 shibumi-0.5.0/shibumi/
+-rw-rw-r--   0 don       (1000) don       (1000)       22 2023-05-06 22:58:36.000000 shibumi-0.5.0/shibumi/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)     9099 2023-05-02 05:01:08.000000 shibumi-0.5.0/shibumi/diagram_writer.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.307577 shibumi-0.5.0/shibumi/margo/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/margo/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      328 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/margo/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)      372 2023-04-25 05:11:40.000000 shibumi-0.5.0/shibumi/margo/state.py
+-rw-rw-r--   0 don       (1000) don       (1000)       46 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/play_shibumi.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.307577 shibumi-0.5.0/shibumi/sandbox/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/sandbox/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      323 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/sandbox/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2807 2022-04-07 04:59:49.000000 shibumi-0.5.0/shibumi/sandbox/game.py
+-rw-rw-r--   0 don       (1000) don       (1000)      899 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/shibumi.py
+-rw-rw-r--   0 don       (1000) don       (1000)    22557 2023-04-25 05:11:40.000000 shibumi-0.5.0/shibumi/shibumi_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     8911 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/shibumi_display_ui.py
+-rw-rw-r--   0 don       (1000) don       (1000)    17097 2023-04-25 05:08:48.000000 shibumi-0.5.0/shibumi/shibumi_game_state.py
+-rw-rw-r--   0 don       (1000) don       (1000)   889093 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/shibumi_images_rc.py
+-rw-rw-r--   0 don       (1000) don       (1000)  1694195 2023-05-02 06:08:58.000000 shibumi-0.5.0/shibumi/shibumi_rules_rc.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.307577 shibumi-0.5.0/shibumi/spaiji/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spaiji/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1354 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spaiji/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     8006 2023-04-25 05:11:40.000000 shibumi-0.5.0/shibumi/spaiji/game.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.307577 shibumi-0.5.0/shibumi/spargo/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spargo/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      612 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spargo/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     6407 2023-04-25 05:11:40.000000 shibumi-0.5.0/shibumi/spargo/game.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.311577 shibumi-0.5.0/shibumi/sparks/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2023-05-01 16:14:43.000000 shibumi-0.5.0/shibumi/sparks/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1052 2023-05-02 02:13:08.000000 shibumi-0.5.0/shibumi/sparks/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     6657 2023-05-06 22:26:28.000000 shibumi-0.5.0/shibumi/sparks/state.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.311577 shibumi-0.5.0/shibumi/spire/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spire/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1033 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spire/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     6935 2023-04-25 05:11:40.000000 shibumi-0.5.0/shibumi/spire/state.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.311577 shibumi-0.5.0/shibumi/spline/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spline/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      539 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spline/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1672 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spline/game.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.311577 shibumi-0.5.0/shibumi/sploof/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/sploof/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      658 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/sploof/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     8225 2023-04-25 05:11:40.000000 shibumi-0.5.0/shibumi/sploof/state.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.311577 shibumi-0.5.0/shibumi/spook/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spook/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1017 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/spook/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)    11221 2023-04-25 05:11:40.000000 shibumi-0.5.0/shibumi/spook/state.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.311577 shibumi-0.5.0/shibumi/utils/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/utils/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1216 2022-04-06 22:49:25.000000 shibumi-0.5.0/shibumi/utils/headcount.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.307577 shibumi-0.5.0/shibumi.egg-info/
+-rw-rw-r--   0 don       (1000) don       (1000)     4188 2023-05-06 22:59:16.000000 shibumi-0.5.0/shibumi.egg-info/PKG-INFO
+-rw-rw-r--   0 don       (1000) don       (1000)     1219 2023-05-06 22:59:16.000000 shibumi-0.5.0/shibumi.egg-info/SOURCES.txt
+-rw-rw-r--   0 don       (1000) don       (1000)        1 2023-05-06 22:59:16.000000 shibumi-0.5.0/shibumi.egg-info/dependency_links.txt
+-rw-rw-r--   0 don       (1000) don       (1000)      479 2023-05-06 22:59:16.000000 shibumi-0.5.0/shibumi.egg-info/entry_points.txt
+-rw-rw-r--   0 don       (1000) don       (1000)       64 2023-05-06 22:59:16.000000 shibumi-0.5.0/shibumi.egg-info/requires.txt
+-rw-rw-r--   0 don       (1000) don       (1000)       14 2023-05-06 22:59:16.000000 shibumi-0.5.0/shibumi.egg-info/top_level.txt
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:59:16.311577 shibumi-0.5.0/tests/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-06 22:49:25.000000 shibumi-0.5.0/tests/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      278 2022-04-06 22:49:25.000000 shibumi-0.5.0/tests/conftest.py
```

### Comparing `shibumi-0.4.0/PKG-INFO` & `shibumi-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
 Metadata-Version: 2.1
 Name: shibumi
-Version: 0.4.0
+Version: 0.5.0
 Summary: Simple board games hiding complexity
 Home-page: https://donkirkby.github.io/shibumi-games/
 Author: Don Kirkby
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/donkirkby/shibumi-games/issues
 Project-URL: Source, https://github.com/donkirkby/shibumi-games
-Description: # Shibumi Games [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
-        ### Simple board games hiding complexity
-        
-        [Build Badge]: https://travis-ci.org/donkirkby/shibumi-games.svg?branch=master
-        [build]: https://travis-ci.org/donkirkby/shibumi-games
-        [Coverage Badge]: https://codecov.io/github/donkirkby/shibumi-games/coverage.svg?branch=master
-        [codecov]: https://codecov.io/github/donkirkby/shibumi-games?branch=master
-        [PyPI Badge]: https://badge.fury.io/py/shibumi.svg
-        [pypi]: https://badge.fury.io/py/shibumi
-        [screenshot]: https://donkirkby.github.io/shibumi-games/images/demo.png
-        [journal]: https://donkirkby.github.io/shibumi-games/journal
-        
-        Play board games that use the [Shibumi] game system of marbles stacked on a 4x4
-        board, build computer opponents for those games, learn strategy, and analyse the
-        structure of the games.
-        
-        ![screenshot]
-        
-        ## Installing Shibumi Games
-        Even though Shibumi Games has a graphical display, it is a regular Python package,
-        so you can install it with `pip install shibumi`. If you haven't installed
-        Python packages before, read Brett Cannon's [quick-and-dirty guide].
-        
-        Then run it with the `shibumi` command.
-        
-        The default installation generates some errors about `bdist_wheel` that don't
-        seem to actually cause any problems. You can either ignore them, or install
-        `wheel` before installing Shibumi Games.
-        
-            pip install wheel
-            pip install shibumi
-            shibumi
-        
-        Known bug on Ubuntu 20.04:
-        
-        > qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though
-        > it was found.
-        
-        This is a [PySide2 bug] that is missing some dependencies. You can work around
-        it by installing those dependencies like this:
-        
-            sudo apt install libxcb-xinerama0
-        
-        [quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
-        [PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
-        
-        ### Game Credits
-        The Shibumi game system was designed by Cameron Browne and Néstor Romeral
-        Andrés. The complete set of games rules are available on the
-        [nestorgames web site], and the games used in this project are used with the
-        generous permission of the designers. There are more games in a [BGG list].
-        * Spline was designed by Néstor Romeral Andrés.
-        * Spaiji was designed by Néstor Romeral Andrés.
-        * Sploof was designed by Matt Green, and took first place in the Shibumi
-        Challenge.
-        * Spargo and Margo were designed by Cameron Browne.
-        * Spire was designed by Dieter Stein, and took second place in the Shibumi
-        Challenge.
-        
-        [nestorgames web site]: https://nestorgames.com/shibumibook_detail.html
-        [BGG list]: https://boardgamegeek.com/boardgamefamily/13434/series-shibumi/linkeditems/boardgamefamily?pageid=1&sort=usersrated
-        
-        ### Image Credits
-        The marble and board graphics were designed by Cameron Browne, and are used with
-        permission.
-        
-        Some of the buttons combine Cameron's POV-Ray graphics with icons from the
-        [Open Iconic] project.
-        
-        [Open Iconic]: https://useiconic.com/open
-        
-        ## More Information
-        If you'd like to help out with the project, or add your own games, see the
-        `CONTRIBUTING.md` file in the source code. For all the details, look through the
-        design [journal] for the project.
-        
-        Shibumi games are built on top of the [Zero Play library] that you can use to
-        build your own games.
-        
-        [Shibumi]: https://boardgamegeek.com/boardgame/135270/shibumi
-        [Zero Play library]: https://donkirkby.github.io/zero-play/
-        
 Keywords: boardgames alphazero machine learning mcts shibumi
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ml
 Provides-Extra: ml-gpu
+License-File: LICENSE
+
+# Shibumi Games [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
+### Simple board games hiding complexity
+
+[Build Badge]: https://github.com/donkirkby/shibumi-games/actions/workflows/py-build.yml/badge.svg?branch=master
+[build]: https://github.com/donkirkby/shibumi-games/actions
+[Coverage Badge]: https://codecov.io/github/donkirkby/shibumi-games/coverage.svg?branch=master
+[codecov]: https://codecov.io/github/donkirkby/shibumi-games?branch=master
+[PyPI Badge]: https://badge.fury.io/py/shibumi.svg
+[pypi]: https://badge.fury.io/py/shibumi
+[screenshot]: https://donkirkby.github.io/shibumi-games/images/demo.png
+[journal]: https://donkirkby.github.io/shibumi-games/journal
+
+Play board games that use the [Shibumi] game system of marbles stacked on a 4x4
+board, build computer opponents for those games, learn strategy, and analyse the
+structure of the games.
+
+![screenshot]
+
+## Installing Shibumi Games
+Even though Shibumi Games has a graphical display, it is a regular Python package,
+so you can install it with `pip install shibumi`. If you haven't installed
+Python packages before, read Brett Cannon's [quick-and-dirty guide].
+
+Then run it with the `shibumi` command.
+
+The default installation generates some errors about `bdist_wheel` that don't
+seem to actually cause any problems. You can either ignore them, or install
+`wheel` before installing Shibumi Games.
+
+    pip install wheel
+    pip install shibumi
+    shibumi
+
+Known bug on Ubuntu 20.04:
+
+> qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though
+> it was found.
+
+This is a [PySide2 bug] that is missing some dependencies. You can work around
+it by installing those dependencies like this:
+
+    sudo apt install libxcb-xinerama0
+
+[quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
+[PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
+
+### Game Credits
+The Shibumi game system was designed by Cameron Browne and Néstor Romeral
+Andrés. The complete set of game rules are available on the
+[nestorgames web site], and the games used in this project are used with the
+generous permission of the designers. There are more games in a [BGG list].
+* Spaiji was designed by Néstor Romeral Andrés.
+* Spargo and Margo were designed by Cameron Browne.
+* Spire was designed by Dieter Stein, and took second place in the Shibumi
+Challenge.
+* Spline was designed by Néstor Romeral Andrés.
+* Sploof was designed by Matt Green, and took first place in the Shibumi
+Challenge.
+* Spook was designed by Dieter Stein.
+
+[nestorgames web site]: https://nestorgames.com/shibumibook_detail.html
+[BGG list]: https://boardgamegeek.com/boardgamefamily/13434/series-shibumi/linkeditems/boardgamefamily?pageid=1&sort=usersrated
+
+### Image Credits
+The marble and board graphics were designed by Cameron Browne, and are used with
+permission.
+
+Some of the buttons combine Cameron's POV-Ray graphics with icons from the
+[Open Iconic] project.
+
+[Open Iconic]: https://useiconic.com/open
+
+## More Information
+If you'd like to help out with the project, or add your own games, see the
+`CONTRIBUTING.md` file in the source code. For all the details, look through the
+design [journal] for the project.
+
+Shibumi games are built on top of the [Zero Play library] that you can use to
+build your own games.
+
+[Shibumi]: https://boardgamegeek.com/boardgame/135270/shibumi
+[Zero Play library]: https://donkirkby.github.io/zero-play/
```

### Comparing `shibumi-0.4.0/README.md` & `shibumi-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Shibumi Games [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
 ### Simple board games hiding complexity
 
-[Build Badge]: https://travis-ci.org/donkirkby/shibumi-games.svg?branch=master
-[build]: https://travis-ci.org/donkirkby/shibumi-games
+[Build Badge]: https://github.com/donkirkby/shibumi-games/actions/workflows/py-build.yml/badge.svg?branch=master
+[build]: https://github.com/donkirkby/shibumi-games/actions
 [Coverage Badge]: https://codecov.io/github/donkirkby/shibumi-games/coverage.svg?branch=master
 [codecov]: https://codecov.io/github/donkirkby/shibumi-games?branch=master
 [PyPI Badge]: https://badge.fury.io/py/shibumi.svg
 [pypi]: https://badge.fury.io/py/shibumi
 [screenshot]: https://donkirkby.github.io/shibumi-games/images/demo.png
 [journal]: https://donkirkby.github.io/shibumi-games/journal
 
@@ -42,24 +42,25 @@
     sudo apt install libxcb-xinerama0
 
 [quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
 [PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
 
 ### Game Credits
 The Shibumi game system was designed by Cameron Browne and Néstor Romeral
-Andrés. The complete set of games rules are available on the
+Andrés. The complete set of game rules are available on the
 [nestorgames web site], and the games used in this project are used with the
 generous permission of the designers. There are more games in a [BGG list].
-* Spline was designed by Néstor Romeral Andrés.
 * Spaiji was designed by Néstor Romeral Andrés.
-* Sploof was designed by Matt Green, and took first place in the Shibumi
-Challenge.
 * Spargo and Margo were designed by Cameron Browne.
 * Spire was designed by Dieter Stein, and took second place in the Shibumi
 Challenge.
+* Spline was designed by Néstor Romeral Andrés.
+* Sploof was designed by Matt Green, and took first place in the Shibumi
+Challenge.
+* Spook was designed by Dieter Stein.
 
 [nestorgames web site]: https://nestorgames.com/shibumibook_detail.html
 [BGG list]: https://boardgamegeek.com/boardgamefamily/13434/series-shibumi/linkeditems/boardgamefamily?pageid=1&sort=usersrated
 
 ### Image Credits
 The marble and board graphics were designed by Cameron Browne, and are used with
 permission.
```

### Comparing `shibumi-0.4.0/setup.py` & `shibumi-0.5.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,25 +25,27 @@
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'Topic :: Games/Entertainment :: Board Games',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3.8'],
       keywords='boardgames alphazero machine learning mcts shibumi',
       packages=setuptools.find_packages(),
-      install_requires=['zero-play', 'numpy<1.19.0', 'PySide2'],
+      install_requires=['zero-play', 'numpy'],
       extras_require={'ml': ['zero-play[ml]'],
                       'ml-gpu': ['zero-play[ml-gpu]']},
       entry_points={
           'gui_scripts': ['shibumi=shibumi.shibumi:main'],
           # The game_display entry point lets you add screens for new games.
           # The zero_play.game_display.GameDisplay class is a useful base class.
           'zero_play.game_display': [
               'margo=shibumi.margo.display:MargoDisplay',
               'sandbox=shibumi.sandbox.display:SandboxDisplay',
               'spaiji=shibumi.spaiji.display:SpaijiDisplay',
               'spargo=shibumi.spargo.display:SpargoDisplay',
+              'sparks=shibumi.sparks.display:SparksDisplay',
               'spire=shibumi.spire.display:SpireDisplay',
               'spook=shibumi.spook.display:SpookDisplay',
+              'sploof=shibumi.sploof.display:SploofDisplay',
               'spline=shibumi.spline.display:SplineDisplay']},
       project_urls={
           'Bug Reports': 'https://github.com/donkirkby/shibumi-games/issues',
           'Source': 'https://github.com/donkirkby/shibumi-games'})
```

### Comparing `shibumi-0.4.0/shibumi/sandbox/game.py` & `shibumi-0.5.0/shibumi/sandbox/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         else:
             new_board.remove(height, row, column)
         return new_board
 
     def get_valid_moves(self) -> np.ndarray:
         valid_spaces = super().get_valid_moves()
         volume = self.calculate_volume(self.size)
-        valid_moves = np.ndarray(volume*4, dtype=bool)
+        valid_moves: np.ndarray = np.ndarray(volume*4, dtype=bool)
         for section in range(3):
             valid_moves[section*volume:(section+1)*volume] = valid_spaces
 
         # Removal section
         section_start = volume*3
         levels = self.get_levels()
         for move_index in range(volume):
```

### Comparing `shibumi-0.4.0/shibumi/shibumi.py` & `shibumi-0.5.0/shibumi/shibumi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import typing
 
-from PySide2.QtWidgets import QApplication
+from PySide6.QtWidgets import QApplication
 from pkg_resources import EntryPoint
 
 from zero_play.zero_play import ZeroPlayWindow
 
 
 class ShibumiWindow(ZeroPlayWindow):
     icon_path = ":/shibumi_images/main_icon.png"
@@ -24,12 +24,12 @@
                 yield entry_point
 
 
 def main():
     app = QApplication(sys.argv)
     window = ShibumiWindow()
     window.show()
-    return app.exec_()
+    return app.exec()
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `shibumi-0.4.0/shibumi/shibumi_display.py` & `shibumi-0.5.0/shibumi/shibumi_display.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 from math import floor
 
-from PySide2.QtCore import QSize
-from PySide2.QtCore import Qt
-from PySide2.QtGui import QImage, QPixmap, QFont, QResizeEvent, QPainter
-from PySide2.QtWidgets import (QGraphicsPixmapItem, QGraphicsSceneHoverEvent,
+from PySide6.QtCore import QSize
+from PySide6.QtCore import Qt
+from PySide6.QtGui import QImage, QPixmap, QFont, QResizeEvent, QPainter
+from PySide6.QtWidgets import (QGraphicsPixmapItem, QGraphicsSceneHoverEvent,
                                QGraphicsSceneMouseEvent, QGraphicsScene)
 
 from shibumi.shibumi_display_ui import Ui_ShibumiDisplay
 from shibumi.shibumi_game_state import ShibumiGameState, MoveType, PlayerCode
 from zero_play.game_display import GameDisplay, center_text_item
 from zero_play.game_state import GameState
 from shibumi import shibumi_images_rc
@@ -126,15 +126,15 @@
                  self.ui.white_count_pixmap),
                 (PlayerCode.RED,
                  self.red_pixmap,
                  self.ui.red_count_pixmap)):
             if code in value:
                 count_pixmap.setPixmap(pixmap)
             else:
-                count_pixmap.setPixmap(None)
+                count_pixmap.setPixmap(QPixmap())
         self.update_count_text()
 
     @property
     def show_counts(self) -> bool:
         return bool(self.visible_counts)
 
     @show_counts.setter
@@ -216,15 +216,15 @@
         right_width = round(full_width * 0.279)
         top_height = round(full_height * 0.28)
         mid_height = round(full_height * 0.21)
         bottom_height = round(full_height * 0.29)
         final_width = left_width+(board_size-2)*mid_width+right_width
         final_height = top_height+(board_size-2)*mid_height+bottom_height
         assembled_board = QPixmap(final_width, final_height)
-        assembled_board.fill(Qt.transparent)
+        assembled_board.fill(Qt.GlobalColor.transparent)
         assembled_painter = QPainter(assembled_board)
         # top left
         assembled_painter.drawPixmap(0, 0,
                                      left_width, top_height,
                                      full_board,
                                      0, 0,
                                      left_width, top_height)
@@ -340,19 +340,21 @@
             self.update_move_text(self.choose_active_text())
         if displayed_player == game_state.WHITE:
             self.ui.player_pixmap.setPixmap(self.white_pixmap)
         elif displayed_player == game_state.BLACK:
             self.ui.player_pixmap.setPixmap(self.black_pixmap)
         elif displayed_player == game_state.RED:
             self.ui.player_pixmap.setPixmap(self.red_pixmap)
+        if displayed_player is not None:
+            displayed_player = int(displayed_player)
         self.ui.player_pixmap.setVisible(displayed_player != game_state.NO_PLAYER)
         if self.show_counts:
             self.update_count_text()
 
-    def update_move_text(self, text: str = None):
+    def update_move_text(self, text: str | None = None):
         if self.debug_message:
             self.ui.move_text.setText(self.debug_message)
         elif text is not None:
             self.ui.move_text.setText(text)
     
     def scene(self) -> QGraphicsScene:
         return self.ui.game_display.scene()
@@ -439,16 +441,16 @@
                 count.setText('')
 
     @staticmethod
     def scale_pixmap(pixmap: QPixmap, width: int, height: int):
         scaled_pixmap = pixmap.scaled(
             width,
             height,
-            Qt.KeepAspectRatio,
-            Qt.SmoothTransformation)
+            Qt.AspectRatioMode.KeepAspectRatio,
+            Qt.TransformationMode.SmoothTransformation)
         return scaled_pixmap
 
     def on_hover_enter(self, piece_item: GraphicsShibumiPieceItem):
         assert isinstance(self.current_state, ShibumiGameState)
         if not self.can_move():
             return
         levels = self.current_state.get_levels()
@@ -486,15 +488,15 @@
                                                 piece_item.column,
                                                 self.selected_move_type)
         valid_moves = self.current_state.get_valid_moves()
         if valid_moves[move_index]:
             self.make_move(move_index)
 
     @staticmethod
-    def load_pixmap(name: str, size: QSize = None) -> QPixmap:
+    def load_pixmap(name: str, size: QSize | None = None) -> QPixmap:
         file_path = ':/shibumi_images/' + name
         image = QImage(str(file_path))
         if image.isNull():
             raise ValueError(f'Unable to load image {file_path}.')
         pixmap = QPixmap(image)
         if size is not None:
             pixmap = ShibumiDisplay.scale_pixmap(pixmap,
```

### Comparing `shibumi-0.4.0/shibumi/shibumi_display_ui.py` & `shibumi-0.5.0/shibumi/shibumi_display_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 ## Form generated from reading UI file 'shibumi_display_ui.ui'
 ##
 ## Created by: Qt User Interface Compiler version 5.15.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide2.QtCore import (QCoreApplication, QDate, QDateTime, QMetaObject,
+from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QMetaObject,
     QObject, QPoint, QRect, QSize, QTime, QUrl, Qt)
-from PySide2.QtGui import (QBrush, QColor, QConicalGradient, QCursor, QFont,
+from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor, QFont,
     QFontDatabase, QIcon, QKeySequence, QLinearGradient, QPalette, QPainter,
     QPixmap, QRadialGradient)
-from PySide2.QtWidgets import *
+from PySide6.QtWidgets import *
 
 from zero_play.scaled_label import ScaledLabel
 from zero_play.scaled_radio_button import ScaledRadioButton
 
 
 class Ui_ShibumiDisplay(object):
     def setupUi(self, ShibumiDisplay):
```

### Comparing `shibumi-0.4.0/shibumi/shibumi_game_state.py` & `shibumi-0.5.0/shibumi/shibumi_game_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,31 +33,34 @@
     display_characters = {BLACK: 'B',
                           WHITE: 'W',
                           RED: 'R',
                           GameState.NO_PLAYER: '.',
                           UNUSABLE: ' '}
 
     def __init__(self,
-                 text: str = None,
-                 board: np.ndarray = None,
+                 text: str | None = None,
+                 board: np.ndarray | None = None,
                  size: int = 4):
         self.size = size
         if board is None:
-            r = np.arange(self.size, dtype=np.int8)
-            heights = r.reshape((self.size, 1, 1))
-            rows = r.reshape((1, self.size, 1))
-            columns = r.reshape((1, 1, self.size))
-            level_sizes = self.size - heights
-            levels = self.UNUSABLE * np.logical_or(rows >= level_sizes,
-                                                   columns >= level_sizes)
+            levels = self.UNUSABLE * np.logical_not(self.get_usable_positions())
             board = levels
             if text is not None:
                 self.load_text(text, levels)
         self.board = board
 
+    def get_usable_positions(self):
+        r = np.arange(self.size, dtype=np.int8)
+        heights = r.reshape((self.size, 1, 1))
+        rows = r.reshape((1, self.size, 1))
+        columns = r.reshape((1, 1, self.size))
+        level_sizes = self.size - heights
+        is_usablex = np.logical_and(rows < level_sizes, columns < level_sizes)
+        return is_usablex
+
     def __eq__(self, other):
         if not isinstance(other, ShibumiGameState):
             return False
         return np.array_equal(self.board, other.board)
 
     def load_text(self, text: str, levels: np.ndarray):
         character_players = {
@@ -225,15 +228,15 @@
                                                  overpass_row2,
                                                  overpass_col2]
                         if (overpass_piece1 != no_player and
                                 overpass_piece2 != no_player):
                             continue
             yield neighbour_height, neighbour_row, neighbour_column
 
-    def calculate_volume(self, base_size: int = None):
+    def calculate_volume(self, base_size: int | None = None):
         if base_size is None:
             base_size = self.size
         return base_size * (base_size + 1) * (2 * base_size + 1) // 6
 
     def display(self, show_coordinates: bool = False) -> str:
         levels = self.get_levels()
         lines = []
@@ -274,24 +277,29 @@
     def display_coordinates(height, row, column):
         row_text = str(height + 1 + 2*row)
         column_text = chr(height + 65 + column*2)
         return row_text + column_text
 
     def get_move_count(self) -> int:
         """ The number of moves that have already been made in the start_state. """
-        pieces = self.board.reshape(self.size * self.size * self.size)
+        pieces = self.exclude_end_spaces()
         return sum(piece in (self.WHITE, self.BLACK)
                    for piece in pieces)
 
     def get_piece_count(self, player: int) -> int:
-        end_spaces = self.size * self.size - 1
-        spaces = self.board.reshape(self.size*self.size*self.size)[:-end_spaces]
+        spaces = self.exclude_end_spaces()
         player_count = (spaces == player).sum()
         return player_count
 
+    def exclude_end_spaces(self):
+        end_space_count = self.size * self.size - 1
+        all_spaces = self.board.reshape(self.size * self.size * self.size)
+        spaces = all_spaces[:-end_space_count]
+        return spaces
+
     def get_spaces(self) -> np.ndarray:
         """ Extract the board spaces from the complete game state. """
         return self.get_levels()
 
     def get_index(self, height: int,
                   row: int = 0,
                   column: int = 0,
```

### Comparing `shibumi-0.4.0/shibumi/shibumi_images_rc.py` & `shibumi-0.5.0/shibumi/shibumi_images_rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Resource object code (Python 3)
 # Created by: object code
 # Created by: The Resource Compiler for Qt version 5.15.0
 # WARNING! All changes made in this file will be lost!
 
-from PySide2 import QtCore
+from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x01(\
 <\
 !DOCTYPE RCC><RC\
 C version=\x221.0\x22>\
 \x0a<qresource>\x0a<fi\
```

### Comparing `shibumi-0.4.0/shibumi/spaiji/display.py` & `shibumi-0.5.0/shibumi/spaiji/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from shibumi.shibumi_display import ShibumiDisplay
 from shibumi.shibumi_game_state import MoveType
 from shibumi.spaiji.game import SpaijiState
 from zero_play.game_state import GameState
 
 
 class SpaijiDisplay(ShibumiDisplay):
-    rules_path = ':/shibumi_rules/spaiji.md'
+    rules_path = ':/shibumi_rules/spaiji.html'
 
     def __init__(self):
         super().__init__(SpaijiState())
         self.visible_counts = (self.start_state.BLACK, self.start_state.WHITE)
         self.visible_move_types = (MoveType.BLACK, MoveType.WHITE)
 
     def update_board(self, game_state: GameState):
```

### Comparing `shibumi-0.4.0/shibumi/spaiji/game.py` & `shibumi-0.5.0/shibumi/spaiji/game.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from shibumi.shibumi_game_state import ShibumiGameState, MoveType
 
 
 class SpaijiState(ShibumiGameState):
     game_name = 'Spaiji'
 
     def __init__(self,
-                 text: str = None,
-                 board: np.ndarray = None,
+                 text: str | None = None,
+                 board: np.ndarray | None = None,
                  size: int = 4):
         if text is None:
             player = self.WHITE
             move_text = ''
         else:
             lines = text.splitlines()
             player_text = lines.pop()
@@ -85,15 +85,15 @@
         else:
             levels[-1, -1, -2] = -1
             levels[-1, -1, -1] *= -1
         return new_board
 
     def get_valid_moves(self) -> np.ndarray:
         volume = self.calculate_volume()
-        valid_moves = np.ndarray(2*volume, bool)
+        valid_moves: np.ndarray = np.ndarray(2*volume, bool)
         valid_spaces = valid_moves[:volume]
         self.fill_supported_moves(valid_spaces)
         levels = self.get_levels()
         old_height, old_row, old_column = levels[-1, -1, 0:3]
         if old_column < 0:
             # This is the first move of the turn
             for move, is_valid in enumerate(valid_spaces):
```

### Comparing `shibumi-0.4.0/shibumi/spargo/display.py` & `shibumi-0.5.0/shibumi/spargo/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from shibumi.shibumi_display import ShibumiDisplay
 from shibumi.shibumi_game_state import PlayerCode
 from shibumi.spargo.game import SpargoState
 
 
 class SpargoDisplay(ShibumiDisplay):
-    rules_path = ':/shibumi_rules/spargo.md'
+    rules_path = ':/shibumi_rules/spargo.html'
 
     def __init__(self, size: int = 4):
         super().__init__(SpargoState(size=size))
         self.visible_counts = PlayerCode.BLACK, PlayerCode.WHITE
 
     @property
     def credit_pairs(self) -> typing.Iterable[typing.Tuple[str, str]]:
```

### Comparing `shibumi-0.4.0/shibumi/spargo/game.py` & `shibumi-0.5.0/shibumi/spargo/game.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 class IllegalMoveError(Exception):
     """ Raised when a requested move is not allowed. """
     pass
 
 
 class SpargoState(ShibumiGameState):
     def __init__(self,
-                 text: str = None,
-                 board: np.ndarray = None,
+                 text: str | None = None,
+                 board: np.ndarray | None = None,
                  size: int = 4,
-                 history: typing.Set[bytes] = None):
+                 history: typing.Set[bytes] | None = None):
         if text is None:
             player = self.BLACK
         else:
             text = text.rstrip()
             player_text = text[-2:]
             if not player_text[0] == '>':
                 player = self.BLACK
```

### Comparing `shibumi-0.4.0/shibumi/spire/display.py` & `shibumi-0.5.0/shibumi/spire/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from shibumi.shibumi_display import ShibumiDisplay
 from shibumi.spire.state import SpireState
 from zero_play.game_state import GameState
 
 
 class SpireDisplay(ShibumiDisplay):
-    rules_path = ':/shibumi_rules/spire.md'
+    rules_path = ':/shibumi_rules/spire.html'
 
     def __init__(self):
         start_state = SpireState()
         super().__init__(start_state)
         self.visible_move_types = (start_state.BLACK,
                                    start_state.RED,
                                    start_state.WHITE)
```

### Comparing `shibumi-0.4.0/shibumi/spire/state.py` & `shibumi-0.5.0/shibumi/spire/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from shibumi.shibumi_game_state import ShibumiGameState, MoveType
 
 
 class SpireState(ShibumiGameState):
     game_name = 'Spire'
 
-    def __init__(self, text: str = None, board: np.ndarray = None):
+    def __init__(self, text: str | None = None, board: np.ndarray | None = None):
         """ Initialize a board state.
 
         :param text: a text representation, like that from display()
         :param board: a copy of the board state from another instance; the last
             position holds the current player, and the second last is RED if a
             red ball has not been played this turn, and NO_PLAYER if one has
         """
@@ -64,15 +64,15 @@
         return colour_display + space_display
 
     def get_active_player(self) -> int:
         return self.board[-1, -1, -1]
 
     def get_valid_moves(self) -> np.ndarray:
         volume = self.calculate_volume(self.size)
-        valid_moves = np.ndarray(volume * 2, bool)
+        valid_moves: np.ndarray = np.ndarray(volume * 2, bool)
         player_moves = valid_moves[:volume]
         self.fill_supported_moves(player_moves)
 
         board = self.board
         player = board[-1, -1, -1]
         red_move = board[-1, -1, -2]
         if red_move == self.NO_PLAYER:
@@ -87,15 +87,15 @@
             self.winner = -player
         self.is_end_checked = True
         return valid_moves
 
     def check_colour_matches(self, valid_moves: np.ndarray, colour: int):
         levels = self.get_levels()
         size = self.size
-        match_counts = np.ndarray(levels.shape, np.int8)
+        match_counts: np.ndarray = np.ndarray(levels.shape, np.int8)
         indexes = self.get_used_indexes(size)
         # Look for matching neighbours within each 2x2 square.
         # delta = dst - src
         for dr in (-1, 1):
             src_row1 = (1 + dr) // 2
             src_row2 = size - (1 - dr) // 2
             dst_row1 = (1 - dr) // 2
```

### Comparing `shibumi-0.4.0/shibumi/spline/display.py` & `shibumi-0.5.0/shibumi/spline/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import shibumi
 from shibumi.shibumi_display import ShibumiDisplay
 from shibumi.spline.game import SplineState
 
 
 class SplineDisplay(ShibumiDisplay):
-    rules_path = ':/shibumi_rules/spline.md'
+    rules_path = ':/shibumi_rules/spline.html'
 
     def __init__(self):
         super().__init__(SplineState())
 
     @property
     def credit_pairs(self) -> typing.Iterable[typing.Tuple[str, str]]:
         return [('Spline Game:', 'Néstor Romeral Andrés'),
```

### Comparing `shibumi-0.4.0/shibumi/spline/game.py` & `shibumi-0.5.0/shibumi/spline/game.py`

 * *Files identical despite different names*

### Comparing `shibumi-0.4.0/shibumi/spook/display.py` & `shibumi-0.5.0/shibumi/spook/display.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from shibumi.shibumi_display import ShibumiDisplay
 from shibumi.spook.state import SpookState
 from zero_play.game_state import GameState
 
 
 class SpookDisplay(ShibumiDisplay):
-    rules_path = ':/shibumi_rules/spook.md'
+    rules_path = ':/shibumi_rules/spook.html'
 
     def __init__(self):
         super().__init__(SpookState())
         self.ui.pass_button.clicked.connect(self.make_pass_move)
 
     def update_board(self, game_state: GameState):
         assert isinstance(game_state, SpookState)
         super().update_board(game_state)
         valid_moves = game_state.get_valid_moves()
         volume = game_state.calculate_volume()
-        is_pass_valid = valid_moves[volume]
+        is_pass_valid = bool(valid_moves[volume])
         self.ui.pass_button.setVisible(is_pass_valid)
 
     def make_pass_move(self):
         volume = self.start_state.calculate_volume()
         self.make_move(volume)
 
     @property
```

### Comparing `shibumi-0.4.0/shibumi/spook/state.py` & `shibumi-0.5.0/shibumi/spook/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
+import typing
 
 from shibumi.shibumi_game_state import ShibumiGameState, PlayerCode
 
 
 class SpookState(ShibumiGameState):
     game_name = 'Spook'
     players = (ShibumiGameState.RED, ShibumiGameState.BLACK)
 
     def __init__(self,
-                 text: str = None,
-                 board: np.ndarray = None,
+                 text: str | None = None,
+                 board: np.ndarray | None = None,
                  size: int = 4):
         super().__init__(text, board, size)
         if board is None:
             if text is None:
                 active_player = self.RED
                 move_line = None
             else:
@@ -65,14 +66,17 @@
 
         display += f'>{player_display}{allowed_display}\n'
         return display
 
     def get_active_player(self) -> int:
         return self.board[-1, -1, -1]
 
+    def get_players(self) -> typing.Iterable[int]:
+        return self.BLACK, self.RED
+
     def make_move(self, move: int) -> 'ShibumiGameState':
         player = self.get_active_player()
         volume = self.calculate_volume()
         new_player = self.BLACK if player == self.RED else self.RED
         move_count = self.get_move_count() + 1
         restricted_colour = self.board[-1, -1, -3]
         if restricted_colour == self.UNUSABLE:
@@ -106,18 +110,21 @@
             new_state.remove(*move_coordinates)
             ghost_coordinates = new_state.find_ghost()
             restricted_colour = self.NO_PLAYER
             if ghost_coordinates != move_coordinates:
                 # This wasn't a ghost drop.
                 is_neighbour_captured = False
                 if new_board[move_coordinates] == self.NO_PLAYER:
-                    ghost_distance = sum(abs(a-b)
-                                         for a, b in zip(ghost_coordinates,
-                                                         move_coordinates))
-                    is_neighbour_captured = ghost_distance == 1
+                    if removed_piece == self.NO_PLAYER:
+                        is_neighbour_captured = False
+                    else:
+                        ghost_distance = sum(abs(a-b)
+                                             for a, b in zip(ghost_coordinates,
+                                                             move_coordinates))
+                        is_neighbour_captured = ghost_distance == 1
                     if is_neighbour_captured or removed_piece == self.NO_PLAYER:
                         # Move ghost.
                         new_board[ghost_coordinates] = self.NO_PLAYER
                         new_board[move_coordinates] = self.WHITE
 
                 if is_neighbour_captured:
                     # Check if more matching neighbours are available.
@@ -139,15 +146,15 @@
 
         new_board[-1, -1, -1] = new_player
         new_board[-1, -1, -2] = move_count
         new_board[-1, -1, -3] = restricted_colour
         return new_state
 
     def get_move_count(self) -> int:
-        return self.board[-1, -1, -2]
+        return int(self.board[-1, -1, -2])
 
     def get_valid_moves(self) -> np.ndarray:
         volume = self.calculate_volume(self.size)
         valid_moves = np.full(volume+1, False)
         if self.is_win(self.RED) or self.is_win(self.BLACK):
             return valid_moves
 
@@ -219,17 +226,17 @@
                     if piece == opponent:
                         if self.is_pinned(height, row, column):
                             continue
                         move = self.get_index(height, row, column)
                         valid_moves[move] = True
         return valid_moves
 
-    def find_ghost(self):
+    def find_ghost(self) -> typing.Tuple[int, int, int]:
         ghost_locations: np.ndarray = np.argwhere(self.board == self.WHITE)
-        return tuple(ghost_locations[0])
+        return tuple(ghost_locations[0])  # type: ignore
 
     def is_win(self, player: int) -> bool:
         if self.board[-1, -1, -3] == self.UNUSABLE:
             return False
         pieces = self.get_piece_count(player)
         return pieces == 0
```

### Comparing `shibumi-0.4.0/shibumi/utils/headcount.py` & `shibumi-0.5.0/shibumi/utils/headcount.py`

 * *Files identical despite different names*

### Comparing `shibumi-0.4.0/shibumi.egg-info/PKG-INFO` & `shibumi-0.5.0/shibumi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
 Metadata-Version: 2.1
 Name: shibumi
-Version: 0.4.0
+Version: 0.5.0
 Summary: Simple board games hiding complexity
 Home-page: https://donkirkby.github.io/shibumi-games/
 Author: Don Kirkby
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/donkirkby/shibumi-games/issues
 Project-URL: Source, https://github.com/donkirkby/shibumi-games
-Description: # Shibumi Games [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
-        ### Simple board games hiding complexity
-        
-        [Build Badge]: https://travis-ci.org/donkirkby/shibumi-games.svg?branch=master
-        [build]: https://travis-ci.org/donkirkby/shibumi-games
-        [Coverage Badge]: https://codecov.io/github/donkirkby/shibumi-games/coverage.svg?branch=master
-        [codecov]: https://codecov.io/github/donkirkby/shibumi-games?branch=master
-        [PyPI Badge]: https://badge.fury.io/py/shibumi.svg
-        [pypi]: https://badge.fury.io/py/shibumi
-        [screenshot]: https://donkirkby.github.io/shibumi-games/images/demo.png
-        [journal]: https://donkirkby.github.io/shibumi-games/journal
-        
-        Play board games that use the [Shibumi] game system of marbles stacked on a 4x4
-        board, build computer opponents for those games, learn strategy, and analyse the
-        structure of the games.
-        
-        ![screenshot]
-        
-        ## Installing Shibumi Games
-        Even though Shibumi Games has a graphical display, it is a regular Python package,
-        so you can install it with `pip install shibumi`. If you haven't installed
-        Python packages before, read Brett Cannon's [quick-and-dirty guide].
-        
-        Then run it with the `shibumi` command.
-        
-        The default installation generates some errors about `bdist_wheel` that don't
-        seem to actually cause any problems. You can either ignore them, or install
-        `wheel` before installing Shibumi Games.
-        
-            pip install wheel
-            pip install shibumi
-            shibumi
-        
-        Known bug on Ubuntu 20.04:
-        
-        > qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though
-        > it was found.
-        
-        This is a [PySide2 bug] that is missing some dependencies. You can work around
-        it by installing those dependencies like this:
-        
-            sudo apt install libxcb-xinerama0
-        
-        [quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
-        [PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
-        
-        ### Game Credits
-        The Shibumi game system was designed by Cameron Browne and Néstor Romeral
-        Andrés. The complete set of games rules are available on the
-        [nestorgames web site], and the games used in this project are used with the
-        generous permission of the designers. There are more games in a [BGG list].
-        * Spline was designed by Néstor Romeral Andrés.
-        * Spaiji was designed by Néstor Romeral Andrés.
-        * Sploof was designed by Matt Green, and took first place in the Shibumi
-        Challenge.
-        * Spargo and Margo were designed by Cameron Browne.
-        * Spire was designed by Dieter Stein, and took second place in the Shibumi
-        Challenge.
-        
-        [nestorgames web site]: https://nestorgames.com/shibumibook_detail.html
-        [BGG list]: https://boardgamegeek.com/boardgamefamily/13434/series-shibumi/linkeditems/boardgamefamily?pageid=1&sort=usersrated
-        
-        ### Image Credits
-        The marble and board graphics were designed by Cameron Browne, and are used with
-        permission.
-        
-        Some of the buttons combine Cameron's POV-Ray graphics with icons from the
-        [Open Iconic] project.
-        
-        [Open Iconic]: https://useiconic.com/open
-        
-        ## More Information
-        If you'd like to help out with the project, or add your own games, see the
-        `CONTRIBUTING.md` file in the source code. For all the details, look through the
-        design [journal] for the project.
-        
-        Shibumi games are built on top of the [Zero Play library] that you can use to
-        build your own games.
-        
-        [Shibumi]: https://boardgamegeek.com/boardgame/135270/shibumi
-        [Zero Play library]: https://donkirkby.github.io/zero-play/
-        
 Keywords: boardgames alphazero machine learning mcts shibumi
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ml
 Provides-Extra: ml-gpu
+License-File: LICENSE
+
+# Shibumi Games [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
+### Simple board games hiding complexity
+
+[Build Badge]: https://github.com/donkirkby/shibumi-games/actions/workflows/py-build.yml/badge.svg?branch=master
+[build]: https://github.com/donkirkby/shibumi-games/actions
+[Coverage Badge]: https://codecov.io/github/donkirkby/shibumi-games/coverage.svg?branch=master
+[codecov]: https://codecov.io/github/donkirkby/shibumi-games?branch=master
+[PyPI Badge]: https://badge.fury.io/py/shibumi.svg
+[pypi]: https://badge.fury.io/py/shibumi
+[screenshot]: https://donkirkby.github.io/shibumi-games/images/demo.png
+[journal]: https://donkirkby.github.io/shibumi-games/journal
+
+Play board games that use the [Shibumi] game system of marbles stacked on a 4x4
+board, build computer opponents for those games, learn strategy, and analyse the
+structure of the games.
+
+![screenshot]
+
+## Installing Shibumi Games
+Even though Shibumi Games has a graphical display, it is a regular Python package,
+so you can install it with `pip install shibumi`. If you haven't installed
+Python packages before, read Brett Cannon's [quick-and-dirty guide].
+
+Then run it with the `shibumi` command.
+
+The default installation generates some errors about `bdist_wheel` that don't
+seem to actually cause any problems. You can either ignore them, or install
+`wheel` before installing Shibumi Games.
+
+    pip install wheel
+    pip install shibumi
+    shibumi
+
+Known bug on Ubuntu 20.04:
+
+> qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though
+> it was found.
+
+This is a [PySide2 bug] that is missing some dependencies. You can work around
+it by installing those dependencies like this:
+
+    sudo apt install libxcb-xinerama0
+
+[quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
+[PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
+
+### Game Credits
+The Shibumi game system was designed by Cameron Browne and Néstor Romeral
+Andrés. The complete set of game rules are available on the
+[nestorgames web site], and the games used in this project are used with the
+generous permission of the designers. There are more games in a [BGG list].
+* Spaiji was designed by Néstor Romeral Andrés.
+* Spargo and Margo were designed by Cameron Browne.
+* Spire was designed by Dieter Stein, and took second place in the Shibumi
+Challenge.
+* Spline was designed by Néstor Romeral Andrés.
+* Sploof was designed by Matt Green, and took first place in the Shibumi
+Challenge.
+* Spook was designed by Dieter Stein.
+
+[nestorgames web site]: https://nestorgames.com/shibumibook_detail.html
+[BGG list]: https://boardgamegeek.com/boardgamefamily/13434/series-shibumi/linkeditems/boardgamefamily?pageid=1&sort=usersrated
+
+### Image Credits
+The marble and board graphics were designed by Cameron Browne, and are used with
+permission.
+
+Some of the buttons combine Cameron's POV-Ray graphics with icons from the
+[Open Iconic] project.
+
+[Open Iconic]: https://useiconic.com/open
+
+## More Information
+If you'd like to help out with the project, or add your own games, see the
+`CONTRIBUTING.md` file in the source code. For all the details, look through the
+design [journal] for the project.
+
+Shibumi games are built on top of the [Zero Play library] that you can use to
+build your own games.
+
+[Shibumi]: https://boardgamegeek.com/boardgame/135270/shibumi
+[Zero Play library]: https://donkirkby.github.io/zero-play/
```

### Comparing `shibumi-0.4.0/shibumi.egg-info/SOURCES.txt` & `shibumi-0.5.0/shibumi.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+LICENSE
 README.md
 setup.py
 shibumi/__init__.py
+shibumi/diagram_writer.py
 shibumi/play_shibumi.py
 shibumi/shibumi.py
 shibumi/shibumi_display.py
 shibumi/shibumi_display_ui.py
 shibumi/shibumi_game_state.py
 shibumi/shibumi_images_rc.py
 shibumi/shibumi_rules_rc.py
@@ -22,18 +24,26 @@
 shibumi/sandbox/game.py
 shibumi/spaiji/__init__.py
 shibumi/spaiji/display.py
 shibumi/spaiji/game.py
 shibumi/spargo/__init__.py
 shibumi/spargo/display.py
 shibumi/spargo/game.py
+shibumi/sparks/__init__.py
+shibumi/sparks/display.py
+shibumi/sparks/state.py
 shibumi/spire/__init__.py
 shibumi/spire/display.py
 shibumi/spire/state.py
 shibumi/spline/__init__.py
 shibumi/spline/display.py
 shibumi/spline/game.py
+shibumi/sploof/__init__.py
+shibumi/sploof/display.py
+shibumi/sploof/state.py
 shibumi/spook/__init__.py
 shibumi/spook/display.py
 shibumi/spook/state.py
 shibumi/utils/__init__.py
-shibumi/utils/headcount.py
+shibumi/utils/headcount.py
+tests/__init__.py
+tests/conftest.py
```

