# Comparing `tmp/pdcscore-1.1.0.tar.gz` & `tmp/pdcscore-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.1.0.tar", last modified: Fri May  5 20:35:08 2023, max compression
+gzip compressed data, was "pdcscore-1.1.1.tar", last modified: Sun May  7 01:24:24 2023, max compression
```

## Comparing `pdcscore-1.1.0.tar` & `pdcscore-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 20:35:08.147213 pdcscore-1.1.0/
--rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4963 2023-05-05 20:35:08.146213 pdcscore-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3688 2023-05-04 17:21:47.000000 pdcscore-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 20:35:08.122213 pdcscore-1.1.0/pdcscore/
--rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.1.0/pdcscore/__init__.py
--rw-rw-rw-   0        0        0     3524 2023-05-05 20:23:41.000000 pdcscore-1.1.0/pdcscore/pdcscore.py
-drwxrwxrwx   0        0        0        0 2023-05-05 20:35:08.144212 pdcscore-1.1.0/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     4963 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 20:35:08.000000 pdcscore-1.1.0/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 20:35:08.147213 pdcscore-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1602 2023-05-05 20:32:31.000000 pdcscore-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:24:24.665067 pdcscore-1.1.1/
+-rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5604 2023-05-07 01:24:24.664067 pdcscore-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4321 2023-05-07 01:22:27.000000 pdcscore-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 01:24:24.643953 pdcscore-1.1.1/pdcscore/
+-rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.1.1/pdcscore/__init__.py
+-rw-rw-rw-   0        0        0     3523 2023-05-07 01:22:49.000000 pdcscore-1.1.1/pdcscore/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:24:24.663068 pdcscore-1.1.1/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     5604 2023-05-07 01:24:24.000000 pdcscore-1.1.1/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-07 01:24:24.000000 pdcscore-1.1.1/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 01:24:24.000000 pdcscore-1.1.1/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 01:24:24.000000 pdcscore-1.1.1/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 01:24:24.000000 pdcscore-1.1.1/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 01:24:24.665067 pdcscore-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1602 2023-05-07 01:15:04.000000 pdcscore-1.1.1/setup.py
```

### Comparing `pdcscore-1.1.0/LICENSE` & `pdcscore-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.1.0/setup.py` & `pdcscore-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdcscore',
-    version='1.1.0',
+    version='1.1.1',
     description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/famutimine/pdcscore',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

