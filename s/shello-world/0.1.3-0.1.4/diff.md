# Comparing `tmp/shello_world-0.1.3.tar.gz` & `tmp/shello_world-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shello_world-0.1.3.tar", max compression
+gzip compressed data, was "shello_world-0.1.4.tar", max compression
```

## Comparing `shello_world-0.1.3.tar` & `shello_world-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      666 2023-05-07 20:19:36.842148 shello_world-0.1.3/LICENSE
--rw-r--r--   0        0        0     1204 2023-05-07 20:54:57.626586 shello_world-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1185 2023-05-07 20:54:46.932388 shello_world-0.1.3/README.md
--rw-r--r--   0        0        0       52 2023-05-07 20:19:36.842148 shello_world-0.1.3/shello_world/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 20:19:36.842148 shello_world-0.1.3/shello_world/shello_world.py
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 shello_world-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      666 2023-05-07 20:19:36.842148 shello_world-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1204 2023-05-07 21:18:59.996740 shello_world-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1187 2023-05-07 21:18:46.241686 shello_world-0.1.4/README.md
+-rw-r--r--   0        0        0       52 2023-05-07 20:19:36.842148 shello_world-0.1.4/shello_world/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 20:19:36.842148 shello_world-0.1.4/shello_world/shello_world.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 shello_world-0.1.4/PKG-INFO
```

### Comparing `shello_world-0.1.3/LICENSE` & `shello_world-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shello_world-0.1.3/pyproject.toml` & `shello_world-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shello-world"
-version = "0.1.3"
+version = "0.1.4"
 description = "A few simple Python functions allow you to run shell commands from your Python code"
 authors = ["numericmaestro <re5lyltx@duck.com>"]
 readme = "README.md"
 license = "0BSD"
 homepage = "https://github.com/numericmaestro/shello-world"
 repository = "https://github.com/numericmaestro/shello-world"
 keywords = ["shell"]
```

### Comparing `shello_world-0.1.3/README.md` & `shello_world-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Shello-world: run shell commands from your Python code via simple functions
-A few simple Python functions allow you to run shell commands from your Python code
+A few simple Python functions allow you to run shell commands from your Python code.
 
 ## Why shello-world?
 It isn't a big library or framework. If you want a quick solution, you could prefer shello-world.
 
 ## Usage
-Let's take a look at a simple example below
+Let's take a look at a simple example below:
 ```python
 from shello_world import shell_execute, shell_run
 
 # Both functions work similarly
 
 # shell_run runs a command directly in your shell
 # Change color to green
```

### Comparing `shello_world-0.1.3/shello_world/shello_world.py` & `shello_world-0.1.4/shello_world/shello_world.py`

 * *Files identical despite different names*

### Comparing `shello_world-0.1.3/PKG-INFO` & `shello_world-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shello-world
-Version: 0.1.3
+Version: 0.1.4
 Summary: A few simple Python functions allow you to run shell commands from your Python code
 Home-page: https://github.com/numericmaestro/shello-world
 License: 0BSD
 Keywords: shell
 Author: numericmaestro
 Author-email: re5lyltx@duck.com
 Requires-Python: >=3.11,<4.0
@@ -23,21 +23,21 @@
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: System :: Systems Administration
 Project-URL: Repository, https://github.com/numericmaestro/shello-world
 Description-Content-Type: text/markdown
 
 # Shello-world: run shell commands from your Python code via simple functions
-A few simple Python functions allow you to run shell commands from your Python code
+A few simple Python functions allow you to run shell commands from your Python code.
 
 ## Why shello-world?
 It isn't a big library or framework. If you want a quick solution, you could prefer shello-world.
 
 ## Usage
-Let's take a look at a simple example below
+Let's take a look at a simple example below:
 ```python
 from shello_world import shell_execute, shell_run
 
 # Both functions work similarly
 
 # shell_run runs a command directly in your shell
 # Change color to green
```

