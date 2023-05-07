# Comparing `tmp/arabic2latin-1.1.1.tar.gz` & `tmp/arabic2latin-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabic2latin-1.1.1.tar", last modified: Tue Apr 25 07:22:14 2023, max compression
+gzip compressed data, was "arabic2latin-1.1.2.tar", last modified: Sun May  7 20:25:09 2023, max compression
```

## Comparing `arabic2latin-1.1.1.tar` & `arabic2latin-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 07:22:14.038426 arabic2latin-1.1.1/
--rw-rw-rw-   0        0        0     1083 2023-04-12 10:51:38.000000 arabic2latin-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3221 2023-04-25 07:22:14.037498 arabic2latin-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-04-10 20:55:54.000000 arabic2latin-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 07:22:14.015653 arabic2latin-1.1.1/arabic2latin/
--rw-rw-rw-   0        0        0       55 2023-04-10 05:39:27.000000 arabic2latin-1.1.1/arabic2latin/__init__.py
--rw-rw-rw-   0        0        0     3719 2023-04-22 16:01:53.000000 arabic2latin-1.1.1/arabic2latin/arabic2latin.py
--rw-rw-rw-   0        0        0       23 2023-04-22 16:01:53.000000 arabic2latin-1.1.1/arabic2latin/version.py
-drwxrwxrwx   0        0        0        0 2023-04-25 07:22:14.035170 arabic2latin-1.1.1/arabic2latin.egg-info/
--rw-rw-rw-   0        0        0     3221 2023-04-25 07:22:13.000000 arabic2latin-1.1.1/arabic2latin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-25 07:22:13.000000 arabic2latin-1.1.1/arabic2latin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 07:22:13.000000 arabic2latin-1.1.1/arabic2latin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 07:22:13.000000 arabic2latin-1.1.1/arabic2latin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      781 2023-04-25 07:20:51.000000 arabic2latin-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 07:22:14.038426 arabic2latin-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-04-12 10:59:40.000000 arabic2latin-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:25:09.930472 arabic2latin-1.1.2/
+-rw-rw-rw-   0        0        0     1083 2023-04-12 10:51:38.000000 arabic2latin-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3219 2023-05-07 20:25:09.930472 arabic2latin-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1203 2023-05-07 20:22:58.000000 arabic2latin-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 20:25:09.905074 arabic2latin-1.1.2/arabic2latin/
+-rw-rw-rw-   0        0        0       55 2023-04-10 05:39:27.000000 arabic2latin-1.1.2/arabic2latin/__init__.py
+-rw-rw-rw-   0        0        0     3758 2023-05-07 20:20:43.000000 arabic2latin-1.1.2/arabic2latin/arabic2latin.py
+-rw-rw-rw-   0        0        0       23 2023-05-07 20:20:43.000000 arabic2latin-1.1.2/arabic2latin/version.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:25:09.930472 arabic2latin-1.1.2/arabic2latin.egg-info/
+-rw-rw-rw-   0        0        0     3219 2023-05-07 20:25:09.000000 arabic2latin-1.1.2/arabic2latin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-07 20:25:09.000000 arabic2latin-1.1.2/arabic2latin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 20:25:09.000000 arabic2latin-1.1.2/arabic2latin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 20:25:09.000000 arabic2latin-1.1.2/arabic2latin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      781 2023-05-07 20:20:43.000000 arabic2latin-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 20:25:09.930472 arabic2latin-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      563 2023-04-12 10:59:40.000000 arabic2latin-1.1.2/setup.py
```

### Comparing `arabic2latin-1.1.1/LICENSE` & `arabic2latin-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arabic2latin-1.1.1/PKG-INFO` & `arabic2latin-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabic2latin
-Version: 1.1.1
+Version: 1.1.2
 Summary: Convert Arabic characters to their Latin (English) homophones.
 Author: rexa222
 Author-email: rexa222@outlook.com
 License: MIT License
         
         Copyright (c) 2023 rexa222
         
@@ -42,22 +42,21 @@
 # arabic2latin
 
 Convert Arabic characters to their Latin (English) homophone.
 
 
 ## Installation
 
