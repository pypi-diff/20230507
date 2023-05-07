# Comparing `tmp/moss-rl-0.0.1.tar.gz` & `tmp/moss-rl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moss-rl-0.0.1.tar", last modified: Sun May  7 03:23:42 2023, max compression
+gzip compressed data, was "moss-rl-0.0.2.tar", last modified: Sun May  7 06:26:20 2023, max compression
```

## Comparing `moss-rl-0.0.1.tar` & `moss-rl-0.0.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.426844 moss-rl-0.0.1/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1074 2023-02-19 11:37:12.000000 moss-rl-0.0.1/LICENSE
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      700 2023-05-07 03:23:42.426844 moss-rl-0.0.1/PKG-INFO
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      102 2023-03-17 14:13:39.000000 moss-rl-0.0.1/README.md
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/examples/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-01-10 13:35:45.000000 moss-rl-0.0.1/examples/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     6634 2023-05-07 03:14:26.000000 moss-rl-0.0.1/examples/atari_impala.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       36 2023-05-07 03:23:35.000000 moss-rl-0.0.1/moss/__init__.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/actor/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       14 2023-05-06 15:06:09.000000 moss-rl-0.0.1/moss/actor/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     4157 2023-05-05 13:46:14.000000 moss-rl-0.0.1/moss/actor/vector.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/agent/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       14 2023-05-06 15:06:09.000000 moss-rl-0.0.1/moss/agent/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1394 2023-04-27 16:14:18.000000 moss-rl-0.0.1/moss/agent/atari.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/buffer/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       22 2023-05-06 15:06:09.000000 moss-rl-0.0.1/moss/buffer/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1265 2023-05-06 15:06:09.000000 moss-rl-0.0.1/moss/buffer/queue.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2088 2023-04-27 16:14:49.000000 moss-rl-0.0.1/moss/buffer/reverb.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2316 2023-04-27 16:08:18.000000 moss-rl-0.0.1/moss/core.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/env/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      365 2023-04-26 13:53:59.000000 moss-rl-0.0.1/moss/env/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2761 2023-04-26 13:47:48.000000 moss-rl-0.0.1/moss/env/base.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     4155 2023-05-05 14:09:16.000000 moss-rl-0.0.1/moss/env/vector_env.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      732 2023-04-26 13:56:20.000000 moss-rl-0.0.1/moss/env/worker.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/learner/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       16 2023-05-06 15:06:09.000000 moss-rl-0.0.1/moss/learner/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3996 2023-04-23 13:07:56.000000 moss-rl-0.0.1/moss/learner/base.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3977 2023-04-26 14:49:47.000000 moss-rl-0.0.1/moss/learner/impala.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/network/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       16 2023-05-06 15:06:08.000000 moss-rl-0.0.1/moss/network/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3239 2023-04-27 13:17:51.000000 moss-rl-0.0.1/moss/network/atari.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1278 2023-05-06 15:06:08.000000 moss-rl-0.0.1/moss/network/base.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/predictor/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       18 2023-05-06 15:06:08.000000 moss-rl-0.0.1/moss/predictor/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3993 2023-04-27 13:17:51.000000 moss-rl-0.0.1/moss/predictor/base.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      736 2023-04-27 15:55:56.000000 moss-rl-0.0.1/moss/types.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.422844 moss-rl-0.0.1/moss/utils/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       14 2023-05-06 15:06:09.000000 moss-rl-0.0.1/moss/utils/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     4158 2023-02-25 15:45:52.000000 moss-rl-0.0.1/moss/utils/async_utils.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.426844 moss-rl-0.0.1/moss/utils/loggers/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2017 2023-03-26 11:40:10.000000 moss-rl-0.0.1/moss/utils/loggers/__init__.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2679 2023-03-26 11:40:10.000000 moss-rl-0.0.1/moss/utils/loggers/aggregators.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1420 2023-02-25 15:48:33.000000 moss-rl-0.0.1/moss/utils/loggers/asynchronous.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2480 2023-02-25 15:49:35.000000 moss-rl-0.0.1/moss/utils/loggers/base.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1548 2023-02-25 15:48:02.000000 moss-rl-0.0.1/moss/utils/loggers/constant.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     4527 2023-03-26 11:40:10.000000 moss-rl-0.0.1/moss/utils/loggers/csv.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1433 2023-02-25 15:59:45.000000 moss-rl-0.0.1/moss/utils/loggers/dataframe.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2989 2023-04-13 00:40:27.000000 moss-rl-0.0.1/moss/utils/loggers/default.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     5392 2023-02-25 15:54:49.000000 moss-rl-0.0.1/moss/utils/loggers/filters.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2009 2023-02-25 15:50:44.000000 moss-rl-0.0.1/moss/utils/loggers/flatten.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2423 2023-03-02 14:19:59.000000 moss-rl-0.0.1/moss/utils/loggers/tensorboard.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3010 2023-02-25 15:57:07.000000 moss-rl-0.0.1/moss/utils/loggers/terminal.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1195 2023-02-25 15:46:59.000000 moss-rl-0.0.1/moss/utils/loggers/timestamp.py
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2500 2023-02-25 15:59:30.000000 moss-rl-0.0.1/moss/utils/paths.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.426844 moss-rl-0.0.1/moss_rl.egg-info/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      700 2023-05-07 03:23:42.000000 moss-rl-0.0.1/moss_rl.egg-info/PKG-INFO
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1190 2023-05-07 03:23:42.000000 moss-rl-0.0.1/moss_rl.egg-info/SOURCES.txt
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)        1 2023-05-07 03:23:42.000000 moss-rl-0.0.1/moss_rl.egg-info/dependency_links.txt
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      361 2023-05-07 03:23:42.000000 moss-rl-0.0.1/moss_rl.egg-info/requires.txt
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       19 2023-05-07 03:23:42.000000 moss-rl-0.0.1/moss_rl.egg-info/top_level.txt
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      978 2023-05-07 03:23:42.426844 moss-rl-0.0.1/setup.cfg
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2209 2023-05-07 03:13:38.000000 moss-rl-0.0.1/setup.py
-drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 03:23:42.426844 moss-rl-0.0.1/test/
--rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       17 2023-04-21 15:16:34.000000 moss-rl-0.0.1/test/__init__.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.731555 moss-rl-0.0.2/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1074 2023-02-19 11:37:12.000000 moss-rl-0.0.2/LICENSE
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      740 2023-05-07 06:26:20.731555 moss-rl-0.0.2/PKG-INFO
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      102 2023-03-17 14:13:39.000000 moss-rl-0.0.2/README.md
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/examples/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-01-10 13:35:45.000000 moss-rl-0.0.2/examples/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     6634 2023-05-07 03:14:26.000000 moss-rl-0.0.2/examples/atari_impala.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       36 2023-05-07 06:23:01.000000 moss-rl-0.0.2/moss/__init__.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/actor/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       14 2023-05-07 04:01:05.000000 moss-rl-0.0.2/moss/actor/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     4157 2023-05-05 13:46:14.000000 moss-rl-0.0.2/moss/actor/vector.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/agent/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       14 2023-05-07 04:01:04.000000 moss-rl-0.0.2/moss/agent/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1394 2023-04-27 16:14:18.000000 moss-rl-0.0.2/moss/agent/atari.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/buffer/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       22 2023-05-07 04:01:05.000000 moss-rl-0.0.2/moss/buffer/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1265 2023-05-07 04:01:05.000000 moss-rl-0.0.2/moss/buffer/queue.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2088 2023-04-27 16:14:49.000000 moss-rl-0.0.2/moss/buffer/reverb.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2316 2023-04-27 16:08:18.000000 moss-rl-0.0.2/moss/core.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/env/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      365 2023-04-26 13:53:59.000000 moss-rl-0.0.2/moss/env/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2761 2023-04-26 13:47:48.000000 moss-rl-0.0.2/moss/env/base.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     4173 2023-05-07 04:00:23.000000 moss-rl-0.0.2/moss/env/vector_env.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      732 2023-04-26 13:56:20.000000 moss-rl-0.0.2/moss/env/worker.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/learner/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       16 2023-05-07 04:01:05.000000 moss-rl-0.0.2/moss/learner/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3996 2023-04-23 13:07:56.000000 moss-rl-0.0.2/moss/learner/base.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3977 2023-04-26 14:49:47.000000 moss-rl-0.0.2/moss/learner/impala.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/network/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       16 2023-05-07 04:01:04.000000 moss-rl-0.0.2/moss/network/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3239 2023-04-27 13:17:51.000000 moss-rl-0.0.2/moss/network/atari.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1278 2023-05-07 04:01:04.000000 moss-rl-0.0.2/moss/network/base.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/predictor/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       18 2023-05-07 04:01:04.000000 moss-rl-0.0.2/moss/predictor/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3993 2023-04-27 13:17:51.000000 moss-rl-0.0.2/moss/predictor/base.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      736 2023-04-27 15:55:56.000000 moss-rl-0.0.2/moss/types.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/utils/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       14 2023-05-07 04:01:04.000000 moss-rl-0.0.2/moss/utils/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     4158 2023-02-25 15:45:52.000000 moss-rl-0.0.2/moss/utils/async_utils.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss/utils/loggers/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2017 2023-03-26 11:40:10.000000 moss-rl-0.0.2/moss/utils/loggers/__init__.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2679 2023-03-26 11:40:10.000000 moss-rl-0.0.2/moss/utils/loggers/aggregators.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1420 2023-02-25 15:48:33.000000 moss-rl-0.0.2/moss/utils/loggers/asynchronous.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2480 2023-02-25 15:49:35.000000 moss-rl-0.0.2/moss/utils/loggers/base.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1548 2023-02-25 15:48:02.000000 moss-rl-0.0.2/moss/utils/loggers/constant.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     4527 2023-03-26 11:40:10.000000 moss-rl-0.0.2/moss/utils/loggers/csv.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1433 2023-02-25 15:59:45.000000 moss-rl-0.0.2/moss/utils/loggers/dataframe.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2989 2023-04-13 00:40:27.000000 moss-rl-0.0.2/moss/utils/loggers/default.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     5392 2023-02-25 15:54:49.000000 moss-rl-0.0.2/moss/utils/loggers/filters.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2009 2023-02-25 15:50:44.000000 moss-rl-0.0.2/moss/utils/loggers/flatten.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2423 2023-03-02 14:19:59.000000 moss-rl-0.0.2/moss/utils/loggers/tensorboard.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     3010 2023-02-25 15:57:07.000000 moss-rl-0.0.2/moss/utils/loggers/terminal.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1195 2023-02-25 15:46:59.000000 moss-rl-0.0.2/moss/utils/loggers/timestamp.py
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2500 2023-02-25 15:59:30.000000 moss-rl-0.0.2/moss/utils/paths.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/moss_rl.egg-info/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      740 2023-05-07 06:26:20.000000 moss-rl-0.0.2/moss_rl.egg-info/PKG-INFO
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     1190 2023-05-07 06:26:20.000000 moss-rl-0.0.2/moss_rl.egg-info/SOURCES.txt
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)        1 2023-05-07 06:26:20.000000 moss-rl-0.0.2/moss_rl.egg-info/dependency_links.txt
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      361 2023-05-07 06:26:20.000000 moss-rl-0.0.2/moss_rl.egg-info/requires.txt
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       19 2023-05-07 06:26:20.000000 moss-rl-0.0.2/moss_rl.egg-info/top_level.txt
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)      978 2023-05-07 06:26:20.731555 moss-rl-0.0.2/setup.cfg
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)     2258 2023-05-07 05:57:20.000000 moss-rl-0.0.2/setup.py
+drwxrwxr-x   0 lanzhiyi  (1000) lanzhiyi  (1000)        0 2023-05-07 06:26:20.727555 moss-rl-0.0.2/test/
+-rw-rw-r--   0 lanzhiyi  (1000) lanzhiyi  (1000)       17 2023-04-21 15:16:34.000000 moss-rl-0.0.2/test/__init__.py
```

### Comparing `moss-rl-0.0.1/LICENSE` & `moss-rl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/PKG-INFO` & `moss-rl-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: moss-rl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for Reinforcement Learning.
 Home-page: https://github.com/hilanzy/moss
 Author: lanzhiyi
 Author-email: lanzhiy.mail@qq.com
 License: MIT
 Keywords: reinforcement-learning python machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="docs/_static/images/moss.jpg">
 
 # Moss
