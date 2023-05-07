# Comparing `tmp/types-flake8-2020-1.7.0.2.tar.gz` & `tmp/types-flake8-2020-1.8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-2020-1.7.0.2.tar", last modified: Tue Feb 21 01:28:43 2023, max compression
+gzip compressed data, was "types-flake8-2020-1.8.0.0.tar", last modified: Sun May  7 09:13:48 2023, max compression
```

## Comparing `types-flake8-2020-1.7.0.2.tar` & `types-flake8-2020-1.8.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:43.662434 types-flake8-2020-1.7.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-02-21 01:28:43.662434 types-flake8-2020-1.7.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:43.662434 types-flake8-2020-1.7.0.2/flake8_2020-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/flake8_2020-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/flake8_2020-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:28:43.662434 types-flake8-2020-1.7.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:43.662434 types-flake8-2020-1.7.0.2/types_flake8_2020.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/types_flake8_2020.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/types_flake8_2020.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/types_flake8_2020.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 01:28:43.000000 types-flake8-2020-1.7.0.2/types_flake8_2020.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/flake8_2020-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/flake8_2020-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/flake8_2020-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-07 09:13:48.000000 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-07 09:13:48.000000 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:13:48.000000 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 09:13:48.000000 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/top_level.txt
```

### Comparing `types-flake8-2020-1.7.0.2/PKG-INFO` & `types-flake8-2020-1.8.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-2020
-Version: 1.7.0.2
+Version: 1.8.0.0
 Summary: Typing stubs for flake8-2020
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-2020.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-2020`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-2020. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `38a11b2f06f455bad02ea91a76cb40cf521105d9`.
```

### Comparing `types-flake8-2020-1.7.0.2/flake8_2020-stubs/__init__.pyi` & `types-flake8-2020-1.8.0.0/flake8_2020-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-2020-1.7.0.2/setup.py` & `types-flake8-2020-1.8.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-2020`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-2020. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `38a11b2f06f455bad02ea91a76cb40cf521105d9`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.7.0.2",
+      version="1.8.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-2020.md",
```

### Comparing `types-flake8-2020-1.7.0.2/types_flake8_2020.egg-info/PKG-INFO` & `types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-2020
-Version: 1.7.0.2
+Version: 1.8.0.0
 Summary: Typing stubs for flake8-2020
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-2020.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-2020`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-2020. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `38a11b2f06f455bad02ea91a76cb40cf521105d9`.
```

