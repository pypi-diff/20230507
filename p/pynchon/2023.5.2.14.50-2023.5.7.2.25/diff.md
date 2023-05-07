# Comparing `tmp/pynchon-2023.5.2.14.50.tar.gz` & `tmp/pynchon-2023.5.7.2.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynchon-2023.5.2.14.50.tar", last modified: Tue May  2 18:50:00 2023, max compression
+gzip compressed data, was "pynchon-2023.5.7.2.25.tar", last modified: Sun May  7 06:25:11 2023, max compression
```

## Comparing `pynchon-2023.5.2.14.50.tar` & `pynchon-2023.5.7.2.25.tar`

### file list

```diff
@@ -1,169 +1,214 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/
--rw-rw-r--   0 matt      (1000) matt      (1000)       50 2022-10-31 17:10:29.000000 pynchon-2023.5.2.14.50/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)      736 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     6135 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)      979 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)     1602 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      730 2022-10-31 16:56:45.000000 pynchon-2023.5.2.14.50/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/
--rw-rw-r--   0 matt      (1000) matt      (1000)      251 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      100 2023-05-02 02:18:56.000000 pynchon-2023.5.2.14.50/src/pynchon/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-05-02 18:49:57.000000 pynchon-2023.5.2.14.50/src/pynchon/_version.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/abcs/
--rw-rw-r--   0 matt      (1000) matt      (1000)      262 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1244 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/attrdict.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2431 2023-05-02 01:26:44.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2909 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/meta.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/path.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/plugin.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4788 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/visitor.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4336 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/annotate.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/api/
--rw-rw-r--   0 matt      (1000) matt      (1000)       20 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/api/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/api/git/
--rw-rw-r--   0 matt      (1000) matt      (1000)      109 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/api/git/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/api/project/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1146 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/api/project/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       28 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/api/pynchon.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2215 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/api/render.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5154 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/app.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/bin/
--rw-rw-r--   0 matt      (1000) matt      (1000)      972 2023-05-02 03:00:09.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/cli.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/dot.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3318 2023-04-30 22:57:08.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/entry.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/groups.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 03:58:20.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/options.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/parse.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/render.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/cli/
--rw-rw-r--   0 matt      (1000) matt      (1000)       54 2023-04-30 18:28:18.000000 pynchon-2023.5.2.14.50/src/pynchon/cli/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6992 2023-05-02 02:54:32.000000 pynchon-2023.5.2.14.50/src/pynchon/cli/common.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/cli/options.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2439 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/click.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/config/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1824 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/config/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4672 2023-04-30 17:56:47.000000 pynchon-2023.5.2.14.50/src/pynchon/config/util.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1059 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/constants.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2856 2023-05-02 01:23:34.000000 pynchon-2023.5.2.14.50/src/pynchon/core.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      115 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/events.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-04-29 21:27:56.000000 pynchon-2023.5.2.14.50/src/pynchon/exceptions.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/fleks/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 02:43:01.000000 pynchon-2023.5.2.14.50/src/pynchon/fleks/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8460 2023-05-02 03:00:09.000000 pynchon-2023.5.2.14.50/src/pynchon/models.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1006 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/api.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       95 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/ast.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      473 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/cicd.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1593 2023-05-02 03:03:42.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/core.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-29 22:36:50.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/cut.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/doctor/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/doctor/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5684 2023-05-02 05:37:02.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/dot.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      374 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/files.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2797 2023-05-02 05:30:45.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/fixme.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      351 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/gen.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/git/
--rw-rw-r--   0 matt      (1000) matt      (1000)      373 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/git/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2448 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/git/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      305 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/globals.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/hooks.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6082 2023-05-02 18:49:46.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/jinja.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3527 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/json.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      722 2023-04-29 19:14:56.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/load.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/makefile/
--rw-rw-r--   0 matt      (1000) matt      (1000)       52 2023-04-28 18:54:48.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/makefile/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      840 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/parse.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1149 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/plugins.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4548 2023-04-30 18:42:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/project.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/
--rw-rw-r--   0 matt      (1000) matt      (1000)      112 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2709 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/api.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/ast.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     7490 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/cli.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      236 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/models.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1525 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/platform.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      456 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/pypi.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      723 2023-04-29 19:14:56.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/release.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4781 2023-04-30 17:58:57.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/render.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       60 2023-04-28 22:07:13.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/rtd.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3434 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1156 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1266 2023-04-30 17:56:47.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/util.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/shimport/
--rw-rw-r--   0 matt      (1000) matt      (1000)      209 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      562 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/abcs.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 01:24:51.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/hooks.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 17:41:25.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/importing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    12287 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/models.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2390 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/module.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 18:08:09.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/registry.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 01:29:20.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/types.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      538 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/util.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       73 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/tagging.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/pynchon/templates/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/cookie_cutter/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/cookie_cutter/.gitkeep
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/github/
--rw-rw-r--   0 matt      (1000) matt      (1000)      295 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/github/header.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/Makefile.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/core/
--rw-rw-r--   0 matt      (1000) matt      (1000)      392 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/fixme/
--rw-rw-r--   0 matt      (1000) matt      (1000)      164 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/
--rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)     1190 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      891 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      322 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)     2985 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/
--rw-rw-r--   0 matt      (1000) matt      (1000)      623 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/cli-toc.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      198 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/detail.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      253 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/main.module.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      284 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/testing.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/util/
--rw-rw-r--   0 matt      (1000) matt      (1000)     2084 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1016 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/click.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4750 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/complexity.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      871 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/util/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      577 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/events.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4348 2023-05-02 05:31:21.000000 pynchon-2023.5.2.14.50/src/pynchon/util/files.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1944 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/util/lme.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      954 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/oop.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-02 05:37:15.000000 pynchon-2023.5.2.14.50/src/pynchon/util/os.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2279 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/python.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2972 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/tagging.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      411 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/testing.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/util/text/
--rw-rw-r--   0 matt      (1000) matt      (1000)      837 2023-05-02 00:54:17.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      365 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/__main__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/
--rw-rw-r--   0 matt      (1000) matt      (1000)     5301 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1033 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1654 2023-05-02 18:49:46.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/loads.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/src/pynchon/util/text/normalize/
--rw-rw-r--   0 matt      (1000) matt      (1000)      740 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/normalize/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       40 2023-04-29 02:48:43.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/normalize/__main__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/src/pynchon/util/text/render/
--rw-rw-r--   0 matt      (1000) matt      (1000)     5245 2023-05-01 23:54:56.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/render/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      963 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/render/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1171 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/typing.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)      736 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     4455 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       46 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      399 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        8 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/top_level.txt
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.371772 pynchon-2023.5.7.2.25/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       50 2022-10-31 17:10:29.000000 pynchon-2023.5.7.2.25/MANIFEST.in
+-rw-rw-r--   0 matt      (1000) matt      (1000)      735 2023-05-07 06:25:11.371772 pynchon-2023.5.7.2.25/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6135 2023-05-07 06:23:36.000000 pynchon-2023.5.7.2.25/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)      979 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1602 2023-05-07 06:25:11.371772 pynchon-2023.5.7.2.25/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)      745 2023-05-06 19:23:30.000000 pynchon-2023.5.7.2.25/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.351772 pynchon-2023.5.7.2.25/src/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.355772 pynchon-2023.5.7.2.25/src/pynchon/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      251 2023-04-30 02:08:52.000000 pynchon-2023.5.7.2.25/src/pynchon/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      100 2023-05-02 02:18:56.000000 pynchon-2023.5.7.2.25/src/pynchon/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       76 2023-05-07 06:25:08.000000 pynchon-2023.5.7.2.25/src/pynchon/_version.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.355772 pynchon-2023.5.7.2.25/src/pynchon/abcs/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      139 2023-05-07 01:31:22.000000 pynchon-2023.5.7.2.25/src/pynchon/abcs/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1244 2023-05-06 04:40:39.000000 pynchon-2023.5.7.2.25/src/pynchon/abcs/attrdict.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2443 2023-05-06 15:53:02.000000 pynchon-2023.5.7.2.25/src/pynchon/abcs/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2152 2023-05-07 04:04:39.000000 pynchon-2023.5.7.2.25/src/pynchon/abcs/path.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4788 2023-05-02 02:11:29.000000 pynchon-2023.5.7.2.25/src/pynchon/abcs/visitor.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4336 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/annotate.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.355772 pynchon-2023.5.7.2.25/src/pynchon/api/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       20 2023-04-27 22:45:44.000000 pynchon-2023.5.7.2.25/src/pynchon/api/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.355772 pynchon-2023.5.7.2.25/src/pynchon/api/git/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      109 2023-04-27 22:45:44.000000 pynchon-2023.5.7.2.25/src/pynchon/api/git/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.355772 pynchon-2023.5.7.2.25/src/pynchon/api/project/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1146 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/api/project/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2023-04-27 22:45:44.000000 pynchon-2023.5.7.2.25/src/pynchon/api/pynchon.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2809 2023-05-06 18:15:17.000000 pynchon-2023.5.7.2.25/src/pynchon/api/render.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4203 2023-05-06 15:29:39.000000 pynchon-2023.5.7.2.25/src/pynchon/app.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.359773 pynchon-2023.5.7.2.25/src/pynchon/bin/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1004 2023-05-06 21:08:32.000000 pynchon-2023.5.7.2.25/src/pynchon/bin/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       24 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/bin/cli.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       24 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/bin/dot.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3457 2023-05-06 22:04:48.000000 pynchon-2023.5.7.2.25/src/pynchon/bin/entry.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/bin/groups.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/bin/options.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       26 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/bin/parse.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/bin/render.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.359773 pynchon-2023.5.7.2.25/src/pynchon/cli/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       89 2023-05-06 21:35:11.000000 pynchon-2023.5.7.2.25/src/pynchon/cli/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      143 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/cli/arguments.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2893 2023-05-06 22:04:48.000000 pynchon-2023.5.7.2.25/src/pynchon/cli/click.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6655 2023-05-03 22:11:03.000000 pynchon-2023.5.7.2.25/src/pynchon/cli/common.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/cli/options.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.359773 pynchon-2023.5.7.2.25/src/pynchon/config/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1778 2023-05-06 20:26:26.000000 pynchon-2023.5.7.2.25/src/pynchon/config/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4061 2023-05-06 21:18:11.000000 pynchon-2023.5.7.2.25/src/pynchon/config/util.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1129 2023-05-05 13:46:48.000000 pynchon-2023.5.7.2.25/src/pynchon/constants.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2855 2023-05-06 20:15:38.000000 pynchon-2023.5.7.2.25/src/pynchon/core.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1553 2023-05-06 16:54:14.000000 pynchon-2023.5.7.2.25/src/pynchon/events.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-04-29 21:27:56.000000 pynchon-2023.5.7.2.25/src/pynchon/exceptions.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.359773 pynchon-2023.5.7.2.25/src/pynchon/fleks/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       43 2023-05-06 15:54:08.000000 pynchon-2023.5.7.2.25/src/pynchon/fleks/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.359773 pynchon-2023.5.7.2.25/src/pynchon/fleks/meta/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      121 2023-05-07 06:24:37.000000 pynchon-2023.5.7.2.25/src/pynchon/fleks/meta/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      908 2023-05-07 01:31:15.000000 pynchon-2023.5.7.2.25/src/pynchon/fleks/meta/namespace.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4138 2023-05-07 01:31:14.000000 pynchon-2023.5.7.2.25/src/pynchon/fleks/meta/oop.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-05-06 21:27:19.000000 pynchon-2023.5.7.2.25/src/pynchon/fleks/plugin.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.359773 pynchon-2023.5.7.2.25/src/pynchon/models/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      122 2023-05-06 16:13:38.000000 pynchon-2023.5.7.2.25/src/pynchon/models/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2390 2023-05-07 06:24:37.000000 pynchon-2023.5.7.2.25/src/pynchon/models/planner.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3980 2023-05-07 01:31:15.000000 pynchon-2023.5.7.2.25/src/pynchon/models/planning.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.359773 pynchon-2023.5.7.2.25/src/pynchon/models/plugin_types/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     9168 2023-05-07 01:31:15.000000 pynchon-2023.5.7.2.25/src/pynchon/models/plugin_types/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       41 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/models/plugin_types/base.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/plugins/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      881 2023-05-06 15:54:39.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      388 2023-05-04 02:17:09.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/__template__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/api.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       95 2023-04-27 22:45:44.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/ast.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      473 2023-05-01 23:36:05.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/cicd.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1051 2023-05-06 22:04:48.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/cookie_cutter.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4927 2023-05-07 06:24:37.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/core.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1701 2023-05-07 04:04:39.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/docs.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/plugins/doctor/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       40 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/doctor/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5068 2023-05-03 22:03:10.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/dot.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      374 2023-05-06 14:56:32.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/files.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3104 2023-05-07 00:23:04.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/fixme.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      350 2023-05-06 15:10:55.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/gen.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2612 2023-05-06 20:21:06.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/git.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      305 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/globals.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      377 2023-05-04 02:17:09.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/griffe.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       30 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/hooks.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4108 2023-05-07 00:20:00.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/jinja.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3524 2023-05-06 15:10:20.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/json.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      722 2023-04-29 19:14:56.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/load.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/plugins/makefile/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       52 2023-04-28 18:54:48.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/makefile/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      388 2023-05-05 13:11:07.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/makefile.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      840 2023-04-27 22:45:44.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/parse.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1024 2023-05-06 14:56:32.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/plugins.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2191 2023-05-03 17:10:13.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/project.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      112 2023-04-28 01:24:33.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2949 2023-05-03 22:05:41.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/api.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       35 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/ast.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7458 2023-05-07 04:04:37.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/cli.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      236 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/models.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1525 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/platform.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      456 2023-04-30 02:08:52.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/python/pypi.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      723 2023-04-29 19:14:56.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/release.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4781 2023-05-03 00:37:41.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/render.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       60 2023-04-28 22:07:13.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/rtd.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/plugins/scaffolding/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2023-05-04 01:46:11.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/scaffolding/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1156 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/scaffolding/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5126 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/src.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      438 2023-05-06 20:32:17.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/tests.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      388 2023-05-05 13:11:16.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/tox.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1266 2023-04-30 17:56:47.000000 pynchon-2023.5.7.2.25/src/pynchon/plugins/util.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/shimport/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      654 2023-05-06 18:35:05.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      732 2023-05-06 18:35:05.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/abcs.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       31 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/hooks.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       35 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/importing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    12466 2023-05-06 15:53:00.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/models.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2127 2023-05-06 17:17:04.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/module.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/registry.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       31 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/types.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      538 2023-05-01 23:36:05.000000 pynchon-2023.5.7.2.25/src/pynchon/shimport/util.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       73 2023-04-30 02:08:52.000000 pynchon-2023.5.7.2.25/src/pynchon/tagging.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.351772 pynchon-2023.5.7.2.25/src/pynchon/templates/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/.gitkeep
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.351772 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1908 2023-05-06 22:13:53.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/.gitignore
+-rw-rw-r--   0 matt      (1000) matt      (1000)      169 2023-05-06 22:12:35.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/.isort.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2540 2023-05-06 22:14:24.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/Makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-06 22:14:43.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)      753 2023-05-06 22:16:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/cookiecutter.json
+-rw-rw-r--   0 matt      (1000) matt      (1000)      979 2023-05-06 22:12:29.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2944 2023-05-06 22:14:13.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)      741 2023-05-07 00:20:00.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/setup.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2240 2023-05-06 22:12:43.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/tox.ini
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.351772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.351772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.363772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/bootstrap/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1150 2023-05-06 23:17:53.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/bootstrap/bash.sh
+-rw-rw-r--   0 matt      (1000) matt      (1000)      799 2023-05-07 04:20:42.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/bootstrap/bashrc.sh
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-03 01:10:30.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/bootstrap/makefile.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-03 01:10:24.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/bootstrap/python.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-03 01:10:13.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/bootstrap/sh.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-03 01:10:02.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/bootstrap/tox.ini
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/github/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      295 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/github/header.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/Makefile.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/core/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      392 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/fixme/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      164 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.351772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1190 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      891 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      322 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2985 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/cli/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      623 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/cli/cli-toc.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      198 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/cli/detail.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      253 2023-05-01 23:44:40.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/cli/main.module.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.355772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/src/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/src/header/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       50 2023-05-06 18:19:25.000000 pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      284 2023-04-27 22:45:44.000000 pynchon-2023.5.7.2.25/src/pynchon/testing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/util/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2084 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/util/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1016 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/util/click.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4782 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/util/complexity.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      871 2023-04-30 02:08:52.000000 pynchon-2023.5.7.2.25/src/pynchon/util/config.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/util/console/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/util/console/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-05-06 21:03:41.000000 pynchon-2023.5.7.2.25/src/pynchon/util/console/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      577 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/util/events.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/util/files/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6833 2023-05-07 06:24:37.000000 pynchon-2023.5.7.2.25/src/pynchon/util/files/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      945 2023-05-06 16:39:51.000000 pynchon-2023.5.7.2.25/src/pynchon/util/files/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2364 2023-05-06 04:31:40.000000 pynchon-2023.5.7.2.25/src/pynchon/util/lme.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      954 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/util/oop.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4260 2023-05-07 06:24:37.000000 pynchon-2023.5.7.2.25/src/pynchon/util/os.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2279 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/util/python.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/util/shfmt/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2545 2023-05-07 06:22:48.000000 pynchon-2023.5.7.2.25/src/pynchon/util/shfmt/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      316 2023-05-07 06:24:37.000000 pynchon-2023.5.7.2.25/src/pynchon/util/shfmt/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2416 2023-05-07 06:24:37.000000 pynchon-2023.5.7.2.25/src/pynchon/util/shfmt/grammar.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2802 2023-05-04 03:42:16.000000 pynchon-2023.5.7.2.25/src/pynchon/util/tagging.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      411 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/util/testing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/util/text/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      837 2023-05-02 00:54:17.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      365 2023-05-01 23:36:05.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/__main__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/util/text/loadf/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5301 2023-05-01 23:36:05.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/loadf/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1033 2023-05-01 23:36:05.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/loadf/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1654 2023-05-02 18:49:46.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/loads.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.367772 pynchon-2023.5.7.2.25/src/pynchon/util/text/normalize/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      740 2023-04-30 03:53:04.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/normalize/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       40 2023-04-29 02:48:43.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/normalize/__main__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.371772 pynchon-2023.5.7.2.25/src/pynchon/util/text/render/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5197 2023-05-03 01:18:56.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/render/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      963 2023-05-01 23:36:05.000000 pynchon-2023.5.7.2.25/src/pynchon/util/text/render/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1171 2023-05-01 23:36:05.000000 pynchon-2023.5.7.2.25/src/pynchon/util/typing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-07 06:25:11.355772 pynchon-2023.5.7.2.25/src/pynchon.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      735 2023-05-07 06:25:11.000000 pynchon-2023.5.7.2.25/src/pynchon.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6282 2023-05-07 06:25:11.000000 pynchon-2023.5.7.2.25/src/pynchon.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-07 06:25:11.000000 pynchon-2023.5.7.2.25/src/pynchon.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       46 2023-05-07 06:25:11.000000 pynchon-2023.5.7.2.25/src/pynchon.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-07 06:25:11.000000 pynchon-2023.5.7.2.25/src/pynchon.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      399 2023-05-07 06:25:11.000000 pynchon-2023.5.7.2.25/src/pynchon.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        8 2023-05-07 06:25:11.000000 pynchon-2023.5.7.2.25/src/pynchon.egg-info/top_level.txt
```

### Comparing `pynchon-2023.5.2.14.50/PKG-INFO` & `pynchon-2023.5.7.2.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2023.5.2.14.50
+Version: 2023.5.7.2.25
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
```

### Comparing `pynchon-2023.5.2.14.50/README.md` & `pynchon-2023.5.7.2.25/README.md`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/pyproject.toml` & `pynchon-2023.5.7.2.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/setup.cfg` & `pynchon-2023.5.7.2.25/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >3.6
 install_requires = 
 	click
-	coloredlogs==15.0.1
 	memoized-property==1.0.3
 	memoization==0.4.0
 	pyjson5==1.6.1
 	pygments
 	Jinja2==3.1.2
 	griffe==0.23.0
 	mccabe==0.7.0
@@ -41,14 +40,15 @@
 	tomli_w==1.0.0
 	pydash==7.0.1
 	enlighten==1.11.2
 	rich==13.3.4
 	multipledispatch==0.6.0
 	blinker==1.6.2
 	pydantic
+	cookiecutter==2.1.1
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `pynchon-2023.5.2.14.50/setup.py` & `pynchon-2023.5.7.2.25/src/pynchon/templates/cookie_cutter/pypkg/{{cookiecutter.project_slug}}/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+""" setup
+"""
 import os
