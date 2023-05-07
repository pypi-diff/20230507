# Comparing `tmp/dj-rest-auth-3.0.0.tar.gz` & `tmp/dj-rest-auth-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-rest-auth-3.0.0.tar", last modified: Mon Feb 13 02:18:33 2023, max compression
+gzip compressed data, was "dj-rest-auth-4.0.0.tar", last modified: Sun May  7 05:38:10 2023, max compression
```

## Comparing `dj-rest-auth-3.0.0.tar` & `dj-rest-auth-4.0.0.tar`

### file list

```diff
@@ -1,189 +1,266 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.217092 dj-rest-auth-3.0.0/
--rw-r--r--   0 michael    (501) staff       (20)       52 2021-03-20 17:51:05.000000 dj-rest-auth-3.0.0/AUTHORS
--rw-r--r--   0 michael    (501) staff       (20)     1102 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)       89 2020-03-01 01:49:31.000000 dj-rest-auth-3.0.0/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     4130 2023-02-13 02:18:33.222175 dj-rest-auth-3.0.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     2815 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.119223 dj-rest-auth-3.0.0/dj_rest_auth/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-3.0.0/dj_rest_auth/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.130823 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      152 2021-07-11 17:17:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      149 2021-07-11 17:17:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/admin.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1467 2021-07-11 17:17:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2070 2022-07-17 22:38:08.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/forms.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     5531 2023-01-02 22:42:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1044 2022-07-17 22:38:08.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    11794 2023-01-02 22:42:47.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2854 2021-07-11 17:17:03.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1012 2021-07-11 17:17:03.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1255 2021-07-11 17:17:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     9589 2022-07-17 22:38:08.000000 dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      354 2023-02-13 02:13:39.000000 dj-rest-auth-3.0.0/dj_rest_auth/__version__.py
--rw-r--r--   0 michael    (501) staff       (20)       65 2021-05-16 17:38:17.000000 dj-rest-auth-3.0.0/dj_rest_auth/admin.py
--rw-r--r--   0 michael    (501) staff       (20)     3075 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/app_settings.py
--rw-r--r--   0 michael    (501) staff       (20)     2644 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/forms.py
--rw-r--r--   0 michael    (501) staff       (20)     6178 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/jwt_auth.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.108338 dj-rest-auth-3.0.0/dj_rest_auth/locale/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.100177 dj-rest-auth-3.0.0/dj_rest_auth/locale/ar/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.131435 dj-rest-auth-3.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3751 2023-02-13 02:02:19.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.100561 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.138833 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:52:06.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!63502!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:54:59.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64462!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:55:51.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64600!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:56:43.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64760!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:05:05.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65418!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65616!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65791!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65995!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!69818!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2443 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3195 2021-03-20 17:51:05.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.100954 dj-rest-auth-3.0.0/dj_rest_auth/locale/de/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.143802 dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65618!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65793!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65997!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!69820!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2230 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2983 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.101359 dj-rest-auth-3.0.0/dj_rest_auth/locale/es/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.147903 dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65620!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65795!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65999!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!69822!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2405 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3151 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.101736 dj-rest-auth-3.0.0/dj_rest_auth/locale/fa/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.148594 dj-rest-auth-3.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3514 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.102257 dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.152871 dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!65622!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!65797!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!66001!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!69824!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2293 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3015 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.102753 dj-rest-auth-3.0.0/dj_rest_auth/locale/hr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.153704 dj-rest-auth-3.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3091 2021-03-18 00:03:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.103330 dj-rest-auth-3.0.0/dj_rest_auth/locale/it/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.155280 dj-rest-auth-3.0.0/dj_rest_auth/locale/it/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3001 2020-05-09 22:17:42.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3904 2020-05-09 22:17:42.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.103731 dj-rest-auth-3.0.0/dj_rest_auth/locale/ja/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.156012 dj-rest-auth-3.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     5628 2020-12-04 02:36:07.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.104118 dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.159186 dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!65624!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!65799!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!66003!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!69826!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2562 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3296 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.104499 dj-rest-auth-3.0.0/dj_rest_auth/locale/nl/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.160295 dj-rest-auth-3.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2958 2021-03-20 17:51:05.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3524 2021-03-20 17:51:05.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.104896 dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.162839 dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!65626!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!65801!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!66005!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!69828!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2265 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2992 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.105282 dj-rest-auth-3.0.0/dj_rest_auth/locale/pt_BR/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.163870 dj-rest-auth-3.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2317 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3090 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.105660 dj-rest-auth-3.0.0/dj_rest_auth/locale/ro/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.165266 dj-rest-auth-3.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2979 2021-03-20 17:51:05.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3537 2021-03-20 17:51:05.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.106034 dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.169354 dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!65629!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!65804!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!66008!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!69831!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2773 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3508 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.106458 dj-rest-auth-3.0.0/dj_rest_auth/locale/sv/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.171142 dj-rest-auth-3.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2565 2020-12-04 02:36:07.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3774 2020-12-04 02:36:07.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.107286 dj-rest-auth-3.0.0/dj_rest_auth/locale/tr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.172690 dj-rest-auth-3.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2222 2020-04-27 03:53:49.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2920 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.107706 dj-rest-auth-3.0.0/dj_rest_auth/locale/uk/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.173416 dj-rest-auth-3.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3502 2021-03-18 00:03:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.108090 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.177333 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65632!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65807!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!66011!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!69834!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2243 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3019 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.108484 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.181748 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65634!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65809!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!66013!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!69836!django.mo
--rw-r--r--   0 michael    (501) staff       (20)      373 2021-05-16 17:13:56.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2337 2020-03-01 01:48:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0 michael    (501) staff       (20)      948 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/models.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.184985 dj-rest-auth-3.0.0/dj_rest_auth/registration/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.189668 dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      165 2021-07-11 17:17:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      811 2021-07-11 17:17:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     8838 2023-01-02 22:42:46.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      747 2022-07-17 22:38:11.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     8336 2022-07-17 22:38:08.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    10528 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/serializers.py
--rw-r--r--   0 michael    (501) staff       (20)     1299 2021-12-20 21:18:06.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/urls.py
--rw-r--r--   0 michael    (501) staff       (20)     7744 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/registration/views.py
--rw-r--r--   0 michael    (501) staff       (20)    12699 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/serializers.py
--rw-r--r--   0 michael    (501) staff       (20)     2990 2021-05-17 04:45:09.000000 dj-rest-auth-3.0.0/dj_rest_auth/social_serializers.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.205810 dj-rest-auth-3.0.0/dj_rest_auth/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.215656 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      158 2021-07-11 17:17:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1793 2022-07-17 22:38:11.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     4196 2022-07-17 22:38:08.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2461 2022-07-17 22:38:07.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    27867 2022-07-17 22:38:08.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     7032 2022-07-17 23:28:09.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     9113 2021-07-11 17:17:02.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     5299 2022-07-17 22:38:10.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2420 2021-12-20 07:18:27.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/django_urls.py
--rw-r--r--   0 michael    (501) staff       (20)     4012 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/mixins.py
--rw-r--r--   0 michael    (501) staff       (20)      140 2023-01-14 17:31:37.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/requirements.pip
--rw-r--r--   0 michael    (501) staff       (20)     2833 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/settings.py
--rw-r--r--   0 michael    (501) staff       (20)    43842 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/test_api.py
--rw-r--r--   0 michael    (501) staff       (20)     7157 2022-07-17 23:14:41.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/test_serializers.py
--rw-r--r--   0 michael    (501) staff       (20)    14004 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/test_social.py
--rw-r--r--   0 michael    (501) staff       (20)      289 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/test_utils.py
--rw-r--r--   0 michael    (501) staff       (20)     4541 2022-02-06 01:01:30.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/urls.py
--rw-r--r--   0 michael    (501) staff       (20)     1031 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/tests/utils.py
--rw-r--r--   0 michael    (501) staff       (20)     1198 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/urls.py
--rw-r--r--   0 michael    (501) staff       (20)      541 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/utils.py
--rw-r--r--   0 michael    (501) staff       (20)    10790 2023-02-13 02:09:01.000000 dj-rest-auth-3.0.0/dj_rest_auth/views.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-13 02:18:33.123225 dj-rest-auth-3.0.0/dj_rest_auth.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     4130 2023-02-13 02:18:32.000000 dj-rest-auth-3.0.0/dj_rest_auth.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     6183 2023-02-13 02:18:32.000000 dj-rest-auth-3.0.0/dj_rest_auth.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-02-13 02:18:32.000000 dj-rest-auth-3.0.0/dj_rest_auth.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2020-03-01 01:18:23.000000 dj-rest-auth-3.0.0/dj_rest_auth.egg-info/not-zip-safe
--rw-r--r--   0 michael    (501) staff       (20)       85 2023-02-13 02:18:32.000000 dj-rest-auth-3.0.0/dj_rest_auth.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       13 2023-02-13 02:18:32.000000 dj-rest-auth-3.0.0/dj_rest_auth.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)      474 2023-02-13 02:18:33.237098 dj-rest-auth-3.0.0/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1542 2023-01-14 17:31:37.000000 dj-rest-auth-3.0.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.092239 dj-rest-auth-4.0.0/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.951946 dj-rest-auth-4.0.0/.circleci/
+-rw-r--r--   0 michael    (501) staff       (20)     1057 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/.circleci/config.yml
+-rw-r--r--   0 michael    (501) staff       (20)       45 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/.coveralls.yml
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.935868 dj-rest-auth-4.0.0/.github/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.953305 dj-rest-auth-4.0.0/.github/workflows/
+-rw-r--r--   0 michael    (501) staff       (20)      352 2020-08-17 05:29:18.000000 dj-rest-auth-4.0.0/.github/workflows/main.yml
+-rw-r--r--   0 michael    (501) staff       (20)      923 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/.github/workflows/stale.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1330 2020-11-17 22:42:53.000000 dj-rest-auth-4.0.0/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)       52 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/AUTHORS
+-rw-r--r--   0 michael    (501) staff       (20)     1102 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)       89 2020-03-01 01:49:31.000000 dj-rest-auth-4.0.0/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3458 2023-05-07 05:38:10.092425 dj-rest-auth-4.0.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     2815 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.954452 dj-rest-auth-4.0.0/demo/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.956159 dj-rest-auth-4.0.0/demo/demo/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/demo/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3782 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/demo/settings.py
+-rw-r--r--   0 michael    (501) staff       (20)     2313 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/demo/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)      385 2020-03-01 05:55:17.000000 dj-rest-auth-4.0.0/demo/demo/wsgi.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      247 2021-08-03 03:29:51.000000 dj-rest-auth-4.0.0/demo/manage.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.957790 dj-rest-auth-4.0.0/demo/react-spa/
+-rw-r--r--   0 michael    (501) staff       (20)      310 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     2884 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/README.md
+-rw-r--r--   0 michael    (501) staff       (20)      745 2020-03-28 16:41:49.000000 dj-rest-auth-4.0.0/demo/react-spa/package.json
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.962974 dj-rest-auth-4.0.0/demo/react-spa/public/
+-rw-r--r--   0 michael    (501) staff       (20)     3150 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/favicon.ico
+-rw-r--r--   0 michael    (501) staff       (20)     1721 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/index.html
+-rw-r--r--   0 michael    (501) staff       (20)     5347 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/logo192.png
+-rw-r--r--   0 michael    (501) staff       (20)     9664 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/logo512.png
+-rw-r--r--   0 michael    (501) staff       (20)      492 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/manifest.json
+-rw-r--r--   0 michael    (501) staff       (20)       67 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/robots.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.969612 dj-rest-auth-4.0.0/demo/react-spa/src/
+-rw-r--r--   0 michael    (501) staff       (20)      594 2020-03-28 18:49:16.000000 dj-rest-auth-4.0.0/demo/react-spa/src/App.css
+-rw-r--r--   0 michael    (501) staff       (20)     1770 2020-03-28 18:50:43.000000 dj-rest-auth-4.0.0/demo/react-spa/src/App.js
+-rw-r--r--   0 michael    (501) staff       (20)      280 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/App.test.js
+-rw-r--r--   0 michael    (501) staff       (20)      821 2020-03-28 18:49:40.000000 dj-rest-auth-4.0.0/demo/react-spa/src/index.css
+-rw-r--r--   0 michael    (501) staff       (20)      503 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/index.js
+-rw-r--r--   0 michael    (501) staff       (20)     2671 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/logo.svg
+-rw-r--r--   0 michael    (501) staff       (20)     5086 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/serviceWorker.js
+-rw-r--r--   0 michael    (501) staff       (20)      255 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/setupTests.js
+-rw-r--r--   0 michael    (501) staff       (20)      234 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/requirements.pip
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.979474 dj-rest-auth-4.0.0/demo/templates/
+-rw-r--r--   0 michael    (501) staff       (20)     4447 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/templates/base.html
+-rw-r--r--   0 michael    (501) staff       (20)      188 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/email_verification.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.986713 dj-rest-auth-4.0.0/demo/templates/fragments/
+-rw-r--r--   0 michael    (501) staff       (20)      652 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/email_verification_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      839 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/login_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      668 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/logout_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      908 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/password_change_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1489 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/password_reset_confirm_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      579 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/password_reset_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      578 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/templates/fragments/resend_email_verification_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1365 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/signup_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1344 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/user_details_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      253 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/home.html
+-rw-r--r--   0 michael    (501) staff       (20)      161 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/login.html
+-rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/logout.html
+-rw-r--r--   0 michael    (501) staff       (20)     1161 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/password_change.html
+-rw-r--r--   0 michael    (501) staff       (20)      179 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/password_reset.html
+-rw-r--r--   0 michael    (501) staff       (20)      724 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/password_reset_confirm.html
+-rw-r--r--   0 michael    (501) staff       (20)      202 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/templates/resend_email_verification.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.987344 dj-rest-auth-4.0.0/demo/templates/rest_framework/
+-rw-r--r--   0 michael    (501) staff       (20)     1754 2020-06-20 18:56:14.000000 dj-rest-auth-4.0.0/demo/templates/rest_framework/api.html
+-rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/signup.html
+-rw-r--r--   0 michael    (501) staff       (20)     1915 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/user_details.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.995046 dj-rest-auth-4.0.0/dj_rest_auth/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.0/dj_rest_auth/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.005155 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      152 2021-07-11 17:17:01.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      149 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/admin.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1467 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2070 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/forms.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     5531 2023-01-02 22:42:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1044 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    11794 2023-01-02 22:42:47.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2854 2021-07-11 17:17:03.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1012 2021-07-11 17:17:03.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1255 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     9589 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      354 2023-05-07 05:37:31.000000 dj-rest-auth-4.0.0/dj_rest_auth/__version__.py
+-rw-r--r--   0 michael    (501) staff       (20)       65 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.0/dj_rest_auth/admin.py
+-rw-r--r--   0 michael    (501) staff       (20)     3075 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/app_settings.py
+-rw-r--r--   0 michael    (501) staff       (20)     2785 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/forms.py
+-rw-r--r--   0 michael    (501) staff       (20)     6282 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/jwt_auth.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.945448 dj-rest-auth-4.0.0/dj_rest_auth/locale/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.938603 dj-rest-auth-4.0.0/dj_rest_auth/locale/ar/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.005908 dj-rest-auth-4.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3751 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.938960 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.011367 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:52:06.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!63502!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:54:59.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64462!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:55:51.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64600!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:56:43.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64760!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:05:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65418!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65616!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65791!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65995!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!69818!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2443 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3195 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.939300 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.015526 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65618!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65793!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65997!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!69820!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2230 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2983 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.939643 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.019198 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65620!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65795!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65999!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!69822!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2405 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3151 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.939964 dj-rest-auth-4.0.0/dj_rest_auth/locale/fa/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.019905 dj-rest-auth-4.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3514 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.940310 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.023426 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!65622!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!65797!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!66001!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!69824!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3755 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     5257 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.940653 dj-rest-auth-4.0.0/dj_rest_auth/locale/hr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.024511 dj-rest-auth-4.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3091 2021-03-18 00:03:01.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.940983 dj-rest-auth-4.0.0/dj_rest_auth/locale/id/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.025495 dj-rest-auth-4.0.0/dj_rest_auth/locale/id/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     4954 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.941315 dj-rest-auth-4.0.0/dj_rest_auth/locale/it/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.027153 dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3001 2020-05-09 22:17:42.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3904 2020-05-09 22:17:42.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.941645 dj-rest-auth-4.0.0/dj_rest_auth/locale/ja/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.028117 dj-rest-auth-4.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     5628 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.941964 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.032200 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!65624!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!65799!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!66003!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!69826!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2562 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3296 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.942627 dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.033849 dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2958 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3524 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.942985 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.039305 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!65626!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!65801!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!66005!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!69828!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2265 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2992 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.943328 dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.041155 dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2317 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3090 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.943653 dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.043501 dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2979 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3537 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.943969 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.047702 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!65629!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!65804!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!66008!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!69831!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2773 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3508 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.944284 dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.049628 dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2565 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3774 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.944595 dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.051876 dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2222 2020-04-27 03:53:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2920 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.944906 dj-rest-auth-4.0.0/dj_rest_auth/locale/uk/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.052642 dj-rest-auth-4.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3502 2021-03-18 00:03:01.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.945244 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.056466 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65632!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65807!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!66011!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!69834!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2243 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3019 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.945581 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.060414 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65634!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65809!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!66013!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!69836!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)      373 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2337 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0 michael    (501) staff       (20)      948 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/models.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.064051 dj-rest-auth-4.0.0/dj_rest_auth/registration/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.072013 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      165 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      811 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     8838 2023-01-02 22:42:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      747 2022-07-17 22:38:11.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     8336 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    10813 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)     1299 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     7732 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/views.py
+-rw-r--r--   0 michael    (501) staff       (20)    12700 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)     2990 2021-05-17 04:45:09.000000 dj-rest-auth-4.0.0/dj_rest_auth/social_serializers.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.078326 dj-rest-auth-4.0.0/dj_rest_auth/tests/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.084999 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      158 2021-07-11 17:17:01.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1793 2022-07-17 22:38:11.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     4196 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2461 2022-07-17 22:38:07.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    27867 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     7032 2022-07-17 23:28:09.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     9113 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     5299 2022-07-17 22:38:10.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2420 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/django_urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     4012 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/mixins.py
+-rw-r--r--   0 michael    (501) staff       (20)      140 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/requirements.pip
+-rw-r--r--   0 michael    (501) staff       (20)     2833 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/settings.py
+-rw-r--r--   0 michael    (501) staff       (20)    44032 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/test_api.py
+-rw-r--r--   0 michael    (501) staff       (20)     7157 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/test_serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)    13998 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/test_social.py
+-rw-r--r--   0 michael    (501) staff       (20)      289 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/test_utils.py
+-rw-r--r--   0 michael    (501) staff       (20)     4541 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     1031 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/utils.py
+-rw-r--r--   0 michael    (501) staff       (20)     1198 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)      541 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/utils.py
+-rw-r--r--   0 michael    (501) staff       (20)    10760 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/views.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.997817 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3458 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     8029 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2020-03-01 01:18:23.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/not-zip-safe
+-rw-r--r--   0 michael    (501) staff       (20)       85 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       13 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/top_level.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.091574 dj-rest-auth-4.0.0/docs/
+-rw-r--r--   0 michael    (501) staff       (20)     6786 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/docs/Makefile
+-rw-r--r--   0 michael    (501) staff       (20)     3219 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/docs/api_endpoints.rst
+-rw-r--r--   0 michael    (501) staff       (20)     8317 2020-05-09 22:29:21.000000 dj-rest-auth-4.0.0/docs/conf.py
+-rw-r--r--   0 michael    (501) staff       (20)     9026 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/docs/configuration.rst
+-rw-r--r--   0 michael    (501) staff       (20)      758 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/docs/demo.rst
+-rw-r--r--   0 michael    (501) staff       (20)      497 2020-05-30 06:34:32.000000 dj-rest-auth-4.0.0/docs/disclosure.rst
+-rw-r--r--   0 michael    (501) staff       (20)     3095 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/docs/faq.rst
+-rw-r--r--   0 michael    (501) staff       (20)      754 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/docs/index.rst
+-rw-r--r--   0 michael    (501) staff       (20)    11426 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/docs/installation.rst
+-rw-r--r--   0 michael    (501) staff       (20)     1301 2020-08-10 01:03:45.000000 dj-rest-auth-4.0.0/docs/introduction.rst
+-rw-r--r--   0 michael    (501) staff       (20)     6713 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/docs/make.bat
+-rw-r--r--   0 michael    (501) staff       (20)      657 2021-03-17 23:58:28.000000 dj-rest-auth-4.0.0/runtests.py
+-rw-r--r--   0 michael    (501) staff       (20)      474 2023-05-07 05:38:10.093057 dj-rest-auth-4.0.0/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1542 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/setup.py
+-rw-r--r--   0 michael    (501) staff       (20)     1135 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/tox.ini
```

### Comparing `dj-rest-auth-3.0.0/LICENSE` & `dj-rest-auth-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/README.md` & `dj-rest-auth-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/forms.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/forms.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/models.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/serializers.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/utils.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/__pycache__/views.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/app_settings.py` & `dj-rest-auth-4.0.0/dj_rest_auth/app_settings.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/forms.py` & `dj-rest-auth-4.0.0/dj_rest_auth/forms.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,30 @@
         filter_users_by_email,
         user_pk_to_url_str,
         user_username,
     )
     from allauth.utils import build_absolute_uri
 
 
