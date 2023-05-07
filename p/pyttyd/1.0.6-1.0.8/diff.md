# Comparing `tmp/pyttyd-1.0.6.tar.gz` & `tmp/pyttyd-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttyd-1.0.6.tar", last modified: Thu Feb 16 10:37:07 2023, max compression
+gzip compressed data, was "pyttyd-1.0.8.tar", last modified: Sun May  7 04:09:29 2023, max compression
```

## Comparing `pyttyd-1.0.6.tar` & `pyttyd-1.0.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.474586 pyttyd-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-16 10:36:49.000000 pyttyd-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-16 10:36:49.000000 pyttyd-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-02-16 10:37:07.474586 pyttyd-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-16 10:36:49.000000 pyttyd-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-16 10:36:49.000000 pyttyd-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-16 10:37:07.474586 pyttyd-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-16 10:36:49.000000 pyttyd-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.462586 pyttyd-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.466586 pyttyd-1.0.6/src/pyttyd/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/ctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/depends.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.466586 pyttyd-1.0.6/src/pyttyd/routes/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/routes/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/routes/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/routes/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.462586 pyttyd-1.0.6/src/pyttyd/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.470586 pyttyd-1.0.6/src/pyttyd/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    25682 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    23411 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    75600 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/bootstrap-theme.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   145933 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   390887 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   121457 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   540434 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/navbar-fixed-top.css
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/css/xterm.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.470586 pyttyd-1.0.6/src/pyttyd/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.470586 pyttyd-1.0.6/src/pyttyd/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    23988 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/img/index.png
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/img/link.png
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/img/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.470586 pyttyd-1.0.6/src/pyttyd/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    75484 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)    39680 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/crypt.js
--rw-r--r--   0 runner    (1001) docker     (123)   198114 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   138453 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/jquery.min.map
--rw-r--r--   0 runner    (1001) docker     (123)    57318 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/jsencrypt.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/nanoid.js
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/terminal.js
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/xterm-addon-fit.js
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/xterm-addon-fit.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   275838 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/xterm.js
--rw-r--r--   0 runner    (1001) docker     (123)  1056796 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/static/js/xterm.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.474586 pyttyd-1.0.6/src/pyttyd/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/template/content1.html
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/template/content2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/template/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.474586 pyttyd-1.0.6/src/pyttyd/template/modal/
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/template/modal/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/template/modal/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/template/terminal.html
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.474586 pyttyd-1.0.6/src/pyttyd/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-16 10:36:49.000000 pyttyd-1.0.6/src/pyttyd/test/test_rsa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 10:37:07.466586 pyttyd-1.0.6/src/pyttyd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-02-16 10:37:07.000000 pyttyd-1.0.6/src/pyttyd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-02-16 10:37:07.000000 pyttyd-1.0.6/src/pyttyd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 10:37:07.000000 pyttyd-1.0.6/src/pyttyd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-16 10:37:07.000000 pyttyd-1.0.6/src/pyttyd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-16 10:37:07.000000 pyttyd-1.0.6/src/pyttyd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-16 10:37:07.000000 pyttyd-1.0.6/src/pyttyd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.270550 pyttyd-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 04:09:11.000000 pyttyd-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-07 04:09:11.000000 pyttyd-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-07 04:09:29.270550 pyttyd-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-07 04:09:11.000000 pyttyd-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-07 04:09:11.000000 pyttyd-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-07 04:09:29.270550 pyttyd-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-07 04:09:11.000000 pyttyd-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.254550 pyttyd-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.258550 pyttyd-1.0.8/src/pyttyd/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/ctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/depends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.262550 pyttyd-1.0.8/src/pyttyd/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/routes/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/routes/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/routes/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.258550 pyttyd-1.0.8/src/pyttyd/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.262550 pyttyd-1.0.8/src/pyttyd/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    25682 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    23411 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    75600 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   145933 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   390887 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   121457 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   540434 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/navbar-fixed-top.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/css/xterm.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.262550 pyttyd-1.0.8/src/pyttyd/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.266550 pyttyd-1.0.8/src/pyttyd/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    23988 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/img/index.png
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/img/link.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/img/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.266550 pyttyd-1.0.8/src/pyttyd/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    75484 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39680 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/crypt.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198114 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   138453 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/jquery.min.map
+-rw-r--r--   0 runner    (1001) docker     (123)    57318 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/jsencrypt.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/nanoid.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/terminal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/xterm-addon-fit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/xterm-addon-fit.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   275838 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/xterm.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1056796 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/static/js/xterm.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.270550 pyttyd-1.0.8/src/pyttyd/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/template/content1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/template/content2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/template/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.270550 pyttyd-1.0.8/src/pyttyd/template/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/template/modal/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/template/modal/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/template/terminal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.270550 pyttyd-1.0.8/src/pyttyd/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-07 04:09:11.000000 pyttyd-1.0.8/src/pyttyd/test/test_rsa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:09:29.258550 pyttyd-1.0.8/src/pyttyd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-07 04:09:29.000000 pyttyd-1.0.8/src/pyttyd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-07 04:09:29.000000 pyttyd-1.0.8/src/pyttyd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:09:29.000000 pyttyd-1.0.8/src/pyttyd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-07 04:09:29.000000 pyttyd-1.0.8/src/pyttyd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 04:09:29.000000 pyttyd-1.0.8/src/pyttyd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 04:09:29.000000 pyttyd-1.0.8/src/pyttyd.egg-info/top_level.txt
```

### Comparing `pyttyd-1.0.6/LICENSE` & `pyttyd-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/PKG-INFO` & `pyttyd-1.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttyd
-Version: 1.0.6
+Version: 1.0.8
 Summary: devtool show by browser
 Home-page: https://zhanglaiya.github.io/
 Author: zhanglaiya
 Author-email: 315396460@qq.com
 Maintainer: zhanglaiya
 Maintainer-email: 315396460@qq.com
 License: Apache
