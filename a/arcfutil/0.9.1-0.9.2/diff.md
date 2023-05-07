# Comparing `tmp/arcfutil-0.9.1.tar.gz` & `tmp/arcfutil-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcfutil-0.9.1.tar", last modified: Sun Jan  8 04:58:15 2023, max compression
+gzip compressed data, was "arcfutil-0.9.2.tar", last modified: Sun May  7 09:40:54 2023, max compression
```

## Comparing `arcfutil-0.9.1.tar` & `arcfutil-0.9.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.759279 arcfutil-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-08 04:58:08.000000 arcfutil-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-01-08 04:58:15.759279 arcfutil-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-01-08 04:58:08.000000 arcfutil-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 04:58:15.759279 arcfutil-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-08 04:58:08.000000 arcfutil-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.755279 arcfutil-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.755279 arcfutil-0.9.1/src/arcfutil/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.759279 arcfutil-0.9.1/src/arcfutil/aff/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.759279 arcfutil-0.9.1/src/arcfutil/aff/easing/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/easing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/easing/cheatsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.759279 arcfutil-0.9.1/src/arcfutil/aff/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/generator/arc_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/generator/timing_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.759279 arcfutil-0.9.1/src/arcfutil/aff/note/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/common_note.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/flick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/notegroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/scenecontrol.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/tap.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/note/validstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/aff/sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.759279 arcfutil-0.9.1/src/arcfutil/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/cli/arcade_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/cli/songlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/cli/sortassets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.759279 arcfutil-0.9.1/src/arcfutil/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-08 04:58:08.000000 arcfutil-0.9.1/src/arcfutil/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 04:58:15.759279 arcfutil-0.9.1/src/arcfutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-01-08 04:58:15.000000 arcfutil-0.9.1/src/arcfutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-08 04:58:15.000000 arcfutil-0.9.1/src/arcfutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 04:58:15.000000 arcfutil-0.9.1/src/arcfutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-08 04:58:15.000000 arcfutil-0.9.1/src/arcfutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 04:58:15.000000 arcfutil-0.9.1/src/arcfutil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-08 04:58:15.000000 arcfutil-0.9.1/src/arcfutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-07 09:40:41.000000 arcfutil-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-07 09:40:54.037000 arcfutil-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-07 09:40:41.000000 arcfutil-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 09:40:54.037000 arcfutil-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-07 09:40:41.000000 arcfutil-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.033000 arcfutil-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/src/arcfutil/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/src/arcfutil/aff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/src/arcfutil/aff/easing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/easing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/easing/cheatsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/src/arcfutil/aff/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/generator/arc_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/generator/timing_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/src/arcfutil/aff/note/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/common_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/flick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/notegroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/scenecontrol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/note/validstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/aff/sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/src/arcfutil/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/cli/arcade_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/cli/songlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/cli/sortassets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/src/arcfutil/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-07 09:40:41.000000 arcfutil-0.9.2/src/arcfutil/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:54.037000 arcfutil-0.9.2/src/arcfutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-07 09:40:53.000000 arcfutil-0.9.2/src/arcfutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 09:40:54.000000 arcfutil-0.9.2/src/arcfutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:40:53.000000 arcfutil-0.9.2/src/arcfutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-07 09:40:53.000000 arcfutil-0.9.2/src/arcfutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:40:53.000000 arcfutil-0.9.2/src/arcfutil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 09:40:53.000000 arcfutil-0.9.2/src/arcfutil.egg-info/top_level.txt
```

### Comparing `arcfutil-0.9.1/LICENSE` & `arcfutil-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/PKG-INFO` & `arcfutil-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcfutil
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python module designed for processing Arcaea related files(.aff chart, songlist, etc.)
 Home-page: https://github.com/feightwywx/arcfutil
 Author: .direwolf
 Author-email: kururinmiracle@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcfutil-0.9.1/README.md` & `arcfutil-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/setup.py` & `arcfutil-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_namespace_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcfutil",
-    version="0.9.1",
+    version="0.9.2",
     author=".direwolf",
     author_email="kururinmiracle@outlook.com",
     description="A Python module designed for processing Arcaea related files(.aff chart, songlist, etc.)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/feightwywx/arcfutil",
     packages=find_namespace_packages('src', include=['arcfutil.*']),
