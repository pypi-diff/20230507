# Comparing `tmp/releng-tool-0.8.0.tar.gz` & `tmp/releng-tool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\releng-tool-0.8.0.tar", last modified: Sun Aug 29 01:56:44 2021, max compression
+gzip compressed data, was "dist\releng-tool-0.9.0.tar", last modified: Sat Oct  2 23:25:46 2021, max compression
```

## Comparing `releng-tool-0.8.0.tar` & `releng-tool-0.9.0.tar`

### file list

```diff
@@ -1,439 +1,455 @@
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.332927 releng-tool-0.8.0/
--rw-rw-rw-   0        0        0     1300 2019-02-13 15:28:24.000000 releng-tool-0.8.0/LICENSE
--rw-rw-rw-   0        0        0      158 2021-04-13 22:39:01.000000 releng-tool-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3289 2021-08-29 01:56:44.333903 releng-tool-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2274 2021-01-01 19:08:47.000000 releng-tool-0.8.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.038024 releng-tool-0.8.0/releng/
--rw-rw-rw-   0        0        0      338 2020-09-27 23:50:14.000000 releng-tool-0.8.0/releng/__init__.py
--rw-rw-rw-   0        0        0      293 2020-09-13 21:06:07.000000 releng-tool-0.8.0/releng/__main__.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.039001 releng-tool-0.8.0/releng/api/
--rw-rw-rw-   0        0        0      417 2020-09-27 23:50:14.000000 releng-tool-0.8.0/releng/api/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.044860 releng-tool-0.8.0/releng_tool/
--rw-rw-rw-   0        0        0     2325 2021-08-29 01:55:42.000000 releng-tool-0.8.0/releng_tool/__init__.py
--rw-rw-rw-   0        0        0     8386 2021-08-28 22:48:02.000000 releng-tool-0.8.0/releng_tool/__main__.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.072200 releng-tool-0.8.0/releng_tool/api/
--rw-rw-rw-   0        0        0    23207 2020-09-24 02:47:10.000000 releng-tool-0.8.0/releng_tool/api/__init__.py
--rw-rw-rw-   0        0        0     8532 2021-08-22 21:54:37.000000 releng-tool-0.8.0/releng_tool/defs.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.080014 releng-tool-0.8.0/releng_tool/engine/
--rw-rw-rw-   0        0        0    32690 2021-08-29 01:30:13.000000 releng-tool-0.8.0/releng_tool/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.082943 releng-tool-0.8.0/releng_tool/engine/autotools/
--rw-rw-rw-   0        0        0       25 2021-01-05 19:32:45.000000 releng-tool-0.8.0/releng_tool/engine/autotools/__init__.py
--rw-rw-rw-   0        0        0     1459 2021-01-05 19:34:26.000000 releng-tool-0.8.0/releng_tool/engine/autotools/build.py
--rw-rw-rw-   0        0        0     1938 2021-01-05 19:34:06.000000 releng-tool-0.8.0/releng_tool/engine/autotools/configure.py
--rw-rw-rw-   0        0        0     1722 2021-01-05 19:34:04.000000 releng-tool-0.8.0/releng_tool/engine/autotools/install.py
--rw-rw-rw-   0        0        0     1712 2021-01-05 20:04:25.000000 releng-tool-0.8.0/releng_tool/engine/bootstrap.py
--rw-rw-rw-   0        0        0     3143 2021-08-23 01:27:12.000000 releng-tool-0.8.0/releng_tool/engine/build.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.085873 releng-tool-0.8.0/releng_tool/engine/cmake/
--rw-rw-rw-   0        0        0       25 2021-01-05 19:34:36.000000 releng-tool-0.8.0/releng_tool/engine/cmake/__init__.py
--rw-rw-rw-   0        0        0     2019 2021-01-05 19:35:48.000000 releng-tool-0.8.0/releng_tool/engine/cmake/build.py
--rw-rw-rw-   0        0        0     3319 2021-01-05 19:35:36.000000 releng-tool-0.8.0/releng_tool/engine/cmake/configure.py
--rw-rw-rw-   0        0        0     1941 2021-01-05 19:35:34.000000 releng-tool-0.8.0/releng_tool/engine/cmake/install.py
--rw-rw-rw-   0        0        0     3537 2021-08-23 01:27:05.000000 releng-tool-0.8.0/releng_tool/engine/configure.py
--rw-rw-rw-   0        0        0     5035 2021-01-05 20:05:49.000000 releng-tool-0.8.0/releng_tool/engine/extract.py
--rw-rw-rw-   0        0        0    10795 2021-01-05 20:05:58.000000 releng-tool-0.8.0/releng_tool/engine/fetch.py
--rw-rw-rw-   0        0        0     2713 2021-08-23 05:20:55.000000 releng-tool-0.8.0/releng_tool/engine/init.py
--rw-rw-rw-   0        0        0     3861 2021-08-23 01:26:59.000000 releng-tool-0.8.0/releng_tool/engine/install.py
--rw-rw-rw-   0        0        0     2652 2021-08-23 01:26:53.000000 releng-tool-0.8.0/releng_tool/engine/patch.py
--rw-rw-rw-   0        0        0     1668 2021-01-05 19:38:47.000000 releng-tool-0.8.0/releng_tool/engine/post.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.088802 releng-tool-0.8.0/releng_tool/engine/python/
--rw-rw-rw-   0        0        0       25 2021-01-05 19:36:02.000000 releng-tool-0.8.0/releng_tool/engine/python/__init__.py
--rw-rw-rw-   0        0        0     2148 2021-01-05 19:36:42.000000 releng-tool-0.8.0/releng_tool/engine/python/build.py
--rw-rw-rw-   0        0        0     2713 2021-01-05 19:36:29.000000 releng-tool-0.8.0/releng_tool/engine/python/install.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.091731 releng-tool-0.8.0/releng_tool/engine/script/
--rw-rw-rw-   0        0        0       25 2021-01-05 19:37:53.000000 releng-tool-0.8.0/releng_tool/engine/script/__init__.py
--rw-rw-rw-   0        0        0     1515 2021-08-07 18:34:05.000000 releng-tool-0.8.0/releng_tool/engine/script/build.py
--rw-rw-rw-   0        0        0     1646 2021-08-07 18:34:15.000000 releng-tool-0.8.0/releng_tool/engine/script/configure.py
--rw-rw-rw-   0        0        0     1594 2021-08-07 18:34:20.000000 releng-tool-0.8.0/releng_tool/engine/script/install.py
--rw-rw-rw-   0        0        0     1066 2021-04-18 17:43:53.000000 releng-tool-0.8.0/releng_tool/exceptions.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.091731 releng-tool-0.8.0/releng_tool/ext/
--rw-rw-rw-   0        0        0       25 2021-01-05 19:50:53.000000 releng-tool-0.8.0/releng_tool/ext/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.092708 releng-tool-0.8.0/releng_tool/ext/seed/
--rw-rw-rw-   0        0        0     1054 2020-09-24 01:42:49.000000 releng-tool-0.8.0/releng_tool/ext/seed/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.095638 releng-tool-0.8.0/releng_tool/extract/
--rw-rw-rw-   0        0        0       25 2021-01-05 19:51:10.000000 releng-tool-0.8.0/releng_tool/extract/__init__.py
--rw-rw-rw-   0        0        0     6213 2021-01-05 19:51:48.000000 releng-tool-0.8.0/releng_tool/extract/archive.py
--rw-rw-rw-   0        0        0     5916 2021-08-28 22:47:26.000000 releng-tool-0.8.0/releng_tool/extract/git.py
--rw-rw-rw-   0        0        0     1197 2021-01-05 19:52:13.000000 releng-tool-0.8.0/releng_tool/extract/mercurial.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.102475 releng-tool-0.8.0/releng_tool/fetch/
--rw-rw-rw-   0        0        0       25 2021-08-21 21:21:05.000000 releng-tool-0.8.0/releng_tool/fetch/__init__.py
--rw-rw-rw-   0        0        0     1306 2021-01-05 19:54:47.000000 releng-tool-0.8.0/releng_tool/fetch/bzr.py
--rw-rw-rw-   0        0        0     2330 2021-08-28 21:27:31.000000 releng-tool-0.8.0/releng_tool/fetch/cvs.py
--rw-rw-rw-   0        0        0    18739 2021-08-29 00:58:23.000000 releng-tool-0.8.0/releng_tool/fetch/git.py
--rw-rw-rw-   0        0        0     2181 2021-01-05 19:53:49.000000 releng-tool-0.8.0/releng_tool/fetch/mercurial.py
--rw-rw-rw-   0        0        0     1082 2021-01-05 19:53:35.000000 releng-tool-0.8.0/releng_tool/fetch/scp.py
--rw-rw-rw-   0        0        0     1602 2021-01-05 19:53:14.000000 releng-tool-0.8.0/releng_tool/fetch/svn.py
--rw-rw-rw-   0        0        0     2987 2021-08-21 21:50:02.000000 releng-tool-0.8.0/releng_tool/fetch/url.py
--rw-rw-rw-   0        0        0    10609 2021-08-08 16:50:23.000000 releng-tool-0.8.0/releng_tool/opts.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.105403 releng-tool-0.8.0/releng_tool/packages/
--rw-rw-rw-   0        0        0     2050 2021-08-28 22:47:26.000000 releng-tool-0.8.0/releng_tool/packages/__init__.py
--rw-rw-rw-   0        0        0     5956 2021-08-07 20:44:23.000000 releng-tool-0.8.0/releng_tool/packages/exceptions.py
--rw-rw-rw-   0        0        0    43142 2021-08-29 01:29:09.000000 releng-tool-0.8.0/releng_tool/packages/manager.py
--rw-rw-rw-   0        0        0     5351 2021-08-22 01:18:56.000000 releng-tool-0.8.0/releng_tool/packages/package.py
--rw-rw-rw-   0        0        0    13383 2021-08-28 21:44:50.000000 releng-tool-0.8.0/releng_tool/packages/pipeline.py
--rw-rw-rw-   0        0        0     5588 2021-01-05 20:00:51.000000 releng-tool-0.8.0/releng_tool/prerequisites.py
--rw-rw-rw-   0        0        0    12723 2021-08-15 23:53:29.000000 releng-tool-0.8.0/releng_tool/registry.py
--rw-rw-rw-   0        0        0    10449 2021-08-28 18:22:38.000000 releng-tool-0.8.0/releng_tool/stats.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.115167 releng-tool-0.8.0/releng_tool/tool/
--rw-rw-rw-   0        0        0     5481 2021-08-22 01:38:09.000000 releng-tool-0.8.0/releng_tool/tool/__init__.py
--rw-rw-rw-   0        0        0      266 2021-01-05 19:56:40.000000 releng-tool-0.8.0/releng_tool/tool/autoreconf.py
--rw-rw-rw-   0        0        0      840 2021-01-05 19:56:30.000000 releng-tool-0.8.0/releng_tool/tool/bzr.py
--rw-rw-rw-   0        0        0      236 2021-01-05 19:56:22.000000 releng-tool-0.8.0/releng_tool/tool/cmake.py
--rw-rw-rw-   0        0        0      676 2021-01-05 19:56:18.000000 releng-tool-0.8.0/releng_tool/tool/cvs.py
--rw-rw-rw-   0        0        0     3661 2021-08-22 05:58:26.000000 releng-tool-0.8.0/releng_tool/tool/git.py
--rw-rw-rw-   0        0        0      723 2021-01-05 19:56:11.000000 releng-tool-0.8.0/releng_tool/tool/hg.py
--rw-rw-rw-   0        0        0      230 2021-01-05 19:56:06.000000 releng-tool-0.8.0/releng_tool/tool/make.py
--rw-rw-rw-   0        0        0      524 2021-01-05 19:56:03.000000 releng-tool-0.8.0/releng_tool/tool/patch.py
--rw-rw-rw-   0        0        0     3852 2021-08-28 22:47:26.000000 releng-tool-0.8.0/releng_tool/tool/python.py
--rw-rw-rw-   0        0        0     1376 2021-01-05 19:56:57.000000 releng-tool-0.8.0/releng_tool/tool/scp.py
--rw-rw-rw-   0        0        0      379 2021-01-05 19:55:36.000000 releng-tool-0.8.0/releng_tool/tool/svn.py
--rw-rw-rw-   0        0        0      381 2021-01-05 19:55:30.000000 releng-tool-0.8.0/releng_tool/tool/tar.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.123956 releng-tool-0.8.0/releng_tool/util/
--rw-rw-rw-   0        0        0      531 2021-04-17 15:29:41.000000 releng-tool-0.8.0/releng_tool/util/__init__.py
--rw-rw-rw-   0        0        0      795 2021-04-18 01:29:24.000000 releng-tool-0.8.0/releng_tool/util/api.py
--rw-rw-rw-   0        0        0      531 2021-08-08 16:59:22.000000 releng-tool-0.8.0/releng_tool/util/enum.py
--rw-rw-rw-   0        0        0     3143 2021-08-22 22:34:46.000000 releng-tool-0.8.0/releng_tool/util/env.py
--rw-rw-rw-   0        0        0     3231 2021-08-08 16:22:47.000000 releng-tool-0.8.0/releng_tool/util/file_flags.py
--rw-rw-rw-   0        0        0     9327 2021-08-22 00:12:36.000000 releng-tool-0.8.0/releng_tool/util/hash.py
--rw-rw-rw-   0        0        0    39375 2021-08-29 00:28:28.000000 releng-tool-0.8.0/releng_tool/util/io.py
--rw-rw-rw-   0        0        0     6415 2021-08-15 05:44:58.000000 releng-tool-0.8.0/releng_tool/util/log.py
--rw-rw-rw-   0        0        0     1325 2021-01-05 19:58:09.000000 releng-tool-0.8.0/releng_tool/util/platform.py
--rw-rw-rw-   0        0        0     3234 2020-09-24 01:19:56.000000 releng-tool-0.8.0/releng_tool/util/sort.py
--rw-rw-rw-   0        0        0     7557 2021-08-27 02:57:05.000000 releng-tool-0.8.0/releng_tool/util/string.py
--rw-rw-rw-   0        0        0     6899 2021-08-28 22:47:26.000000 releng-tool-0.8.0/releng_tool/util/win32.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.072200 releng-tool-0.8.0/releng_tool.egg-info/
--rw-rw-rw-   0        0        0     3289 2021-08-29 01:56:43.000000 releng-tool-0.8.0/releng_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17990 2021-08-29 01:56:43.000000 releng-tool-0.8.0/releng_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-29 01:56:43.000000 releng-tool-0.8.0/releng_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2021-08-29 01:56:43.000000 releng-tool-0.8.0/releng_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-08-29 01:56:43.000000 releng-tool-0.8.0/releng_tool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2021-08-29 01:56:43.000000 releng-tool-0.8.0/releng_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2021-08-29 01:56:43.000000 releng-tool-0.8.0/releng_tool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.024353 releng-tool-0.8.0/scripts/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.125908 releng-tool-0.8.0/scripts/completion/
--rw-rw-rw-   0        0        0     3143 2021-08-22 22:52:33.000000 releng-tool-0.8.0/scripts/completion/bash
--rw-rw-rw-   0        0        0     3927 2021-08-22 22:52:24.000000 releng-tool-0.8.0/scripts/completion/fish
--rw-rw-rw-   0        0        0     1032 2020-10-11 02:36:53.000000 releng-tool-0.8.0/scripts/completion/zsh
--rw-rw-rw-   0        0        0      318 2021-08-29 01:56:44.338786 releng-tool-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2170 2021-08-29 01:55:26.000000 releng-tool-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.127862 releng-tool-0.8.0/tests/
--rw-rw-rw-   0        0        0     6838 2021-08-16 01:38:40.000000 releng-tool-0.8.0/tests/__init__.py
--rw-rw-rw-   0        0        0     4136 2021-08-23 05:16:49.000000 releng-tool-0.8.0/tests/__main__.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.129816 releng-tool-0.8.0/tests/support/
--rw-rw-rw-   0        0        0      403 2021-08-16 01:05:34.000000 releng-tool-0.8.0/tests/support/__init__.py
--rw-rw-rw-   0        0        0     2167 2021-08-16 00:41:03.000000 releng-tool-0.8.0/tests/support/pkg_config_test.py
--rw-rw-rw-   0        0        0     6227 2021-08-22 05:57:15.000000 releng-tool-0.8.0/tests/support/site_tool_test.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.031188 releng-tool-0.8.0/tests/templates/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.130791 releng-tool-0.8.0/tests/templates/licenses/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.025329 releng-tool-0.8.0/tests/templates/licenses/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.132744 releng-tool-0.8.0/tests/templates/licenses/package/test-a/
--rw-rw-rw-   0        0        0       19 2021-08-07 15:39:00.000000 releng-tool-0.8.0/tests/templates/licenses/package/test-a/COPYING.bsd
--rw-rw-rw-   0        0        0       19 2021-08-07 15:39:00.000000 releng-tool-0.8.0/tests/templates/licenses/package/test-a/COPYING.mit
--rw-rw-rw-   0        0        0      189 2021-08-07 15:39:00.000000 releng-tool-0.8.0/tests/templates/licenses/package/test-a/test-a
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.133720 releng-tool-0.8.0/tests/templates/licenses/package/test-b/
--rw-rw-rw-   0        0        0       74 2021-08-07 15:39:00.000000 releng-tool-0.8.0/tests/templates/licenses/package/test-b/test-b
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.134697 releng-tool-0.8.0/tests/templates/licenses/package/test-c/
--rw-rw-rw-   0        0        0       19 2021-08-07 15:39:00.000000 releng-tool-0.8.0/tests/templates/licenses/package/test-c/LICENSE
--rw-rw-rw-   0        0        0      161 2021-08-07 15:39:00.000000 releng-tool-0.8.0/tests/templates/licenses/package/test-c/test-c
--rw-rw-rw-   0        0        0      112 2021-08-07 15:39:00.000000 releng-tool-0.8.0/tests/templates/licenses/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.135674 releng-tool-0.8.0/tests/templates/minimal/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.026306 releng-tool-0.8.0/tests/templates/minimal/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.135674 releng-tool-0.8.0/tests/templates/minimal/package/minimal/
--rw-rw-rw-   0        0        0       76 2020-09-13 21:48:20.000000 releng-tool-0.8.0/tests/templates/minimal/package/minimal/minimal
--rw-rw-rw-   0        0        0       83 2021-01-06 22:29:46.000000 releng-tool-0.8.0/tests/templates/minimal/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.136652 releng-tool-0.8.0/tests/templates/no-packages/
--rw-rw-rw-   0        0        0       67 2021-01-06 22:29:36.000000 releng-tool-0.8.0/tests/templates/no-packages/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.137627 releng-tool-0.8.0/tests/templates/remote-cfg/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.028259 releng-tool-0.8.0/tests/templates/remote-cfg/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.145439 releng-tool-0.8.0/tests/templates/remote-cfg/package/test/
--rw-rw-rw-   0        0        0       71 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg/package/test/.releng-tool
--rw-rw-rw-   0        0        0       97 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg/package/test/test
--rw-rw-rw-   0        0        0      141 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg/package/test/test-bootstrap
--rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.138603 releng-tool-0.8.0/tests/templates/remote-cfg-disabled/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.027282 releng-tool-0.8.0/tests/templates/remote-cfg-disabled/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.140556 releng-tool-0.8.0/tests/templates/remote-cfg-disabled/package/test/
--rw-rw-rw-   0        0        0       71 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg-disabled/package/test/.releng-tool
--rw-rw-rw-   0        0        0      129 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg-disabled/package/test/test
--rw-rw-rw-   0        0        0      141 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg-disabled/package/test/test-bootstrap
--rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg-disabled/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.141533 releng-tool-0.8.0/tests/templates/remote-cfg-override/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.028259 releng-tool-0.8.0/tests/templates/remote-cfg-override/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.143486 releng-tool-0.8.0/tests/templates/remote-cfg-override/package/test/
--rw-rw-rw-   0        0        0       71 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg-override/package/test/.releng-tool
--rw-rw-rw-   0        0        0      118 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg-override/package/test/test
--rw-rw-rw-   0        0        0      141 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg-override/package/test/test-bootstrap
--rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-cfg-override/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.146415 releng-tool-0.8.0/tests/templates/remote-scripts/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.031188 releng-tool-0.8.0/tests/templates/remote-scripts/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.163016 releng-tool-0.8.0/tests/templates/remote-scripts/package/test/
--rw-rw-rw-   0        0        0      128 2021-08-07 18:25:39.000000 releng-tool-0.8.0/tests/templates/remote-scripts/package/test/releng-build
--rw-rw-rw-   0        0        0      132 2021-08-07 18:25:41.000000 releng-tool-0.8.0/tests/templates/remote-scripts/package/test/releng-configure
--rw-rw-rw-   0        0        0      130 2021-08-07 18:25:36.000000 releng-tool-0.8.0/tests/templates/remote-scripts/package/test/releng-install
--rw-rw-rw-   0        0        0       97 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-scripts/package/test/test
--rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-scripts/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.146415 releng-tool-0.8.0/tests/templates/remote-scripts-disabled/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.029236 releng-tool-0.8.0/tests/templates/remote-scripts-disabled/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.149346 releng-tool-0.8.0/tests/templates/remote-scripts-disabled/package/test/
--rw-rw-rw-   0        0        0      128 2021-08-07 18:25:39.000000 releng-tool-0.8.0/tests/templates/remote-scripts-disabled/package/test/releng-build
--rw-rw-rw-   0        0        0      132 2021-08-07 18:25:41.000000 releng-tool-0.8.0/tests/templates/remote-scripts-disabled/package/test/releng-configure
--rw-rw-rw-   0        0        0      130 2021-08-07 18:25:36.000000 releng-tool-0.8.0/tests/templates/remote-scripts-disabled/package/test/releng-install
--rw-rw-rw-   0        0        0      130 2021-08-07 18:27:48.000000 releng-tool-0.8.0/tests/templates/remote-scripts-disabled/package/test/test
--rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-scripts-disabled/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.150324 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.030211 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.155204 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/test/
--rw-rw-rw-   0        0        0      128 2021-08-07 18:25:39.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/test/releng-build
--rw-rw-rw-   0        0        0      132 2021-08-07 18:25:41.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/test/releng-configure
--rw-rw-rw-   0        0        0      130 2021-08-07 18:25:36.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/test/releng-install
--rw-rw-rw-   0        0        0       97 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/test/test
--rw-rw-rw-   0        0        0      130 2021-08-07 18:26:47.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/test/test-build
--rw-rw-rw-   0        0        0      134 2021-08-07 18:26:45.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/test/test-configure
--rw-rw-rw-   0        0        0      132 2021-08-07 18:26:42.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/package/test/test-install
--rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-all/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.156180 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.030211 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.160087 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/package/test/
--rw-rw-rw-   0        0        0      128 2021-08-07 18:25:39.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/package/test/releng-build
--rw-rw-rw-   0        0        0      132 2021-08-07 18:25:41.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/package/test/releng-configure
--rw-rw-rw-   0        0        0      130 2021-08-07 18:25:36.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/package/test/releng-install
--rw-rw-rw-   0        0        0       97 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/package/test/test
--rw-rw-rw-   0        0        0      132 2021-08-07 18:26:42.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/package/test/test-install
--rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.8.0/tests/templates/remote-scripts-override-subset/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.163016 releng-tool-0.8.0/tests/templates/site-tool/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.031188 releng-tool-0.8.0/tests/templates/site-tool/package/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.163993 releng-tool-0.8.0/tests/templates/site-tool/package/test/
--rw-rw-rw-   0        0        0       90 2021-08-16 01:05:34.000000 releng-tool-0.8.0/tests/templates/site-tool/package/test/test
--rw-rw-rw-   0        0        0       80 2021-08-16 01:05:34.000000 releng-tool-0.8.0/tests/templates/site-tool/releng
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.165946 releng-tool-0.8.0/tests/tool-tests/
--rw-rw-rw-   0        0        0       25 2021-08-16 01:05:34.000000 releng-tool-0.8.0/tests/tool-tests/__init__.py
--rw-rw-rw-   0        0        0    14258 2021-08-22 05:19:48.000000 releng-tool-0.8.0/tests/tool-tests/test_tool_git.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.182546 releng-tool-0.8.0/tests/unit-tests/
--rw-rw-rw-   0        0        0       25 2021-01-02 21:11:50.000000 releng-tool-0.8.0/tests/unit-tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.033141 releng-tool-0.8.0/tests/unit-tests/assets/
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.313396 releng-tool-0.8.0/tests/unit-tests/assets/configs/
--rw-rw-rw-   0        0        0       59 2021-04-17 19:47:53.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/autotools-autoreconf-disabled
--rw-rw-rw-   0        0        0       58 2021-04-17 19:41:30.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/autotools-autoreconf-enabled
--rw-rw-rw-   0        0        0       63 2021-04-17 19:42:09.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/autotools-autoreconf-invalid
--rw-rw-rw-   0        0        0       53 2021-04-17 20:43:49.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-defs-invalid-base-type
--rw-rw-rw-   0        0        0       67 2021-04-17 21:20:10.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-defs-invalid-key-type
--rw-rw-rw-   0        0        0      108 2021-04-17 20:47:36.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-defs-invalid-strs
--rw-rw-rw-   0        0        0       68 2021-04-17 20:44:03.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-defs-invalid-value-type
--rw-rw-rw-   0        0        0      109 2021-04-17 21:06:40.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-defs-valid
--rw-rw-rw-   0        0        0       52 2021-04-17 20:54:04.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-env-invalid-base-type
--rw-rw-rw-   0        0        0       66 2021-04-17 21:20:08.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-env-invalid-key-type
--rw-rw-rw-   0        0        0      107 2021-04-17 20:54:03.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-env-invalid-strs
--rw-rw-rw-   0        0        0       67 2021-04-17 20:54:01.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-env-invalid-value-type
--rw-rw-rw-   0        0        0      108 2021-04-17 21:06:43.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-env-valid
--rw-rw-rw-   0        0        0       49 2021-04-17 21:25:39.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-opts-invalid-base-type
--rw-rw-rw-   0        0        0       68 2021-04-17 21:09:56.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-opts-invalid-key-type
--rw-rw-rw-   0        0        0       68 2021-04-17 21:09:54.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-opts-invalid-value-type
--rw-rw-rw-   0        0        0      109 2021-04-17 21:09:53.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-opts-valid-dict
--rw-rw-rw-   0        0        0       52 2021-04-17 21:26:32.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-opts-valid-str
--rw-rw-rw-   0        0        0       96 2021-04-17 21:09:50.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/build-opts-valid-strs
--rw-rw-rw-   0        0        0       52 2021-04-17 20:46:30.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-defs-invalid-base-type
--rw-rw-rw-   0        0        0       66 2021-04-17 21:20:05.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-defs-invalid-key-type
--rw-rw-rw-   0        0        0      107 2021-04-17 20:47:24.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-defs-invalid-strs
--rw-rw-rw-   0        0        0       67 2021-04-17 20:46:25.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-defs-invalid-value-type
--rw-rw-rw-   0        0        0      108 2021-04-17 21:06:44.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-defs-valid
--rw-rw-rw-   0        0        0       51 2021-04-17 20:53:59.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-env-invalid-base-type
--rw-rw-rw-   0        0        0       65 2021-04-17 21:20:03.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-env-invalid-key-type
--rw-rw-rw-   0        0        0      106 2021-04-17 20:53:57.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-env-invalid-strs
--rw-rw-rw-   0        0        0       66 2021-04-17 20:53:56.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-env-invalid-value-type
--rw-rw-rw-   0        0        0      107 2021-04-17 21:06:46.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-env-valid
--rw-rw-rw-   0        0        0       48 2021-04-17 21:25:38.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-opts-invalid-base-type
--rw-rw-rw-   0        0        0       67 2021-04-17 21:10:22.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-opts-invalid-key-type
--rw-rw-rw-   0        0        0       67 2021-04-17 21:10:18.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-opts-invalid-value-type
--rw-rw-rw-   0        0        0      108 2021-04-17 21:10:13.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-opts-valid-dict
--rw-rw-rw-   0        0        0       51 2021-04-17 21:26:28.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-opts-valid-str
--rw-rw-rw-   0        0        0       95 2021-04-17 21:10:25.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/conf-opts-valid-strs
--rw-rw-rw-   0        0        0       49 2021-04-17 21:45:35.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/deps-invalid-type
--rw-rw-rw-   0        0        0       74 2021-04-17 21:43:34.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/deps-invalid-value
--rw-rw-rw-   0        0        0       48 2021-04-17 21:43:58.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/deps-valid-empty
--rw-rw-rw-   0        0        0       89 2021-04-17 21:43:53.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/deps-valid-multiple
--rw-rw-rw-   0        0        0       51 2021-04-17 21:46:07.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/deps-valid-single
--rw-rw-rw-   0        0        0       59 2021-04-17 19:53:08.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/devmode-ignore-cache-disabled
--rw-rw-rw-   0        0        0       58 2021-04-17 19:53:07.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/devmode-ignore-cache-enabled
--rw-rw-rw-   0        0        0       63 2021-04-17 19:53:05.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/devmode-ignore-cache-invalid
--rw-rw-rw-   0        0        0       53 2021-04-18 21:54:06.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/devmode-revision-invalid-type
--rw-rw-rw-   0        0        0       71 2021-04-18 21:54:23.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/devmode-revision-valid
--rw-rw-rw-   0        0        0       42 2021-04-18 00:15:42.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/ext-mods-invalid-type
--rw-rw-rw-   0        0        0      130 2021-04-18 00:20:30.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/ext-mods-valid-data
--rw-rw-rw-   0        0        0       42 2021-04-18 00:20:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/ext-mods-valid-empty
--rw-rw-rw-   0        0        0       47 2021-04-18 03:22:59.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/external-flag-disabled
--rw-rw-rw-   0        0        0       46 2021-04-18 03:23:05.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/external-flag-enabled
--rw-rw-rw-   0        0        0       51 2021-04-18 03:23:02.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/external-flag-invalid
--rw-rw-rw-   0        0        0       49 2021-04-18 22:02:22.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/extract-type-invalid-type
--rw-rw-rw-   0        0        0       74 2021-04-18 22:09:33.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/extract-type-valid
--rw-rw-rw-   0        0        0       53 2021-04-17 19:55:28.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/fixed-jobs-invalid-type
--rw-rw-rw-   0        0        0       45 2021-04-17 19:58:05.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/fixed-jobs-invalid-value
--rw-rw-rw-   0        0        0       46 2021-04-17 19:55:35.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/fixed-jobs-valid
--rw-rw-rw-   0        0        0       53 2021-04-18 20:08:42.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-config-invalid-base-type
--rw-rw-rw-   0        0        0       67 2021-04-18 20:08:40.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-config-invalid-key-type
--rw-rw-rw-   0        0        0      108 2021-04-18 20:09:23.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-config-invalid-strs
--rw-rw-rw-   0        0        0       68 2021-04-18 20:08:37.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-config-invalid-value-type
--rw-rw-rw-   0        0        0      109 2021-04-18 20:08:44.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-config-valid
--rw-rw-rw-   0        0        0       52 2021-04-18 13:46:32.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-depth-invalid-type
--rw-rw-rw-   0        0        0       45 2021-04-18 13:46:34.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-depth-invalid-value
--rw-rw-rw-   0        0        0       45 2021-04-18 13:46:37.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-depth-valid-nonzero
--rw-rw-rw-   0        0        0       44 2021-04-18 13:46:35.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-depth-valid-zero
--rw-rw-rw-   0        0        0       49 2021-04-18 20:02:50.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-refspecs-invalid-type
--rw-rw-rw-   0        0        0       76 2021-04-18 20:03:36.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-refspecs-invalid-value
--rw-rw-rw-   0        0        0       48 2021-04-18 20:02:58.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-refspecs-valid-empty
--rw-rw-rw-   0        0        0      101 2021-04-18 20:03:34.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-refspecs-valid-multiple
--rw-rw-rw-   0        0        0       55 2021-04-18 20:03:27.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-refspecs-valid-single
--rw-rw-rw-   0        0        0       51 2021-08-22 01:18:56.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-submodules-disabled
--rw-rw-rw-   0        0        0       50 2021-08-22 01:18:56.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-submodules-enabled
--rw-rw-rw-   0        0        0       55 2021-08-22 01:18:56.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/git-submodules-invalid
--rw-rw-rw-   0        0        0       55 2021-04-17 20:46:07.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-defs-invalid-base-type
--rw-rw-rw-   0        0        0       69 2021-04-17 21:20:00.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-defs-invalid-key-type
--rw-rw-rw-   0        0        0      110 2021-04-17 20:47:14.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-defs-invalid-strs
--rw-rw-rw-   0        0        0       70 2021-04-17 20:46:04.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-defs-invalid-value-type
--rw-rw-rw-   0        0        0      111 2021-04-17 21:06:50.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-defs-valid
--rw-rw-rw-   0        0        0       54 2021-04-17 20:54:12.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-env-invalid-base-type
--rw-rw-rw-   0        0        0       68 2021-04-17 21:19:58.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-env-invalid-key-type
--rw-rw-rw-   0        0        0      109 2021-04-17 20:54:10.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-env-invalid-strs
--rw-rw-rw-   0        0        0       69 2021-04-17 20:54:08.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-env-invalid-value-type
--rw-rw-rw-   0        0        0      110 2021-04-17 21:06:52.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-env-valid
--rw-rw-rw-   0        0        0       51 2021-04-17 21:25:35.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-opts-invalid-base-type
--rw-rw-rw-   0        0        0       70 2021-04-17 20:59:40.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-opts-invalid-key-type
--rw-rw-rw-   0        0        0       70 2021-04-17 20:58:22.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-opts-invalid-value-type
--rw-rw-rw-   0        0        0      111 2021-04-17 21:07:03.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-opts-valid-dict
--rw-rw-rw-   0        0        0       54 2021-04-17 21:26:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-opts-valid-str
--rw-rw-rw-   0        0        0       98 2021-04-17 21:00:32.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-opts-valid-strs
--rw-rw-rw-   0        0        0       51 2021-04-18 02:08:44.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-type-invalid-type
--rw-rw-rw-   0        0        0       55 2021-04-18 02:08:46.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-type-invalid-value
--rw-rw-rw-   0        0        0       52 2021-04-18 01:41:21.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-type-valid-host
--rw-rw-rw-   0        0        0       54 2021-04-18 01:41:18.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-type-valid-images
--rw-rw-rw-   0        0        0       55 2021-04-18 01:55:11.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-type-valid-staging
--rw-rw-rw-   0        0        0       66 2021-04-18 01:41:36.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-type-valid-staging-target
--rw-rw-rw-   0        0        0       54 2021-04-18 01:41:29.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/install-type-valid-target
--rw-rw-rw-   0        0        0       68 2021-04-18 03:24:03.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/internal-external-flag-conflict1
--rw-rw-rw-   0        0        0       70 2021-04-18 03:23:49.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/internal-external-flag-conflict2
--rw-rw-rw-   0        0        0       69 2021-04-18 03:55:16.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/internal-external-flag-disabled
--rw-rw-rw-   0        0        0       69 2021-04-18 03:55:13.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/internal-external-flag-enabled
--rw-rw-rw-   0        0        0       47 2021-04-18 03:22:02.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/internal-flag-disabled
--rw-rw-rw-   0        0        0       46 2021-04-18 03:22:05.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/internal-flag-enabled
--rw-rw-rw-   0        0        0       51 2021-04-18 03:22:07.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/internal-flag-invalid
--rw-rw-rw-   0        0        0       50 2021-04-18 19:45:07.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-files-invalid-type
--rw-rw-rw-   0        0        0       82 2021-04-18 19:46:13.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-files-invalid-value
--rw-rw-rw-   0        0        0       49 2021-04-18 19:45:03.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-files-valid-empty
--rw-rw-rw-   0        0        0      117 2021-04-18 19:45:57.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-files-valid-multiple
--rw-rw-rw-   0        0        0       61 2021-04-18 19:46:05.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-files-valid-single
--rw-rw-rw-   0        0        0       44 2021-04-18 19:45:29.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-invalid-type
--rw-rw-rw-   0        0        0       71 2021-04-18 19:45:40.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-invalid-value
--rw-rw-rw-   0        0        0       43 2021-04-18 19:45:25.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-valid-empty
--rw-rw-rw-   0        0        0       96 2021-04-18 19:45:45.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-valid-multiple
--rw-rw-rw-   0        0        0       50 2021-04-18 19:46:40.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/license-valid-single
--rw-rw-rw-   0        0        0       24 2021-04-17 19:47:07.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/missing
--rw-rw-rw-   0        0        0       52 2021-04-18 03:21:39.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/no-extraction-disabled
--rw-rw-rw-   0        0        0       51 2021-04-18 03:21:42.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/no-extraction-enabled
--rw-rw-rw-   0        0        0       56 2021-04-18 03:21:44.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/no-extraction-invalid
--rw-rw-rw-   0        0        0       50 2021-04-18 19:14:33.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/pkg-type-invalid-type
--rw-rw-rw-   0        0        0       47 2021-04-18 19:14:31.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/pkg-type-invalid-value
--rw-rw-rw-   0        0        0       49 2021-04-18 19:14:38.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/pkg-type-valid-autotools
--rw-rw-rw-   0        0        0       45 2021-04-18 19:15:18.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/pkg-type-valid-cmake
--rw-rw-rw-   0        0        0       46 2021-04-18 19:15:11.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/pkg-type-valid-python
--rw-rw-rw-   0        0        0       46 2021-04-18 19:15:06.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/pkg-type-valid-script
--rw-rw-rw-   0        0        0       43 2021-04-18 19:31:24.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/prefix-invalid-type
--rw-rw-rw-   0        0        0       50 2021-04-18 19:31:29.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/prefix-valid
--rw-rw-rw-   0        0        0       55 2021-04-18 19:24:34.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/python-interpreter-invalid-type
--rw-rw-rw-   0        0        0       62 2021-04-18 19:24:46.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/python-interpreter-valid
--rw-rw-rw-   0        0        0       45 2021-04-18 19:29:51.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/revision-invalid-type
--rw-rw-rw-   0        0        0       54 2021-04-18 19:30:19.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/revision-valid-explicit
--rw-rw-rw-   0        0        0       28 2021-04-18 19:30:27.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/revision-valid-implicit
--rw-rw-rw-   0        0        0       43 2021-04-18 19:20:49.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/site-invalid-type
--rw-rw-rw-   0        0        0       68 2021-04-18 19:21:21.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/site-valid
--rw-rw-rw-   0        0        0       57 2021-08-07 15:30:54.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/skip-remote-config-disabled
--rw-rw-rw-   0        0        0       56 2021-08-07 15:30:53.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/skip-remote-config-enabled
--rw-rw-rw-   0        0        0       61 2021-08-07 15:30:48.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/skip-remote-config-invalid
--rw-rw-rw-   0        0        0       58 2021-08-07 17:49:23.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/skip-remote-scripts-disabled
--rw-rw-rw-   0        0        0       57 2021-08-07 17:49:22.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/skip-remote-scripts-enabled
--rw-rw-rw-   0        0        0       62 2021-08-07 17:49:18.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/skip-remote-scripts-invalid
--rw-rw-rw-   0        0        0       54 2021-04-18 13:47:03.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/strip-count-invalid-type
--rw-rw-rw-   0        0        0       47 2021-04-18 13:47:02.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/strip-count-invalid-value
--rw-rw-rw-   0        0        0       46 2021-04-18 13:47:05.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/strip-count-valid-nonzero
--rw-rw-rw-   0        0        0       46 2021-04-18 13:47:00.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/strip-count-valid-zero
--rw-rw-rw-   0        0        0       47 2021-04-18 14:41:23.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-bzr-nosite
--rw-rw-rw-   0        0        0       47 2021-04-18 14:43:00.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-cvs-nosite
--rw-rw-rw-   0        0        0       47 2021-04-18 14:43:04.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-git-nosite
--rw-rw-rw-   0        0        0       46 2021-04-18 14:42:36.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-hg-nosite
--rw-rw-rw-   0        0        0       47 2021-04-18 14:42:47.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-scp-nosite
--rw-rw-rw-   0        0        0       47 2021-04-18 14:42:51.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-svn-nosite
--rw-rw-rw-   0        0        0       54 2021-04-18 14:13:56.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-type
--rw-rw-rw-   0        0        0       47 2021-04-18 14:42:55.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-url-nosite
--rw-rw-rw-   0        0        0       51 2021-04-18 14:12:40.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-invalid-value
--rw-rw-rw-   0        0        0       68 2021-04-18 14:40:13.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-bzr-explicit
--rw-rw-rw-   0        0        0       51 2021-04-18 14:23:11.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-bzr-implicit
--rw-rw-rw-   0        0        0       68 2021-04-18 14:40:15.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-explicit
--rw-rw-rw-   0        0        0       51 2021-04-18 14:23:18.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit
--rw-rw-rw-   0        0        0      100 2021-08-29 00:35:32.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit2
--rw-rw-rw-   0        0        0       92 2021-08-29 00:35:39.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit3
--rw-rw-rw-   0        0        0       95 2021-08-29 00:41:03.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit4
--rw-rw-rw-   0        0        0       96 2021-08-29 00:41:55.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit5
--rw-rw-rw-   0        0        0       96 2021-08-29 00:41:54.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit6
--rw-rw-rw-   0        0        0       68 2021-04-18 14:40:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-git-explicit
--rw-rw-rw-   0        0        0       51 2021-04-18 14:23:42.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-git-implicit1
--rw-rw-rw-   0        0        0       51 2021-04-18 14:23:49.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-git-implicit2
--rw-rw-rw-   0        0        0       67 2021-04-18 14:40:18.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-hg-explicit
--rw-rw-rw-   0        0        0       50 2021-04-18 14:23:59.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-hg-implicit
--rw-rw-rw-   0        0        0       49 2021-04-18 14:19:45.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-local-explicit
--rw-rw-rw-   0        0        0       45 2021-04-18 14:24:52.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-local-implicit
--rw-rw-rw-   0        0        0       48 2021-04-18 14:19:42.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-none-explicit
--rw-rw-rw-   0        0        0       24 2021-04-18 14:25:18.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-none-implicit
--rw-rw-rw-   0        0        0       68 2021-04-18 14:40:19.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-scp-explicit
--rw-rw-rw-   0        0        0       51 2021-04-18 14:24:21.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-scp-implicit
--rw-rw-rw-   0        0        0       68 2021-04-18 14:40:20.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-svn-explicit
--rw-rw-rw-   0        0        0       51 2021-04-18 14:24:31.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-svn-implicit
--rw-rw-rw-   0        0        0       68 2021-04-18 14:40:22.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-url-explicit
--rw-rw-rw-   0        0        0       51 2021-04-18 14:23:01.000000 releng-tool-0.8.0/tests/unit-tests/assets/configs/vcs-type-valid-url-implicit
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.315349 releng-tool-0.8.0/tests/unit-tests/assets/copy-check-01/
--rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/copy-check-01/test-file-a
--rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/copy-check-01/test-file-b
--rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/copy-check-01/test-file-x
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.317303 releng-tool-0.8.0/tests/unit-tests/assets/copy-check-02/
--rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/copy-check-02/test-file-b
--rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/copy-check-02/test-file-c
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.328044 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/
--rw-rw-rw-   0        0        0       78 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/invalid-hash-sample-a
--rw-rw-rw-   0        0        0       80 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/invalid-hash-sample-b
--rw-rw-rw-   0        0        0       94 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/invalid-hash-sample-c
--rw-rw-rw-   0        0        0       72 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/sample-asset
--rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-a
--rw-rw-rw-   0        0        0      322 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-b
--rw-rw-rw-   0        0        0      539 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-c
--rw-rw-rw-   0        0        0       39 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-d
--rw-rw-rw-   0        0        0      107 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/verify-bad-format
--rw-rw-rw-   0        0        0      122 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/verify-bad-hash
--rw-rw-rw-   0        0        0       31 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/verify-empty
--rw-rw-rw-   0        0        0      161 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/verify-missing-archive
--rw-rw-rw-   0        0        0      163 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/verify-missing-listed
--rw-rw-rw-   0        0        0      612 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/verify-success
--rw-rw-rw-   0        0        0       84 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/verify-unknown-hash-type
-drwxrwxrwx   0        0        0        0 2021-08-29 01:56:44.332927 releng-tool-0.8.0/tests/unit-tests/assets/shebang-interpreter/
--rw-rw-rw-   0        0        0       40 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/shebang-interpreter/example.py
--rw-rw-rw-   0        0        0       48 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/shebang-interpreter/interpreter
--rw-rw-rw-   0        0        0       55 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/shebang-interpreter/interpreter-arg
--rw-rw-rw-   0        0        0      102 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/shebang-interpreter/interpreter-args-multiple
--rw-rw-rw-   0        0        0     5084 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/shebang-interpreter/interpreter-extremely-long
--rw-rw-rw-   0        0        0      161 2020-09-13 21:08:17.000000 releng-tool-0.8.0/tests/unit-tests/assets/shebang-interpreter/interpreter-whitespaces
--rw-rw-rw-   0        0        0     1139 2021-08-08 16:59:05.000000 releng-tool-0.8.0/tests/unit-tests/test_engine_run_actions.py
--rw-rw-rw-   0        0        0     1389 2021-08-07 15:31:28.000000 releng-tool-0.8.0/tests/unit-tests/test_engine_run_defaults.py
--rw-rw-rw-   0        0        0      758 2021-04-10 04:22:56.000000 releng-tool-0.8.0/tests/unit-tests/test_engine_run_file_flags.py
--rw-rw-rw-   0        0        0     1938 2021-01-02 21:44:37.000000 releng-tool-0.8.0/tests/unit-tests/test_file_flags.py
--rw-rw-rw-   0        0        0    11471 2021-08-07 17:48:35.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_configs.py
--rw-rw-rw-   0        0        0      945 2021-04-18 18:21:15.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_autotools.py
--rw-rw-rw-   0        0        0     2257 2021-04-18 21:58:00.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_devmode.py
--rw-rw-rw-   0        0        0     2372 2021-08-08 15:36:26.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_extensions.py
--rw-rw-rw-   0        0        0     3738 2021-08-22 01:18:56.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_git.py
--rw-rw-rw-   0        0        0    12236 2021-04-18 18:23:41.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_stageopts.py
--rw-rw-rw-   0        0        0     1495 2021-04-18 19:16:31.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_type.py
--rw-rw-rw-   0        0        0     5993 2021-08-29 00:42:03.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_vcs_type.py
--rw-rw-rw-   0        0        0     2173 2021-08-28 21:45:15.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_pipeline_licenses.py
--rw-rw-rw-   0        0        0     1328 2021-08-07 19:10:57.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_pipeline_remote_cfg.py
--rw-rw-rw-   0        0        0     2596 2021-08-07 19:10:47.000000 releng-tool-0.8.0/tests/unit-tests/test_pkg_pipeline_remote_scripts.py
--rw-rw-rw-   0        0        0      863 2021-04-17 15:38:34.000000 releng-tool-0.8.0/tests/unit-tests/test_util_common.py
--rw-rw-rw-   0        0        0     2387 2021-08-22 22:36:00.000000 releng-tool-0.8.0/tests/unit-tests/test_util_env.py
--rw-rw-rw-   0        0        0     5001 2021-08-16 00:39:58.000000 releng-tool-0.8.0/tests/unit-tests/test_util_hash.py
--rw-rw-rw-   0        0        0    17072 2021-08-16 01:05:34.000000 releng-tool-0.8.0/tests/unit-tests/test_util_io.py
--rw-rw-rw-   0        0        0     4541 2020-09-24 04:32:39.000000 releng-tool-0.8.0/tests/unit-tests/test_util_sort.py
--rw-rw-rw-   0        0        0     3124 2020-09-24 02:54:03.000000 releng-tool-0.8.0/tests/unit-tests/test_util_string.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.413546 releng-tool-0.9.0/
+-rw-rw-rw-   0        0        0     1300 2021-08-30 02:55:47.000000 releng-tool-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      158 2021-04-13 22:39:01.000000 releng-tool-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3446 2021-10-02 23:25:46.413546 releng-tool-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2431 2021-09-29 03:31:28.000000 releng-tool-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.984818 releng-tool-0.9.0/releng/
+-rw-rw-rw-   0        0        0      338 2020-09-27 23:50:14.000000 releng-tool-0.9.0/releng/__init__.py
+-rw-rw-rw-   0        0        0      293 2020-09-13 21:06:07.000000 releng-tool-0.9.0/releng/__main__.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.985784 releng-tool-0.9.0/releng/api/
+-rw-rw-rw-   0        0        0      417 2020-09-27 23:50:14.000000 releng-tool-0.9.0/releng/api/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.993593 releng-tool-0.9.0/releng_tool/
+-rw-rw-rw-   0        0        0     2325 2021-10-02 23:23:44.000000 releng-tool-0.9.0/releng_tool/__init__.py
+-rw-rw-rw-   0        0        0     8436 2021-08-30 02:55:47.000000 releng-tool-0.9.0/releng_tool/__main__.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.022890 releng-tool-0.9.0/releng_tool/api/
+-rw-rw-rw-   0        0        0    23206 2021-10-02 00:17:00.000000 releng-tool-0.9.0/releng_tool/api/__init__.py
+-rw-rw-rw-   0        0        0     8608 2021-10-01 02:56:33.000000 releng-tool-0.9.0/releng_tool/defs.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.031679 releng-tool-0.9.0/releng_tool/engine/
+-rw-rw-rw-   0        0        0    33430 2021-10-02 23:18:46.000000 releng-tool-0.9.0/releng_tool/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.035585 releng-tool-0.9.0/releng_tool/engine/autotools/
+-rw-rw-rw-   0        0        0       25 2021-01-05 19:32:45.000000 releng-tool-0.9.0/releng_tool/engine/autotools/__init__.py
+-rw-rw-rw-   0        0        0     1459 2021-01-05 19:34:26.000000 releng-tool-0.9.0/releng_tool/engine/autotools/build.py
+-rw-rw-rw-   0        0        0     1938 2021-01-05 19:34:06.000000 releng-tool-0.9.0/releng_tool/engine/autotools/configure.py
+-rw-rw-rw-   0        0        0     1722 2021-01-05 19:34:04.000000 releng-tool-0.9.0/releng_tool/engine/autotools/install.py
+-rw-rw-rw-   0        0        0     1712 2021-01-05 20:04:25.000000 releng-tool-0.9.0/releng_tool/engine/bootstrap.py
+-rw-rw-rw-   0        0        0     3143 2021-08-23 01:27:12.000000 releng-tool-0.9.0/releng_tool/engine/build.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.038513 releng-tool-0.9.0/releng_tool/engine/cmake/
+-rw-rw-rw-   0        0        0       25 2021-01-05 19:34:36.000000 releng-tool-0.9.0/releng_tool/engine/cmake/__init__.py
+-rw-rw-rw-   0        0        0     2019 2021-01-05 19:35:48.000000 releng-tool-0.9.0/releng_tool/engine/cmake/build.py
+-rw-rw-rw-   0        0        0     3319 2021-01-05 19:35:36.000000 releng-tool-0.9.0/releng_tool/engine/cmake/configure.py
+-rw-rw-rw-   0        0        0     1941 2021-01-05 19:35:34.000000 releng-tool-0.9.0/releng_tool/engine/cmake/install.py
+-rw-rw-rw-   0        0        0     3537 2021-08-23 01:27:05.000000 releng-tool-0.9.0/releng_tool/engine/configure.py
+-rw-rw-rw-   0        0        0     5035 2021-01-05 20:05:49.000000 releng-tool-0.9.0/releng_tool/engine/extract.py
+-rw-rw-rw-   0        0        0    12525 2021-10-02 03:01:09.000000 releng-tool-0.9.0/releng_tool/engine/fetch.py
+-rw-rw-rw-   0        0        0     2713 2021-08-23 05:20:55.000000 releng-tool-0.9.0/releng_tool/engine/init.py
+-rw-rw-rw-   0        0        0     3861 2021-08-23 01:26:59.000000 releng-tool-0.9.0/releng_tool/engine/install.py
+-rw-rw-rw-   0        0        0     2652 2021-08-23 01:26:53.000000 releng-tool-0.9.0/releng_tool/engine/patch.py
+-rw-rw-rw-   0        0        0     1668 2021-01-05 19:38:47.000000 releng-tool-0.9.0/releng_tool/engine/post.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.041443 releng-tool-0.9.0/releng_tool/engine/python/
+-rw-rw-rw-   0        0        0       25 2021-01-05 19:36:02.000000 releng-tool-0.9.0/releng_tool/engine/python/__init__.py
+-rw-rw-rw-   0        0        0     2148 2021-01-05 19:36:42.000000 releng-tool-0.9.0/releng_tool/engine/python/build.py
+-rw-rw-rw-   0        0        0     2713 2021-01-05 19:36:29.000000 releng-tool-0.9.0/releng_tool/engine/python/install.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.044373 releng-tool-0.9.0/releng_tool/engine/script/
+-rw-rw-rw-   0        0        0       25 2021-01-05 19:37:53.000000 releng-tool-0.9.0/releng_tool/engine/script/__init__.py
+-rw-rw-rw-   0        0        0     1515 2021-08-07 18:34:05.000000 releng-tool-0.9.0/releng_tool/engine/script/build.py
+-rw-rw-rw-   0        0        0     1646 2021-08-07 18:34:15.000000 releng-tool-0.9.0/releng_tool/engine/script/configure.py
+-rw-rw-rw-   0        0        0     1594 2021-08-07 18:34:20.000000 releng-tool-0.9.0/releng_tool/engine/script/install.py
+-rw-rw-rw-   0        0        0     1066 2021-04-18 17:43:53.000000 releng-tool-0.9.0/releng_tool/exceptions.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.045351 releng-tool-0.9.0/releng_tool/ext/
+-rw-rw-rw-   0        0        0       25 2021-01-05 19:50:53.000000 releng-tool-0.9.0/releng_tool/ext/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.046325 releng-tool-0.9.0/releng_tool/ext/seed/
+-rw-rw-rw-   0        0        0     1054 2020-09-24 01:42:49.000000 releng-tool-0.9.0/releng_tool/ext/seed/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.050231 releng-tool-0.9.0/releng_tool/extract/
+-rw-rw-rw-   0        0        0       25 2021-01-05 19:51:10.000000 releng-tool-0.9.0/releng_tool/extract/__init__.py
+-rw-rw-rw-   0        0        0     6213 2021-01-05 19:51:48.000000 releng-tool-0.9.0/releng_tool/extract/archive.py
+-rw-rw-rw-   0        0        0     5916 2021-10-02 17:49:30.000000 releng-tool-0.9.0/releng_tool/extract/git.py
+-rw-rw-rw-   0        0        0     1197 2021-01-05 19:52:13.000000 releng-tool-0.9.0/releng_tool/extract/mercurial.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.058044 releng-tool-0.9.0/releng_tool/fetch/
+-rw-rw-rw-   0        0        0       25 2021-08-21 21:21:05.000000 releng-tool-0.9.0/releng_tool/fetch/__init__.py
+-rw-rw-rw-   0        0        0     1306 2021-01-05 19:54:47.000000 releng-tool-0.9.0/releng_tool/fetch/bzr.py
+-rw-rw-rw-   0        0        0     2330 2021-08-29 02:15:53.000000 releng-tool-0.9.0/releng_tool/fetch/cvs.py
+-rw-rw-rw-   0        0        0    20999 2021-10-02 17:49:42.000000 releng-tool-0.9.0/releng_tool/fetch/git.py
+-rw-rw-rw-   0        0        0     2181 2021-01-05 19:53:49.000000 releng-tool-0.9.0/releng_tool/fetch/mercurial.py
+-rw-rw-rw-   0        0        0     1082 2021-01-05 19:53:35.000000 releng-tool-0.9.0/releng_tool/fetch/scp.py
+-rw-rw-rw-   0        0        0     1602 2021-01-05 19:53:14.000000 releng-tool-0.9.0/releng_tool/fetch/svn.py
+-rw-rw-rw-   0        0        0     2987 2021-08-29 02:15:53.000000 releng-tool-0.9.0/releng_tool/fetch/url.py
+-rw-rw-rw-   0        0        0    10655 2021-10-01 02:56:33.000000 releng-tool-0.9.0/releng_tool/opts.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.063909 releng-tool-0.9.0/releng_tool/packages/
+-rw-rw-rw-   0        0        0     2050 2021-08-29 02:15:53.000000 releng-tool-0.9.0/releng_tool/packages/__init__.py
+-rw-rw-rw-   0        0        0     5956 2021-08-07 20:44:23.000000 releng-tool-0.9.0/releng_tool/packages/exceptions.py
+-rw-rw-rw-   0        0        0    43496 2021-10-02 03:04:06.000000 releng-tool-0.9.0/releng_tool/packages/manager.py
+-rw-rw-rw-   0        0        0     5023 2021-10-02 00:04:25.000000 releng-tool-0.9.0/releng_tool/packages/package.py
+-rw-rw-rw-   0        0        0    13383 2021-08-29 02:15:53.000000 releng-tool-0.9.0/releng_tool/packages/pipeline.py
+-rw-rw-rw-   0        0        0     5588 2021-01-05 20:00:51.000000 releng-tool-0.9.0/releng_tool/prerequisites.py
+-rw-rw-rw-   0        0        0    12723 2021-08-15 23:53:29.000000 releng-tool-0.9.0/releng_tool/registry.py
+-rw-rw-rw-   0        0        0    10547 2021-08-30 02:55:47.000000 releng-tool-0.9.0/releng_tool/stats.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.075621 releng-tool-0.9.0/releng_tool/tool/
+-rw-rw-rw-   0        0        0     5473 2021-08-31 02:46:27.000000 releng-tool-0.9.0/releng_tool/tool/__init__.py
+-rw-rw-rw-   0        0        0      266 2021-01-05 19:56:40.000000 releng-tool-0.9.0/releng_tool/tool/autoreconf.py
+-rw-rw-rw-   0        0        0      840 2021-01-05 19:56:30.000000 releng-tool-0.9.0/releng_tool/tool/bzr.py
+-rw-rw-rw-   0        0        0      236 2021-01-05 19:56:22.000000 releng-tool-0.9.0/releng_tool/tool/cmake.py
+-rw-rw-rw-   0        0        0      676 2021-01-05 19:56:18.000000 releng-tool-0.9.0/releng_tool/tool/cvs.py
+-rw-rw-rw-   0        0        0     3951 2021-10-02 18:54:50.000000 releng-tool-0.9.0/releng_tool/tool/git.py
+-rw-rw-rw-   0        0        0     1060 2021-08-30 02:56:50.000000 releng-tool-0.9.0/releng_tool/tool/gpg.py
+-rw-rw-rw-   0        0        0      723 2021-01-05 19:56:11.000000 releng-tool-0.9.0/releng_tool/tool/hg.py
+-rw-rw-rw-   0        0        0      230 2021-01-05 19:56:06.000000 releng-tool-0.9.0/releng_tool/tool/make.py
+-rw-rw-rw-   0        0        0      524 2021-01-05 19:56:03.000000 releng-tool-0.9.0/releng_tool/tool/patch.py
+-rw-rw-rw-   0        0        0     3852 2021-08-29 02:15:53.000000 releng-tool-0.9.0/releng_tool/tool/python.py
+-rw-rw-rw-   0        0        0     1376 2021-01-05 19:56:57.000000 releng-tool-0.9.0/releng_tool/tool/scp.py
+-rw-rw-rw-   0        0        0      379 2021-01-05 19:55:36.000000 releng-tool-0.9.0/releng_tool/tool/svn.py
+-rw-rw-rw-   0        0        0      381 2021-01-05 19:55:30.000000 releng-tool-0.9.0/releng_tool/tool/tar.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.087339 releng-tool-0.9.0/releng_tool/util/
+-rw-rw-rw-   0        0        0      531 2021-04-17 15:29:41.000000 releng-tool-0.9.0/releng_tool/util/__init__.py
+-rw-rw-rw-   0        0        0      795 2021-04-18 01:29:24.000000 releng-tool-0.9.0/releng_tool/util/api.py
+-rw-rw-rw-   0        0        0      531 2021-08-08 16:59:22.000000 releng-tool-0.9.0/releng_tool/util/enum.py
+-rw-rw-rw-   0        0        0     3143 2021-10-01 04:47:53.000000 releng-tool-0.9.0/releng_tool/util/env.py
+-rw-rw-rw-   0        0        0     3338 2021-10-02 17:42:36.000000 releng-tool-0.9.0/releng_tool/util/file_flags.py
+-rw-rw-rw-   0        0        0     9260 2021-08-30 04:11:43.000000 releng-tool-0.9.0/releng_tool/util/hash.py
+-rw-rw-rw-   0        0        0    39375 2021-08-29 02:15:53.000000 releng-tool-0.9.0/releng_tool/util/io.py
+-rw-rw-rw-   0        0        0     6415 2021-10-02 17:49:58.000000 releng-tool-0.9.0/releng_tool/util/log.py
+-rw-rw-rw-   0        0        0     1325 2021-01-05 19:58:09.000000 releng-tool-0.9.0/releng_tool/util/platform.py
+-rw-rw-rw-   0        0        0     3234 2020-09-24 01:19:56.000000 releng-tool-0.9.0/releng_tool/util/sort.py
+-rw-rw-rw-   0        0        0     7632 2021-08-30 02:55:47.000000 releng-tool-0.9.0/releng_tool/util/string.py
+-rw-rw-rw-   0        0        0     6899 2021-08-29 02:15:53.000000 releng-tool-0.9.0/releng_tool/util/win32.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.021913 releng-tool-0.9.0/releng_tool.egg-info/
+-rw-rw-rw-   0        0        0     3446 2021-10-02 23:25:45.000000 releng-tool-0.9.0/releng_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18422 2021-10-02 23:25:45.000000 releng-tool-0.9.0/releng_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-10-02 23:25:45.000000 releng-tool-0.9.0/releng_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2021-10-02 23:25:45.000000 releng-tool-0.9.0/releng_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2021-10-02 23:25:45.000000 releng-tool-0.9.0/releng_tool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2021-10-02 23:25:45.000000 releng-tool-0.9.0/releng_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2021-10-02 23:25:45.000000 releng-tool-0.9.0/releng_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.967229 releng-tool-0.9.0/scripts/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.091246 releng-tool-0.9.0/scripts/completion/
+-rw-rw-rw-   0        0        0     2866 2021-08-30 02:55:47.000000 releng-tool-0.9.0/scripts/completion/bash
+-rw-rw-rw-   0        0        0     4040 2021-08-30 02:55:47.000000 releng-tool-0.9.0/scripts/completion/fish
+-rw-rw-rw-   0        0        0     1093 2021-08-30 02:55:47.000000 releng-tool-0.9.0/scripts/completion/zsh
+-rw-rw-rw-   0        0        0      334 2021-10-02 23:25:46.420380 releng-tool-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2170 2021-10-02 23:23:44.000000 releng-tool-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.092222 releng-tool-0.9.0/tests/
+-rw-rw-rw-   0        0        0     7002 2021-08-30 02:55:47.000000 releng-tool-0.9.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4136 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/__main__.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.094174 releng-tool-0.9.0/tests/support/
+-rw-rw-rw-   0        0        0      403 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/support/__init__.py
+-rw-rw-rw-   0        0        0     2167 2021-09-29 01:59:44.000000 releng-tool-0.9.0/tests/support/pkg_config_test.py
+-rw-rw-rw-   0        0        0     6227 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/support/site_tool_test.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.976019 releng-tool-0.9.0/tests/templates/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.095156 releng-tool-0.9.0/tests/templates/cyclic/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.969181 releng-tool-0.9.0/tests/templates/cyclic/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.097105 releng-tool-0.9.0/tests/templates/cyclic/package/test-a/
+-rw-rw-rw-   0        0        0      106 2021-09-29 01:49:04.000000 releng-tool-0.9.0/tests/templates/cyclic/package/test-a/test-a
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.098080 releng-tool-0.9.0/tests/templates/cyclic/package/test-b/
+-rw-rw-rw-   0        0        0      106 2021-09-29 01:49:11.000000 releng-tool-0.9.0/tests/templates/cyclic/package/test-b/test-b
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.098080 releng-tool-0.9.0/tests/templates/cyclic/package/test-c/
+-rw-rw-rw-   0        0        0      106 2021-09-29 01:49:17.000000 releng-tool-0.9.0/tests/templates/cyclic/package/test-c/test-c
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.099056 releng-tool-0.9.0/tests/templates/cyclic/package/test-d/
+-rw-rw-rw-   0        0        0      106 2021-09-29 01:58:34.000000 releng-tool-0.9.0/tests/templates/cyclic/package/test-d/test-d
+-rw-rw-rw-   0        0        0      112 2021-08-07 15:39:00.000000 releng-tool-0.9.0/tests/templates/cyclic/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.100034 releng-tool-0.9.0/tests/templates/licenses/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.970157 releng-tool-0.9.0/tests/templates/licenses/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.102964 releng-tool-0.9.0/tests/templates/licenses/package/test-a/
+-rw-rw-rw-   0        0        0       19 2021-08-07 15:39:00.000000 releng-tool-0.9.0/tests/templates/licenses/package/test-a/COPYING.bsd
+-rw-rw-rw-   0        0        0       19 2021-08-07 15:39:00.000000 releng-tool-0.9.0/tests/templates/licenses/package/test-a/COPYING.mit
+-rw-rw-rw-   0        0        0      189 2021-08-07 15:39:00.000000 releng-tool-0.9.0/tests/templates/licenses/package/test-a/test-a
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.103939 releng-tool-0.9.0/tests/templates/licenses/package/test-b/
+-rw-rw-rw-   0        0        0       74 2021-08-07 15:39:00.000000 releng-tool-0.9.0/tests/templates/licenses/package/test-b/test-b
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.104916 releng-tool-0.9.0/tests/templates/licenses/package/test-c/
+-rw-rw-rw-   0        0        0       19 2021-08-07 15:39:00.000000 releng-tool-0.9.0/tests/templates/licenses/package/test-c/LICENSE
+-rw-rw-rw-   0        0        0      161 2021-08-07 15:39:00.000000 releng-tool-0.9.0/tests/templates/licenses/package/test-c/test-c
+-rw-rw-rw-   0        0        0      112 2021-08-07 15:39:00.000000 releng-tool-0.9.0/tests/templates/licenses/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.105892 releng-tool-0.9.0/tests/templates/minimal/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.970157 releng-tool-0.9.0/tests/templates/minimal/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.106869 releng-tool-0.9.0/tests/templates/minimal/package/minimal/
+-rw-rw-rw-   0        0        0       76 2020-09-13 21:48:20.000000 releng-tool-0.9.0/tests/templates/minimal/package/minimal/minimal
+-rw-rw-rw-   0        0        0       83 2021-01-06 22:29:46.000000 releng-tool-0.9.0/tests/templates/minimal/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.107845 releng-tool-0.9.0/tests/templates/no-packages/
+-rw-rw-rw-   0        0        0       67 2021-01-06 22:29:36.000000 releng-tool-0.9.0/tests/templates/no-packages/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.108822 releng-tool-0.9.0/tests/templates/remote-cfg/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.973088 releng-tool-0.9.0/tests/templates/remote-cfg/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.117611 releng-tool-0.9.0/tests/templates/remote-cfg/package/test/
+-rw-rw-rw-   0        0        0       71 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg/package/test/.releng-tool
+-rw-rw-rw-   0        0        0       97 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg/package/test/test
+-rw-rw-rw-   0        0        0      141 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg/package/test/test-bootstrap
+-rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.109799 releng-tool-0.9.0/tests/templates/remote-cfg-disabled/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.972110 releng-tool-0.9.0/tests/templates/remote-cfg-disabled/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.111750 releng-tool-0.9.0/tests/templates/remote-cfg-disabled/package/test/
+-rw-rw-rw-   0        0        0       71 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg-disabled/package/test/.releng-tool
+-rw-rw-rw-   0        0        0      129 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg-disabled/package/test/test
+-rw-rw-rw-   0        0        0      141 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg-disabled/package/test/test-bootstrap
+-rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg-disabled/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.112733 releng-tool-0.9.0/tests/templates/remote-cfg-override/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.973088 releng-tool-0.9.0/tests/templates/remote-cfg-override/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.114683 releng-tool-0.9.0/tests/templates/remote-cfg-override/package/test/
+-rw-rw-rw-   0        0        0       71 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg-override/package/test/.releng-tool
+-rw-rw-rw-   0        0        0      118 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg-override/package/test/test
+-rw-rw-rw-   0        0        0      141 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg-override/package/test/test-bootstrap
+-rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-cfg-override/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.118587 releng-tool-0.9.0/tests/templates/remote-scripts/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.976019 releng-tool-0.9.0/tests/templates/remote-scripts/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.140069 releng-tool-0.9.0/tests/templates/remote-scripts/package/test/
+-rw-rw-rw-   0        0        0      128 2021-08-07 18:25:39.000000 releng-tool-0.9.0/tests/templates/remote-scripts/package/test/releng-build
+-rw-rw-rw-   0        0        0      132 2021-08-07 18:25:41.000000 releng-tool-0.9.0/tests/templates/remote-scripts/package/test/releng-configure
+-rw-rw-rw-   0        0        0      130 2021-08-07 18:25:36.000000 releng-tool-0.9.0/tests/templates/remote-scripts/package/test/releng-install
+-rw-rw-rw-   0        0        0       97 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-scripts/package/test/test
+-rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-scripts/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.119563 releng-tool-0.9.0/tests/templates/remote-scripts-disabled/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.974070 releng-tool-0.9.0/tests/templates/remote-scripts-disabled/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.122494 releng-tool-0.9.0/tests/templates/remote-scripts-disabled/package/test/
+-rw-rw-rw-   0        0        0      128 2021-08-07 18:25:39.000000 releng-tool-0.9.0/tests/templates/remote-scripts-disabled/package/test/releng-build
+-rw-rw-rw-   0        0        0      132 2021-08-07 18:25:41.000000 releng-tool-0.9.0/tests/templates/remote-scripts-disabled/package/test/releng-configure
+-rw-rw-rw-   0        0        0      130 2021-08-07 18:25:36.000000 releng-tool-0.9.0/tests/templates/remote-scripts-disabled/package/test/releng-install
+-rw-rw-rw-   0        0        0      130 2021-08-07 18:27:48.000000 releng-tool-0.9.0/tests/templates/remote-scripts-disabled/package/test/test
+-rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-scripts-disabled/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.123475 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.975041 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.131282 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/test/
+-rw-rw-rw-   0        0        0      128 2021-08-07 18:25:39.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/test/releng-build
+-rw-rw-rw-   0        0        0      132 2021-08-07 18:25:41.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/test/releng-configure
+-rw-rw-rw-   0        0        0      130 2021-08-07 18:25:36.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/test/releng-install
+-rw-rw-rw-   0        0        0       97 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/test/test
+-rw-rw-rw-   0        0        0      130 2021-08-07 18:26:47.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/test/test-build
+-rw-rw-rw-   0        0        0      134 2021-08-07 18:26:45.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/test/test-configure
+-rw-rw-rw-   0        0        0      132 2021-08-07 18:26:42.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/package/test/test-install
+-rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-all/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.132259 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.976019 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.136161 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/package/test/
+-rw-rw-rw-   0        0        0      128 2021-08-07 18:25:39.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/package/test/releng-build
+-rw-rw-rw-   0        0        0      132 2021-08-07 18:25:41.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/package/test/releng-configure
+-rw-rw-rw-   0        0        0      130 2021-08-07 18:25:36.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/package/test/releng-install
+-rw-rw-rw-   0        0        0       97 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/package/test/test
+-rw-rw-rw-   0        0        0      132 2021-08-07 18:26:42.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/package/test/test-install
+-rw-rw-rw-   0        0        0       80 2021-08-07 17:18:11.000000 releng-tool-0.9.0/tests/templates/remote-scripts-override-subset/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.141045 releng-tool-0.9.0/tests/templates/site-tool/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.976995 releng-tool-0.9.0/tests/templates/site-tool/package/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.142024 releng-tool-0.9.0/tests/templates/site-tool/package/test/
+-rw-rw-rw-   0        0        0       90 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/templates/site-tool/package/test/test
+-rw-rw-rw-   0        0        0       80 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/templates/site-tool/releng
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.143001 releng-tool-0.9.0/tests/tool-tests/
+-rw-rw-rw-   0        0        0       25 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/tool-tests/__init__.py
+-rw-rw-rw-   0        0        0    19267 2021-10-02 17:19:48.000000 releng-tool-0.9.0/tests/tool-tests/test_tool_git.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.165460 releng-tool-0.9.0/tests/unit-tests/
+-rw-rw-rw-   0        0        0       25 2021-01-02 21:11:50.000000 releng-tool-0.9.0/tests/unit-tests/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:45.978947 releng-tool-0.9.0/tests/unit-tests/assets/
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.385227 releng-tool-0.9.0/tests/unit-tests/assets/configs/
+-rw-rw-rw-   0        0        0       59 2021-04-17 19:47:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/autotools-autoreconf-disabled
+-rw-rw-rw-   0        0        0       58 2021-04-17 19:41:30.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/autotools-autoreconf-enabled
+-rw-rw-rw-   0        0        0       63 2021-04-17 19:42:09.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/autotools-autoreconf-invalid
+-rw-rw-rw-   0        0        0       53 2021-04-17 20:43:49.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-defs-invalid-base-type
+-rw-rw-rw-   0        0        0       67 2021-04-17 21:20:10.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-defs-invalid-key-type
+-rw-rw-rw-   0        0        0      108 2021-04-17 20:47:36.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-defs-invalid-strs
+-rw-rw-rw-   0        0        0       68 2021-04-17 20:44:03.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-defs-invalid-value-type
+-rw-rw-rw-   0        0        0      109 2021-04-17 21:06:40.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-defs-valid
+-rw-rw-rw-   0        0        0       52 2021-04-17 20:54:04.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-env-invalid-base-type
+-rw-rw-rw-   0        0        0       66 2021-04-17 21:20:08.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-env-invalid-key-type
+-rw-rw-rw-   0        0        0      107 2021-04-17 20:54:03.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-env-invalid-strs
+-rw-rw-rw-   0        0        0       67 2021-04-17 20:54:01.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-env-invalid-value-type
+-rw-rw-rw-   0        0        0      108 2021-04-17 21:06:43.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-env-valid
+-rw-rw-rw-   0        0        0       49 2021-04-17 21:25:39.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-opts-invalid-base-type
+-rw-rw-rw-   0        0        0       68 2021-04-17 21:09:56.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-opts-invalid-key-type
+-rw-rw-rw-   0        0        0       68 2021-04-17 21:09:54.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-opts-invalid-value-type
+-rw-rw-rw-   0        0        0      109 2021-04-17 21:09:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-opts-valid-dict
+-rw-rw-rw-   0        0        0       52 2021-04-17 21:26:32.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-opts-valid-str
+-rw-rw-rw-   0        0        0       96 2021-04-17 21:09:50.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/build-opts-valid-strs
+-rw-rw-rw-   0        0        0       52 2021-04-17 20:46:30.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-defs-invalid-base-type
+-rw-rw-rw-   0        0        0       66 2021-04-17 21:20:05.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-defs-invalid-key-type
+-rw-rw-rw-   0        0        0      107 2021-04-17 20:47:24.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-defs-invalid-strs
+-rw-rw-rw-   0        0        0       67 2021-04-17 20:46:25.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-defs-invalid-value-type
+-rw-rw-rw-   0        0        0      108 2021-04-17 21:06:44.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-defs-valid
+-rw-rw-rw-   0        0        0       51 2021-04-17 20:53:59.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-env-invalid-base-type
+-rw-rw-rw-   0        0        0       65 2021-04-17 21:20:03.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-env-invalid-key-type
+-rw-rw-rw-   0        0        0      106 2021-04-17 20:53:57.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-env-invalid-strs
+-rw-rw-rw-   0        0        0       66 2021-04-17 20:53:56.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-env-invalid-value-type
+-rw-rw-rw-   0        0        0      107 2021-04-17 21:06:46.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-env-valid
+-rw-rw-rw-   0        0        0       48 2021-04-17 21:25:38.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-opts-invalid-base-type
+-rw-rw-rw-   0        0        0       67 2021-04-17 21:10:22.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-opts-invalid-key-type
+-rw-rw-rw-   0        0        0       67 2021-04-17 21:10:18.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-opts-invalid-value-type
+-rw-rw-rw-   0        0        0      108 2021-04-17 21:10:13.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-opts-valid-dict
+-rw-rw-rw-   0        0        0       51 2021-04-17 21:26:28.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-opts-valid-str
+-rw-rw-rw-   0        0        0       95 2021-04-17 21:10:25.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/conf-opts-valid-strs
+-rw-rw-rw-   0        0        0       49 2021-04-17 21:45:35.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/deps-invalid-type
+-rw-rw-rw-   0        0        0       74 2021-04-17 21:43:34.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/deps-invalid-value
+-rw-rw-rw-   0        0        0       48 2021-04-17 21:43:58.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/deps-valid-empty
+-rw-rw-rw-   0        0        0       89 2021-04-17 21:43:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/deps-valid-multiple
+-rw-rw-rw-   0        0        0       51 2021-04-17 21:46:07.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/deps-valid-single
+-rw-rw-rw-   0        0        0       59 2021-04-17 19:53:08.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/devmode-ignore-cache-disabled
+-rw-rw-rw-   0        0        0       58 2021-04-17 19:53:07.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/devmode-ignore-cache-enabled
+-rw-rw-rw-   0        0        0       63 2021-04-17 19:53:05.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/devmode-ignore-cache-invalid
+-rw-rw-rw-   0        0        0       53 2021-04-18 21:54:06.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/devmode-revision-invalid-type
+-rw-rw-rw-   0        0        0       71 2021-04-18 21:54:23.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/devmode-revision-valid
+-rw-rw-rw-   0        0        0       42 2021-04-18 00:15:42.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/ext-mods-invalid-type
+-rw-rw-rw-   0        0        0      130 2021-04-18 00:20:30.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/ext-mods-valid-data
+-rw-rw-rw-   0        0        0       42 2021-04-18 00:20:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/ext-mods-valid-empty
+-rw-rw-rw-   0        0        0       47 2021-04-18 03:22:59.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/external-flag-disabled
+-rw-rw-rw-   0        0        0       46 2021-04-18 03:23:05.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/external-flag-enabled
+-rw-rw-rw-   0        0        0       51 2021-04-18 03:23:02.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/external-flag-invalid
+-rw-rw-rw-   0        0        0       49 2021-04-18 22:02:22.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/extract-type-invalid-type
+-rw-rw-rw-   0        0        0       74 2021-04-18 22:09:33.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/extract-type-valid
+-rw-rw-rw-   0        0        0       53 2021-04-17 19:55:28.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/fixed-jobs-invalid-type
+-rw-rw-rw-   0        0        0       45 2021-04-17 19:58:05.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/fixed-jobs-invalid-value
+-rw-rw-rw-   0        0        0       46 2021-04-17 19:55:35.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/fixed-jobs-valid
+-rw-rw-rw-   0        0        0       53 2021-04-18 20:08:42.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-config-invalid-base-type
+-rw-rw-rw-   0        0        0       67 2021-04-18 20:08:40.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-config-invalid-key-type
+-rw-rw-rw-   0        0        0      108 2021-04-18 20:09:23.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-config-invalid-strs
+-rw-rw-rw-   0        0        0       68 2021-04-18 20:08:37.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-config-invalid-value-type
+-rw-rw-rw-   0        0        0      109 2021-04-18 20:08:44.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-config-valid
+-rw-rw-rw-   0        0        0       52 2021-04-18 13:46:32.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-depth-invalid-type
+-rw-rw-rw-   0        0        0       45 2021-04-18 13:46:34.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-depth-invalid-value
+-rw-rw-rw-   0        0        0       45 2021-04-18 13:46:37.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-depth-valid-nonzero
+-rw-rw-rw-   0        0        0       44 2021-04-18 13:46:35.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-depth-valid-zero
+-rw-rw-rw-   0        0        0       49 2021-04-18 20:02:50.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-refspecs-invalid-type
+-rw-rw-rw-   0        0        0       76 2021-04-18 20:03:36.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-refspecs-invalid-value
+-rw-rw-rw-   0        0        0       48 2021-04-18 20:02:58.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-refspecs-valid-empty
+-rw-rw-rw-   0        0        0      101 2021-04-18 20:03:34.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-refspecs-valid-multiple
+-rw-rw-rw-   0        0        0       55 2021-04-18 20:03:27.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-refspecs-valid-single
+-rw-rw-rw-   0        0        0       51 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-submodules-disabled
+-rw-rw-rw-   0        0        0       50 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-submodules-enabled
+-rw-rw-rw-   0        0        0       55 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-submodules-invalid
+-rw-rw-rw-   0        0        0       56 2021-08-30 11:01:07.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-verify-disabled
+-rw-rw-rw-   0        0        0       55 2021-08-30 11:01:05.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-verify-enabled
+-rw-rw-rw-   0        0        0       60 2021-08-30 11:01:03.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/git-verify-invalid
+-rw-rw-rw-   0        0        0       55 2021-04-17 20:46:07.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-defs-invalid-base-type
+-rw-rw-rw-   0        0        0       69 2021-04-17 21:20:00.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-defs-invalid-key-type
+-rw-rw-rw-   0        0        0      110 2021-04-17 20:47:14.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-defs-invalid-strs
+-rw-rw-rw-   0        0        0       70 2021-04-17 20:46:04.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-defs-invalid-value-type
+-rw-rw-rw-   0        0        0      111 2021-04-17 21:06:50.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-defs-valid
+-rw-rw-rw-   0        0        0       54 2021-04-17 20:54:12.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-env-invalid-base-type
+-rw-rw-rw-   0        0        0       68 2021-04-17 21:19:58.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-env-invalid-key-type
+-rw-rw-rw-   0        0        0      109 2021-04-17 20:54:10.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-env-invalid-strs
+-rw-rw-rw-   0        0        0       69 2021-04-17 20:54:08.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-env-invalid-value-type
+-rw-rw-rw-   0        0        0      110 2021-04-17 21:06:52.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-env-valid
+-rw-rw-rw-   0        0        0       51 2021-04-17 21:25:35.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-opts-invalid-base-type
+-rw-rw-rw-   0        0        0       70 2021-04-17 20:59:40.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-opts-invalid-key-type
+-rw-rw-rw-   0        0        0       70 2021-04-17 20:58:22.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-opts-invalid-value-type
+-rw-rw-rw-   0        0        0      111 2021-04-17 21:07:03.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-opts-valid-dict
+-rw-rw-rw-   0        0        0       54 2021-04-17 21:26:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-opts-valid-str
+-rw-rw-rw-   0        0        0       98 2021-04-17 21:00:32.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-opts-valid-strs
+-rw-rw-rw-   0        0        0       51 2021-04-18 02:08:44.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-type-invalid-type
+-rw-rw-rw-   0        0        0       55 2021-04-18 02:08:46.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-type-invalid-value
+-rw-rw-rw-   0        0        0       52 2021-04-18 01:41:21.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-type-valid-host
+-rw-rw-rw-   0        0        0       54 2021-04-18 01:41:18.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-type-valid-images
+-rw-rw-rw-   0        0        0       55 2021-04-18 01:55:11.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-type-valid-staging
+-rw-rw-rw-   0        0        0       66 2021-04-18 01:41:36.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-type-valid-staging-target
+-rw-rw-rw-   0        0        0       54 2021-04-18 01:41:29.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/install-type-valid-target
+-rw-rw-rw-   0        0        0       68 2021-04-18 03:24:03.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/internal-external-flag-conflict1
+-rw-rw-rw-   0        0        0       70 2021-04-18 03:23:49.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/internal-external-flag-conflict2
+-rw-rw-rw-   0        0        0       69 2021-04-18 03:55:16.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/internal-external-flag-disabled
+-rw-rw-rw-   0        0        0       69 2021-04-18 03:55:13.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/internal-external-flag-enabled
+-rw-rw-rw-   0        0        0       47 2021-04-18 03:22:02.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/internal-flag-disabled
+-rw-rw-rw-   0        0        0       46 2021-04-18 03:22:05.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/internal-flag-enabled
+-rw-rw-rw-   0        0        0       51 2021-04-18 03:22:07.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/internal-flag-invalid
+-rw-rw-rw-   0        0        0       50 2021-04-18 19:45:07.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-files-invalid-type
+-rw-rw-rw-   0        0        0       82 2021-04-18 19:46:13.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-files-invalid-value
+-rw-rw-rw-   0        0        0       49 2021-04-18 19:45:03.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-files-valid-empty
+-rw-rw-rw-   0        0        0      117 2021-04-18 19:45:57.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-files-valid-multiple
+-rw-rw-rw-   0        0        0       61 2021-04-18 19:46:05.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-files-valid-single
+-rw-rw-rw-   0        0        0       44 2021-04-18 19:45:29.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-invalid-type
+-rw-rw-rw-   0        0        0       71 2021-04-18 19:45:40.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-invalid-value
+-rw-rw-rw-   0        0        0       43 2021-04-18 19:45:25.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-valid-empty
+-rw-rw-rw-   0        0        0       96 2021-04-18 19:45:45.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-valid-multiple
+-rw-rw-rw-   0        0        0       50 2021-04-18 19:46:40.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/license-valid-single
+-rw-rw-rw-   0        0        0       24 2021-04-17 19:47:07.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/missing
+-rw-rw-rw-   0        0        0       52 2021-04-18 03:21:39.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/no-extraction-disabled
+-rw-rw-rw-   0        0        0       51 2021-04-18 03:21:42.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/no-extraction-enabled
+-rw-rw-rw-   0        0        0       56 2021-04-18 03:21:44.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/no-extraction-invalid
+-rw-rw-rw-   0        0        0       50 2021-04-18 19:14:33.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/pkg-type-invalid-type
+-rw-rw-rw-   0        0        0       47 2021-04-18 19:14:31.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/pkg-type-invalid-value
+-rw-rw-rw-   0        0        0       49 2021-04-18 19:14:38.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/pkg-type-valid-autotools
+-rw-rw-rw-   0        0        0       45 2021-04-18 19:15:18.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/pkg-type-valid-cmake
+-rw-rw-rw-   0        0        0       46 2021-04-18 19:15:11.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/pkg-type-valid-python
+-rw-rw-rw-   0        0        0       46 2021-04-18 19:15:06.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/pkg-type-valid-script
+-rw-rw-rw-   0        0        0       43 2021-04-18 19:31:24.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/prefix-invalid-type
+-rw-rw-rw-   0        0        0       50 2021-04-18 19:31:29.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/prefix-valid
+-rw-rw-rw-   0        0        0       55 2021-04-18 19:24:34.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/python-interpreter-invalid-type
+-rw-rw-rw-   0        0        0       62 2021-04-18 19:24:46.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/python-interpreter-valid
+-rw-rw-rw-   0        0        0       45 2021-04-18 19:29:51.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/revision-invalid-type
+-rw-rw-rw-   0        0        0       54 2021-04-18 19:30:19.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/revision-valid-explicit
+-rw-rw-rw-   0        0        0       28 2021-04-18 19:30:27.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/revision-valid-implicit
+-rw-rw-rw-   0        0        0       43 2021-04-18 19:20:49.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/site-invalid-type
+-rw-rw-rw-   0        0        0       68 2021-04-18 19:21:21.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/site-valid
+-rw-rw-rw-   0        0        0       57 2021-08-07 15:30:54.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/skip-remote-config-disabled
+-rw-rw-rw-   0        0        0       56 2021-08-07 15:30:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/skip-remote-config-enabled
+-rw-rw-rw-   0        0        0       61 2021-08-07 15:30:48.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/skip-remote-config-invalid
+-rw-rw-rw-   0        0        0       58 2021-08-07 17:49:23.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/skip-remote-scripts-disabled
+-rw-rw-rw-   0        0        0       57 2021-08-07 17:49:22.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/skip-remote-scripts-enabled
+-rw-rw-rw-   0        0        0       62 2021-08-07 17:49:18.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/skip-remote-scripts-invalid
+-rw-rw-rw-   0        0        0       54 2021-04-18 13:47:03.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/strip-count-invalid-type
+-rw-rw-rw-   0        0        0       47 2021-04-18 13:47:02.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/strip-count-invalid-value
+-rw-rw-rw-   0        0        0       46 2021-04-18 13:47:05.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/strip-count-valid-nonzero
+-rw-rw-rw-   0        0        0       46 2021-04-18 13:47:00.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/strip-count-valid-zero
+-rw-rw-rw-   0        0        0       47 2021-04-18 14:41:23.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-bzr-nosite
+-rw-rw-rw-   0        0        0       47 2021-04-18 14:43:00.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-cvs-nosite
+-rw-rw-rw-   0        0        0       47 2021-04-18 14:43:04.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-git-nosite
+-rw-rw-rw-   0        0        0       46 2021-04-18 14:42:36.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-hg-nosite
+-rw-rw-rw-   0        0        0       47 2021-04-18 14:42:47.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-scp-nosite
+-rw-rw-rw-   0        0        0       47 2021-04-18 14:42:51.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-svn-nosite
+-rw-rw-rw-   0        0        0       54 2021-04-18 14:13:56.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-type
+-rw-rw-rw-   0        0        0       47 2021-04-18 14:42:55.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-url-nosite
+-rw-rw-rw-   0        0        0       51 2021-04-18 14:12:40.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-invalid-value
+-rw-rw-rw-   0        0        0       68 2021-04-18 14:40:13.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-bzr-explicit
+-rw-rw-rw-   0        0        0       51 2021-04-18 14:23:11.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-bzr-implicit
+-rw-rw-rw-   0        0        0       68 2021-04-18 14:40:15.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-explicit
+-rw-rw-rw-   0        0        0       51 2021-04-18 14:23:18.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit
+-rw-rw-rw-   0        0        0       98 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit2
+-rw-rw-rw-   0        0        0       90 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit3
+-rw-rw-rw-   0        0        0       93 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit4
+-rw-rw-rw-   0        0        0       94 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit5
+-rw-rw-rw-   0        0        0       94 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-cvs-implicit6
+-rw-rw-rw-   0        0        0       68 2021-04-18 14:40:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-git-explicit
+-rw-rw-rw-   0        0        0       51 2021-04-18 14:23:42.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-git-implicit1
+-rw-rw-rw-   0        0        0       51 2021-04-18 14:23:49.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-git-implicit2
+-rw-rw-rw-   0        0        0       67 2021-04-18 14:40:18.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-hg-explicit
+-rw-rw-rw-   0        0        0       50 2021-04-18 14:23:59.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-hg-implicit
+-rw-rw-rw-   0        0        0       49 2021-04-18 14:19:45.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-local-explicit
+-rw-rw-rw-   0        0        0       45 2021-04-18 14:24:52.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-local-implicit
+-rw-rw-rw-   0        0        0       48 2021-04-18 14:19:42.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-none-explicit
+-rw-rw-rw-   0        0        0       24 2021-04-18 14:25:18.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-none-implicit
+-rw-rw-rw-   0        0        0       68 2021-04-18 14:40:19.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-scp-explicit
+-rw-rw-rw-   0        0        0       51 2021-04-18 14:24:21.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-scp-implicit
+-rw-rw-rw-   0        0        0       68 2021-04-18 14:40:20.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-svn-explicit
+-rw-rw-rw-   0        0        0       51 2021-04-18 14:24:31.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-svn-implicit
+-rw-rw-rw-   0        0        0       68 2021-04-18 14:40:22.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-url-explicit
+-rw-rw-rw-   0        0        0       51 2021-04-18 14:23:01.000000 releng-tool-0.9.0/tests/unit-tests/assets/configs/vcs-type-valid-url-implicit
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.388158 releng-tool-0.9.0/tests/unit-tests/assets/copy-check-01/
+-rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/copy-check-01/test-file-a
+-rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/copy-check-01/test-file-b
+-rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/copy-check-01/test-file-x
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.390112 releng-tool-0.9.0/tests/unit-tests/assets/copy-check-02/
+-rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/copy-check-02/test-file-b
+-rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/copy-check-02/test-file-c
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.405735 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/
+-rw-rw-rw-   0        0        0       78 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/invalid-hash-sample-a
+-rw-rw-rw-   0        0        0       80 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/invalid-hash-sample-b
+-rw-rw-rw-   0        0        0       94 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/invalid-hash-sample-c
+-rw-rw-rw-   0        0        0       72 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/sample-asset
+-rw-rw-rw-   0        0        0       15 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-a
+-rw-rw-rw-   0        0        0      322 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-b
+-rw-rw-rw-   0        0        0      539 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-c
+-rw-rw-rw-   0        0        0       39 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-d
+-rw-rw-rw-   0        0        0      107 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/verify-bad-format
+-rw-rw-rw-   0        0        0      122 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/verify-bad-hash
+-rw-rw-rw-   0        0        0       31 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/verify-empty
+-rw-rw-rw-   0        0        0      161 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/verify-missing-archive
+-rw-rw-rw-   0        0        0      163 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/verify-missing-listed
+-rw-rw-rw-   0        0        0      612 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/verify-success
+-rw-rw-rw-   0        0        0       84 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/verify-unknown-hash-type
+drwxrwxrwx   0        0        0        0 2021-10-02 23:25:46.412570 releng-tool-0.9.0/tests/unit-tests/assets/shebang-interpreter/
+-rw-rw-rw-   0        0        0       40 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/shebang-interpreter/example.py
+-rw-rw-rw-   0        0        0       48 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/shebang-interpreter/interpreter
+-rw-rw-rw-   0        0        0       55 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/shebang-interpreter/interpreter-arg
+-rw-rw-rw-   0        0        0      102 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/shebang-interpreter/interpreter-args-multiple
+-rw-rw-rw-   0        0        0     5084 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/shebang-interpreter/interpreter-extremely-long
+-rw-rw-rw-   0        0        0      161 2020-09-13 21:08:17.000000 releng-tool-0.9.0/tests/unit-tests/assets/shebang-interpreter/interpreter-whitespaces
+-rw-rw-rw-   0        0        0     1139 2021-08-08 16:59:05.000000 releng-tool-0.9.0/tests/unit-tests/test_engine_run_actions.py
+-rw-rw-rw-   0        0        0     1389 2021-08-07 15:31:28.000000 releng-tool-0.9.0/tests/unit-tests/test_engine_run_defaults.py
+-rw-rw-rw-   0        0        0      758 2021-04-10 04:22:56.000000 releng-tool-0.9.0/tests/unit-tests/test_engine_run_file_flags.py
+-rw-rw-rw-   0        0        0     1938 2021-08-31 03:57:26.000000 releng-tool-0.9.0/tests/unit-tests/test_file_flags.py
+-rw-rw-rw-   0        0        0    11471 2021-09-29 01:59:53.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs.py
+-rw-rw-rw-   0        0        0      945 2021-04-18 18:21:15.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_autotools.py
+-rw-rw-rw-   0        0        0     1201 2021-09-29 02:03:40.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_cyclic.py
+-rw-rw-rw-   0        0        0     2257 2021-04-18 21:58:00.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_devmode.py
+-rw-rw-rw-   0        0        0     2372 2021-08-08 15:36:26.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_extensions.py
+-rw-rw-rw-   0        0        0     4361 2021-08-30 11:00:43.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_git.py
+-rw-rw-rw-   0        0        0    12236 2021-04-18 18:23:41.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_stageopts.py
+-rw-rw-rw-   0        0        0     1495 2021-04-18 19:16:31.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_type.py
+-rw-rw-rw-   0        0        0     5993 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_vcs_type.py
+-rw-rw-rw-   0        0        0     2173 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_pipeline_licenses.py
+-rw-rw-rw-   0        0        0     1328 2021-08-07 19:10:57.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_pipeline_remote_cfg.py
+-rw-rw-rw-   0        0        0     2596 2021-08-07 19:10:47.000000 releng-tool-0.9.0/tests/unit-tests/test_pkg_pipeline_remote_scripts.py
+-rw-rw-rw-   0        0        0      863 2021-04-17 15:38:34.000000 releng-tool-0.9.0/tests/unit-tests/test_util_common.py
+-rw-rw-rw-   0        0        0     2906 2021-10-01 04:54:39.000000 releng-tool-0.9.0/tests/unit-tests/test_util_env.py
+-rw-rw-rw-   0        0        0     5387 2021-10-01 04:29:18.000000 releng-tool-0.9.0/tests/unit-tests/test_util_hash.py
+-rw-rw-rw-   0        0        0    17072 2021-08-29 02:15:53.000000 releng-tool-0.9.0/tests/unit-tests/test_util_io.py
+-rw-rw-rw-   0        0        0     4541 2020-09-24 04:32:39.000000 releng-tool-0.9.0/tests/unit-tests/test_util_sort.py
+-rw-rw-rw-   0        0        0     3124 2020-09-24 02:54:03.000000 releng-tool-0.9.0/tests/unit-tests/test_util_string.py
```

### Comparing `releng-tool-0.8.0/LICENSE` & `releng-tool-0.9.0/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2018-2019 releng-tool
+Copyright 2018-2021 releng-tool
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `releng-tool-0.8.0/PKG-INFO` & `releng-tool-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: releng-tool
-Version: 0.8.0
+Version: 0.9.0
 Summary: release engineering utility tool
 Home-page: https://releng.io
 Author: releng-tool
 Author-email: releng@releng.io
 License: BSD-2-Clause
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -43,59 +43,64 @@
 .. image:: https://img.shields.io/pypi/dm/releng-tool.svg
     :target: https://pypi.python.org/pypi/releng-tool
     :alt: PyPI download month
 
 releng-tool aims to provide a method to prepare a structured environment to
 assist in the release engineering of a project.
 
-overview
+Overview
 --------
 
 When dealing with the release engineering of a project, assets may be found in
 multiple locations and may require various methods to extract, build and more.
 releng-tool can be used to process a defined set of projects/packages which
 identify where resources can be fetched, how packages can be extracted and
 methods to patch, configure, build and install each individual package for a
 target root.
 
 For detailed documentation on the releng-tool project, please consult the
 `releng-tool documentation`_.
 
-requirements
+Requirements
 ------------
 
 * Python_ 2.7 or 3.4+
 
 Host tools such as Git_, scp, etc. may be required depending on the project
 being processed (e.g. if a package's sources fetch from a Git source, a Git
 client tool is required to perform said fetch).
 
-installation
+Installation
 ------------
 
 This tool can be installed using pip_:
 
 .. code-block:: shell
 
    pip install releng-tool
     (or)
    python -m pip install releng-tool
 
-usage
+For Arch Linux users, this package is also available on AUR:
+
+ | Arch User Repository - releng-tool
+ | https://aur.archlinux.org/packages/releng-tool/
+
+Usage
 -----
 
 This tool can be invoked from a command line using:
 
 .. code-block:: shell
 
    releng-tool --help
     (or)
    python -m releng_tool --help
 
-examples
+Examples
 --------
 
 Examples of releng-tool projects can be found in
 `releng-tool's examples repository`_.
 
 .. _Git: https://git-scm.com/
 .. _Python: https://www.python.org/