+def default_url_generator(request, user, temp_key):
+    path = reverse(
+        'password_reset_confirm',
+        args=[user_pk_to_url_str(user), temp_key],
+    )
+
+    if api_settings.PASSWORD_RESET_USE_SITES_DOMAIN:
+        url = build_absolute_uri(None, path)
+    else:
+        url = build_absolute_uri(request, path)
+
+    url = url.replace('%3F', '?')
+
+    return url
+
+
 class AllAuthPasswordResetForm(DefaultPasswordResetForm):
     def clean_email(self):
         """
         Invalid email should not raise error, as this would leak users
         for unit test: test_password_reset_with_invalid_email
         """
         email = self.cleaned_data["email"]
@@ -40,25 +56,16 @@
             temp_key = token_generator.make_token(user)
 
             # save it to the password reset model
             # password_reset = PasswordReset(user=user, temp_key=temp_key)
             # password_reset.save()
 
             # send the password reset email
-            path = reverse(
-                'password_reset_confirm',
-                args=[user_pk_to_url_str(user), temp_key],
-            )
-
-            if api_settings.PASSWORD_RESET_USE_SITES_DOMAIN:
-                url = build_absolute_uri(None, path)
-            else:
-                url = build_absolute_uri(request, path)
-
-            url = url.replace("%3F", "?")
+            url_generator = kwargs.get('url_generator', default_url_generator)
+            url = url_generator(request, user, temp_key)
 
             context = {
                 'current_site': current_site,
                 'user': user,
                 'password_reset_url': url,
                 'request': request,
             }
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/jwt_auth.py` & `dj-rest-auth-4.0.0/dj_rest_auth/jwt_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,18 @@
 
     class RefreshViewWithCookieSupport(TokenRefreshView):
         serializer_class = CookieTokenRefreshSerializer
 
         def finalize_response(self, request, response, *args, **kwargs):
             if response.status_code == status.HTTP_200_OK and 'access' in response.data:
                 set_jwt_access_cookie(response, response.data['access'])