+
 from setuptools import setup
 
 GIT_COMMIT = os.environ.get('GIT_COMMIT', 'local')
 if os.environ.get('PYPI_RELEASE', None):
     USE_CALVER = f"%Y.%m.%d.%H.%M"
 else:
     USE_CALVER = f"%Y.%m.%d+{GIT_COMMIT}"
@@ -10,15 +13,15 @@
 if __name__ == "__main__":
 
     try:
         setup(
             # use_calver=f"%Y.%m.%d.%H.%M+{GIT_COMMIT}",
             use_calver=USE_CALVER,
             setup_requires=['calver'],
-            )
+        )
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
         )
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/abcs/attrdict.py` & `pynchon-2023.5.7.2.25/src/pynchon/abcs/attrdict.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/abcs/config.py` & `pynchon-2023.5.7.2.25/src/pynchon/abcs/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ pynchon.abcs.config
 """
 from pynchon.util import typing, lme
+from pynchon.fleks.meta import Meta
 from pynchon.util.tagging import tags
 
-from .meta import Meta
-
 LOGGER = lme.get_logger(__name__)
 
 
 class Config(
     dict,
     metaclass=Meta,
 ):
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/abcs/path.py` & `pynchon-2023.5.7.2.25/src/pynchon/abcs/path.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,28 @@
 
 LOGGER = lme.get_logger(__name__)
 
 
 class Path(typing.PathType):
     """ """
 
+    def path_truncated(self):
+        """ """
+        return self.parents[0] / self.stem_truncated()
+
+    def full_extension(self):
+        """
+        no extension truncation, i.e. `.tar.gz`
+        """
+        return self.name[self.name.find('.') :]
+
+    def stem_truncated(self):
+        """truncated stem"""
+        return self.name[: self.name.rfind(self.full_extension())]
+
     def siblings(self):
         return self.parents[0].list()
 
     def match_any_glob(self, exclude_patterns: typing.List[str], quiet: bool = True):
         for exclude in exclude_patterns:
             match = self.match_glob(exclude)
             if match:
@@ -34,15 +48,33 @@
     def list(self) -> typing.List[str]:
         return [x for x in os.listdir(str(self))]
 
 
 class JSONEncoder(json.JSONEncoder):
     """ """
 
+    def encode(self, obj):
+        """ """
+        result = None
+
+        def default():
+            return super(JSONEncoder, self).encode(obj)
+
+        try:
+            toJSON = getattr(obj, 'toJSON', default) or default
+        except (Exception,) as exc:
+            toJSON = default
+        return toJSON()
+
+    # FIXME: use multimethod
     def default(self, obj):
+        toJSON = getattr(obj, 'toJSON', None)
+        if toJSON is not None:
+            LOGGER.debug(f'{type(object)} brings custom toJSON')
+            return obj.toJSON()
         if isinstance(obj, Path):
             return str(obj)
         if isinstance(obj, MappingProxyType):
             return dict(obj)
         if isinstance(obj, map):
             return list(obj)
-        return json.JSONEncoder.default(self, obj)
+        return super(JSONEncoder, self).default(obj)
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/abcs/plugin.py` & `pynchon-2023.5.7.2.25/src/pynchon/fleks/plugin.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/abcs/visitor.py` & `pynchon-2023.5.7.2.25/src/pynchon/abcs/visitor.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/annotate.py` & `pynchon-2023.5.7.2.25/src/pynchon/annotate.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/api/project/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/api/render.py` & `pynchon-2023.5.7.2.25/src/pynchon/api/render.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Looking for the JinjaPlugin?  See pynchon.plugins.jinja
 """
 
 import os
 import functools
 
 import pynchon
-from pynchon import abcs
+from pynchon import abcs, events
 
 from pynchon.util import typing, lme  # noqa
 
 LOGGER = lme.get_logger(__name__)
 import jinja2  # noqa
 from jinja2 import Environment  # Template,; UndefinedError,
 from jinja2 import FileSystemLoader, StrictUndefined
@@ -25,54 +25,76 @@
 
     return JinjaDict(input).render(context)
 
 
 @functools.lru_cache(maxsize=None)
 def get_jinja_globals():
     """ """
+    events.lifecycle.send(__name__, msg='finalizing jinja globals')
 
     def invoke_helper(*args, **kwargs) -> typing.StringMaybe:
         """
         A jinja filter/extension
         """
         from pynchon.util.os import invoke
 
         out = invoke(*args, **kwargs)
         assert out.succeeded
         return out.stdout
 
-    return dict(invoke=invoke_helper, env=os.getenv)
+    return dict(
+        sh=invoke_helper,
+        bash=invoke_helper,
+        invoke=invoke_helper,
+        map=map,
+        eval=eval,
+        env=os.getenv,
+    )
 
 
 @functools.lru_cache(maxsize=None)
 def get_jinja_env(*includes, quiet: bool = False):
-    """
-    FIXME: Move to pynchon.api.render
-    """
+    """ """
+    events.lifecycle.send(__name__, msg='finalizing jinja-Env')
     includes = list(includes)
     ptemp = abcs.Path(pynchon.__file__).parents[0] / 'templates' / 'includes'
     includes += [ptemp]
     includes = [abcs.Path(t) for t in includes]
 
     for template_dir in includes:
         if not template_dir.exists:
             err = f"template directory @ `{template_dir}` does not exist"
             raise ValueError(err)
     # includes and (not quiet) and LOGGER.warning(f"Includes: {includes}")
     env = Environment(
         loader=FileSystemLoader([str(t) for t in includes]),
         undefined=StrictUndefined,
     )
+    env.pynchon_includes = includes
 
     env.globals.update(**get_jinja_globals())
 
     known_templates = list(map(abcs.Path, set(env.loader.list_templates())))
