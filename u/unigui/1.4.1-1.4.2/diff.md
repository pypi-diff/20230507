# Comparing `tmp/unigui-1.4.1.tar.gz` & `tmp/unigui-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.4.1.tar", last modified: Sun May  7 00:17:29 2023, max compression
+gzip compressed data, was "dist/unigui-1.4.2.tar", last modified: Sun May  7 00:26:14 2023, max compression
```

## Comparing `unigui-1.4.1.tar` & `unigui-1.4.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.1/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     7695 2023-05-03 16:32:01.000000 unigui-1.4.1/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.1/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.1/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.1/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.1/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/css/365.b8547d97.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/vendor.c0de6c67.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/193.b4cc3ffe.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/430.4be6e8a8.js
--rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/app.bfd9bd6e.js
--rw-rw-r--   0 george    (1000) george    (1000)    39843 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/365.3c494fbf.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.1/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      565 2023-05-07 00:16:30.000000 unigui-1.4.1/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-07 00:17:29.000000 unigui-1.4.1/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-07 00:17:29.000000 unigui-1.4.1/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-03 16:32:01.000000 unigui-1.4.1/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.1/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-07 00:17:28.000000 unigui-1.4.1/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-07 00:17:28.000000 unigui-1.4.1/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.1/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1194 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-07 00:17:28.000000 unigui-1.4.1/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.2/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7695 2023-05-03 16:32:01.000000 unigui-1.4.2/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.2/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.2/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.2/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.2/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/css/365.b8547d97.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/vendor.c0de6c67.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/193.b4cc3ffe.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/430.4be6e8a8.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/app.bfd9bd6e.js
+-rw-rw-r--   0 george    (1000) george    (1000)    39843 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/js/365.3c494fbf.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-07 00:13:46.000000 unigui-1.4.2/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.2/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-07 00:26:03.000000 unigui-1.4.2/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-07 00:26:14.000000 unigui-1.4.2/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-07 00:26:14.000000 unigui-1.4.2/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-03 16:32:01.000000 unigui-1.4.2/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.2/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.2/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-07 00:26:14.000000 unigui-1.4.2/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.4.1/unigui/manager.py` & `unigui-1.4.2/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/guielements.py` & `unigui-1.4.2/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/server.py` & `unigui-1.4.2/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/utils.py` & `unigui-1.4.2/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/favicon.ico` & `unigui-1.4.2/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/css/365.b8547d97.css` & `unigui-1.4.2/unigui/web/css/365.b8547d97.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.4.2/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/icons/favicon-96x96.png` & `unigui-1.4.2/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/icons/favicon-16x16.png` & `unigui-1.4.2/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/icons/favicon-32x32.png` & `unigui-1.4.2/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/icons/favicon-128x128.png` & `unigui-1.4.2/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.4.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.4.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.4.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.4.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.4.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/js/vendor.c0de6c67.js` & `unigui-1.4.2/unigui/web/js/vendor.c0de6c67.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.4.2/unigui/web/js/193.b4cc3ffe.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/js/430.4be6e8a8.js` & `unigui-1.4.2/unigui/web/js/430.4be6e8a8.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/js/app.bfd9bd6e.js` & `unigui-1.4.2/unigui/web/js/app.bfd9bd6e.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/js/365.3c494fbf.js` & `unigui-1.4.2/unigui/web/js/365.3c494fbf.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui/web/index.html` & `unigui-1.4.2/unigui/web/index.html`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/LICENSE` & `unigui-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/PKG-INFO` & `unigui-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.1
+Version: 1.4.2
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.1/README.md` & `unigui-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.4.1/unigui.egg-info/PKG-INFO` & `unigui-1.4.2/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.1
+Version: 1.4.2
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.1/unigui.egg-info/SOURCES.txt` & `unigui-1.4.2/unigui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 unigui/server.py
 unigui/userset.py
 unigui/utils.py
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
+unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
 unigui/web/css/365.b8547d97.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
```