@@ -38,27 +38,14 @@
 ```
 
 浏览器打开[http://127.0.0.1:8221](http://127.0.0.1:8221)
 
 ![](./src/pyttyd/static/img/index.png)
 ![](./src/pyttyd/static/img/terminal.png)
 
-### pyttyctl
-
-```commandline
-$ pyttyctl list
-ID               连接名称      主机       端口   用户名   密码      创建时间             更新时间           
-d4c19a0bbdc44fb  我爱北天安门  127.0.0.1  2222   root    ****  2023-01-28 06:11:36  2023-02-13 07:03:10
-626bab7b8239488  1111         127.0.0.1  2223   root    ****  2023-01-30 03:37:50  2023-02-01 08:25:46
-$ pyttyctl conn d4c19a0bbdc44fb
-Last login: Tue Feb 01 00:00:00 2023 from 172.29.0.1
-root@a7272ab29048:~# pwd
-/root
-root@a7272ab29048:~# 
-```
 感谢！！！  
 [@bootstrap](https://getbootstrap.com/docs/3.4/)  
 [@paramiko](https://github.com/paramiko/paramiko)  
 [@FastApi](https://github.com/tiangolo/fastapi)  
 [@Jinja2](https://github.com/pallets/jinja)  
 [@cryptography](https://github.com/pyca/cryptography)  
 [@JSEncrypt](https://github.com/travist/jsencrypt)
```

### Comparing `pyttyd-1.0.6/setup.cfg` & `pyttyd-1.0.8/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	pyttyd = pyttyd.__main__:main
-	pyttyctl = pyttyd.__main__:ctl
 
 [tool:pytest]
 testpaths = tests
 filterwarnings = 
 	error
 
 [coverage:run]
```

### Comparing `pyttyd-1.0.6/src/pyttyd/crud.py` & `pyttyd-1.0.8/src/pyttyd/crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,32 @@
                 or_(
                     tb_ssh_connect.c.name.contains(q),
                     tb_ssh_connect.c.host.contains(q),
                     tb_ssh_connect.c.user.contains(q),
                 )
             )
         res = conn.execute(stmt)
-        data = res.fetchone()
-    return ('id', 'name', 'host', 'port', 'user', 'password', 'create_time', 'update_time'), data
+        data = res.mappings().fetchone()
+    return data
 
 
 def get_conns(q=None):
     with engine.connect() as conn:
         stmt = select(tb_ssh_connect)
         if q is not None:
             stmt = stmt.where(
                 or_(
                     tb_ssh_connect.c.name.contains(q),
                     tb_ssh_connect.c.host.contains(q),
                     tb_ssh_connect.c.user.contains(q),
                 )
             )
         res = conn.execute(stmt)
-        data = res.fetchall()
-    return ('id', 'name', 'host', 'port', 'user', 'password', 'create_time', 'update_time'), data
+        data = res.mappings().fetchall()
+    return data
 
 
 def create_conn(item):
     with engine.connect() as conn:
         result = conn.execute(
             insert(tb_ssh_connect).values(
                 id=uuid.uuid4().hex,
@@ -48,26 +48,29 @@
                 host=item['host'],
                 port=item['port'],
                 user=item['user'],
                 password=item['password']
             )
         )
         lastrowid = result.lastrowid
+        conn.commit()
     return lastrowid
 
 
 def update_conn(item):
     with engine.connect() as conn:
         result = conn.execute(update(tb_ssh_connect).where(tb_ssh_connect.c.id == item['id']).values(
             name=item['name'],
             host=item['host'],
             port=item['port'],
             user=item['user'],
             password=item['password']
         ))
         rowcount = result.rowcount