-    # known_templates = [str(p) for p in known_templates if dot not in p.parents]
 
     if known_templates:
         from pynchon.util import text as util_text
 
         msg = "Known template search paths (includes folders only): "
-        # LOGGER.warning(msg)
         tmp = list(set([p.parents[0] for p in known_templates]))
         LOGGER.info(msg + util_text.to_json(tmp))
     return env
+
+
+def get_template(
+    template_name: str,
+    env=None,
+):
+    """ """
+    env = env or get_jinja_env()
+    try:
+        return env.get_template(template_name)
+    except (jinja2.exceptions.TemplateNotFound,) as exc:
+        LOGGER.critical(f"Template exception: {exc}")
+        LOGGER.critical(f"Jinja-includes: {env.pynchon_includes}")
+        err = getattr(exc, 'templates', exc.message)
+        LOGGER.critical(f"Problem template: {err}")
+        raise
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/app.py` & `pynchon-2023.5.7.2.25/src/pynchon/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,19 @@
 import atexit
 
 import enlighten
 from rich.text import Text
 from rich.console import Console, Theme
 from memoized_property import memoized_property
 
+from pynchon import events
 from pynchon.util import lme
 
 LOGGER = lme.get_logger(__name__)
 
-import blinker
-
-
-class Events:
-    lifecycle = blinker.signal('lifecyle')
-    bootstrap = blinker.signal('bootstrap')
-
-
-events = Events()
-
 
 class AppBase(object):
     pass
 
 
 class AppConsole(AppBase):
     Text = Text
@@ -47,20 +38,19 @@
     #         # LOGGER.critical(f"STAGE ({tmp}): {stage}")
     #         self.status_bar.update(stage=stage)
 
     @memoized_property
     def status_bar(self):
         """ """
         tmp = self.manager.status_bar(
-            status_format=u'{app}{fill}{stage}:{fill}{msg}{fill}{elapsed}',
+            status_format=u'{app}{fill}{stage}{fill}{elapsed}',
             color='bold_underline_bright_white_on_lightslategray',
             justify=enlighten.Justify.LEFT,
             app='Pynchon',
             stage='...',
-            msg='...',
             autorefresh=True,
             min_delta=0.1,
         )
 
         atexit.register(
             lambda: self.events.lifecycle.send(self, stage="\o/", msg='')
         )  # noqa: W605
@@ -113,60 +103,42 @@
         self.exception = exc
         self._orig_exc_handler(self, exc_type, exc, *args)
 
     def sys_exit_handler(self):
         if self.exit_code is not None and not self.exit_code == 0:
             tmp = f"death by sys.exit({self.exit_code})"
             self.events.lifecycle.send(self, stage=tmp)
-            # status.update(stage=tmp)
+            return True
 
     def exit_handler(self):
         """ """
         handled = self.sys_exit_handler()
         handled = handled or self.exc_exit_handler()
-        handled = handled or self.def_exit_handler()
+        handled = handled or self.default_exit_handler()
         return handled
 
     def exc_exit_handler(self):
         """ """
         if self.exception is not None:
             text = f"Exception: {self.exception}"
             text = self.Text(text)
             text.stylize('bold red', 0, 6)
             self.console.print(text)
             self.events.lifecycle.send(self, stage='❌')
 
-    def def_exit_handler(self):
+    def default_exit_handler(self):
         """ """
         # LOGGER.info("ok")
         return True
 
 
 class AppEvents(AppBase):
     def __init__(self, **kwargs):
         """ """
         self.events = events
-        events.lifecycle.connect(self.lifecycle_msg)
-        events.lifecycle.connect(self.lifecycle_stage)
-
-    # FIXME: use multi-dispatch over kwargs and define `lifecyle` repeatedly
-    def lifecycle_stage(self, sender, stage=None, **kwargs):
-        """ """
-        if stage:
-            tmp = getattr(sender, '__name__', str(sender))
-            # LOGGER.critical(f"STAGE ({tmp}): {stage}")
-            self.status_bar.update(stage=stage)
-
-    # FIXME: use multi-dispatch over kwargs and define `lifecyle` repeatedly
-    def lifecycle_msg(self, sender, msg=None, **kwargs):
-        """ """
-        if msg:
-            tmp = getattr(sender, 'name', getattr(sender, '__name__', str(sender)))
-            LOGGER.critical(f"LIFECYCLE ({tmp}): {msg}")
-            self.status_bar.update(msg=msg)
 
 
 class App(AppConsole, AppEvents, AppExitHooks):
     def __init__(self, **kwargs):
         """ """
         AppConsole.__init__(self, **kwargs)
         AppEvents.__init__(self, **kwargs)
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/bin/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/bin/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,9 +22,11 @@
     try:
         p_entry = init_fxn()
     except (Exception,) as exc:
         LOGGER.critical(f"  failed to initialize cli for {plugin_kls.__name__}:")
         LOGGER.critical(f"    {exc}")
         if name == 'core':
             raise
+        else:
+            raise
     else:
         registry[name] = dict(plugin=plugin_kls, entry=p_entry)
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/bin/entry.py` & `pynchon-2023.5.7.2.25/src/pynchon/bin/entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 pynchon: a utility for docs generation and template-rendering
 """
 import collections
 from gettext import gettext as _
 
-from pynchon import abcs, click, shimport
+from pynchon import fleks, abcs, cli, shimport
 
 from pynchon.util import lme, typing  # noqa
 
-
-# import click
-
-
+click = cli.click
 plugins = shimport.lazy(
     'pynchon.plugins',
 )
 
 
 class RootGroup(click.Group):
     """ """
@@ -43,15 +40,15 @@
             toplevel = dict(core=[], plugins=collections.defaultdict(list))
             for subcommand, cmd in commands:
                 help = cmd.get_short_help_str(limit)
                 is_plugin = subcommand in plugin_subs
                 label = ''
                 if is_plugin:
                     plugin_kls = plugin_subs[subcommand]['kls']
-                    if issubclass(plugin_kls, (abcs.Plugin,)):
+                    if issubclass(plugin_kls, (fleks.Plugin,)):
                         tmp = plugin_kls.cli_label
                         toplevel['plugins'][tmp].append(
                             (f"{subcommand}:", f"{cmd.help}")
                         )
                 else:
                     toplevel['core'].append((f"{subcommand}:", f"{cmd.help}"))
                 # category.append((f"{subcommand}", f"{label}{help}"))
@@ -79,19 +76,23 @@
     def format_usage(self, ctx, formatter):
         """ """
         # terminal_width, _ = click.get_terminal_size()
         terminal_width = 30
         click.echo('-' * terminal_width)
         super(RootGroup, self).format_usage(ctx, formatter)
 
+    def get_command(self, *args, **kwargs):
+        tmp = super(RootGroup, self).get_command(*args, **kwargs)
+        return tmp
+
 
 @click.version_option()
 @click.option('--plugins', help='shortcut for `--set plugins=...`')
 @click.option('--set', 'set_config', help='config overrides')
 @click.option('--get', 'get_config', help='config retrieval')
 @click.group("pynchon", cls=RootGroup)
 def entry(
     plugins: str = '',
     set_config: str = '',  # noqa
     get_config: str = '',
 ):
-    pass
+    """ """
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/cli/common.py` & `pynchon-2023.5.7.2.25/src/pynchon/cli/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # import io
 import json
 import functools
 
 import click
 from rich import print_json
 
-from pynchon.util import lme, typing
+from pynchon.util import text
+
+from pynchon.util import lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
 def load_groups_from_children(root=None, parent=None):
     from pynchon import shimport
     from pynchon.cli import click
@@ -28,28 +30,14 @@
         lambda name, fxn: [
             setattr(fxn, 'name', name),
             click.group_copy(fxn, parent),
         ]
     )
 
 
-# from rich.console import Console
-# class BetterGroup(click.Group):
-#     def format_usage(self,ctx,formatter):
-#         super(BetterGroup,self).format_usage(ctx,formatter)
-#     def format_epilog(self,ctx,formatter):
-#         return super(BetterGroup,self).format_epilog(ctx,formatter)
-#     def format_help(self, ctx, formatter):
-#         super(BetterGroup,self).format_help(ctx,formatter)
-#     def format_options(self,ctx,formatter):
-#         super(BetterGroup,self).format_options(ctx,formatter)
-#     def format_help_text(self,ctx,formatter):
-#         super(BetterGroup,self).format_help_text(ctx,formatter)
-
-
 class handler(object):
     """ """
 
     priority = -1
 
     def __init__(self, parent=None):
         self.parent = parent
@@ -209,47 +197,50 @@
 
     def wrapper(self, *args, **call_kwargs):
         """ """
         assert self.fxn
 
         @functools.wraps(self.fxn)
         def newf(*args, **call_kwargs):
-            self.logger.debug(f"Invoking {self.parent.name}.{self.name}")
-            self.logger.debug(f" with: {call_kwargs}")
+            self.logger.info(f"Wrapping invocation: {self.parent.name}.{self.name}")
+            call_kwargs and self.logger.debug(f" with: {call_kwargs}")
             result = self.fxn(*args, **call_kwargs)
-
-            # for tformer in self.transformers:
-            #     if tformer.match(call_kwargs):
-            #         result = tformer.transform(result, **call_kwargs)
-            # for handler in self.handlers:
-            #     if handler.match(call_kwargs):
-            #         self.logger.debug(f"Handling with `{handler.__class__.__name__}`")
-            #         handler.handle(result, **call_kwargs)
-            from pynchon.util.text import to_json
-
-            print(to_json(result))
+            if result is not None:
+                result and LOGGER.info(f'json conversion for type: {type(result)}')
+                tmp = text.to_json(result)
+                print(tmp)
             return result
 
         return newf
 
     def __call__(self, fxn: typing.Callable):
         """ """
         self.fxn = fxn
         assert fxn, 'function cannot be None!'
-        f = self.cmd(self.wrapper())
 
-        f.help = ' '.join(
-            [x.strip() for x in (f.help or fxn.__doc__ or "").split('\n')]
-        ).lstrip()
+        f = self.cmd(self.wrapper())
+        tmp = [x.strip() for x in (f.help or fxn.__doc__ or "").split('\n')]
+        f.help = ' '.join(tmp).lstrip()
 
         for opt in self.options:
             f = opt(f)
         for arg in self.arguments:
             f = arg(f)
-        # import IPython; IPython.embed()
-        # for opt_or_arg in click_params:
-        #     f=opt_or_arg(f)
         return f
 
 
 class groop(kommand):
+    """
+    # class BetterGroup(click.Group):
+    #     def format_usage(self,ctx,formatter):
+    #         super(BetterGroup,self).format_usage(ctx,formatter)
+    #     def format_epilog(self,ctx,formatter):
+    #         return super(BetterGroup,self).format_epilog(ctx,formatter)
+    #     def format_help(self, ctx, formatter):
+    #         super(BetterGroup,self).format_help(ctx,formatter)
+    #     def format_options(self,ctx,formatter):
+    #         super(BetterGroup,self).format_options(ctx,formatter)
+    #     def format_help_text(self,ctx,formatter):
+    #         super(BetterGroup,self).format_help_text(ctx,formatter)
+    """
+
     is_group = True
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/cli/options.py` & `pynchon-2023.5.7.2.25/src/pynchon/cli/options.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/click.py` & `pynchon-2023.5.7.2.25/src/pynchon/cli/click.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """ pynchon.click
 """
 import click
 
 from click import (  # noqa
     echo,
+    pass_context,
+    get_current_context,
     argument,
     option,
     version_option,
     command,
     Command,
     group,
     Group,
@@ -63,14 +65,30 @@
 #                 self._previous_parser_process = our_parser.process
 #                 our_parser.process = parser_process
 #                 break
 #         # raise Exception(locals())
 #         return retval
 
 
+def walk_group(parent, path='', tree={}):
+    """ """
+    tree = {
+        **tree,
+        **{
+            f"{path} {sub}": sub
+            for sub, item in parent.commands.items()
+            if isinstance(item, (Command,))
+        },
+    }
+    for sub, item in parent.commands.items():
+        if isinstance(item, (Group,)):
+            tree.update(**walk_group(item, path=f'{path} {sub}'))
+    return tree
+
+
 def group_merge(g1: click.Group, g2: click.Group):
     """ """
 
     def fxn():
         pass
 
     fxn.__doc__ = g1.help
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/config/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/config/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 """ pynchon.config
 """
 # from pynchon import abcs
 from pynchon.api import render
 from pynchon.app import app
 from pynchon.core import Config as CoreConfig
 from pynchon.util import lme  # typing
-from pynchon.abcs.plugin import Meta
+from pynchon.fleks.plugin import Meta
 
 from .util import config_folders  # noqa
 from .util import load_config_from_files  # noqa
 from .util import get_config_files  # noqa
 from .util import finalize  # noqa
 from pynchon.plugins.git import GitConfig  # noqa
 
 LOGGER = lme.get_logger(__name__)
 events = app.events
 
 # FIXME: abstract into phases inside pynchon.app
 msg = "Loading raw-config from OS.."
-# LOGGER.critical(msg)
 events.lifecycle.send(__name__, stage=msg)
 git = GIT = GitConfig()
 
 msg = "Building raw-config from files.."
-# LOGGER.critical(msg)
 events.lifecycle.send(
     __name__,
     msg=msg,
     stage=msg,
 )
-
 CONFIG_FILES = []
 MERGED_CONFIG_FILES = {}
 for cfg_src, config in load_config_from_files().items():
     MERGED_CONFIG_FILES = {**MERGED_CONFIG_FILES, **config}
     config and CONFIG_FILES.append(cfg_src)
 
 # NB: this content is potentially templated
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/config/util.py` & `pynchon-2023.5.7.2.25/src/pynchon/config/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,82 @@
-"""
+""" pynchon.config.util
 """
 import os
 import functools
