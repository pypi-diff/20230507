# Comparing `tmp/django-erp-framework-0.9.0.tar.gz` & `tmp/django-erp-framework-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-erp-framework-0.9.0.tar", last modified: Sat May  6 12:35:53 2023, max compression
+gzip compressed data, was "django-erp-framework-0.9.1.tar", last modified: Sun May  7 13:03:00 2023, max compression
```

## Comparing `django-erp-framework-0.9.0.tar` & `django-erp-framework-0.9.1.tar`

### file list

```diff
@@ -1,84 +1,64 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/
--rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-0.9.0/LICENSE
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-0.9.0/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4976 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3352 2023-05-06 12:34:52.000000 django-erp-framework-0.9.0/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/django_erp_framework.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4976 2023-05-06 12:35:53.000000 django-erp-framework-0.9.0/django_erp_framework.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2381 2023-05-06 12:35:53.000000 django-erp-framework-0.9.0/django_erp_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 12:35:53.000000 django-erp-framework-0.9.0/django_erp_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      205 2023-05-06 12:35:53.000000 django-erp-framework-0.9.0/django_erp_framework.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-06 12:35:53.000000 django-erp-framework-0.9.0/django_erp_framework.egg-info/top_level.txt
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       97 2023-05-06 12:35:45.000000 django-erp-framework-0.9.0/erp_framework/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/activity/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/activity/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8367 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/activity/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/activity/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/activity/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/activity/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/activity/migrations/0002_auto_20200711_1253.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/activity/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/activity/models.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/admin/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       62 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    51228 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7476 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/base.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      667 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/helpers.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/admin/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2450 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/templatetags/erp_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4338 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/templatetags/ra_admin_list.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1783 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/templatetags/ra_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    18435 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/admin/templatetags/suit_menu.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      618 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/base/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/base/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2992 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/base/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7609 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/base/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    16862 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/base/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3415 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/base/registry.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1726 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/base/widgets.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2422 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/checks.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/contrib/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/contrib/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/contrib/jazzmin_integration/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/contrib/jazzmin_integration/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.941654 django-erp-framework-0.9.0/erp_framework/erp/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/erp_framework/erp/expense/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/expense/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      416 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/expense/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      285 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/expense/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/erp_framework/erp/expense/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     6810 2023-05-06 01:10:30.000000 django-erp-framework-0.9.0/erp_framework/erp/expense/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      831 2022-09-04 05:18:22.000000 django-erp-framework-0.9.0/erp_framework/erp/expense/migrations/0002_auto_20200711_1253.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2020-06-01 20:49:48.000000 django-erp-framework-0.9.0/erp_framework/erp/expense/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      593 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/expense/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5964 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/expense/reports.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/erp_framework/erp/treasury/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       70 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/treasury/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/treasury/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      258 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/treasury/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/erp_framework/erp/treasury/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3368 2023-05-06 01:10:30.000000 django-erp-framework-0.9.0/erp_framework/erp/treasury/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      835 2022-09-04 05:18:22.000000 django-erp-framework-0.9.0/erp_framework/erp/treasury/migrations/0002_auto_20200711_1253.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2020-06-01 20:49:53.000000 django-erp-framework-0.9.0/erp_framework/erp/treasury/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      235 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/erp/treasury/models.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/erp_framework/reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      346 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/reporting/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      164 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/reporting/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/reporting/printing.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5552 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/reporting/registry.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    26893 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/reporting/views.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/erp_framework/utils/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/utils/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      454 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/utils/navigation.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3937 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/utils/permissions.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-0.9.0/erp_framework/utils/views.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1761 2023-05-06 12:35:53.945654 django-erp-framework-0.9.0/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-0.9.0/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-0.9.1/LICENSE
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-0.9.1/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4976 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3352 2023-05-06 12:34:52.000000 django-erp-framework-0.9.1/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/django_erp_framework.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4976 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1756 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      205 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-07 13:03:00.000000 django-erp-framework-0.9.1/django_erp_framework.egg-info/top_level.txt
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       97 2023-05-07 13:02:56.000000 django-erp-framework-0.9.1/erp_framework/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/activity/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8367 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/activity/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/migrations/0002_auto_20200711_1253.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-0.9.1/erp_framework/activity/migrations/0003_alter_myactivity_options.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/activity/models.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/admin/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       62 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    51228 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7476 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/base.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      667 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/helpers.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/admin/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2450 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/erp_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4338 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/ra_admin_list.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1783 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/ra_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    18435 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/admin/templatetags/suit_menu.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      618 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/base/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2992 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7609 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    16862 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3415 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/registry.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1726 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/base/widgets.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2422 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/checks.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/contrib/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/contrib/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/contrib/jazzmin_integration/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/contrib/jazzmin_integration/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      346 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      164 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/printing.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5552 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/reporting/registry.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    26830 2023-05-07 05:11:23.000000 django-erp-framework-0.9.1/erp_framework/reporting/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/erp_framework/utils/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/utils/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      454 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/utils/navigation.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3937 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/utils/permissions.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-0.9.1/erp_framework/utils/views.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1761 2023-05-07 13:03:00.710692 django-erp-framework-0.9.1/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-0.9.1/setup.py
```

### Comparing `django-erp-framework-0.9.0/LICENSE` & `django-erp-framework-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/PKG-INFO` & `django-erp-framework-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 0.9.0
+Version: 0.9.1
 Summary: A light-weight effective Django based framework to create diverse business applications
 Home-page: https://github.com/ra-systems/RA
 Author: Ra Systems
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
```

### Comparing `django-erp-framework-0.9.0/README.rst` & `django-erp-framework-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/django_erp_framework.egg-info/PKG-INFO` & `django-erp-framework-0.9.1/django_erp_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 0.9.0
+Version: 0.9.1
 Summary: A light-weight effective Django based framework to create diverse business applications
 Home-page: https://github.com/ra-systems/RA
 Author: Ra Systems
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
```

### Comparing `django-erp-framework-0.9.0/django_erp_framework.egg-info/SOURCES.txt` & `django-erp-framework-0.9.1/django_erp_framework.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 erp_framework/checks.py
 erp_framework/activity/__init__.py
 erp_framework/activity/admin.py
 erp_framework/activity/apps.py
 erp_framework/activity/models.py
 erp_framework/activity/migrations/0001_initial.py
 erp_framework/activity/migrations/0002_auto_20200711_1253.py