```

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/__init__.py` & `arcfutil-0.9.2/src/arcfutil/aff/__init__.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/easing/__init__.py` & `arcfutil-0.9.2/src/arcfutil/aff/easing/__init__.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/easing/cheatsheet.py` & `arcfutil-0.9.2/src/arcfutil/aff/easing/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/generator/arc_sample.py` & `arcfutil-0.9.2/src/arcfutil/aff/generator/arc_sample.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/generator/timing_sample.py` & `arcfutil-0.9.2/src/arcfutil/aff/generator/timing_sample.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/arc.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/arc.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,19 @@
         if self.skynote:
             for each in enumerate(self.skynote):
                 self.skynote[each[0]] += value
         return self
         
     def align(self, bpm: float, error: int = 3, lcm = 96):
         super(Arc, self).align(bpm, error, lcm)
+        # 防止单天键出 bug
+        if self.time == self.totime:
+            if self.skynote:
+                self.totime += 1
+        
         if self.skynote:
             for each in enumerate(self.skynote):
                 self.skynote[each[0]] = time_align(self.skynote[each[0]], bpm, error, lcm)
         return self
     
     def transfer(self, x_value: float, y_value: float):
         self.fromx += x_value
```

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/camera.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/camera.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/common_note.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/common_note.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 # -*- coding: UTF-8 -*-
 
 # Author: .direwolf <kururinmiracle@outlook.com>
 # Licensed under the MIT License.
 
 from copy import deepcopy
 from typing import Iterable
-
+import math
 
 def time_align(time: int, bpm: float, error: int = 3, lcm = 96):
     fpb = 60000 * 4 / bpm / lcm
     alignedTime = 0
-    atime1 = round(time//fpb*fpb) #向下取grid时间戳
-    atime2 = round((time//fpb+1)*fpb) #向上取grid时间戳
+    # atime1 = round(time//fpb*fpb) #向下取grid时间戳
+    # atime2 = round((time//fpb+1)*fpb) #向上取grid时间戳
+    # 因为 sb616 在游戏本体里用的好像是向下取整，所以这里用 floor 好了
+    atime1 = math.floor(time//fpb*fpb) #向下取grid时间戳
+    atime2 = math.floor((time//fpb+1)*fpb) #向上取grid时间戳
     abs1 = abs(time - atime1) #atime1与time的距离
     abs2 = abs(time - atime2)
     ok1 = (abs1 <= error) #abs1是否在容差内
     ok2 = (abs2 <= error)
     if ok1 & ok2:
         #哪个距离小就用哪个
         if abs1 > abs2:
```

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/flick.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/flick.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/hold.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/hold.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,10 +71,10 @@
         super(Hold, self).offsetto(value)
         self.totime += value
         return self
         
     def align(self, bpm: float, error: int = 3, lcm = 96):
         super(Hold, self).align(bpm, error, lcm)
         self.totime = time_align(self.totime, bpm, error, lcm)
-        if self.time == self.totime:
-            self.totime += 1
+        # if self.time == self.totime:
+        #    self.totime += 1
         return self
```

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/notegroup.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/notegroup.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/scenecontrol.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/scenecontrol.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/tap.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/tap.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/note/validstrings.py` & `arcfutil-0.9.2/src/arcfutil/aff/note/validstrings.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/parser.py` & `arcfutil-0.9.2/src/arcfutil/aff/parser.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/aff/sorter.py` & `arcfutil-0.9.2/src/arcfutil/aff/sorter.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/cli/arcade_clean.py` & `arcfutil-0.9.2/src/arcfutil/cli/arcade_clean.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/cli/cli.py` & `arcfutil-0.9.2/src/arcfutil/cli/cli.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/cli/songlist.py` & `arcfutil-0.9.2/src/arcfutil/cli/songlist.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil/cli/sortassets.py` & `arcfutil-0.9.2/src/arcfutil/cli/sortassets.py`

 * *Files identical despite different names*

### Comparing `arcfutil-0.9.1/src/arcfutil.egg-info/PKG-INFO` & `arcfutil-0.9.2/src/arcfutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcfutil
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python module designed for processing Arcaea related files(.aff chart, songlist, etc.)
 Home-page: https://github.com/feightwywx/arcfutil
 Author: .direwolf
 Author-email: kururinmiracle@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcfutil-0.9.1/src/arcfutil.egg-info/SOURCES.txt` & `arcfutil-0.9.2/src/arcfutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

