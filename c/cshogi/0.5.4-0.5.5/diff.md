# Comparing `tmp/cshogi-0.5.4.tar.gz` & `tmp/cshogi-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshogi-0.5.4.tar", last modified: Sun May  7 08:57:41 2023, max compression
+gzip compressed data, was "cshogi-0.5.5.tar", last modified: Sun May  7 09:09:05 2023, max compression
```

## Comparing `cshogi-0.5.4.tar` & `cshogi-0.5.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.148699 cshogi-0.5.4/
--rw-rw-rw-   0        0        0    35823 2023-05-07 08:57:02.000000 cshogi-0.5.4/LICENSE
--rw-rw-rw-   0        0        0      358 2023-05-07 08:57:41.148699 cshogi-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     5135 2023-05-07 08:57:02.000000 cshogi-0.5.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi/
--rw-rw-rw-   0        0        0     2774 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/CSA.py
--rw-rw-rw-   0        0        0    18556 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/KI2.py
--rw-rw-rw-   0        0        0    17360 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/KIF.py
--rw-rw-rw-   0        0        0     2988 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/PGN.py
--rw-rw-rw-   0        0        0       27 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/__init__.py
--rw-rw-rw-   0        0        0    28993 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/_cshogi.pyx
--rw-rw-rw-   0        0        0    25971 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi/dlshogi/
--rw-rw-rw-   0        0        0      327 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/dlshogi/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/elo.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi/gym_shogi/
--rw-rw-rw-   0        0        0      132 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/gym_shogi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi/gym_shogi/envs/
--rw-rw-rw-   0        0        0      118 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/gym_shogi/envs/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/gym_shogi/envs/shogi_env.pyx
--rw-rw-rw-   0        0        0      755 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/gym_shogi/envs/shogi_vec_env.pyx
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi/usi/
--rw-rw-rw-   0        0        0     6725 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/usi/Engine.py
--rw-rw-rw-   0        0        0       26 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/usi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi/web/
--rw-rw-rw-   0        0        0    13662 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/web/app.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi/web/static/
--rw-rw-rw-   0        0        0    13931 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/web/static/board.js
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi/web/templates/
--rw-rw-rw-   0        0        0    17362 2023-05-07 08:57:02.000000 cshogi-0.5.4/cshogi/web/templates/board.html
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.133120 cshogi-0.5.4/cshogi.egg-info/
--rw-rw-rw-   0        0        0      358 2023-05-07 08:57:40.000000 cshogi-0.5.4/cshogi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-05-07 08:57:41.000000 cshogi-0.5.4/cshogi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 08:57:40.000000 cshogi-0.5.4/cshogi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 08:57:40.000000 cshogi-0.5.4/cshogi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 08:57:41.148699 cshogi-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0     2006 2023-05-07 08:57:02.000000 cshogi-0.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.148699 cshogi-0.5.4/src/
--rw-rw-rw-   0        0        0     8208 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/bitboard.cpp
--rw-rw-rw-   0        0        0     2225 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/book.cpp
--rw-rw-rw-   0        0        0     1350 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/common.cpp
--rw-rw-rw-   0        0        0    28484 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/dfpn.cpp
--rw-rw-rw-   0        0        0    50568 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/generateMoves.cpp
--rw-rw-rw-   0        0        0     1789 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/hand.cpp
--rw-rw-rw-   0        0        0    19051 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/init.cpp
--rw-rw-rw-   0        0        0     6937 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/mate.cpp
--rw-rw-rw-   0        0        0     2163 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/move.cpp
--rw-rw-rw-   0        0        0     1172 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/mt64bit.cpp
--rw-rw-rw-   0        0        0   174059 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/position.cpp
--rw-rw-rw-   0        0        0     3308 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/search.cpp
--rw-rw-rw-   0        0        0     1416 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/square.cpp
--rw-rw-rw-   0        0        0     6627 2023-05-07 08:57:02.000000 cshogi-0.5.4/src/usi.cpp
-drwxrwxrwx   0        0        0        0 2023-05-07 08:57:41.148699 cshogi-0.5.4/test/
--rw-rw-rw-   0        0        0      824 2023-05-07 08:57:02.000000 cshogi-0.5.4/test/test_usi_engine.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.030838 cshogi-0.5.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-07 09:08:23.000000 cshogi-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-05-07 09:09:05.030838 cshogi-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5135 2023-05-07 09:08:23.000000 cshogi-0.5.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/
+-rw-rw-rw-   0        0        0     2774 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/CSA.py
+-rw-rw-rw-   0        0        0    18556 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/KI2.py
+-rw-rw-rw-   0        0        0    17360 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/KIF.py
+-rw-rw-rw-   0        0        0     2988 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/PGN.py
+-rw-rw-rw-   0        0        0       27 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/__init__.py
+-rw-rw-rw-   0        0        0    28993 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/_cshogi.pyx
+-rw-rw-rw-   0        0        0    25971 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/dlshogi/
+-rw-rw-rw-   0        0        0      327 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/dlshogi/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/elo.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/gym_shogi/
+-rw-rw-rw-   0        0        0      132 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/gym_shogi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/gym_shogi/envs/
+-rw-rw-rw-   0        0        0      118 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/gym_shogi/envs/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/gym_shogi/envs/shogi_env.pyx
+-rw-rw-rw-   0        0        0      755 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/gym_shogi/envs/shogi_vec_env.pyx
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/usi/
+-rw-rw-rw-   0        0        0     6725 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/usi/Engine.py
+-rw-rw-rw-   0        0        0       26 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/usi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/web/
+-rw-rw-rw-   0        0        0    13662 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/web/app.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/web/static/
+-rw-rw-rw-   0        0        0    13931 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/web/static/board.js
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/web/templates/
+-rw-rw-rw-   0        0        0    17362 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/web/templates/board.html
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-05-07 09:09:04.000000 cshogi-0.5.5/cshogi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-05-07 09:09:04.000000 cshogi-0.5.5/cshogi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 09:09:04.000000 cshogi-0.5.5/cshogi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 09:09:04.000000 cshogi-0.5.5/cshogi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 09:09:05.030838 cshogi-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     2006 2023-05-07 09:08:23.000000 cshogi-0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.030838 cshogi-0.5.5/src/
+-rw-rw-rw-   0        0        0     8208 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/bitboard.cpp
+-rw-rw-rw-   0        0        0     2225 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/book.cpp
+-rw-rw-rw-   0        0        0     1350 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/common.cpp
+-rw-rw-rw-   0        0        0    28484 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/dfpn.cpp
+-rw-rw-rw-   0        0        0    50568 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/generateMoves.cpp
+-rw-rw-rw-   0        0        0     1789 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/hand.cpp
+-rw-rw-rw-   0        0        0    19051 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/init.cpp
+-rw-rw-rw-   0        0        0     6937 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/mate.cpp
+-rw-rw-rw-   0        0        0     2163 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/move.cpp
+-rw-rw-rw-   0        0        0     1172 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/mt64bit.cpp
+-rw-rw-rw-   0        0        0   174059 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/position.cpp
+-rw-rw-rw-   0        0        0     3308 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/search.cpp
+-rw-rw-rw-   0        0        0     1416 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/square.cpp
+-rw-rw-rw-   0        0        0     6627 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/usi.cpp
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.030838 cshogi-0.5.5/test/
+-rw-rw-rw-   0        0        0      824 2023-05-07 09:08:23.000000 cshogi-0.5.5/test/test_usi_engine.py
```

### Comparing `cshogi-0.5.4/LICENSE` & `cshogi-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/README.rst` & `cshogi-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/CSA.py` & `cshogi-0.5.5/cshogi/CSA.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/KI2.py` & `cshogi-0.5.5/cshogi/KI2.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/KIF.py` & `cshogi-0.5.5/cshogi/KIF.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/PGN.py` & `cshogi-0.5.5/cshogi/PGN.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/_cshogi.pyx` & `cshogi-0.5.5/cshogi/_cshogi.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/cli.py` & `cshogi-0.5.5/cshogi/cli.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/elo.py` & `cshogi-0.5.5/cshogi/elo.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/gym_shogi/envs/shogi_env.pyx` & `cshogi-0.5.5/cshogi/gym_shogi/envs/shogi_env.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/gym_shogi/envs/shogi_vec_env.pyx` & `cshogi-0.5.5/cshogi/gym_shogi/envs/shogi_vec_env.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/usi/Engine.py` & `cshogi-0.5.5/cshogi/usi/Engine.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/web/app.py` & `cshogi-0.5.5/cshogi/web/app.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/web/static/board.js` & `cshogi-0.5.5/cshogi/web/static/board.js`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi/web/templates/board.html` & `cshogi-0.5.5/cshogi/web/templates/board.html`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/cshogi.egg-info/SOURCES.txt` & `cshogi-0.5.5/cshogi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/setup.py` & `cshogi-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     Extension('cshogi.gym_shogi.envs.shogi_vec_env',
         ['cshogi/gym_shogi/envs/shogi_vec_env.pyx'],
         language='c++'),
 ]
 
 setup(
     name='cshogi',
-    version='0.5.4',
+    version='0.5.5',
     packages=['cshogi', 'cshogi.usi', 'cshogi.gym_shogi', 'cshogi.gym_shogi.envs', 'cshogi.dlshogi', 'cshogi.web', 'cshogi.web.templates', 'cshogi.web.static'],
     package_data={'cshogi.web.templates': ['*'], 'cshogi.web.static': ['*']},
     ext_modules=ext_modules,
     cmdclass={'build_ext': my_build_ext},
     author='Tadao Yamaoka',
     url='https://github.com/TadaoYamaoka/cshogi',
     description = 'A fast Python shogi library',
```

### Comparing `cshogi-0.5.4/src/bitboard.cpp` & `cshogi-0.5.5/src/bitboard.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/book.cpp` & `cshogi-0.5.5/src/book.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/common.cpp` & `cshogi-0.5.5/src/common.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/dfpn.cpp` & `cshogi-0.5.5/src/dfpn.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/generateMoves.cpp` & `cshogi-0.5.5/src/generateMoves.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/hand.cpp` & `cshogi-0.5.5/src/hand.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/init.cpp` & `cshogi-0.5.5/src/init.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/mate.cpp` & `cshogi-0.5.5/src/mate.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/move.cpp` & `cshogi-0.5.5/src/move.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/mt64bit.cpp` & `cshogi-0.5.5/src/mt64bit.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/position.cpp` & `cshogi-0.5.5/src/position.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/search.cpp` & `cshogi-0.5.5/src/search.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/square.cpp` & `cshogi-0.5.5/src/square.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/src/usi.cpp` & `cshogi-0.5.5/src/usi.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.4/test/test_usi_engine.py` & `cshogi-0.5.5/test/test_usi_engine.py`

 * *Files identical despite different names*

