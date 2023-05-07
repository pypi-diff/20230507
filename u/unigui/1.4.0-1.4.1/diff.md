# Comparing `tmp/unigui-1.4.0.tar.gz` & `tmp/unigui-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.4.0.tar", last modified: Fri May  5 20:46:42 2023, max compression
+gzip compressed data, was "dist/unigui-1.4.1.tar", last modified: Sun May  7 00:17:29 2023, max compression
```

## Comparing `unigui-1.4.0.tar` & `unigui-1.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.0/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     7695 2023-05-03 16:32:01.000000 unigui-1.4.0/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.0/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.0/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.0/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.0/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/css/702.ee87c168.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/vendor.c0de6c67.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/app.b57ab5bb.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/193.b4cc3ffe.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/430.4be6e8a8.js
--rw-rw-r--   0 george    (1000) george    (1000)    39968 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/702.aec0d6a9.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.0/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      565 2023-05-05 20:46:11.000000 unigui-1.4.0/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-05 20:46:42.000000 unigui-1.4.0/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-05 20:46:42.000000 unigui-1.4.0/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-03 16:32:01.000000 unigui-1.4.0/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.0/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.0/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1194 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.1/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7695 2023-05-03 16:32:01.000000 unigui-1.4.1/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.1/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.1/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.1/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.1/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/css/365.b8547d97.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/vendor.c0de6c67.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/193.b4cc3ffe.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/430.4be6e8a8.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/app.bfd9bd6e.js
+-rw-rw-r--   0 george    (1000) george    (1000)    39843 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/js/365.3c494fbf.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-07 00:13:46.000000 unigui-1.4.1/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.1/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      565 2023-05-07 00:16:30.000000 unigui-1.4.1/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-07 00:17:29.000000 unigui-1.4.1/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-07 00:17:29.000000 unigui-1.4.1/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-03 16:32:01.000000 unigui-1.4.1/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.1/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-07 00:17:28.000000 unigui-1.4.1/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-07 00:17:28.000000 unigui-1.4.1/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.1/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1194 2023-05-07 00:17:29.000000 unigui-1.4.1/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-07 00:17:28.000000 unigui-1.4.1/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.4.0/unigui/manager.py` & `unigui-1.4.1/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/guielements.py` & `unigui-1.4.1/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/server.py` & `unigui-1.4.1/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/utils.py` & `unigui-1.4.1/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/favicon.ico` & `unigui-1.4.1/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/css/702.ee87c168.css` & `unigui-1.4.1/unigui/web/css/365.b8547d97.css`

 * *Files 24% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-0440fa69]{display:flex;justify-content:center}.custom-caption[data-v-0440fa69]{padding:5px!important}.web-camera-container[data-v-0440fa69]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-0440fa69]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-0440fa69]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-0440fa69]{opacity:1}.web-camera-container .camera-shoot[data-v-0440fa69]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-0440fa69]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-0440fa69]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-0440fa69]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-0440fa69]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-0440fa69]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-0440fa69]{animation:preload-0440fa69 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-0440fa69]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-0440fa69]:nth-child(3){animation-delay:.4s}@keyframes preload-0440fa69{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-0440fa69]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-7cd4ac4c]{display:flex;justify-content:center}.custom-caption[data-v-7cd4ac4c]{padding:5px!important}.web-camera-container[data-v-7cd4ac4c]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-7cd4ac4c]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-7cd4ac4c]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-7cd4ac4c]{opacity:1}.web-camera-container .camera-shoot[data-v-7cd4ac4c]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-7cd4ac4c]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-7cd4ac4c]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-7cd4ac4c]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-7cd4ac4c]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-7cd4ac4c]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-7cd4ac4c]{animation:preload-7cd4ac4c 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-7cd4ac4c]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-7cd4ac4c]:nth-child(3){animation-delay:.4s}@keyframes preload-7cd4ac4c{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-7cd4ac4c]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.4.0/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.4.1/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/icons/favicon-96x96.png` & `unigui-1.4.1/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/icons/favicon-16x16.png` & `unigui-1.4.1/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/icons/favicon-32x32.png` & `unigui-1.4.1/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/icons/favicon-128x128.png` & `unigui-1.4.1/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.4.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.4.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.4.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.4.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.4.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/js/vendor.c0de6c67.js` & `unigui-1.4.1/unigui/web/js/vendor.c0de6c67.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/js/app.b57ab5bb.js` & `unigui-1.4.1/unigui/web/js/app.bfd9bd6e.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(702)]).then(r.bind(r, 9702)),
+                        component: () => Promise.all([r.e(736), r.e(365)]).then(r.bind(r, 365)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -44,30 +44,30 @@
                                     top: 0
                                 }),
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
-                async function g(e, t) {
+                async function b(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
                         n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
-                var b = r(6417),
+                var g = r(6417),
                     y = r(5597);
                 const w = {
                         config: {
                             notify: {}
                         },
                         plugins: {
-                            Notify: b.Z,
+                            Notify: g.Z,
                             Dialog: y.Z
                         }
                     },
                     O = "";
                 async function k({
                     app: e,
                     router: t
@@ -94,15 +94,15 @@
                             urlPath: i,
                             publicPath: O
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== n && (e.use(t), e.mount("#q-app"))
                 }
-                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                b(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
                     k(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
                     default: () => o
@@ -159,24 +159,24 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "b4cc3ffe",
-            430: "4be6e8a8",
-            702: "aec0d6a9"
+            365: "3c494fbf",
+            430: "4be6e8a8"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            702: "ee87c168",
+            365: "b8547d97",
             736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                702: 1
+                365: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.4.0/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.4.1/unigui/web/js/193.b4cc3ffe.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/js/430.4be6e8a8.js` & `unigui-1.4.1/unigui/web/js/430.4be6e8a8.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui/web/js/702.aec0d6a9.js` & `unigui-1.4.1/unigui/web/js/365.3c494fbf.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [702], {
-        9702: (e, t, a) => {
+    [365], {
+        365: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => Wt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                 class: "q-pa-lg"
@@ -187,15 +187,15 @@
             function Q() {
                 q && (q.disconnect(), q = null), q = new MutationObserver(D), q.observe(u.$el, O)
             }
 
             function W(e) {
                 Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), g && console.log("------------------recalc design");
                 const t = V(e),
-                    a = H(e);
+                    a = E(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = b[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = y[d];
                     for (let a of r.data.childs)
@@ -209,15 +209,15 @@
                         } else if (a.name == e.data.name) {
                         o = e;
                         break
                     }
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
-                    e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
+                    e.styleSize = `height: ${h+Math.floor(s)}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
             function V(e) {
                 const t = u.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
@@ -268,15 +268,15 @@
                 }
                 let n = Array.from(s.entries());
                 n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function H(e) {
+            function E(e) {
                 e = null;
                 const t = e ? [e] : u.screen.blocks;
                 let a = window.innerWidth - 30,
                     l = [],
                     s = {};
                 for (let n of t)
                     if (0 == l.length)
@@ -335,15 +335,15 @@
                             s[a.fullname] = [Math.floor(n / e), t[l]]
                         }
                     }
                 }
                 for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
                 return s
             }
