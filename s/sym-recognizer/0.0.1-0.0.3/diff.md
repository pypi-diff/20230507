# Comparing `tmp/sym-recognizer-0.0.1.tar.gz` & `tmp/sym-recognizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym-recognizer-0.0.1.tar", last modified: Fri May  5 18:46:50 2023, max compression
+gzip compressed data, was "sym-recognizer-0.0.3.tar", last modified: Sun May  7 07:56:46 2023, max compression
```

## Comparing `sym-recognizer-0.0.1.tar` & `sym-recognizer-0.0.3.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-05 18:46:50.623594 sym-recognizer-0.0.1/
--rw-r--r--   0 mixx3      (502) staff       (20)     1317 2022-10-19 22:23:18.000000 sym-recognizer-0.0.1/LICENSE.md
--rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-05 18:46:50.623452 sym-recognizer-0.0.1/PKG-INFO
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-05 18:46:50.614476 sym-recognizer-0.0.1/recognizer/
--rw-r--r--   0 mixx3      (502) staff       (20)      239 2023-05-04 03:37:01.000000 sym-recognizer-0.0.1/recognizer/__init__.py
--rw-r--r--   0 mixx3      (502) staff       (20)      701 2023-05-04 04:48:33.000000 sym-recognizer-0.0.1/recognizer/alphabet.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-05 18:46:50.621791 sym-recognizer-0.0.1/recognizer/data/
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:15:32.000000 sym-recognizer-0.0.1/recognizer/data/A.png
--rw-r--r--   0 mixx3      (502) staff       (20)      219 2020-09-11 18:15:40.000000 sym-recognizer-0.0.1/recognizer/data/B.png
--rw-r--r--   0 mixx3      (502) staff       (20)      224 2020-09-11 18:15:50.000000 sym-recognizer-0.0.1/recognizer/data/C.png
--rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:15:56.000000 sym-recognizer-0.0.1/recognizer/data/D.png
--rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:00.000000 sym-recognizer-0.0.1/recognizer/data/E.png
--rw-r--r--   0 mixx3      (502) staff       (20)      167 2020-09-11 18:16:04.000000 sym-recognizer-0.0.1/recognizer/data/F.png
--rw-r--r--   0 mixx3      (502) staff       (20)      244 2020-09-11 18:16:08.000000 sym-recognizer-0.0.1/recognizer/data/G.png
--rw-r--r--   0 mixx3      (502) staff       (20)      162 2020-09-11 18:16:16.000000 sym-recognizer-0.0.1/recognizer/data/H.png
--rw-r--r--   0 mixx3      (502) staff       (20)      129 2020-09-11 18:16:28.000000 sym-recognizer-0.0.1/recognizer/data/I.png
--rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:34.000000 sym-recognizer-0.0.1/recognizer/data/J.png
--rw-r--r--   0 mixx3      (502) staff       (20)      247 2020-09-11 18:16:34.000000 sym-recognizer-0.0.1/recognizer/data/K.png
--rw-r--r--   0 mixx3      (502) staff       (20)      141 2020-09-11 18:16:36.000000 sym-recognizer-0.0.1/recognizer/data/L.png
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:36.000000 sym-recognizer-0.0.1/recognizer/data/M.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:36.000000 sym-recognizer-0.0.1/recognizer/data/N.png
--rw-r--r--   0 mixx3      (502) staff       (20)      248 2020-09-11 18:16:36.000000 sym-recognizer-0.0.1/recognizer/data/O.png
--rw-r--r--   0 mixx3      (502) staff       (20)      189 2020-09-11 18:16:36.000000 sym-recognizer-0.0.1/recognizer/data/P.png
--rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:36.000000 sym-recognizer-0.0.1/recognizer/data/Q.png
--rw-r--r--   0 mixx3      (502) staff       (20)      225 2020-09-11 18:16:38.000000 sym-recognizer-0.0.1/recognizer/data/R.png
--rw-r--r--   0 mixx3      (502) staff       (20)      251 2020-09-11 18:16:38.000000 sym-recognizer-0.0.1/recognizer/data/S.png
--rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:38.000000 sym-recognizer-0.0.1/recognizer/data/T.png
--rw-r--r--   0 mixx3      (502) staff       (20)      179 2020-09-11 18:16:38.000000 sym-recognizer-0.0.1/recognizer/data/U.png
--rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:38.000000 sym-recognizer-0.0.1/recognizer/data/V.png
--rw-r--r--   0 mixx3      (502) staff       (20)      267 2020-09-11 18:16:38.000000 sym-recognizer-0.0.1/recognizer/data/W.png
--rw-r--r--   0 mixx3      (502) staff       (20)      264 2020-09-11 18:16:40.000000 sym-recognizer-0.0.1/recognizer/data/X.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.1/recognizer/data/Y.png
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:40.000000 sym-recognizer-0.0.1/recognizer/data/Z.png
--rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:16:40.000000 sym-recognizer-0.0.1/recognizer/data/a_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.1/recognizer/data/b_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      198 2020-09-11 18:16:42.000000 sym-recognizer-0.0.1/recognizer/data/c_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.1/recognizer/data/d_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.1/recognizer/data/e_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:42.000000 sym-recognizer-0.0.1/recognizer/data/f_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:42.000000 sym-recognizer-0.0.1/recognizer/data/g_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      185 2020-09-11 18:16:44.000000 sym-recognizer-0.0.1/recognizer/data/h_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:44.000000 sym-recognizer-0.0.1/recognizer/data/i_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:44.000000 sym-recognizer-0.0.1/recognizer/data/j_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      217 2020-09-11 18:16:44.000000 sym-recognizer-0.0.1/recognizer/data/k_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      128 2020-09-11 18:16:44.000000 sym-recognizer-0.0.1/recognizer/data/l_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.1/recognizer/data/m_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:46.000000 sym-recognizer-0.0.1/recognizer/data/n_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.1/recognizer/data/o_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:46.000000 sym-recognizer-0.0.1/recognizer/data/p_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:46.000000 sym-recognizer-0.0.1/recognizer/data/q_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      155 2020-09-11 18:16:46.000000 sym-recognizer-0.0.1/recognizer/data/r_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      216 2020-09-11 18:16:48.000000 sym-recognizer-0.0.1/recognizer/data/s_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      166 2020-09-11 18:16:48.000000 sym-recognizer-0.0.1/recognizer/data/t_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:48.000000 sym-recognizer-0.0.1/recognizer/data/u_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      204 2020-09-11 18:16:48.000000 sym-recognizer-0.0.1/recognizer/data/v_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:50.000000 sym-recognizer-0.0.1/recognizer/data/w_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.1/recognizer/data/x_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.1/recognizer/data/y_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      187 2020-09-11 18:16:50.000000 sym-recognizer-0.0.1/recognizer/data/z_.png
--rw-r--r--   0 mixx3      (502) staff       (20)     1016 2023-05-05 18:40:44.000000 sym-recognizer-0.0.1/recognizer/data.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-05 18:46:50.622590 sym-recognizer-0.0.1/recognizer/methods/
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2023-05-03 23:17:37.000000 sym-recognizer-0.0.1/recognizer/methods/__init__.py
--rw-r--r--   0 mixx3      (502) staff       (20)      323 2023-05-03 23:48:11.000000 sym-recognizer-0.0.1/recognizer/methods/base.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1161 2023-05-05 17:05:13.000000 sym-recognizer-0.0.1/recognizer/methods/corr.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1450 2023-05-05 15:18:45.000000 sym-recognizer-0.0.1/recognizer/methods/morph.py
--rw-r--r--   0 mixx3      (502) staff       (20)      659 2023-05-05 18:05:55.000000 sym-recognizer-0.0.1/recognizer/recognizer.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1571 2023-05-05 15:29:46.000000 sym-recognizer-0.0.1/recognizer/split.py
--rw-r--r--   0 mixx3      (502) staff       (20)       98 2023-05-04 04:24:06.000000 sym-recognizer-0.0.1/recognizer/symbol.py
--rw-r--r--   0 mixx3      (502) staff       (20)       38 2023-05-05 18:46:50.623628 sym-recognizer-0.0.1/setup.cfg
--rw-r--r--   0 mixx3      (502) staff       (20)      519 2023-05-05 18:46:46.000000 sym-recognizer-0.0.1/setup.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-05 18:46:50.623262 sym-recognizer-0.0.1/sym_recognizer.egg-info/
--rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-05 18:46:50.000000 sym-recognizer-0.0.1/sym_recognizer.egg-info/PKG-INFO
--rw-r--r--   0 mixx3      (502) staff       (20)     1622 2023-05-05 18:46:50.000000 sym-recognizer-0.0.1/sym_recognizer.egg-info/SOURCES.txt
--rw-r--r--   0 mixx3      (502) staff       (20)        1 2023-05-05 18:46:50.000000 sym-recognizer-0.0.1/sym_recognizer.egg-info/dependency_links.txt
--rw-r--r--   0 mixx3      (502) staff       (20)       31 2023-05-05 18:46:50.000000 sym-recognizer-0.0.1/sym_recognizer.egg-info/requires.txt
--rw-r--r--   0 mixx3      (502) staff       (20)       11 2023-05-05 18:46:50.000000 sym-recognizer-0.0.1/sym_recognizer.egg-info/top_level.txt
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.106320 sym-recognizer-0.0.3/
+-rw-r--r--   0 mixx3      (502) staff       (20)     1317 2022-10-19 22:23:18.000000 sym-recognizer-0.0.3/LICENSE.md
+-rw-r--r--   0 mixx3      (502) staff       (20)       25 2023-05-07 07:54:57.000000 sym-recognizer-0.0.3/MANIFEST.in
+-rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 07:56:46.106175 sym-recognizer-0.0.3/PKG-INFO
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.097630 sym-recognizer-0.0.3/recognizer/
+-rw-r--r--   0 mixx3      (502) staff       (20)      239 2023-05-04 03:37:01.000000 sym-recognizer-0.0.3/recognizer/__init__.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      731 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/alphabet.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.104559 sym-recognizer-0.0.3/recognizer/data/
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:15:32.000000 sym-recognizer-0.0.3/recognizer/data/A.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      219 2020-09-11 18:15:40.000000 sym-recognizer-0.0.3/recognizer/data/B.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      224 2020-09-11 18:15:50.000000 sym-recognizer-0.0.3/recognizer/data/C.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:15:56.000000 sym-recognizer-0.0.3/recognizer/data/D.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:00.000000 sym-recognizer-0.0.3/recognizer/data/E.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      167 2020-09-11 18:16:04.000000 sym-recognizer-0.0.3/recognizer/data/F.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      244 2020-09-11 18:16:08.000000 sym-recognizer-0.0.3/recognizer/data/G.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      162 2020-09-11 18:16:16.000000 sym-recognizer-0.0.3/recognizer/data/H.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      129 2020-09-11 18:16:28.000000 sym-recognizer-0.0.3/recognizer/data/I.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:34.000000 sym-recognizer-0.0.3/recognizer/data/J.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      247 2020-09-11 18:16:34.000000 sym-recognizer-0.0.3/recognizer/data/K.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      141 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/L.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/M.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/N.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      248 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/O.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      189 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/P.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/Q.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      225 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/R.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      251 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/S.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/T.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      179 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/U.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/V.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      267 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/W.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      264 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/X.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/Y.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/Z.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/a_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/b_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      198 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/c_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/d_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/e_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/f_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/g_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      185 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/h_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/i_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/j_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      217 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/k_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      128 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/l_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/m_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/n_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/o_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/p_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/q_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      155 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/r_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      216 2020-09-11 18:16:48.000000 sym-recognizer-0.0.3/recognizer/data/s_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      166 2020-09-11 18:16:48.000000 sym-recognizer-0.0.3/recognizer/data/t_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:48.000000 sym-recognizer-0.0.3/recognizer/data/u_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      204 2020-09-11 18:16:48.000000 sym-recognizer-0.0.3/recognizer/data/v_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:50.000000 sym-recognizer-0.0.3/recognizer/data/w_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.3/recognizer/data/x_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.3/recognizer/data/y_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      187 2020-09-11 18:16:50.000000 sym-recognizer-0.0.3/recognizer/data/z_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)     1020 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/data.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.105332 sym-recognizer-0.0.3/recognizer/methods/
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2023-05-03 23:17:37.000000 sym-recognizer-0.0.3/recognizer/methods/__init__.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      321 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/methods/base.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1263 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/methods/corr.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1479 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/methods/morph.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      659 2023-05-05 18:05:55.000000 sym-recognizer-0.0.3/recognizer/recognizer.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1675 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/split.py
+-rw-r--r--   0 mixx3      (502) staff       (20)       98 2023-05-04 04:24:06.000000 sym-recognizer-0.0.3/recognizer/symbol.py
+-rw-r--r--   0 mixx3      (502) staff       (20)       38 2023-05-07 07:56:46.106353 sym-recognizer-0.0.3/setup.cfg
+-rw-r--r--   0 mixx3      (502) staff       (20)      442 2023-05-07 07:56:41.000000 sym-recognizer-0.0.3/setup.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.105994 sym-recognizer-0.0.3/sym_recognizer.egg-info/
+-rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/PKG-INFO
+-rw-r--r--   0 mixx3      (502) staff       (20)     1634 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/SOURCES.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)        1 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/dependency_links.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)       31 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/requires.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)       11 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/top_level.txt
```

### Comparing `sym-recognizer-0.0.1/LICENSE.md` & `sym-recognizer-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.1/recognizer/alphabet.py` & `sym-recognizer-0.0.3/recognizer/alphabet.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,11 +17,13 @@
 class CustomAlphabet(Alphabet):
     symbols = None
 
     @classmethod
     def from_repository(cls, path):
         for img_name in glob.glob(f"{path}/*.png"):
             s = Symbol()
