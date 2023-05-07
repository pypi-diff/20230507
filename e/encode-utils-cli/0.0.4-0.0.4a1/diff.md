# Comparing `tmp/encode_utils_cli-0.0.4.tar.gz` & `tmp/encode_utils_cli-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encode_utils_cli-0.0.4.tar", max compression
+gzip compressed data, was "encode_utils_cli-0.0.4a1.tar", max compression
```

## Comparing `encode_utils_cli-0.0.4.tar` & `encode_utils_cli-0.0.4a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/LICENSE
--rw-r--r--   0        0        0      828 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/README.md
--rw-r--r--   0        0        0     2591 2023-05-07 14:48:23.982615 encode_utils_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       70 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/__init__.py
--rw-r--r--   0        0        0      177 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/__main__.py
--rw-r--r--   0        0        0      970 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/_cli.py
--rw-r--r--   0        0        0     2087 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/chapt2bmqpyml.py
--rw-r--r--   0        0        0      666 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/frames_denum.py
--rwxr-xr-x   0        0        0     1209 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/mpls2chap.py
--rw-r--r--   0        0        0      427 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/num_frames.py
--rw-r--r--   0        0        0     1163 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/re_chapters.py
--rwxr-xr-x   0        0        0     1042 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/re_titles.py
--rwxr-xr-x   0        0        0      966 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/screens2bm.py
--rw-r--r--   0        0        0       35 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/util/__init__.py
--rw-r--r--   0        0        0     2012 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/util/load_mpls.py
--rw-r--r--   0        0        0      312 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/util/source.py
--rw-r--r--   0        0        0      672 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/util/timeconv.py
--rw-r--r--   0        0        0     2203 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/vs_screens.py
--rwxr-xr-x   0        0        0      758 2023-05-07 14:48:07.850459 encode_utils_cli-0.0.4/src/encode_utils_cli/zones_validator.py
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 encode_utils_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/LICENSE
+-rw-r--r--   0        0        0      828 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/README.md
+-rw-r--r--   0        0        0     2599 2023-05-05 09:18:11.132545 encode_utils_cli-0.0.4a1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/__init__.py
+-rw-r--r--   0        0        0      177 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/__main__.py
+-rw-r--r--   0        0        0      970 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/_cli.py
+-rw-r--r--   0        0        0     2087 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/chapt2bmqpyml.py
+-rw-r--r--   0        0        0      666 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/frames_denum.py
+-rwxr-xr-x   0        0        0     1209 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/mpls2chap.py
+-rw-r--r--   0        0        0      427 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/num_frames.py
+-rw-r--r--   0        0        0     1163 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_chapters.py
+-rwxr-xr-x   0        0        0     1042 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_titles.py
+-rwxr-xr-x   0        0        0      966 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/screens2bm.py
+-rw-r--r--   0        0        0       35 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/__init__.py
+-rw-r--r--   0        0        0     2012 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/load_mpls.py
+-rw-r--r--   0        0        0      312 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/source.py
+-rw-r--r--   0        0        0      672 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/timeconv.py
+-rw-r--r--   0        0        0     2203 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/vs_screens.py
+-rwxr-xr-x   0        0        0      758 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/zones_validator.py
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 encode_utils_cli-0.0.4a1/PKG-INFO
```

### Comparing `encode_utils_cli-0.0.4/LICENSE` & `encode_utils_cli-0.0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/README.md` & `encode_utils_cli-0.0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/pyproject.toml` & `encode_utils_cli-0.0.4a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "encode-utils-cli"
-version = "0.0.4"
+version = "0.0.4-alpha.1"
 description = "Encode utils collection"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/encode-utils-cli"
 repository = "https://github.com/DeadNews/encode-utils-cli"
 keywords = ["cli", "encode", "vapoursynth", "mpls"]
@@ -30,15 +30,15 @@
 schema = "^0.7.5"
 tomli = "^2.0.1"
 
 [tool.poetry.group.ci.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 poethepoet = "^0.20.0"
-ruff = "^0.0.265"
+ruff = "^0.0.264"
 types-pyyaml = "^6.0.12.9"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/_cli.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/chapt2bmqpyml.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/chapt2bmqpyml.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/frames_denum.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/frames_denum.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/mpls2chap.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/mpls2chap.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/re_chapters.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_chapters.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/re_titles.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_titles.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/screens2bm.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/screens2bm.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/util/load_mpls.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/load_mpls.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/util/timeconv.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/timeconv.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/vs_screens.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/vs_screens.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/src/encode_utils_cli/zones_validator.py` & `encode_utils_cli-0.0.4a1/src/encode_utils_cli/zones_validator.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4/PKG-INFO` & `encode_utils_cli-0.0.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encode-utils-cli
-Version: 0.0.4
+Version: 0.0.4a1
 Summary: Encode utils collection
 Home-page: https://github.com/DeadNews/encode-utils-cli
 License: MIT
 Keywords: cli,encode,vapoursynth,mpls
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
```