```

### Comparing `moss-rl-0.0.1/examples/atari_impala.py` & `moss-rl-0.0.2/examples/atari_impala.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/actor/vector.py` & `moss-rl-0.0.2/moss/actor/vector.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/agent/atari.py` & `moss-rl-0.0.2/moss/agent/atari.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/buffer/queue.py` & `moss-rl-0.0.2/moss/buffer/queue.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/buffer/reverb.py` & `moss-rl-0.0.2/moss/buffer/reverb.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/core.py` & `moss-rl-0.0.2/moss/core.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/env/base.py` & `moss-rl-0.0.2/moss/env/base.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/env/vector_env.py` & `moss-rl-0.0.2/moss/env/vector_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,17 @@
   ) -> None:
     """Init.
 
     Args:
       num_envs: Num of vectorized environments.
       env_maker: Environment maker function.
       worker_fn: Environment worker function.
-      process_fn: Function to package the return timestep of all environments
-        into `List[TimeStep]` format.
+      process_fn: Function to split the timesteps returned by the environment
+        into single-agent timestep format and repackage them into
+        `List[TimeStep]` format.
       kwargs: Any other arguments.
     """
     self._num_envs = num_envs
     self._envs = [env_maker() for _ in range(num_envs)]
     self._workers = [worker_fn(env) for env in self._envs]
     self._process_fn = process_fn
     if kwargs.get("observation_spec") is not None:
@@ -43,16 +44,17 @@
     if kwargs.get("action_spec") is not None:
       self.action_spec = kwargs["action_spec"]  # type: ignore
 
   def reset(self) -> Dict[int, List[TimeStep]]:
     """Vectorized environments reset.
 
     Returns:
-      A `TimeStep` list containing all timesteps(split by env_id and player_id)
-        of this vectorized multi-agent(maybe) environments.
+      A `Dict[int, List[TimeStep]]`:
+        Key: env_id.
+        Value: `List[TimeStep]` containing all player's timestep.
     """
     timesteps_dict = {
       env_id: self._process_fn(worker.reset())
       for env_id, worker in enumerate(self._workers)
     }
     return timesteps_dict
 
@@ -60,17 +62,17 @@
     """Vectorized environments step.
 
     Args:
       actions: A NumPy array, or a nested dict, list or tuple of arrays
       corresponding to `action_spec()`.
 
     Returns:
-      A `TimeStep` list containing:
-        All timesteps(split by env_id and player_id) of this vectorized
-          multi-agent(maybe) environments.
+      A `Dict[int, List[TimeStep]]`:
+        Key: env_id.
+        Value: `List[TimeStep]` containing all player's timestep.
     """
     timesteps_dict = {
       env_id: self._process_fn(worker.step(actions[env_id]))
       for env_id, worker in enumerate(self._workers)
     }
     return timesteps_dict
