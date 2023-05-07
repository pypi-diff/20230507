# Comparing `tmp/md-anchors-0.2.1.tar.gz` & `tmp/md-anchors-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md-anchors-0.2.1.tar", last modified: Thu Mar 16 13:07:41 2023, max compression
+gzip compressed data, was "md-anchors-0.2.2.tar", last modified: Sun May  7 10:38:07 2023, max compression
```

## Comparing `md-anchors-0.2.1.tar` & `md-anchors-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:07:41.345426 md-anchors-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-16 13:07:21.000000 md-anchors-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-16 13:07:41.345426 md-anchors-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-16 13:07:21.000000 md-anchors-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:07:41.345426 md-anchors-0.2.1/md_anchors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-16 13:07:41.000000 md-anchors-0.2.1/md_anchors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-16 13:07:41.000000 md-anchors-0.2.1/md_anchors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:07:41.000000 md-anchors-0.2.1/md_anchors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-16 13:07:41.000000 md-anchors-0.2.1/md_anchors.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:07:41.345426 md-anchors-0.2.1/mdanchors/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-16 13:07:21.000000 md-anchors-0.2.1/mdanchors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-03-16 13:07:21.000000 md-anchors-0.2.1/mdanchors/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-16 13:07:21.000000 md-anchors-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-16 13:07:41.349426 md-anchors-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:07:41.345426 md-anchors-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:07:21.000000 md-anchors-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-03-16 13:07:21.000000 md-anchors-0.2.1/tests/test_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:38:07.166505 md-anchors-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-07 10:37:48.000000 md-anchors-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-07 10:38:07.166505 md-anchors-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-07 10:37:48.000000 md-anchors-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:38:07.166505 md-anchors-0.2.2/md_anchors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-07 10:38:07.000000 md-anchors-0.2.2/md_anchors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-07 10:38:07.000000 md-anchors-0.2.2/md_anchors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:38:07.000000 md-anchors-0.2.2/md_anchors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 10:38:07.000000 md-anchors-0.2.2/md_anchors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:38:07.166505 md-anchors-0.2.2/mdanchors/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-07 10:37:48.000000 md-anchors-0.2.2/mdanchors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-07 10:37:48.000000 md-anchors-0.2.2/mdanchors/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 10:37:48.000000 md-anchors-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-07 10:38:07.166505 md-anchors-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:38:07.166505 md-anchors-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:37:48.000000 md-anchors-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-07 10:37:48.000000 md-anchors-0.2.2/tests/test_converters.py
```

### Comparing `md-anchors-0.2.1/LICENSE` & `md-anchors-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `md-anchors-0.2.1/PKG-INFO` & `md-anchors-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md-anchors
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tiny lib to work with Markdown / CommonMark anchors.
 Home-page: https://github.com/LeMinaw/md-anchors
 Author: LeMinaw
 Author-email: leminaw@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `md-anchors-0.2.1/md_anchors.egg-info/PKG-INFO` & `md-anchors-0.2.2/md_anchors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md-anchors
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tiny lib to work with Markdown / CommonMark anchors.
 Home-page: https://github.com/LeMinaw/md-anchors
 Author: LeMinaw
 Author-email: leminaw@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `md-anchors-0.2.1/mdanchors/converters.py` & `md-anchors-0.2.2/mdanchors/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class AnchorConverter:
     """Class allowing to perform anchor conversions operations on a Markdown /
     CommonMark source text.
     """
     # Match inline URIs
-    inlines_exp = re.compile(r'\[[^()[\]]*\]\s?\((?P<uri>[^()[\]]+)\)')
+    inlines_exp = re.compile(r'[^]]\s*\[[^()[\]]*\]\s?\((?P<uri>[^()[\]]+)\)')
     # Match inline anchors identifiers
     anchors_exp = re.compile(r'\[[^()[\]]*\]\s?\[(?P<ref>[^()[\]]+)\]')
     # Match reference-style anchors
     references_exp = re.compile(
         r'^\s*\[(?P<ref>[^()[\]]+)\]\s*:\s*(?P<uri>[^\r\n]*)\s*$', re.M
     )
```

### Comparing `md-anchors-0.2.1/setup.cfg` & `md-anchors-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `md-anchors-0.2.1/tests/test_converters.py` & `md-anchors-0.2.2/tests/test_converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,26 @@
         "uri://hello",
         "uri://hi",
         "uri://other",
         "uri://unused"
     }
 
 
-def test_get_crlf():
+def test_get_uris_brakets():
+    text = (
+        "Hello, [something][1] (some more info).\n"
+        "Some [other stuff][2][hey].\n"
+        "\n"
+        "[1]: uri://hello\n"
+        "[2]: uri://other\n"
+    )
+    assert AnchorConverter(text).uris == { "uri://hello", "uri://other" }
+
+
+def test_get_uris_crlf():
     text = (
         "Hello, [inline link][1], [inline link][2].\r\n"
         "\r\n"
         "[1]: uri://hi\r\n"
         "[2]: uri://other\r\n"
     )
     assert AnchorConverter(text).uris == { "uri://hi", "uri://other" }
```

