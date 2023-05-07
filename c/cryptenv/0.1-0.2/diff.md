# Comparing `tmp/cryptenv-0.1.tar.gz` & `tmp/cryptenv-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptenv-0.1.tar", last modified: Sun May  7 14:57:42 2023, max compression
+gzip compressed data, was "cryptenv-0.2.tar", last modified: Sun May  7 15:33:40 2023, max compression
```

## Comparing `cryptenv-0.1.tar` & `cryptenv-0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:57:42.760244 cryptenv-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-07 14:57:25.000000 cryptenv-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 14:57:42.760244 cryptenv-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-07 14:57:25.000000 cryptenv-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:57:42.756244 cryptenv-0.1/cryptenv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:57:42.756244 cryptenv-0.1/cryptenv/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:57:25.000000 cryptenv-0.1/cryptenv/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-07 14:57:25.000000 cryptenv-0.1/cryptenv/actions/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:57:42.756244 cryptenv-0.1/cryptenv/cryptenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 14:57:42.000000 cryptenv-0.1/cryptenv/cryptenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-07 14:57:42.000000 cryptenv-0.1/cryptenv/cryptenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:57:42.000000 cryptenv-0.1/cryptenv/cryptenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 14:57:42.000000 cryptenv-0.1/cryptenv/cryptenv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 14:57:42.000000 cryptenv-0.1/cryptenv/cryptenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 14:57:42.000000 cryptenv-0.1/cryptenv/cryptenv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:57:42.756244 cryptenv-0.1/cryptenv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:57:25.000000 cryptenv-0.1/cryptenv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-07 14:57:25.000000 cryptenv-0.1/cryptenv/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-07 14:57:25.000000 cryptenv-0.1/cryptenv/utils/exit_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-07 14:57:25.000000 cryptenv-0.1/cryptenv/utils/password.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-07 14:57:25.000000 cryptenv-0.1/cryptenv/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-07 14:57:25.000000 cryptenv-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 14:57:42.760244 cryptenv-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:57:42.760244 cryptenv-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-07 14:57:25.000000 cryptenv-0.1/tests/test_env_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:33:40.996651 cryptenv-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-07 15:33:25.000000 cryptenv-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 15:33:40.996651 cryptenv-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-07 15:33:25.000000 cryptenv-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:33:40.992651 cryptenv-0.2/cryptenv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:33:40.992651 cryptenv-0.2/cryptenv/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:33:25.000000 cryptenv-0.2/cryptenv/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-07 15:33:25.000000 cryptenv-0.2/cryptenv/actions/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:33:40.996651 cryptenv-0.2/cryptenv/cryptenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 15:33:40.000000 cryptenv-0.2/cryptenv/cryptenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-07 15:33:40.000000 cryptenv-0.2/cryptenv/cryptenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:33:40.000000 cryptenv-0.2/cryptenv/cryptenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 15:33:40.000000 cryptenv-0.2/cryptenv/cryptenv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 15:33:40.000000 cryptenv-0.2/cryptenv/cryptenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 15:33:40.000000 cryptenv-0.2/cryptenv/cryptenv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:33:40.996651 cryptenv-0.2/cryptenv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:33:25.000000 cryptenv-0.2/cryptenv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-07 15:33:25.000000 cryptenv-0.2/cryptenv/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-07 15:33:25.000000 cryptenv-0.2/cryptenv/utils/exit_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-07 15:33:25.000000 cryptenv-0.2/cryptenv/utils/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-07 15:33:25.000000 cryptenv-0.2/cryptenv/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-07 15:33:25.000000 cryptenv-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 15:33:40.996651 cryptenv-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:33:40.996651 cryptenv-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-07 15:33:25.000000 cryptenv-0.2/tests/test_env_file.py
```

### Comparing `cryptenv-0.1/LICENSE` & `cryptenv-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptenv-0.1/PKG-INFO` & `cryptenv-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptenv
-Version: 0.1
+Version: 0.2
 Summary: A CLI tool to encrypt and decrypt variables in .env files.
 Author-email: Vasilis Papadopoulos <vpapadopoulos155@gmail.com>
 License: MIT
 Project-URL: GitHub, https://github.com/vaspapadopoulos/cryptenv
 Keywords: env,encrypt,decrypt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `cryptenv-0.1/README.md` & `cryptenv-0.2/README.md`

 * *Files identical despite different names*

### Comparing `cryptenv-0.1/cryptenv/actions/file.py` & `cryptenv-0.2/cryptenv/actions/file.py`

 * *Files identical despite different names*

### Comparing `cryptenv-0.1/cryptenv/cryptenv.egg-info/PKG-INFO` & `cryptenv-0.2/cryptenv/cryptenv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptenv
-Version: 0.1
+Version: 0.2
 Summary: A CLI tool to encrypt and decrypt variables in .env files.
 Author-email: Vasilis Papadopoulos <vpapadopoulos155@gmail.com>
 License: MIT
 Project-URL: GitHub, https://github.com/vaspapadopoulos/cryptenv
 Keywords: env,encrypt,decrypt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `cryptenv-0.1/cryptenv/utils/env_file.py` & `cryptenv-0.2/cryptenv/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `cryptenv-0.1/cryptenv/utils/exit_codes.py` & `cryptenv-0.2/cryptenv/utils/exit_codes.py`

 * *Files identical despite different names*

### Comparing `cryptenv-0.1/cryptenv/utils/password.py` & `cryptenv-0.2/cryptenv/utils/password.py`

 * *Files identical despite different names*

### Comparing `cryptenv-0.1/cryptenv/utils/version.py` & `cryptenv-0.2/cryptenv/utils/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from packaging import version
 from typing import Final
 
 from cryptenv.utils.exit_codes import UNSUPPORTED_PYTHON_VERSION
 
 PYTHON_MIN_VERSION: Final[str] = "3.9"
-CRYPTENV_VERSION: Final[str] = "0.1"
+CRYPTENV_VERSION: Final[str] = "0.2"
 
 
 def print_version(raw: bool) -> None:
     if (raw):
         print(CRYPTENV_VERSION)
     else:
         print(CRYPTENV_VERSION + " blah")
```

### Comparing `cryptenv-0.1/pyproject.toml` & `cryptenv-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools==67.7.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cryptenv"
-version = "0.1"
+version = "0.2"
 authors = [
     {name = "Vasilis Papadopoulos", email = "vpapadopoulos155@gmail.com"},
 ]
 description = "A CLI tool to encrypt and decrypt variables in .env files."
 requires-python = ">=3.9"
 keywords = ["env", "encrypt", "decrypt"]
 license = {text = "MIT"}
```

