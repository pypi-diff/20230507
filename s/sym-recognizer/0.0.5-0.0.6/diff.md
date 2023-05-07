# Comparing `tmp/sym-recognizer-0.0.5.tar.gz` & `tmp/sym-recognizer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym-recognizer-0.0.5.tar", last modified: Sun May  7 08:36:59 2023, max compression
+gzip compressed data, was "sym-recognizer-0.0.6.tar", last modified: Sun May  7 08:37:52 2023, max compression
```

## Comparing `sym-recognizer-0.0.5.tar` & `sym-recognizer-0.0.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:36:59.938652 sym-recognizer-0.0.5/
--rw-r--r--   0 mixx3      (502) staff       (20)     1317 2022-10-19 22:23:18.000000 sym-recognizer-0.0.5/LICENSE.md
--rw-r--r--   0 mixx3      (502) staff       (20)       23 2023-05-07 08:32:02.000000 sym-recognizer-0.0.5/MANIFEST.in
--rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 08:36:59.938516 sym-recognizer-0.0.5/PKG-INFO
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:36:59.928840 sym-recognizer-0.0.5/recognizer/
--rw-r--r--   0 mixx3      (502) staff       (20)      239 2023-05-04 03:37:01.000000 sym-recognizer-0.0.5/recognizer/__init__.py
--rw-r--r--   0 mixx3      (502) staff       (20)      731 2023-05-07 07:56:22.000000 sym-recognizer-0.0.5/recognizer/alphabet.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:36:59.936507 sym-recognizer-0.0.5/recognizer/data/
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:15:32.000000 sym-recognizer-0.0.5/recognizer/data/A.png
--rw-r--r--   0 mixx3      (502) staff       (20)      219 2020-09-11 18:15:40.000000 sym-recognizer-0.0.5/recognizer/data/B.png
--rw-r--r--   0 mixx3      (502) staff       (20)      224 2020-09-11 18:15:50.000000 sym-recognizer-0.0.5/recognizer/data/C.png
--rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:15:56.000000 sym-recognizer-0.0.5/recognizer/data/D.png
--rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:00.000000 sym-recognizer-0.0.5/recognizer/data/E.png
--rw-r--r--   0 mixx3      (502) staff       (20)      167 2020-09-11 18:16:04.000000 sym-recognizer-0.0.5/recognizer/data/F.png
--rw-r--r--   0 mixx3      (502) staff       (20)      244 2020-09-11 18:16:08.000000 sym-recognizer-0.0.5/recognizer/data/G.png
--rw-r--r--   0 mixx3      (502) staff       (20)      162 2020-09-11 18:16:16.000000 sym-recognizer-0.0.5/recognizer/data/H.png
--rw-r--r--   0 mixx3      (502) staff       (20)      129 2020-09-11 18:16:28.000000 sym-recognizer-0.0.5/recognizer/data/I.png
--rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:34.000000 sym-recognizer-0.0.5/recognizer/data/J.png
--rw-r--r--   0 mixx3      (502) staff       (20)      247 2020-09-11 18:16:34.000000 sym-recognizer-0.0.5/recognizer/data/K.png
--rw-r--r--   0 mixx3      (502) staff       (20)      141 2020-09-11 18:16:36.000000 sym-recognizer-0.0.5/recognizer/data/L.png
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:36.000000 sym-recognizer-0.0.5/recognizer/data/M.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:36.000000 sym-recognizer-0.0.5/recognizer/data/N.png
--rw-r--r--   0 mixx3      (502) staff       (20)      248 2020-09-11 18:16:36.000000 sym-recognizer-0.0.5/recognizer/data/O.png
--rw-r--r--   0 mixx3      (502) staff       (20)      189 2020-09-11 18:16:36.000000 sym-recognizer-0.0.5/recognizer/data/P.png
--rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:36.000000 sym-recognizer-0.0.5/recognizer/data/Q.png
--rw-r--r--   0 mixx3      (502) staff       (20)      225 2020-09-11 18:16:38.000000 sym-recognizer-0.0.5/recognizer/data/R.png
--rw-r--r--   0 mixx3      (502) staff       (20)      251 2020-09-11 18:16:38.000000 sym-recognizer-0.0.5/recognizer/data/S.png
--rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:38.000000 sym-recognizer-0.0.5/recognizer/data/T.png
--rw-r--r--   0 mixx3      (502) staff       (20)      179 2020-09-11 18:16:38.000000 sym-recognizer-0.0.5/recognizer/data/U.png
--rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:38.000000 sym-recognizer-0.0.5/recognizer/data/V.png
--rw-r--r--   0 mixx3      (502) staff       (20)      267 2020-09-11 18:16:38.000000 sym-recognizer-0.0.5/recognizer/data/W.png
--rw-r--r--   0 mixx3      (502) staff       (20)      264 2020-09-11 18:16:40.000000 sym-recognizer-0.0.5/recognizer/data/X.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.5/recognizer/data/Y.png
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:40.000000 sym-recognizer-0.0.5/recognizer/data/Z.png
--rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:16:40.000000 sym-recognizer-0.0.5/recognizer/data/a_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.5/recognizer/data/b_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      198 2020-09-11 18:16:42.000000 sym-recognizer-0.0.5/recognizer/data/c_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.5/recognizer/data/d_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.5/recognizer/data/e_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:42.000000 sym-recognizer-0.0.5/recognizer/data/f_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:42.000000 sym-recognizer-0.0.5/recognizer/data/g_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      185 2020-09-11 18:16:44.000000 sym-recognizer-0.0.5/recognizer/data/h_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:44.000000 sym-recognizer-0.0.5/recognizer/data/i_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:44.000000 sym-recognizer-0.0.5/recognizer/data/j_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      217 2020-09-11 18:16:44.000000 sym-recognizer-0.0.5/recognizer/data/k_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      128 2020-09-11 18:16:44.000000 sym-recognizer-0.0.5/recognizer/data/l_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.5/recognizer/data/m_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:46.000000 sym-recognizer-0.0.5/recognizer/data/n_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.5/recognizer/data/o_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:46.000000 sym-recognizer-0.0.5/recognizer/data/p_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:46.000000 sym-recognizer-0.0.5/recognizer/data/q_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      155 2020-09-11 18:16:46.000000 sym-recognizer-0.0.5/recognizer/data/r_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      216 2020-09-11 18:16:48.000000 sym-recognizer-0.0.5/recognizer/data/s_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      166 2020-09-11 18:16:48.000000 sym-recognizer-0.0.5/recognizer/data/t_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:48.000000 sym-recognizer-0.0.5/recognizer/data/u_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      204 2020-09-11 18:16:48.000000 sym-recognizer-0.0.5/recognizer/data/v_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:50.000000 sym-recognizer-0.0.5/recognizer/data/w_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.5/recognizer/data/x_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.5/recognizer/data/y_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      187 2020-09-11 18:16:50.000000 sym-recognizer-0.0.5/recognizer/data/z_.png
--rw-r--r--   0 mixx3      (502) staff       (20)     1065 2023-05-07 08:36:47.000000 sym-recognizer-0.0.5/recognizer/data.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:36:59.937332 sym-recognizer-0.0.5/recognizer/methods/
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2023-05-03 23:17:37.000000 sym-recognizer-0.0.5/recognizer/methods/__init__.py
--rw-r--r--   0 mixx3      (502) staff       (20)      321 2023-05-07 07:56:22.000000 sym-recognizer-0.0.5/recognizer/methods/base.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1263 2023-05-07 07:56:22.000000 sym-recognizer-0.0.5/recognizer/methods/corr.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1479 2023-05-07 07:56:22.000000 sym-recognizer-0.0.5/recognizer/methods/morph.py
--rw-r--r--   0 mixx3      (502) staff       (20)      659 2023-05-05 18:05:55.000000 sym-recognizer-0.0.5/recognizer/recognizer.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1675 2023-05-07 07:56:22.000000 sym-recognizer-0.0.5/recognizer/split.py
--rw-r--r--   0 mixx3      (502) staff       (20)       98 2023-05-04 04:24:06.000000 sym-recognizer-0.0.5/recognizer/symbol.py
--rw-r--r--   0 mixx3      (502) staff       (20)       38 2023-05-07 08:36:59.938704 sym-recognizer-0.0.5/setup.cfg
--rw-r--r--   0 mixx3      (502) staff       (20)      461 2023-05-07 08:36:56.000000 sym-recognizer-0.0.5/setup.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:36:59.938172 sym-recognizer-0.0.5/sym_recognizer.egg-info/
--rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 08:36:59.000000 sym-recognizer-0.0.5/sym_recognizer.egg-info/PKG-INFO
--rw-r--r--   0 mixx3      (502) staff       (20)     1634 2023-05-07 08:36:59.000000 sym-recognizer-0.0.5/sym_recognizer.egg-info/SOURCES.txt
--rw-r--r--   0 mixx3      (502) staff       (20)        1 2023-05-07 08:36:59.000000 sym-recognizer-0.0.5/sym_recognizer.egg-info/dependency_links.txt
--rw-r--r--   0 mixx3      (502) staff       (20)       31 2023-05-07 08:36:59.000000 sym-recognizer-0.0.5/sym_recognizer.egg-info/requires.txt
--rw-r--r--   0 mixx3      (502) staff       (20)       11 2023-05-07 08:36:59.000000 sym-recognizer-0.0.5/sym_recognizer.egg-info/top_level.txt
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:37:52.139162 sym-recognizer-0.0.6/
+-rw-r--r--   0 mixx3      (502) staff       (20)     1317 2022-10-19 22:23:18.000000 sym-recognizer-0.0.6/LICENSE.md
+-rw-r--r--   0 mixx3      (502) staff       (20)       29 2023-05-07 08:37:41.000000 sym-recognizer-0.0.6/MANIFEST.in
+-rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 08:37:52.139045 sym-recognizer-0.0.6/PKG-INFO
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:37:52.129983 sym-recognizer-0.0.6/recognizer/
+-rw-r--r--   0 mixx3      (502) staff       (20)      239 2023-05-04 03:37:01.000000 sym-recognizer-0.0.6/recognizer/__init__.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      731 2023-05-07 07:56:22.000000 sym-recognizer-0.0.6/recognizer/alphabet.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:37:52.137423 sym-recognizer-0.0.6/recognizer/data/
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:15:32.000000 sym-recognizer-0.0.6/recognizer/data/A.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      219 2020-09-11 18:15:40.000000 sym-recognizer-0.0.6/recognizer/data/B.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      224 2020-09-11 18:15:50.000000 sym-recognizer-0.0.6/recognizer/data/C.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:15:56.000000 sym-recognizer-0.0.6/recognizer/data/D.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:00.000000 sym-recognizer-0.0.6/recognizer/data/E.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      167 2020-09-11 18:16:04.000000 sym-recognizer-0.0.6/recognizer/data/F.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      244 2020-09-11 18:16:08.000000 sym-recognizer-0.0.6/recognizer/data/G.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      162 2020-09-11 18:16:16.000000 sym-recognizer-0.0.6/recognizer/data/H.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      129 2020-09-11 18:16:28.000000 sym-recognizer-0.0.6/recognizer/data/I.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:34.000000 sym-recognizer-0.0.6/recognizer/data/J.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      247 2020-09-11 18:16:34.000000 sym-recognizer-0.0.6/recognizer/data/K.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      141 2020-09-11 18:16:36.000000 sym-recognizer-0.0.6/recognizer/data/L.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:36.000000 sym-recognizer-0.0.6/recognizer/data/M.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:36.000000 sym-recognizer-0.0.6/recognizer/data/N.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      248 2020-09-11 18:16:36.000000 sym-recognizer-0.0.6/recognizer/data/O.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      189 2020-09-11 18:16:36.000000 sym-recognizer-0.0.6/recognizer/data/P.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:36.000000 sym-recognizer-0.0.6/recognizer/data/Q.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      225 2020-09-11 18:16:38.000000 sym-recognizer-0.0.6/recognizer/data/R.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      251 2020-09-11 18:16:38.000000 sym-recognizer-0.0.6/recognizer/data/S.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:38.000000 sym-recognizer-0.0.6/recognizer/data/T.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      179 2020-09-11 18:16:38.000000 sym-recognizer-0.0.6/recognizer/data/U.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:38.000000 sym-recognizer-0.0.6/recognizer/data/V.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      267 2020-09-11 18:16:38.000000 sym-recognizer-0.0.6/recognizer/data/W.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      264 2020-09-11 18:16:40.000000 sym-recognizer-0.0.6/recognizer/data/X.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.6/recognizer/data/Y.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:40.000000 sym-recognizer-0.0.6/recognizer/data/Z.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:16:40.000000 sym-recognizer-0.0.6/recognizer/data/a_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.6/recognizer/data/b_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      198 2020-09-11 18:16:42.000000 sym-recognizer-0.0.6/recognizer/data/c_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.6/recognizer/data/d_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.6/recognizer/data/e_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:42.000000 sym-recognizer-0.0.6/recognizer/data/f_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:42.000000 sym-recognizer-0.0.6/recognizer/data/g_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      185 2020-09-11 18:16:44.000000 sym-recognizer-0.0.6/recognizer/data/h_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:44.000000 sym-recognizer-0.0.6/recognizer/data/i_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:44.000000 sym-recognizer-0.0.6/recognizer/data/j_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      217 2020-09-11 18:16:44.000000 sym-recognizer-0.0.6/recognizer/data/k_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      128 2020-09-11 18:16:44.000000 sym-recognizer-0.0.6/recognizer/data/l_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.6/recognizer/data/m_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:46.000000 sym-recognizer-0.0.6/recognizer/data/n_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.6/recognizer/data/o_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:46.000000 sym-recognizer-0.0.6/recognizer/data/p_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:46.000000 sym-recognizer-0.0.6/recognizer/data/q_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      155 2020-09-11 18:16:46.000000 sym-recognizer-0.0.6/recognizer/data/r_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      216 2020-09-11 18:16:48.000000 sym-recognizer-0.0.6/recognizer/data/s_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      166 2020-09-11 18:16:48.000000 sym-recognizer-0.0.6/recognizer/data/t_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:48.000000 sym-recognizer-0.0.6/recognizer/data/u_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      204 2020-09-11 18:16:48.000000 sym-recognizer-0.0.6/recognizer/data/v_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:50.000000 sym-recognizer-0.0.6/recognizer/data/w_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.6/recognizer/data/x_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.6/recognizer/data/y_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      187 2020-09-11 18:16:50.000000 sym-recognizer-0.0.6/recognizer/data/z_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)     1065 2023-05-07 08:36:47.000000 sym-recognizer-0.0.6/recognizer/data.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:37:52.138270 sym-recognizer-0.0.6/recognizer/methods/
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2023-05-03 23:17:37.000000 sym-recognizer-0.0.6/recognizer/methods/__init__.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      321 2023-05-07 07:56:22.000000 sym-recognizer-0.0.6/recognizer/methods/base.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1263 2023-05-07 07:56:22.000000 sym-recognizer-0.0.6/recognizer/methods/corr.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1479 2023-05-07 07:56:22.000000 sym-recognizer-0.0.6/recognizer/methods/morph.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      659 2023-05-05 18:05:55.000000 sym-recognizer-0.0.6/recognizer/recognizer.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1675 2023-05-07 07:56:22.000000 sym-recognizer-0.0.6/recognizer/split.py
+-rw-r--r--   0 mixx3      (502) staff       (20)       98 2023-05-04 04:24:06.000000 sym-recognizer-0.0.6/recognizer/symbol.py
+-rw-r--r--   0 mixx3      (502) staff       (20)       38 2023-05-07 08:37:52.139300 sym-recognizer-0.0.6/setup.cfg
+-rw-r--r--   0 mixx3      (502) staff       (20)      461 2023-05-07 08:37:45.000000 sym-recognizer-0.0.6/setup.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:37:52.138879 sym-recognizer-0.0.6/sym_recognizer.egg-info/
+-rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 08:37:52.000000 sym-recognizer-0.0.6/sym_recognizer.egg-info/PKG-INFO
+-rw-r--r--   0 mixx3      (502) staff       (20)     1634 2023-05-07 08:37:52.000000 sym-recognizer-0.0.6/sym_recognizer.egg-info/SOURCES.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)        1 2023-05-07 08:37:52.000000 sym-recognizer-0.0.6/sym_recognizer.egg-info/dependency_links.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)       31 2023-05-07 08:37:52.000000 sym-recognizer-0.0.6/sym_recognizer.egg-info/requires.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)       11 2023-05-07 08:37:52.000000 sym-recognizer-0.0.6/sym_recognizer.egg-info/top_level.txt
```

### Comparing `sym-recognizer-0.0.5/LICENSE.md` & `sym-recognizer-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.5/recognizer/alphabet.py` & `sym-recognizer-0.0.6/recognizer/alphabet.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.5/recognizer/data.py` & `sym-recognizer-0.0.6/recognizer/data.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.5/recognizer/methods/corr.py` & `sym-recognizer-0.0.6/recognizer/methods/corr.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.5/recognizer/methods/morph.py` & `sym-recognizer-0.0.6/recognizer/methods/morph.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.5/recognizer/recognizer.py` & `sym-recognizer-0.0.6/recognizer/recognizer.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.5/recognizer/split.py` & `sym-recognizer-0.0.6/recognizer/split.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.5/sym_recognizer.egg-info/SOURCES.txt` & `sym-recognizer-0.0.6/sym_recognizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

