# Comparing `tmp/jilei-0.0.8.tar.gz` & `tmp/jilei-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jilei-0.0.8.tar", last modified: Sun May  7 09:00:39 2023, max compression
+gzip compressed data, was "dist\jilei-0.0.9.tar", last modified: Sun May  7 09:09:10 2023, max compression
```

## Comparing `jilei-0.0.8.tar` & `jilei-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 09:00:39.077004 jilei-0.0.8/
--rw-rw-rw-   0        0        0      448 2023-05-07 09:00:39.076004 jilei-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-07 08:49:40.000000 jilei-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 09:00:39.068997 jilei-0.0.8/jilei/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:09:34.000000 jilei-0.0.8/jilei/__init__.py
--rw-rw-rw-   0        0        0       54 2023-05-07 09:00:26.000000 jilei-0.0.8/jilei/docker_tools.py
--rw-rw-rw-   0        0        0     1006 2023-04-20 06:23:15.000000 jilei-0.0.8/jilei/nnunet_tools.py
--rw-rw-rw-   0        0        0     1123 2023-05-07 08:59:35.000000 jilei-0.0.8/jilei/system_tools.py
--rw-rw-rw-   0        0        0     1744 2023-04-12 12:32:46.000000 jilei-0.0.8/jilei/wxwork.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:00:39.076004 jilei-0.0.8/jilei.egg-info/
--rw-rw-rw-   0        0        0      448 2023-05-07 09:00:39.000000 jilei-0.0.8/jilei.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-05-07 09:00:39.000000 jilei-0.0.8/jilei.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 09:00:39.000000 jilei-0.0.8/jilei.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 09:00:39.000000 jilei-0.0.8/jilei.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 09:00:39.077004 jilei-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-05-07 09:00:38.000000 jilei-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:10.348440 jilei-0.0.9/
+-rw-rw-rw-   0        0        0      448 2023-05-07 09:09:10.348440 jilei-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-07 08:49:40.000000 jilei-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:10.339431 jilei-0.0.9/jilei/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:09:34.000000 jilei-0.0.9/jilei/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-05-07 09:06:02.000000 jilei-0.0.9/jilei/docker_tools.py
+-rw-rw-rw-   0        0        0     1006 2023-04-20 06:23:15.000000 jilei-0.0.9/jilei/nnunet_tools.py
+-rw-rw-rw-   0        0        0     1123 2023-05-07 08:59:35.000000 jilei-0.0.9/jilei/system_tools.py
+-rw-rw-rw-   0        0        0     1744 2023-04-12 12:32:46.000000 jilei-0.0.9/jilei/wxwork.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:09:10.347438 jilei-0.0.9/jilei.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-05-07 09:09:10.000000 jilei-0.0.9/jilei.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-07 09:09:10.000000 jilei-0.0.9/jilei.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 09:09:10.000000 jilei-0.0.9/jilei.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 09:09:10.000000 jilei-0.0.9/jilei.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 09:09:10.348440 jilei-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-05-07 09:09:10.000000 jilei-0.0.9/setup.py
```

### Comparing `jilei-0.0.8/jilei/nnunet_tools.py` & `jilei-0.0.9/jilei/nnunet_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.0.8/jilei/system_tools.py` & `jilei-0.0.9/jilei/system_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.0.8/jilei/wxwork.py` & `jilei-0.0.9/jilei/wxwork.py`

 * *Files identical despite different names*

### Comparing `jilei-0.0.8/setup.py` & `jilei-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jilei",
-    version="0.0.8",
+    version="0.0.9",
     author="jilei",
     author_email="developer@jlzn.cc",
     description="For internal use.",
     long_description="python setup.py bdist_wheel\ntwine upload ./dist/*",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

