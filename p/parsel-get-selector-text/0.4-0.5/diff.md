# Comparing `tmp/parsel_get_selector_text-0.4.tar.gz` & `tmp/parsel_get_selector_text-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsel_get_selector_text-0.4.tar", last modified: Sun May  7 21:15:38 2023, max compression
+gzip compressed data, was "parsel_get_selector_text-0.5.tar", last modified: Sun May  7 21:18:27 2023, max compression
```

## Comparing `parsel_get_selector_text-0.4.tar` & `parsel_get_selector_text-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-07 21:15:38.611670 parsel_get_selector_text-0.4/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1089 2023-04-23 23:41:13.000000 parsel_get_selector_text-0.4/LICENSE
--rw-r--r--   0 andrei    (1000) andrei    (1000)      700 2023-05-07 21:15:38.611670 parsel_get_selector_text-0.4/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-23 22:53:37.000000 parsel_get_selector_text-0.4/README.md
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-07 21:15:38.608337 parsel_get_selector_text-0.4/parsel_get_selector_text/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2445 2023-05-06 20:05:07.000000 parsel_get_selector_text-0.4/parsel_get_selector_text/__init__.py
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-07 21:15:38.611670 parsel_get_selector_text-0.4/parsel_get_selector_text.egg-info/
--rw-r--r--   0 andrei    (1000) andrei    (1000)      700 2023-05-07 21:15:38.000000 parsel_get_selector_text-0.4/parsel_get_selector_text.egg-info/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)      317 2023-05-07 21:15:38.000000 parsel_get_selector_text-0.4/parsel_get_selector_text.egg-info/SOURCES.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2023-05-07 21:15:38.000000 parsel_get_selector_text-0.4/parsel_get_selector_text.egg-info/dependency_links.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       27 2023-05-07 21:15:38.000000 parsel_get_selector_text-0.4/parsel_get_selector_text.egg-info/requires.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       25 2023-05-07 21:15:38.000000 parsel_get_selector_text-0.4/parsel_get_selector_text.egg-info/top_level.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-24 01:01:58.000000 parsel_get_selector_text-0.4/pyproject.toml
--rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2023-05-07 21:15:38.611670 parsel_get_selector_text-0.4/setup.cfg
--rw-r--r--   0 andrei    (1000) andrei    (1000)      953 2023-05-07 21:14:42.000000 parsel_get_selector_text-0.4/setup.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-07 21:18:27.469649 parsel_get_selector_text-0.5/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1089 2023-04-23 23:41:13.000000 parsel_get_selector_text-0.5/LICENSE
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      700 2023-05-07 21:18:27.469649 parsel_get_selector_text-0.5/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-23 22:53:37.000000 parsel_get_selector_text-0.5/README.md
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-07 21:18:27.466316 parsel_get_selector_text-0.5/parsel_get_selector_text/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2445 2023-05-06 20:05:07.000000 parsel_get_selector_text-0.5/parsel_get_selector_text/__init__.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-07 21:18:27.469649 parsel_get_selector_text-0.5/parsel_get_selector_text.egg-info/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      700 2023-05-07 21:18:27.000000 parsel_get_selector_text-0.5/parsel_get_selector_text.egg-info/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      317 2023-05-07 21:18:27.000000 parsel_get_selector_text-0.5/parsel_get_selector_text.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2023-05-07 21:18:27.000000 parsel_get_selector_text-0.5/parsel_get_selector_text.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       27 2023-05-07 21:18:27.000000 parsel_get_selector_text-0.5/parsel_get_selector_text.egg-info/requires.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       25 2023-05-07 21:18:27.000000 parsel_get_selector_text-0.5/parsel_get_selector_text.egg-info/top_level.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-24 01:01:58.000000 parsel_get_selector_text-0.5/pyproject.toml
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2023-05-07 21:18:27.469649 parsel_get_selector_text-0.5/setup.cfg
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      953 2023-05-07 21:17:47.000000 parsel_get_selector_text-0.5/setup.py
```

### Comparing `parsel_get_selector_text-0.4/LICENSE` & `parsel_get_selector_text-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `parsel_get_selector_text-0.4/PKG-INFO` & `parsel_get_selector_text-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsel_get_selector_text
-Version: 0.4
+Version: 0.5
 Summary: Extracts all text results from an XPath query on a parsel Selector object.
 Home-page: https://github.com/carlosplanchon/parsel_get_selector_text
 Author: Carlos A. Planchón
 Author-email: carlosandresplanchonprestes@gmail.com
 License: MIT
 Keywords: dom,parsel,scraping,xpath
 Classifier: Intended Audience :: Developers
```

### Comparing `parsel_get_selector_text-0.4/parsel_get_selector_text/__init__.py` & `parsel_get_selector_text-0.5/parsel_get_selector_text/__init__.py`

 * *Files identical despite different names*

### Comparing `parsel_get_selector_text-0.4/parsel_get_selector_text.egg-info/PKG-INFO` & `parsel_get_selector_text-0.5/parsel_get_selector_text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsel-get-selector-text
-Version: 0.4
+Version: 0.5
 Summary: Extracts all text results from an XPath query on a parsel Selector object.
 Home-page: https://github.com/carlosplanchon/parsel_get_selector_text
 Author: Carlos A. Planchón
 Author-email: carlosandresplanchonprestes@gmail.com
 License: MIT
 Keywords: dom,parsel,scraping,xpath
 Classifier: Intended Audience :: Developers
```

### Comparing `parsel_get_selector_text-0.4/setup.py` & `parsel_get_selector_text-0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="parsel_get_selector_text",
     packages=find_packages(),
-    version="0.4",
+    version="0.5",
     license="MIT",
     description="Extracts all text results from an XPath "\
         "query on a parsel Selector object.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Carlos A. Planchón",
     author_email="carlosandresplanchonprestes@gmail.com",
```