-                response.data['access_token_expiration'] = (timezone.now() + jwt_settings.ACCESS_TOKEN_LIFETIME)
+                response.data['access_expiration'] = (timezone.now() + jwt_settings.ACCESS_TOKEN_LIFETIME)
             if response.status_code == status.HTTP_200_OK and 'refresh' in response.data:
                 set_jwt_refresh_cookie(response, response.data['refresh'])
+                response.data['refresh_expiration'] = (timezone.now() + jwt_settings.REFRESH_TOKEN_LIFETIME)
             return super().finalize_response(request, response, *args, **kwargs)
     return RefreshViewWithCookieSupport
 
 
 class JWTCookieAuthentication(JWTAuthentication):
     """
     An authentication plugin that hopefully authenticates requests through a JSON web
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.po`

 * *Files 17% similar despite different names*

```diff
@@ -3,96 +3,93 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-12-22 11:37-0800\n"
-"PO-Revision-Date: 2017-02-14 13:27+0100\n"
-"Language: fr\n"
+"POT-Creation-Date: 2017-03-05 21:56-0800\n"
+"PO-Revision-Date: 2018-10-13 19:37+0300\n"
+"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "Last-Translator: \n"
 "Language-Team: \n"
-"X-Generator: Poedit 1.8.11\n"
+"X-Generator: Poedit 2.2\n"
 
-#: registration/serializers.py:53
+#: registration/serializers.py:67
 msgid "View is not defined, pass it as a context variable"
-msgstr "La “View” n’est pas définie, passez la en variable contextuelle"
+msgstr "“View” tanımlanmadı, “context” değişkeni olarak tanımla"
 
-#: registration/serializers.py:58
+#: registration/serializers.py:72
 msgid "Define adapter_class in view"
-msgstr "Définissez “adapter_class” dans la vue"
+msgstr "“view” içerisinde  “adapter_class” tanımla"
 
-#: registration/serializers.py:77
+#: registration/serializers.py:91
 msgid "Define callback_url in view"
-msgstr "Définissez “callback_url” dans la vue"
+msgstr "“view” içerisinde  “callback_url” tanımla"
 
-#: registration/serializers.py:81
+#: registration/serializers.py:95
 msgid "Define client_class in view"
-msgstr "Définissez “client_class” dans la vue"
+msgstr "“view” içerisinde  “client_class” tanımla"
 
-#: registration/serializers.py:102
+#: registration/serializers.py:116
 msgid "Incorrect input. access_token or code is required."
-msgstr "Paramètres incorrects. Il faut “access_token” ou “code”."
+msgstr "Geçersiz girdi. “access_token” veya “code” gerekli."
 
-#: registration/serializers.py:111
+#: registration/serializers.py:125
 msgid "Incorrect value"
-msgstr "Paramètre incorrect"
+msgstr "Geçersiz değer"
 
-#: registration/serializers.py:140
+#: registration/serializers.py:185
 msgid "A user is already registered with this e-mail address."
-msgstr "Un utilisateur existe déjà avec cette adresse email."
+msgstr "Bu e-posta adresi ile bir kullanıcı zaten kayıt olmuştu."
 
-#: registration/serializers.py:148
+#: registration/serializers.py:193
 msgid "The two password fields didn't match."
-msgstr "Les deux mots de passes ne sont pas les mêmes."
+msgstr "İki şifre alanı eşleşmiyor."
 
-#: registration/views.py:82
+#: registration/views.py:98
 msgid "ok"
-msgstr "Ok"
+msgstr "tamam"
 
-#: serializers.py:30
+#: serializers.py:33
 msgid "Must include \"email\" and \"password\"."
-msgstr "Doit inclure “email” et “password”."
+msgstr "\"email\" ve \"password\" içermelidir."
 
-#: serializers.py:41
+#: serializers.py:44
 msgid "Must include \"username\" and \"password\"."
-msgstr "Doit inclure “username” et “password”."
+msgstr "“username\" und \"password\" içermelidir."
 
-#: serializers.py:54
+#: serializers.py:57
 msgid "Must include either \"username\" or \"email\" and \"password\"."
-msgstr "Doit inclure un “username” ou “email”, et un “password”."
+msgstr "Ya ”username\" yada \"email\" ve \"password\" içermelidir."
 
-#: serializers.py:95
+#: serializers.py:98
 msgid "User account is disabled."
-msgstr "Le compte utilisateur est désactivé."
+msgstr "Kullanıcı hesap pasiftir."
 
-#: serializers.py:98
+#: serializers.py:101
 msgid "Unable to log in with provided credentials."
-msgstr "Connexion impossible avec les informations fournies."
+msgstr "Sağlanan kimlik bilgileri ile giriş yapılamıyor."
 
-#: serializers.py:107
+#: serializers.py:110
 msgid "E-mail is not verified."
-msgstr "L’adresse email n’a pas été vérifiée."
+msgstr "E-posta adresi doğrulanmadı."
 
-#: views.py:114
+#: views.py:127
 msgid "Successfully logged out."
-msgstr "Déconnexion effectuée avec succès."
+msgstr "Başarılı bir şekilde çıkış yapıldı."
 
-#: views.py:162
+#: views.py:175
 msgid "Password reset e-mail has been sent."
-msgstr "L’email de réinitialisation du mot de passe a été envoyé."
+msgstr "Şifre sıfırlama e-postası gönderildi."
 
-#: views.py:184
+#: views.py:201
 msgid "Password has been reset with the new password."
-msgstr "Le mot de passe a été réinitialisé."
+msgstr "Yeni şifre ile şifre sıfırlandı."
 
-#: views.py:202
+#: views.py:223
 msgid "New password has been saved."
-msgstr "Le nouveau mot de passe est sauvé."
-
-#~ msgid "Error"
-#~ msgstr "Fehler"
+msgstr "Yeni şifre kaydedildi."
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,104 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-03-05 21:56-0800\n"
-"PO-Revision-Date: 2018-10-13 19:37+0300\n"
-"Language: tr\n"
+"POT-Creation-Date: 2018-10-28 11:41+0800\n"
+"PO-Revision-Date: 2018-10-28 11:45+0806\n"
+"Last-Translator: b'  <admin@xx.com>'\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"Last-Translator: \n"
-"Language-Team: \n"
-"X-Generator: Poedit 2.2\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Translated-Using: django-rosetta 0.9.0\n"
 
 #: registration/serializers.py:67
 msgid "View is not defined, pass it as a context variable"
-msgstr "“View” tanımlanmadı, “context” değişkeni olarak tanımla"
+msgstr "View未定义，请通过context变量传入"
 
 #: registration/serializers.py:72
 msgid "Define adapter_class in view"
-msgstr "“view” içerisinde  “adapter_class” tanımla"
+msgstr "请在View中定义adapter_class"
 
 #: registration/serializers.py:91
 msgid "Define callback_url in view"
-msgstr "“view” içerisinde  “callback_url” tanımla"
+msgstr "请在view中定义callback_url"
 
 #: registration/serializers.py:95
 msgid "Define client_class in view"
-msgstr "“view” içerisinde  “client_class” tanımla"
+msgstr "请在view中定义client_class"
 
 #: registration/serializers.py:116
 msgid "Incorrect input. access_token or code is required."
-msgstr "Geçersiz girdi. “access_token” veya “code” gerekli."
+msgstr "输入错误。access_token或code是必填项。"
 
 #: registration/serializers.py:125
 msgid "Incorrect value"
-msgstr "Geçersiz değer"
+msgstr "错误的值"
+
+#: registration/serializers.py:139
+msgid "User is already registered with this e-mail address."
+msgstr "该邮箱地址已被注册。"
 
 #: registration/serializers.py:185
 msgid "A user is already registered with this e-mail address."
-msgstr "Bu e-posta adresi ile bir kullanıcı zaten kayıt olmuştu."
+msgstr "该邮箱地址已被注册。"
 
 #: registration/serializers.py:193
 msgid "The two password fields didn't match."
-msgstr "İki şifre alanı eşleşmiyor."
+msgstr "两次输入的密码不相同"
+
+#: registration/views.py:51
+msgid "Verification e-mail sent."
+msgstr "验证邮件已发送。"
 
 #: registration/views.py:98
 msgid "ok"
-msgstr "tamam"
+msgstr "好的"
 
 #: serializers.py:33
 msgid "Must include \"email\" and \"password\"."
-msgstr "\"email\" ve \"password\" içermelidir."
+msgstr "比如包含\"email\"和\"password\"。"
 
 #: serializers.py:44
 msgid "Must include \"username\" and \"password\"."
-msgstr "“username\" und \"password\" içermelidir."
+msgstr "比如包含\"username\"和\"password\"。"
 
 #: serializers.py:57
 msgid "Must include either \"username\" or \"email\" and \"password\"."
-msgstr "Ya ”username\" yada \"email\" ve \"password\" içermelidir."
+msgstr "比如包含\"username\"，\"email\"，\"password\"其中一个。"
 
 #: serializers.py:98
 msgid "User account is disabled."
-msgstr "Kullanıcı hesap pasiftir."
+msgstr "用户账号已被禁用。"
 
 #: serializers.py:101
 msgid "Unable to log in with provided credentials."
-msgstr "Sağlanan kimlik bilgileri ile giriş yapılamıyor."
+msgstr "无法使用提供的信息登录。"
 
 #: serializers.py:110
 msgid "E-mail is not verified."
-msgstr "E-posta adresi doğrulanmadı."
+msgstr "邮箱未验证。"
 
 #: views.py:127
 msgid "Successfully logged out."
-msgstr "Başarılı bir şekilde çıkış yapıldı."
+msgstr "已成功登出。"
 
 #: views.py:175
 msgid "Password reset e-mail has been sent."
-msgstr "Şifre sıfırlama e-postası gönderildi."
+msgstr "密码重置邮件已发送。"
 
 #: views.py:201
 msgid "Password has been reset with the new password."
-msgstr "Yeni şifre ile şifre sıfırlandı."
+msgstr "密码重置成功。"
 
 #: views.py:223
 msgid "New password has been saved."
-msgstr "Yeni şifre kaydedildi."
+msgstr "新密码已设置成功。"
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/models.py` & `dj-rest-auth-4.0.0/dj_rest_auth/models.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/registration/serializers.py` & `dj-rest-auth-4.0.0/dj_rest_auth/registration/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from allauth.socialaccount.providers.oauth2.client import OAuth2Error
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ValidationError as DjangoValidationError
 from django.http import HttpRequest, HttpResponseBadRequest
 from django.urls.exceptions import NoReverseMatch
 from django.utils.translation import gettext_lazy as _
 from requests.exceptions import HTTPError
 from rest_framework import serializers
@@ -126,15 +127,20 @@
                 adapter.access_token_url,
                 self.callback_url,
                 scope,
                 scope_delimiter=adapter.scope_delimiter,
                 headers=adapter.headers,
                 basic_auth=adapter.basic_auth,
             )
-            token = client.get_access_token(code)
+            try:
+                token = client.get_access_token(code)
+            except OAuth2Error as ex:
+                raise serializers.ValidationError(
+                    _('Failed to exchange code for access token')
+                ) from ex
             access_token = token['access_token']
             tokens_to_parse = {'access_token': access_token}
 
             # If available we add additional data to the dictionary
             for key in ['refresh_token', 'id_token', adapter.expires_in_key]:
                 if key in token:
                     tokens_to_parse[key] = token[key]
@@ -143,15 +149,15 @@
                 _('Incorrect input. access_token or code is required.'),
             )
 
         social_token = adapter.parse_token(tokens_to_parse)
         social_token.app = app
 
         try:
-            if adapter.provider_id == 'google':
+            if adapter.provider_id == 'google' and not code:
                 login = self.get_social_login(adapter, app, social_token, response={'id_token': token})
             else:
                 login = self.get_social_login(adapter, app, social_token, token)
             ret = complete_social_login(request, login)
         except HTTPError:
             raise serializers.ValidationError(_('Incorrect value'))
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/registration/urls.py` & `dj-rest-auth-4.0.0/dj_rest_auth/registration/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/registration/views.py` & `dj-rest-auth-4.0.0/dj_rest_auth/registration/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         if allauth_account_settings.EMAIL_VERIFICATION == \
                 allauth_account_settings.EmailVerificationMethod.MANDATORY:
             return {'detail': _('Verification e-mail sent.')}
 
         if api_settings.USE_JWT:
             data = {
                 'user': user,
-                'access_token': self.access_token,
-                'refresh_token': self.refresh_token,
+                'access': self.access_token,
+                'refresh': self.refresh_token,
             }
             return api_settings.JWT_SERIALIZER(data, context=self.get_serializer_context()).data
         elif api_settings.SESSION_LOGIN:
             return None
         else:
             return api_settings.TOKEN_SERIALIZER(user.auth_token, context=self.get_serializer_context()).data
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/serializers.py` & `dj-rest-auth-4.0.0/dj_rest_auth/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     @staticmethod
     def validate_auth_user_status(user):
         if not user.is_active:
             msg = _('User account is disabled.')
             raise exceptions.ValidationError(msg)
 
     @staticmethod
-    def validate_email_verification_status(user):
+    def validate_email_verification_status(user, email=None):
         from allauth.account import app_settings as allauth_account_settings
         if (
             allauth_account_settings.EMAIL_VERIFICATION == allauth_account_settings.EmailVerificationMethod.MANDATORY
             and not user.emailaddress_set.filter(email=user.email, verified=True).exists()
         ):
             raise serializers.ValidationError(_('E-mail is not verified.'))
 
@@ -126,15 +126,15 @@
             raise exceptions.ValidationError(msg)
 
         # Did we get back an active user?
         self.validate_auth_user_status(user)
 
         # If required, is the email verified?
         if 'dj_rest_auth.registration' in settings.INSTALLED_APPS:
-            self.validate_email_verification_status(user)
+            self.validate_email_verification_status(user, email=email)
 
         attrs['user'] = user
         return attrs
 
 
 class TokenSerializer(serializers.ModelSerializer):
     """
