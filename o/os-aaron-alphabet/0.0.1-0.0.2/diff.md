# Comparing `tmp/os-aaron-alphabet-0.0.1.tar.gz` & `tmp/os-aaron-alphabet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-aaron-alphabet-0.0.1.tar", last modified: Sun May  7 07:21:08 2023, max compression
+gzip compressed data, was "os-aaron-alphabet-0.0.2.tar", last modified: Sun May  7 07:29:52 2023, max compression
```

## Comparing `os-aaron-alphabet-0.0.1.tar` & `os-aaron-alphabet-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 07:21:08.986044 os-aaron-alphabet-0.0.1/
--rwxrwxrwx   0 lk        (1002) lk        (1002)     1066 2023-03-01 20:28:52.000000 os-aaron-alphabet-0.0.1/LICENSE
--rw-rw-r--   0 lk        (1002) lk        (1002)     1466 2023-05-07 07:21:08.986044 os-aaron-alphabet-0.0.1/PKG-INFO
--rwxrwxrwx   0 lk        (1002) lk        (1002)      495 2023-05-07 07:20:54.000000 os-aaron-alphabet-0.0.1/pyproject.toml
--rwxrwxrwx   0 lk        (1002) lk        (1002)       38 2023-05-07 07:21:08.986044 os-aaron-alphabet-0.0.1/setup.cfg
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 07:21:08.986044 os-aaron-alphabet-0.0.1/src/
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 07:21:08.986044 os-aaron-alphabet-0.0.1/src/os_aaron_alphabet.egg-info/
--rw-rw-r--   0 lk        (1002) lk        (1002)     1466 2023-05-07 07:21:08.000000 os-aaron-alphabet-0.0.1/src/os_aaron_alphabet.egg-info/PKG-INFO
--rw-rw-r--   0 lk        (1002) lk        (1002)      237 2023-05-07 07:21:08.000000 os-aaron-alphabet-0.0.1/src/os_aaron_alphabet.egg-info/SOURCES.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-05-07 07:21:08.000000 os-aaron-alphabet-0.0.1/src/os_aaron_alphabet.egg-info/dependency_links.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       18 2023-05-07 07:21:08.000000 os-aaron-alphabet-0.0.1/src/os_aaron_alphabet.egg-info/top_level.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)      450 2023-05-07 07:17:11.000000 os-aaron-alphabet-0.0.1/src/os_aaron_alphabet.py
+drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 07:29:52.796965 os-aaron-alphabet-0.0.2/
+-rwxrwxrwx   0 lk        (1002) lk        (1002)     1066 2023-03-01 20:28:52.000000 os-aaron-alphabet-0.0.2/LICENSE
+-rw-rw-r--   0 lk        (1002) lk        (1002)     1466 2023-05-07 07:29:52.796965 os-aaron-alphabet-0.0.2/PKG-INFO
+-rwxrwxrwx   0 lk        (1002) lk        (1002)      495 2023-05-07 07:29:42.000000 os-aaron-alphabet-0.0.2/pyproject.toml
+-rwxrwxrwx   0 lk        (1002) lk        (1002)       38 2023-05-07 07:29:52.796965 os-aaron-alphabet-0.0.2/setup.cfg
+drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 07:29:52.796965 os-aaron-alphabet-0.0.2/src/
+drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 07:29:52.796965 os-aaron-alphabet-0.0.2/src/os_aaron_alphabet.egg-info/
+-rw-rw-r--   0 lk        (1002) lk        (1002)     1466 2023-05-07 07:29:52.000000 os-aaron-alphabet-0.0.2/src/os_aaron_alphabet.egg-info/PKG-INFO
+-rw-rw-r--   0 lk        (1002) lk        (1002)      237 2023-05-07 07:29:52.000000 os-aaron-alphabet-0.0.2/src/os_aaron_alphabet.egg-info/SOURCES.txt
+-rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-05-07 07:29:52.000000 os-aaron-alphabet-0.0.2/src/os_aaron_alphabet.egg-info/dependency_links.txt
+-rw-rw-r--   0 lk        (1002) lk        (1002)       18 2023-05-07 07:29:52.000000 os-aaron-alphabet-0.0.2/src/os_aaron_alphabet.egg-info/top_level.txt
+-rw-rw-r--   0 lk        (1002) lk        (1002)      440 2023-05-07 07:26:14.000000 os-aaron-alphabet-0.0.2/src/os_aaron_alphabet.py
```

### Comparing `os-aaron-alphabet-0.0.1/LICENSE` & `os-aaron-alphabet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `os-aaron-alphabet-0.0.1/PKG-INFO` & `os-aaron-alphabet-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os-aaron-alphabet
-Version: 0.0.1
+Version: 0.0.2
 Summary: os-library-extension. 
 Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `os-aaron-alphabet-0.0.1/src/os_aaron_alphabet.egg-info/PKG-INFO` & `os-aaron-alphabet-0.0.2/src/os_aaron_alphabet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os-aaron-alphabet
-Version: 0.0.1
+Version: 0.0.2
 Summary: os-library-extension. 
 Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

