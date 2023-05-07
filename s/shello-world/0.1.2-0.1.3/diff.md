# Comparing `tmp/shello_world-0.1.2.tar.gz` & `tmp/shello_world-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shello_world-0.1.2.tar", max compression
+gzip compressed data, was "shello_world-0.1.3.tar", max compression
```

## Comparing `shello_world-0.1.2.tar` & `shello_world-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      666 2023-05-07 20:19:36.842148 shello_world-0.1.2/LICENSE
--rw-r--r--   0        0        0     1204 2023-05-07 20:52:47.365892 shello_world-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1183 2023-05-07 20:52:32.335772 shello_world-0.1.2/README.md
--rw-r--r--   0        0        0       52 2023-05-07 20:19:36.842148 shello_world-0.1.2/shello_world/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 20:19:36.842148 shello_world-0.1.2/shello_world/shello_world.py
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 shello_world-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      666 2023-05-07 20:19:36.842148 shello_world-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1204 2023-05-07 20:54:57.626586 shello_world-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-05-07 20:54:46.932388 shello_world-0.1.3/README.md
+-rw-r--r--   0        0        0       52 2023-05-07 20:19:36.842148 shello_world-0.1.3/shello_world/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 20:19:36.842148 shello_world-0.1.3/shello_world/shello_world.py
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 shello_world-0.1.3/PKG-INFO
```

### Comparing `shello_world-0.1.2/LICENSE` & `shello_world-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shello_world-0.1.2/pyproject.toml` & `shello_world-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shello-world"
-version = "0.1.2"
+version = "0.1.3"
 description = "A few simple Python functions allow you to run shell commands from your Python code"
 authors = ["numericmaestro <re5lyltx@duck.com>"]
 readme = "README.md"
 license = "0BSD"
 homepage = "https://github.com/numericmaestro/shello-world"
 repository = "https://github.com/numericmaestro/shello-world"
 keywords = ["shell"]
```

### Comparing `shello_world-0.1.2/README.md` & `shello_world-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 print(systeminfo.split())
 ```
 
 ## Installation
 You can install this library with ```pip install shello-world``` command.
 
 ## Links
-[PyPI](https://pypi.org/project/shello-world/)
+[PyPI](https://pypi.org/project/shello-world/)  
 [GitHub](https://github.com/numericmaestro/shello-world)
```

### Comparing `shello_world-0.1.2/shello_world/shello_world.py` & `shello_world-0.1.3/shello_world/shello_world.py`

 * *Files identical despite different names*

### Comparing `shello_world-0.1.2/PKG-INFO` & `shello_world-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shello-world
-Version: 0.1.2
+Version: 0.1.3
 Summary: A few simple Python functions allow you to run shell commands from your Python code
 Home-page: https://github.com/numericmaestro/shello-world
 License: 0BSD
 Keywords: shell
 Author: numericmaestro
 Author-email: re5lyltx@duck.com
 Requires-Python: >=3.11,<4.0
@@ -54,9 +54,9 @@
 print(systeminfo.split())
 ```
 
 ## Installation
 You can install this library with ```pip install shello-world``` command.
 
 ## Links
-[PyPI](https://pypi.org/project/shello-world/)
+[PyPI](https://pypi.org/project/shello-world/)  
 [GitHub](https://github.com/numericmaestro/shello-world)
```