+        conn.commit()
     return rowcount
 
 
 def delete_conn(item):
     with engine.connect() as conn:
         conn.execute(delete(tb_ssh_connect).where(tb_ssh_connect.c.id == item['id']))
+        conn.commit()
```

### Comparing `pyttyd-1.0.6/src/pyttyd/crypto.py` & `pyttyd-1.0.8/src/pyttyd/crypto.py`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/depends.py` & `pyttyd-1.0.8/src/pyttyd/depends.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def decrypt(self, encrypted):
         return self._cryptor.decrypt(encrypted)
 
     def encrypt(self, src):
         return self._cryptor.encrypt(src)
 
 
-def to_dict(keys, values):
+def to_dict(row):
     dct = {}
-    for i, k in enumerate(keys):
-        if isinstance(values[i], datetime.datetime):
-            dct[k] = values[i].strftime('%Y-%m-%d %H:%M:%S')
+    for k, v in row.items():
+        if isinstance(v, datetime.datetime):
+            dct[k] = v.strftime('%Y-%m-%d %H:%M:%S')
         else:
-            dct[k] = values[i]
+            dct[k] = v
     return dct
```

### Comparing `pyttyd-1.0.6/src/pyttyd/model.py` & `pyttyd-1.0.8/src/pyttyd/model.py`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/routes/html.py` & `pyttyd-1.0.8/src/pyttyd/routes/html.py`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/routes/ssh.py` & `pyttyd-1.0.8/src/pyttyd/routes/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,27 @@
     return name
 
 
 @router.get("/", response_model=CommonResponse)
 async def ssh(q: str = None, cryptor: CryptoDepend = Depends(CryptoDepend)):
     if cryptor.token:
         ssh_id = cryptor.decrypt(cryptor.token)
-        data = crud.get_conn(ssh_id, q=q)
-        dct = to_dict(*data)
-        dct['ellipsis'] = _ellipsis(dct['name'])
+        dct = crud.get_conn(ssh_id, q=q)
+        data = to_dict(dct)
+        data['ellipsis'] = _ellipsis(data['name'])
 
     else:
-        data = crud.get_conns(q=q)
-        dct = [to_dict(data[0], vs) for vs in data[1]]
+        lst = crud.get_conns(q=q)
+        data = [to_dict(row) for row in lst]
 
-        for i in dct:
-            i['ellipsis'] = _ellipsis(i['name'])
+        for dct in data:
+            dct['ellipsis'] = _ellipsis(dct['name'])
 
     return {
-        'data': cryptor.encrypt(json.dumps(dct).encode())
+        'data': cryptor.encrypt(json.dumps(data).encode())
     }
 
 
 @router.post("/", response_model=CommonResponse)
 async def ssh(*, cryptor: CryptoDepend = Depends(CryptoDepend)):
 
     # data = cryptor.decrypt(cryptor.token)