@@ -181,16 +181,16 @@
         read_only_fields = ('email',)
 
 
 class JWTSerializer(serializers.Serializer):
     """
     Serializer for JWT authentication.
     """
-    access_token = serializers.CharField()
-    refresh_token = serializers.CharField()
+    access = serializers.CharField()
+    refresh = serializers.CharField()
     user = serializers.SerializerMethodField()
 
     def get_user(self, obj):
         """
         Required to allow using custom USER_DETAILS_SERIALIZER in
         JWTSerializer. Defining it here to avoid circular imports
         """
@@ -200,16 +200,16 @@
         return user_data
 
 
 class JWTSerializerWithExpiration(JWTSerializer):
     """
     Serializer for JWT authentication with expiration times.
     """
-    access_token_expiration = serializers.DateTimeField()
-    refresh_token_expiration = serializers.DateTimeField()
+    access_expiration = serializers.DateTimeField()
+    refresh_expiration = serializers.DateTimeField()
 
 
 class PasswordResetSerializer(serializers.Serializer):
     """
     Serializer for requesting a password reset e-mail.
     """
     email = serializers.EmailField()
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/social_serializers.py` & `dj-rest-auth-4.0.0/dj_rest_auth/social_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/django_urls.py` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/django_urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/mixins.py` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/settings.py` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/test_api.py` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,16 @@
         payload = {
             'username': self.USERNAME,
             'password': self.PASS,
         }
         get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
 
         self.post(self.login_url, data=payload, status_code=200)
