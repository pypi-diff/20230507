# Comparing `tmp/prompt_man-0.1.4.tar.gz` & `tmp/prompt_man-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_man-0.1.4.tar", max compression
+gzip compressed data, was "prompt_man-0.1.5.tar", max compression
```

## Comparing `prompt_man-0.1.4.tar` & `prompt_man-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0      968 2023-05-06 20:51:52.049872 prompt_man-0.1.4/README.md
--rwxr-xr-x   0        0        0      169 2023-05-06 22:03:10.351152 prompt_man-0.1.4/prompt_man/__init__.py
--rwxr-xr-x   0        0        0       77 2023-05-06 22:03:01.245287 prompt_man-0.1.4/prompt_man/hello.py
--rwxr-xr-x   0        0        0     1161 2023-05-06 21:53:18.053315 prompt_man-0.1.4/prompt_man/stablediffusion.py
--rwxr-xr-x   0        0        0      559 2023-05-06 22:07:30.903318 prompt_man-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 prompt_man-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0      968 2023-05-06 20:51:52.049872 prompt_man-0.1.5/README.md
+-rwxr-xr-x   0        0        0      145 2023-05-07 10:36:45.803453 prompt_man-0.1.5/prompt_man/__init__.py
+-rwxr-xr-x   0        0        0       77 2023-05-06 22:03:01.245287 prompt_man-0.1.5/prompt_man/hello.py
+-rwxr-xr-x   0        0        0     7941 2023-05-07 10:42:17.631488 prompt_man-0.1.5/prompt_man/stablediffusion.py
+-rwxr-xr-x   0        0        0      494 2023-05-07 10:42:03.859526 prompt_man-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 prompt_man-0.1.5/PKG-INFO
```

### Comparing `prompt_man-0.1.4/README.md` & `prompt_man-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `prompt_man-0.1.4/PKG-INFO` & `prompt_man-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: prompt-man
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package for prompt engineering
 Home-page: https://github.com/Amar-89
 License: MIT
 Author: Amar
 Author-email: amar439412@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openai (>=0.27.6,<0.28.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: replicate (>=0.8.1,<0.9.0)
 Project-URL: Repository, https://github.com/Amar-89/prompt-man
 Description-Content-Type: text/markdown
 
 # Prompt Man
 
 Prompt engineering package for AI models.
```