-Install from source:
-
+Install from PyPI:
 ```bash
-pip install git+https://github.com/rexa222/arabic2latin
+pip install arabic2latin
 ```
-Alternatively, install from PyPI:
+Alternatively, install from source:
 ```bash
-pip install arabic2latin
+pip install git+https://github.com/rexa222/arabic2latin
 ```
 ## Usage/Examples
 
 ```python
 from arabic2latin import arabic_to_latin
 
 arabic_text = "السَّلَامُ عَلَيْكَ"
```

### Comparing `arabic2latin-1.1.1/README.md` & `arabic2latin-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 # arabic2latin
 
 Convert Arabic characters to their Latin (English) homophone.
 
 
 ## Installation
 
-Install from source:
-
+Install from PyPI:
 ```bash
-pip install git+https://github.com/rexa222/arabic2latin
+pip install arabic2latin
 ```
-Alternatively, install from PyPI:
+Alternatively, install from source:
 ```bash
-pip install arabic2latin
+pip install git+https://github.com/rexa222/arabic2latin
 ```
 ## Usage/Examples
 
 ```python
 from arabic2latin import arabic_to_latin
 
 arabic_text = "السَّلَامُ عَلَيْكَ"
```

### Comparing `arabic2latin-1.1.1/arabic2latin/arabic2latin.py` & `arabic2latin-1.1.2/arabic2latin/arabic2latin.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,22 +41,22 @@
                 else:
                     result += MAPPING[char]
 
             elif char in "ىيی" and (c != n-1 and text[c+1] in MAPPING):
                 result += "i"
 
             elif char == "و":
-                if text[c+1] in "اىيی" and (c == n-2 or "وا " in text[c:]):
+                if (c != n-1 and text[c+1] in "اىيی") and (c == n-2 or text[c:].startswith("وا ")):
                     if result[-1] == "o":
                         result += "o"
                     else:
                         result += "oo"
                     special_case = True
 
-                elif text[c-1] in "اىيی" or text[c+1] in "اىيی":
+                elif text[c-1] in "اىيی" or (c != n-1 and text[c+1] in "اىيی"):
                     if result[-1] not in VOWELS and result[-3:] not in " al" and MAPPING[char] != "y":
                         if not no_vowel:
                             result += "a"
                         else:
                             no_vowel = False
 
                     result += "v"
```

### Comparing `arabic2latin-1.1.1/arabic2latin.egg-info/PKG-INFO` & `arabic2latin-1.1.2/arabic2latin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabic2latin
-Version: 1.1.1
+Version: 1.1.2
 Summary: Convert Arabic characters to their Latin (English) homophones.
 Author: rexa222
 Author-email: rexa222@outlook.com
 License: MIT License
         
         Copyright (c) 2023 rexa222
         
@@ -42,22 +42,21 @@
 # arabic2latin
 
 Convert Arabic characters to their Latin (English) homophone.
 
 
 ## Installation
 
-Install from source:
-
+Install from PyPI:
 ```bash
-pip install git+https://github.com/rexa222/arabic2latin
+pip install arabic2latin
 ```
-Alternatively, install from PyPI:
+Alternatively, install from source:
 ```bash
-pip install arabic2latin
+pip install git+https://github.com/rexa222/arabic2latin
 ```
 ## Usage/Examples
 
 ```python
 from arabic2latin import arabic_to_latin
 
 arabic_text = "السَّلَامُ عَلَيْكَ"
```

### Comparing `arabic2latin-1.1.1/pyproject.toml` & `arabic2latin-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arabic2latin"
-version = "1.1.1"
+version = "1.1.2"
 description = "Convert Arabic characters to their Latin (English) homophones."
 readme = "README.md"
 requires-python = ">=3.6"
 license= {file = "LICENSE"}
 keywords=["arabic", "homophone", "arabic to english", "arabic to latin"]
 authors = [
   {email = "rexa222@outlook.com"},
```

### Comparing `arabic2latin-1.1.1/setup.py` & `arabic2latin-1.1.2/setup.py`

 * *Files identical despite different names*