+import collections
 from types import MappingProxyType
-from collections import OrderedDict
 
 import pyjson5
 
-from pynchon import abcs
+from pynchon import abcs, events
+from pynchon import config as config_module
 from pynchon.util import typing, lme
+from pynchon.plugins.util import PluginNotRegistered, get_plugin
 
 LOGGER = lme.get_logger(__name__)
 
 
 @functools.lru_cache(maxsize=100, typed=False)
 def finalize():
-    from pynchon import config
-    from pynchon.plugins import get_plugin
 
     result = abcs.AttrDict(
         pynchon=MappingProxyType(
-            dict([[k, v] for k, v in config.RAW.items() if not isinstance(v, (dict,))])
+            dict(
+                [
+                    [k, v]
+                    for k, v in config_module.RAW.items()
+                    if not isinstance(v, (dict,))
+                ]
+            )
         ),
-        git=config.GIT,
+        git=config_module.GIT,
     )
     plugins = []
-    from pynchon.plugins.util import PluginNotRegistered
 
     pnames = result.pynchon['plugins']
     for pname in pnames:
         try:
             tmp = get_plugin(pname)
         except (PluginNotRegistered,) as exc:
-            LOGGER.critical(exc)
+            LOGGER.critical(f"PluginNotRegistered: {exc}")
             continue
         else:
             plugins.append(tmp)
-    # raise Exception(plugins)
-    from pynchon import config as THIS_MODULE
-    from pynchon.app import app
 
-    events = app.events
     for plugin_kls in plugins:
         pconf_kls = getattr(plugin_kls, 'config_class', None)
+        conf_key = plugin_kls.get_config_key()
         if pconf_kls is None:
-            LOGGER.warning(f"{plugin_kls.__name__}.`config_class` not set!")
             plugin_config = abcs.Config()
         else:
-
-            # plugin_defaults = getattr(plugin_kls,'defaults',None)
-            # if plugin_defaults is not None:
-            #     raise Exception(plugin_kls)
             # NB: module access
-            user_defaults = config.USER_DEFAULTS.get(plugin_kls.name, {})
             user_defaults = (
-                config.PYNCHON_CORE if plugin_kls.name == 'base' else user_defaults
+                config_module.PYNCHON_CORE
+                if plugin_kls.name == 'base'
+                else config_module.USER_DEFAULTS.get(plugin_kls.name, {})
             )
-            # user_defaults = user_defaults if not
-            if pconf_kls is None:
-                LOGGER.warning(f"{plugin_kls} does not define `config_class`")
-                conf_key = None
-                plugin_config = {}
-            else:
-                conf_key = getattr(
-                    pconf_kls, 'config_key', plugin_kls.name.replace('-', '_')
-                )
-                if not conf_key:
-                    msg = f'failed to determine conf-key for {pconf_kls}'
-                    LOGGER.critical(msg)
-                    raise TypeError(msg)
-                plugin_config = pconf_kls(
-                    **{
-                        # **plugin_defaults,
-                        **user_defaults,
-                    }
-                )
-                setattr(THIS_MODULE, conf_key, plugin_config)
-                result.update({conf_key: plugin_config})
-
-            plugin_obj = plugin_kls(final=plugin_config)
-            from pynchon.plugins import registry as plugins_registry
-
-            # plugins_registry.register(plugin_obj)
-            plugins_registry[plugin_kls.name]['obj'] = plugin_obj
-            events.lifecycle.send(plugin_obj, msg=f'finalized {plugin_kls.__name__}')
+            plugin_config = pconf_kls(
+                **{
+                    # **plugin_defaults,
+                    **user_defaults,
+                }
+            )
+        setattr(config_module, conf_key, plugin_config)
+        result.update({conf_key: plugin_config})
+
+        plugin_obj = plugin_kls(final=plugin_config)
+        from pynchon.plugins import registry as plugins_registry
+
+        # plugins_registry.register(plugin_obj)
+        plugins_registry[plugin_kls.name]['obj'] = plugin_obj
+        events.lifecycle.send(plugin_obj, plugin=f'finalized {plugin_kls.__name__}')
+    # for msg, offenders in warnings.items():
+    #     offenders = [x.__name__ for x in offenders]
+    #     LOGGER.warning(f"{msg}")
+    #     LOGGER.warning(f"offenders={offenders}")
     return result
 
 
 def get_config_files():
     """ """
 
     if os.environ.get('PYNCHON_CONFIG', None):
@@ -119,15 +108,15 @@
     return [abcs.Path(f) for f in folders]
 
 
 def load_config_from_files() -> typing.Dict[str, str]:
     """ """
     from pynchon.util import python
 
-    contents = OrderedDict()
+    contents = collections.OrderedDict()
     for src in get_config_files():
         if not src.exists():
             LOGGER.warning(f"src@`{src}` doesn't exist, skipping it")
             continue
         if src.name.endswith('pyproject.toml'):
             LOGGER.info(f"Loading from toml: {src}")
             tmp = python.load_pyprojecttoml(path=src)
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/constants.py` & `pynchon-2023.5.7.2.25/src/pynchon/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """ pynchon.constants
 """
