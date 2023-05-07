# Comparing `tmp/ecg_quality-0.1.1.tar.gz` & `tmp/ecg_quality-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecg_quality-0.1.1.tar", last modified: Sat May  6 23:18:34 2023, max compression
+gzip compressed data, was "ecg_quality-0.1.2.tar", last modified: Sun May  7 01:23:28 2023, max compression
```

## Comparing `ecg_quality-0.1.1.tar` & `ecg_quality-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 23:18:34.564142 ecg_quality-0.1.1/
--rw-rw-rw-   0        0        0    35149 2023-04-21 20:39:12.000000 ecg_quality-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      416 2023-05-06 23:18:34.565141 ecg_quality-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-04-21 20:39:12.000000 ecg_quality-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 23:18:34.542821 ecg_quality-0.1.1/ecg_quality/
-drwxrwxrwx   0        0        0        0 2023-05-06 23:18:34.563106 ecg_quality-0.1.1/ecg_quality/ecg_quality.egg-info/
--rw-rw-rw-   0        0        0      416 2023-05-06 23:18:34.000000 ecg_quality-0.1.1/ecg_quality/ecg_quality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-06 23:18:34.000000 ecg_quality-0.1.1/ecg_quality/ecg_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 23:18:34.000000 ecg_quality-0.1.1/ecg_quality/ecg_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-06 23:18:34.000000 ecg_quality-0.1.1/ecg_quality/ecg_quality.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 23:18:34.000000 ecg_quality-0.1.1/ecg_quality/ecg_quality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-06 23:18:34.566108 ecg_quality-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-05-06 23:12:45.000000 ecg_quality-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:23:28.818211 ecg_quality-0.1.2/
+-rw-rw-rw-   0        0        0    35149 2023-04-21 20:39:12.000000 ecg_quality-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      416 2023-05-07 01:23:28.818211 ecg_quality-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-04-21 20:39:12.000000 ecg_quality-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 01:23:28.768785 ecg_quality-0.1.2/ecg_quality/
+-rw-rw-rw-   0        0        0    10091 2023-05-06 22:43:31.000000 ecg_quality-0.1.2/ecg_quality/ECGQualityChecker.py
+-rw-rw-rw-   0        0        0       41 2023-05-06 20:18:00.000000 ecg_quality-0.1.2/ecg_quality/__init__.py
+-rw-rw-rw-   0        0        0      807 2023-04-22 20:35:15.000000 ecg_quality-0.1.2/ecg_quality/model.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:23:28.817178 ecg_quality-0.1.2/ecg_quality/models/
+-rw-rw-rw-   0        0        0   128640 2023-04-29 16:55:23.000000 ecg_quality-0.1.2/ecg_quality/models/CNN2s.h5
+-rw-rw-rw-   0        0        0  7528704 2023-05-02 21:37:58.000000 ecg_quality-0.1.2/ecg_quality/models/CNN5s.h5
+-rw-rw-rw-   0        0        0  1224424 2023-04-29 16:55:22.000000 ecg_quality-0.1.2/ecg_quality/models/LSTM2s.h5
+-rw-rw-rw-   0        0        0   472672 2023-05-05 11:00:32.000000 ecg_quality-0.1.2/ecg_quality/models/OSCNN2s.h5
+-rw-rw-rw-   0        0        0        0 2023-05-07 00:50:50.000000 ecg_quality-0.1.2/ecg_quality/models/__init__.py
+-rw-rw-rw-   0        0        0     1024 2023-05-06 23:14:45.000000 ecg_quality-0.1.2/ecg_quality/tf_model.py
+-rw-rw-rw-   0        0        0     1107 2023-05-06 23:14:45.000000 ecg_quality-0.1.2/ecg_quality/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:23:28.797701 ecg_quality-0.1.2/ecg_quality.egg-info/
+-rw-rw-rw-   0        0        0      416 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-07 01:23:28.819211 ecg_quality-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-05-07 01:20:36.000000 ecg_quality-0.1.2/setup.py
```

### Comparing `ecg_quality-0.1.1/LICENSE` & `ecg_quality-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.1/setup.py` & `ecg_quality-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from distutils.core import setup
 import setuptools
 
 setuptools.setup(
   name = 'ecg_quality',
-  packages = setuptools.find_packages(where='ecg_quality'),
-  package_dir = {"": "ecg_quality"},
-  include_package_data=True,
-  version = '0.1.1',
+  packages = setuptools.find_packages(),
+  package_data={'ecg_quality': ['models/*.h5']},
+  version = '0.1.2',
   license='gpl-3.0',
   description = 'Library that classifies quality of ECG signal using deep learning methods',
   author = 'Jozef Koleda',
   author_email = 'koledjoz@cvut.cz',
   url = 'https://github.com/koledjoz/ecg_quality',
-  download_url = 'https://github.com/koledjoz/ecg_quality/releases/tag/v0.1.1',
+  download_url = 'https://github.com/koledjoz/ecg_quality/releases/tag/v0.1.2',
   keywords = ['ECG', 'quality', 'classification', 'deep learning'],
   install_requires=[
           'tensorflow',
           'numpy',
           'neurokit2',
       ]
 )
```