-            s.vector = NativeSplitter.split_into_symbols(cv.imread(img_name, cv.IMREAD_GRAYSCALE))[0].vector
+            s.vector = NativeSplitter.split_into_symbols(
+                cv.imread(img_name, cv.IMREAD_GRAYSCALE)
+            )[0].vector
             s.sym_mapper = img_name.split("/")[-1].replace(".png", "").replace("_", "")
             cls.symbols.append(s)
         return cls
```

### Comparing `sym-recognizer-0.0.1/recognizer/data.py` & `sym-recognizer-0.0.3/recognizer/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         s = Symbol()
         img = cv.imread(img_name, cv.IMREAD_GRAYSCALE)
         ret2, th2 = cv.threshold(img, 0, 255, cv.THRESH_BINARY_INV + cv.THRESH_OTSU)
         kernel = cv.getStructuringElement(cv.MORPH_RECT, (5, 5))
         thresh = cv.morphologyEx(th2, cv.MORPH_CLOSE, kernel)
         contours, _ = cv.findContours(thresh, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_NONE)
         x, y, w, h = cv.boundingRect(contours[0])
-        img_c = thresh[y:y + h, x:x + w].copy()
+        img_c = thresh[y : y + h, x : x + w].copy()
         mn = img_c.mean()
         fmin = img_c < mn
         fmax = img_c >= mn
         img_c[fmin] = 0
         img_c[fmax] = 255
         s.vector = img_c
         s.vector = s.vector / np.linalg.norm(s.vector)