+import os
+
+LOG_LEVEL = os.environ.get('PYNCHON_LOG_LEVEL', 'WARNING')
 DEFAULT_PLUGINS = [
     # FIXME: docs
     "core",
     "plugins",
     "project",
     "globals",
     "git",
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/core.py` & `pynchon-2023.5.7.2.25/src/pynchon/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class Config(abcs.Config):
     """ """
 
     priority = 1
     config_key = "pynchon"
     defaults = dict(
         version=__version__,
-        src_root=abcs.Path("."),
+        # src_root=abcs.Path("."),
         plugins=list(set(constants.DEFAULT_PLUGINS)),
     )
 
     def validate_plugins(self, plugin_list: typing.List = []):
         """ """
         # LOGGER.warning('skipping plugin validation..')
         defaults = set(constants.DEFAULT_PLUGINS)
@@ -66,16 +66,15 @@
         from pynchon import config
 
         root = self.get("root")
         root = root or os.environ.get("PYNCHON_ROOT")
         root = root or config.GIT.get("root")
         return root and abcs.Path(root)
 
-    @tagging.tags(conflict_strategy='override')
-    @property
+    @tagging.tagged_property(conflict_strategy='override')
     def plugins(self):
         result = sorted(
             list(set(self.get('plugins', []) + self.__class__.defaults['plugins']))
         )
         self['plugins'] = result
         return result
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/models.py` & `pynchon-2023.5.7.2.25/src/pynchon/models/plugin_types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,118 @@
-""" pynchon.models
 """
-from pynchon.util import typing, lme  # noqa
+"""
+import typing
 
-from pynchon import shimport
-from pynchon.api import project
-from pynchon.app import app
+from pynchon import api, cli, shimport
 from pynchon.bin import entry
-from pynchon.cli import click, common
-from pynchon.abcs.plugin import Plugin as AbstractPlugin
+from pynchon.fleks.plugin import Plugin as AbstractPlugin
 from pynchon.plugins.util import get_plugin_obj
 from pynchon.util.tagging import tags
 
-from pynchon.util import lme, typing  # noqa
+from pynchon.util import typing, lme  # noqa
+
 
 config_mod = shimport.lazy(
     'pynchon.config',
 )
 
 LOGGER = lme.get_logger(__name__)
-events = app.events
+
+
+import collections
+
+
+def v_require_conf_key(kls, **vdata):
+    """ """
+    pconf_kls = getattr(kls, 'config_class', None)
+    conf_key = getattr(pconf_kls, 'config_key', kls.name.replace('-', '_'))
+    if not conf_key:
+        msg = f'failed to determine conf-key for {kls}'
+        LOGGER.critical(msg)
+        raise PynchonPlugin.PluginMalformed(msg)
+    return vdata
+
+
+def v_warn_config_kls(kls, warnings=collections.defaultdict(list), **vdata):
+    pconf_kls = getattr(kls, 'config_class', None)
+    if pconf_kls is None:
+        warnings["`config_kls` not set!"].append(kls)
+    vdata.update(warnings=warnings)
+    return vdata
 
 
 @tags(cli_label='<<Abstract>>')
 class PynchonPlugin(AbstractPlugin):
     """
     Pynchon-specific plugin-functionality
     """
 
+    name = '<<Abstract>>'
     cli_label = '<<Abstract>>'
+    __class_validators__ = [
+        v_require_conf_key,
+        v_warn_config_kls,
+    ]
 
-    @property
-    def plugin_config(self):
-        """ """
-        return self.get_current_config()
+    @typing.classproperty
+    def instance(kls):
+        """class-property: the instance for this plugin"""
+        return get_plugin_obj(kls.name)
 
     @typing.classproperty
     def project_config(self):
         """class-property: finalized project-config"""
-        return project.get_config()
+        return api.project.get_config()
 
-    @typing.classproperty
-    def instance(kls):
-        """class-property: the instance for this plugin"""
-        return get_plugin_obj(kls.name)
+    @classmethod
+    def get_config_key(kls):
+        """ """
+        default = kls.name.replace('-', '_')
+        config_kls = getattr(kls, 'config_class', None)
+        return getattr(config_kls, 'config_key', default) or default
 
     @classmethod
     def get_current_config(kls):
         """class-method: get the current config for this plugin"""
-        assert kls.config_class
-        conf_key = getattr(kls.config_class, 'config_key', kls.name)
-        assert conf_key
+        conf_class = getattr(kls, 'config_class', None)
+        if conf_class is None:
+            return {}
+        conf_key = kls.get_config_key()
         result = getattr(config_mod, conf_key)
         return result
 
+    @property
+    def plugin_config(self):
+        """ """
+        return self.get_current_config()
+
+    @property
+    def active_plugins(self):
+        """ """
+        result = []
+        from pynchon.plugins import util as plugins_util
+        from pynchon.plugins import registry
+
+        for plugin in registry.keys():
+            if plugin == self.name:
+                continue
+            result.append(plugins_util.get_plugin_obj(plugin))
+        return sorted(result, key=lambda p: p.priority)
+
+    @property
     def config(self):
+        """ """
+        return self.cfg()
+
+    def cfg(self):
         """Shows current config for this plugin"""
         kls = self.__class__
-        LOGGER.debug(f"config class: {kls.config_class}")
+        conf_class = getattr(kls, 'config_class', None)
+        conf_class_name = conf_class.__name__ if conf_class else '(None)'
+        LOGGER.debug(f"config class: {conf_class_name}")
         LOGGER.debug("current config:")
         result = kls.get_current_config()
         return result
 
 
 @tags(cli_label='<<Default>>')
 class CliPlugin(PynchonPlugin):
@@ -81,50 +133,52 @@
             return cached
 
         def plugin_main():
             pass
 
         plugin_main.__doc__ = (kls.__doc__ or "").lstrip()
         gname = getattr(kls, 'cli_name', kls.name)
-        groop = common.groop(gname, parent=kls.click_entry)
+        groop = cli.common.groop(gname, parent=kls.click_entry)
         plugin_main = groop(plugin_main)
         kls._finalized_click_groups[kls] = plugin_main
         return plugin_main
 
-    @PynchonPlugin.classmethod_dispatch(click.Group)
-    def click_acquire(kls, grp: click.Group):  # noqa F811
+    @PynchonPlugin.classmethod_dispatch(cli.click.Group)
+    def click_acquire(kls, grp: cli.click.Group):  # noqa F811
         """ """
         parent = kls.click_group
         LOGGER.critical(
             f"{kls.__name__} acquires group@`{grp.name}` to: parent@`{parent.name}`"
         )
         raise NotImplementedError("groups are not supported yet!")
 
     @PynchonPlugin.classmethod_dispatch(typing.FunctionType)
     def click_acquire(kls, fxn: typing.FunctionType):  # noqa F811
         """ """
         msg = f'{kls.__name__} acquires naked fxn: {fxn.__name__}'
         assert fxn.__annotations__
         cmd_name = f'{fxn.__name__}'.replace('_', '-')
-        kls.click_group.add_command(click.command(cmd_name)(fxn))
+        kls.click_group.add_command(cli.click.command(cmd_name)(fxn))
 
-    @PynchonPlugin.classmethod_dispatch(click.Command)
-    def click_acquire(kls, cmd: click.Command):  # noqa F811
+    @PynchonPlugin.classmethod_dispatch(cli.click.Command)
+    def click_acquire(kls, cmd: cli.click.Command):  # noqa F811
         """ """
         parent = kls.click_group
         LOGGER.info(f"{kls.__name__} acquires {cmd.name} to: group@{parent.name}")
         parent.add_command(cmd)
         return parent
 
     @classmethod
     def init_cli(kls):
         """ """
-        LOGGER.info(f"{kls.__name__}.init_cli:")
+        from pynchon import events
         from pynchon.plugins.core import Core
 
+        events.lifecycle.send(kls, plugin='initializing CLI')
+
         if kls != Core:
             config_mod.finalize()
 
         obj = kls.instance
         if obj is None:
             err = f"{kls.__name__}.`instance` is not ready?"
             LOGGER.warning(err)
@@ -145,30 +199,40 @@
 
             def wrapper(*args, fxn=fxn, **kwargs):
                 LOGGER.debug(f"calling {fxn} from wrapper")
                 result = fxn(*args, **kwargs)
                 # FIXME: this wraps twice?
                 # from rich import print_json
                 # print_json(text.to_json(result))
+                # if hasattr(result, 'display'):
+                rproto = getattr(result, '__rich__', None)
+                if rproto:
+                    from pynchon.util.lme import CONSOLE
+
+                    CONSOLE.print(result)
+                # try:
+                #     renderable =rproto()
+                #     # getattr(result, 'display', lambda: None)()
+                # except KeyError:
+                #     pass
                 return result
 
             commands = [kls.click_create_cmd(fxn, wrapper=wrapper, alias=None)]
             for alias in click_aliases:
                 tmp = kls.click_create_cmd(
                     fxn,
                     alias=alias,
                     wrapper=wrapper,
                 )
                 commands.append(tmp)
             cli_commands += commands
 
-        # if method_name == 'bootstrap':
         msg = [cmd.name for cmd in cli_commands]
-        msg = ' | '.join(msg)
-        LOGGER.info(f" created commands: '{msg}'")
+        if len(msg) > 1:
+            events.lifecycle.send(kls, plugin=f'created {len(msg)} commands')
         kls.init_cli_children()
         return kls.click_group
 
     @classmethod
     def init_cli_children(kls):
         """ """
         cli_subsumes = getattr(kls, 'cli_subsumes', [])
@@ -183,111 +247,67 @@
         """ """
         assert fxn
         assert wrapper
         name = alias or fxn.__name__
         name = name.replace('_', '-')
         help = f'(alias for `{alias}`)' if alias else (fxn.__doc__ or "")
         help = help.lstrip()
-        cmd = common.kommand(
+        cmd = cli.common.kommand(
             name,
             help=help,
             alias=alias,
             parent=kls.click_group,
         )(wrapper)
         options = getattr(fxn, '__click_params__', [])
         cmd.params += options
         return cmd
 
 
 @tags(cli_label='Provider')
 class Provider(CliPlugin):
     """
-    ProviderPlugin provides context-information, but little other functionality
+    ProviderPlugin provides context-information,
+    but little other functionality
     """
 
     cli_label = 'Provider'
     contribute_plan_apply = False
-    # class config_class(abcs.Config):
-    #     config_key = None
-
-
-@tags(cli_label='NameSpace')
-class NameSpace(CliPlugin):
-    """
-    `CliNamespace` collects functionality
-    from elsewhere under a single namespace
-    """
-
-    cli_label = 'NameSpace'
-    contribute_plan_apply = False
-    priority = -1
+    priority = 2
+    __class_validators__ = [
+        v_require_conf_key,
+        # v_warn_config_kls,
+    ]
 
 
 @tags(cli_label='Tool')
 class ToolPlugin(CliPlugin):
     """
-    Tool plugins may have their own config, but generally should not need project-config.
+    Tool plugins may have their own config,
+    but generally should not need project-config.
     """
 
     cli_label = 'Tool'
     contribute_plan_apply = False
+    __class_validators__ = [
+        # v_require_conf_key,
+        # v_warn_config_kls,
+    ]
 
 
 class BasePlugin(CliPlugin):
     """
     The default plugin-type most new plugins will use
     """
 
     priority = 10
 
 
-@tags(cli_label='Planner')
-class AbstractPlanner(BasePlugin):
-    """
-    AbstractPlanner is a plugin-type that provides plan/apply basics
-    """
-
-    cli_label = 'Planner'
-
-    def plan(self, config=None) -> typing.List:
-        """Creates a plan for this plugin"""
-        events.lifecycle.send(
-            # writes status event (used by the app-console)
-            stage=f"Planning for `{self.__class__.name}`"
-        )
-        self.state = config
-        return []
-
-    def apply(self, config=None) -> None:
-        """Executes the plan for this plugin"""
-        from pynchon.util.os import invoke
-
-        events.lifecycle.send(
-            # write status event (used by the app-console)
-            stage=f"applying for `{self.__class__.name}`"
-        )
-        plan = self.plan(config=config)
-        return [invoke(p).succeeded for p in plan]
-
-
-class ShyPlanner(AbstractPlanner):
+@tags(cli_label='NameSpace')
+class NameSpace(CliPlugin):
     """
-    ShyPlanner uses plan/apply workflows, but they must be
-    executed directly.  ProjectPlugin (or any other parent plugins)
-    won't include this as a sub-plan.
+    `CliNamespace` collects functionality
+    from elsewhere under a single namespace
     """
 
+    cli_label = 'NameSpace'
     contribute_plan_apply = False
-
-
-@tags(cli_label='Manager')
-class Manager(ShyPlanner):
-    cli_label = 'Manager'
-
-
-class Planner(ShyPlanner):
-    """
-    Planner uses plan/apply workflows, and contributes it's plans
-    to ProjectPlugin (or any other parent plugins).
-    """
-
-    contribute_plan_apply = True
+    priority = 1
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/core.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/python/platform.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-""" pynchon.plugins.Core
+""" pynchon.plugins.python.platform
 """
-from pynchon import models, cli
-from pynchon.api import project
-from pynchon.bin import entry
-from pynchon.core import Config as CoreConfig
-from pynchon.util import lme, typing
+import platform as stdlib_platform
+
+from memoized_property import memoized_property
+
+from pynchon import abcs, models
+from pynchon.util import typing, lme
+from pynchon.util.os import invoke
 
 LOGGER = lme.get_logger(__name__)
 
 
-class Core(models.Planner):
-    """Core Plugin"""
+class PythonPlatform(models.Provider):
+    """Context for python-platform"""
 
-    name = "core"
-    config_class = CoreConfig
-    contribute_plan_apply = False
-
-    @typing.classproperty
-    def click_group(kls):
-        kls._finalized_click_groups[kls] = entry.entry
-        return kls._finalized_click_groups[kls]
+    priority = 2
+    name = 'python'
 
-    @classmethod
-    def get_current_config(kls):
-        """ """
-        from pynchon import config as config_mod
+    class config_class(abcs.Config):
+        config_key = "python"
+        defaults = dict(
+            version=stdlib_platform.python_version(),
+        )
+
+        @memoized_property
+        def is_package(self) -> bool:
+            # self.logger.debug("checking if this a python package..")
+            cmd = invoke("python setup.py --version 2>/dev/null", log_command=False)
+            return cmd.succeeded
+
+        @property
+        def package(self) -> typing.Dict:
+            """ """
+            if self.is_package:
+                return PackageConfig()
+            else:
+                return {}
+
+
+class PackageConfig(abcs.Config):
+    parent = PythonPlatform.config_class
+    config_key = "package"
 
-        result = getattr(config_mod, getattr(kls.config_class, 'config_key', kls.name))
-        return result
+    @property
+    def name(self) -> str:
+        """ """
+        from pynchon.util import python
 
-    def plan(self, config=None) -> typing.List:
-        """Creates a plan for all plugins"""
-        raise NotImplementedError()
-
-    def apply(self, config=None) -> None:
-        """Executes the result returned by planner"""
-        raise NotImplementedError()
-
-    def config(self):
-        """Show current project config (with templating/interpolation)"""
-        return project.get_config()
-
-    @cli.click.option('--bash', default=False, is_flag=True, help='bootstrap bash')
-    def bootstrap(self, bash: bool = False, strict: bool = False) -> None:
-        """
-        bootstrappery
-        """
-        if bash:
-            return 'alias p=pynchon'
-
-    def raw(self) -> None:
-        """
-        Returns (almost) raw config,
-        without interpolation
-        """
-        from pynchon.config import RAW
+        return python.load_setupcfg().get("metadata", {}).get("name")
 
-        return RAW
+    @memoized_property
+    def version(self) -> str:
+        """ """
+        # self.logger.debug("resolving project version..")
+        cmd = invoke("python setup.py --version 2>/dev/null", log_command=False)
+        return cmd.succeeded and cmd.stdout.strip()
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/dot.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/dot.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         return list(
             set(
                 config.dot.get('exclude_patterns', [])
                 + config.globals['exclude_patterns']
             )
         )
 
-    def list(self, config=None):
+    def list(self, config=None) -> typing.List[str]:
         """ """
-        config = config or api.project.get_config()
+        config = config or self.project_config
         proj_conf = config.project.get("subproject", config.project)
         project_root = proj_conf.get("root", config.git["root"])
         search = [
             abcs.Path(project_root).joinpath("**/*.dot"),
         ]
         self.logger.debug(f"search pattern is {search}")
         result = files.find_globs(search)
@@ -95,44 +95,29 @@
             output = os.path.splitext(file)[0] + ".png"
         cmd = f"cat {file} | docker run --rm --entrypoint dot -i {img} -T{output_mode} > {output}"
         return invoke(cmd, system=True).succeeded
 
     def plan(
         self,
         config=None,
-    ) -> typing.List[str]:
+    ) -> models.Plan:
         config = config or api.project.get_config()
         plan = super(self.__class__, self).plan(config)
-        # render_instructions = self.render_instructions
-        # if "dot" in render_instructions:
         self.logger.debug("planning for rendering for .dot graph files..")
-        resources = self.list(config)
-        for rsrc in resources:
-            plan += [
-                f"pynchon dot render {rsrc} --in-place --output-mode png",
-            ]
-        # dot_config = config["pynchon"].get("dot", {})
-        # script = dot_config.get("script")
-        # # assert script, '`"dot" in pynchon.generate` but pynchon.dot.script is not set!'
-        # from pynchon.api import render
-        # # FIXME: do this substition everywhere!
-        # script = render._render(text=script, context=config)
-        # cmd = "pynchon gen dot files --script {script}"
-        # plan += [cmd]
+        cmd_t = "pynchon dot render {resource} --in-place --output-mode png"
+        for resource in self.list(config):
+            plan.append(
+                models.Goal(
+                    resource=resource,
+                    command=cmd_t.format(resource=resource),
+                    type='render',
+                )
+            )
         return plan
 
-    # @classmethod
-    # def init_cli(kls):
-    #     """
-    #     Option parsing for the `dot` subcommands
-    #     """
-    #     parent = kls.click_group
-    #     LOGGER = lme.get_logger(__name__)
-    #     files_arg = click.argument("files", nargs=-1)
-
     # @common.kommand(
     #     name="files",
     #     parent=parent,
     #     options=[
     #         options.script,
     #         options.includes,
     #         click.option(
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/fixme.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/fixme.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """ pynchon.plugins.fixme
 """
 from fnmatch import fnmatch
 
 from pynchon import constants, abcs, models
-from pynchon.cli import click, options, common
 from pynchon.util import typing, lme
 from pynchon.util.os import invoke
 
+from pynchon.cli import click, options, common  # noqa
+
 LOGGER = lme.get_logger(__name__)
 
 
 class FixMeConfig(abcs.Config):
     config_key = 'fixme'
 
 
@@ -19,67 +20,85 @@
 
     name = "fixme"
     config_class = FixMeConfig
     defaults = dict()
 
     def plan(self, config: dict = None) -> typing.List:
         """...."""
-        from pynchon.config import pynchon
-
         config = config or self.__class__.get_current_config()
         plan = super(self.__class__, self).plan(config)
-        plan += [f"pynchon fixme gen --output {pynchon['docs_root']}/FIXME.md"]
+        target = abcs.Path(self.project_config['docs']['root']) / 'FIXME.md'
+        plan.append(
+            models.Goal(
+                type='gen',
+                resource=target,
+                command=f"pynchon fixme gen --output {target}",
+            )
+        )
         return plan
 
+    @click.option(
+        "--output",
+        "-o",
+        default="docs/FIXME.md",
+        help=("output file to write.  (optional)"),
+    )
+    @options.should_print
+    @options.header
+    def gen(
+        self,
+        output,
+        should_print,
+        header,
+    ):
+        """
+        Generate FIXME.md files, aggregating references to all FIXME's in code-base
+        """
+        from pynchon import api
+
+        config = self.__class__.project_config
+        src_root = config.src['root']
+        exclude_patterns = config.fixme.get('exclude_patterns', [])
+        cmd = invoke(f'grep --line-number -R FIXME {src_root}')
+        assert cmd.succeeded
+        items = []
+        skipped = {}
+        for line in cmd.stdout.split('\n'):
+            line = line.strip()
+            if not line or line.startswith('Binary file'):
+                continue
+            bits = line.split(":")
+            file = bits.pop(0)
+            path = abcs.Path(file)
+            for g in exclude_patterns:
+                if fnmatch(file, g):
+                    skipped[g] = skipped.get(g, []) + [file]
+                    break
+            else:
+                line_no = bits.pop(0)
+                items.append(
+                    dict(
+                        file=abcs.Path(file).relative_to(
+                            abcs.Path(config['git']['root']).absolute()
+                        ),
+                        line=':'.join(bits),
+                        line_no=line_no,
+                    )
+                )
+        for g in skipped:
+            msg = f"exclude_pattern @ `{g}` skipped {len(skipped[g])} matches"
+            LOGGER.info(msg)
+        result = api.render.get_template(
+            'pynchon/plugins/fixme/FIXME.md.j2',
+        ).render(**dict(items=items))
+        msg = result
+        print(msg, file=open(output, 'w'))
+        if should_print and output != '/dev/stdout':
+            print(msg)
+
     @classmethod
     def asdasdinit_cli(kls):
         """"""
         parent = kls.click_group
         T_FIXME = constants.ENV.get_template(
             "pynchon/plugins/plugins/fixme/FIXME.md.j2"
         )