```

### Comparing `releng-tool-0.8.0/README.rst` & `releng-tool-0.9.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -16,59 +16,64 @@
 .. image:: https://img.shields.io/pypi/dm/releng-tool.svg
     :target: https://pypi.python.org/pypi/releng-tool
     :alt: PyPI download month
 
 releng-tool aims to provide a method to prepare a structured environment to
 assist in the release engineering of a project.
 
-overview
+Overview
 --------
 
 When dealing with the release engineering of a project, assets may be found in
 multiple locations and may require various methods to extract, build and more.
 releng-tool can be used to process a defined set of projects/packages which
 identify where resources can be fetched, how packages can be extracted and
 methods to patch, configure, build and install each individual package for a
 target root.
 
 For detailed documentation on the releng-tool project, please consult the
 `releng-tool documentation`_.
 
-requirements
+Requirements
 ------------
 
 * Python_ 2.7 or 3.4+
 
 Host tools such as Git_, scp, etc. may be required depending on the project
 being processed (e.g. if a package's sources fetch from a Git source, a Git
 client tool is required to perform said fetch).
 
-installation
+Installation
 ------------
 
 This tool can be installed using pip_:
 
 .. code-block:: shell
 
    pip install releng-tool
     (or)
    python -m pip install releng-tool
 