-        self.assertEqual('access_token' in self.response.json.keys(), True)
-        self.token = self.response.json['access_token']
+        self.assertEqual('access' in self.response.json.keys(), True)
+        self.token = self.response.json['access']
 
     @modify_settings(INSTALLED_APPS={'remove': ['allauth', 'allauth.account']})
     def test_login_by_email(self):
         payload = {
             'email': self.EMAIL.lower(),
             'password': self.PASS,
         }
@@ -274,15 +274,15 @@
     def test_password_change_honors_password_validators(self):
         login_payload = {"username": self.USERNAME, "password": self.PASS}
         get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
         self.post(self.login_url, data=login_payload, status_code=200)
         self.token = self.response.json['key']
         new_password_payload = {"new_password1": 123, "new_password2": 123}
         self.post(self.password_change_url, data=new_password_payload, status_code=400)
-    
+
     @override_api_settings(OLD_PASSWORD_FIELD_ENABLED=True)
     def test_password_change_with_old_password(self):
         login_payload = {
             'username': self.USERNAME,
             'password': self.PASS,
         }
         get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
@@ -435,15 +435,15 @@
     def test_user_details_using_jwt(self):
         user = get_user_model().objects.create_user(self.USERNAME, self.EMAIL, self.PASS)
         payload = {
             'username': self.USERNAME,
             'password': self.PASS,
         }
         self.post(self.login_url, data=payload, status_code=200)