-
-        @common.kommand(
-            name="gen",
-            parent=parent,
-            formatters=dict(markdown=T_FIXME),
-            options=[
-                options.format_markdown,
-                click.option(
-                    "--output",
-                    "-o",
-                    default="docs/FIXME.md",
-                    help=("output file to write.  (optional)"),
-                ),
-                options.stdout,
-                options.header,
-            ],
-        )
-        def gen(output, format, stdout, header):
-            """
-            Generate FIXME.md files, aggregating references to all FIXME's in code-base
-            """
-            config = kls.project_config
-            src_root = config.pynchon['src_root']
-            exclude_patterns = config.fixme.get('exclude_patterns', [])
-            cmd = invoke(f'grep --line-number -R FIXME {src_root}')
-            assert cmd.succeeded
-            items = []
-            skipped = {}
-            for line in cmd.stdout.split('\n'):
-                line = line.strip()
-                if not line or line.startswith('Binary file'):
-                    continue
-                bits = line.split(":")
-                file = bits.pop(0)
-                path = abcs.Path(file)
-                for g in exclude_patterns:
-                    if fnmatch(file, g):
-                        skipped[g] = skipped.get(g, []) + [file]
-                        break
-                else:
-                    line_no = bits.pop(0)
-                    items.append(dict(file=file, line=':'.join(bits), line_no=line_no))
-            for g in skipped:
-                msg = f"exclude_pattern @ `{g}` skipped {len(skipped[g])} matches"
-                LOGGER.warning(msg)
-            return dict(items=items)
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/git/config.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/git.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ pynchon.plugins.git
 """
 from memoized_property import memoized_property
 
-from pynchon import abcs
+from pynchon import models, abcs
 from pynchon.abcs import Path
 from pynchon.util import lme, typing, files
 from pynchon.util.os import invoke
 
 LOGGER = lme.get_logger(__name__)
 
 
@@ -79,7 +79,16 @@
         return cmd.succeeded and cmd.stdout.strip()
 
     @property
     def hash(self) -> str:
         """ """
         cmd = self._run("git rev-parse HEAD")
         return cmd.succeeded and cmd.stdout.strip()
+
+
+class Git(models.Provider):
+    """Context for git"""
+
+    priority = -2
+    name = 'git'
+    defaults: typing.Dict = dict()
+    config_class = GitConfig
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/json.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" pynchon.plugins.render
+""" pynchon.plugins.json
 """
 from pynchon.util import lme, typing  # noqa
 
 from pynchon import models, abcs
 
 # from pynchon.util.os import invoke
 
@@ -49,15 +49,15 @@
 
 class Json(models.ToolPlugin):
     """
     Tools for working with JSON & JSON5
     """
 
     name = 'json'
-    priority = -1
+    priority = 1
     config_class = None
     cli_name = name
     # cli_subsumes: typing.List[typing.Callable] = [
     #     loadf_main.json5,
     #     loadf_main.json,
     #     loadf_main.j5,
     #     # loadf_main.json,
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/load.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/load.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/parse.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/parse.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/project.py` & `pynchon-2023.5.7.2.25/src/pynchon/models/planning.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,159 +1,134 @@
-""" pynchon.plugins.project
-"""
-import os
+import typing
+import collections
 
-from pynchon import abcs, config, models
-from pynchon.cli import common, options
-from pynchon.util import lme, typing
+from pynchon import abcs
+from pynchon.fleks import meta
 
-LOGGER = lme.get_logger(__name__)
+# from pynchon.fleks.plugin import Plugin as AbstractPlugin
+# from pynchon.plugins.util import get_plugin_obj
 
+from pynchon.util import typing, lme  # noqa
 
-class ProjectConfig(abcs.Config):
+# from pynchon.util.tagging import tags
+
+
+class Goal(typing.NamedTuple, metaclass=meta.namespace):
     """ """
 
-    priority = 1
-    config_key = "project"
-    # @property
-    # def src_root(self) -> str:
-    #     """ """
-    #     return self.subproject and pynchon["working_dir"]
+    resource: str = '??'
+    command: str = 'echo'
+    type: str = 'unknown'
 
-    @property
-    def name(self) -> typing.StringMaybe:
+    def __rich__(self) -> str:
+        from pynchon.util import shfmt
+
+        pretty = shfmt.bash_fmt(self.command)
+        from rich.syntax import Syntax
+        from rich.console import Console
+
+        # console = kwargs.pop('console', None) or Console(stderr=True)
+        # result = bash_fmt(*args, **kwargs)
+        syntax = Syntax(pretty, 'bash', line_numbers=True)
+        return syntax
+
+    def __str__(self):
+        return f"<{self.__class__.__name__}[{self.resource}]>"
+
+
+class Action(typing.NamedTuple, metaclass=meta.namespace):
+    """ """
+
+    type: str = 'unknown_action_type'
+    result: object = None
+    resource: str = '??'
+    command: str = 'echo'
+
+    def __str__(self):
+        return f"<{self.__class__.__name__}[{self.result}]>"
+
+
+class Plan(typing.List[Goal], metaclass=meta.namespace):
+    """ """
+
+    def __rich__(self) -> str:
+        syntaxes = [g.__rich__() for g in self]
+        from rich import box
+        from rich.text import Text
+        from rich.table import Table
+        from rich.syntax import Syntax
+        from rich.console import Console
+        from rich.markdown import Markdown
+
+        table = Table(
+            title=f'{self.__class__.__name__}',
+            # box=box.MINIMAL_DOUBLE_HEAD,
+            expand=True,
+        )
+        # table.add_column("idx", justify="left", style="bold magenta", no_wrap=True)
+        table.add_column("action", justify="left", style="green", no_wrap=True)
+        [[table.add_row(x), table.add_row()] for i, x in enumerate(syntaxes)]
+        return table
+
+    def __init__(self, *args):
         """ """
-        repo_name = config.git.get("repo_name")
-        return repo_name or os.path.split(os.getcwd())[-1]
+        for arg in args:
+            if not isinstance(arg, (Goal,)):
+                err = f'plan can only include goals, got {arg} with type={type(arg)}'
+                raise TypeError(err)
+            super(Plan, self).__init__(*args)
+
+    def __str__(self):
+        return f"<{self.__class__.__name__}[{len(self)} goals]>"
 
     @property
-    def root(self) -> str:
+    def _dict(self):
         """ """
-        git = config.GIT
-        return (
-            os.environ.get("PYNCHON_ROOT") or (git and git.get("root")) or os.getcwd()
-        )
+        result = collections.OrderedDict()
+        result['resources'] = list(set([g.resource for g in self]))
+        actions_by_type = collections.defaultdict(list)
+        for g in self:
+            actions_by_type[g.type].append(g.command)
+        result.update(**actions_by_type)
+        return result
+
+    # @typing.validate_arguments
+    def __add__(self, other):
+        """ """
+        assert isinstance(other, (Plan,))
+        return Plan(*(other + self))
+
+    __iadd__ = __add__
+
+    # @typing.validate_arguments
+    def append(self, other: Goal):
+        """ """
+        assert isinstance(other, (Goal,))
+        return super(Plan, self).append(other)
+
+    # @typing.validate_arguments
+    def extend(self, other):
+        """ """
+        assert isinstance(other, (Goal,))
+        return super(Plan, self).extend(other)
+
+
+class ApplyResults(typing.List[Action], metaclass=meta.namespace):
+    def __str__(self):
+        return f"<{self.__class__.__name__}[{len(self)} actions]>"
 
     @property
-    def subproject(self) -> typing.Dict:
+    def _dict(self):
         """ """
-        if os.environ.get("PYNCHON_ROOT"):
-            return {}
-        git = config.GIT
-        git_root = git["root"]
-        workdir = abcs.Path('.')
-        # workdir = pynchon["working_dir"]
-        r1 = workdir.absolute()
-        r2 = git_root and git_root.absolute()
-        if r2 and (r1 != r2):
-            self.logger.warning("subproject detected ({tmp}!=git[root])")
-            return dict(name=workdir.name, root=workdir.absolute())
-        return {}
-
-
-class Project(models.Manager):
-    """Macros for plan/applies across plugins"""
-
-    name = 'project'
-    priority = 2
-    defaults = dict()
-    config_class = ProjectConfig
-
-    @classmethod
-    def init_cli(kls):
-        """pynchon.bin.project"""
-        parent = kls.click_group
-
-        from pynchon import constants, util
-        from pynchon.api import project
-        from pynchon.util import lme, text
-        from pynchon.util.os import invoke
-
-        LOGGER = lme.get_logger(__name__)
-
-        @common.kommand(
-            name="entrypoints",
-            parent=parent,
-            formatters=dict(markdown=constants.T_TOC_CLI),
-            options=[
-                options.file_setupcfg,
-                options.format,
-                options.stdout,
-                options.output,
-                options.header,
-            ],
-        )
-        def project_entrypoints(format, file, stdout, output, header) -> None:
-            """
-            Describe entrypoints for this project (parses setup.cfg)
-            """
-            config, plan = project.plan()
-            return {
-                **util.python.load_entrypoints(util.python.load_setupcfg(file=file)),
-                **dict(__main__=config.get("source", {}).get("__main__", [])),
-            }
-
-        @common.kommand(
-            name="version",
-            parent=parent,
-            formatters=dict(markdown=constants.T_VERSION_METADATA),
-            options=[
-                # FIXME: options.output_with_default('docs/VERSION.md'),
-                options.format_markdown,
-                options.output,
-                options.header,
-            ],
-        )
-        def project_version(format, output, header) -> None:
-            """
-            Describes version details for this package (and pynchon itself).
-            """
-            # from pynchon.api import python #, git
-            import pynchon
-            from pynchon.config import git, python
-
-            return dict(
-                pynchon_version=pynchon.__version__,
-                package_version=python.package.version,
-                git_hash=git.hash,
-            )
-
-        @parent.command(
-            name="config",
-            # parent=parent,
-            # options=[],
-        )
-        def project_config(config=None) -> None:
-            """
-            Describe the config for this project
-            """
-            tmp = project.get_config()
-            print(text.to_json(tmp))
-
-        @common.kommand(
-            name="apply",
-            parent=parent,
-            options=[],
-        )
-        def project_apply() -> None:
-            """
-            Apply the plan created by `pynchon project plan`
-            """
-            config, plan = project.plan()
-            for p in plan:
-                invoke(p)
-            return plan
-
-        @common.kommand(
-            name="plan",
-            parent=parent,
-            options=[
-                options.stdout,
-            ],
-        )
-        def project_plan(stdout):
-            """
-            List goals for auto-documenting this project
-            """
-            config, plan = project.plan()
-            config["plan"] = plan
-            return text.to_json(config)
+
+        def past_tense(x):
+            return f"{x}ed"
+
+        result = collections.OrderedDict()
+        result['ok'] = all([a.result for a in self])
+        result['resources'] = list(set([a.resource for a in self]))
+        result['actions'] = [g.command for g in self]
+        result['state'] = list(set([g.type for g in self]))
+        result['state'] = dict([past_tense(k), []] for k in result['state'])
+        for g in self:
+            result['state'][past_tense(g.type)].append(g.resource)
+        return result
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/python/api.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/python/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 from pynchon import abcs, models
 from pynchon.util import typing, lme
 
 LOGGER = lme.get_logger(__name__)
 
 
-class PythonAPI(models.Planner):
+class PythonAPI(models.ShyPlanner):
     """Tools for generating python-api docs"""
 
     # @common.groop("api", parent=groups.gen)
     # def gen_api() -> None:
     #     """
     #     Generate API docs from python modules, packages, etc
     #     """
@@ -69,17 +69,27 @@
         #     )
         #     header = f"{header}\n\n" if header else ""
         #     return dict(
         #         header=f"## API for '{package}' package\n\n{header}" + "-" * 80,
         #         blocks=result,
         #     )
 
-    def plan(self, config) -> typing.List:
+    def plan(self, config=None) -> typing.List:
+        """ """
+        config = config or self.project_config
         plan = super(self.__class__, self).plan(config)
-        # self.logger.debug("planning for API docs..")
         api_root = f"{config.pynchon['docs_root']}/api"
-        plan += [f"mkdir -p {api_root}"]
+        plan.append(
+            models.Goal(command=f"mkdir -p {api_root}", resource=None, type='gen')
+        )
+
         tmp = config.python["package"]["name"]
-        plan += [
-            "pynchon gen api toc" f' --package {tmp}' f" --output {api_root}/README.md"
-        ]
+        plan.append(
+            models.Goal(
+                command="pynchon gen api toc"
+                + f' --package {tmp}'
+                + f" --output {api_root}/README.md",
+                resource=None,
+                type='gen',
+            )
+        )
         return plan
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/python/cli.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/python/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,213 +1,240 @@
 """ pynchon.plugins.python.cli
 """