-usage
+For Arch Linux users, this package is also available on AUR:
+
+ | Arch User Repository - releng-tool
+ | https://aur.archlinux.org/packages/releng-tool/
+
+Usage
 -----
 
 This tool can be invoked from a command line using:
 
 .. code-block:: shell
 
    releng-tool --help
     (or)
    python -m releng_tool --help
 
-examples
+Examples
 --------
 
 Examples of releng-tool projects can be found in
 `releng-tool's examples repository`_.
 
 .. _Git: https://git-scm.com/
 .. _Python: https://www.python.org/
```

### Comparing `releng-tool-0.8.0/releng_tool/__init__.py` & `releng-tool-0.9.0/releng_tool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Copyright 2018-2021 releng-tool
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 # Below should contain a series of helper implementations to assist releng-tool
 # developer's wanting to explicitly import script helpers into scripts not
 # directly invoked by releng-tool. When releng-tool invokes a project's script
 # (whether it be a configuration script, a package stage-specific script (e.g.
 # a package's build script), etc.), a series of utility functions will be made
 # available with a pre-populated globals module. If a project defines their own
```

### Comparing `releng-tool-0.8.0/releng_tool/__main__.py` & `releng-tool-0.9.0/releng_tool/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
 (mode options)
  -D, --development         enable development mode
  --local-sources           use development sources from a local path
 
 (other)
  --debug                   show debug-related messages
  -h, --help                show this help