-        self.token = self.response.json['access_token']
+        self.token = self.response.json['access']
         self.get(self.user_url, status_code=200)
 
         self.patch(self.user_url, data=self.BASIC_USER_DATA, status_code=200)
         user = get_user_model().objects.get(pk=user.pk)
         self.assertEqual(user.email, self.response.json['email'])
 
     @override_api_settings(SESSION_LOGIN=False)
@@ -518,15 +518,15 @@
     @override_api_settings(USE_JWT=True)
     def test_registration_with_jwt(self):
         user_count = get_user_model().objects.all().count()
 
         self.post(self.register_url, data={}, status_code=400)
 
         result = self.post(self.register_url, data=self.REGISTRATION_DATA, status_code=201)
-        self.assertIn('access_token', result.data)
+        self.assertIn('access', result.data)
         self.assertEqual(get_user_model().objects.all().count(), user_count + 1)
 
         self._login()
         self._logout()
 
     @override_api_settings(SESSION_LOGIN=True)
     @override_api_settings(TOKEN_MODEL=None)
@@ -723,15 +723,15 @@
     def test_blacklisting_not_installed(self):
         payload = {
             'username': self.USERNAME,
             'password': self.PASS,
         }
         get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
         resp = self.post(self.login_url, data=payload, status_code=200)
