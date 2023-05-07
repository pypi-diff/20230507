# Comparing `tmp/mc-pdf2txt-0.2.0.tar.gz` & `tmp/mc-pdf2txt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc-pdf2txt-0.2.0.tar", last modified: Sat Jul 30 19:05:12 2022, max compression
+gzip compressed data, was "mc-pdf2txt-0.3.0.tar", last modified: Sun May  7 09:06:38 2023, max compression
```

## Comparing `mc-pdf2txt-0.2.0.tar` & `mc-pdf2txt-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2022-07-30 19:05:12.679134 mc-pdf2txt-0.2.0/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1211 2021-03-21 01:39:03.000000 mc-pdf2txt-0.2.0/LICENSE
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1931 2022-07-30 19:05:12.679134 mc-pdf2txt-0.2.0/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1317 2022-07-30 19:01:31.000000 mc-pdf2txt-0.2.0/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2022-07-30 19:05:12.679134 mc-pdf2txt-0.2.0/mc_pdf2txt/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      106 2022-03-24 17:59:08.000000 mc-pdf2txt-0.2.0/mc_pdf2txt/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4661 2022-03-24 18:03:19.000000 mc-pdf2txt-0.2.0/mc_pdf2txt/main.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2022-07-30 19:05:12.679134 mc-pdf2txt-0.2.0/mc_pdf2txt.egg-info/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1931 2022-07-30 19:05:12.000000 mc-pdf2txt-0.2.0/mc_pdf2txt.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      284 2022-07-30 19:05:12.000000 mc-pdf2txt-0.2.0/mc_pdf2txt.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2022-07-30 19:05:12.000000 mc-pdf2txt-0.2.0/mc_pdf2txt.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       47 2022-07-30 19:05:12.000000 mc-pdf2txt-0.2.0/mc_pdf2txt.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       63 2022-07-30 19:05:12.000000 mc-pdf2txt-0.2.0/mc_pdf2txt.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       11 2022-07-30 19:05:12.000000 mc-pdf2txt-0.2.0/mc_pdf2txt.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      787 2022-07-30 19:05:12.679134 mc-pdf2txt-0.2.0/setup.cfg
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2022-03-24 17:31:19.000000 mc-pdf2txt-0.2.0/setup.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-05-07 09:06:38.155404 mc-pdf2txt-0.3.0/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1211 2021-03-21 01:39:03.000000 mc-pdf2txt-0.3.0/LICENSE
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1619 2023-05-07 09:06:38.155404 mc-pdf2txt-0.3.0/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      946 2023-05-07 08:41:39.000000 mc-pdf2txt-0.3.0/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-05-07 09:06:38.155404 mc-pdf2txt-0.3.0/mc_pdf2txt/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-05-07 08:48:19.000000 mc-pdf2txt-0.3.0/mc_pdf2txt/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-05-07 08:47:59.000000 mc-pdf2txt-0.3.0/mc_pdf2txt/_version.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4645 2023-05-07 09:03:24.000000 mc-pdf2txt-0.3.0/mc_pdf2txt/main.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-05-07 09:06:38.155404 mc-pdf2txt-0.3.0/mc_pdf2txt.egg-info/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1619 2023-05-07 09:06:38.000000 mc-pdf2txt-0.3.0/mc_pdf2txt.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      270 2023-05-07 09:06:38.000000 mc-pdf2txt-0.3.0/mc_pdf2txt.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-05-07 09:06:38.000000 mc-pdf2txt-0.3.0/mc_pdf2txt.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       47 2023-05-07 09:06:38.000000 mc-pdf2txt-0.3.0/mc_pdf2txt.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       11 2023-05-07 09:06:38.000000 mc-pdf2txt-0.3.0/mc_pdf2txt.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1020 2023-05-07 08:51:42.000000 mc-pdf2txt-0.3.0/pyproject.toml
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-05-07 09:06:38.155404 mc-pdf2txt-0.3.0/setup.cfg
```

### Comparing `mc-pdf2txt-0.2.0/LICENSE` & `mc-pdf2txt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mc-pdf2txt-0.2.0/PKG-INFO` & `mc-pdf2txt-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: mc-pdf2txt
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multi-column PDF to Text
-Home-page: https://github.com/tos-kamiya/mc-pdf2txt
-Author: Toshihiro kamiya
-Author-email: kamiya@mbj.nifty.com
+Author-email: Toshihiro Kamiya <kamiya@mbj.nifty.com>
 License: BSD 2-Clause License
