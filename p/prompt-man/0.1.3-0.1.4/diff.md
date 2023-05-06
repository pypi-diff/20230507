# Comparing `tmp/prompt_man-0.1.3.tar.gz` & `tmp/prompt_man-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_man-0.1.3.tar", max compression
+gzip compressed data, was "prompt_man-0.1.4.tar", max compression
```

## Comparing `prompt_man-0.1.3.tar` & `prompt_man-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0      968 2023-05-06 20:51:52.049872 prompt_man-0.1.3/README.md
--rwxr-xr-x   0        0        0      146 2023-05-06 21:24:20.074180 prompt_man-0.1.3/prompt_man/__init__.py
--rwxr-xr-x   0        0        0       81 2023-05-05 22:42:28.854955 prompt_man-0.1.3/prompt_man/hello.py
--rwxr-xr-x   0        0        0      460 2023-05-06 15:50:38.465651 prompt_man-0.1.3/prompt_man/stablediffusion.py
--rwxr-xr-x   0        0        0      559 2023-05-06 21:25:06.125047 prompt_man-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 prompt_man-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0      968 2023-05-06 20:51:52.049872 prompt_man-0.1.4/README.md
+-rwxr-xr-x   0        0        0      169 2023-05-06 22:03:10.351152 prompt_man-0.1.4/prompt_man/__init__.py
+-rwxr-xr-x   0        0        0       77 2023-05-06 22:03:01.245287 prompt_man-0.1.4/prompt_man/hello.py
+-rwxr-xr-x   0        0        0     1161 2023-05-06 21:53:18.053315 prompt_man-0.1.4/prompt_man/stablediffusion.py
+-rwxr-xr-x   0        0        0      559 2023-05-06 22:07:30.903318 prompt_man-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 prompt_man-0.1.4/PKG-INFO
```

### Comparing `prompt_man-0.1.3/README.md` & `prompt_man-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `prompt_man-0.1.3/pyproject.toml` & `prompt_man-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prompt-man"
-version = "0.1.3"
+version = "0.1.4"
 description = "Package for prompt engineering"
 authors = ["Amar <amar439412@gmail.com>"]
 readme = "README.md"
 packages = [{include = "prompt_man"}]
 license = "MIT"
 homepage = "https://github.com/Amar-89"
 repository = "https://github.com/Amar-89/prompt-man"
```

### Comparing `prompt_man-0.1.3/PKG-INFO` & `prompt_man-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-man
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for prompt engineering
 Home-page: https://github.com/Amar-89
 License: MIT
 Author: Amar
 Author-email: amar439412@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

