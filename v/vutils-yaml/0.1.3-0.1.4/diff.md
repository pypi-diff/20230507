# Comparing `tmp/vutils-yaml-0.1.3.tar.gz` & `tmp/vutils-yaml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-yaml-0.1.3.tar", last modified: Thu Apr 20 22:25:30 2023, max compression
+gzip compressed data, was "vutils-yaml-0.1.4.tar", last modified: Sun May  7 20:15:47 2023, max compression
```

## Comparing `vutils-yaml-0.1.3.tar` & `vutils-yaml-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.482668 vutils-yaml-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.482668 vutils-yaml-0.1.3/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.482668 vutils-yaml-0.1.3/src/vutils/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/load.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.482668 vutils-yaml-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:15:47.360629 vutils-yaml-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-07 20:15:47.360629 vutils-yaml-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-07 20:15:47.364629 vutils-yaml-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:15:47.356629 vutils-yaml-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:15:47.356629 vutils-yaml-0.1.4/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:15:47.360629 vutils-yaml-0.1.4/src/vutils/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/src/vutils/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/src/vutils/yaml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/src/vutils/yaml/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/src/vutils/yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/src/vutils/yaml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/src/vutils/yaml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:15:47.360629 vutils-yaml-0.1.4/src/vutils_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-07 20:15:47.000000 vutils-yaml-0.1.4/src/vutils_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-07 20:15:47.000000 vutils-yaml-0.1.4/src/vutils_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:15:47.000000 vutils-yaml-0.1.4/src/vutils_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:15:47.000000 vutils-yaml-0.1.4/src/vutils_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 20:15:47.000000 vutils-yaml-0.1.4/src/vutils_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 20:15:47.000000 vutils-yaml-0.1.4/src/vutils_yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:15:47.360629 vutils-yaml-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:15:47.360629 vutils-yaml-0.1.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/tests/unit/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/tests/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-07 20:15:21.000000 vutils-yaml-0.1.4/tox.ini
```

### Comparing `vutils-yaml-0.1.3/LICENSE` & `vutils-yaml-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/PKG-INFO` & `vutils-yaml-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-yaml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Working with YAML format
 Home-page: https://github.com/i386x/vutils-yaml
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-yaml/issues
 Project-URL: Source, https://github.com/i386x/vutils-yaml
```

### Comparing `vutils-yaml-0.1.3/README.md` & `vutils-yaml-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/pyproject.toml` & `vutils-yaml-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/setup.cfg` & `vutils-yaml-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/src/vutils/yaml/__init__.pyi` & `vutils-yaml-0.1.4/src/vutils/yaml/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/src/vutils/yaml/load.py` & `vutils-yaml-0.1.4/src/vutils/yaml/load.py`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/src/vutils/yaml/utils.py` & `vutils-yaml-0.1.4/src/vutils/yaml/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     """
     Holds YAML values annotation.
 
     :ivar location: The value's location
     """
 
     location: Location
+
     __slots__ = ("location",)
 
     def __init__(self, location: "Location | None" = None) -> None:
         """
         Initialize annotation object.
 
         :param location: The YAML value's location
@@ -112,14 +113,16 @@
         return hash(None)
 
 
 class BoolType(YamlDataType):
     """
     Represent a Boolean type.
 
+    :ivar __value: The truth value
+
     Since :class:`bool` is not an acceptable base class this workaround is used
     to store annotation alongside with Boolean values.
     """
 
     __value: bool
 
     def __init__(self, value: bool) -> None:
```

### Comparing `vutils-yaml-0.1.3/src/vutils_yaml.egg-info/PKG-INFO` & `vutils-yaml-0.1.4/src/vutils_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-yaml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Working with YAML format
 Home-page: https://github.com/i386x/vutils-yaml
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-yaml/issues
 Project-URL: Source, https://github.com/i386x/vutils-yaml
```

### Comparing `vutils-yaml-0.1.3/src/vutils_yaml.egg-info/SOURCES.txt` & `vutils-yaml-0.1.4/src/vutils_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/tests/unit/test_load.py` & `vutils-yaml-0.1.4/tests/unit/test_load.py`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/tests/unit/test_utils.py` & `vutils-yaml-0.1.4/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/tests/unit/test_version.py` & `vutils-yaml-0.1.4/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.3/tox.ini` & `vutils-yaml-0.1.4/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 passenv = *
 description =
     {envname}: Run unit tests for {envname}
 deps =
     safety
     pytest
     pytest-cov
+    PyYAML
     vutils-python
     vutils-validator
     vutils-testing
     coveralls
 commands =
     safety check --full-report
     pytest -v --cov=vutils.yaml --cov-report=term-missing tests
```