+Project-URL: Homepage, https://github.com/tos-kamiya/mc-pdf2txt
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: docopt-ng
-Provides-Extra: docopt
 License-File: LICENSE
 
 mc-pdf2txt
 ==========
 
 Convert multi-column pdf to text with `poppler` and `tesseract`.
 
@@ -42,28 +41,18 @@
 
 ```sh
 sudo apt install tesseract-ocr-jpn
 ```
 
 (2) Install mc-pdf2txt
 
-To make `mc-pdf2txt` compatible with both `docopt` and `docopt-ng`, dependencies on them are now explicitly extra dependencies.
-
-If you know either `docopt` or `docopt-ng` is already installed on your system, just try the following:
-
 ```sh
 pip3 install mc-pdf2txt
 ```
 
-If you are unsure `docopt` or `docopt-ng` is installed on your system, try the following:
-
-```sh
-pip3 install mc-pdf2txt[docopt-ng]
-```
-
 ## Usage
 
 ```
 Usage:
   mc-pdf2txt [options] <input>...
 
 Options:
```

### Comparing `mc-pdf2txt-0.2.0/README.md` & `mc-pdf2txt-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -23,28 +23,18 @@
 
 ```sh
 sudo apt install tesseract-ocr-jpn
 ```
 
 (2) Install mc-pdf2txt
 
-To make `mc-pdf2txt` compatible with both `docopt` and `docopt-ng`, dependencies on them are now explicitly extra dependencies.
-
-If you know either `docopt` or `docopt-ng` is already installed on your system, just try the following:
-
 ```sh
 pip3 install mc-pdf2txt
 ```
 
-If you are unsure `docopt` or `docopt-ng` is installed on your system, try the following:
-
-```sh
-pip3 install mc-pdf2txt[docopt-ng]
-```
-
 ## Usage
 
 ```
 Usage:
   mc-pdf2txt [options] <input>...
 
 Options:
```

### Comparing `mc-pdf2txt-0.2.0/mc_pdf2txt.egg-info/PKG-INFO` & `mc-pdf2txt-0.3.0/mc_pdf2txt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: mc-pdf2txt
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multi-column PDF to Text
-Home-page: https://github.com/tos-kamiya/mc-pdf2txt
-Author: Toshihiro kamiya
-Author-email: kamiya@mbj.nifty.com
+Author-email: Toshihiro Kamiya <kamiya@mbj.nifty.com>
 License: BSD 2-Clause License
+Project-URL: Homepage, https://github.com/tos-kamiya/mc-pdf2txt
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: docopt-ng
-Provides-Extra: docopt
 License-File: LICENSE
 
 mc-pdf2txt
 ==========
 
 Convert multi-column pdf to text with `poppler` and `tesseract`.
 
@@ -42,28 +41,18 @@
 
 ```sh
 sudo apt install tesseract-ocr-jpn
 ```
 
 (2) Install mc-pdf2txt
 
-To make `mc-pdf2txt` compatible with both `docopt` and `docopt-ng`, dependencies on them are now explicitly extra dependencies.
-
-If you know either `docopt` or `docopt-ng` is already installed on your system, just try the following:
-
 ```sh
 pip3 install mc-pdf2txt
 ```
 
-If you are unsure `docopt` or `docopt-ng` is installed on your system, try the following:
-
-```sh
-pip3 install mc-pdf2txt[docopt-ng]
-```
-
 ## Usage
 
 ```
 Usage:
   mc-pdf2txt [options] <input>...
 
 Options:
```