-            const E = (0, l.aZ)({
+            const H = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
                         C(["root", this.name])
                     }
                 },
                 props: {
@@ -354,28 +354,28 @@
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
             var U = a(4260),
-                T = a(3414),
-                K = a(2035),
-                P = a(4554),
+                K = a(3414),
+                P = a(2035),
+                T = a(4554),
                 N = a(2350),
                 I = a(7518),
                 R = a.n(I);
-            const L = (0, U.Z)(E, [
+            const L = (0, U.Z)(H, [
                     ["render", n]
                 ]),
                 B = L;
-            R()(E, "components", {
-                QItem: T.Z,
-                QItemSection: K.Z,
-                QIcon: P.Z,
+            R()(H, "components", {
+                QItem: K.Z,
+                QItemSection: P.Z,
+                QIcon: T.Z,
                 QItemLabel: N.Z
             });
             const F = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
                 Y = {
@@ -477,15 +477,15 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                     _: 1
                 })
             }
             var oe = a(8880);
-            const ne = e => ((0, l.dD)("data-v-0440fa69"), e = e(), (0, l.Cn)(), e),
+            const ne = e => ((0, l.dD)("data-v-7cd4ac4c"), e = e(), (0, l.Cn)(), e),
                 de = ["width", "height"],
                 re = ["src"],
                 ce = {
                     key: 15,
                     class: "web-camera-container"
                 },
                 he = {
@@ -1006,31 +1006,33 @@
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
                             return a
                         },
                         o = i(),
                         n = (0, Ae.iH)(o),
-                        d = (0, Ae.iH)(!Array.isArray(t.value.value)),
-                        r = (e, l) => {
+                        d = (0, Ae.iH)(o),
+                        r = (0, Ae.iH)(!Array.isArray(t.value.value)),
+                        c = (e, l) => {
                             C([a.value.name, t.value.name, e, l])
                         },
-                        c = (0, l.Fl)((() => d.value ? n.value.length > 0 ? n.value[0].iiid : null : n.value.map((e => e.iiid)))),
-                        h = (0, l.Fl)((() => t.value.value));
+                        h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
+                        u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
-                        n.value = i(), o = n.value
+                        d.value = i(), n.value = d.value
                     })), (0, l.YP)(t, ((e, a) => {
-                        g && console.log("data update", a.name), n.value = i(), o = n.value, d.value = !Array.isArray(t.value.value)
+                        g && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
                     })), {
                         rows: s,
-                        value: c,
-                        selected: n,
-                        singleMode: d,
-                        sendMessage: r,
-                        datavalue: h
+                        value: h,
+                        selected: d,
+                        singleMode: r,
+                        sendMessage: c,
+                        datavalue: u,
+                        updated: n
                     }
                 },
                 data() {
                     return {
                         search: "",
                         editMode: !1,
                         options: [],
@@ -1148,18 +1150,15 @@
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
-                        void 0 === this.updated ? this.updated = this.selected : Ze(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
-                    },
-                    data(e) {
-                        g && console.log("data update", this.name), this.updated = void 0
+                        Ze(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
                     }
                 },
                 computed: {
                     redit() {
                         return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
@@ -1187,41 +1186,41 @@
             var $e = a(9267),
                 ze = a(4842),
                 De = a(2165),
                 Oe = a(8870),
                 Qe = a(8186),
                 We = a(2414),
                 Ve = a(3884),
-                He = a(5735),
-                Ee = a(7208);
+                Ee = a(5735),
+                He = a(7208);
             const Ue = (0, U.Z)(Me, [
                     ["render", Se]
                 ]),
-                Te = Ue;
+                Ke = Ue;
             R()(Me, "components", {
                 QTable: $e.Z,
                 QInput: ze.Z,
-                QIcon: P.Z,
+                QIcon: T.Z,
                 QBtn: De.Z,
                 QTooltip: Oe.Z,
                 QTr: Qe.Z,
                 QTh: We.Z,
                 QTd: Ve.Z,
-                QCheckbox: He.Z,
-                QSelect: Ee.Z
+                QCheckbox: Ee.Z,
+                QSelect: He.Z
             });
-            const Ke = ["nodes", "edges"];
+            const Pe = ["nodes", "edges"];
 
-            function Pe(e, t, a, i, o, n) {
+            function Te(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Ke)
+                }, null, 12, Pe)
             }
             var Ne = a(2393),
                 Ie = a.n(Ne);
             const Re = Ie().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4"
                 }).selector(".selected").css({
@@ -1423,15 +1422,15 @@
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
                 Ye = (0, U.Z)(Fe, [
-                    ["render", Pe]
+                    ["render", Te]
                 ]),
                 Xe = Ye;
 
             function Je(e) {
                 let t = e.minheight ? e.minheight : m,
                     a = e.minwidth ? e.minwidth : f;
                 return `height: ${t}px; width: ${a}px`
@@ -1444,15 +1443,15 @@
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
             const et = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Te,
+                    utable: Ke,
                     cgraph: Xe
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
@@ -1654,37 +1653,37 @@
                         g && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize = Je(this.data), console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
+                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize || (this.styleSize = Je(this.data), console.log(`${this.name} size changed`))), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
                     }
                 }
             });
             var tt = a(4027),
                 at = a(9721),
                 lt = a(8886),
                 st = a(8761),
                 it = a(1232),
                 ot = a(5551),
                 nt = a(5869),
                 dt = a(1745);
             const rt = (0, U.Z)(et, [
                     ["render", xe],
-                    ["__scopeId", "data-v-0440fa69"]
+                    ["__scopeId", "data-v-7cd4ac4c"]
                 ]),
                 ct = rt;
             R()(et, "components", {
                 QImg: tt.Z,
-                QIcon: P.Z,
-                QSelect: Ee.Z,
+                QIcon: T.Z,
+                QSelect: He.Z,
                 QBadge: at.Z,
-                QCheckbox: He.Z,
+                QCheckbox: Ee.Z,
                 QToggle: lt.Z,
                 QBtnToggle: st.Z,
                 QInput: ze.Z,
                 QScrollArea: it.Z,
                 QTree: ot.Z,
                 QSeparator: nt.Z,
                 QUploader: dt.Z,
@@ -1771,15 +1770,15 @@
             var ut = a(151);
             const pt = (0, U.Z)(ht, [
                     ["render", ie]
                 ]),
                 gt = pt;
             R()(ht, "components", {
                 QCard: ut.Z,
-                QIcon: P.Z,
+                QIcon: T.Z,
                 QScrollArea: it.Z
             });
             const mt = (0, l.aZ)({
                     name: "zone",
                     components: {
                         block: gt
                     },
@@ -1891,16 +1890,15 @@
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         localServer: !0,
                         statusConnect: !1,
                         screen: {
                             blocks: []
-                        },
-                        prevHeight: 0
+                        }
                     }
                 },
                 components: {
                     menubar: B,
                     zone: wt
                 },
                 created() {
@@ -1913,16 +1911,15 @@
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         C(["root", e])
                     },
                     onResize(e) {
-                        const t = e.currentTarget.innerHeight;
-                        this.prevHeight != t && (g && console.log("window has been resized", t, window.innerHeight), this.prevHeight = t, D())
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), D()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
```

### Comparing `unigui-1.4.0/unigui/web/index.html` & `unigui-1.4.1/unigui/web/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.b57ab5bb.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.bfd9bd6e.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.4.0/LICENSE` & `unigui-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/setup.py` & `unigui-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.4.0',      
+      version='1.4.1',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.4.0/PKG-INFO` & `unigui-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.0
+Version: 1.4.1
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.0/README.md` & `unigui-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.4.0/unigui.egg-info/PKG-INFO` & `unigui-1.4.1/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.0
+Version: 1.4.1
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.4.0/unigui.egg-info/SOURCES.txt` & `unigui-1.4.1/unigui.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/702.ee87c168.css
+unigui/web/css/365.b8547d97.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -27,11 +27,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.b4cc3ffe.js
+unigui/web/js/365.3c494fbf.js
 unigui/web/js/430.4be6e8a8.js
-unigui/web/js/702.aec0d6a9.js
-unigui/web/js/app.b57ab5bb.js
+unigui/web/js/app.bfd9bd6e.js
 unigui/web/js/vendor.c0de6c67.js
```