```

### Comparing `pyttyd-1.0.6/src/pyttyd/routes/terminal.py` & `pyttyd-1.0.8/src/pyttyd/routes/terminal.py`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/bootstrap-theme.css` & `pyttyd-1.0.8/src/pyttyd/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/bootstrap-theme.css.map` & `pyttyd-1.0.8/src/pyttyd/static/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/bootstrap-theme.min.css` & `pyttyd-1.0.8/src/pyttyd/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/bootstrap-theme.min.css.map` & `pyttyd-1.0.8/src/pyttyd/static/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/bootstrap.css` & `pyttyd-1.0.8/src/pyttyd/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/bootstrap.css.map` & `pyttyd-1.0.8/src/pyttyd/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/bootstrap.min.css` & `pyttyd-1.0.8/src/pyttyd/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/bootstrap.min.css.map` & `pyttyd-1.0.8/src/pyttyd/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/css/xterm.css` & `pyttyd-1.0.8/src/pyttyd/static/css/xterm.css`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.eot` & `pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.svg` & `pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.ttf` & `pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.woff` & `pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/fonts/glyphicons-halflings-regular.woff2` & `pyttyd-1.0.8/src/pyttyd/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/img/favicon-32x32.png` & `pyttyd-1.0.8/src/pyttyd/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/img/favicon.ico` & `pyttyd-1.0.8/src/pyttyd/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/img/index.png` & `pyttyd-1.0.8/src/pyttyd/static/img/index.png`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/img/terminal.png` & `pyttyd-1.0.8/src/pyttyd/static/img/terminal.png`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/bootstrap.js` & `pyttyd-1.0.8/src/pyttyd/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/bootstrap.min.js` & `pyttyd-1.0.8/src/pyttyd/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/clipboard.min.js` & `pyttyd-1.0.8/src/pyttyd/static/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/crypt.js` & `pyttyd-1.0.8/src/pyttyd/static/js/crypt.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/crypto-js.js` & `pyttyd-1.0.8/src/pyttyd/static/js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/index.js` & `pyttyd-1.0.8/src/pyttyd/static/js/index.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/jquery.min.js` & `pyttyd-1.0.8/src/pyttyd/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/jquery.min.map` & `pyttyd-1.0.8/src/pyttyd/static/js/jquery.min.map`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/jsencrypt.min.js` & `pyttyd-1.0.8/src/pyttyd/static/js/jsencrypt.min.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/terminal.js` & `pyttyd-1.0.8/src/pyttyd/static/js/terminal.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/xterm-addon-fit.js` & `pyttyd-1.0.8/src/pyttyd/static/js/xterm-addon-fit.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/xterm-addon-fit.js.map` & `pyttyd-1.0.8/src/pyttyd/static/js/xterm-addon-fit.js.map`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/xterm.js` & `pyttyd-1.0.8/src/pyttyd/static/js/xterm.js`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/static/js/xterm.js.map` & `pyttyd-1.0.8/src/pyttyd/static/js/xterm.js.map`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/template/content1.html` & `pyttyd-1.0.8/src/pyttyd/template/content1.html`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/template/content2.html` & `pyttyd-1.0.8/src/pyttyd/template/content2.html`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/template/index.html` & `pyttyd-1.0.8/src/pyttyd/template/index.html`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/template/modal/edit.html` & `pyttyd-1.0.8/src/pyttyd/template/modal/edit.html`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/template/modal/new.html` & `pyttyd-1.0.8/src/pyttyd/template/modal/new.html`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/template/terminal.html` & `pyttyd-1.0.8/src/pyttyd/template/terminal.html`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd/terminal.py` & `pyttyd-1.0.8/src/pyttyd/terminal.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,18 @@
             )
             for task in pending:
                 task.cancel()
 
     async def read_chan(self, chan):
         while not chan.closed:
             try:
-                data = await asyncio.to_thread(chan.recv, 1024)
+                if hasattr(asyncio, 'to_thread'):
+                    data = await asyncio.to_thread(chan.recv, 1024)
+                else:
+                    data = await asyncio.get_running_loop().run_in_executor(None, chan.recv, 1024)
                 # print('chan.recv: ', data)
             except Exception as e:
                 logging.error('chan.recv error', exc_info=e)
                 await self._ws.close(reason=str(e))
                 break
             if data:
                 await self._ws.send_text(data.decode(self._encoding))
```

### Comparing `pyttyd-1.0.6/src/pyttyd/test/test_rsa.py` & `pyttyd-1.0.8/src/pyttyd/test/test_rsa.py`

 * *Files identical despite different names*

### Comparing `pyttyd-1.0.6/src/pyttyd.egg-info/PKG-INFO` & `pyttyd-1.0.8/src/pyttyd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttyd
-Version: 1.0.6
+Version: 1.0.8
 Summary: devtool show by browser
 Home-page: https://zhanglaiya.github.io/
 Author: zhanglaiya
 Author-email: 315396460@qq.com
 Maintainer: zhanglaiya
 Maintainer-email: 315396460@qq.com
 License: Apache
@@ -38,27 +38,14 @@
 ```
 
 浏览器打开[http://127.0.0.1:8221](http://127.0.0.1:8221)
 
 ![](./src/pyttyd/static/img/index.png)
 ![](./src/pyttyd/static/img/terminal.png)
 
-### pyttyctl
-
-```commandline
-$ pyttyctl list
-ID               连接名称      主机       端口   用户名   密码      创建时间             更新时间           
-d4c19a0bbdc44fb  我爱北天安门  127.0.0.1  2222   root    ****  2023-01-28 06:11:36  2023-02-13 07:03:10
-626bab7b8239488  1111         127.0.0.1  2223   root    ****  2023-01-30 03:37:50  2023-02-01 08:25:46
-$ pyttyctl conn d4c19a0bbdc44fb
-Last login: Tue Feb 01 00:00:00 2023 from 172.29.0.1
-root@a7272ab29048:~# pwd
-/root
-root@a7272ab29048:~# 
-```
 感谢！！！  
 [@bootstrap](https://getbootstrap.com/docs/3.4/)  
 [@paramiko](https://github.com/paramiko/paramiko)  
 [@FastApi](https://github.com/tiangolo/fastapi)  
 [@Jinja2](https://github.com/pallets/jinja)  
 [@cryptography](https://github.com/pyca/cryptography)  
 [@JSEncrypt](https://github.com/travist/jsencrypt)
```

### Comparing `pyttyd-1.0.6/src/pyttyd.egg-info/SOURCES.txt` & `pyttyd-1.0.8/src/pyttyd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