+ --help-quirks             show available quirks
  --nocolorout              explicitly disable colorized output
  --quirk <value>           inject in quirk into this run
  -V, --verbose             show additional messages
  --version                 show the version
 """
 
 def usage_quirks():
```

### Comparing `releng-tool-0.8.0/releng_tool/api/__init__.py` & `releng-tool-0.9.0/releng_tool/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         revision: revision to use to fetch from source control
         site: the site (uri) to acquire a package's resources
     """
     def __init__(self):
         super(RelengFetchOptions, self).__init__()
         self.cache_dir = None
         self.cache_file = None
-        self.ignore_cache = False
+        self.ignore_cache = None
         self.revision = None
         self.site = None
 
 class RelengInstallOptions(RelengPackageOptions):
     """
     releng install-type options
```

### Comparing `releng-tool-0.8.0/releng_tool/defs.py` & `releng-tool-0.9.0/releng_tool/defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 RPK_EXTOPT = 'EXTOPT' #: extension-defined package modifiers (if any)
 RPK_EXTRACT_TYPE = 'EXTRACT_TYPE' #: extraction type for sources
 RPK_FIXED_JOBS = 'FIXED_JOBS' #: fixed job count for the project
 RPK_GIT_CONFIG = 'GIT_CONFIG' #: git configurations to set (if any)
 RPK_GIT_DEPTH = 'GIT_DEPTH' #: git fetch depth (if any)
 RPK_GIT_REFSPECS = 'GIT_REFSPECS' #: additional git refspecs to fetch (if any)
 RPK_GIT_SUBMODULES = 'GIT_SUBMODULES' #: fetch any submodules (if any)
+RPK_GIT_VERIFY_REVISION = 'GIT_VERIFY_REVISION' #: verify signed revisions
 RPK_INSTALL_TYPE = 'INSTALL_TYPE' #: install container target for the package
 RPK_INTERNAL = 'INTERNAL' #: whether or not package is considered "internal"
 RPK_LICENSE = 'LICENSE' #: license information for the package
 RPK_LICENSE_FILES = 'LICENSE_FILES' #: source file(s) with license information
 RPK_NO_EXTRACTION = 'NO_EXTRACTION' #: whether or not package extraction is done
 RPK_PREFIX = 'PREFIX' #: system root prefix override (if needed)
 RPK_REVISION = 'REVISION' #: revision to acquire from sources (if any)
```

### Comparing `releng-tool-0.8.0/releng_tool/engine/__init__.py` & `releng-tool-0.9.0/releng_tool/engine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 from releng_tool.defs import GlobalAction
 from releng_tool.defs import PkgAction
 from releng_tool.defs import VcsType
 from releng_tool.engine.fetch import stage as fetch_stage
 from releng_tool.engine.init import initialize_sample
 from releng_tool.exceptions import RelengToolMissingConfigurationError
 from releng_tool.exceptions import RelengToolMissingPackagesError
+from releng_tool.opts import RELENG_POST_BUILD_NAME
 from releng_tool.packages.exceptions import RelengToolStageFailure
 from releng_tool.packages.manager import RelengPackageManager
 from releng_tool.packages.pipeline import RelengPackagePipeline
 from releng_tool.prerequisites import RelengPrerequisites
 from releng_tool.registry import RelengRegistry
 from releng_tool.stats import RelengStats
-from releng_tool.util.env import extend_script_env
 from releng_tool.util.env import env_value
+from releng_tool.util.env import extend_script_env
 from releng_tool.util.file_flags import FileFlag
 from releng_tool.util.file_flags import check_file_flag
 from releng_tool.util.file_flags import process_file_flag
 from releng_tool.util.io import FailedToPrepareWorkingDirectoryError
 from releng_tool.util.io import ensure_dir_exists
 from releng_tool.util.io import execute
 from releng_tool.util.io import execute_rv
@@ -105,15 +106,15 @@
         self.start_time = datetime.now().replace(microsecond=0)
         verbose("loading user's configuration...")
         gbls = {
             'releng_args': opts.forward_args,
             'releng_version': releng_version,
         }
 
-        verbose('loading statistics...')
+        debug('loading statistics...')
         self.stats.load()
 
         # prepare script environment to make helpers available to configuration
         # script(s)
         self._prepare_script_environment(gbls, gaction, opts.pkg_action)
 
         conf_point, conf_point_exists = opt_file(opts.conf_point)
@@ -213,17 +214,20 @@
             requested_preconfig = pa in [
                 PkgAction.EXTRACT,
                 PkgAction.FETCH,
                 PkgAction.LICENSE,
                 PkgAction.PATCH,
             ]
 
+            # determine if an explicit fetch request has been made
+            requested_fetch = None
+            if gaction == GlobalAction.FETCH or pa == PkgAction.FETCH:
+                requested_fetch = True
+
             # ensure all package sources are acquired first
-            requested_fetch = (
-                gaction == GlobalAction.FETCH or pa == PkgAction.FETCH)
             for pkg in pkgs:
                 if not self._stage_init(pkg):
                     return False
 
                 # if this is a package-specific pre-configure action, only
                 # ensure a fetched this specific package
                 if requested_preconfig and pkg.name != opts.target_action:
@@ -417,16 +421,20 @@
             path_remove(self.opts.dl_dir)
 
         if gaction in (GlobalAction.MRPROPER, GlobalAction.DISTCLEAN):
             verbose('removing output directory')
             path_remove(self.opts.out_dir)
 
             verbose('removing file flags')
-            path_remove(self.opts.ff_local_srcs)
-            path_remove(self.opts.ff_devmode)
+            if os.path.exists(self.opts.ff_devmode):
+                if path_remove(self.opts.ff_devmode):
+                    warn('development mode has been unconfigured')
+            if os.path.exists(self.opts.ff_local_srcs):
+                if path_remove(self.opts.ff_local_srcs):
+                    warn('local-sources mode has been unconfigured')
         else:
             verbose('removing build directory')
             path_remove(self.opts.build_dir)
             verbose('removing host directory')
             path_remove(self.opts.host_dir)
             verbose('removing license directory')
             path_remove(self.opts.license_dir)
@@ -505,36 +513,44 @@
             env: environment settings to apply for processing script
 
         Returns:
             ``True`` if the post-processing script has executed correctly or no
             post-processing script exists; ``False`` if an error has occurred
             when processing the post-processing script
         """
