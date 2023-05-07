# Comparing `tmp/django-eremaea2-2.0.8.tar.gz` & `tmp/django-eremaea2-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-eremaea2-2.0.8.tar", last modified: Wed Aug 10 17:06:59 2016, max compression
+gzip compressed data, was "dist/django-eremaea2-2.0.9.tar", last modified: Wed Aug 31 16:38:41 2016, max compression
```

## Comparing `django-eremaea2-2.0.8.tar` & `django-eremaea2-2.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/
--rw-r--r--   0 matwey    (1000) users      (100)      170 2016-04-10 11:52:37.000000 django-eremaea2-2.0.8/eremaea-purge@.service
--rw-r--r--   0 matwey    (1000) users      (100)     4350 2016-04-10 10:55:40.000000 django-eremaea2-2.0.8/README.md
--rw-r--r--   0 matwey    (1000) users      (100)       59 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/setup.cfg
-drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/django_eremaea2.egg-info/
--rw-r--r--   0 matwey    (1000) users      (100)      779 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/django_eremaea2.egg-info/SOURCES.txt
--rw-r--r--   0 matwey    (1000) users      (100)     5658 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/django_eremaea2.egg-info/PKG-INFO
--rw-r--r--   0 matwey    (1000) users      (100)        1 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/django_eremaea2.egg-info/dependency_links.txt
--rw-r--r--   0 matwey    (1000) users      (100)       81 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/django_eremaea2.egg-info/entry_points.txt
--rw-r--r--   0 matwey    (1000) users      (100)        8 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/django_eremaea2.egg-info/top_level.txt
-drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/tests/
--rw-r--r--   0 matwey    (1000) users      (100)     2432 2016-03-31 17:31:42.000000 django-eremaea2-2.0.8/tests/collection.py
--rw-r--r--   0 matwey    (1000) users      (100)     5757 2016-04-05 18:52:22.000000 django-eremaea2-2.0.8/tests/snapshot.py
--rw-r--r--   0 matwey    (1000) users      (100)     3968 2016-04-07 15:49:53.000000 django-eremaea2-2.0.8/tests/retention.py
--rw-r--r--   0 matwey    (1000) users      (100)     1107 2016-04-07 15:49:53.000000 django-eremaea2-2.0.8/tests/test_settings.py
--rw-r--r--   0 matwey    (1000) users      (100)        0 2016-03-31 17:31:42.000000 django-eremaea2-2.0.8/tests/__init__.py
--rw-r--r--   0 matwey    (1000) users      (100)       97 2016-03-31 17:31:42.000000 django-eremaea2-2.0.8/tests/urls.py
--rw-r--r--   0 matwey    (1000) users      (100)      359 2016-06-15 17:23:47.000000 django-eremaea2-2.0.8/tests/conf.py
--rw-r--r--   0 matwey    (1000) users      (100)      391 2016-06-15 17:16:24.000000 django-eremaea2-2.0.8/tests/test_all.py
-drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/tests/ctl/
--rw-r--r--   0 matwey    (1000) users      (100)     1940 2016-04-05 16:00:08.000000 django-eremaea2-2.0.8/tests/ctl/file.py
--rw-r--r--   0 matwey    (1000) users      (100)     2641 2016-04-07 16:58:32.000000 django-eremaea2-2.0.8/tests/ctl/client.py
--rw-r--r--   0 matwey    (1000) users      (100)        0 2016-04-01 09:38:29.000000 django-eremaea2-2.0.8/tests/ctl/__init__.py
--rw-r--r--   0 matwey    (1000) users      (100)      157 2016-08-10 15:47:12.000000 django-eremaea2-2.0.8/MANIFEST.in
-drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/eremaea/
--rw-r--r--   0 matwey    (1000) users      (100)        0 2016-03-31 17:31:42.000000 django-eremaea2-2.0.8/eremaea/__init__.py
-drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/eremaea/migrations/
--rw-r--r--   0 matwey    (1000) users      (100)        0 2016-04-02 13:30:43.000000 django-eremaea2-2.0.8/eremaea/migrations/__init__.py
--rw-r--r--   0 matwey    (1000) users      (100)     2310 2016-04-02 13:33:07.000000 django-eremaea2-2.0.8/eremaea/migrations/0001_initial.py
--rw-r--r--   0 matwey    (1000) users      (100)      398 2016-04-03 14:01:53.000000 django-eremaea2-2.0.8/eremaea/urls.py
--rw-r--r--   0 matwey    (1000) users      (100)     2789 2016-04-05 19:56:53.000000 django-eremaea2-2.0.8/eremaea/views.py
--rw-r--r--   0 matwey    (1000) users      (100)      333 2016-06-15 17:13:11.000000 django-eremaea2-2.0.8/eremaea/conf.py
--rw-r--r--   0 matwey    (1000) users      (100)     3262 2016-06-15 17:35:27.000000 django-eremaea2-2.0.8/eremaea/models.py
--rw-r--r--   0 matwey    (1000) users      (100)     1731 2016-03-31 17:31:42.000000 django-eremaea2-2.0.8/eremaea/serializers.py
-drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/eremaea/ctl/
--rw-r--r--   0 matwey    (1000) users      (100)     1602 2016-04-05 16:00:08.000000 django-eremaea2-2.0.8/eremaea/ctl/file.py
--rw-r--r--   0 matwey    (1000) users      (100)     2372 2016-08-10 17:00:37.000000 django-eremaea2-2.0.8/eremaea/ctl/commandline.py
--rw-r--r--   0 matwey    (1000) users      (100)     1311 2016-08-10 15:47:12.000000 django-eremaea2-2.0.8/eremaea/ctl/client.py
--rw-r--r--   0 matwey    (1000) users      (100)        0 2016-04-01 07:53:00.000000 django-eremaea2-2.0.8/eremaea/ctl/__init__.py
--rw-r--r--   0 matwey    (1000) users      (100)      360 2016-03-31 17:31:42.000000 django-eremaea2-2.0.8/runtests.py
--rw-r--r--   0 matwey    (1000) users      (100)     1170 2016-08-10 17:05:41.000000 django-eremaea2-2.0.8/setup.py
--rw-r--r--   0 matwey    (1000) users      (100)     5658 2016-08-10 17:06:59.000000 django-eremaea2-2.0.8/PKG-INFO
--rw-r--r--   0 matwey    (1000) users      (100)      272 2016-08-10 16:45:16.000000 django-eremaea2-2.0.8/eremaea-pull@.service
--rw-r--r--   0 matwey    (1000) users      (100)      163 2016-04-10 09:57:33.000000 django-eremaea2-2.0.8/eremaea-purge@.timer
+drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/
+-rw-r--r--   0 matwey    (1000) users      (100)      170 2016-04-10 11:52:37.000000 django-eremaea2-2.0.9/eremaea-purge@.service
+-rw-r--r--   0 matwey    (1000) users      (100)     4350 2016-04-10 10:55:40.000000 django-eremaea2-2.0.9/README.md
+-rw-r--r--   0 matwey    (1000) users      (100)       59 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/setup.cfg
+drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/django_eremaea2.egg-info/
+-rw-r--r--   0 matwey    (1000) users      (100)      779 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/django_eremaea2.egg-info/SOURCES.txt
+-rw-r--r--   0 matwey    (1000) users      (100)     5658 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/django_eremaea2.egg-info/PKG-INFO
+-rw-r--r--   0 matwey    (1000) users      (100)        1 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/django_eremaea2.egg-info/dependency_links.txt
+-rw-r--r--   0 matwey    (1000) users      (100)       81 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/django_eremaea2.egg-info/entry_points.txt
+-rw-r--r--   0 matwey    (1000) users      (100)        8 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/django_eremaea2.egg-info/top_level.txt
+drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/tests/
+-rw-r--r--   0 matwey    (1000) users      (100)     2432 2016-03-31 17:31:42.000000 django-eremaea2-2.0.9/tests/collection.py
+-rw-r--r--   0 matwey    (1000) users      (100)     5757 2016-04-05 18:52:22.000000 django-eremaea2-2.0.9/tests/snapshot.py
+-rw-r--r--   0 matwey    (1000) users      (100)     3968 2016-04-07 15:49:53.000000 django-eremaea2-2.0.9/tests/retention.py
+-rw-r--r--   0 matwey    (1000) users      (100)     1107 2016-04-07 15:49:53.000000 django-eremaea2-2.0.9/tests/test_settings.py
+-rw-r--r--   0 matwey    (1000) users      (100)        0 2016-03-31 17:31:42.000000 django-eremaea2-2.0.9/tests/__init__.py
+-rw-r--r--   0 matwey    (1000) users      (100)       97 2016-03-31 17:31:42.000000 django-eremaea2-2.0.9/tests/urls.py
+-rw-r--r--   0 matwey    (1000) users      (100)      359 2016-06-15 17:23:47.000000 django-eremaea2-2.0.9/tests/conf.py
+-rw-r--r--   0 matwey    (1000) users      (100)      391 2016-06-15 17:16:24.000000 django-eremaea2-2.0.9/tests/test_all.py
+drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/tests/ctl/
+-rw-r--r--   0 matwey    (1000) users      (100)     1940 2016-04-05 16:00:08.000000 django-eremaea2-2.0.9/tests/ctl/file.py
+-rw-r--r--   0 matwey    (1000) users      (100)     2641 2016-04-07 16:58:32.000000 django-eremaea2-2.0.9/tests/ctl/client.py
+-rw-r--r--   0 matwey    (1000) users      (100)        0 2016-04-01 09:38:29.000000 django-eremaea2-2.0.9/tests/ctl/__init__.py
+-rw-r--r--   0 matwey    (1000) users      (100)      157 2016-08-10 15:47:12.000000 django-eremaea2-2.0.9/MANIFEST.in
+drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/eremaea/
+-rw-r--r--   0 matwey    (1000) users      (100)        0 2016-03-31 17:31:42.000000 django-eremaea2-2.0.9/eremaea/__init__.py
+drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/eremaea/migrations/
+-rw-r--r--   0 matwey    (1000) users      (100)        0 2016-04-02 13:30:43.000000 django-eremaea2-2.0.9/eremaea/migrations/__init__.py
+-rw-r--r--   0 matwey    (1000) users      (100)     2310 2016-04-02 13:33:07.000000 django-eremaea2-2.0.9/eremaea/migrations/0001_initial.py
+-rw-r--r--   0 matwey    (1000) users      (100)      398 2016-04-03 14:01:53.000000 django-eremaea2-2.0.9/eremaea/urls.py
+-rw-r--r--   0 matwey    (1000) users      (100)     2789 2016-04-05 19:56:53.000000 django-eremaea2-2.0.9/eremaea/views.py
+-rw-r--r--   0 matwey    (1000) users      (100)      333 2016-06-15 17:13:11.000000 django-eremaea2-2.0.9/eremaea/conf.py
+-rw-r--r--   0 matwey    (1000) users      (100)     3262 2016-06-15 17:35:27.000000 django-eremaea2-2.0.9/eremaea/models.py
+-rw-r--r--   0 matwey    (1000) users      (100)     1731 2016-03-31 17:31:42.000000 django-eremaea2-2.0.9/eremaea/serializers.py
+drwxr-xr-x   0 matwey    (1000) users      (100)        0 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/eremaea/ctl/
+-rw-r--r--   0 matwey    (1000) users      (100)     1602 2016-04-05 16:00:08.000000 django-eremaea2-2.0.9/eremaea/ctl/file.py
+-rw-r--r--   0 matwey    (1000) users      (100)     2372 2016-08-10 17:00:37.000000 django-eremaea2-2.0.9/eremaea/ctl/commandline.py
+-rw-r--r--   0 matwey    (1000) users      (100)     1311 2016-08-10 15:47:12.000000 django-eremaea2-2.0.9/eremaea/ctl/client.py
+-rw-r--r--   0 matwey    (1000) users      (100)        0 2016-04-01 07:53:00.000000 django-eremaea2-2.0.9/eremaea/ctl/__init__.py
+-rw-r--r--   0 matwey    (1000) users      (100)      360 2016-03-31 17:31:42.000000 django-eremaea2-2.0.9/runtests.py
+-rw-r--r--   0 matwey    (1000) users      (100)     1170 2016-08-31 16:38:10.000000 django-eremaea2-2.0.9/setup.py
+-rw-r--r--   0 matwey    (1000) users      (100)     5658 2016-08-31 16:38:41.000000 django-eremaea2-2.0.9/PKG-INFO
+-rw-r--r--   0 matwey    (1000) users      (100)      310 2016-08-10 17:38:04.000000 django-eremaea2-2.0.9/eremaea-pull@.service
+-rw-r--r--   0 matwey    (1000) users      (100)      163 2016-04-10 09:57:33.000000 django-eremaea2-2.0.9/eremaea-purge@.timer
```

### Comparing `django-eremaea2-2.0.8/README.md` & `django-eremaea2-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/django_eremaea2.egg-info/SOURCES.txt` & `django-eremaea2-2.0.9/django_eremaea2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/django_eremaea2.egg-info/PKG-INFO` & `django-eremaea2-2.0.9/django_eremaea2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-eremaea2
-Version: 2.0.8
+Version: 2.0.9
 Summary: A simple Django application to store and show webcam snapshots
 Home-page: https://github.com/matwey/django-eremaea2
 Author: Matwey V. Kornilov
 Author-email: matwey.kornilov@gmail.com
 License: BSD-2-Clause
 Description: # django-eremaea2
