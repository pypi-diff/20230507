# Comparing `tmp/pdcscore-1.1.2.tar.gz` & `tmp/pdcscore-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.1.2.tar", last modified: Sun May  7 01:35:03 2023, max compression
+gzip compressed data, was "pdcscore-1.1.3.tar", last modified: Sun May  7 01:42:35 2023, max compression
```

## Comparing `pdcscore-1.1.2.tar` & `pdcscore-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 01:35:03.433900 pdcscore-1.1.2/
--rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     5604 2023-05-07 01:35:03.431900 pdcscore-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4321 2023-05-07 01:22:27.000000 pdcscore-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 01:35:03.416704 pdcscore-1.1.2/pdcscore/
--rw-rw-rw-   0        0        0       79 2023-05-07 01:32:59.000000 pdcscore-1.1.2/pdcscore/__init__.py
--rw-rw-rw-   0        0        0     3523 2023-05-07 01:22:49.000000 pdcscore-1.1.2/pdcscore/pdcscore.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:35:03.430899 pdcscore-1.1.2/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     5604 2023-05-07 01:35:03.000000 pdcscore-1.1.2/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-07 01:35:03.000000 pdcscore-1.1.2/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 01:35:03.000000 pdcscore-1.1.2/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 01:35:03.000000 pdcscore-1.1.2/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 01:35:03.000000 pdcscore-1.1.2/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 01:35:03.434901 pdcscore-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1602 2023-05-07 01:33:23.000000 pdcscore-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:42:35.635275 pdcscore-1.1.3/
+-rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5604 2023-05-07 01:42:35.635275 pdcscore-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4321 2023-05-07 01:22:27.000000 pdcscore-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 01:42:35.617275 pdcscore-1.1.3/pdcscore/
+-rw-rw-rw-   0        0        0       79 2023-05-07 01:41:34.000000 pdcscore-1.1.3/pdcscore/__init__.py
+-rw-rw-rw-   0        0        0     3523 2023-05-07 01:22:49.000000 pdcscore-1.1.3/pdcscore/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:42:35.633275 pdcscore-1.1.3/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     5604 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 01:42:35.635275 pdcscore-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1602 2023-05-07 01:41:49.000000 pdcscore-1.1.3/setup.py
```

### Comparing `pdcscore-1.1.2/LICENSE` & `pdcscore-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.1.2/PKG-INFO` & `pdcscore-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: https://github.com/famutimine/pdcscore
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
```

### Comparing `pdcscore-1.1.2/README.md` & `pdcscore-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pdcscore-1.1.2/pdcscore/pdcscore.py` & `pdcscore-1.1.3/pdcscore/pdcscore.py`

 * *Files identical despite different names*

### Comparing `pdcscore-1.1.2/pdcscore.egg-info/PKG-INFO` & `pdcscore-1.1.3/pdcscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: https://github.com/famutimine/pdcscore
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
```

### Comparing `pdcscore-1.1.2/setup.py` & `pdcscore-1.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdcscore',
-    version='1.1.2',
+    version='1.1.3',
     description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/famutimine/pdcscore',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

