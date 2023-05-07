# Comparing `tmp/dorado-2.0.6.dev97.tar.gz` & `tmp/dorado-2.0.6.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorado-2.0.6.dev97.tar", last modified: Mon Mar 27 21:01:46 2023, max compression
+gzip compressed data, was "dorado-2.0.6.dev99.tar", last modified: Mon Mar 27 21:20:41 2023, max compression
```

## Comparing `dorado-2.0.6.dev97.tar` & `dorado-2.0.6.dev99.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.253708 dorado-2.0.6.dev97/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      833 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/.gitignore
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      185 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/.readthedocs.yml
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.241707 dorado-2.0.6.dev97/.vscode/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      160 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/.vscode/settings.json
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2875 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/CHANGES.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      312 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/MANIFEST.in
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      432 2023-03-27 21:01:46.257708 dorado-2.0.6.dev97/PKG-INFO
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     6187 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/README.rst
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.245708 dorado-2.0.6.dev97/docs/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     4714 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/Makefile
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     7362 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/conf.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.245708 dorado-2.0.6.dev97/docs/dorado/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2908 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/GettingStarted.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     6187 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/README.rst
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.245708 dorado-2.0.6.dev97/docs/dorado/_static/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    32286 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/_static/clippy.jfif
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    32286 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/_static/clippy.png
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2990 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/ceres.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     5130 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/core.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1844 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/dorphot.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     5127 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/filer.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)        0 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/graphing.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     6386 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/index.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     4016 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/puttingItTogether.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2887 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/reader.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       96 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/stack.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2181 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/target.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)        0 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/dorado/timeseries.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2038 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/index.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     4721 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/docs/make.bat
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.249708 dorado-2.0.6.dev97/dorado/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      922 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/__init__.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1851 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/_astropy_init.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.249708 dorado-2.0.6.dev97/dorado/ceres/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      303 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/ceres/__init__.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     6066 2023-03-15 17:27:34.000000 dorado-2.0.6.dev97/dorado/ceres/ceresClass.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2006 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/conftest.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.249708 dorado-2.0.6.dev97/dorado/core/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      361 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/core/__init__.py
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)    22761 2023-03-15 17:24:16.000000 dorado-2.0.6.dev97/dorado/core/coreClass.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    18572 2023-03-15 18:11:37.000000 dorado-2.0.6.dev97/dorado/core/readerClass.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.249708 dorado-2.0.6.dev97/dorado/dorphot/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      307 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/dorphot/__init__.py
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)    38399 2023-03-27 20:54:56.000000 dorado-2.0.6.dev97/dorado/dorphot/dorphotClass.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.253708 dorado-2.0.6.dev97/dorado/graf/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      303 2023-02-03 17:54:02.000000 dorado-2.0.6.dev97/dorado/graf/__init__.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     9895 2023-03-27 21:01:19.000000 dorado-2.0.6.dev97/dorado/graf/grafClass.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    41837 2023-03-18 21:59:25.000000 dorado-2.0.6.dev97/dorado/graf/style.mplstyle
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.253708 dorado-2.0.6.dev97/dorado/stack/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       76 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/stack/__init__.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     3961 2023-03-15 20:04:29.000000 dorado-2.0.6.dev97/dorado/stack/stackClass.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.253708 dorado-2.0.6.dev97/dorado/target/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       74 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/target/__init__.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    16117 2023-03-11 19:58:24.000000 dorado-2.0.6.dev97/dorado/target/targetClass.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.253708 dorado-2.0.6.dev97/dorado/tests/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      112 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/tests/__init__.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      504 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/tests/pollution.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      369 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/tests/test_example.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.253708 dorado-2.0.6.dev97/dorado/timeseries/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       84 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/timeseries/__init__.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     3709 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/dorado/timeseries/timeseriesClass.py
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)      343 2023-03-27 21:01:46.000000 dorado-2.0.6.dev97/dorado/version.py
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.249708 dorado-2.0.6.dev97/dorado.egg-info/
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)      432 2023-03-27 21:01:46.000000 dorado-2.0.6.dev97/dorado.egg-info/PKG-INFO
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)     1463 2023-03-27 21:01:46.000000 dorado-2.0.6.dev97/dorado.egg-info/SOURCES.txt
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)        1 2023-03-27 21:01:46.000000 dorado-2.0.6.dev97/dorado.egg-info/dependency_links.txt
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)       20 2023-03-27 21:01:46.000000 dorado-2.0.6.dev97/dorado.egg-info/entry_points.txt
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)        1 2023-01-13 22:40:54.000000 dorado-2.0.6.dev97/dorado.egg-info/not-zip-safe
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)      147 2023-03-27 21:01:46.000000 dorado-2.0.6.dev97/dorado.egg-info/requires.txt
--rw-r--r--   0 mucephie  (1000) mucephie  (1000)        7 2023-03-27 21:01:46.000000 dorado-2.0.6.dev97/dorado.egg-info/top_level.txt
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       43 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/draco.code-workspace
-drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:01:46.253708 dorado-2.0.6.dev97/licenses/
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1494 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/licenses/LICENSE.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      381 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/licenses/README.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1690 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/licenses/TEMPLATE_LICENCE.rst
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      246 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/pyproject.toml
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1499 2023-03-27 21:01:46.257708 dorado-2.0.6.dev97/setup.cfg
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2499 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/setup.py
--rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2779 2022-11-17 21:26:14.000000 dorado-2.0.6.dev97/tox.ini
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.931638 dorado-2.0.6.dev99/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      833 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/.gitignore
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      185 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/.readthedocs.yml
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.907638 dorado-2.0.6.dev99/.vscode/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      160 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/.vscode/settings.json
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2875 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/CHANGES.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      312 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/MANIFEST.in
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      432 2023-03-27 21:20:41.931638 dorado-2.0.6.dev99/PKG-INFO
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     6187 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/README.rst
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.907638 dorado-2.0.6.dev99/docs/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     4714 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/Makefile
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     7362 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/conf.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.911638 dorado-2.0.6.dev99/docs/dorado/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2908 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/GettingStarted.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     6187 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/README.rst
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.911638 dorado-2.0.6.dev99/docs/dorado/_static/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    32286 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/_static/clippy.jfif
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    32286 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/_static/clippy.png
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2990 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/ceres.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     5130 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/core.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1844 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/dorphot.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     5127 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/filer.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)        0 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/graphing.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     6386 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/index.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     4016 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/puttingItTogether.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2887 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/reader.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       96 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/stack.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2181 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/target.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)        0 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/dorado/timeseries.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2038 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/index.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     4721 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/docs/make.bat
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.911638 dorado-2.0.6.dev99/dorado/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      922 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/__init__.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1851 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/_astropy_init.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.915638 dorado-2.0.6.dev99/dorado/ceres/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      303 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/ceres/__init__.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     6066 2023-03-15 17:27:34.000000 dorado-2.0.6.dev99/dorado/ceres/ceresClass.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2006 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/conftest.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.919638 dorado-2.0.6.dev99/dorado/core/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      361 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/core/__init__.py
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)    22761 2023-03-15 17:24:16.000000 dorado-2.0.6.dev99/dorado/core/coreClass.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    18572 2023-03-15 18:11:37.000000 dorado-2.0.6.dev99/dorado/core/readerClass.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.919638 dorado-2.0.6.dev99/dorado/dorphot/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      307 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/dorphot/__init__.py
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)    38667 2023-03-27 21:19:32.000000 dorado-2.0.6.dev99/dorado/dorphot/dorphotClass.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.923638 dorado-2.0.6.dev99/dorado/graf/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      303 2023-02-03 17:54:02.000000 dorado-2.0.6.dev99/dorado/graf/__init__.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     9895 2023-03-27 21:12:44.000000 dorado-2.0.6.dev99/dorado/graf/grafClass.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    41837 2023-03-18 21:59:25.000000 dorado-2.0.6.dev99/dorado/graf/style.mplstyle
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.923638 dorado-2.0.6.dev99/dorado/stack/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       76 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/stack/__init__.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     3961 2023-03-15 20:04:29.000000 dorado-2.0.6.dev99/dorado/stack/stackClass.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.923638 dorado-2.0.6.dev99/dorado/target/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       74 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/target/__init__.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)    16117 2023-03-11 19:58:24.000000 dorado-2.0.6.dev99/dorado/target/targetClass.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.927638 dorado-2.0.6.dev99/dorado/tests/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      112 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/tests/__init__.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      504 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/tests/pollution.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      369 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/tests/test_example.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.927638 dorado-2.0.6.dev99/dorado/timeseries/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       84 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/timeseries/__init__.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     3709 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/dorado/timeseries/timeseriesClass.py
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)      343 2023-03-27 21:20:41.000000 dorado-2.0.6.dev99/dorado/version.py
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.915638 dorado-2.0.6.dev99/dorado.egg-info/
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)      432 2023-03-27 21:20:41.000000 dorado-2.0.6.dev99/dorado.egg-info/PKG-INFO
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)     1463 2023-03-27 21:20:41.000000 dorado-2.0.6.dev99/dorado.egg-info/SOURCES.txt
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)        1 2023-03-27 21:20:41.000000 dorado-2.0.6.dev99/dorado.egg-info/dependency_links.txt
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)       20 2023-03-27 21:20:41.000000 dorado-2.0.6.dev99/dorado.egg-info/entry_points.txt
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)        1 2023-01-13 22:40:54.000000 dorado-2.0.6.dev99/dorado.egg-info/not-zip-safe
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)      147 2023-03-27 21:20:41.000000 dorado-2.0.6.dev99/dorado.egg-info/requires.txt
+-rw-r--r--   0 mucephie  (1000) mucephie  (1000)        7 2023-03-27 21:20:41.000000 dorado-2.0.6.dev99/dorado.egg-info/top_level.txt
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)       43 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/draco.code-workspace
+drwxrwxr-x   0 mucephie  (1000) mucephie  (1000)        0 2023-03-27 21:20:41.931638 dorado-2.0.6.dev99/licenses/
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1494 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/licenses/LICENSE.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      381 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/licenses/README.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1690 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/licenses/TEMPLATE_LICENCE.rst
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)      246 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/pyproject.toml
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     1499 2023-03-27 21:20:41.931638 dorado-2.0.6.dev99/setup.cfg
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2499 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/setup.py
+-rw-rw-r--   0 mucephie  (1000) mucephie  (1000)     2779 2022-11-17 21:26:14.000000 dorado-2.0.6.dev99/tox.ini
```

### Comparing `dorado-2.0.6.dev97/.gitignore` & `dorado-2.0.6.dev99/.gitignore`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/CHANGES.rst` & `dorado-2.0.6.dev99/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/README.rst` & `dorado-2.0.6.dev99/README.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/Makefile` & `dorado-2.0.6.dev99/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/conf.py` & `dorado-2.0.6.dev99/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/GettingStarted.rst` & `dorado-2.0.6.dev99/docs/dorado/GettingStarted.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/README.rst` & `dorado-2.0.6.dev99/docs/dorado/README.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/_static/clippy.jfif` & `dorado-2.0.6.dev99/docs/dorado/_static/clippy.jfif`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/_static/clippy.png` & `dorado-2.0.6.dev99/docs/dorado/_static/clippy.png`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/ceres.rst` & `dorado-2.0.6.dev99/docs/dorado/ceres.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/core.rst` & `dorado-2.0.6.dev99/docs/dorado/core.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/dorphot.rst` & `dorado-2.0.6.dev99/docs/dorado/dorphot.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/filer.rst` & `dorado-2.0.6.dev99/docs/dorado/filer.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/index.rst` & `dorado-2.0.6.dev99/docs/dorado/index.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/puttingItTogether.rst` & `dorado-2.0.6.dev99/docs/dorado/puttingItTogether.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/reader.rst` & `dorado-2.0.6.dev99/docs/dorado/reader.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/dorado/target.rst` & `dorado-2.0.6.dev99/docs/dorado/target.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/index.rst` & `dorado-2.0.6.dev99/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/docs/make.bat` & `dorado-2.0.6.dev99/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/__init__.py` & `dorado-2.0.6.dev99/dorado/__init__.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/_astropy_init.py` & `dorado-2.0.6.dev99/dorado/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/ceres/ceresClass.py` & `dorado-2.0.6.dev99/dorado/ceres/ceresClass.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/conftest.py` & `dorado-2.0.6.dev99/dorado/conftest.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/core/coreClass.py` & `dorado-2.0.6.dev99/dorado/core/coreClass.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/core/readerClass.py` & `dorado-2.0.6.dev99/dorado/core/readerClass.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/dorphot/dorphotClass.py` & `dorado-2.0.6.dev99/dorado/dorphot/dorphotClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -743,16 +743,20 @@
         self.stars['aperture_sum_raw'] = np.zeros(len(self.stars))
         self.stars['inst_mag_raw'] = np.zeros(len(self.stars))
         for i in range(len(self.stars)):
             pos = (self.stars[i]['x'], self.stars[i]['y'])
             # TODO :: why is there no annulus? seriously, this is basic photometry
             # and I haven't even made an annulus aperture. pathetic
             shape = float(1.2 * self.stars[i]['detection_r']) # its possible this was handing back a row instead of a float
+            if len(self.stars[i]['detection_r']) > 1:            
+                print('more than one value encountered', len(self.stars[i]['detection_r']))
+            if shape <= 0:
+                print('negative or zero shape encountered', shape)
             aperture = CircularAperture(pos, r=shape)
-            annulus_aperture = CircularAnnulus(pos, r_in = (shape + 2), r_out = (shape + 5))
+            annulus_aperture = CircularAnnulus(positions = pos, r_in = (shape + 2), r_out = (shape + 5))
             apers = [aperture, annulus_aperture]
             phot_table = aperture_photometry(self.image.data, apers)
             bkg_mean = phot_table['aperture_sum_1'] / annulus_aperture.area
             bkg_sum = bkg_mean * aperture.area
             self.stars[i]['aperture_sum_raw'] = phot_table['aperture_sum_0']
             self.stars[i]['aperture_sum'] = phot_table['aperture_sum_0'] - bkg_sum
             self.stars[i]['inst_mag_raw'] = mag(phot_table['aperture_sum_0'], self.exp)
```