```

### Comparing `moss-rl-0.0.1/moss/env/worker.py` & `moss-rl-0.0.2/moss/env/worker.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/learner/base.py` & `moss-rl-0.0.2/moss/learner/base.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/learner/impala.py` & `moss-rl-0.0.2/moss/learner/impala.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/network/atari.py` & `moss-rl-0.0.2/moss/network/atari.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/network/base.py` & `moss-rl-0.0.2/moss/network/base.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/predictor/base.py` & `moss-rl-0.0.2/moss/predictor/base.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/types.py` & `moss-rl-0.0.2/moss/types.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/async_utils.py` & `moss-rl-0.0.2/moss/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/__init__.py` & `moss-rl-0.0.2/moss/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/aggregators.py` & `moss-rl-0.0.2/moss/utils/loggers/aggregators.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/asynchronous.py` & `moss-rl-0.0.2/moss/utils/loggers/asynchronous.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/base.py` & `moss-rl-0.0.2/moss/utils/loggers/base.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/constant.py` & `moss-rl-0.0.2/moss/utils/loggers/constant.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/csv.py` & `moss-rl-0.0.2/moss/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/dataframe.py` & `moss-rl-0.0.2/moss/utils/loggers/dataframe.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/default.py` & `moss-rl-0.0.2/moss/utils/loggers/default.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/filters.py` & `moss-rl-0.0.2/moss/utils/loggers/filters.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/flatten.py` & `moss-rl-0.0.2/moss/utils/loggers/flatten.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/tensorboard.py` & `moss-rl-0.0.2/moss/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/terminal.py` & `moss-rl-0.0.2/moss/utils/loggers/terminal.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/loggers/timestamp.py` & `moss-rl-0.0.2/moss/utils/loggers/timestamp.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss/utils/paths.py` & `moss-rl-0.0.2/moss/utils/paths.py`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/moss_rl.egg-info/PKG-INFO` & `moss-rl-0.0.2/moss_rl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: moss-rl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for Reinforcement Learning.
 Home-page: https://github.com/hilanzy/moss
 Author: lanzhiyi
 Author-email: lanzhiy.mail@qq.com
 License: MIT
 Keywords: reinforcement-learning python machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="docs/_static/images/moss.jpg">
 
 # Moss
```

### Comparing `moss-rl-0.0.1/moss_rl.egg-info/SOURCES.txt` & `moss-rl-0.0.2/moss_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/setup.cfg` & `moss-rl-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `moss-rl-0.0.1/setup.py` & `moss-rl-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
 
 setup(
   name="moss-rl",
   version=get_version(),
   description="A Python library for Reinforcement Learning.",
   long_description=open("README.md", encoding="utf8").read(),
+  long_description_content_type="text/markdown",
   author="lanzhiyi",
   author_email="lanzhiy.mail@qq.com",
   url="https://github.com/hilanzy/moss",
   packages=find_packages(),
   license="MIT",
   python_requires=">=3.8",
   install_requires=get_install_requires(),
```

