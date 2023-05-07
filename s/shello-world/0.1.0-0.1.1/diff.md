# Comparing `tmp/shello_world-0.1.0.tar.gz` & `tmp/shello_world-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shello_world-0.1.0.tar", max compression
+gzip compressed data, was "shello_world-0.1.1.tar", max compression
```

## Comparing `shello_world-0.1.0.tar` & `shello_world-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      666 2023-05-07 10:46:08.018580 shello_world-0.1.0/LICENSE
--rw-r--r--   0        0        0     1204 2023-05-07 20:06:27.204301 shello_world-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1064 2023-05-07 20:07:23.424265 shello_world-0.1.0/README.md
--rw-r--r--   0        0        0       52 2023-05-07 20:10:21.723734 shello_world-0.1.0/shello_world/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 13:50:07.806886 shello_world-0.1.0/shello_world/shello_world.py
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 shello_world-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      666 2023-05-07 10:46:08.018580 shello_world-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1204 2023-05-07 20:17:29.738025 shello_world-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1065 2023-05-07 20:13:16.685281 shello_world-0.1.1/README.md
+-rw-r--r--   0        0        0       52 2023-05-07 20:10:21.723734 shello_world-0.1.1/shello_world/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 13:50:07.806886 shello_world-0.1.1/shello_world/shello_world.py
+-rw-r--r--   0        0        0     2286 1970-01-01 00:00:00.000000 shello_world-0.1.1/PKG-INFO
```

### Comparing `shello_world-0.1.0/LICENSE` & `shello_world-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shello_world-0.1.0/pyproject.toml` & `shello_world-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shello-world"
-version = "0.1.0"
+version = "0.1.1"
 description = "A few simple Python functions allow you to run shell commands from your Python code"
 authors = ["numericmaestro <re5lyltx@duck.com>"]
 readme = "README.md"
 license = "0BSD"
 homepage = "https://github.com/numericmaestro/shello-world"
 repository = "https://github.com/numericmaestro/shello-world"
 keywords = ["shell"]
```

### Comparing `shello_world-0.1.0/README.md` & `shello_world-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 systeminfo = shell_execute("systeminfo") # This line doesn't print anything
 # But it always returns result as a string
 print(systeminfo.upper())
 print(systeminfo.split())
 ```
 
 ## Installation
-You can install this library with ```pip install shello-world`` command.
+You can install this library with ```pip install shello-world``` command.
```

### Comparing `shello_world-0.1.0/shello_world/shello_world.py` & `shello_world-0.1.1/shello_world/shello_world.py`

 * *Files identical despite different names*

### Comparing `shello_world-0.1.0/PKG-INFO` & `shello_world-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shello-world
-Version: 0.1.0
+Version: 0.1.1
 Summary: A few simple Python functions allow you to run shell commands from your Python code
 Home-page: https://github.com/numericmaestro/shello-world
 License: 0BSD
 Keywords: shell
 Author: numericmaestro
 Author-email: re5lyltx@duck.com
 Requires-Python: >=3.11,<4.0
@@ -51,8 +51,8 @@
 systeminfo = shell_execute("systeminfo") # This line doesn't print anything
 # But it always returns result as a string
 print(systeminfo.upper())
 print(systeminfo.split())
 ```
 
 ## Installation
-You can install this library with ```pip install shello-world`` command.
+You can install this library with ```pip install shello-world``` command.
```

