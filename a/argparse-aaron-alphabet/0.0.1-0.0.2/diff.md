# Comparing `tmp/argparse-aaron-alphabet-0.0.1.tar.gz` & `tmp/argparse-aaron-alphabet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse-aaron-alphabet-0.0.1.tar", last modified: Sun May  7 09:36:42 2023, max compression
+gzip compressed data, was "argparse-aaron-alphabet-0.0.2.tar", last modified: Sun May  7 09:37:40 2023, max compression
```

## Comparing `argparse-aaron-alphabet-0.0.1.tar` & `argparse-aaron-alphabet-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:36:42.516277 argparse-aaron-alphabet-0.0.1/
--rwxrwxrwx   0 lk        (1002) lk        (1002)     1066 2023-03-01 20:28:52.000000 argparse-aaron-alphabet-0.0.1/LICENSE
--rw-rw-r--   0 lk        (1002) lk        (1002)     1472 2023-05-07 09:36:42.516277 argparse-aaron-alphabet-0.0.1/PKG-INFO
--rwxrwxrwx   0 lk        (1002) lk        (1002)      501 2023-05-07 09:34:28.000000 argparse-aaron-alphabet-0.0.1/pyproject.toml
--rwxrwxrwx   0 lk        (1002) lk        (1002)       38 2023-05-07 09:36:42.516277 argparse-aaron-alphabet-0.0.1/setup.cfg
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:36:42.516277 argparse-aaron-alphabet-0.0.1/src/
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:36:42.516277 argparse-aaron-alphabet-0.0.1/src/argparse_aaron_alphabet.egg-info/
--rw-rw-r--   0 lk        (1002) lk        (1002)     1472 2023-05-07 09:36:42.000000 argparse-aaron-alphabet-0.0.1/src/argparse_aaron_alphabet.egg-info/PKG-INFO
--rw-rw-r--   0 lk        (1002) lk        (1002)      267 2023-05-07 09:36:42.000000 argparse-aaron-alphabet-0.0.1/src/argparse_aaron_alphabet.egg-info/SOURCES.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-05-07 09:36:42.000000 argparse-aaron-alphabet-0.0.1/src/argparse_aaron_alphabet.egg-info/dependency_links.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       24 2023-05-07 09:36:42.000000 argparse-aaron-alphabet-0.0.1/src/argparse_aaron_alphabet.egg-info/top_level.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)      175 2023-05-07 09:36:06.000000 argparse-aaron-alphabet-0.0.1/src/argparse_aaron_alphabet.py
+drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/
+-rwxrwxrwx   0 lk        (1002) lk        (1002)     1066 2023-03-01 20:28:52.000000 argparse-aaron-alphabet-0.0.2/LICENSE
+-rw-rw-r--   0 lk        (1002) lk        (1002)     1472 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/PKG-INFO
+-rwxrwxrwx   0 lk        (1002) lk        (1002)      501 2023-05-07 09:37:29.000000 argparse-aaron-alphabet-0.0.2/pyproject.toml
+-rwxrwxrwx   0 lk        (1002) lk        (1002)       38 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/setup.cfg
+drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/src/
+drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/
+-rw-rw-r--   0 lk        (1002) lk        (1002)     1472 2023-05-07 09:37:40.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/PKG-INFO
+-rw-rw-r--   0 lk        (1002) lk        (1002)      267 2023-05-07 09:37:40.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/SOURCES.txt
+-rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-05-07 09:37:40.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/dependency_links.txt
+-rw-rw-r--   0 lk        (1002) lk        (1002)       24 2023-05-07 09:37:40.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/top_level.txt
+-rw-rw-r--   0 lk        (1002) lk        (1002)      184 2023-05-07 09:37:18.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.py
```

### Comparing `argparse-aaron-alphabet-0.0.1/LICENSE` & `argparse-aaron-alphabet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse-aaron-alphabet-0.0.1/PKG-INFO` & `argparse-aaron-alphabet-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-aaron-alphabet
-Version: 0.0.1
+Version: 0.0.2
 Summary: os-library-extension. 
 Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `argparse-aaron-alphabet-0.0.1/src/argparse_aaron_alphabet.egg-info/PKG-INFO` & `argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-aaron-alphabet
-Version: 0.0.1
+Version: 0.0.2
 Summary: os-library-extension. 
 Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

