# Comparing `tmp/django-app-helper-3.2.0.tar.gz` & `tmp/django-app-helper-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-app-helper-3.2.0.tar", last modified: Thu Jan 19 07:09:23 2023, max compression
+gzip compressed data, was "django-app-helper-3.3.0.tar", last modified: Sun May  7 16:48:47 2023, max compression
```

## Comparing `django-app-helper-3.2.0.tar` & `django-app-helper-3.3.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.177998 django-app-helper-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-01-19 07:09:23.177998 django-app-helper-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/app_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23598 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/default_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.169998 django-app-helper-3.2.0/app_helper/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.169998 django-app-helper-3.2.0/app_helper/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/app_helper/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/pytest_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/app_helper/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/test_data/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/app_helper/test_data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/test_data/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/test_data/templates/fullwidth.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/test_data/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/app_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/django_app_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-01-19 07:09:23.000000 django-app-helper-3.2.0/django_app_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-19 07:09:23.000000 django-app-helper-3.2.0/django_app_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 07:09:23.000000 django-app-helper-3.2.0/django_app_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-19 07:09:23.000000 django-app-helper-3.2.0/django_app_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 07:09:11.000000 django-app-helper-3.2.0/django_app_helper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-19 07:09:23.000000 django-app-helper-3.2.0/django_app_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-19 07:09:23.000000 django-app-helper-3.2.0/django_app_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/djangocms_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/djangocms_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-01-19 07:09:23.177998 django-app-helper-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    38326 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_others.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/cms_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/cms_helper_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/cms_helper_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/cms_helper_extra_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.173998 django-app-helper-3.2.0/tests/test_utils/custom_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/custom_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/custom_user/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.177998 django-app-helper-3.2.0/tests/test_utils/example1/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/cms_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/cms_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.177998 django-app-helper-3.2.0/tests/test_utils/example1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/tests/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 07:09:23.177998 django-app-helper-3.2.0/tests/test_utils/example2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/example2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/helper_no_cms.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-01-19 07:08:48.000000 django-app-helper-3.2.0/tests/test_utils/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14350 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.029045 django-app-helper-3.3.0/app_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23598 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/default_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.025045 django-app-helper-3.3.0/app_helper/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.025045 django-app-helper-3.3.0/app_helper/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.029045 django-app-helper-3.3.0/app_helper/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/pytest_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.029045 django-app-helper-3.3.0/app_helper/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.029045 django-app-helper-3.3.0/app_helper/test_data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/templates/fullwidth.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/django_app_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14350 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:48:28.000000 django-app-helper-3.3.0/django_app_helper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/djangocms_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/djangocms_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38637 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_others.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/cms_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/cms_helper_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/cms_helper_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/cms_helper_extra_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/tests/test_utils/custom_user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/custom_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/custom_user/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/tests/test_utils/example1/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/cms_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/cms_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/tests/test_utils/example1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/tests/test_utils/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/helper_no_cms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/runners.py
```

### Comparing `django-app-helper-3.2.0/CONTRIBUTING.rst` & `django-app-helper-3.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/HISTORY.rst` & `django-app-helper-3.3.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+3.3.0 (2023-05-07)
+==================
+
+Features
+--------
+
+- Add support for Django 4.x (#208)
+
+
 3.2.0 (2023-01-19)
 ==================
 
 Features
 --------
 
 - Add djangocms 3.11 to tox, fix tests accordingly (#311)
```

### Comparing `django-app-helper-3.2.0/LICENSE` & `django-app-helper-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/PKG-INFO` & `django-app-helper-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-app-helper
-Version: 3.2.0
+Version: 3.3.0
 Summary: Helper for django applications development
 Home-page: https://github.com/nephila/django-app-helper
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: GPLv2+
 Project-URL: Documentation, https://django-app-helper.readthedocs.io/
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -204,14 +205,23 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+3.3.0 (2023-05-07)
+==================
+
+Features
+--------
+
+- Add support for Django 4.x (#208)
+
+
 3.2.0 (2023-01-19)
 ==================
 
 Features
 --------
 
 - Add djangocms 3.11 to tox, fix tests accordingly (#311)
```

### Comparing `django-app-helper-3.2.0/README.rst` & `django-app-helper-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/base_test.py` & `django-app-helper-3.3.0/app_helper/base_test.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/default_settings.py` & `django-app-helper-3.3.0/app_helper/default_settings.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/locale/en/LC_MESSAGES/django.po` & `django-app-helper-3.3.0/app_helper/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/main.py` & `django-app-helper-3.3.0/app_helper/main.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/pytest_runner.py` & `django-app-helper-3.3.0/app_helper/pytest_runner.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/runner.py` & `django-app-helper-3.3.0/app_helper/runner.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/server.py` & `django-app-helper-3.3.0/app_helper/server.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/test_data/templates/base.html` & `django-app-helper-3.3.0/app_helper/test_data/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/app_helper/urls.py` & `django-app-helper-3.3.0/app_helper/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django.conf import settings
-from django.conf.urls import include
 from django.conf.urls.i18n import i18n_patterns
 from django.contrib import admin
 from django.contrib.staticfiles.urls import staticfiles_urlpatterns
-from django.urls import re_path
+from django.urls import include, path, re_path
 from django.views.i18n import JavaScriptCatalog
 from django.views.static import serve
 
 from .utils import load_from_file
 
 admin.autodiscover()
 
@@ -24,11 +23,11 @@
     i18n_urls.append(
         re_path(r"^%s/" % settings.BASE_APPLICATION, include("%s.urls" % settings.BASE_APPLICATION))
     )  # NOQA
 except OSError:  # pragma: no cover
     pass
 
 if settings.USE_CMS:
-    i18n_urls.append(re_path(r"^", include("cms.urls")))  # NOQA
+    i18n_urls.append(path("", include("cms.urls")))  # NOQA
 
 urlpatterns += i18n_patterns(*i18n_urls)
 urlpatterns += staticfiles_urlpatterns()
```

### Comparing `django-app-helper-3.2.0/app_helper/utils.py` & `django-app-helper-3.3.0/app_helper/utils.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/django_app_helper.egg-info/PKG-INFO` & `django-app-helper-3.3.0/django_app_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-app-helper
-Version: 3.2.0
+Version: 3.3.0
 Summary: Helper for django applications development
 Home-page: https://github.com/nephila/django-app-helper
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: GPLv2+
 Project-URL: Documentation, https://django-app-helper.readthedocs.io/
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -204,14 +205,23 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+3.3.0 (2023-05-07)
+==================
+
+Features
+--------
+
+- Add support for Django 4.x (#208)
+
+
 3.2.0 (2023-01-19)
 ==================
 
 Features
 --------
 
 - Add djangocms 3.11 to tox, fix tests accordingly (#311)
```

### Comparing `django-app-helper-3.2.0/django_app_helper.egg-info/SOURCES.txt` & `django-app-helper-3.3.0/django_app_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/setup.cfg` & `django-app-helper-3.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [bumpversion]
-current_version = 3.2.0
+current_version = 3.3.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.?)(?P<release>[a-z]*)(?P<relver>\d*)
 serialize = 
 	{major}.{minor}.{patch}.{release}{relver}
 	{major}.{minor}.{patch}
 commit = True
-tag = True
+tag = False
 sign_tags = True
 tag_name = {new_version}
 message = Release {new_version}
 
 [bumpversion:part:release]
 optional_value = gamma
 values = 
@@ -34,16 +34,17 @@
 long_description_content_type = text/x-rst
 license = GPLv2+
 license_file = LICENSE
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
-	Framework :: Django :: 2.2
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
```

### Comparing `django-app-helper-3.2.0/tests/test_base_classes.py` & `django-app-helper-3.3.0/tests/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/tests/test_commands.py` & `django-app-helper-3.3.0/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,16 @@
                         # Check template dirs
                         self.assertTrue("some/dir" in local_settings.TEMPLATES[0]["DIRS"])
 
     @patch("app_helper.server.autoreload.run_with_reloader")
     def test_server_django(self, run_with_reloader):
         """Run server command and create default user - django version."""
         with work_in(self.basedir):
+            User = get_user_model()
+            User.objects.all().delete()
             with captured_output() as (out, err):
                 args = copy(DEFAULT_ARGS)
                 args["server"] = True
                 core(args, self.application)
             self.assertTrue("A admin user (username: admin, password: admin) has been created." in out.getvalue())
             self.assertEqual(run_with_reloader.call_args[0][0].__module__, "django.core.management.commands.runserver")
         User.objects.all().delete()
@@ -397,14 +399,16 @@
     @patch("app_helper.server.autoreload.run_with_reloader")
     def test_server_channels(self, run_with_reloader):
         """Run server command and create default user - channels version."""
         try:
             import channels  # noqa: F401
         except ImportError:
             raise unittest.SkipTest("channels is not available, skipping test")
+        if channels.__version__ > "4.0":
+            raise unittest.SkipTest("channels 4 removed support for runserver, use daphne version instead, skipping")
         with work_in(self.basedir):
             with captured_output() as (out, err):
                 args = copy(DEFAULT_ARGS)
                 args["server"] = True
                 args["--use-channels"] = True
                 core(args, self.application)
             self.assertTrue("A admin user (username: admin, password: admin) has been created." in out.getvalue())
@@ -416,14 +420,16 @@
     def test_server_daphne(self, run_with_reloader):
         """Run server command and create default user - daphne version."""
         try:
             import daphne  # noqa: F401
         except ImportError:
             raise unittest.SkipTest("daphne is not available, skipping test")
         with work_in(self.basedir):
+            User = get_user_model()
+            User.objects.all().delete()
             with captured_output() as (out, err):
                 args = copy(DEFAULT_ARGS)
                 args["server"] = True
                 args["--use-daphne"] = True
                 core(args, self.application)
             self.assertTrue("A admin user (username: admin, password: admin) has been created." in out.getvalue())
             self.assertEqual(run_with_reloader.call_args[0][0].__module__, "daphne.cli")
```

### Comparing `django-app-helper-3.2.0/tests/test_others.py` & `django-app-helper-3.3.0/tests/test_others.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/tests/test_utils/cms_helper.py` & `django-app-helper-3.3.0/tests/test_utils/cms_helper.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/tests/test_utils/cms_helper_custom.py` & `django-app-helper-3.3.0/tests/test_utils/cms_helper_custom.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/tests/test_utils/cms_helper_extra.py` & `django-app-helper-3.3.0/tests/test_utils/cms_helper_extra.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/tests/test_utils/example1/tests/test_fake.py` & `django-app-helper-3.3.0/tests/test_utils/example1/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/tests/test_utils/helper.py` & `django-app-helper-3.3.0/tests/test_utils/helper.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/tests/test_utils/helper_no_cms.py` & `django-app-helper-3.3.0/tests/test_utils/helper_no_cms.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.2.0/tests/test_utils/runners.py` & `django-app-helper-3.3.0/tests/test_utils/runners.py`

 * *Files identical despite different names*

