# Comparing `tmp/code_aimpetus-0.1.0-py3-none-any.whl.zip` & `tmp/code_aimpetus-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 5762 bytes, number of entries: 15
--rw-r--r--  2.0 fat       49 b- defN 20-Feb-02 00:00 code_aimpetus/__init__.py
--rw-r--r--  2.0 fat      530 b- defN 20-Feb-02 00:00 code_aimpetus/__main__.py
--rw-r--r--  2.0 fat      204 b- defN 20-Feb-02 00:00 code_aimpetus/celery_app.py
+Zip file size: 5878 bytes, number of entries: 15
+-rw-r--r--  2.0 fat      116 b- defN 20-Feb-02 00:00 code_aimpetus/__init__.py
+-rw-r--r--  2.0 fat      526 b- defN 20-Feb-02 00:00 code_aimpetus/__main__.py
+-rw-r--r--  2.0 fat      357 b- defN 20-Feb-02 00:00 code_aimpetus/celery.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 code_aimpetus/gh/__init__.py
 -rw-r--r--  2.0 fat      854 b- defN 20-Feb-02 00:00 code_aimpetus/gh/repo.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/__init__.py
 -rw-r--r--  2.0 fat      709 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/close.py
 -rw-r--r--  2.0 fat      643 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/list.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 code_aimpetus/gh/pull_requests/__init__.py
 -rw-r--r--  2.0 fat      635 b- defN 20-Feb-02 00:00 code_aimpetus/gh/pull_requests/list.py
-?rw-r--r--  2.0 fat      986 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat       55 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 fat     1092 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat     1287 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.0.dist-info/RECORD
-15 files, 7131 bytes uncompressed, 3584 bytes compressed:  49.7%
+?rw-r--r--  2.0 fat      986 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.1.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat       55 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 fat     1092 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat     1284 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.1.dist-info/RECORD
+15 files, 7344 bytes uncompressed, 3708 bytes compressed:  49.5%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
 Filename: code_aimpetus/__init__.py
 Comment: 
 
 Filename: code_aimpetus/__main__.py
 Comment: 
 
-Filename: code_aimpetus/celery_app.py
+Filename: code_aimpetus/celery.py
 Comment: 
 
 Filename: code_aimpetus/gh/__init__.py
 Comment: 
 
 Filename: code_aimpetus/gh/repo.py
 Comment: 
@@ -24,23 +24,23 @@
 
 Filename: code_aimpetus/gh/pull_requests/__init__.py
 Comment: 
 
 Filename: code_aimpetus/gh/pull_requests/list.py
 Comment: 
 
-Filename: code_aimpetus-0.1.0.dist-info/METADATA
+Filename: code_aimpetus-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: code_aimpetus-0.1.0.dist-info/WHEEL
+Filename: code_aimpetus-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: code_aimpetus-0.1.0.dist-info/entry_points.txt
+Filename: code_aimpetus-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: code_aimpetus-0.1.0.dist-info/licenses/LICENSE
+Filename: code_aimpetus-0.1.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: code_aimpetus-0.1.0.dist-info/RECORD
+Filename: code_aimpetus-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_aimpetus/__init__.py

```diff
@@ -1,3 +1,7 @@
 from dotenv import load_dotenv
 
+from .celery import app as celery_app
+
 load_dotenv()
+
+__all__ = ["celery_app"]
```

## code_aimpetus/__main__.py

```diff
@@ -1,9 +1,9 @@
 import click
-from celery_app import start_app
+from celery import start_app
 
 from code_aimpetus.gh.issues.close import close_issue
 from code_aimpetus.gh.issues.list import list_issues
 from code_aimpetus.gh.pull_requests.list import list_pull_requests
 from code_aimpetus.gh.repo import create_github_repo
```

## Comparing `code_aimpetus-0.1.0.dist-info/METADATA` & `code_aimpetus-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-aimpetus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Code.
 Project-URL: Homepage, https://github.com/BillSchumacher/CodeAImpteus
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/CodeAImpteus
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `code_aimpetus-0.1.0.dist-info/licenses/LICENSE` & `code_aimpetus-0.1.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