-from pynchon.util import typing, lme  # noqa
+# import os
+import glob
 
 from pynchon import abcs, models, shimport
 
+from pynchon.util import typing, lme  # noqa
+
 config_mod = shimport.lazy(
     'pynchon.config',
 )
 LOGGER = lme.get_logger(__name__)
 
 
 class PythonCliConfig(abcs.Config):
     config_key = "python-cli"
-    #
-    # @common.groop("cli", parent=groups.gen)
-    # def gen_cli():
-    #     """Generate CLI docs"""
-    #
 
     @property
-    def entrypoints(self) -> dict:
+    def src_root(self):
         """ """
-        import os
-        import glob
-
-        src_root = config_mod.project.get(
-            "src_root", config_mod.pynchon.get("src_root")
-        )
+        # src_root = abcs.Path(
+        # config_mod.project.get(
+        #     "src_root", config_mod.pynchon.get("src_root")
+        # )).absolute()
+        src_root = abcs.Path("./src").absolute()
         if not src_root:
             msg = "`src_root` not set for pynchon or project config; cannot enumerate entrypoints"
             LOGGER.critical(msg)
             return []
-        pat = os.path.sep.join([str(src_root), "**", "__main__.py"])
-        matches = [[os.path.relpath(x), {}] for x in glob.glob(pat, recursive=True)]
+        return src_root
+
+    @property
+    def entrypoints(self) -> dict:
+        """ """
+        src_root = self.src_root
+        pat = src_root / "**" / "__main__.py"
+        matches = [[x, {}] for x in glob.glob(str(pat), recursive=True)]
         matches = dict(matches)
         pkg_name = config_mod.python['package']["name"] or "unknown"
         for f, meta in matches.items():
-            tmp = f[len(str(src_root)) : -len("__main__.py")]
-            tmp = tmp[1:] if tmp.startswith("/") else tmp
-            tmp = tmp[:-1] if tmp.endswith("/") else tmp
-            matches[f] = {**matches[f], **dict(dotpath=".".join(tmp.split("/")))}
+            LOGGER.info(f'found entry-point: {f}')
+            dotpath = abcs.Path(f).relative_to(src_root)
+            dotpath = '.'.join(str(dotpath).split('/')[:-1])
+            matches[f] = {
+                **matches[f],
+                **dict(
+                    # src_root=src_root,
+                    dotpath=dotpath,
+                ),
+            }
         return matches
 
 
-class PythonCLI(models.Planner):
+class PythonCLI(models.ShyPlanner):
     """Tools for generating CLI docs"""
 
     name = "python-cli"
     config_class = PythonCliConfig
 
-    @classmethod
-    def init_cli(kls):
-        """pynchon.bin.cli:
-        Option parsing for the `cli` subcommand
-        """
-
-        # @common.kommand(
-        #     name="toc",
-        #     parent=Core.gen_cli,
-        #     formatters=dict(markdown=constants.T_TOC_CLI),
-        #     options=[
-        #         options.file_setupcfg,
-        #         options.format_markdown,
-        #         click.option(
-        #             "--output",
-        #             "-o",
-        #             default="docs/cli/README.md",
-        #             help=("output file to write.  (optional)"),
-        #         ),
-        #         options.stdout,
-        #         options.header,
-        #     ],
-        # )
-        # def toc(format, file, stdout, output, header):
-        #     """
-        #     Describe entrypoints for this project (parses setup.cfg)
-        #     """
-        #     from pynchon.api import project
-        #
-        #     config, plan = project.plan()
-        #     return config
-        #
-        # @common.kommand(
-        #     name="all",
-        #     parent=Core.gen_cli,
-        #     options=[
-        #         options.file_setupcfg,
-        #         options.output_dir,
-        #         options.stdout,
-        #     ],
-        # )
-        # def _all(
-        #     file,
-        #     stdout,
-        #     output_dir,
-        # ) -> list:
-        #     """
-        #     Generates help for every entrypoint
-        #     """
-        #     conf = util.python.load_entrypoints(util.python.load_setupcfg(path=file))
-        #     entrypoints = conf.get("entrypoints", {})
-        #     if not entrypoints:
-        #         LOGGER.warning(f"failed loading entrypoints from {file}")
-        #         return []
-        #     docs = {}
-        #     for e in entrypoints:
-        #         bin_name = str(e["bin_name"])
-        #         epoint = e["setuptools_entrypoint"]
-        #         fname = os.path.join(output_dir, bin_name)
-        #         fname = f"{fname}.md"
-        #         LOGGER.debug(f"{epoint}: -> `{fname}`")
-        #         docs[fname] = {**_entrypoint_docs(name=e["setuptools_entrypoint"]), **e}
-        #
-        #     for fname in docs:
-        #         with open(fname, "w") as fhandle:
-        #             fhandle.write(constants.T_DETAIL_CLI.render(docs[fname]))
-        #         LOGGER.debug(f"wrote: {fname}")
-        #     return list(docs.keys())
-        #
-        # @common.kommand(
-        #     name="main",
-        #     parent=Core.gen_cli,
-        #     formatters=dict(markdown=constants.T_CLI_MAIN_MODULE),
-        #     options=[
-        #         options.format_markdown,
-        #         options.stdout,
-        #         options.header,
-        #         options.file,
-        #         options.output_dir,
-        #         options.name,
-        #         options.module,
-        #     ],
-        # )
-        # def main_docs(format, module, file, output_dir, stdout, header, name):
-        #     """
-        #     Autogenenerate docs for python modules using __main__
-        #     """
-        #     from pynchon.api import project
-        #     from pynchon.util.os import invoke
-        #
-        #     config, plan = project.plan()
-        #     for fname, metadata in config["python"]["entrypoints"].items():
-        #         if fname == file:
-        #             dotpath = metadata["dotpath"]
-        #             cmd = invoke(f"python -m{dotpath} --help")
-        #             help = cmd.succeeded and cmd.stdout.strip()
-        #             config["python"]["entrypoints"][fname] = {
-        #                 **metadata,
-        #                 **dict(help=help),
-        #             }
-        #             return config
-        #
-        # @common.kommand(
-        #     name="entrypoint",
-        #     parent=Core.gen_cli,
-        #     formatters=dict(markdown=constants.T_DETAIL_CLI),
-        #     options=[
-        #         options.format_markdown,
-        #         options.stdout,
-        #         options.header,
-        #         options.file,
-        #         options.output,
-        #         options.name,
-        #         options.module,
-        #     ],
-        # )
-        # def entrypoint_docs(format, module, file, output, stdout, header, name):
-        #     """
-        #     Autogenenerate docs for python CLIs using click
-        #     """
-        #     tmp = _entrypoint_docs(module=module, name=name)
-        #     return tmp
-        #
-        # def _entrypoint_docs(module=None, name=None):
-        #     """ """
-        #     import importlib
-        #
-        #     result = []
-        #     if name and not module:
-        #         module, name = name.split(":")
-        #     if module and name:
-        #         mod = importlib.import_module(module)
-        #         entrypoint = getattr(mod, name)
-        #     else:
-        #         msg = "No entrypoint found"
-        #         LOGGER.warning(msg)
-        #         return dict(error=msg)
-        #     LOGGER.debug(f"Recursive help for `{module}:{name}`")
-        #     result = util.click_recursive_help(entrypoint, parent=None)
-        #     package = module.split(".")[0]
-        #     return dict(
-        #         package=module.split(".")[0],
-        #         module=module,
-        #         entrypoint=name,
-        #         commands=result,
-        #     )
+    # @common.kommand(
+    #     name="toc",
+    #     parent=Core.gen_cli,
+    #     formatters=dict(markdown=constants.T_TOC_CLI),
+    #     options=[
+    #         options.file_setupcfg,
+    #         options.format_markdown,
+    #         click.option(
+    #             "--output",
+    #             "-o",
+    #             default="docs/cli/README.md",
+    #             help=("output file to write.  (optional)"),
+    #         ),
+    #         options.stdout,
+    #         options.header,
+    #     ],
+    # )
+    # def toc(format, file, stdout, output, header):
+    #     """
+    #     Describe entrypoints for this project (parses setup.cfg)
+    #     """
+    #     from pynchon.api import project
+    #
+    #     config, plan = project.plan()
+    #     return config
+    #
+    # @common.kommand(
+    #     name="all",
+    #     parent=Core.gen_cli,
+    #     options=[
+    #         options.file_setupcfg,
+    #         options.output_dir,
+    #         options.stdout,
+    #     ],
+    # )
+    # def _all(
+    #     file,
+    #     stdout,
+    #     output_dir,
+    # ) -> list:
+    #     """
+    #     Generates help for every entrypoint
+    #     """
+    #     conf = util.python.load_entrypoints(util.python.load_setupcfg(path=file))
+    #     entrypoints = conf.get("entrypoints", {})
+    #     if not entrypoints:
+    #         LOGGER.warning(f"failed loading entrypoints from {file}")
+    #         return []
+    #     docs = {}
+    #     for e in entrypoints:
+    #         bin_name = str(e["bin_name"])
+    #         epoint = e["setuptools_entrypoint"]
+    #         fname = os.path.join(output_dir, bin_name)
+    #         fname = f"{fname}.md"
+    #         LOGGER.debug(f"{epoint}: -> `{fname}`")
+    #         docs[fname] = {**_entrypoint_docs(name=e["setuptools_entrypoint"]), **e}
+    #
+    #     for fname in docs:
+    #         with open(fname, "w") as fhandle:
+    #             fhandle.write(constants.T_DETAIL_CLI.render(docs[fname]))
+    #         LOGGER.debug(f"wrote: {fname}")
+    #     return list(docs.keys())
+    #
+    # @common.kommand(
+    #     name="main",
+    #     parent=Core.gen_cli,
+    #     formatters=dict(markdown=constants.T_CLI_MAIN_MODULE),
+    #     options=[
+    #         options.format_markdown,
+    #         options.stdout,
+    #         options.header,
+    #         options.file,
+    #         options.output_dir,
+    #         options.name,
+    #         options.module,
+    #     ],
+    # )
+    # def main_docs(format, module, file, output_dir, stdout, header, name):
+    #     """
+    #     Autogenenerate docs for python modules using __main__
+    #     """
+    #     from pynchon.api import project
+    #     from pynchon.util.os import invoke
+    #
+    #     config, plan = project.plan()
+    #     for fname, metadata in config["python"]["entrypoints"].items():
+    #         if fname == file:
+    #             dotpath = metadata["dotpath"]
+    #             cmd = invoke(f"python -m{dotpath} --help")
+    #             help = cmd.succeeded and cmd.stdout.strip()
+    #             config["python"]["entrypoints"][fname] = {
+    #                 **metadata,
+    #                 **dict(help=help),
+    #             }
+    #             return config
+    #
+    # @common.kommand(
+    #     name="entrypoint",
+    #     parent=Core.gen_cli,
+    #     formatters=dict(markdown=constants.T_DETAIL_CLI),
+    #     options=[
+    #         options.format_markdown,
+    #         options.stdout,
+    #         options.header,
+    #         options.file,
+    #         options.output,
+    #         options.name,
+    #         options.module,
+    #     ],
+    # )
+    # def entrypoint_docs(format, module, file, output, stdout, header, name):
+    #     """
+    #     Autogenenerate docs for python CLIs using click
+    #     """
+    #     tmp = _entrypoint_docs(module=module, name=name)
+    #     return tmp
+    #
+    # def _entrypoint_docs(module=None, name=None):
+    #     """ """
+    #     import importlib
+    #
+    #     result = []
+    #     if name and not module:
+    #         module, name = name.split(":")
+    #     if module and name:
+    #         mod = importlib.import_module(module)
+    #         entrypoint = getattr(mod, name)
+    #     else:
+    #         msg = "No entrypoint found"
+    #         LOGGER.warning(msg)
+    #         return dict(error=msg)
+    #     LOGGER.debug(f"Recursive help for `{module}:{name}`")
+    #     result = util.click_recursive_help(entrypoint, parent=None)
+    #     package = module.split(".")[0]
+    #     return dict(
+    #         package=module.split(".")[0],
+    #         module=module,
+    #         entrypoint=name,
+    #         commands=result,
+    #     )
 
     def plan(self, config=None):
-        from pynchon.api import project
+        from pynchon import api
 
-        config = config or project.get_config()
+        config = config or api.project.get_config()
         plan = super(self.__class__, self).plan(config)
         droot = config.pynchon['docs_root']
         cli_root = f"{droot}/cli"