```

### Comparing `sym-recognizer-0.0.1/recognizer/methods/corr.py` & `sym-recognizer-0.0.3/recognizer/methods/corr.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,28 @@
 class Correlation(RecognitionMethod):
     @staticmethod
     def recognize(img: np.ndarray, alphabet: Alphabet, splitter: Splitter) -> str:
         splitted = splitter.split_into_symbols(img)
         for sym in splitted:
             max_val = 0
             for et in alphabet.symbols:
-                cur_val = np.linalg.norm(Correlation.check_correlation(sym.vector, et.vector))
+                cur_val = np.linalg.norm(
+                    Correlation.check_correlation(sym.vector, et.vector)
+                )
                 if cur_val > max_val:
                     max_val = cur_val
                     sym.sym_mapper = et.sym_mapper
         return "".join(sym.sym_mapper for sym in splitted)
 
     @staticmethod
     def check_correlation(img: np.ndarray, eth: np.ndarray) -> float:
         if img.shape != eth.shape:
             img = cv.resize(img, (eth.shape[1], eth.shape[0]))
         img = img / np.linalg.norm(img)
         eth = eth / np.linalg.norm(eth)
         if np.linalg.norm(img) * np.linalg.norm(eth) != 0:
-            return np.dot(img.flatten(), eth.flatten()) / np.linalg.norm(img) * np.linalg.norm(eth)
+            return (
+                np.dot(img.flatten(), eth.flatten())
+                / np.linalg.norm(img)
+                * np.linalg.norm(eth)
+            )
         return 0