### Comparing `dorado-2.0.6.dev97/dorado/graf/grafClass.py` & `dorado-2.0.6.dev99/dorado/graf/grafClass.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -81,18 +81,18 @@
     "savefig.dpi": 72,
 }
 color_cycle = np.flip([
     "#EEFC75",  # Cantelope
     "#BDFD23",  # limish yellow green
     "#F8E604",  # lemon
     "#FDD023",  # bumble bee yellow
-    "#FF6700",  # tangerine
     "#FB9062",  # pink peach
     "#FF9248",  # peach
     "#FF4E50",  # watermelon red
+    "#FF6700",  # tangerine
     "#D41501",  # Red
     "#602320",  # burgandy
     "#280202"
 ])  # Dark
 
 try:
     # This is a dependency of matplotlib, so should be present if matplotlib
```

### Comparing `dorado-2.0.6.dev97/dorado/graf/style.mplstyle` & `dorado-2.0.6.dev99/dorado/graf/style.mplstyle`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/stack/stackClass.py` & `dorado-2.0.6.dev99/dorado/stack/stackClass.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/target/targetClass.py` & `dorado-2.0.6.dev99/dorado/target/targetClass.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado/timeseries/timeseriesClass.py` & `dorado-2.0.6.dev99/dorado/timeseries/timeseriesClass.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/dorado.egg-info/SOURCES.txt` & `dorado-2.0.6.dev99/dorado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/licenses/LICENSE.rst` & `dorado-2.0.6.dev99/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/licenses/TEMPLATE_LICENCE.rst` & `dorado-2.0.6.dev99/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/setup.cfg` & `dorado-2.0.6.dev99/setup.cfg`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/setup.py` & `dorado-2.0.6.dev99/setup.py`

 * *Files identical despite different names*

### Comparing `dorado-2.0.6.dev97/tox.ini` & `dorado-2.0.6.dev99/tox.ini`

 * *Files identical despite different names*

