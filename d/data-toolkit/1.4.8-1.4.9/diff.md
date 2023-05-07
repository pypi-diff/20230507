# Comparing `tmp/data-toolkit-1.4.8.tar.gz` & `tmp/data-toolkit-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-toolkit-1.4.8.tar", last modified: Sun Apr 30 19:47:44 2023, max compression
+gzip compressed data, was "data-toolkit-1.4.9.tar", last modified: Sun May  7 20:12:13 2023, max compression
```

## Comparing `data-toolkit-1.4.8.tar` & `data-toolkit-1.4.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-30 19:47:44.088044 data-toolkit-1.4.8/
--rw-r--r--   0 jlangr     (501) staff       (20)       58 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/CHANGELOG.md
--rw-r--r--   0 jlangr     (501) staff       (20)        1 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/LICENSE.md
--rw-r--r--   0 jlangr     (501) staff       (20)      130 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/MANIFEST.in
--rw-r--r--   0 jlangr     (501) staff       (20)     3592 2023-04-30 19:47:44.088341 data-toolkit-1.4.8/PKG-INFO
--rw-r--r--   0 jlangr     (501) staff       (20)     3259 2022-12-20 15:23:48.000000 data-toolkit-1.4.8/README.md
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-30 19:47:44.053005 data-toolkit-1.4.8/data_toolkit.egg-info/
--rw-r--r--   0 jlangr     (501) staff       (20)     3592 2023-04-30 19:47:42.000000 data-toolkit-1.4.8/data_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 jlangr     (501) staff       (20)     1087 2023-04-30 19:47:43.000000 data-toolkit-1.4.8/data_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jlangr     (501) staff       (20)        1 2023-04-30 19:47:43.000000 data-toolkit-1.4.8/data_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jlangr     (501) staff       (20)       36 2023-04-30 19:47:43.000000 data-toolkit-1.4.8/data_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 jlangr     (501) staff       (20)      112 2023-04-30 19:47:43.000000 data-toolkit-1.4.8/data_toolkit.egg-info/requires.txt
--rw-r--r--   0 jlangr     (501) staff       (20)        3 2023-04-30 19:47:43.000000 data-toolkit-1.4.8/data_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-30 19:47:44.053784 data-toolkit-1.4.8/dt/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/__init__.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-30 19:47:44.054165 data-toolkit-1.4.8/dt/controllers/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/controllers/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)    33855 2023-04-30 19:16:44.000000 data-toolkit-1.4.8/dt/controllers/base.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-30 19:47:44.055774 data-toolkit-1.4.8/dt/core/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/core/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)     5741 2023-02-27 16:32:40.000000 data-toolkit-1.4.8/dt/core/data_diff.py
--rw-r--r--   0 jlangr     (501) staff       (20)       67 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/core/exc.py
--rw-r--r--   0 jlangr     (501) staff       (20)      176 2023-04-30 19:16:44.000000 data-toolkit-1.4.8/dt/core/version.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-30 19:47:44.083672 data-toolkit-1.4.8/dt/ext/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)     8919 2023-04-30 19:16:44.000000 data-toolkit-1.4.8/dt/ext/asana.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3759 2022-08-14 21:17:02.000000 data-toolkit-1.4.8/dt/ext/aws_ec2.py
--rw-r--r--   0 jlangr     (501) staff       (20)     8287 2023-01-07 23:59:43.000000 data-toolkit-1.4.8/dt/ext/aws_s3.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3959 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/aws_s3_list.py
--rw-r--r--   0 jlangr     (501) staff       (20)     7025 2022-09-04 16:24:11.000000 data-toolkit-1.4.8/dt/ext/aws_sg.py
--rw-r--r--   0 jlangr     (501) staff       (20)     2685 2022-12-22 21:21:09.000000 data-toolkit-1.4.8/dt/ext/codex.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1042 2023-02-27 16:33:26.000000 data-toolkit-1.4.8/dt/ext/config.py
--rw-r--r--   0 jlangr     (501) staff       (20)     4963 2023-04-30 19:01:16.000000 data-toolkit-1.4.8/dt/ext/fake_data.py
--rw-r--r--   0 jlangr     (501) staff       (20)     4100 2022-12-03 18:16:05.000000 data-toolkit-1.4.8/dt/ext/firelit.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1195 2023-02-27 16:32:40.000000 data-toolkit-1.4.8/dt/ext/gcp.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1354 2022-09-15 21:51:05.000000 data-toolkit-1.4.8/dt/ext/gdrive_dl.py
--rw-r--r--   0 jlangr     (501) staff       (20)     5627 2023-02-27 16:32:40.000000 data-toolkit-1.4.8/dt/ext/github.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1237 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/gkeep.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3914 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/hist.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1080 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/monitor.py
--rw-r--r--   0 jlangr     (501) staff       (20)     7769 2023-02-27 16:32:40.000000 data-toolkit-1.4.8/dt/ext/ms_outlook.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3490 2022-12-20 15:23:48.000000 data-toolkit-1.4.8/dt/ext/notes.py
--rw-r--r--   0 jlangr     (501) staff       (20)    14061 2023-04-21 12:30:29.000000 data-toolkit-1.4.8/dt/ext/notions.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1334 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/python_exec.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1619 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/run.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1367 2022-08-14 21:17:00.000000 data-toolkit-1.4.8/dt/ext/sftp_conf.py
--rw-r--r--   0 jlangr     (501) staff       (20)     2212 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/ssh_params.py
--rw-r--r--   0 jlangr     (501) staff       (20)     8758 2022-12-03 18:16:05.000000 data-toolkit-1.4.8/dt/ext/sshconf.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3189 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/ext/tracking.py
--rw-r--r--   0 jlangr     (501) staff       (20)     2694 2022-08-14 21:17:02.000000 data-toolkit-1.4.8/dt/ext/tree.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3808 2023-02-27 16:32:40.000000 data-toolkit-1.4.8/dt/ext/zshrc.txt
--rw-r--r--   0 jlangr     (501) staff       (20)      813 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/help.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1855 2022-07-27 22:31:14.000000 data-toolkit-1.4.8/dt/main.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-30 19:47:44.084481 data-toolkit-1.4.8/dt/plugins/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/plugins/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)     6659 2022-08-14 21:28:36.000000 data-toolkit-1.4.8/dt/plugins/viz_utils.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-30 19:47:44.087281 data-toolkit-1.4.8/dt/templates/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/templates/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)       64 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/templates/command1.jinja2
--rw-r--r--   0 jlangr     (501) staff       (20)      458 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/dt/templates/sftp.json
--rw-r--r--   0 jlangr     (501) staff       (20)       99 2022-07-27 22:30:58.000000 data-toolkit-1.4.8/requirements-dev.txt
--rw-r--r--   0 jlangr     (501) staff       (20)       92 2022-09-08 17:42:10.000000 data-toolkit-1.4.8/requirements.txt
--rw-r--r--   0 jlangr     (501) staff       (20)       38 2023-04-30 19:47:44.089133 data-toolkit-1.4.8/setup.cfg
--rw-r--r--   0 jlangr     (501) staff       (20)     1130 2022-12-20 15:23:48.000000 data-toolkit-1.4.8/setup.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-05-07 20:12:13.194234 data-toolkit-1.4.9/
+-rw-r--r--   0 jlangr     (501) staff       (20)       58 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/CHANGELOG.md
+-rw-r--r--   0 jlangr     (501) staff       (20)        1 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/LICENSE.md
+-rw-r--r--   0 jlangr     (501) staff       (20)      130 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/MANIFEST.in
+-rw-r--r--   0 jlangr     (501) staff       (20)     3592 2023-05-07 20:12:13.194337 data-toolkit-1.4.9/PKG-INFO
+-rw-r--r--   0 jlangr     (501) staff       (20)     3259 2022-12-20 15:23:48.000000 data-toolkit-1.4.9/README.md
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-05-07 20:12:13.186599 data-toolkit-1.4.9/data_toolkit.egg-info/
+-rw-r--r--   0 jlangr     (501) staff       (20)     3592 2023-05-07 20:12:12.000000 data-toolkit-1.4.9/data_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jlangr     (501) staff       (20)     1087 2023-05-07 20:12:13.000000 data-toolkit-1.4.9/data_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)        1 2023-05-07 20:12:12.000000 data-toolkit-1.4.9/data_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)       36 2023-05-07 20:12:12.000000 data-toolkit-1.4.9/data_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)      112 2023-05-07 20:12:13.000000 data-toolkit-1.4.9/data_toolkit.egg-info/requires.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)        3 2023-05-07 20:12:13.000000 data-toolkit-1.4.9/data_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-05-07 20:12:13.186995 data-toolkit-1.4.9/dt/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/__init__.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-05-07 20:12:13.187331 data-toolkit-1.4.9/dt/controllers/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/controllers/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)    33855 2023-04-30 19:16:44.000000 data-toolkit-1.4.9/dt/controllers/base.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-05-07 20:12:13.187953 data-toolkit-1.4.9/dt/core/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/core/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     5741 2023-02-27 16:32:40.000000 data-toolkit-1.4.9/dt/core/data_diff.py
+-rw-r--r--   0 jlangr     (501) staff       (20)       67 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/core/exc.py
+-rw-r--r--   0 jlangr     (501) staff       (20)      176 2023-05-07 20:12:09.000000 data-toolkit-1.4.9/dt/core/version.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-05-07 20:12:13.193131 data-toolkit-1.4.9/dt/ext/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     8885 2023-05-07 20:12:09.000000 data-toolkit-1.4.9/dt/ext/asana.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3759 2022-08-14 21:17:02.000000 data-toolkit-1.4.9/dt/ext/aws_ec2.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     8287 2023-01-07 23:59:43.000000 data-toolkit-1.4.9/dt/ext/aws_s3.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3959 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/aws_s3_list.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     7025 2022-09-04 16:24:11.000000 data-toolkit-1.4.9/dt/ext/aws_sg.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     2685 2022-12-22 21:21:09.000000 data-toolkit-1.4.9/dt/ext/codex.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1042 2023-02-27 16:33:26.000000 data-toolkit-1.4.9/dt/ext/config.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     4963 2023-04-30 19:01:16.000000 data-toolkit-1.4.9/dt/ext/fake_data.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     4100 2022-12-03 18:16:05.000000 data-toolkit-1.4.9/dt/ext/firelit.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1195 2023-02-27 16:32:40.000000 data-toolkit-1.4.9/dt/ext/gcp.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1354 2022-09-15 21:51:05.000000 data-toolkit-1.4.9/dt/ext/gdrive_dl.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     5627 2023-02-27 16:32:40.000000 data-toolkit-1.4.9/dt/ext/github.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1237 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/gkeep.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3914 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/hist.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1080 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/monitor.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     7769 2023-02-27 16:32:40.000000 data-toolkit-1.4.9/dt/ext/ms_outlook.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3490 2022-12-20 15:23:48.000000 data-toolkit-1.4.9/dt/ext/notes.py
+-rw-r--r--   0 jlangr     (501) staff       (20)    14061 2023-04-21 12:30:29.000000 data-toolkit-1.4.9/dt/ext/notions.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1334 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/python_exec.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1619 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/run.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1367 2022-08-14 21:17:00.000000 data-toolkit-1.4.9/dt/ext/sftp_conf.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     2212 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/ssh_params.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     8758 2022-12-03 18:16:05.000000 data-toolkit-1.4.9/dt/ext/sshconf.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3189 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/ext/tracking.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     2694 2022-08-14 21:17:02.000000 data-toolkit-1.4.9/dt/ext/tree.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3808 2023-02-27 16:32:40.000000 data-toolkit-1.4.9/dt/ext/zshrc.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)      813 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/help.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1855 2022-07-27 22:31:14.000000 data-toolkit-1.4.9/dt/main.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-05-07 20:12:13.193398 data-toolkit-1.4.9/dt/plugins/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/plugins/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     6659 2022-08-14 21:28:36.000000 data-toolkit-1.4.9/dt/plugins/viz_utils.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-05-07 20:12:13.194013 data-toolkit-1.4.9/dt/templates/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/templates/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)       64 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/templates/command1.jinja2
+-rw-r--r--   0 jlangr     (501) staff       (20)      458 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/dt/templates/sftp.json
+-rw-r--r--   0 jlangr     (501) staff       (20)       99 2022-07-27 22:30:58.000000 data-toolkit-1.4.9/requirements-dev.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)       92 2022-09-08 17:42:10.000000 data-toolkit-1.4.9/requirements.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)       38 2023-05-07 20:12:13.194714 data-toolkit-1.4.9/setup.cfg
+-rw-r--r--   0 jlangr     (501) staff       (20)     1130 2022-12-20 15:23:48.000000 data-toolkit-1.4.9/setup.py
```

### Comparing `data-toolkit-1.4.8/PKG-INFO` & `data-toolkit-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-toolkit
-Version: 1.4.8
+Version: 1.4.9
 Summary: ML & data helper code!
 Home-page: https://github.com/jakublangr/data-toolkit/
 Author: Jakub Langr
 Author-email: james.langr@gmail.com
 License: (c) Jakub Langr
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `data-toolkit-1.4.8/README.md` & `data-toolkit-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/data_toolkit.egg-info/PKG-INFO` & `data-toolkit-1.4.9/data_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-toolkit
-Version: 1.4.8
+Version: 1.4.9
 Summary: ML & data helper code!
 Home-page: https://github.com/jakublangr/data-toolkit/
 Author: Jakub Langr
 Author-email: james.langr@gmail.com
 License: (c) Jakub Langr
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `data-toolkit-1.4.8/data_toolkit.egg-info/SOURCES.txt` & `data-toolkit-1.4.9/data_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/controllers/base.py` & `data-toolkit-1.4.9/dt/controllers/base.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/core/data_diff.py` & `data-toolkit-1.4.9/dt/core/data_diff.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/asana.py` & `data-toolkit-1.4.9/dt/ext/asana.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,14 @@
         # 'projects': [workspace_id]
     }
     
     # if project_name == '-1':
     #     del data['projects']
         
     print("posting", data)
