# Comparing `tmp/sym-recognizer-0.0.3.tar.gz` & `tmp/sym-recognizer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym-recognizer-0.0.3.tar", last modified: Sun May  7 07:56:46 2023, max compression
+gzip compressed data, was "sym-recognizer-0.0.4.tar", last modified: Sun May  7 08:08:37 2023, max compression
```

## Comparing `sym-recognizer-0.0.3.tar` & `sym-recognizer-0.0.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.106320 sym-recognizer-0.0.3/
--rw-r--r--   0 mixx3      (502) staff       (20)     1317 2022-10-19 22:23:18.000000 sym-recognizer-0.0.3/LICENSE.md
--rw-r--r--   0 mixx3      (502) staff       (20)       25 2023-05-07 07:54:57.000000 sym-recognizer-0.0.3/MANIFEST.in
--rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 07:56:46.106175 sym-recognizer-0.0.3/PKG-INFO
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.097630 sym-recognizer-0.0.3/recognizer/
--rw-r--r--   0 mixx3      (502) staff       (20)      239 2023-05-04 03:37:01.000000 sym-recognizer-0.0.3/recognizer/__init__.py
--rw-r--r--   0 mixx3      (502) staff       (20)      731 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/alphabet.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.104559 sym-recognizer-0.0.3/recognizer/data/
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:15:32.000000 sym-recognizer-0.0.3/recognizer/data/A.png
--rw-r--r--   0 mixx3      (502) staff       (20)      219 2020-09-11 18:15:40.000000 sym-recognizer-0.0.3/recognizer/data/B.png
--rw-r--r--   0 mixx3      (502) staff       (20)      224 2020-09-11 18:15:50.000000 sym-recognizer-0.0.3/recognizer/data/C.png
--rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:15:56.000000 sym-recognizer-0.0.3/recognizer/data/D.png
--rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:00.000000 sym-recognizer-0.0.3/recognizer/data/E.png
--rw-r--r--   0 mixx3      (502) staff       (20)      167 2020-09-11 18:16:04.000000 sym-recognizer-0.0.3/recognizer/data/F.png
--rw-r--r--   0 mixx3      (502) staff       (20)      244 2020-09-11 18:16:08.000000 sym-recognizer-0.0.3/recognizer/data/G.png
--rw-r--r--   0 mixx3      (502) staff       (20)      162 2020-09-11 18:16:16.000000 sym-recognizer-0.0.3/recognizer/data/H.png
--rw-r--r--   0 mixx3      (502) staff       (20)      129 2020-09-11 18:16:28.000000 sym-recognizer-0.0.3/recognizer/data/I.png
--rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:34.000000 sym-recognizer-0.0.3/recognizer/data/J.png
--rw-r--r--   0 mixx3      (502) staff       (20)      247 2020-09-11 18:16:34.000000 sym-recognizer-0.0.3/recognizer/data/K.png
--rw-r--r--   0 mixx3      (502) staff       (20)      141 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/L.png
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/M.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/N.png
--rw-r--r--   0 mixx3      (502) staff       (20)      248 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/O.png
--rw-r--r--   0 mixx3      (502) staff       (20)      189 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/P.png
--rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:36.000000 sym-recognizer-0.0.3/recognizer/data/Q.png
--rw-r--r--   0 mixx3      (502) staff       (20)      225 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/R.png
--rw-r--r--   0 mixx3      (502) staff       (20)      251 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/S.png
--rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/T.png
--rw-r--r--   0 mixx3      (502) staff       (20)      179 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/U.png
--rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/V.png
--rw-r--r--   0 mixx3      (502) staff       (20)      267 2020-09-11 18:16:38.000000 sym-recognizer-0.0.3/recognizer/data/W.png
--rw-r--r--   0 mixx3      (502) staff       (20)      264 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/X.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/Y.png
--rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/Z.png
--rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/a_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.3/recognizer/data/b_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      198 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/c_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/d_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/e_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/f_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:42.000000 sym-recognizer-0.0.3/recognizer/data/g_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      185 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/h_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/i_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/j_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      217 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/k_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      128 2020-09-11 18:16:44.000000 sym-recognizer-0.0.3/recognizer/data/l_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/m_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/n_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/o_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/p_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/q_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      155 2020-09-11 18:16:46.000000 sym-recognizer-0.0.3/recognizer/data/r_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      216 2020-09-11 18:16:48.000000 sym-recognizer-0.0.3/recognizer/data/s_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      166 2020-09-11 18:16:48.000000 sym-recognizer-0.0.3/recognizer/data/t_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:48.000000 sym-recognizer-0.0.3/recognizer/data/u_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      204 2020-09-11 18:16:48.000000 sym-recognizer-0.0.3/recognizer/data/v_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:50.000000 sym-recognizer-0.0.3/recognizer/data/w_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.3/recognizer/data/x_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.3/recognizer/data/y_.png
--rw-r--r--   0 mixx3      (502) staff       (20)      187 2020-09-11 18:16:50.000000 sym-recognizer-0.0.3/recognizer/data/z_.png
--rw-r--r--   0 mixx3      (502) staff       (20)     1020 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/data.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.105332 sym-recognizer-0.0.3/recognizer/methods/
--rw-r--r--   0 mixx3      (502) staff       (20)      174 2023-05-03 23:17:37.000000 sym-recognizer-0.0.3/recognizer/methods/__init__.py
--rw-r--r--   0 mixx3      (502) staff       (20)      321 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/methods/base.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1263 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/methods/corr.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1479 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/methods/morph.py
--rw-r--r--   0 mixx3      (502) staff       (20)      659 2023-05-05 18:05:55.000000 sym-recognizer-0.0.3/recognizer/recognizer.py
--rw-r--r--   0 mixx3      (502) staff       (20)     1675 2023-05-07 07:56:22.000000 sym-recognizer-0.0.3/recognizer/split.py
--rw-r--r--   0 mixx3      (502) staff       (20)       98 2023-05-04 04:24:06.000000 sym-recognizer-0.0.3/recognizer/symbol.py
--rw-r--r--   0 mixx3      (502) staff       (20)       38 2023-05-07 07:56:46.106353 sym-recognizer-0.0.3/setup.cfg
--rw-r--r--   0 mixx3      (502) staff       (20)      442 2023-05-07 07:56:41.000000 sym-recognizer-0.0.3/setup.py
-drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 07:56:46.105994 sym-recognizer-0.0.3/sym_recognizer.egg-info/
--rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/PKG-INFO
--rw-r--r--   0 mixx3      (502) staff       (20)     1634 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/SOURCES.txt
--rw-r--r--   0 mixx3      (502) staff       (20)        1 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/dependency_links.txt
--rw-r--r--   0 mixx3      (502) staff       (20)       31 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/requires.txt
--rw-r--r--   0 mixx3      (502) staff       (20)       11 2023-05-07 07:56:46.000000 sym-recognizer-0.0.3/sym_recognizer.egg-info/top_level.txt
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:08:37.316885 sym-recognizer-0.0.4/
+-rw-r--r--   0 mixx3      (502) staff       (20)     1317 2022-10-19 22:23:18.000000 sym-recognizer-0.0.4/LICENSE.md
+-rw-r--r--   0 mixx3      (502) staff       (20)       25 2023-05-07 07:54:57.000000 sym-recognizer-0.0.4/MANIFEST.in
+-rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 08:08:37.316756 sym-recognizer-0.0.4/PKG-INFO
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:08:37.306618 sym-recognizer-0.0.4/recognizer/
+-rw-r--r--   0 mixx3      (502) staff       (20)      239 2023-05-04 03:37:01.000000 sym-recognizer-0.0.4/recognizer/__init__.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      731 2023-05-07 07:56:22.000000 sym-recognizer-0.0.4/recognizer/alphabet.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:08:37.315179 sym-recognizer-0.0.4/recognizer/data/
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:15:32.000000 sym-recognizer-0.0.4/recognizer/data/A.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      219 2020-09-11 18:15:40.000000 sym-recognizer-0.0.4/recognizer/data/B.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      224 2020-09-11 18:15:50.000000 sym-recognizer-0.0.4/recognizer/data/C.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:15:56.000000 sym-recognizer-0.0.4/recognizer/data/D.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:00.000000 sym-recognizer-0.0.4/recognizer/data/E.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      167 2020-09-11 18:16:04.000000 sym-recognizer-0.0.4/recognizer/data/F.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      244 2020-09-11 18:16:08.000000 sym-recognizer-0.0.4/recognizer/data/G.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      162 2020-09-11 18:16:16.000000 sym-recognizer-0.0.4/recognizer/data/H.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      129 2020-09-11 18:16:28.000000 sym-recognizer-0.0.4/recognizer/data/I.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:34.000000 sym-recognizer-0.0.4/recognizer/data/J.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      247 2020-09-11 18:16:34.000000 sym-recognizer-0.0.4/recognizer/data/K.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      141 2020-09-11 18:16:36.000000 sym-recognizer-0.0.4/recognizer/data/L.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:36.000000 sym-recognizer-0.0.4/recognizer/data/M.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:36.000000 sym-recognizer-0.0.4/recognizer/data/N.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      248 2020-09-11 18:16:36.000000 sym-recognizer-0.0.4/recognizer/data/O.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      189 2020-09-11 18:16:36.000000 sym-recognizer-0.0.4/recognizer/data/P.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:36.000000 sym-recognizer-0.0.4/recognizer/data/Q.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      225 2020-09-11 18:16:38.000000 sym-recognizer-0.0.4/recognizer/data/R.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      251 2020-09-11 18:16:38.000000 sym-recognizer-0.0.4/recognizer/data/S.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:38.000000 sym-recognizer-0.0.4/recognizer/data/T.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      179 2020-09-11 18:16:38.000000 sym-recognizer-0.0.4/recognizer/data/U.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:38.000000 sym-recognizer-0.0.4/recognizer/data/V.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      267 2020-09-11 18:16:38.000000 sym-recognizer-0.0.4/recognizer/data/W.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      264 2020-09-11 18:16:40.000000 sym-recognizer-0.0.4/recognizer/data/X.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.4/recognizer/data/Y.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      241 2020-09-11 18:16:40.000000 sym-recognizer-0.0.4/recognizer/data/Z.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      222 2020-09-11 18:16:40.000000 sym-recognizer-0.0.4/recognizer/data/a_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      213 2020-09-11 18:16:40.000000 sym-recognizer-0.0.4/recognizer/data/b_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      198 2020-09-11 18:16:42.000000 sym-recognizer-0.0.4/recognizer/data/c_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.4/recognizer/data/d_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      218 2020-09-11 18:16:42.000000 sym-recognizer-0.0.4/recognizer/data/e_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:42.000000 sym-recognizer-0.0.4/recognizer/data/f_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      261 2020-09-11 18:16:42.000000 sym-recognizer-0.0.4/recognizer/data/g_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      185 2020-09-11 18:16:44.000000 sym-recognizer-0.0.4/recognizer/data/h_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      145 2020-09-11 18:16:44.000000 sym-recognizer-0.0.4/recognizer/data/i_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      140 2020-09-11 18:16:44.000000 sym-recognizer-0.0.4/recognizer/data/j_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      217 2020-09-11 18:16:44.000000 sym-recognizer-0.0.4/recognizer/data/k_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      128 2020-09-11 18:16:44.000000 sym-recognizer-0.0.4/recognizer/data/l_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.4/recognizer/data/m_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      173 2020-09-11 18:16:46.000000 sym-recognizer-0.0.4/recognizer/data/n_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      210 2020-09-11 18:16:46.000000 sym-recognizer-0.0.4/recognizer/data/o_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      228 2020-09-11 18:16:46.000000 sym-recognizer-0.0.4/recognizer/data/p_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:46.000000 sym-recognizer-0.0.4/recognizer/data/q_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      155 2020-09-11 18:16:46.000000 sym-recognizer-0.0.4/recognizer/data/r_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      216 2020-09-11 18:16:48.000000 sym-recognizer-0.0.4/recognizer/data/s_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      166 2020-09-11 18:16:48.000000 sym-recognizer-0.0.4/recognizer/data/t_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2020-09-11 18:16:48.000000 sym-recognizer-0.0.4/recognizer/data/u_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      204 2020-09-11 18:16:48.000000 sym-recognizer-0.0.4/recognizer/data/v_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      221 2020-09-11 18:16:50.000000 sym-recognizer-0.0.4/recognizer/data/w_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.4/recognizer/data/x_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      209 2020-09-11 18:16:50.000000 sym-recognizer-0.0.4/recognizer/data/y_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)      187 2020-09-11 18:16:50.000000 sym-recognizer-0.0.4/recognizer/data/z_.png
+-rw-r--r--   0 mixx3      (502) staff       (20)     1020 2023-05-07 07:56:22.000000 sym-recognizer-0.0.4/recognizer/data.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:08:37.315909 sym-recognizer-0.0.4/recognizer/methods/
+-rw-r--r--   0 mixx3      (502) staff       (20)      174 2023-05-03 23:17:37.000000 sym-recognizer-0.0.4/recognizer/methods/__init__.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      321 2023-05-07 07:56:22.000000 sym-recognizer-0.0.4/recognizer/methods/base.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1263 2023-05-07 07:56:22.000000 sym-recognizer-0.0.4/recognizer/methods/corr.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1479 2023-05-07 07:56:22.000000 sym-recognizer-0.0.4/recognizer/methods/morph.py
+-rw-r--r--   0 mixx3      (502) staff       (20)      659 2023-05-05 18:05:55.000000 sym-recognizer-0.0.4/recognizer/recognizer.py
+-rw-r--r--   0 mixx3      (502) staff       (20)     1675 2023-05-07 07:56:22.000000 sym-recognizer-0.0.4/recognizer/split.py
+-rw-r--r--   0 mixx3      (502) staff       (20)       98 2023-05-04 04:24:06.000000 sym-recognizer-0.0.4/recognizer/symbol.py
+-rw-r--r--   0 mixx3      (502) staff       (20)       38 2023-05-07 08:08:37.316917 sym-recognizer-0.0.4/setup.cfg
+-rw-r--r--   0 mixx3      (502) staff       (20)      461 2023-05-07 08:08:27.000000 sym-recognizer-0.0.4/setup.py
+drwxr-xr-x   0 mixx3      (502) staff       (20)        0 2023-05-07 08:08:37.316549 sym-recognizer-0.0.4/sym_recognizer.egg-info/
+-rw-r--r--   0 mixx3      (502) staff       (20)      260 2023-05-07 08:08:37.000000 sym-recognizer-0.0.4/sym_recognizer.egg-info/PKG-INFO
+-rw-r--r--   0 mixx3      (502) staff       (20)     1634 2023-05-07 08:08:37.000000 sym-recognizer-0.0.4/sym_recognizer.egg-info/SOURCES.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)        1 2023-05-07 08:08:37.000000 sym-recognizer-0.0.4/sym_recognizer.egg-info/dependency_links.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)       31 2023-05-07 08:08:37.000000 sym-recognizer-0.0.4/sym_recognizer.egg-info/requires.txt
+-rw-r--r--   0 mixx3      (502) staff       (20)       11 2023-05-07 08:08:37.000000 sym-recognizer-0.0.4/sym_recognizer.egg-info/top_level.txt
```

### Comparing `sym-recognizer-0.0.3/LICENSE.md` & `sym-recognizer-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.3/recognizer/alphabet.py` & `sym-recognizer-0.0.4/recognizer/alphabet.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.3/recognizer/data.py` & `sym-recognizer-0.0.4/recognizer/data.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.3/recognizer/methods/corr.py` & `sym-recognizer-0.0.4/recognizer/methods/corr.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.3/recognizer/methods/morph.py` & `sym-recognizer-0.0.4/recognizer/methods/morph.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.3/recognizer/recognizer.py` & `sym-recognizer-0.0.4/recognizer/recognizer.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.3/recognizer/split.py` & `sym-recognizer-0.0.4/recognizer/split.py`

 * *Files identical despite different names*

### Comparing `sym-recognizer-0.0.3/sym_recognizer.egg-info/SOURCES.txt` & `sym-recognizer-0.0.4/sym_recognizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