-        plan += [f"mkdir -p {cli_root}"]
-        plan += [f"pynchon gen cli toc --output {cli_root}/README.md"]
-        plan += [f"pynchon gen cli all --output-dir {cli_root}"]
-        plan += [
-            f"pynchon gen cli main --file {fname} --output-dir {cli_root}"
+
+        plan.append(
+            self.goal(command=f"mkdir -p {cli_root}", type='mkdir', resource=cli_root)
+        )
+        plan.append(
+            self.goal(
+                command=f"pynchon gen cli toc --output {cli_root}/README.md",
+                type='gen',
+                resource=cli_root,
+            )
+        )
+
+        plan.append(
+            self.goal(
+                command=f"pynchon gen cli all --output-dir {cli_root}",
+                type='gen',
+                resource=cli_root,
+            )
+        )
+
+        [
+            plan.append(
+                self.goal(
+                    command=f"pynchon gen cli main --file {fname} --output-dir {cli_root}",
+                    type='gen',
+                    resource=fname,
+                )
+            )
             for fname in config['python-cli'].entrypoints
         ]
+
         return plan
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/python/platform.py` & `pynchon-2023.5.7.2.25/src/pynchon/models/planner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,87 @@
-""" pynchon.plugins.python.platform
 """
-import platform as stdlib_platform
-
-from memoized_property import memoized_property
+"""
+import typing
 
-from pynchon import abcs, models
-from pynchon.util import typing, lme
-from pynchon.util.os import invoke
+# from pynchon import abcs, api, cli,
+from pynchon import events
 
-LOGGER = lme.get_logger(__name__)
+# from pynchon.bin import entry
+# from pynchon.fleks.plugin import Plugin as AbstractPlugin
+# from pynchon.plugins.util import get_plugin_obj
+from pynchon.util.tagging import tags
 
+# from .planning import *
+from . import planning
+from .plugin_types import BasePlugin
 
-class PythonPlatform(models.Provider):
-    """Context for python-platform"""
+from pynchon.util import typing, lme  # noqa
 
-    priority = 2
-    name = 'python'
 
-    class config_class(abcs.Config):
-        config_key = "python"
-        defaults = dict(
-            version=stdlib_platform.python_version(),
-        )
+@tags(cli_label='Planner')
+class AbstractPlanner(BasePlugin):
+    """
+    AbstractPlanner is a plugin-type that provides plan/apply basics
+    """
 
-        @memoized_property
-        def is_package(self) -> bool:
-            # self.logger.debug("checking if this a python package..")
-            cmd = invoke("python setup.py --version 2>/dev/null", log_command=False)
-            return cmd.succeeded
-
-        @property
-        def package(self) -> typing.Dict:
-            """ """
-            if self.is_package:
-                return PackageConfig()
-            else:
-                return {}
-
-
-class PackageConfig(abcs.Config):
-    parent = PythonPlatform.config_class
-    config_key = "package"
+    cli_label = 'Planner'
 
-    @property
-    def name(self) -> str:
+    def goal(self, **kwargs):
         """ """
-        from pynchon.util import python
+        return planning.Goal(**kwargs)
 
-        return python.load_setupcfg().get("metadata", {}).get("name")
+    def plan(self, config=None) -> planning.Plan:
+        """Creates a plan for this plugin"""
+        config = config or self.cfg()
+        events.lifecycle.send(
+            # writes status event (used by the app-console)
+            stage=f"Planning for `{self.__class__.name}`"
+        )
+        plan = planning.Plan()
+        return plan
 
-    @memoized_property
-    def version(self) -> str:
-        """ """
-        # self.logger.debug("resolving project version..")
-        cmd = invoke("python setup.py --version 2>/dev/null", log_command=False)
-        return cmd.succeeded and cmd.stdout.strip()
+    def apply(self, config=None) -> planning.ApplyResults:
+        """Executes the plan for this plugin"""
+        from pynchon.util.os import invoke
+
+        events.lifecycle.send(
+            # write status event (used by the app-console)
+            stage=f"applying for `{self.__class__.name}`"
+        )
+        plan = self.plan(config=config)
+        results = []
+        for action_item in plan:
+            events.lifecycle.send(self, applying=action_item)
+            application = invoke(action_item.command)
+            tmp = planning.Action(
+                result=application.succeeded,
+                command=action_item.command,
+                resource=action_item.resource,
+                type=action_item.type,
+            )
+            results.append(tmp)
+        results = planning.ApplyResults(results)
+        return results
+
+
+class ShyPlanner(AbstractPlanner):
+    """
+    ShyPlanner uses plan/apply workflows, but they must be
+    executed directly.  ProjectPlugin (or any other parent plugins)
+    won't include this as a sub-plan.
+    """
+
+    contribute_plan_apply = False
+
+
+@tags(cli_label='Manager')
+class Manager(ShyPlanner):
+    cli_label = 'Manager'
+
+
+class Planner(ShyPlanner):
+    """
+    Planner uses plan/apply workflows, and contributes it's plans
+    to ProjectPlugin (or any other parent plugins).
+    """
+
+    contribute_plan_apply = True
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/release.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/release.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/render.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/render.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/scaffolding/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 from .config import ScaffoldingConfig, ScaffoldingItem
 
 tags = tagging.tags
 LOGGER = lme.get_logger(__name__)
 
 
-class Scaffolding(models.Manager):
+class Scaffolding(models.ShyPlanner):
     """Management tool for project boilerplate"""
 
     contribute_plan_apply = False
     priority = 3
     name = "scaffolding"
     cli_name = 'scaffold'
     defaults = dict()
+    cli_label = 'Manager'
     config_class = ScaffoldingConfig
 
     def match(self, pattern=None):
         """
         returns files that match for all scaffolds
         """
         if pattern:
@@ -95,9 +96,15 @@
         return result
 
     def plan(self, config=None) -> typing.List[str]:
         """ """
         config or self.plugin_config
         plan = super(Scaffolding, self).plan(config)
         for delta in self.diff()['modified']:
-            plan += [f"cp {delta['src']} {delta['fname']}"]
+            plan.append(
+                models.Goal(
+                    type='scaffold',
+                    resource=delta['fname'],
+                    command=f"cp {delta['src']} {delta['fname']}",
+                )
+            )
         return plan
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/config.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/scaffolding/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/plugins/util.py` & `pynchon-2023.5.7.2.25/src/pynchon/plugins/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/shimport/models.py` & `pynchon-2023.5.7.2.25/src/pynchon/shimport/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,20 @@
 
     def prune(self, **filters):
         """ """
         # self.logger.critical(f"prune: {filters}")
         self.namespace = self.filter(**filters)
         return self if self.namespace else None
 
+    def sorted(self, key=None):
+        tmp = self.namespace.items()
+        tmp = sorted(tmp, key=key)
+        self.namespace = collections.OrderedDict(tmp)
+        return self
+
     def get_folder_children(
         self,
         include_main: str = True,
         exclude_private=True,
     ):
         """ """
         import os
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/shimport/module.py` & `pynchon-2023.5.7.2.25/src/pynchon/shimport/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,30 +69,13 @@
     result = models.ModulesWrapper(name, import_names=[f'{name}.*'], **kwargs)
     return result
 
 
 wrapper = wrap
 
 
-def registry_builder(
-    name,
-    # itemizer=None,
-    **kargs,
-):
-    """ """
-    wrapped = wrap(
-        name,
-    )
-    return wrapped
-    # return dict(itemizer(obj) for obj in built)
-
-
-registry = registry_builder
-build_registry = registry_builder
-
-
-def lazy_import(
+def lazy(
     module_name: str,
 ) -> models.LazyModule:
     """ """
     assert module_name
     return models.LazyModule(module_name)
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/shimport/util.py` & `pynchon-2023.5.7.2.25/src/pynchon/shimport/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2` & `pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2` & `pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2` & `pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2` & `pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2` & `pynchon-2023.5.7.2.25/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/click.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/click.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/complexity.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/complexity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+""" pynchon.util.complexity
+"""
 GLYPH_COMPLEXITY = "🐉 Complex"
 
 import os
 import ast
 import sys
 from collections import OrderedDict
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/config.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/events.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/lme.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/lme.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 """ {{pkg}}.util.lme
 """
 import logging
 
+from rich.style import Style
+from rich.theme import Theme
+from rich.console import Console
+from rich.logging import RichHandler
+from rich.default_styles import DEFAULT_STYLES
+
+from pynchon import constants
+
+THEME = Theme(
+    {
+        **DEFAULT_STYLES,
+        **{
+            "logging.keyword": Style(bold=True, color="yellow"),
+            # "logging.level.notset": Style(dim=True),
+            "logging.level.debug": Style(color="green"),
+            "logging.level.info": Style(
+                dim=True,
+                # color="blue",
+            ),
+            "logging.level.warning": Style(color="yellow"),
+            "logging.level.error": Style(color="red", dim=True, bold=True),
+            "logging.level.critical": Style(
+                color="red",
+                bold=True,
+                # reverse=True
+            ),
+            "log.level": Style.null(),
+            "log.time": Style(color="cyan", dim=True),
+            "log.message": Style.null(),
+            "log.path": Style(dim=True),
+        },
+    }
+)
+CONSOLE = Console(theme=THEME, stderr=True)
 
-def get_logger(name):
+
+def set_global_level(level):
+    """
+    https://stackoverflow.com/questions/19617355/dynamically-changing-log-level-without-restarting-the-application
+    """
+    logger = logging.getLogger()
+    logger.setLevel(level)
+    for handler in logger.handlers:
+        handler.setLevel(level)
+        # if isinstance(handler, type(logging.StreamHandler())):
+        #     handler.setLevel(logging.DEBUG)
+        #     logger.debug('Debug logging enabled')
+
+
+def get_logger(name, console=CONSOLE):
     """
     utility function for returning a logger
     with standard formatting patterns, etc
     """
-    from rich.style import Style
-    from rich.theme import Theme
-    from rich.console import Console
-    from rich.logging import RichHandler
-    from rich.default_styles import DEFAULT_STYLES
-
-    theme = Theme(
-        {
-            **DEFAULT_STYLES,
-            **{
-                "logging.keyword": Style(bold=True, color="yellow"),
-                # "logging.level.notset": Style(dim=True),
-                "logging.level.debug": Style(color="green"),
-                "logging.level.info": Style(
-                    dim=True,
-                    # color="blue",
-                ),
-                "logging.level.warning": Style(color="yellow"),
-                "logging.level.error": Style(color="red", dim=True, bold=True),
-                "logging.level.critical": Style(
-                    color="red",
-                    bold=True,
-                    # reverse=True
-                ),
-                "log.level": Style.null(),
-                "log.time": Style(color="cyan", dim=True),
-                "log.message": Style.null(),
-                "log.path": Style(dim=True),
-            },
-        }
-    )
+
     log_handler = RichHandler(
         rich_tracebacks=True,
-        console=Console(theme=theme, stderr=True),
+        console=CONSOLE,
         show_time=False,
     )
 
     logging.basicConfig(
-        # level="DEBUG",
         format="%(message)s",
         datefmt="[%X]",
         handlers=[log_handler],
     )
     FormatterClass = logging.Formatter
     formatter = FormatterClass(
         fmt=" ".join(["%(name)s", "%(message)s"]),
@@ -58,9 +75,11 @@
         datefmt="",
     )
     log_handler.setFormatter(formatter)
 
     logger = logging.getLogger(name)
 
     # FIXME: get this from some kind of global config
-    logger.setLevel("DEBUG")
+    # logger.setLevel("DEBUG")
+    logger.setLevel(constants.LOG_LEVEL)
+
     return logger
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/oop.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/oop.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/python.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/python.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/tagging.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/tagging.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,28 +13,35 @@
 
 from collections import defaultdict
 
 from pynchon.util import typing, lme
 
 LOGGER = lme.get_logger(__name__)
 
-#         # if inspect.iscoroutinefunction(func):
-#         #     @functools.wraps(func)
-#         #     async def async_wrapped(*args: Any, **kwargs: Any) -> Awaitable:
-#         #         return await func(*args, **kwargs)
-#         #     return async_wrapped
-#         # else:
-#         #     @functools.wraps(func)
-#         #     def sync_wrapped(*args: Any, **kwargs: Any) -> Any:
-#         #         return func(*args, **kwargs)
-#         #     return sync_wrapped
-#
-#     return decorator
-#
-#
+
+def tagged_property(**ftags):
+    """
+    Equivalent to:
+        @tagging.tags(foo=bar)
+        @property
+        def method(self):
+            ...
+    """
+
+    def dec(fxn):
+        @tags(**ftags)
+        @property
+        def newf(*args, **kwargs):
+            return fxn(*args, **kwargs)
+
+        return newf
+
+    return dec
+
+
 def tag_factory(*args) -> typing.Any:
     """ """
 
     class tagger(dict):
         # def tag(self, **tags):
         #     self.tags = tags
         # tag = staticmethod(
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/text/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/text/loadf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/__main__.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/text/loadf/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/text/loads.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/text/loads.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/text/normalize/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/text/normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/text/render/__init__.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/text/render/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,14 @@
         # import IPython; IPython.embed()
         raise
     except (jinja2.exceptions.TemplateNotFound,) as exc:
         LOGGER.critical(f"Template exception: {exc}")
         LOGGER.critical(f"Jinja-includes: {includes}")
         err = getattr(exc, 'templates', exc.message)
         LOGGER.critical(f"Problem template: {err}")
-        import IPython
-
-        IPython.embed()
         raise
 
 
 @options.output
 @options.inplace
 @options.should_print
 @options.includes
```

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/text/render/__main__.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/text/render/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon/util/typing.py` & `pynchon-2023.5.7.2.25/src/pynchon/util/typing.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.50/src/pynchon.egg-info/PKG-INFO` & `pynchon-2023.5.7.2.25/src/pynchon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2023.5.2.14.50
+Version: 2023.5.7.2.25
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
```