```

### Comparing `sym-recognizer-0.0.1/recognizer/methods/morph.py` & `sym-recognizer-0.0.3/recognizer/methods/morph.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from recognizer.alphabet import Alphabet
 from recognizer.split import Splitter
 from recognizer.data import Symbol
 import cv2 as cv
 
 
 class Morphology(RecognitionMethod):
-
     @staticmethod
     def recognize(img: np.ndarray, alphabet: Alphabet, splitter: Splitter) -> str:
         splitted: list[Symbol] = splitter.split_into_symbols(img)
         for sym in splitted:
             min_dist = np.inf
             for eth in alphabet.symbols:
                 cur_dist = Morphology.dist(sym.vector, eth.vector)
@@ -32,9 +31,11 @@
     def dist(img: np.ndarray, eth: np.ndarray):
         if img.shape != eth.shape:
             img = cv.resize(img, (eth.shape[1], eth.shape[0]))
         img = img / np.linalg.norm(img)
         eth = eth / np.linalg.norm(eth)
         c = np.ones_like(img)
         if np.linalg.norm(img - c) != 0:
-            return np.linalg.norm(img - Morphology.project(eth, img)) / np.linalg.norm(img - c)
+            return np.linalg.norm(img - Morphology.project(eth, img)) / np.linalg.norm(
+                img - c
+            )
         return 1
