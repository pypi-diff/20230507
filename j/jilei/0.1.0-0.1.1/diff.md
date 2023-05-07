# Comparing `tmp/jilei-0.1.0.tar.gz` & `tmp/jilei-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jilei-0.1.0.tar", last modified: Sun May  7 09:32:09 2023, max compression
+gzip compressed data, was "dist\jilei-0.1.1.tar", last modified: Sun May  7 09:36:43 2023, max compression
```

## Comparing `jilei-0.1.0.tar` & `jilei-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 09:32:09.943514 jilei-0.1.0/
--rw-rw-rw-   0        0        0      448 2023-05-07 09:32:09.943514 jilei-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-07 08:49:40.000000 jilei-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 09:32:09.939511 jilei-0.1.0/jilei/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:09:34.000000 jilei-0.1.0/jilei/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-05-07 09:20:50.000000 jilei-0.1.0/jilei/docker_tools.py
--rw-rw-rw-   0        0        0     1006 2023-04-20 06:23:15.000000 jilei-0.1.0/jilei/nnunet_tools.py
--rw-rw-rw-   0        0        0     1210 2023-05-07 09:28:32.000000 jilei-0.1.0/jilei/system_tools.py
--rw-rw-rw-   0        0        0     1744 2023-04-12 12:32:46.000000 jilei-0.1.0/jilei/wxwork.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:32:09.943514 jilei-0.1.0/jilei.egg-info/
--rw-rw-rw-   0        0        0      448 2023-05-07 09:32:09.000000 jilei-0.1.0/jilei.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-05-07 09:32:09.000000 jilei-0.1.0/jilei.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 09:32:09.000000 jilei-0.1.0/jilei.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 09:32:09.000000 jilei-0.1.0/jilei.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 09:32:09.944515 jilei-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-05-07 09:32:09.000000 jilei-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:36:43.664660 jilei-0.1.1/
+-rw-rw-rw-   0        0        0      448 2023-05-07 09:36:43.664660 jilei-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-07 08:49:40.000000 jilei-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 09:36:43.660656 jilei-0.1.1/jilei/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:09:34.000000 jilei-0.1.1/jilei/__init__.py
+-rw-rw-rw-   0        0        0     2666 2023-05-07 09:36:16.000000 jilei-0.1.1/jilei/docker_tools.py
+-rw-rw-rw-   0        0        0     1006 2023-04-20 06:23:15.000000 jilei-0.1.1/jilei/nnunet_tools.py
+-rw-rw-rw-   0        0        0     1210 2023-05-07 09:28:32.000000 jilei-0.1.1/jilei/system_tools.py
+-rw-rw-rw-   0        0        0     1744 2023-04-12 12:32:46.000000 jilei-0.1.1/jilei/wxwork.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:36:43.663659 jilei-0.1.1/jilei.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-05-07 09:36:43.000000 jilei-0.1.1/jilei.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-07 09:36:43.000000 jilei-0.1.1/jilei.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 09:36:43.000000 jilei-0.1.1/jilei.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 09:36:43.000000 jilei-0.1.1/jilei.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 09:36:43.664660 jilei-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-05-07 09:36:43.000000 jilei-0.1.1/setup.py
```

### Comparing `jilei-0.1.0/jilei/nnunet_tools.py` & `jilei-0.1.1/jilei/nnunet_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.1.0/jilei/system_tools.py` & `jilei-0.1.1/jilei/system_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.1.0/jilei/wxwork.py` & `jilei-0.1.1/jilei/wxwork.py`

 * *Files identical despite different names*

### Comparing `jilei-0.1.0/setup.py` & `jilei-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jilei",
-    version="0.1.0",
+    version="0.1.1",
     author="jilei",
     author_email="developer@jlzn.cc",
     description="For internal use.",
     long_description="python setup.py bdist_wheel\ntwine upload ./dist/*",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