-        script, script_exists = opt_file(self.opts.post_point)
+        build_script, postbuild_exists = opt_file(self.opts.post_build_point)
 
         # TODO remove deprecated configuration load in (at maximum) v1.0
-        if not script_exists:
-            script = os.path.join(self.opts.root_dir, 'post.py')
-            if os.path.isfile(script):
-                warn('using deprecated post-processing file post.py -- switch '
-                     'to releng-post for future projects')
-                script_exists = True
+        if not postbuild_exists:
+            deprecated_posts = [
+                'releng-post',
+                'post.py',
+            ]
+
+            for script_name in deprecated_posts:
+                build_script = os.path.join(self.opts.root_dir, script_name)
+                if os.path.isfile(build_script):
+                    warn('using deprecated post-processing file {} -- switch '
+                         'to {} for future projects', script_name,
+                         RELENG_POST_BUILD_NAME)
+                    postbuild_exists = True
+                    break
 
-        if script_exists:
-            verbose('performing post-processing...')
+        if postbuild_exists:
+            verbose('performing post-processing (build)...')
 
             # ensure images directory exists (as the post-processing script will
             # most likely populate it)
             if not ensure_dir_exists(self.opts.images_dir):
                 return False
 
-            if not run_script(script, env, subject='post-processing'):
+            if not run_script(build_script, env, subject='post-build'):
                 return False
 