-    import ipdb; ipdb.set_trace()
     result = client.tasks.create_in_workspace(workspace_id, data)
 
     print(json.dumps(result, indent=4))
     
 def done_todo(task_id):
     client = get_client(True)
     data =  {'completed': True}
```

### Comparing `data-toolkit-1.4.8/dt/ext/aws_ec2.py` & `data-toolkit-1.4.9/dt/ext/aws_ec2.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/aws_s3.py` & `data-toolkit-1.4.9/dt/ext/aws_s3.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/aws_s3_list.py` & `data-toolkit-1.4.9/dt/ext/aws_s3_list.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/aws_sg.py` & `data-toolkit-1.4.9/dt/ext/aws_sg.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/codex.py` & `data-toolkit-1.4.9/dt/ext/codex.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/config.py` & `data-toolkit-1.4.9/dt/ext/config.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/fake_data.py` & `data-toolkit-1.4.9/dt/ext/fake_data.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/firelit.py` & `data-toolkit-1.4.9/dt/ext/firelit.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/gcp.py` & `data-toolkit-1.4.9/dt/ext/gcp.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/gdrive_dl.py` & `data-toolkit-1.4.9/dt/ext/gdrive_dl.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/github.py` & `data-toolkit-1.4.9/dt/ext/github.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/gkeep.py` & `data-toolkit-1.4.9/dt/ext/gkeep.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/hist.py` & `data-toolkit-1.4.9/dt/ext/hist.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/monitor.py` & `data-toolkit-1.4.9/dt/ext/monitor.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/ms_outlook.py` & `data-toolkit-1.4.9/dt/ext/ms_outlook.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/notes.py` & `data-toolkit-1.4.9/dt/ext/notes.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/notions.py` & `data-toolkit-1.4.9/dt/ext/notions.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/python_exec.py` & `data-toolkit-1.4.9/dt/ext/python_exec.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/run.py` & `data-toolkit-1.4.9/dt/ext/run.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/sftp_conf.py` & `data-toolkit-1.4.9/dt/ext/sftp_conf.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/ssh_params.py` & `data-toolkit-1.4.9/dt/ext/ssh_params.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/sshconf.py` & `data-toolkit-1.4.9/dt/ext/sshconf.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/tracking.py` & `data-toolkit-1.4.9/dt/ext/tracking.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/tree.py` & `data-toolkit-1.4.9/dt/ext/tree.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/ext/zshrc.txt` & `data-toolkit-1.4.9/dt/ext/zshrc.txt`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/help.py` & `data-toolkit-1.4.9/dt/help.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/main.py` & `data-toolkit-1.4.9/dt/main.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/dt/plugins/viz_utils.py` & `data-toolkit-1.4.9/dt/plugins/viz_utils.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.8/setup.py` & `data-toolkit-1.4.9/setup.py`

 * *Files identical despite different names*