-        token = resp.data['refresh_token']
+        token = resp.data['refresh']
         resp = self.post(self.logout_url, status=200, data={'refresh': token})
         self.assertEqual(resp.status_code, 200)
         self.assertEqual(
             resp.data['detail'],
             'Neither cookies or blacklist are enabled, so the token has not been deleted server side. '
             'Please make sure the token is deleted client side.',
         )
@@ -741,15 +741,15 @@
     def test_blacklisting(self):
         payload = {
             'username': self.USERNAME,
             'password': self.PASS,
         }
         get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
         resp = self.post(self.login_url, data=payload, status_code=200)
-        token = resp.data['refresh_token']
+        token = resp.data['refresh']
         # test refresh token not included in request data
         self.post(self.logout_url, status_code=401)
         # test token is invalid or expired
         self.post(self.logout_url, status_code=401, data={'refresh': '1'})
         # test successful logout
         self.post(self.logout_url, status_code=200, data={'refresh': token})
         # test token is blacklisted
@@ -772,16 +772,16 @@
         payload = {
             'username': self.USERNAME,
             'password': self.PASS,
         }
         get_user_model().objects.create_user(self.USERNAME, self.EMAIL, self.PASS)
 
         self.post(self.login_url, data=payload, status_code=200)
-        self.assertEqual('access_token' in self.response.json.keys(), True)
-        self.token = self.response.json['access_token']
+        self.assertEqual('access' in self.response.json.keys(), True)
+        self.token = self.response.json['access']
         claims = decode_jwt(self.token, settings.SECRET_KEY, algorithms='HS256')
         self.assertEquals(claims['user_id'], 1)
         self.assertEquals(claims['name'], 'person')
         self.assertEquals(claims['email'], 'person1@world.com')
 
     @override_api_settings(USE_JWT=True)
     @override_api_settings(JWT_AUTH_COOKIE='jwt-auth')
@@ -835,15 +835,15 @@
 
         resp = client.post(self.login_url, payload)
         self.assertTrue('jwt-auth' in list(client.cookies.keys()))
         self.assertEquals(resp.status_code, 200)
 
         ## TEST WITH JWT AUTH HEADER
         jwtclient = APIClient(enforce_csrf_checks=True)
-        token = resp.data['access_token']
+        token = resp.data['access']
         resp = jwtclient.get('/protected-view/', HTTP_AUTHORIZATION='Bearer ' + token)
         self.assertEquals(resp.status_code, 200)
         resp = jwtclient.post('/protected-view/', {}, HTTP_AUTHORIZATION='Bearer ' + token)
         self.assertEquals(resp.status_code, 200)
 
         ## TEST WITH COOKIES
         resp = client.get('/protected-view/')
