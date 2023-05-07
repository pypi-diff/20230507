# Comparing `tmp/neapolitan-23.8.tar.gz` & `tmp/neapolitan-23.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-23.8.tar", last modified: Mon Apr 24 09:55:40 2023, max compression
+gzip compressed data, was "neapolitan-23.9.tar", last modified: Fri Apr 28 10:28:08 2023, max compression
```

## Comparing `neapolitan-23.8.tar` & `neapolitan-23.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.8/.gitignore
--rw-r--r--   0        0        0      653 2023-04-24 09:42:29.532121 neapolitan-23.8/CHANGELOG.rst
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.8/LICENSE
--rw-r--r--   0        0        0     1933 2023-04-21 14:19:08.925095 neapolitan-23.8/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.8/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.8/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.8/docs/source/conf.py
--rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.8/docs/source/crud-view.rst
--rw-r--r--   0        0        0     2016 2023-04-21 16:00:29.106838 neapolitan-23.8/docs/source/index.rst
--rw-r--r--   0        0        0     1028 2023-04-24 09:51:45.493372 neapolitan-23.8/docs/source/templates.rst
--rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.8/justfile
--rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.8/pyproject.toml
--rw-r--r--   0        0        0      978 2023-04-24 09:54:57.892476 neapolitan-23.8/src/neapolitan/__init__.py
--rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.8/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.8/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      427 2023-04-12 09:54:30.457200 neapolitan-23.8/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      381 2023-04-12 07:36:22.945023 neapolitan-23.8/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.8/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.8/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.8/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1899 2023-04-24 09:52:53.326834 neapolitan-23.8/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.8/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.8/tests/__init__.py
--rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.8/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.8/tests/migrations/__init__.py
--rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.8/tests/models.py
--rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.8/tests/settings.py
--rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.8/tests/templates/base.html
--rw-r--r--   0        0        0     4434 2023-04-12 09:58:49.359041 neapolitan-23.8/tests/tests.py
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 neapolitan-23.8/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-04-28 08:55:04.319695 neapolitan-23.9/.gitignore
+-rw-r--r--   0        0        0     1552 2023-04-28 10:25:22.626352 neapolitan-23.9/CHANGELOG.rst
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.9/LICENSE
+-rw-r--r--   0        0        0     1933 2023-04-21 14:19:08.925095 neapolitan-23.9/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.9/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.9/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.9/docs/source/conf.py
+-rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.9/docs/source/crud-view.rst
+-rw-r--r--   0        0        0     2016 2023-04-21 16:00:29.106838 neapolitan-23.9/docs/source/index.rst
+-rw-r--r--   0        0        0     2120 2023-04-28 10:24:39.883366 neapolitan-23.9/docs/source/templates.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.9/justfile
+-rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.9/pyproject.toml
+-rw-r--r--   0        0        0      978 2023-04-26 07:49:09.307070 neapolitan-23.9/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.9/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.9/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      658 2023-04-27 15:58:09.343227 neapolitan-23.9/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      828 2023-04-26 08:25:21.941626 neapolitan-23.9/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      337 2023-04-26 07:59:35.829107 neapolitan-23.9/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0     1142 2023-04-26 08:56:04.084378 neapolitan-23.9/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.9/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1899 2023-04-24 09:52:53.326834 neapolitan-23.9/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.9/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.9/tests/__init__.py
+-rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.9/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.9/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.9/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.9/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.9/tests/templates/base.html
+-rw-r--r--   0        0        0     4434 2023-04-12 09:58:49.359041 neapolitan-23.9/tests/tests.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 neapolitan-23.9/PKG-INFO
```

### Comparing `neapolitan-23.8/LICENSE` & `neapolitan-23.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/README.rst` & `neapolitan-23.9/README.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/docs/Makefile` & `neapolitan-23.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/docs/make.bat` & `neapolitan-23.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/docs/source/conf.py` & `neapolitan-23.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/docs/source/index.rst` & `neapolitan-23.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/pyproject.toml` & `neapolitan-23.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/src/neapolitan/__init__.py` & `neapolitan-23.9/src/neapolitan/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 """
 
-__version__ = "23.8"
+__version__ = "23.9"
```

### Comparing `neapolitan-23.8/src/neapolitan/templatetags/neapolitan.py` & `neapolitan-23.9/src/neapolitan/templatetags/neapolitan.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/src/neapolitan/views.py` & `neapolitan-23.9/src/neapolitan/views.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/tests/migrations/0001_initial.py` & `neapolitan-23.9/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/tests/settings.py` & `neapolitan-23.9/tests/settings.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/tests/tests.py` & `neapolitan-23.9/tests/tests.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.8/PKG-INFO` & `neapolitan-23.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neapolitan
-Version: 23.8
+Version: 23.9
 Summary: Neapolitan: quick CRUD views for Django.
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django
 Requires-Dist: django-filter
 Requires-Dist: Sphinx ; extra == "docs"
```

