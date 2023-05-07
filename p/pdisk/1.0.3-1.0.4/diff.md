# Comparing `tmp/pdisk-1.0.3.tar.gz` & `tmp/pdisk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdisk-1.0.3.tar", last modified: Sun May  7 06:27:04 2023, max compression
+gzip compressed data, was "pdisk-1.0.4.tar", last modified: Sun May  7 06:30:55 2023, max compression
```

## Comparing `pdisk-1.0.3.tar` & `pdisk-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 06:27:04.166945 pdisk-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-05-06 19:48:25.000000 pdisk-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2614 2023-05-07 06:27:04.166945 pdisk-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4288 2023-05-06 21:59:58.000000 pdisk-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 06:27:04.157564 pdisk-1.0.3/pdisk/
--rw-rw-rw-   0        0        0       26 2023-05-06 15:56:36.000000 pdisk-1.0.3/pdisk/__init__.py
--rw-rw-rw-   0        0        0    11369 2023-05-06 21:23:35.000000 pdisk-1.0.3/pdisk/pdisk.py
--rw-rw-rw-   0        0        0     2540 2023-05-06 18:03:15.000000 pdisk-1.0.3/pdisk/type.py
-drwxrwxrwx   0        0        0        0 2023-05-07 06:27:04.166945 pdisk-1.0.3/pdisk.egg-info/
--rw-rw-rw-   0        0        0     2614 2023-05-07 06:27:03.000000 pdisk-1.0.3/pdisk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-07 06:27:03.000000 pdisk-1.0.3/pdisk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 06:27:03.000000 pdisk-1.0.3/pdisk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 06:27:03.000000 pdisk-1.0.3/pdisk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 06:27:03.000000 pdisk-1.0.3/pdisk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 06:27:04.166945 pdisk-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-05-07 06:26:17.000000 pdisk-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:30:55.938193 pdisk-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-05-06 19:48:25.000000 pdisk-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2614 2023-05-07 06:30:55.938193 pdisk-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4288 2023-05-06 21:59:58.000000 pdisk-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 06:30:55.927433 pdisk-1.0.4/pdisk/
+-rw-rw-rw-   0        0        0       26 2023-05-06 15:56:36.000000 pdisk-1.0.4/pdisk/__init__.py
+-rw-rw-rw-   0        0        0    11369 2023-05-06 21:23:35.000000 pdisk-1.0.4/pdisk/pdisk.py
+-rw-rw-rw-   0        0        0     2540 2023-05-06 18:03:15.000000 pdisk-1.0.4/pdisk/type.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:30:55.938193 pdisk-1.0.4/pdisk.egg-info/
+-rw-rw-rw-   0        0        0     2614 2023-05-07 06:30:55.000000 pdisk-1.0.4/pdisk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-07 06:30:55.000000 pdisk-1.0.4/pdisk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 06:30:55.000000 pdisk-1.0.4/pdisk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 06:30:55.000000 pdisk-1.0.4/pdisk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 06:30:55.000000 pdisk-1.0.4/pdisk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 06:30:55.938193 pdisk-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2023-05-07 06:30:25.000000 pdisk-1.0.4/setup.py
```

### Comparing `pdisk-1.0.3/LICENSE` & `pdisk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdisk-1.0.3/PKG-INFO` & `pdisk-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdisk
-Version: 1.0.3
+Version: 1.0.4
 Summary: An Unofficial Asynchronous Python version of pdisk API wrapper
 Home-page: https://github.com/kalanakt/pdisk
 Author: kalanakt
 Author-email: kalanakt@uvew.xyz
 License: MIT
 Keywords: python,pdisk,earn money 
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pdisk-1.0.3/README.md` & `pdisk-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pdisk-1.0.3/pdisk/pdisk.py` & `pdisk-1.0.4/pdisk/pdisk.py`

 * *Files identical despite different names*

### Comparing `pdisk-1.0.3/pdisk/type.py` & `pdisk-1.0.4/pdisk/type.py`

 * *Files identical despite different names*

### Comparing `pdisk-1.0.3/pdisk.egg-info/PKG-INFO` & `pdisk-1.0.4/pdisk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdisk
-Version: 1.0.3
+Version: 1.0.4
 Summary: An Unofficial Asynchronous Python version of pdisk API wrapper
 Home-page: https://github.com/kalanakt/pdisk
 Author: kalanakt
 Author-email: kalanakt@uvew.xyz
 License: MIT
 Keywords: python,pdisk,earn money 
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pdisk-1.0.3/setup.py` & `pdisk-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "package.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'An Unofficial Asynchronous Python version of pdisk API wrapper'
 
 # Setting up
 setup(
     name="pdisk",
     version=VERSION,
     author="kalanakt",
```