@@ -881,15 +881,15 @@
         resp = client.post(self.login_url, payload)
         self.assertTrue('jwt-auth' in list(client.cookies.keys()))
         self.assertTrue('csrftoken' in list(client.cookies.keys()))
         self.assertEquals(resp.status_code, 200)
 
         ## TEST WITH JWT AUTH HEADER
         jwtclient = APIClient(enforce_csrf_checks=True)
-        token = resp.data['access_token']
+        token = resp.data['access']
         resp = jwtclient.get('/protected-view/')
         self.assertEquals(resp.status_code, 403)
         resp = jwtclient.get('/protected-view/', HTTP_AUTHORIZATION='Bearer ' + token)
         self.assertEquals(resp.status_code, 200)
         resp = jwtclient.post('/protected-view/', {})
         self.assertEquals(resp.status_code, 403)
         resp = jwtclient.post('/protected-view/', {}, HTTP_AUTHORIZATION='Bearer ' + token)
@@ -1013,16 +1013,16 @@
             'password': self.PASS,
         }
 
         # create user
         get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
 
         resp = self.post(self.login_url, data=payload, status_code=200)
-        self.assertIn('access_token_expiration', resp.data.keys())
-        self.assertIn('refresh_token_expiration', resp.data.keys())
+        self.assertIn('access_expiration', resp.data.keys())
+        self.assertIn('refresh_expiration', resp.data.keys())
 
     @override_api_settings(JWT_AUTH_RETURN_EXPIRATION=True)
     @override_api_settings(USE_JWT=True)
     @override_api_settings(JWT_AUTH_COOKIE='xxx')
     @override_settings(ACCOUNT_LOGOUT_ON_GET=True)
     @override_api_settings(JWT_AUTH_REFRESH_COOKIE='refresh-xxx')
     @override_api_settings(JWT_AUTH_REFRESH_COOKIE_PATH='/foo/bar')
@@ -1049,43 +1049,50 @@
         payload = {
             'username': self.USERNAME,
             'password': self.PASS,
         }
 
         get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
         resp = self.post(self.login_url, data=payload, status_code=200)
-        refresh = resp.data.get('refresh_token')
+        refresh = resp.data.get('refresh')
         refresh_resp = self.post(
             reverse('token_refresh'),
             data=dict(refresh=refresh),
             status_code=200,
         )
         self.assertIn('xxx', refresh_resp.cookies)
 
+        # Ensure access keys are provided in response
+        self.assertIn('access', refresh_resp.data)
+        self.assertIn('access_expiration', refresh_resp.data)
+
     @override_api_settings(USE_JWT=True)
     @override_api_settings(JWT_AUTH_HTTPONLY=False)
     def test_rotate_token_refresh_view(self):
         from rest_framework_simplejwt.settings import api_settings as jwt_settings
         jwt_settings.ROTATE_REFRESH_TOKENS = True
         payload = {
             'username': self.USERNAME,
             'password': self.PASS,
         }
 
         get_user_model().objects.create_user(self.USERNAME, '', self.PASS)
         resp = self.post(self.login_url, data=payload)
         self.assertEqual(resp.status_code, status.HTTP_200_OK)
 
-        refresh = resp.data.get('refresh_token', None)
+        refresh = resp.data.get('refresh', None)
         resp = self.post(
             reverse('token_refresh'),
             data=dict(refresh=refresh),
         )
         self.assertEqual(resp.status_code, status.HTTP_200_OK)
+
+        # Ensure access keys are provided in response
         self.assertIn('refresh', resp.data)
+        self.assertIn('refresh_expiration', resp.data)
 
     @override_api_settings(TOKEN_MODEL=None)
     @modify_settings(INSTALLED_APPS={'remove': ['rest_framework.authtoken']})
     def test_login_with_no_token_model(self):
         payload = {'username': self.USERNAME, 'password': self.PASS}
         # there is no users in db so it should throw error (400)
         resp = self.post(self.login_url, data=payload, status_code=status.HTTP_400_BAD_REQUEST)
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/test_serializers.py` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/test_social.py` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/test_social.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
 
         users_count = get_user_model().objects.all().count()
         payload = {
             'access_token': 'abc123',
         }
 
         self.post(self.fb_login_url, data=payload, status_code=200)
-        self.assertIn('access_token', self.response.json.keys())
+        self.assertIn('access', self.response.json.keys())
         self.assertIn('user', self.response.json.keys())
 
         self.assertEqual(get_user_model().objects.all().count(), users_count + 1)
 
 
 @override_settings(ROOT_URLCONF='tests.urls')
 class TestSocialConnectAuth(TestsMixin, TestCase):
```

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/urls.py` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/tests/utils.py` & `dj-rest-auth-4.0.0/dj_rest_auth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/urls.py` & `dj-rest-auth-4.0.0/dj_rest_auth/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/utils.py` & `dj-rest-auth-4.0.0/dj_rest_auth/utils.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-3.0.0/dj_rest_auth/views.py` & `dj-rest-auth-4.0.0/dj_rest_auth/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,26 +84,26 @@
             access_token_expiration = (timezone.now() + jwt_settings.ACCESS_TOKEN_LIFETIME)
             refresh_token_expiration = (timezone.now() + jwt_settings.REFRESH_TOKEN_LIFETIME)
             return_expiration_times = api_settings.JWT_AUTH_RETURN_EXPIRATION
             auth_httponly = api_settings.JWT_AUTH_HTTPONLY
 
             data = {
                 'user': self.user,
-                'access_token': self.access_token,
+                'access': self.access_token,
             }
 
             if not auth_httponly:
-                data['refresh_token'] = self.refresh_token
+                data['refresh'] = self.refresh_token
             else:
                 # Wasnt sure if the serializer needed this
-                data['refresh_token'] = ""
+                data['refresh'] = ""
 
             if return_expiration_times:
-                data['access_token_expiration'] = access_token_expiration
-                data['refresh_token_expiration'] = refresh_token_expiration
+                data['access_expiration'] = access_token_expiration
+                data['refresh_expiration'] = refresh_token_expiration
 
             serializer = serializer_class(
                 instance=data,
                 context=self.get_serializer_context(),
             )
         elif self.token:
             serializer = serializer_class(
```

### Comparing `dj-rest-auth-3.0.0/setup.py` & `dj-rest-auth-4.0.0/setup.py`

 * *Files identical despite different names*