```

### Comparing `django-eremaea2-2.0.8/tests/collection.py` & `django-eremaea2-2.0.9/tests/collection.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/tests/snapshot.py` & `django-eremaea2-2.0.9/tests/snapshot.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/tests/retention.py` & `django-eremaea2-2.0.9/tests/retention.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/tests/test_settings.py` & `django-eremaea2-2.0.9/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/tests/ctl/file.py` & `django-eremaea2-2.0.9/tests/ctl/file.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/tests/ctl/client.py` & `django-eremaea2-2.0.9/tests/ctl/client.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/eremaea/migrations/0001_initial.py` & `django-eremaea2-2.0.9/eremaea/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/eremaea/views.py` & `django-eremaea2-2.0.9/eremaea/views.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/eremaea/models.py` & `django-eremaea2-2.0.9/eremaea/models.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/eremaea/serializers.py` & `django-eremaea2-2.0.9/eremaea/serializers.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/eremaea/ctl/file.py` & `django-eremaea2-2.0.9/eremaea/ctl/file.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/eremaea/ctl/commandline.py` & `django-eremaea2-2.0.9/eremaea/ctl/commandline.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/eremaea/ctl/client.py` & `django-eremaea2-2.0.9/eremaea/ctl/client.py`

 * *Files identical despite different names*

### Comparing `django-eremaea2-2.0.8/setup.py` & `django-eremaea2-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 	README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 	name='django-eremaea2',
-	version='2.0.8',
+	version='2.0.9',
 	packages=['eremaea','eremaea.ctl','eremaea.migrations'],
 	entry_points={'console_scripts': [
 		'eremaeactl = eremaea.ctl.commandline:execute_from_commandline',
 	]},
 	include_package_data=True,
 	license='BSD-2-Clause',
 	description='A simple Django application to store and show webcam snapshots',
```

### Comparing `django-eremaea2-2.0.8/PKG-INFO` & `django-eremaea2-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-eremaea2
-Version: 2.0.8
+Version: 2.0.9
 Summary: A simple Django application to store and show webcam snapshots
 Home-page: https://github.com/matwey/django-eremaea2
 Author: Matwey V. Kornilov
 Author-email: matwey.kornilov@gmail.com
 License: BSD-2-Clause
 Description: # django-eremaea2
```