```

### Comparing `sym-recognizer-0.0.1/recognizer/recognizer.py` & `sym-recognizer-0.0.3/recognizer/recognizer.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.1/recognizer/split.py` & `sym-recognizer-0.0.3/recognizer/split.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,39 +9,44 @@
     @abstractmethod
     def split_into_symbols(img: np.ndarray) -> list[Symbol]:
         raise NotImplementedError
 
 
 class NativeSplitter(Splitter):
     @staticmethod
-    def split_into_symbols(img: np.ndarray) -> list[Symbol]:
+    def split_into_symbols(
+        img: np.ndarray, kernel_size: tuple[int] = (5, 5)
+    ) -> list[Symbol]:
         ret2, th2 = cv.threshold(img, 0, 255, cv.THRESH_BINARY_INV + cv.THRESH_OTSU)
 
-        kernel = cv.getStructuringElement(cv.MORPH_RECT, (5, 5))
+        kernel = cv.getStructuringElement(cv.MORPH_RECT, kernel_size)
         thresh = cv.morphologyEx(th2, cv.MORPH_CLOSE, kernel)
         contours, _ = cv.findContours(thresh, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_NONE)
         symbols = []
         for idx, contour in enumerate(contours):
             x, y, w, h = cv.boundingRect(contour)
-            img_c = thresh[y:y + h, x:x + w].copy()
-            fmin = img_c < 30
-            fmax = img_c >= 30
+            img_c = thresh[y : y + h, x : x + w].copy()
+            mn = img_c.mean()
+            fmin = img_c < mn
+            fmax = img_c >= mn
             img_c[fmin] = 0
             img_c[fmax] = 255
             ic = Symbol()
             ic.vector = img_c
-            ic.pos_mapper = x ** 2 + y ** 20
+            ic.pos_mapper = x**2 + y**2
             symbols.append(ic)
         symbols.sort(key=lambda x: x.pos_mapper)
         return symbols
 
     @staticmethod
     def _make_border(img: np.ndarray, chunk_size: int, color: list = [0, 0, 0]):
         b_size = chunk_size // 2 + 1
-        constant = cv.copyMakeBorder(img, b_size, b_size, b_size, b_size, cv.BORDER_CONSTANT, value=color)
+        constant = cv.copyMakeBorder(
+            img, b_size, b_size, b_size, b_size, cv.BORDER_CONSTANT, value=color
+        )
         return constant
 
     @staticmethod
     def normalize(v):
         norm = np.linalg.norm(v)
         if norm == 0:
             return v
```

### Comparing `sym-recognizer-0.0.1/sym_recognizer.egg-info/SOURCES.txt` & `sym-recognizer-0.0.3/sym_recognizer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.md
+MANIFEST.in
 setup.py
 recognizer/__init__.py
 recognizer/alphabet.py
 recognizer/data.py
 recognizer/recognizer.py
 recognizer/split.py
 recognizer/symbol.py
```