+erp_framework/activity/migrations/0003_alter_myactivity_options.py
 erp_framework/activity/migrations/__init__.py
 erp_framework/admin/__init__.py
 erp_framework/admin/admin.py
 erp_framework/admin/apps.py
 erp_framework/admin/base.py
 erp_framework/admin/forms.py
 erp_framework/admin/helpers.py
@@ -33,30 +34,14 @@
 erp_framework/base/app_settings.py
 erp_framework/base/helpers.py
 erp_framework/base/models.py
 erp_framework/base/registry.py
 erp_framework/base/widgets.py
 erp_framework/contrib/__init__.py
 erp_framework/contrib/jazzmin_integration/__init__.py
-erp_framework/erp/__init__.py
-erp_framework/erp/expense/__init__.py
-erp_framework/erp/expense/admin.py
-erp_framework/erp/expense/apps.py
-erp_framework/erp/expense/models.py
-erp_framework/erp/expense/reports.py
-erp_framework/erp/expense/migrations/0001_initial.py
-erp_framework/erp/expense/migrations/0002_auto_20200711_1253.py
-erp_framework/erp/expense/migrations/__init__.py
-erp_framework/erp/treasury/__init__.py
-erp_framework/erp/treasury/admin.py
-erp_framework/erp/treasury/apps.py
-erp_framework/erp/treasury/models.py
-erp_framework/erp/treasury/migrations/0001_initial.py
-erp_framework/erp/treasury/migrations/0002_auto_20200711_1253.py
-erp_framework/erp/treasury/migrations/__init__.py
 erp_framework/reporting/__init__.py
 erp_framework/reporting/apps.py
 erp_framework/reporting/forms.py
 erp_framework/reporting/models.py
 erp_framework/reporting/printing.py
 erp_framework/reporting/registry.py
 erp_framework/reporting/views.py
```

### Comparing `django-erp-framework-0.9.0/erp_framework/activity/admin.py` & `django-erp-framework-0.9.1/erp_framework/activity/admin.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/activity/migrations/0001_initial.py` & `django-erp-framework-0.9.1/erp_framework/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/admin/admin.py` & `django-erp-framework-0.9.1/erp_framework/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/admin/base.py` & `django-erp-framework-0.9.1/erp_framework/admin/base.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/admin/forms.py` & `django-erp-framework-0.9.1/erp_framework/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/admin/helpers.py` & `django-erp-framework-0.9.1/erp_framework/admin/helpers.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/admin/templatetags/erp_reporting_tags.py` & `django-erp-framework-0.9.1/erp_framework/admin/templatetags/erp_reporting_tags.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/admin/templatetags/ra_admin_list.py` & `django-erp-framework-0.9.1/erp_framework/admin/templatetags/ra_admin_list.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/admin/templatetags/ra_tags.py` & `django-erp-framework-0.9.1/erp_framework/admin/templatetags/ra_tags.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/admin/templatetags/suit_menu.py` & `django-erp-framework-0.9.1/erp_framework/admin/templatetags/suit_menu.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/apps.py` & `django-erp-framework-0.9.1/erp_framework/apps.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/base/app_settings.py` & `django-erp-framework-0.9.1/erp_framework/base/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/base/helpers.py` & `django-erp-framework-0.9.1/erp_framework/base/helpers.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/base/models.py` & `django-erp-framework-0.9.1/erp_framework/base/models.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/base/registry.py` & `django-erp-framework-0.9.1/erp_framework/base/registry.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/base/widgets.py` & `django-erp-framework-0.9.1/erp_framework/base/widgets.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/checks.py` & `django-erp-framework-0.9.1/erp_framework/checks.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/reporting/forms.py` & `django-erp-framework-0.9.1/erp_framework/reporting/forms.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/reporting/printing.py` & `django-erp-framework-0.9.1/erp_framework/reporting/printing.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/reporting/registry.py` & `django-erp-framework-0.9.1/erp_framework/reporting/registry.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/reporting/views.py` & `django-erp-framework-0.9.1/erp_framework/reporting/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,17 +294,14 @@
     # required , the main model which the report is about.
     # We will be getting the doc_types (if any) from this model and be basing the calculation on.
     base_model = None
 
     # the report form, A subclass of ReportForm is to expected
     form_class = None
 
-    # control the settings of report
-    form_settings = None
-
     # control the chart settings, passed to front end as is.
     chart_settings = None
 
     other_namespaces = None
     columns = None
 
     report_slug = ""
```

### Comparing `django-erp-framework-0.9.0/erp_framework/utils/permissions.py` & `django-erp-framework-0.9.1/erp_framework/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/erp_framework/utils/views.py` & `django-erp-framework-0.9.1/erp_framework/utils/views.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-0.9.0/setup.cfg` & `django-erp-framework-0.9.1/setup.cfg`

 * *Files identical despite different names*