-            verbose('post-processing completed')
+            verbose('post-processing (build) completed')
 
         return True
 
     def _prepare_script_environment(self, script_env, gaction, paction):
         """
         prepare the script environment with common project values
```

### Comparing `releng-tool-0.8.0/releng_tool/engine/autotools/build.py` & `releng-tool-0.9.0/releng_tool/engine/autotools/build.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/autotools/configure.py` & `releng-tool-0.9.0/releng_tool/engine/autotools/configure.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/autotools/install.py` & `releng-tool-0.9.0/releng_tool/engine/autotools/install.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/bootstrap.py` & `releng-tool-0.9.0/releng_tool/engine/bootstrap.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/build.py` & `releng-tool-0.9.0/releng_tool/engine/build.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/cmake/build.py` & `releng-tool-0.9.0/releng_tool/engine/cmake/build.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/cmake/configure.py` & `releng-tool-0.9.0/releng_tool/engine/cmake/configure.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/cmake/install.py` & `releng-tool-0.9.0/releng_tool/engine/cmake/install.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/configure.py` & `releng-tool-0.9.0/releng_tool/engine/configure.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/extract.py` & `releng-tool-0.9.0/releng_tool/engine/extract.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/fetch.py` & `releng-tool-0.9.0/releng_tool/engine/fetch.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from releng_tool.fetch.bzr import fetch as fetch_bzr
 from releng_tool.fetch.cvs import fetch as fetch_cvs
 from releng_tool.fetch.git import fetch as fetch_git
 from releng_tool.fetch.mercurial import fetch as fetch_mercurial
 from releng_tool.fetch.scp import fetch as fetch_scp
 from releng_tool.fetch.svn import fetch as fetch_svn
 from releng_tool.fetch.url import fetch as fetch_url
+from releng_tool.tool.gpg import GPG
 from releng_tool.util.api import replicate_package_attribs
 from releng_tool.util.hash import HashResult
 from releng_tool.util.hash import verify as verify_hashes
 from releng_tool.util.io import ensure_dir_exists
 from releng_tool.util.io import generate_temp_dir
 from releng_tool.util.io import interim_working_dir
 from releng_tool.util.io import path_remove
@@ -56,16 +57,18 @@
 local sources option to use the default process).
 
        Package: {}
  Expected Path: {}""".format(name, pkg.build_dir))
         return False
 
     # if the vcs-type is archive-based, flag that hash checks are needed
+    perform_file_asc_check = False
     perform_file_hash_check = False
     if pkg.vcs_type == VcsType.URL:
+        perform_file_asc_check = os.path.exists(pkg.asc_file)
         perform_file_hash_check = True
 
     fetch_opts = RelengFetchOptions()
     replicate_package_attribs(fetch_opts, pkg)
     fetch_opts.cache_dir = pkg.cache_dir
     fetch_opts.ext = pkg.ext_modifiers
     fetch_opts.ignore_cache = ignore_cache
@@ -91,59 +94,82 @@
             # a VCS source will make a cache file from the branch and will
             # remain until manually removed from a cache file. A user may wish
             # to re-build the local cache file after cleaning their project.
             # While the releng-tool framework separates fetching/extraction into
             # two parts, ignoring cached assets can be partially achieved by
             # just removing any detected cache file if a project is configured
             # to ignore a cache file.
-            if engine.opts.devmode and pkg.devmode_ignore_cache:
-                fetch_opts.ignore_cache = True
+            if engine.opts.devmode and pkg.devmode_ignore_cache is not None:
+                fetch_opts.ignore_cache = pkg.devmode_ignore_cache
 
-                if os.path.exists(pkg.cache_file):
+                if pkg.devmode_ignore_cache and os.path.exists(pkg.cache_file):
                     verbose('removing cache file (per configuration): ' + name)
                     if not path_remove(pkg.cache_file):
                         return False
+            # force explicit ignore cache when not in development mode
+            elif not engine.opts.devmode and ignore_cache is None:
+                fetch_opts.ignore_cache = False
 
             if os.path.exists(pkg.cache_file):
                 rv = None
                 if perform_file_hash_check:
                     hr = verify_hashes(
                         pkg.hash_file, pkg.cache_file, relaxed=True)
 
                     if hr == HashResult.VERIFIED:
                         rv = True
                     elif hr == HashResult.BAD_PATH:
-                        if not pkg.is_internal:
+                        if not perform_file_asc_check and not pkg.is_internal:
                             warn('missing hash file for package: ' + name)
                         rv = True # no hash file to compare with; assuming ok
                     elif hr == HashResult.EMPTY:
                         if not pkg.is_internal:
                             warn('hash file for package is empty: ' + name)
                         rv = True # empty hash file; assuming ok
                     elif hr == HashResult.MISMATCH:
                         if not path_remove(pkg.cache_file):
                             rv = False
                     elif hr in (HashResult.BAD_FORMAT, HashResult.UNSUPPORTED):
                         rv = False
                     elif hr == HashResult.MISSING_ARCHIVE:
-                        err('missing archive hash for verification')
-                        err("""\
+                        if not perform_file_asc_check:
+                            err("""\
+missing archive hash for verification
+
 The hash file for this package does not have an entry for the cache file to be
 verified. Ensure the hash file defines an entry for the expected cache file:
 
     Hash File: {}
          File: {}""".format(pkg.hash_file, cache_filename))
-                        rv = False
+                            rv = False
                     else:
                         err('invalid fetch operation (internal error; '
                             'hash-check failure: {})'.format(hr))
                         rv = False
                 else:
                     rv = True
 
+                if rv is not False and perform_file_asc_check and \
+                        os.path.exists(pkg.cache_file):
+                    if GPG.validate(pkg.asc_file, pkg.cache_file):
+                        rv = True
+                    else:
+                        if not path_remove(pkg.cache_file):
+                            err("""\
+failed to validate against ascii-armor
+
+Validation of a package resource failed to verify against a provided ASCII-armor
+file. Ensure that the package's public key has been registered into gpg.
+
+ ASC File: {}
+     File: {}""".format(pkg.asc_file, cache_filename))
+                            rv = False
+                        else:
+                            rv = None
+
                 if rv is not None:
                     if ignore_cache:
                         verbose('ignoring cache not supported for package: {}',
                             name)
                     return rv
 
             # find fetching method for the target vcs-type
@@ -197,37 +223,51 @@
             # checked and then be moved into the download cache
             elif fetched == interim_cache_file:
                 if perform_file_hash_check:
                     hr = verify_hashes(pkg.hash_file, fetched)
                     if hr == HashResult.VERIFIED:
                         pass
                     elif hr == HashResult.BAD_PATH:
-                        if not pkg.is_internal:
+                        if not perform_file_asc_check and not pkg.is_internal:
                             warn('missing hash file for package: ' + name)
                     elif hr == HashResult.EMPTY:
                         if not pkg.is_internal:
                             warn('hash file for package is empty: ' + name)
                     elif hr == HashResult.MISMATCH:
                         return False
                     elif hr in (HashResult.BAD_FORMAT, HashResult.UNSUPPORTED):
                         return False
                     elif hr == HashResult.MISSING_ARCHIVE:
-                        err('missing archive hash for verification')
-                        err("""\
+                        if not perform_file_asc_check:
+                            err("""\
+missing archive hash for verification
+
 The hash file for this package does not have an entry for the cache file to be
 verified. Ensure the hash file defines an entry for the expected cache file:
 
     Hash File: {}
          File: {}""".format(pkg.hash_file, cache_filename))
-                        return False
+                            return False
                     else:
                         err('invalid fetch operation (internal error; '
                             'hash-check failure: {})'.format(hr))
                         return False
 
+                if perform_file_asc_check:
+                    if not GPG.validate(pkg.asc_file, interim_cache_file):
+                        err("""\
+failed to validate against ascii-armor
+
+Validation of a package resource failed to verify against a provided ASCII-armor
+file. Ensure that the package's public key has been registered into gpg.
+
+     ASC File: {}
+         File: {}""".format(pkg.asc_file, cache_filename))
+                        return False
+
                 debug('fetch successful; moving cache file')
 
                 # ensure the download directory exists
                 if not ensure_dir_exists(engine.opts.dl_dir):
                     return False
 
                 try:
```

### Comparing `releng-tool-0.8.0/releng_tool/engine/init.py` & `releng-tool-0.9.0/releng_tool/engine/init.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/install.py` & `releng-tool-0.9.0/releng_tool/engine/install.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/patch.py` & `releng-tool-0.9.0/releng_tool/engine/patch.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/post.py` & `releng-tool-0.9.0/releng_tool/engine/post.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/python/build.py` & `releng-tool-0.9.0/releng_tool/engine/python/build.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/python/install.py` & `releng-tool-0.9.0/releng_tool/engine/python/install.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/script/build.py` & `releng-tool-0.9.0/releng_tool/engine/script/build.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/script/configure.py` & `releng-tool-0.9.0/releng_tool/engine/script/configure.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/engine/script/install.py` & `releng-tool-0.9.0/releng_tool/engine/script/install.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/exceptions.py` & `releng-tool-0.9.0/releng_tool/exceptions.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/ext/seed/__init__.py` & `releng-tool-0.9.0/releng_tool/ext/seed/__init__.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/extract/archive.py` & `releng-tool-0.9.0/releng_tool/extract/archive.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/extract/git.py` & `releng-tool-0.9.0/releng_tool/extract/git.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/extract/mercurial.py` & `releng-tool-0.9.0/releng_tool/extract/mercurial.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/fetch/bzr.py` & `releng-tool-0.9.0/releng_tool/fetch/bzr.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/fetch/cvs.py` & `releng-tool-0.9.0/releng_tool/fetch/cvs.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/fetch/git.py` & `releng-tool-0.9.0/releng_tool/fetch/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,33 @@
     """
     git exists type
 
     Enumeration of types of existence states when verifying a configured
     revision exists in a Git repository.
 
     Attributes:
-        EXISTS: revision exists
+        EXISTS_BRANCH: branch exists
+        EXISTS_HASH: hash exists
+        EXISTS_TAG: tag exists
         MISSING: revision does not exist
         MISSING_HASH: a hash-provided revision does not exist
     """
-    EXISTS = 'exists'
+    EXISTS_BRANCH = 'exists_branch'
+    EXISTS_HASH = 'exists_hash'
+    EXISTS_TAG = 'exists_tag'
     MISSING = 'missing'
     MISSING_HASH = 'missing_hash'
 
+# types indicating a revision exists
+REVISION_EXISTS = [
+    GitExistsType.EXISTS_BRANCH,
+    GitExistsType.EXISTS_HASH,
+    GitExistsType.EXISTS_TAG,
+]
+
 def fetch(opts):
     """
     support fetching from git sources
 
     With provided fetch options (``RelengFetchOptions``), the fetch stage will
     be processed.
 
@@ -54,53 +65,36 @@
         err('unable to fetch package; git is not installed')
         return None
 
     git_dir = '--git-dir=' + cache_dir
 
     # check if we have the target revision cached; if so, package is ready
     if os.path.isdir(cache_dir) and not opts.ignore_cache:
-        if revision_exists(git_dir, revision) == GitExistsType.EXISTS:
+        erv = revision_exists(git_dir, revision)
+        if erv in REVISION_EXISTS:
             # ensure configuration is properly synchronized
             if not _sync_git_configuration(opts):
                 return None
 
-            return cache_dir
+            # if no explicit ignore-cache request and if the revision is a
+            # branch, force ignore-cache on and allow fetching to proceed
+            if opts.ignore_cache is None and erv == GitExistsType.EXISTS_BRANCH:
+                opts.ignore_cache = True
+            # return cache dir if not verifying or verification succeeds
+            elif not opts._git_verify_revision or _verify_revision(
+                    git_dir, revision, quiet=True):
+                return cache_dir
 
     note('fetching {}...'.format(name))
     sys.stdout.flush()
 
-    # if we have a cache dir, ensure it's stable
-    #
-    # If we have a cache directory for this page but didn't find the the target
-    # revision above, first check if the Git cache has been corrupted. If
-    # anything is suspected wrong, start from a fresh state.
-    has_cache = False
-    clean_cache = False
-    if os.path.isdir(cache_dir):
-        if opts.ignore_cache:
-            verbose('sanity checking if cached directory is valid')
-            if GIT.execute([git_dir, 'rev-parse'], cwd=cache_dir, quiet=True):
-                has_cache = True
-            else:
-                clean_cache = True
-        else:
-            log('cache directory exists for package; validating')
-            if GIT.execute([git_dir, 'fsck', '--full'], cwd=cache_dir,
-                    quiet=True):
-                has_cache = True
-            else:
-                clean_cache = True
-
-    if clean_cache:
-        log('cache directory has errors; will re-downloaded')
-
-        if not path_remove(cache_dir):
-            err('''unable to cleanup cache folder for package
-(cache folder: {})'''.format(cache_dir))
-            return None
+    # validate any cache directory (if one exists)
+    has_cache, bad_validation = _validate_cache(cache_dir)
+    if bad_validation:
+        return None
 
     # if we have no cache for this repository, build one
     if not has_cache:
         if not ensure_dir_exists(cache_dir):
             return None
 
         if not GIT.execute([git_dir, 'init', '--bare'], cwd=cache_dir):
@@ -111,14 +105,28 @@
     if not _sync_git_configuration(opts):
         return None
 
     # fetch sources for this repository
     if not _fetch_srcs(opts, cache_dir, revision, refspecs=opts._git_refspecs):
         return None
 
+    # verify revision (if configured to check it)
+    if opts._git_verify_revision:
+        if not _verify_revision(git_dir, revision):
+            err("""\
+failed to validate git revision
+
+Package has been configured to require the verification of the GPG signature
+for the target revision. The verification has failed. Ensure that the revision
+is signed and that the package's public key has been registered in the system.
+
+      Package: {}
+     Revision: {}""".format(name, revision))
+            return None
+
     # fetch submodules (if configured to do so)
     if opts._git_submodules:
         if not _fetch_submodules(opts, cache_dir, revision):
             return None
 
     return cache_dir
 
@@ -225,28 +233,28 @@
     if not GIT.execute(fetch_cmd, cwd=cache_dir):
         err('unable to fetch branches/tags from remote repository')
         return False
 
     if revision:
         verbose('verifying target revision exists')
         exists_state = revision_exists(git_dir, revision)
-        if exists_state == GitExistsType.EXISTS:
+        if exists_state in REVISION_EXISTS:
             pass
         elif (exists_state == GitExistsType.MISSING_HASH and
                 limited_fetch and opts._git_depth is None):
             warn('failed to find hash on depth-limited fetch; fetching all...')
 
             fetch_cmd = list(prepared_fetch_cmd)
             fetch_cmd.append('--unshallow')
 
             if not GIT.execute(fetch_cmd, cwd=cache_dir):
                 err('unable to unshallow fetch state')
                 return False
 
-            if revision_exists(git_dir, revision) != GitExistsType.EXISTS:
+            if revision_exists(git_dir, revision) not in REVISION_EXISTS:
                 err('unable to find matching revision in ' + desc)
                 err(' (revision: {}) '.format(revision))
                 return False
         else:
             err('unable to find matching revision in ' + desc)
             err(' (revision: {}) '.format(revision))
             return False
@@ -264,14 +272,18 @@
         git_dir: the Git directory
         revision: the revision (branch, tag, hash) to look for
 
     Returns:
         a value of ``GitExistsType``
     """
 
+    if GIT.execute([git_dir, 'rev-parse', '--quiet', '--verify',
+            'refs/tags/' + revision], quiet=True):
+        return GitExistsType.EXISTS_TAG
+
     output = []
     if not GIT.execute([git_dir, 'rev-parse', '--quiet', '--verify',
             revision], quiet=True, capture=output):
         if not GIT.execute([git_dir, 'rev-parse', '--quiet', '--verify',
                 'origin/' + revision], quiet=True, capture=output):
             return GitExistsType.MISSING
 
@@ -279,18 +291,20 @@
     #
     # A call to `rev-parse` with a full hash may succeed even through the
     # hash does not exist in a repository (short hashes are valid though).
     # To handle this case, check if the revision matches the returned hash
     # valid provided. If so, perform a `cat-file` request to ensure the long
     # hash entry is indeed a valid commit.
     if output and output[0] == revision:
-        if not GIT.execute([git_dir, 'cat-file', '-t', revision], quiet=True):
+        if GIT.execute([git_dir, 'cat-file', '-t', revision], quiet=True):
+            return GitExistsType.EXISTS_HASH
+        else:
             return GitExistsType.MISSING_HASH
 
-    return GitExistsType.EXISTS
+    return GitExistsType.EXISTS_BRANCH
 
 def _sync_git_configuration(opts):
     """
     ensure the git configuration is properly synchronized with this repository
 
     This call ensures that various Git configuration options are properly
     synchronized with the cached Git repository. This includes:
@@ -467,41 +481,24 @@
     git_dir = '--git-dir=' + cache_dir
 
     # check if we have the target revision cached; if so, submodule is ready
     if os.path.isdir(cache_dir) and not opts.ignore_cache:
         if not revision:
             return _sync_git_origin(cache_dir, site)
 
-        if revision_exists(git_dir, revision) == GitExistsType.EXISTS:
+        if revision_exists(git_dir, revision) in REVISION_EXISTS:
             return _sync_git_origin(cache_dir, site)
 
     log('processing submodule (package: {}) {}...'.format(opts.name, name))
     sys.stdout.flush()
 
-    # if we have a cache dir, ensure it's stable
-    #
-    # If we have a cache directory for this page but didn't find the the target
-    # revision above, first check if the Git cache has been corrupted. If
-    # anything is suspected wrong, start from a fresh state.
-    has_cache = False
-    if os.path.isdir(cache_dir):
-        if opts.ignore_cache:
-            has_cache = True
-        else:
-            log('cache directory exists for submodule; validating')
-            if GIT.execute([git_dir, 'fsck', '--full'], cwd=cache_dir,
-                    quiet=True):
-                has_cache = True
-            else:
-                log('cache directory has errors; will re-downloaded')
-
-                if not path_remove(cache_dir):
-                    err('''unable to cleanup cache folder for package
- (cache folder: {})'''.format(cache_dir))
-                    return False
+    # validate any cache directory (if one exists)
+    has_cache, bad_validation = _validate_cache(cache_dir)
+    if bad_validation:
+        return None
 
     # if we have no cache for this repository, build one
     if not has_cache:
         if not ensure_dir_exists(cache_dir):
             return False
 
         if not GIT.execute([git_dir, 'init', '--bare'], cwd=cache_dir):
@@ -511,7 +508,77 @@
     # ensure configuration is properly synchronized
     if not _sync_git_origin(cache_dir, site):
         return False
 
     # fetch sources for this submodule
     desc = 'submodule ({}): {}'.format(opts.name, name)
     return _fetch_srcs(opts, cache_dir, revision, desc=desc)
+
+def _validate_cache(cache_dir):
+    """
+    validate an existing cache directory to fetch on
+
+    A fetch operation may occur on an existing cache directory, typically when
+    a force-fetch or a configured revision has changed. This call helps
+    validate the existing cache directory (from a bad state such as a corrupted
+    repository). If a cache directory does exist,
+
+    Args:
+        cache_dir: the cache/bare repository to fetch into
+
+    Returns:
+        a 2-tuple (if a cache directory exists; and if validation failed)
+    """
+
+    git_dir = '--git-dir=' + cache_dir
+
+    bad_validation = False
+    has_cache = False
+    if os.path.isdir(cache_dir):
+        log('cache directory detected; validating')
+        if GIT.execute([git_dir, 'rev-parse'], cwd=cache_dir, quiet=True):
+            debug('cache directory validated')
+            has_cache = True
+        else:
+            log('cache directory has errors; will re-downloaded')
+            if not path_remove(cache_dir):
+                err('unable to cleanup cache folder for package\n'
+                    ' (cache folder: {})', cache_dir)
+                bad_validation = True
+
+    return has_cache, bad_validation
+
+def _verify_revision(git_dir, revision, quiet=False):
+    """
+    verify the gpg signature for a target revision
+
+    The GPG signature for a provided revision (tag or commit) will be checked
+    to validate the revision.
+
+    Args:
+        git_dir: the Git directory
+        revision: the revision to verify
+        quiet (optional): whether or not the log if verification is happening
+
+    Returns:
+        ``True`` if the revision is signed; ``False`` otherwise
+    """
+
+    if not quiet:
+        log('verifying the gpg signature on the target revision')
+    else:
+        verbose('verifying the gpg signature on the target revision')
+
+    if GIT.execute([git_dir, 'rev-parse', '--quiet',
+            '--verify', revision + '^{tag}'], quiet=True):
+        verified_cmd = 'verify-tag'
+    else:
+        verified_cmd = 'verify-commit'
+
+        # acquire the commit if (if not already set), to ensure we can verify
+        # against commits or branches
+        rv, revision = GIT.execute_rv(git_dir, 'rev-parse', revision)
+        if rv != 0:
+            verbose('failed to determine the commit id for a revision')
+            return False
+
+    return GIT.execute([git_dir, verified_cmd, revision], quiet=quiet)
```

### Comparing `releng-tool-0.8.0/releng_tool/fetch/mercurial.py` & `releng-tool-0.9.0/releng_tool/fetch/mercurial.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/fetch/scp.py` & `releng-tool-0.9.0/releng_tool/fetch/scp.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/fetch/svn.py` & `releng-tool-0.9.0/releng_tool/fetch/svn.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/fetch/url.py` & `releng-tool-0.9.0/releng_tool/fetch/url.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/opts.py` & `releng-tool-0.9.0/releng_tool/opts.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 DEFAULT_SYMBOLS_DIR  = 'symbols'   #: default symbols container directory
 DEFAULT_TARGET_DIR   = 'target'    #: default target container directory
 
 # default directory/file paths
 RELENG_CONF_EXTENDED_NAME = '.releng-tool' #: extended configuration script
 RELENG_CONF_NAME = 'releng' #: configuration script filename
 RELENG_CONF_OVERRIDES_NAME = 'releng-overrides' #: conf. overrides filename
-RELENG_POST_NAME = 'releng-post' #: post script filename
+RELENG_POST_BUILD_NAME = 'releng-post-build' #: post build script filename
 FF_PREFIX = '.releng-flag-' #: prefix for all file flags
 FF_DEVMODE_NAME = 'devmode' #: postfix for development mode file flag
 FF_LOCALSRCS_NAME = 'local-sources' #: postfix for local sources mode file flag
 
 # default other
 DEFAULT_SYSROOT_PREFIX = os.sep + 'usr' #: default system root prefix
 
@@ -66,15 +66,15 @@
         jobsconf: number of jobs to allow at a given time (0: auto)
         license_dir: directory container for license information
         license_header: header content for a generated license file (if any)
         local_srcs: whether or not local sources are used
         no_color_out: whether or not colored messages are shown
         out_dir: directory container for all output data
         pkg_action: the specific package-action to perform (if any)
-        post_point: resource to process holding a releng project's post-work
+        post_build_point: resource to process a releng project's post-build work
         prerequisites: list of required host tools (if any)
         quirks: advanced configuration quirks for the running instance
         revision_override: dictionary to override revision values
         root_dir: directory container for all (configuration, output, etc.)
         sites_override: dictionary to override site values
         staging_dir: directory container for staged content
         symbols_dir: directory container for symbols content
@@ -107,15 +107,15 @@
         self.jobsconf = 0
         self.license_dir = None
         self.license_header = None
         self.local_srcs = None
         self.no_color_out = False
         self.out_dir = None
         self.pkg_action = None
-        self.post_point = None
+        self.post_build_point = None
         self.prerequisites = []
         self.quirks = []
         self.revision_override = None
         self.root_dir = None
         self.sites_override = None
         self.staging_dir = None
         self.symbols_dir = None
@@ -218,16 +218,16 @@
             self.conf_point = join(root, RELENG_CONF_NAME)
         if not self.conf_point_overrides:
             self.conf_point_overrides = join(root, RELENG_CONF_OVERRIDES_NAME)
         if not self.ff_devmode:
             self.ff_devmode = join(root, FF_PREFIX + FF_DEVMODE_NAME)
         if not self.ff_local_srcs:
             self.ff_local_srcs = join(root, FF_PREFIX + FF_LOCALSRCS_NAME)
-        if not self.post_point:
-            self.post_point = join(root, RELENG_POST_NAME)
+        if not self.post_build_point:
+            self.post_build_point = join(root, RELENG_POST_BUILD_NAME)
 
         # provided fixed job count with auto-configuration (value: 0)
         #
         # The option ``jobsconf`` defines the number of jobs the user wants to
         # use for the process. When providing this information to tools, a value
         # of zero allows a tool to configure its own automatic parallel
         # processing. In some scenarios, a tool may not provide the ability to
```

### Comparing `releng-tool-0.8.0/releng_tool/packages/__init__.py` & `releng-tool-0.9.0/releng_tool/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/packages/exceptions.py` & `releng-tool-0.9.0/releng_tool/packages/exceptions.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/packages/manager.py` & `releng-tool-0.9.0/releng_tool/packages/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from releng_tool.defs import RPK_EXTOPT
 from releng_tool.defs import RPK_EXTRACT_TYPE
 from releng_tool.defs import RPK_FIXED_JOBS
 from releng_tool.defs import RPK_GIT_CONFIG
 from releng_tool.defs import RPK_GIT_DEPTH
 from releng_tool.defs import RPK_GIT_REFSPECS
 from releng_tool.defs import RPK_GIT_SUBMODULES
+from releng_tool.defs import RPK_GIT_VERIFY_REVISION
 from releng_tool.defs import RPK_INSTALL_DEFS
 from releng_tool.defs import RPK_INSTALL_ENV
 from releng_tool.defs import RPK_INSTALL_OPTS
 from releng_tool.defs import RPK_INSTALL_TYPE
 from releng_tool.defs import RPK_INTERNAL
 from releng_tool.defs import RPK_LICENSE
 from releng_tool.defs import RPK_LICENSE_FILES
@@ -138,14 +139,15 @@
         self._register_conf(RPK_EXTOPT, PkgKeyType.DICT)
         self._register_conf(RPK_EXTRACT_TYPE, PkgKeyType.STR)
         self._register_conf(RPK_FIXED_JOBS, PkgKeyType.INT_POSITIVE)
         self._register_conf(RPK_GIT_CONFIG, PkgKeyType.DICT_STR_STR)
         self._register_conf(RPK_GIT_DEPTH, PkgKeyType.INT_NONNEGATIVE)
         self._register_conf(RPK_GIT_REFSPECS, PkgKeyType.STRS)
         self._register_conf(RPK_GIT_SUBMODULES, PkgKeyType.BOOL)
+        self._register_conf(RPK_GIT_VERIFY_REVISION, PkgKeyType.BOOL)
         self._register_conf(RPK_INSTALL_DEFS, PkgKeyType.DICT_STR_STR)
         self._register_conf(RPK_INSTALL_ENV, PkgKeyType.DICT_STR_STR)
         self._register_conf(RPK_INSTALL_OPTS, PkgKeyType.DICT_STR_STR_OR_STRS)
         self._register_conf(RPK_INSTALL_TYPE, PkgKeyType.STR)
         self._register_conf(RPK_INTERNAL, PkgKeyType.BOOL)
         self._register_conf(RPK_LICENSE, PkgKeyType.STRS)
         self._register_conf(RPK_LICENSE_FILES, PkgKeyType.STRS)
@@ -240,15 +242,15 @@
         debug('sorting packages...')
         def fetch_deps(pkg):
             return pkg.deps
         sorter = TopologicalSorter(fetch_deps)
         sorted_pkgs = []
         for pkg in pkgs.values():
             sorted_pkgs = sorter.sort(pkg)
-            if not sorted:
+            if sorted_pkgs is None:
                 raise RelengToolCyclicPackageDependency({
                     'pkg_name': name,
                 })
         debug('sorted packages)')
         for pkg in sorted_pkgs:
             debug(' {}'.format(pkg.name))
 
@@ -485,14 +487,17 @@
 
         # git-refspecs
         pkg_git_refspecs = self._fetch(RPK_GIT_REFSPECS)
 
         # git-submodules
         pkg_git_submodules = self._fetch(RPK_GIT_SUBMODULES)
 
+        # git-verify
+        pkg_git_verify_revision = self._fetch(RPK_GIT_VERIFY_REVISION)
+
         # ######################################################################
 
         # checks
         if pkg_is_external is not None and pkg_is_internal is not None:
             if pkg_is_external == pkg_is_internal:
                 raise RelengToolConflictingConfiguration({
                     'pkg_name': name,
@@ -635,26 +640,28 @@
 
             # adjust the cache directory and save any new cache changes
             pkg_cache_dir = os.path.join(opts.cache_dir, pkg_cache_dirname)
             self._save_dvcs_cache()
 
         # (commons)
         pkg = RelengPackage(name, pkg_version)
+        pkg.asc_file = os.path.join(pkg_def_dir, name + '.asc')
         pkg.build_dir = pkg_build_dir
         pkg.build_output_dir = pkg_build_output_dir
         pkg.build_subdir = pkg_build_subdir
         pkg.cache_dir = pkg_cache_dir
         pkg.cache_file = pkg_cache_file
         pkg.def_dir = pkg_def_dir
         pkg.devmode_ignore_cache = pkg_devmode_ignore_cache
         pkg.extract_type = pkg_extract_type
         pkg.git_config = pkg_git_config
         pkg.git_depth = pkg_git_depth
         pkg.git_refspecs = pkg_git_refspecs
         pkg.git_submodules = pkg_git_submodules
+        pkg.git_verify_revision = pkg_git_verify_revision
         pkg.has_devmode_option = pkg_has_devmode_option
         pkg.hash_file = os.path.join(pkg_def_dir, name + '.hash')
         pkg.is_internal = pkg_is_internal
         pkg.no_extraction = pkg_no_extraction
         pkg.revision = pkg_revision
         pkg.site = pkg_site
         pkg.skip_remote_config = pkg_skip_remote_config
```

### Comparing `releng-tool-0.8.0/releng_tool/packages/package.py` & `releng-tool-0.9.0/releng_tool/packages/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
     A package tracks the name, options and dependencies of the package.
 
     Args:
         name: the name of the package
 
     Attributes:
+        asc_file: file containing ascii-armored data to validate this package
         build_dir: directory for a package's buildable content
         build_output_dir: build output directory for the package process
         build_subdir: override for a package's buildable content (if applicable)
         cache_dir: cache directory for the package (if applicable)
         cache_file: cache file for the package (if applicable)
         def_dir: directory for the package definition
         deps: list of dependencies for this package
@@ -22,14 +23,15 @@
         ext_modifiers: extension-defined modifiers (dict)
         extract_type: extraction type override (for extensions, if applicable)
         fixed_jobs: fixed job count for this specific package
         git_config: git config options to apply (if applicable)
         git_depth: git fetch depth (if applicable)
         git_refspecs: additional git refspecs to fetch (if applicable)
         git_submodules: fetch any git submodules (if applicable)
+        git_verify_revision: verify signed git revisions
         has_devmode_option: whether or not the package has a devmode revision
         hash_file: file containing hashes to validate this package
         install_type: install container for the package (target, staged, etc.)
         is_internal: whether or not this package is an project internal package
         license: license(s) of the package
         license_files: list of files in sources holding license information
         name: name of the package
@@ -60,22 +62,23 @@
         python_interpreter: python interpreter to invoke stages with
     """
     def __init__(self, name, version):
         self.name = name
         self.nv = '{}-{}'.format(name, version)
         self.version = version
         # (commons)
+        self.asc_file = None
         self.build_dir = None
         self.build_subdir = None
         self.build_output_dir = None
         self.cache_dir = None
         self.cache_file = None
         self.def_dir = None
         self.deps = []
-        self.devmode_ignore_cache = False
+        self.devmode_ignore_cache = None
         self.fixed_jobs = None
         self.has_devmode_option = None
         self.hash_file = None
         self.ext_modifiers = None
         self.extract_type = None
         self.install_type = None
         self.is_internal = None
@@ -103,28 +106,10 @@
         # (package type - autotools)
         self.autotools_autoreconf = None
         # (other - git)
         self.git_config = None
         self.git_depth = None
         self.git_refspecs = None
         self.git_submodules = None
+        self.git_verify_revision = None
         # (other - python)
         self.python_interpreter = None
-
-    def __str__(self):
-        return (
-            'package "{}"\n'
-            '      build: {}\n'
-            '  build-out: {}\n'
-            ' definition: {}\n'
-            '       site: {}\n'
-            '   vcs-type: {}\n'
-            '    version: {}'
-            ).format(
-                self.name,
-                self.build_dir,
-                self.build_output_dir,
-                self.def_dir,
-                self.site,
-                self.vcs_type,
-                self.version,
-                )
```

### Comparing `releng-tool-0.8.0/releng_tool/packages/pipeline.py` & `releng-tool-0.9.0/releng_tool/packages/pipeline.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/prerequisites.py` & `releng-tool-0.9.0/releng_tool/prerequisites.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/registry.py` & `releng-tool-0.9.0/releng_tool/registry.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/stats.py` & `releng-tool-0.9.0/releng_tool/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,9 +296,13 @@
 
             # generate figures
             dur_pdf = os.path.join(self.out_dir, 'durations.pdf')
             fig_pkgs.savefig(dur_pdf)
 
             dur_pdf_total = os.path.join(self.out_dir, 'durations-total.pdf')
             fig_total.savefig(dur_pdf_total)
+
+            # close/cleanup figures
+            for fig in figs:
+                plt.close()
         else:
             debug('duration statistics plot not supported')
```

### Comparing `releng-tool-0.8.0/releng_tool/tool/__init__.py` & `releng-tool-0.9.0/releng_tool/tool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,20 +105,20 @@
             poll (optional): force polling stdin/stdout for output data
             capture (optional): list to capture output into
 
         Returns:
             the return code of the execution request
         """
         if not self.exists():
-            return False
+            return 1
 
         if args and not is_sequence_not_string(args):
             err('invalid argument type provided into execute (should be list): '
                 + str(args))
-            return False
+            return 1
 
         final_env = None
         if self.include or self.sanitize or env:
             final_env = os.environ.copy()
             if self.sanitize:
                 for key in self.sanitize:
                     final_env.pop(key, None)
```

### Comparing `releng-tool-0.8.0/releng_tool/tool/bzr.py` & `releng-tool-0.9.0/releng_tool/tool/bzr.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/tool/cvs.py` & `releng-tool-0.9.0/releng_tool/tool/cvs.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/tool/git.py` & `releng-tool-0.9.0/releng_tool/tool/git.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,22 +58,26 @@
         Args:
             bare_dir: the bare repository
 
         Returns:
             the revision; ``None`` when a revision cannot be extracted
         """
 
-        rv, ref = self.execute_rv(
-            '--git-dir=' + bare_dir, 'show-ref', '--head')
+        rv, ref = self.execute_rv('--git-dir=' + bare_dir, 'show-ref', '--head')
         if rv != 0:
             err('failed to extract a submodule revision')
             return None
 
-        revision = ref.split(' ', 1)[1]
-        revision = revision[len('refs/remotes/origin/'):]
+        # a `--head` fetch may fetch more than one reference; extract the first
+        # entry and remove any known ref prefix from it
+        revision = ref.split(None, 2)[1]
+        if revision.startswith('refs/heads/'):
+            revision = revision[len('refs/heads/'):]
+        elif revision.startswith('refs/remotes/origin/'):
+            revision = revision[len('refs/remotes/origin/'):]
         return revision
 
     def parse_cfg_file(self, target):
         """
         return a configuration parser for a provided git configuration file
 
         Returns a prepared configuration parser based of a Git configuration
```

### Comparing `releng-tool-0.8.0/releng_tool/tool/hg.py` & `releng-tool-0.9.0/releng_tool/tool/hg.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/tool/patch.py` & `releng-tool-0.9.0/releng_tool/tool/patch.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/tool/python.py` & `releng-tool-0.9.0/releng_tool/tool/python.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/tool/scp.py` & `releng-tool-0.9.0/releng_tool/tool/scp.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/__init__.py` & `releng-tool-0.9.0/releng_tool/util/__init__.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/api.py` & `releng-tool-0.9.0/releng_tool/util/api.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/enum.py` & `releng-tool-0.9.0/releng_tool/util/enum.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/env.py` & `releng-tool-0.9.0/releng_tool/util/env.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/file_flags.py` & `releng-tool-0.9.0/releng_tool/util/file_flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,28 +41,29 @@
 
     Returns:
         ``FileFlag.EXISTS`` if the flag is enabled; ``FileFlag.NO_EXIST`` if the
             flag is not enabled
     """
     return process_file_flag(None, file)
 
-def process_file_flag(flag, file):
+def process_file_flag(flag, file, quiet=False):
     """
     process a file flag event
 
     Will either write a file flag configuration event or attempt to read a file
     flag state. If the ``flag`` option is set to ``True``, this process event
     will assume that this instance is attempting to configure a file flag (on)
     state and generate the target file flag on the system. If the flag option is
     set to ``False``, the file's existence will be checked to reflect whether or
     not the flag is considered enabled.
 
     Args:
         flag: the flag option to used; ``None`` to check flag state
         file: the filename
+        quiet: suppression of any error messages to standard out
 
     Returns:
         ``FileFlag.EXISTS`` if the flag is enabled; ``FileFlag.NO_EXIST`` if the
             flag is not enabled; ``FileFlag.CONFIGURED`` if the flag was
             configured as requested; ``FileFlag.NOT_CONFIGURED`` if the flag
             could not be configured as requested
     """
@@ -75,14 +76,15 @@
         if touch(file):
             rv = FileFlag.CONFIGURED
         else:
             if os.path.isfile(file):
                 rv = FileFlag.CONFIGURED
             else:
                 rv = FileFlag.NOT_CONFIGURED
-                err('unable to configure file flag: {}'.format(file))
+                if not quiet:
+                    err('unable to configure file flag: {}', file)
     elif flag is None and os.path.isfile(file):
         rv = FileFlag.EXISTS
     else:
         rv = FileFlag.NO_EXIST
 
     return rv
```

### Comparing `releng-tool-0.8.0/releng_tool/util/hash.py` & `releng-tool-0.9.0/releng_tool/util/hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,17 @@
     # load hashes
     try:
         hash_info = load(hash_file)
     except BadFileHashLoadError:
         return HashResult.BAD_PATH
     except BadFormatHashLoadError as e:
         if not quiet:
-            err('hash file is not properly formatted')
             err("""\
+hash file is not properly formatted
+
 The hash file provided is incorrectly formatted. The hash file expects lines
 with the hash type, hash and target file provided. For example:
 
     sha1 f572d396fae9206628714fb2ce00f72e94f2258f my-file
 
 Please correct the following hash file:
 
@@ -182,16 +183,17 @@
 
     for asset, type_hashes in hash_catalog.items():
         hashers = {}
         for hash_type in type_hashes.keys():
             hashers[hash_type] = _get_hasher(hash_type)
             if not hashers[hash_type]:
                 if not quiet:
-                    err('unsupported hash type')
                     err("""\
+unsupported hash type
+
 The hash file defines a hash type not supported by the releng-tool. Officially
 supported hash types are FIPS-180 algorithms (sha1, sha224, sha256, sha384 and
 sha512) as well as (but not recommended) RSA'S MD5 algorithm. Other algorithms,
 while unofficially supported, can be used if provided by the system's OpenSSL
 library.
 
      Hash File: {}
@@ -207,16 +209,17 @@
                         hasher.update(buf)
                     buf = f.read(HASH_READ_BLOCKSIZE)
         except IOError:
             if not quiet:
                 if relaxed:
                     warn('missing expected file for verification: ' + asset)
                 else:
-                    err('missing expected file for verification')
                     err("""\
+missing expected file for verification
+
 A defined hash entry cannot be verified since the target file does not exist.
 Ensure the hash file correctly names an expected file.
 
     Hash File: {}
          File: {}""".format(hash_file, asset))
             return HashResult.MISSING_LISTED
```

### Comparing `releng-tool-0.8.0/releng_tool/util/io.py` & `releng-tool-0.9.0/releng_tool/util/io.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/log.py` & `releng-tool-0.9.0/releng_tool/util/log.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/platform.py` & `releng-tool-0.9.0/releng_tool/util/platform.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/sort.py` & `releng-tool-0.9.0/releng_tool/util/sort.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool/util/string.py` & `releng-tool-0.9.0/releng_tool/util/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # -*- coding: utf-8 -*-
-# Copyright 2018-2019 releng-tool
+# Copyright 2018-2021 releng-tool
 
-from collections import Sequence
 import os
 
 try:
     basestring
 except NameError:
     basestring = str
 
+try:
+    from collections.abc import Sequence
+except ImportError:
+    from collections import Sequence
+
 def expand(obj, kv=None):
     """
     perform variable expansion on strings
 
     This expand utility method will attempt to expand variables in detected
     string types. For a detected string which contains substrings in the form of
     ``$value`` or ``${value}``, these substrings will be replaced with their
```

### Comparing `releng-tool-0.8.0/releng_tool/util/win32.py` & `releng-tool-0.9.0/releng_tool/util/win32.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/releng_tool.egg-info/PKG-INFO` & `releng-tool-0.9.0/releng_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: releng-tool
-Version: 0.8.0
+Version: 0.9.0
 Summary: release engineering utility tool
 Home-page: https://releng.io
 Author: releng-tool
 Author-email: releng@releng.io
 License: BSD-2-Clause
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -43,59 +43,64 @@
 .. image:: https://img.shields.io/pypi/dm/releng-tool.svg
     :target: https://pypi.python.org/pypi/releng-tool
     :alt: PyPI download month
 
 releng-tool aims to provide a method to prepare a structured environment to
 assist in the release engineering of a project.
 
-overview
+Overview
 --------
 
 When dealing with the release engineering of a project, assets may be found in
 multiple locations and may require various methods to extract, build and more.
 releng-tool can be used to process a defined set of projects/packages which
 identify where resources can be fetched, how packages can be extracted and
 methods to patch, configure, build and install each individual package for a
 target root.
 
 For detailed documentation on the releng-tool project, please consult the
 `releng-tool documentation`_.
 
-requirements
+Requirements
 ------------
 
 * Python_ 2.7 or 3.4+
 
 Host tools such as Git_, scp, etc. may be required depending on the project
 being processed (e.g. if a package's sources fetch from a Git source, a Git
 client tool is required to perform said fetch).
 
-installation
+Installation
 ------------
 
 This tool can be installed using pip_:
 
 .. code-block:: shell
 
    pip install releng-tool
     (or)
    python -m pip install releng-tool
 
-usage
+For Arch Linux users, this package is also available on AUR:
+
+ | Arch User Repository - releng-tool
+ | https://aur.archlinux.org/packages/releng-tool/
+
+Usage
 -----
 
 This tool can be invoked from a command line using:
 
 .. code-block:: shell
 
    releng-tool --help
     (or)
    python -m releng_tool --help
 
-examples
+Examples
 --------
 
 Examples of releng-tool projects can be found in
 `releng-tool's examples repository`_.
 
 .. _Git: https://git-scm.com/
 .. _Python: https://www.python.org/
```

### Comparing `releng-tool-0.8.0/releng_tool.egg-info/SOURCES.txt` & `releng-tool-0.9.0/releng_tool.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 releng_tool/packages/pipeline.py
 releng_tool/tool/__init__.py
 releng_tool/tool/autoreconf.py
 releng_tool/tool/bzr.py
 releng_tool/tool/cmake.py
 releng_tool/tool/cvs.py
 releng_tool/tool/git.py
+releng_tool/tool/gpg.py
 releng_tool/tool/hg.py
 releng_tool/tool/make.py
 releng_tool/tool/patch.py
 releng_tool/tool/python.py
 releng_tool/tool/scp.py
 releng_tool/tool/svn.py
 releng_tool/tool/tar.py
@@ -95,14 +96,19 @@
 scripts/completion/fish
 scripts/completion/zsh
 tests/__init__.py
 tests/__main__.py
 tests/support/__init__.py
 tests/support/pkg_config_test.py
 tests/support/site_tool_test.py
+tests/templates/cyclic/releng
+tests/templates/cyclic/package/test-a/test-a
+tests/templates/cyclic/package/test-b/test-b
+tests/templates/cyclic/package/test-c/test-c
+tests/templates/cyclic/package/test-d/test-d
 tests/templates/licenses/releng
 tests/templates/licenses/package/test-a/COPYING.bsd
 tests/templates/licenses/package/test-a/COPYING.mit
 tests/templates/licenses/package/test-a/test-a
 tests/templates/licenses/package/test-b/test-b
 tests/templates/licenses/package/test-c/LICENSE
 tests/templates/licenses/package/test-c/test-c
@@ -152,14 +158,15 @@
 tests/unit-tests/__init__.py
 tests/unit-tests/test_engine_run_actions.py
 tests/unit-tests/test_engine_run_defaults.py
 tests/unit-tests/test_engine_run_file_flags.py
 tests/unit-tests/test_file_flags.py
 tests/unit-tests/test_pkg_configs.py
 tests/unit-tests/test_pkg_configs_autotools.py
+tests/unit-tests/test_pkg_configs_cyclic.py
 tests/unit-tests/test_pkg_configs_devmode.py
 tests/unit-tests/test_pkg_configs_extensions.py
 tests/unit-tests/test_pkg_configs_git.py
 tests/unit-tests/test_pkg_configs_stageopts.py
 tests/unit-tests/test_pkg_configs_type.py
 tests/unit-tests/test_pkg_configs_vcs_type.py
 tests/unit-tests/test_pkg_pipeline_licenses.py
@@ -240,14 +247,17 @@
 tests/unit-tests/assets/configs/git-refspecs-invalid-value
 tests/unit-tests/assets/configs/git-refspecs-valid-empty
 tests/unit-tests/assets/configs/git-refspecs-valid-multiple
 tests/unit-tests/assets/configs/git-refspecs-valid-single
 tests/unit-tests/assets/configs/git-submodules-disabled
 tests/unit-tests/assets/configs/git-submodules-enabled
 tests/unit-tests/assets/configs/git-submodules-invalid
+tests/unit-tests/assets/configs/git-verify-disabled
+tests/unit-tests/assets/configs/git-verify-enabled
+tests/unit-tests/assets/configs/git-verify-invalid
 tests/unit-tests/assets/configs/install-defs-invalid-base-type
 tests/unit-tests/assets/configs/install-defs-invalid-key-type
 tests/unit-tests/assets/configs/install-defs-invalid-strs
 tests/unit-tests/assets/configs/install-defs-invalid-value-type
 tests/unit-tests/assets/configs/install-defs-valid
 tests/unit-tests/assets/configs/install-env-invalid-base-type
 tests/unit-tests/assets/configs/install-env-invalid-key-type
```

### Comparing `releng-tool-0.8.0/scripts/completion/fish` & `releng-tool-0.9.0/scripts/completion/fish`

 * *Files 2% similar despite different names*

```diff
@@ -79,32 +79,35 @@
     --description 'enables development mode'
 complete --command releng-tool --long-option='dl-dir' \
     --require-parameter \
     --description 'directory for download archives'
 complete --command releng-tool --long-option='help' --short-option=h \
     --no-files \
     --description 'show help'
+complete --command releng-tool --long-option='help-quirks' \
+    --no-files \
+    --description 'show available quirks'
 complete --command releng-tool --long-option='jobs' --short-option=j \
     --no-files --require-parameter \
     --description 'numbers of jobs to handle'
 complete --command releng-tool --long-option='local-sources' \
     --no-files \
     --description 'enables local-sources mode'
 complete --command releng-tool --long-option='nocolorout' \
     --no-files \
     --description 'explicitly disable colorized output'
 complete --command releng-tool --long-option='out-dir' \
     --require-parameter \
     --description 'directory for output'
 complete --command releng-tool --long-option='root-dir' \
     --require-parameter \
-    --description 'directory to process a releng-tool project'
+    --description 'directory of the project to process'
 complete --command releng-tool --long-option='quirk' \
     --no-files \
     --require-parameter \
     --description 'quirk to apply to a run'
 complete --command releng-tool --long-option='verbose' \
     --no-files \
     --description 'show additional messages'
 complete --command releng-tool --long-option='version' \
     --no-files \
-    --description "show releng-tool's version"
+    --description "print the version and exit"
```

### Comparing `releng-tool-0.8.0/scripts/completion/zsh` & `releng-tool-0.9.0/scripts/completion/zsh`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 
     _arguments -C \
         '--cache-dir[directory for distributed version control cache]: :_files' \
         '--debug[show debug-related messages]' \
         '--development[enables development mode]' \
         '--dl-dir[directory for download archives]: :_files' \
         '--help[show help]' '-h[show help]' \
+        '--help-quirks[show available quirks]' \
         '--jobs[numbers of jobs to handle]: ' '-j[numbers of jobs to handle]: ' \
         '--local-sources[enables local-sources mode]' \
         '--nocolorout[explicitly disable colorized output]' \
         '--out-dir[directory for output]: :_files' \
-        '--root-dir[directory to process a releng-tool project]: :_files' \
+        '--root-dir[directory of the project to process]: :_files' \
         '--quirk[quirk to apply to a run]: ' \
         '--verbose[show additional messages]' \
-        "--version[show releng-tool's version]" \
+        "--version[print the version and exit]" \
         "1: :($opts)"
 }
+
+_releng_tool "$@"
```

### Comparing `releng-tool-0.8.0/setup.py` & `releng-tool-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,10 +64,10 @@
     license='BSD-2-Clause',
     long_description=read('README.rst'),
     name='releng-tool',
     packages=find_packages(exclude=["tests*"]),
     platforms='any',
     test_suite='tests',
     url='https://releng.io',
-    version='0.8.0',
+    version='0.9.0',
     zip_safe=False,
 )
```

### Comparing `releng-tool-0.8.0/tests/__init__.py` & `releng-tool-0.9.0/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,21 @@
     A utility call to return the absolute path of the "tests" directory for this
     implementation. This is to support interpreters (i.e. Python 2.7) which do
     not provide an absolute path via the `__file__` variable.
 
     Returns:
         the path
     """
-    return os.path.dirname(os.path.abspath(sys.argv[0]))
+
+    test_base = os.path.dirname(os.path.realpath(__file__))
+
+    if not os.path.exists(os.path.join(test_base, 'templates')):
+        test_base = os.path.dirname(os.path.abspath(sys.argv[0]))
+
+    return test_base
 
 class RelengToolTestSuite(unittest.TestSuite):
     def run(self, result):
         """
         a releng-tool helper test suite
 
         Provides a `unittest.TestSuite` which will ensure stdout is flushed
```

### Comparing `releng-tool-0.8.0/tests/__main__.py` & `releng-tool-0.9.0/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/support/pkg_config_test.py` & `releng-tool-0.9.0/tests/support/pkg_config_test.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/support/site_tool_test.py` & `releng-tool-0.9.0/tests/support/site_tool_test.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/tool-tests/test_tool_git.py` & `releng-tool-0.9.0/tests/tool-tests/test_tool_git.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,15 +73,23 @@
         self.defconfig_add('VERSION', first_tag)
         rv = self.engine.run()
         self.assertTrue(rv)
 
         current_hash = self._git_cache('rev-parse', 'HEAD')
         self.assertEqual(current_hash, first_hash)
 
-    def test_tool_git_custom_options(self):
+    def test_tool_git_custom_options_invalid(self):
+        self.defconfig_add('GIT_CONFIG', {
+            'bad-config-key': '',
+        })
+        self.defconfig_add('VERSION', DEFAULT_BRANCH)
+        rv = self.engine.run()
+        self.assertFalse(rv)
+
+    def test_tool_git_custom_options_valid(self):
         MY_CUSTOM_CFG = 'tmp.example'
         MY_CUSTOM_CFG_VALUE = 'my-value'
 
         self.defconfig_add('GIT_CONFIG', {
             MY_CUSTOM_CFG: MY_CUSTOM_CFG_VALUE,
         })
         self.defconfig_add('VERSION', DEFAULT_BRANCH)
@@ -184,14 +192,80 @@
         self.assertTrue(rv)
 
         current_hash = self._git_cache('rev-parse', 'HEAD')
         self.assertEqual(current_hash, commit_a)
         rev_count = self._git_cache('rev-list', '--count', 'HEAD')
         self.assertNotEqual(int(rev_count), 1)
 
+    def test_tool_git_devmode_auto_fetch_branch(self):
+        # create a new branch with a commit
+        TARGET_BRANCH = 'target'
+        self._git_repo('checkout', '-b', TARGET_BRANCH)
+        first_hash = self._create_commit('first')
+
+        # enable development mode
+        touch(self.engine.opts.ff_devmode)
+
+        # note: default state should be automatic cache-ignoring
+        #        (i.e enabled in development mode)
+
+        # fetch the target
+        self.defconfig_add('VERSION', TARGET_BRANCH)
+        rv = self.engine.run()
+        self.assertTrue(rv)
+
+        current_hash = self._git_cache('rev-parse', 'HEAD')
+        self.assertEqual(current_hash, first_hash)
+
+        # cleanup
+        self.cleanup_outdir()
+        self.engine.opts.devmode = None
+
+        # create a new commit
+        second_hash = self._create_commit('second')
+
+        # extract project; should be the second commit
+        rv = self.engine.run()
+        self.assertTrue(rv)
+
+        current_hash = self._git_cache('rev-parse', 'HEAD')
+        self.assertEqual(current_hash, second_hash)
+
+        # cleanup
+        self.cleanup_outdir()
+        self.engine.opts.devmode = None
+
+        # create a new commit
+        third_hash = self._create_commit('third')
+
+        # explicitly indicate that cache-ignoring should not happen
+        self.defconfig_add('DEVMODE_IGNORE_CACHE', False)
+        self.defconfig_dump()
+
+        # extract; should be the second commit
+        rv = self.engine.run()
+        self.assertTrue(rv)
+
+        current_hash = self._git_cache('rev-parse', 'HEAD')
+        self.assertEqual(current_hash, second_hash)
+
+        # cleanup
+        self.cleanup_outdir()
+        self.engine.opts.devmode = None
+
+        # explicitly indicate that cache-ignoring can happen
+        self.defconfig_add('DEVMODE_IGNORE_CACHE', True)
+
+        # extract; should be the third commit
+        rv = self.engine.run()
+        self.assertTrue(rv)
+
+        current_hash = self._git_cache('rev-parse', 'HEAD')
+        self.assertEqual(current_hash, third_hash)
+
     def test_tool_git_diverged_branch(self):
         # create a new branch with a commit
         TARGET_BRANCH = 'target'
         self._git_repo('checkout', '-b', TARGET_BRANCH)
         first_hash = self._create_commit('first')
 
         # fetch the target
@@ -284,15 +358,15 @@
             touch(os.path.join(repo2, 'file2'))
             self._create_commit('add file', repo=repo2, add=True)
 
             # add a submodule repo2 to repo1
             self._git_repo('submodule', 'add', repo2, 'repo2', repo=repo1)
             self._create_commit('add module', repo=repo1, add=True)
 
-            # extract package but not submodules (by defaylt)
+            # extract package but not submodules (by default)
             self.engine.opts.gbl_action = GlobalAction.EXTRACT
             rv = self.engine.run()
             self.assertTrue(rv)
 
             # verify expected content from main package; not submodules
             out_dir = os.path.join(
                 self.engine.opts.build_dir, 'test-' + DEFAULT_BRANCH)
@@ -342,14 +416,78 @@
             repo1_file = os.path.join(out_dir, 'file1')
             repo2_file = os.path.join(out_dir, 'repo2', 'file2')
             repo3_file = os.path.join(out_dir, 'repo2', 'repo3', 'file3')
             self.assertTrue(os.path.exists(repo1_file))
             self.assertTrue(os.path.exists(repo2_file))
             self.assertTrue(os.path.exists(repo3_file))
 
+    def test_tool_git_submodules_branch_revision(self):
+        self.defconfig_add('GIT_SUBMODULES', True)
+        self.defconfig_add('VERSION', DEFAULT_BRANCH)
+
+        with generate_temp_dir() as repo2:
+            # prepare additional mock repository directories
+            repo1 = self.repo_dir
+            self.prepare_repo_dir(repo2)
+
+            # dummy file on repo1
+            touch(os.path.join(repo1, 'file1'))
+            self._create_commit('add file', repo=repo1, add=True)
+
+            # dummy files on repo2 for two branches
+            CUSTOM_BRANCH = 'custom'
+
+            touch(os.path.join(repo2, 'file2'))
+            self._create_commit('add file', repo=repo2, add=True)
+
+            self._git_repo('checkout', '-b', CUSTOM_BRANCH, repo=repo2)
+
+            touch(os.path.join(repo2, 'file3'))
+            self._create_commit('add file', repo=repo2, add=True)
+
+            self._git_repo('checkout', DEFAULT_BRANCH, repo=repo2)
+
+            # add a submodule repo2 to repo1
+            self._git_repo('submodule', 'add', repo2, 'repo2', repo=repo1)
+            self._create_commit('add module', repo=repo1, add=True)
+
+            # extract package but not submodules (by default)
+            self.engine.opts.gbl_action = GlobalAction.EXTRACT
+            rv = self.engine.run()
+            self.assertTrue(rv)
+
+            # verify expected content from main package; not submodules
+            out_dir = os.path.join(
+                self.engine.opts.build_dir, 'test-' + DEFAULT_BRANCH)
+            repo1_file = os.path.join(out_dir, 'file1')
+            repo2_file = os.path.join(out_dir, 'repo2', 'file2')
+            self.assertTrue(os.path.exists(repo1_file))
+            self.assertTrue(os.path.exists(repo2_file))
+
+            # cleanup
+            self.cleanup_outdir()
+
+            # adjust submodule to target the custom branch
+            self._git_repo('config', '-f', '.gitmodules',
+                'submodule.repo2.branch', CUSTOM_BRANCH, repo=repo1)
+
+            # force a fetch (which should update the cache)
+            self.engine.opts.gbl_action = GlobalAction.FETCH
+            rv = self.engine.run()
+            self.assertTrue(rv)
+
+            # re-extract package and submodules
+            self.engine.opts.gbl_action = GlobalAction.EXTRACT
+            rv = self.engine.run()
+            self.assertTrue(rv)
+
+            # verify expected content from main package and submodules
+            repo3_file = os.path.join(out_dir, 'repo2', 'file3')
+            self.assertTrue(os.path.exists(repo3_file))
+
     def test_tool_git_unknown_branch_tag(self):
         self.defconfig_add('VERSION', 'unknown')
         rv = self.engine.run()
         self.assertFalse(rv)
 
     def test_tool_git_unknown_hash(self):
         self.defconfig_add('VERSION',
```

### Comparing `releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-c` & `releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/valid-hash-sample-c`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/assets/hash-samples/verify-success` & `releng-tool-0.9.0/tests/unit-tests/assets/hash-samples/verify-success`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/assets/shebang-interpreter/interpreter-extremely-long` & `releng-tool-0.9.0/tests/unit-tests/assets/shebang-interpreter/interpreter-extremely-long`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_engine_run_actions.py` & `releng-tool-0.9.0/tests/unit-tests/test_engine_run_actions.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_engine_run_defaults.py` & `releng-tool-0.9.0/tests/unit-tests/test_engine_run_defaults.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_engine_run_file_flags.py` & `releng-tool-0.9.0/tests/unit-tests/test_engine_run_file_flags.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_file_flags.py` & `releng-tool-0.9.0/tests/unit-tests/test_file_flags.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_configs.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_configs.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_autotools.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_autotools.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_devmode.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_devmode.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_extensions.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_extensions.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_git.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_git.py`

 * *Files 18% similar despite different names*

```diff
@@ -94,7 +94,23 @@
     def test_pkgconfig_git_submodules_invalid(self):
         with self.assertRaises(RelengToolInvalidPackageKeyValue):
             self.LOAD('git-submodules-invalid')
 
     def test_pkgconfig_git_submodules_missing(self):
         pkg, _, _ = self.LOAD('missing')
         self.assertIsNone(pkg.git_submodules)
+
+    def test_pkgconfig_git_verify_disabled(self):
+        pkg, _, _ = self.LOAD('git-verify-disabled')
+        self.assertFalse(pkg.git_verify_revision)
+
+    def test_pkgconfig_git_verify_enabled(self):
+        pkg, _, _ = self.LOAD('git-verify-enabled')
+        self.assertTrue(pkg.git_verify_revision)
+
+    def test_pkgconfig_git_verify_invalid(self):
+        with self.assertRaises(RelengToolInvalidPackageKeyValue):
+            self.LOAD('git-verify-invalid')
+
+    def test_pkgconfig_git_verify_missing(self):
+        pkg, _, _ = self.LOAD('missing')
+        self.assertIsNone(pkg.git_verify_revision)
```

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_stageopts.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_stageopts.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_type.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_type.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_configs_vcs_type.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_configs_vcs_type.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_pipeline_licenses.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_pipeline_licenses.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_pipeline_remote_cfg.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_pipeline_remote_cfg.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_pkg_pipeline_remote_scripts.py` & `releng-tool-0.9.0/tests/unit-tests/test_pkg_pipeline_remote_scripts.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_util_common.py` & `releng-tool-0.9.0/tests/unit-tests/test_util_common.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_util_env.py` & `releng-tool-0.9.0/tests/unit-tests/test_util_env.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,14 +26,28 @@
         self.assertEqual(env['a'], 1)
         self.assertEqual(env['b'], 3)
 
         # magic values are ignored
         extend_script_env(env, {'__magic__': 4})
         self.assertEqual(len(env.keys()), 2)
 
+        # imported built-in functions are ignored
+        extend_script_env(env,
+            {'test': globals()['__builtins__']['hash']})
+        self.assertEqual(len(env.keys()), 2)
+
+        # imported functions are ignored
+        extend_script_env(env,
+            {'test': globals()['extend_script_env']})
+        self.assertEqual(len(env.keys()), 2)
+
+        # imported modules are ignored
+        extend_script_env(env, {'test': globals()['unittest']})
+        self.assertEqual(len(env.keys()), 2)
+
     def test_utilenv_env_value(self):
         test_env_key = 'RELENG_TOOL_UNIT_TEST_KEY'
         test_env_val = 'NEW_VALUE'
 
         # check a (should be) empty/unset environment variable
         value = os.environ.get(test_env_key)
         self.assertIsNone(value)
```

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_util_hash.py` & `releng-tool-0.9.0/tests/unit-tests/test_util_hash.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,18 +84,17 @@
         # empty hash file provided an empty list
         file = os.path.join(samples, 'valid-hash-sample-d')
         data = load_hashes(file)
         self.assertEqual(data, [])
 
     def test_utilhash_verify(self):
         samples = self.samples_dir
-
-        # archive-specific check
         target_sample = os.path.join(samples, 'sample-asset')
 
+        # archive-specific check
         file = os.path.join(samples, 'verify-missing-archive')
         result = verify_hashes(file, target_sample, quiet=True)
         self.assertEqual(result, HashResult.MISSING_ARCHIVE)
 
         file = os.path.join(samples, 'verify-success')
         result = verify_hashes(file, target_sample, quiet=True)
         self.assertEqual(result, HashResult.VERIFIED)
@@ -124,7 +123,17 @@
         file = os.path.join(samples, 'verify-success')
         result = verify_hashes(file, samples, quiet=True)
         self.assertEqual(result, HashResult.VERIFIED)
 
         file = os.path.join(samples, 'verify-unknown-hash-type')
         result = verify_hashes(file, samples, quiet=True)
         self.assertEqual(result, HashResult.UNSUPPORTED)
+
+        # missing check
+        result = verify_hashes('', '', quiet=True)
+        self.assertEqual(result, HashResult.BAD_PATH)
+
+        # excluded/empty
+        exclude = ['sample-asset']
+        file = os.path.join(samples, 'verify-success')
+        result = verify_hashes(file, target_sample, exclude=exclude, quiet=True)
+        self.assertEqual(result, HashResult.EMPTY)
```

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_util_io.py` & `releng-tool-0.9.0/tests/unit-tests/test_util_io.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_util_sort.py` & `releng-tool-0.9.0/tests/unit-tests/test_util_sort.py`

 * *Files identical despite different names*

### Comparing `releng-tool-0.8.0/tests/unit-tests/test_util_string.py` & `releng-tool-0.9.0/tests/unit-tests/test_util_string.py`

 * *Files identical despite different names*

