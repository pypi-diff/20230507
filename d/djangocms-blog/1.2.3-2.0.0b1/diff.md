# Comparing `tmp/djangocms-blog-1.2.3.tar.gz` & `tmp/djangocms-blog-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-blog-1.2.3.tar", last modified: Mon Dec 21 11:06:03 2020, max compression
+gzip compressed data, was "/srv/dev/apps/djangocms-blog/dist/.tmp-_3i33xqi/djangocms-blog-2.0.0b1.tar", last modified: Sun May  7 19:56:19 2023, max compression
```

## Comparing `djangocms-blog-1.2.3.tar` & `djangocms-blog-2.0.0b1.tar`

### file list

```diff
@@ -1,197 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.120410 djangocms-blog-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (116)      834 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5728 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)    10936 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1478 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      195 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    19445 2020-12-21 11:06:03.124410 djangocms-blog-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3376 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/
--rw-r--r--   0 runner    (1001) docker     (116)      149 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1015 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/addon.json
--rw-r--r--   0 runner    (1001) docker     (116)    21445 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/admin.py
--rw-r--r--   0 runner    (1001) docker     (116)      191 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/apps.py
--rw-r--r--   0 runner    (1001) docker     (116)     9366 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/cms_appconfig.py
--rw-r--r--   0 runner    (1001) docker     (116)     1221 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/cms_apps.py
--rw-r--r--   0 runner    (1001) docker     (116)     7219 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/cms_menus.py
--rw-r--r--   0 runner    (1001) docker     (116)     7515 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (116)     3494 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/cms_toolbars.py
--rw-r--r--   0 runner    (1001) docker     (116)     4260 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/cms_wizards.py
--rw-r--r--   0 runner    (1001) docker     (116)     6635 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/feeds.py
--rw-r--r--   0 runner    (1001) docker     (116)      152 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/fields.py
--rw-r--r--   0 runner    (1001) docker     (116)     6279 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/liveblog/
--rw-r--r--   0 runner    (1001) docker     (116)       70 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      197 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/apps.py
--rw-r--r--   0 runner    (1001) docker     (116)      912 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (116)      869 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/consumers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/liveblog/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)     2058 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)      397 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/migrations/0002_liveblog_title.py
--rw-r--r--   0 runner    (1001) docker     (116)      924 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/migrations/0003_auto_20160917_0123.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3916 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/models.py
--rw-r--r--   0 runner    (1001) docker     (116)      204 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.104410 djangocms-blog-1.2.3/djangocms_blog/liveblog/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.104410 djangocms-blog-1.2.3/djangocms_blog/liveblog/static/liveblog/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/liveblog/static/liveblog/js/
--rw-r--r--   0 runner    (1001) docker     (116)     1094 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/static/liveblog/js/liveblog.js
--rw-r--r--   0 runner    (1001) docker     (116)     3100 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/static/liveblog/js/reconnecting-websocket.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.104410 djangocms-blog-1.2.3/djangocms_blog/liveblog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.104410 djangocms-blog-1.2.3/djangocms_blog/liveblog/templates/liveblog/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/liveblog/templates/liveblog/includes/
--rw-r--r--   0 runner    (1001) docker     (116)      447 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/templates/liveblog/includes/post_detail.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/liveblog/templates/liveblog/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)      253 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/templates/liveblog/plugins/liveblog.html
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/liveblog/templates/liveblog/plugins/unpublished.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.104410 djangocms-blog-1.2.3/djangocms_blog/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     1823 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    13239 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.104410 djangocms-blog-1.2.3/djangocms_blog/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)    11399 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    16518 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.104410 djangocms-blog-1.2.3/djangocms_blog/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)      396 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    12461 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.104410 djangocms-blog-1.2.3/djangocms_blog/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     3012 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    13434 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     5418 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    13893 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     8355 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    15484 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)    11643 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    16423 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)    11970 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    17146 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/nb_NO/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     7867 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    14970 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/nb_NO/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)    10036 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    15927 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/pl_PL/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/pl_PL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)    11295 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    16351 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/pl_PL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     8139 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    15195 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)    14597 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    19870 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     6324 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    14458 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     4160 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    13800 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (116)     6952 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.116410 djangocms-blog-1.2.3/djangocms_blog/media/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3843 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/media/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.120410 djangocms-blog-1.2.3/djangocms_blog/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)    11682 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)      659 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0002_post_sites.py
--rw-r--r--   0 runner    (1001) docker     (116)      634 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0003_auto_20141201_2252.py
--rw-r--r--   0 runner    (1001) docker     (116)     1913 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0004_auto_20150108_1435.py
--rw-r--r--   0 runner    (1001) docker     (116)      777 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0005_auto_20150212_1118.py
--rw-r--r--   0 runner    (1001) docker     (116)      486 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0006_auto_20150214_1907.py
--rw-r--r--   0 runner    (1001) docker     (116)     8054 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0007_auto_20150719_0933.py
--rw-r--r--   0 runner    (1001) docker     (116)      487 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0008_auto_20150814_0831.py
--rw-r--r--   0 runner    (1001) docker     (116)     2270 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0009_latestpostsplugin_tags_new.py
--rw-r--r--   0 runner    (1001) docker     (116)     5867 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0010_auto_20150923_1151.py
--rw-r--r--   0 runner    (1001) docker     (116)     3170 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0011_auto_20151024_1809.py
--rw-r--r--   0 runner    (1001) docker     (116)      363 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0012_auto_20151220_1734.py
--rw-r--r--   0 runner    (1001) docker     (116)      514 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0013_auto_20160201_2235.py
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0014_auto_20160215_1331.py
--rw-r--r--   0 runner    (1001) docker     (116)      443 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0015_auto_20160408_1849.py
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0016_auto_20160502_1741.py
--rw-r--r--   0 runner    (1001) docker     (116)      280 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0017_thumbnail_move.py
--rw-r--r--   0 runner    (1001) docker     (116)     1453 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0018_thumbnail_move2.py
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0019_thumbnail_move3.py
--rw-r--r--   0 runner    (1001) docker     (116)     1098 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0020_thumbnail_move4.py
--rw-r--r--   0 runner    (1001) docker     (116)     2518 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0021_auto_20160823_2008.py
--rw-r--r--   0 runner    (1001) docker     (116)      524 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0021_post_liveblog.py
--rw-r--r--   0 runner    (1001) docker     (116)      469 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0022_auto_20160605_2305.py
--rw-r--r--   0 runner    (1001) docker     (116)      843 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0022_auto_20170304_1040.py
--rw-r--r--   0 runner    (1001) docker     (116)     1088 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0023_auto_20160626_1539.py
--rw-r--r--   0 runner    (1001) docker     (116)     1642 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0024_auto_20160706_1524.py
--rw-r--r--   0 runner    (1001) docker     (116)      679 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0025_auto_20160803_0858.py
--rw-r--r--   0 runner    (1001) docker     (116)      282 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0026_merge.py
--rw-r--r--   0 runner    (1001) docker     (116)      426 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0027_post_date_featured.py
--rw-r--r--   0 runner    (1001) docker     (116)      843 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0028_auto_20170304_1040.py
--rw-r--r--   0 runner    (1001) docker     (116)      450 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0029_post_related.py
--rw-r--r--   0 runner    (1001) docker     (116)      495 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0030_auto_20170509_1831.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0031_auto_20170610_1744.py
--rw-r--r--   0 runner    (1001) docker     (116)     1671 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0032_auto_20180109_0023.py
--rw-r--r--   0 runner    (1001) docker     (116)      422 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0033_auto_20180226_1410.py
--rw-r--r--   0 runner    (1001) docker     (116)      241 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0034_merge.py
--rw-r--r--   0 runner    (1001) docker     (116)      438 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0035_posttranslation_subtitle.py
--rw-r--r--   0 runner    (1001) docker     (116)      462 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0036_auto_20180913_1809.py
--rw-r--r--   0 runner    (1001) docker     (116)     2853 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0037_auto_20190806_0743.py
--rw-r--r--   0 runner    (1001) docker     (116)      730 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0038_post_media.py
--rw-r--r--   0 runner    (1001) docker     (116)     1023 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/0039_auto_20200331_2227.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22873 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     3192 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/search_indexes.py
--rw-r--r--   0 runner    (1001) docker     (116)    11942 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.120410 djangocms-blog-1.2.3/djangocms_blog/sitemaps/
--rw-r--r--   0 runner    (1001) docker     (116)     1780 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/sitemaps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/static/djangocms_blog/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.120410 djangocms-blog-1.2.3/djangocms_blog/static/djangocms_blog/css/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/static/djangocms_blog/css/djangocms_blog.css
--rw-r--r--   0 runner    (1001) docker     (116)      939 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/static/djangocms_blog/css/djangocms_blog_admin.css
--rw-r--r--   0 runner    (1001) docker     (116)      277 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/taggit_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.108410 djangocms-blog-1.2.3/djangocms_blog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.120410 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/
--rw-r--r--   0 runner    (1001) docker     (116)      703 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/base.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.120410 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/includes/
--rw-r--r--   0 runner    (1001) docker     (116)     1461 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/includes/blog_item.html
--rw-r--r--   0 runner    (1001) docker     (116)     1373 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/includes/blog_meta.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.120410 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)     1419 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/archive.html
--rw-r--r--   0 runner    (1001) docker     (116)      751 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/authors.html
--rw-r--r--   0 runner    (1001) docker     (116)      716 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/authors_posts.html
--rw-r--r--   0 runner    (1001) docker     (116)      790 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/categories.html
--rw-r--r--   0 runner    (1001) docker     (116)      392 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/latest_entries.html
--rw-r--r--   0 runner    (1001) docker     (116)      754 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/tags.html
--rw-r--r--   0 runner    (1001) docker     (116)       46 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/post_archive.html
--rw-r--r--   0 runner    (1001) docker     (116)     1906 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/post_detail.html
--rw-r--r--   0 runner    (1001) docker     (116)     1592 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/post_instant_article.html
--rw-r--r--   0 runner    (1001) docker     (116)     1803 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/post_list.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.120410 djangocms-blog-1.2.3/djangocms_blog/templatetags/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2531 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/templatetags/djangocms_blog.py
--rw-r--r--   0 runner    (1001) docker     (116)     1338 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)     7304 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/djangocms_blog/views.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-21 11:06:03.112410 djangocms-blog-1.2.3/djangocms_blog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    19445 2020-12-21 11:06:02.000000 djangocms-blog-1.2.3/djangocms_blog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6311 2020-12-21 11:06:03.000000 djangocms-blog-1.2.3/djangocms_blog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-21 11:06:02.000000 djangocms-blog-1.2.3/djangocms_blog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-21 11:05:56.000000 djangocms-blog-1.2.3/djangocms_blog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      356 2020-12-21 11:06:02.000000 djangocms-blog-1.2.3/djangocms_blog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2020-12-21 11:06:02.000000 djangocms-blog-1.2.3/djangocms_blog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      674 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     2239 2020-12-21 11:06:03.124410 djangocms-blog-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-21 11:05:34.000000 djangocms-blog-1.2.3/setup.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/
+-rw-rw-r--   0 yakky     (1000)     1004      834 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/AUTHORS.rst
+-rw-rw-r--   0 yakky     (1000)     1004     5728 2020-12-20 11:09:27.000000 djangocms-blog-2.0.0b1/CONTRIBUTING.rst
+-rw-rw-r--   0 yakky     (1000)     1004    10936 2020-12-21 11:05:34.000000 djangocms-blog-2.0.0b1/HISTORY.rst
+-rw-rw-r--   0 yakky     (1000)     1004     1478 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/LICENSE
+-rw-rw-r--   0 yakky     (1000)     1004      195 2020-11-01 15:46:03.000000 djangocms-blog-2.0.0b1/MANIFEST.in
+-rw-rw-r--   0 yakky     (1000)     1004    15071 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/PKG-INFO
+-rw-rw-r--   0 yakky     (1000)     1004     3100 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/README.rst
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/
+-rw-rw-r--   0 yakky     (1000)     1004       94 2023-05-07 19:55:07.000000 djangocms-blog-2.0.0b1/djangocms_blog/__init__.py
+-rw-rw-r--   0 yakky     (1000)     1004     1015 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/addon.json
+-rw-rw-r--   0 yakky     (1000)     1004    21344 2023-04-20 22:18:56.000000 djangocms-blog-2.0.0b1/djangocms_blog/admin.py
+-rw-rw-r--   0 yakky     (1000)     1004      191 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/apps.py
+-rw-rw-r--   0 yakky     (1000)     1004     9366 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/cms_appconfig.py
+-rw-rw-r--   0 yakky     (1000)     1004     1221 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/cms_apps.py
+-rw-rw-r--   0 yakky     (1000)     1004     7219 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/cms_menus.py
+-rw-rw-r--   0 yakky     (1000)     1004     7515 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/cms_plugins.py
+-rw-rw-r--   0 yakky     (1000)     1004     3757 2023-04-20 22:18:56.000000 djangocms-blog-2.0.0b1/djangocms_blog/cms_toolbars.py
+-rw-rw-r--   0 yakky     (1000)     1004     4280 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/cms_wizards.py
+-rw-rw-r--   0 yakky     (1000)     1004     6691 2023-04-20 22:18:56.000000 djangocms-blog-2.0.0b1/djangocms_blog/feeds.py
+-rw-rw-r--   0 yakky     (1000)     1004      211 2023-04-20 21:51:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/fields.py
+-rw-rw-r--   0 yakky     (1000)     1004     6279 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/forms.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/
+-rw-rw-r--   0 yakky     (1000)     1004        0 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/__init__.py
+-rw-rw-r--   0 yakky     (1000)     1004      197 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/apps.py
+-rw-rw-r--   0 yakky     (1000)     1004      895 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/cms_plugins.py
+-rw-rw-r--   0 yakky     (1000)     1004      966 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/consumers.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/migrations/
+-rw-rw-r--   0 yakky     (1000)     1004     2057 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/migrations/0001_initial.py
+-rw-rw-r--   0 yakky     (1000)     1004      396 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/migrations/0002_liveblog_title.py
+-rw-rw-r--   0 yakky     (1000)     1004      923 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/migrations/0003_auto_20160917_0123.py
+-rw-rw-r--   0 yakky     (1000)     1004        0 2020-04-04 11:11:04.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/migrations/__init__.py
+-rw-rw-r--   0 yakky     (1000)     1004     3942 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/models.py
+-rw-rw-r--   0 yakky     (1000)     1004      214 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/routing.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/static/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/static/liveblog/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/static/liveblog/js/
+-rw-rw-r--   0 yakky     (1000)     1004     1094 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/static/liveblog/js/liveblog.js
+-rw-rw-r--   0 yakky     (1000)     1004     3100 2020-04-04 11:11:04.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/static/liveblog/js/reconnecting-websocket.min.js
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/templates/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/templates/liveblog/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/templates/liveblog/includes/
+-rw-rw-r--   0 yakky     (1000)     1004      447 2020-04-04 11:11:04.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/templates/liveblog/includes/post_detail.html
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/templates/liveblog/plugins/
+-rw-rw-r--   0 yakky     (1000)     1004      253 2020-04-04 11:11:04.000000 djangocms-blog-2.0.0b1/djangocms_blog/liveblog/templates/liveblog/plugins/liveblog.html
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/ar/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004     1823 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    13239 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/ar/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/de/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004    11399 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    16518 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/en/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004      396 2020-12-21 08:34:03.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    12461 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/en/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/es/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004     3012 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    13434 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/es/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/et/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004     5418 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    13893 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/et/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/fr/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004     8355 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    15484 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/fr/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/it/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004    11643 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    16423 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/it/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/lt/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004    11970 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    17146 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/lt/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/nb_NO/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/nb_NO/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004     7867 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    14970 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/nb_NO/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/nl/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004    10036 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    15927 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/nl/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/pl_PL/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/pl_PL/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004    11295 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    16351 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/pl_PL/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/pt_BR/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004     8139 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    15195 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/ru/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004    14597 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    19870 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/ru/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/sl/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004     6324 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    14458 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/sl/LC_MESSAGES/django.po
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/tr/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000)     1004     4160 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000)     1004    13800 2020-12-21 10:59:34.000000 djangocms-blog-2.0.0b1/djangocms_blog/locale/tr/LC_MESSAGES/django.po
+-rw-rw-r--   0 yakky     (1000)     1004     7231 2023-04-20 22:18:56.000000 djangocms-blog-2.0.0b1/djangocms_blog/managers.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/media/
+-rw-rw-r--   0 yakky     (1000)     1004        0 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/media/__init__.py
+-rw-rw-r--   0 yakky     (1000)     1004     3843 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/media/base.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/
+-rw-rw-r--   0 yakky     (1000)     1004    11693 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0001_initial.py
+-rw-rw-r--   0 yakky     (1000)     1004      678 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0002_post_sites.py
+-rw-rw-r--   0 yakky     (1000)     1004      652 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0003_auto_20141201_2252.py
+-rw-rw-r--   0 yakky     (1000)     1004     1912 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0004_auto_20150108_1435.py
+-rw-rw-r--   0 yakky     (1000)     1004      776 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0005_auto_20150212_1118.py
+-rw-rw-r--   0 yakky     (1000)     1004      477 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0006_auto_20150214_1907.py
+-rw-rw-r--   0 yakky     (1000)     1004     8053 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0007_auto_20150719_0933.py
+-rw-rw-r--   0 yakky     (1000)     1004      478 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0008_auto_20150814_0831.py
+-rw-rw-r--   0 yakky     (1000)     1004     2255 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0009_latestpostsplugin_tags_new.py
+-rw-rw-r--   0 yakky     (1000)     1004     5897 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0010_auto_20150923_1151.py
+-rw-rw-r--   0 yakky     (1000)     1004     3169 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0011_auto_20151024_1809.py
+-rw-rw-r--   0 yakky     (1000)     1004      354 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0012_auto_20151220_1734.py
+-rw-rw-r--   0 yakky     (1000)     1004      513 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0013_auto_20160201_2235.py
+-rw-rw-r--   0 yakky     (1000)     1004     1686 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0014_auto_20160215_1331.py
+-rw-rw-r--   0 yakky     (1000)     1004      442 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0015_auto_20160408_1849.py
+-rw-rw-r--   0 yakky     (1000)     1004      586 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0016_auto_20160502_1741.py
+-rw-rw-r--   0 yakky     (1000)     1004      220 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0017_thumbnail_move.py
+-rw-rw-r--   0 yakky     (1000)     1004     1452 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0018_thumbnail_move2.py
+-rw-rw-r--   0 yakky     (1000)     1004     1203 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0019_thumbnail_move3.py
+-rw-rw-r--   0 yakky     (1000)     1004     1089 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0020_thumbnail_move4.py
+-rw-rw-r--   0 yakky     (1000)     1004     2517 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0021_auto_20160823_2008.py
+-rw-rw-r--   0 yakky     (1000)     1004      527 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0021_post_liveblog.py
+-rw-rw-r--   0 yakky     (1000)     1004      435 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0022_auto_20160605_2305.py
+-rw-rw-r--   0 yakky     (1000)     1004      843 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0022_auto_20170304_1040.py
+-rw-rw-r--   0 yakky     (1000)     1004     1087 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0023_auto_20160626_1539.py
+-rw-rw-r--   0 yakky     (1000)     1004     1641 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0024_auto_20160706_1524.py
+-rw-rw-r--   0 yakky     (1000)     1004      678 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0025_auto_20160803_0858.py
+-rw-rw-r--   0 yakky     (1000)     1004      281 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0026_merge.py
+-rw-rw-r--   0 yakky     (1000)     1004      425 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0027_post_date_featured.py
+-rw-rw-r--   0 yakky     (1000)     1004      843 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0028_auto_20170304_1040.py
+-rw-rw-r--   0 yakky     (1000)     1004      449 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0029_post_related.py
+-rw-rw-r--   0 yakky     (1000)     1004      494 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0030_auto_20170509_1831.py
+-rw-rw-r--   0 yakky     (1000)     1004      594 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0031_auto_20170610_1744.py
+-rw-rw-r--   0 yakky     (1000)     1004     1670 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0032_auto_20180109_0023.py
+-rw-rw-r--   0 yakky     (1000)     1004      421 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0033_auto_20180226_1410.py
+-rw-rw-r--   0 yakky     (1000)     1004      232 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0034_merge.py
+-rw-rw-r--   0 yakky     (1000)     1004      437 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0035_posttranslation_subtitle.py
+-rw-rw-r--   0 yakky     (1000)     1004      461 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0036_auto_20180913_1809.py
+-rw-rw-r--   0 yakky     (1000)     1004     2852 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0037_auto_20190806_0743.py
+-rw-rw-r--   0 yakky     (1000)     1004      729 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0038_post_media.py
+-rw-rw-r--   0 yakky     (1000)     1004     1022 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0039_auto_20200331_2227.py
+-rw-rw-r--   0 yakky     (1000)     1004      432 2023-04-20 22:18:56.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/0040_post_include_in_rss.py
+-rw-rw-r--   0 yakky     (1000)     1004        0 2020-04-04 11:11:04.000000 djangocms-blog-2.0.0b1/djangocms_blog/migrations/__init__.py
+-rw-rw-r--   0 yakky     (1000)     1004    22976 2023-04-20 22:18:56.000000 djangocms-blog-2.0.0b1/djangocms_blog/models.py
+-rw-rw-r--   0 yakky     (1000)     1004    12043 2023-04-20 21:51:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/settings.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/sitemaps/
+-rw-rw-r--   0 yakky     (1000)     1004     1780 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/sitemaps/__init__.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/static/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/static/djangocms_blog/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/static/djangocms_blog/css/
+-rw-rw-r--   0 yakky     (1000)     1004        0 2020-04-04 11:11:04.000000 djangocms-blog-2.0.0b1/djangocms_blog/static/djangocms_blog/css/djangocms_blog.css
+-rw-rw-r--   0 yakky     (1000)     1004      939 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/static/djangocms_blog/css/djangocms_blog_admin.css
+-rw-rw-r--   0 yakky     (1000)     1004      252 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/djangocms_blog/taggit_urls.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/
+-rw-rw-r--   0 yakky     (1000)     1004      703 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/base.html
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/includes/
+-rw-rw-r--   0 yakky     (1000)     1004     1461 2020-05-04 19:57:52.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/includes/blog_item.html
+-rw-rw-r--   0 yakky     (1000)     1004     1433 2023-05-07 19:52:35.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/includes/blog_meta.html
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/
+-rw-rw-r--   0 yakky     (1000)     1004     1419 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/archive.html
+-rw-rw-r--   0 yakky     (1000)     1004      751 2020-05-04 20:15:49.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/authors.html
+-rw-rw-r--   0 yakky     (1000)     1004      716 2020-05-04 20:15:49.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/authors_posts.html
+-rw-rw-r--   0 yakky     (1000)     1004      790 2020-04-04 11:11:04.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/categories.html
+-rw-rw-r--   0 yakky     (1000)     1004      392 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/latest_entries.html
+-rw-rw-r--   0 yakky     (1000)     1004      754 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/tags.html
+-rw-rw-r--   0 yakky     (1000)     1004       46 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/post_archive.html
+-rw-rw-r--   0 yakky     (1000)     1004     1906 2020-05-04 19:57:52.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/post_detail.html
+-rw-rw-r--   0 yakky     (1000)     1004     1592 2020-05-04 19:57:52.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/post_instant_article.html
+-rw-rw-r--   0 yakky     (1000)     1004     1803 2020-04-04 11:11:04.000000 djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/post_list.html
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog/templatetags/
+-rw-rw-r--   0 yakky     (1000)     1004        0 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/templatetags/__init__.py
+-rw-rw-r--   0 yakky     (1000)     1004     2531 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/templatetags/djangocms_blog.py
+-rw-rw-r--   0 yakky     (1000)     1004     1338 2020-12-20 11:09:27.000000 djangocms-blog-2.0.0b1/djangocms_blog/urls.py
+-rw-rw-r--   0 yakky     (1000)     1004     7304 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/djangocms_blog/views.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog.egg-info/
+-rw-rw-r--   0 yakky     (1000)     1004    15071 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog.egg-info/PKG-INFO
+-rw-rw-r--   0 yakky     (1000)     1004     6524 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog.egg-info/SOURCES.txt
+-rw-rw-r--   0 yakky     (1000)     1004        1 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog.egg-info/dependency_links.txt
+-rw-rw-r--   0 yakky     (1000)     1004        1 2023-04-20 22:02:19.000000 djangocms-blog-2.0.0b1/djangocms_blog.egg-info/not-zip-safe
+-rw-rw-r--   0 yakky     (1000)     1004      332 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog.egg-info/requires.txt
+-rw-rw-r--   0 yakky     (1000)     1004       15 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/djangocms_blog.egg-info/top_level.txt
+-rw-rw-r--   0 yakky     (1000)     1004      984 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/pyproject.toml
+-rw-rw-r--   0 yakky     (1000)     1004     1759 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/setup.cfg
+-rw-rw-r--   0 yakky     (1000)     1004       38 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/setup.py
+drwxrwsr-x   0 yakky     (1000)     1004        0 2023-05-07 19:56:19.000000 djangocms-blog-2.0.0b1/tests/
+-rw-rw-r--   0 yakky     (1000)     1004     4198 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/tests/test_extension.py
+-rw-rw-r--   0 yakky     (1000)     1004     3149 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/tests/test_indexing.py
+-rw-rw-r--   0 yakky     (1000)     1004     7950 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/tests/test_liveblog.py
+-rw-rw-r--   0 yakky     (1000)     1004     3823 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/tests/test_media.py
+-rw-rw-r--   0 yakky     (1000)     1004    12468 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/tests/test_menu.py
+-rw-rw-r--   0 yakky     (1000)     1004    65701 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/tests/test_models.py
+-rw-rw-r--   0 yakky     (1000)     1004     1829 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/tests/test_namespace.py
+-rw-rw-r--   0 yakky     (1000)     1004    17671 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/tests/test_plugins.py
+-rw-rw-r--   0 yakky     (1000)     1004     2607 2023-04-20 21:20:15.000000 djangocms-blog-2.0.0b1/tests/test_setup.py
+-rw-rw-r--   0 yakky     (1000)     1004     2847 2023-04-20 22:18:56.000000 djangocms-blog-2.0.0b1/tests/test_toolbar.py
+-rw-rw-r--   0 yakky     (1000)     1004    23540 2023-04-20 22:18:56.000000 djangocms-blog-2.0.0b1/tests/test_views.py
+-rw-rw-r--   0 yakky     (1000)     1004     7667 2020-11-14 18:33:53.000000 djangocms-blog-2.0.0b1/tests/test_wizards.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `djangocms-blog-1.2.3/AUTHORS.rst` & `djangocms-blog-2.0.0b1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/CONTRIBUTING.rst` & `djangocms-blog-2.0.0b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/HISTORY.rst` & `djangocms-blog-2.0.0b1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/LICENSE` & `djangocms-blog-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/README.rst` & `djangocms-blog-2.0.0b1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,19 @@
 
 |Gitter| |PyPiVersion| |PyVersion| |GAStatus| |TestCoverage| |CodeClimate| |License|
 
 django CMS blog application - Support for multilingual posts, placeholders, social network meta tags and configurable apphooks.
 
 Supported Django versions:
 
-* Django 2.2, 3.0, 3.1
+* Django 3.2 - 4.2
 
 Supported django CMS versions:
 
-* django CMS 3.7, 3.8+
-
-.. warning:: For Django<2.2, django CMS<3.7 versions support, use djangocms-blog 1.1x.
-
-.. warning:: Version 1.2 introduce a breaking change for customized ``BLOG_PERMALINK_URLS``.
-             Check the `permalinks`_ documentation for update information.
+* django CMS 3.9 - 3.11+
 
 ************
 Installation
 ************
 
 See `installation documentation`_
 
@@ -41,15 +36,14 @@
 * Per-Apphook configuration
 * Configurable permalinks
 * Configurable django CMS menu
 * Per-Apphook templates set
 * Auto Apphook setup
 * Django sitemap framework
 * django CMS Wizard integration
-* Haystack index
 * Desktop notifications
 * Liveblog
 
 *****************************
 Known djangocms-blog websites
 *****************************
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/addon.json` & `djangocms-blog-2.0.0b1/djangocms_blog/addon.json`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/admin.py` & `djangocms-blog-2.0.0b1/djangocms_blog/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             return queryset
         except Site.DoesNotExist as e:  # pragma: no cover
             raise admin.options.IncorrectLookupParameters(e)
         except ValidationError as e:  # pragma: no cover
             raise admin.options.IncorrectLookupParameters(e)
 
 
+@admin.register(BlogCategory)
 class BlogCategoryAdmin(ModelAppHookConfig, TranslatableAdmin):
     form = CategoryAdminForm
     list_display = [
         "name",
         "parent",
         "app_config",
         "all_languages_column",
@@ -100,14 +101,15 @@
             return {}
         return {"slug": ("name",)}
 
     class Media:
         css = {"all": ("{}djangocms_blog/css/{}".format(settings.STATIC_URL, "djangocms_blog_admin.css"),)}
 
 
+@admin.register(Post)
 class PostAdmin(PlaceholderAdminMixin, FrontendEditableAdminMixin, ModelAppHookConfig, TranslatableAdmin):
     form = PostAdminForm
     list_display = ["title", "author", "date_published", "app_config", "all_languages_column", "date_published_end"]
     search_fields = ("translations__title",)
     date_hierarchy = "date_published"
     raw_id_fields = ["author"]
     frontend_editable_fields = ("title", "abstract", "post_text")
@@ -118,15 +120,15 @@
         "enable_comments",
         "disable_comments",
     ]
     inlines = []
     if apps.is_installed("djangocms_blog.liveblog"):
         actions += ["enable_liveblog", "disable_liveblog"]
     _fieldsets = [
-        (None, {"fields": ["title", "subtitle", "slug", "publish", ["categories", "app_config"]]}),
+        (None, {"fields": ["title", "subtitle", "slug", "publish", "include_in_rss", ["categories", "app_config"]]}),
         # left empty for sites, author and related fields
         (None, {"fields": [[]]}),
         (
             _("Info"),
             {
                 "fields": ["tags", ["date_published", "date_published_end", "date_featured"], ["enable_comments"]],
                 "classes": ("collapse",),
@@ -163,14 +165,15 @@
     an optional third value if the target "fields" has subgroups.
     """
 
     app_config_values = {"default_published": "publish"}
     _sites = None
 
     # Bulk actions for post admin
+    @admin.action(description=_("Publish selection"))
     def make_published(self, request, queryset):
         """
         Bulk action to mark selected posts as published.
         If the date_published field is empty the current time is saved as date_published.
         queryset must not be empty (ensured by django CMS).
         """
         cnt1 = queryset.filter(
@@ -184,85 +187,84 @@
         messages.add_message(
             request,
             messages.INFO,
             __("%(updates)d entry published.", "%(updates)d entries published.", cnt1 + cnt2)
             % {"updates": cnt1 + cnt2},
         )
 
+    @admin.action(description=_("Unpublish selection"))
     def make_unpublished(self, request, queryset):
         """
         Bulk action to mark selected posts as unpublished.
         queryset must not be empty (ensured by django CMS).
         """
         updates = queryset.filter(publish=True).update(publish=False)
         messages.add_message(
             request,
             messages.INFO,
             __("%(updates)d entry unpublished.", "%(updates)d entries unpublished.", updates) % {"updates": updates},
         )
 
+    @admin.action(description=_("Enable comments for selection"))
     def enable_comments(self, request, queryset):
         """
         Bulk action to enable comments for selected posts.
         queryset must not be empty (ensured by django CMS).
         """
         updates = queryset.filter(enable_comments=False).update(enable_comments=True)
         messages.add_message(
             request,
             messages.INFO,
             __("Comments for %(updates)d entry enabled.", "Comments for %(updates)d entries enabled", updates)
             % {"updates": updates},
         )
 
+    @admin.action(description=_("Disable comments for selection "))
     def disable_comments(self, request, queryset):
         """
         Bulk action to disable comments for selected posts.
         queryset must not be empty (ensured by django CMS).
         """
         updates = queryset.filter(enable_comments=True).update(enable_comments=False)
         messages.add_message(
             request,
             messages.INFO,
             __("Comments for %(updates)d entry disabled.", "Comments for %(updates)d entries disabled.", updates)
             % {"updates": updates},
         )
 
+    @admin.action(description=_("Enable liveblog for selection"))
     def enable_liveblog(self, request, queryset):
         """
         Bulk action to enable comments for selected posts.
         queryset must not be empty (ensured by django CMS).
         """
         updates = queryset.filter(enable_liveblog=False).update(enable_liveblog=True)
         messages.add_message(
             request,
             messages.INFO,
             __("Liveblog for %(updates)d entry enabled.", "Liveblog for %(updates)d entries enabled.", updates)
             % {"updates": updates},
         )
 
+    @admin.action(description=_("Disable liveblog for selection "))
     def disable_liveblog(self, request, queryset):
         """
         Bulk action to disable comments for selected posts.
         queryset must not be empty (ensured by django CMS).
         """
         updates = queryset.filter(enable_liveblog=True).update(enable_liveblog=False)
         messages.add_message(
             request,
             messages.INFO,
             __("Liveblog for %(updates)d entry enabled.", "Liveblog for %(updates)d entries enabled.")
             % {"updates": updates},
         )
 
     # Make bulk action menu entries localizable
-    make_published.short_description = _("Publish selection")
-    make_unpublished.short_description = _("Unpublish selection")
-    enable_comments.short_description = _("Enable comments for selection")
-    disable_comments.short_description = _("Disable comments for selection ")
-    enable_liveblog.short_description = _("Enable liveblog for selection")
-    disable_liveblog.short_description = _("Disable liveblog for selection ")
 
     def get_list_filter(self, request):
         filters = ["app_config", "publish", "date_published"]
         if get_setting("MULTISITE"):
             filters.append(SiteListFilter)
         try:
             from taggit_helpers.admin import TaggitListFilter
@@ -315,15 +317,15 @@
         try:
             post = Post.objects.get(pk=int(pk))
             post.publish = True
             post.save()
             return HttpResponseRedirect(post.get_absolute_url(language))
         except Exception:
             try:
-                return HttpResponseRedirect(request.META["HTTP_REFERER"])
+                return HttpResponseRedirect(request.headers["referer"])
             except KeyError:
                 return HttpResponseRedirect(reverse("djangocms_blog:posts-latest"))
 
     def has_restricted_sites(self, request):
         """
         Whether the current user has permission on one site only
 
@@ -449,14 +451,15 @@
                 form.instance.sites.add(*self.get_restricted_sites(request).all().values_list("pk", flat=True))
         super().save_related(request, form, formsets, change)
 
     class Media:
         css = {"all": ("{}djangocms_blog/css/{}".format(settings.STATIC_URL, "djangocms_blog_admin.css"),)}
 
 
+@admin.register(BlogConfig)
 class BlogConfigAdmin(BaseAppHookConfig, TranslatableAdmin):
     @property
     def declared_fieldsets(self):
         return self.get_fieldsets(None)
 
     def get_fieldsets(self, request, obj=None):
         """
@@ -547,12 +550,7 @@
         Clear menu cache when changing menu structure
         """
         if "config.menu_structure" in form.changed_data:
             from menus.menu_pool import menu_pool
 
             menu_pool.clear(all=True)
         return super().save_model(request, obj, form, change)
-
-
-admin.site.register(BlogCategory, BlogCategoryAdmin)
-admin.site.register(Post, PostAdmin)
-admin.site.register(BlogConfig, BlogConfigAdmin)
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/cms_appconfig.py` & `djangocms-blog-2.0.0b1/djangocms_blog/cms_appconfig.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/cms_apps.py` & `djangocms-blog-2.0.0b1/djangocms_blog/cms_apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/cms_menus.py` & `djangocms-blog-2.0.0b1/djangocms_blog/cms_menus.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/cms_plugins.py` & `djangocms-blog-2.0.0b1/djangocms_blog/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/cms_toolbars.py` & `djangocms-blog-2.0.0b1/djangocms_blog/cms_toolbars.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,21 @@
             not self.is_current_app and not get_setting("ENABLE_THROUGH_TOOLBAR_MENU")
         ) or not self.request.user.has_perm("djangocms_blog.add_post"):
             return  # pragma: no cover
         admin_menu = self.toolbar.get_or_create_menu("djangocms_blog", _("Blog"))
         with override(self.current_lang):
             url = reverse("admin:djangocms_blog_post_changelist")
             admin_menu.add_modal_item(_("Post list"), url=url)
+
+            url = reverse("admin:djangocms_blog_blogcategory_changelist")
+            admin_menu.add_modal_item(_("Category list"), url=url)
+
+            url = reverse("admin:taggit_tag_changelist")
+            admin_menu.add_modal_item(_("Tag list"), url=url)
+
             url = reverse("admin:djangocms_blog_post_add")
             admin_menu.add_modal_item(_("Add post"), url=url)
             current_config = getattr(self.request, get_setting("CURRENT_NAMESPACE"), None)
             if current_config:
                 url = reverse("admin:djangocms_blog_blogconfig_change", args=(current_config.pk,))
                 admin_menu.add_modal_item(_("Edit configuration"), url=url)
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/cms_wizards.py` & `djangocms-blog-2.0.0b1/djangocms_blog/cms_wizards.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,11 +111,12 @@
     try:
         wizard_pool.register(post_wizard)
     except AlreadyRegisteredException:  # pragma: no cover
         if settings.DEBUG:
             raise
         else:
             warnings.warn(
-                "Wizard {} cannot be registered. Please make sure that "
-                "BlogConfig.namespace {} and BlogConfig.app_title {} are"
-                "unique together".format(seed, config.namespace, config.app_title)
+                f"Wizard {seed} cannot be registered. Please make sure that "
+                f"BlogConfig.namespace {config.namespace} and BlogConfig.app_title {config.app_title} are"
+                "unique together",
+                stacklevel=2,
             )
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/feeds.py` & `djangocms-blog-2.0.0b1/djangocms_blog/feeds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from html import unescape
+from io import BytesIO
 
 from aldryn_apphooks_config.utils import get_app_instance
 from django.contrib.sites.models import Site
 from django.contrib.syndication.views import Feed
 from django.core.cache import cache
 from django.urls import reverse
 from django.utils.encoding import force_str
 from django.utils.feedgenerator import Rss201rev2Feed
 from django.utils.html import strip_tags
 from django.utils.safestring import mark_safe
 from django.utils.text import normalize_newlines
 from django.utils.translation import get_language_from_request, gettext as _
 from lxml import etree
-from six import BytesIO
 
 from djangocms_blog.settings import get_setting
 from djangocms_blog.views import PostDetailView
 
 from .models import Post
 
 
@@ -35,15 +35,19 @@
     def title(self):
         return Site.objects.get_current().name
 
     def description(self):
         return _("Blog articles on %(site_name)s") % {"site_name": Site.objects.get_current().name}
 
     def items(self, obj=None):
-        return Post.objects.namespace(self.namespace).published().order_by("-date_published")[: self.feed_items_number]
+        return (
+            Post.objects.namespace(self.namespace)
+            .published_on_rss()
+            .order_by("-date_published")[: self.feed_items_number]
+        )
 
     def item_title(self, item):
         return mark_safe(item.safe_translation_getter("title"))
 
     def item_description(self, item):
         if item.app_config.use_abstract:
             return mark_safe(item.safe_translation_getter("abstract"))
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/forms.py` & `djangocms-blog-2.0.0b1/djangocms_blog/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/liveblog/cms_plugins.py` & `djangocms-blog-2.0.0b1/djangocms_blog/liveblog/cms_plugins.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from djangocms_text_ckeditor.cms_plugins import TextPlugin
 
 from djangocms_blog.settings import get_setting
 
 from .models import Liveblog
 
 
+@plugin_pool.register_plugin
 class LiveblogPlugin(TextPlugin):
     module = get_setting("PLUGIN_MODULE_NAME")
     name = _("Liveblog item")
     model = Liveblog
     fields = ("title", "publish", "body", "post_date")
     render_template = "liveblog/plugins/liveblog.html"
 
@@ -20,10 +21,7 @@
             obj.send(request)
 
     def render(self, context, instance, placeholder):
         context = super().render(context, instance, placeholder)
         instance.content = context["body"]
         context["instance"] = instance
         return context
-
-
-plugin_pool.register_plugin(LiveblogPlugin)
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/liveblog/consumers.py` & `djangocms-blog-2.0.0b1/djangocms_blog/liveblog/consumers.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,10 @@
         Connect users to the group of the post according to the URL parameters
         """
         post = self._get_post(self.scope["url_route"]["kwargs"])
         if post:
             return [post.liveblog_group]
         else:
             return []
+
+    def send_json(self, content, close=False):
+        return super().send_json(content, close)
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/liveblog/migrations/0001_initial.py` & `djangocms-blog-2.0.0b1/djangocms_blog/liveblog/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import django.db.models.deletion
 import filer.fields.image
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("cms", "0013_urlconfrevision"),
         ("filer", "0003_thumbnailoption"),
     ]
 
     operations = [
         migrations.CreateModel(
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/liveblog/migrations/0003_auto_20160917_0123.py` & `djangocms-blog-2.0.0b1/djangocms_blog/liveblog/migrations/0003_auto_20160917_0123.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 import django.utils.timezone
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("liveblog", "0002_liveblog_title"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="liveblog",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/liveblog/models.py` & `djangocms-blog-2.0.0b1/djangocms_blog/liveblog/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,16 @@
                 "id": self.pk,
                 "content": content,
                 "creation_date": self.post_date.strftime(DATE_FORMAT),
                 "changed_date": self.changed_date.strftime(DATE_FORMAT),
                 "type": "send.json",
             }
             channel_layer = get_channel_layer()
-            async_to_sync(channel_layer.group_send)(self.liveblog_group, notification)
+            group = self.liveblog_group
+            async_to_sync(channel_layer.group_send)(group, notification)
 
 
 class Liveblog(LiveblogInterface, AbstractText):
     """
     Basic liveblog plugin model
     """
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/liveblog/static/liveblog/js/liveblog.js` & `djangocms-blog-2.0.0b1/djangocms_blog/liveblog/static/liveblog/js/liveblog.js`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/liveblog/static/liveblog/js/reconnecting-websocket.min.js` & `djangocms-blog-2.0.0b1/djangocms_blog/liveblog/static/liveblog/js/reconnecting-websocket.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/ar/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/ar/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/de/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/de/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/en/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/es/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/es/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/et/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/et/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/fr/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/fr/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/it/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/it/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/lt/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/lt/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/nb_NO/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/nb_NO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/nb_NO/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/nl/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/nl/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/pl_PL/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/pl_PL/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/pt_BR/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/pt_BR/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/ru/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/ru/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/sl/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/sl/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/tr/LC_MESSAGES/django.mo` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/locale/tr/LC_MESSAGES/django.po` & `djangocms-blog-2.0.0b1/djangocms_blog/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/managers.py` & `djangocms-blog-2.0.0b1/djangocms_blog/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
     def published(self, current_site=True):
         queryset = self.published_future(current_site)
         if self.start_date_field:
             return queryset.filter(**{"%s__lte" % self.start_date_field: now()})
         else:
             return queryset
 
+    def published_on_rss(self, current_site=True):
+        queryset = self.published_future(current_site)
+        return queryset.exclude(include_in_rss=False)
+
     def published_future(self, current_site=True):
         if current_site:
             queryset = self.on_site()
         else:
             queryset = self
         if self.end_date_field:
             qfilter = models.Q(**{"%s__gte" % self.end_date_field: now()}) | models.Q(
@@ -140,14 +144,17 @@
 
     def get_queryset(self, *args, **kwargs):
         return super().get_queryset(*args, **kwargs)
 
     def published(self, current_site=True):
         return self.get_queryset().published(current_site)
 
+    def published_on_rss(self, current_site=True):
+        return self.get_queryset().published_on_rss(current_site)
+
     def available(self, current_site=True):
         return self.get_queryset().available(current_site)
 
     def archived(self, current_site=True):
         return self.get_queryset().archived(current_site)
 
     def published_future(self, current_site=True):
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/media/base.py` & `djangocms-blog-2.0.0b1/djangocms_blog/media/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0001_initial.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 
 from djangocms_blog.models import thumbnail_model
 
 ACTUAL_FILER_IMAGE_MODEL = FILER_IMAGE_MODEL or "filer.Image"
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         migrations.swappable_dependency(ACTUAL_FILER_IMAGE_MODEL),
-        ("cms", "__first__"),
+        ("cms", "0020_old_tree_cleanup"),
         ("taggit", "__first__"),
         ("filer", "0003_thumbnailoption"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="AuthorEntriesPlugin",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0002_post_sites.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0002_post_sites.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("sites", "__first__"),
         ("djangocms_blog", "0001_initial"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="post",
             name="sites",
             field=models.ManyToManyField(
-                help_text="Select sites in which to show the post. If none is set it will bevisible in all the configured sites.",
+                help_text="Select sites in which to show the post. If none is set it will be "
+                "visible in all the configured sites.",
                 to="sites.Site",
                 null=True,
                 verbose_name="Site(s",
                 blank=True,
             ),
             preserve_default=True,
         ),
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0003_auto_20141201_2252.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0003_auto_20141201_2252.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0002_post_sites"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="post",
             name="sites",
             field=models.ManyToManyField(
-                help_text="Select sites in which to show the post. If none is set it will be visible in all the configured sites.",
+                help_text="Select sites in which to show the post. If none is set it will "
+                "be visible in all the configured sites.",
                 to="sites.Site",
                 null=True,
                 verbose_name="Site(s)",
                 blank=True,
             ),
             preserve_default=True,
         ),
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0004_auto_20150108_1435.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0004_auto_20150108_1435.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from djangocms_blog.models import thumbnail_model
 
 ACTUAL_FILER_IMAGE_MODEL = FILER_IMAGE_MODEL or "filer.Image"
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(ACTUAL_FILER_IMAGE_MODEL),
         ("djangocms_blog", "0003_auto_20141201_2252"),
         ("filer", "0003_thumbnailoption"),
     ]
 
     operations = [
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0005_auto_20150212_1118.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0005_auto_20150212_1118.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import cms.models.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0004_auto_20150108_1435"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="post",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0007_auto_20150719_0933.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0007_auto_20150719_0933.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from djangocms_blog.models import thumbnail_model
 
 ACTUAL_FILER_IMAGE_MODEL = FILER_IMAGE_MODEL or "filer.Image"
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0006_auto_20150214_1907"),
         migrations.swappable_dependency(ACTUAL_FILER_IMAGE_MODEL),
         ("filer", "0003_thumbnailoption"),
     ]
 
     operations = [
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0009_latestpostsplugin_tags_new.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0009_latestpostsplugin_tags_new.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import taggit_autosuggest.managers
 from django.contrib.contenttypes.models import ContentType
-from django.db import migrations, models
+from django.db import migrations
 
 
 def migrate_tags(apps, schema_editor):
     LatestPostsPlugin = apps.get_model("djangocms_blog", "LatestPostsPlugin")
     Tag = apps.get_model("taggit", "Tag")
     TaggedItem = apps.get_model("taggit", "TaggedItem")
     plugin_content_type = ContentType.objects.get_for_model(LatestPostsPlugin)
@@ -14,25 +14,24 @@
                 tag=tag, object_id=plugin.pk, content_type_id=plugin_content_type.pk
             ).exists():
                 TaggedItem.objects.create(tag=tag, object_id=plugin.pk, content_type_id=plugin_content_type.pk)
 
 
 def migrate_tags_reverse(apps, schema_editor):
     LatestPostsPlugin = apps.get_model("djangocms_blog", "LatestPostsPlugin")
-    Tag = apps.get_model("taggit", "Tag")
+    apps.get_model("taggit", "Tag")
     TaggedItem = apps.get_model("taggit", "TaggedItem")
     plugin_content_type = ContentType.objects.get_for_model(LatestPostsPlugin)
     for tagged in TaggedItem.objects.filter(content_type_id=plugin_content_type.pk):
         post = LatestPostsPlugin.objects.get(pk=tagged.object_id)
         post.tags.add(tagged.tag)
         tagged.delete()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("taggit", "__first__"),
         ("djangocms_blog", "0008_auto_20150814_0831"),
     ]
 
     operations = [
         migrations.AddField(
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0010_auto_20150923_1151.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0010_auto_20150923_1151.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import aldryn_apphooks_config.fields
 import app_data.fields
 import djangocms_text_ckeditor.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("cms", "__first__"),
+        ("cms", "0020_old_tree_cleanup"),
         ("djangocms_blog", "0009_latestpostsplugin_tags_new"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="BlogConfig",
             fields=[
@@ -141,13 +140,14 @@
             unique_together={("language_code", "master")},
         ),
         migrations.AlterField(
             model_name="post",
             name="sites",
             field=models.ManyToManyField(
                 to="sites.Site",
-                help_text="Select sites in which to show the post. If none is set it will be visible in all the configured sites.",
+                help_text="Select sites in which to show the post. "
+                "If none is set it will be visible in all the configured sites.",
                 blank=True,
                 verbose_name="Site(s)",
             ),
         ),
     ]
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0011_auto_20151024_1809.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0011_auto_20151024_1809.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import django.utils.timezone
 from django.db import migrations, models
 
 from djangocms_blog.settings import get_setting
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0010_auto_20150923_1151"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="blogconfigtranslation",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0013_auto_20160201_2235.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0013_auto_20160201_2235.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 1.9.2 on 2016-02-01 21:35
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0012_auto_20151220_1734"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="post",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0014_auto_20160215_1331.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0014_auto_20160215_1331.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from cms.models import Page
 from cms.utils.i18n import get_language_list
-from django.db import migrations, models
+from django.db import migrations
 
 
 def forwards(apps, schema_editor):
     BlogConfig = apps.get_model("djangocms_blog", "BlogConfig")
     BlogConfigTranslation = apps.get_model("djangocms_blog", "BlogConfigTranslation")
     Post = apps.get_model("djangocms_blog", "Post")
     BlogCategory = apps.get_model("djangocms_blog", "BlogCategory")
@@ -13,31 +13,28 @@
     AuthorEntriesPlugin = apps.get_model("djangocms_blog", "AuthorEntriesPlugin")
     config = None
     for page in Page.objects.drafts().filter(application_urls="BlogApp"):
         config, created = BlogConfig.objects.get_or_create(namespace=page.application_namespace)
         if not BlogConfigTranslation.objects.exists():
             for lang in get_language_list():
                 title = page.get_title(lang)
-                translation = BlogConfigTranslation.objects.create(
-                    language_code=lang, master_id=config.pk, app_title=title
-                )
+                BlogConfigTranslation.objects.create(language_code=lang, master_id=config.pk, app_title=title)
     if config:
         for model in (Post, BlogCategory, GenericBlogPlugin, LatestPostsPlugin, AuthorEntriesPlugin):
             for item in model.objects.filter(app_config__isnull=True):
                 item.app_config = config
                 item.save()
 
 
 def backwards(apps, schema_editor):
     # No need for backward data migration
     pass
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("cms", "0004_auto_20140924_1038"),
         ("djangocms_blog", "0013_auto_20160201_2235"),
     ]
 
     operations = [
         migrations.RunPython(forwards, backwards),
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0016_auto_20160502_1741.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0016_auto_20160502_1741.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0015_auto_20160408_1849"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="blogcategorytranslation",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0018_thumbnail_move2.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0018_thumbnail_move2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.db import migrations, models
 
 from djangocms_blog.models import thumbnail_model
 
 
 class Migration(migrations.Migration):
-
     if "cmsplugin_filer" not in thumbnail_model:
         dependencies = [
             ("djangocms_blog", "0017_thumbnail_move"),
         ]
 
         operations = [
             migrations.AddField(
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0019_thumbnail_move3.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0019_thumbnail_move3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.db import migrations, models
+from django.db import migrations
 
 from djangocms_blog.models import thumbnail_model
 
 
 def move_thumbnail_opt_to_filer(apps, schema_editor):
     Post = apps.get_model("djangocms_blog", "Post")
     for post in Post.objects.all():
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0020_thumbnail_move4.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0020_thumbnail_move4.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from django.db import migrations, models
+from django.db import migrations
 
 from djangocms_blog.models import thumbnail_model
 
 
 class Migration(migrations.Migration):
-
     if "cmsplugin_filer" not in thumbnail_model:
         dependencies = [
             ("djangocms_blog", "0019_thumbnail_move3"),
         ]
 
         operations = [
             migrations.RemoveField(model_name="post", name="main_image_full"),
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0021_auto_20160823_2008.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0021_auto_20160823_2008.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 from djangocms_blog.models import thumbnail_model
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0020_thumbnail_move4"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorentriesplugin",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0021_post_liveblog.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0025_auto_20160803_0858.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-import cms.models.fields
+# Generated by Django 1.9.9 on 2016-08-03 06:58
+
+import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("cms", "__first__"),
-        ("djangocms_blog", "0020_thumbnail_move4"),
+        ("djangocms_blog", "0024_auto_20160706_1524"),
     ]
 
     operations = [
-        migrations.AddField(
-            model_name="post",
-            name="liveblog",
-            field=cms.models.fields.PlaceholderField(
-                related_name="live_blog", slotname="live_blog", editable=False, to="cms.Placeholder", null=True
+        migrations.AlterField(
+            model_name="blogcategory",
+            name="parent",
+            field=models.ForeignKey(
+                blank=True,
+                null=True,
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name="children",
+                to="djangocms_blog.BlogCategory",
+                verbose_name="parent",
             ),
         ),
     ]
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0022_auto_20170304_1040.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0022_auto_20170304_1040.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0023_auto_20160626_1539.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0023_auto_20160626_1539.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 1.9.6 on 2016-06-26 13:39
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0022_auto_20160605_2305"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="authorentriesplugin",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0024_auto_20160706_1524.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0024_auto_20160706_1524.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from djangocms_blog.settings import get_setting
 
 BLOG_PLUGIN_TEMPLATE_FOLDERS = get_setting("PLUGIN_TEMPLATE_FOLDERS")
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0023_auto_20160626_1539"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="authorentriesplugin",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0025_auto_20160803_0858.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0039_auto_20200331_2227.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-# Generated by Django 1.9.9 on 2016-08-03 06:58
+# Generated by Django 2.2.11 on 2020-03-31 20:27
 
-import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("djangocms_blog", "0024_auto_20160706_1524"),
+        ("djangocms_blog", "0038_post_media"),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name="blogcategory",
-            name="parent",
-            field=models.ForeignKey(
-                blank=True,
-                null=True,
-                on_delete=django.db.models.deletion.CASCADE,
-                related_name="children",
-                to="djangocms_blog.BlogCategory",
-                verbose_name="parent",
-            ),
+            model_name="blogcategorytranslation",
+            name="name",
+            field=models.CharField(max_length=752, verbose_name="name"),
+        ),
+        migrations.AlterField(
+            model_name="blogcategorytranslation",
+            name="slug",
+            field=models.SlugField(blank=True, max_length=752, verbose_name="slug"),
+        ),
+        migrations.AlterField(
+            model_name="posttranslation",
+            name="slug",
+            field=models.SlugField(allow_unicode=True, blank=True, max_length=752, verbose_name="slug"),
+        ),
+        migrations.AlterField(
+            model_name="posttranslation",
+            name="title",
+            field=models.CharField(max_length=752, verbose_name="title"),
         ),
     ]
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0028_auto_20170304_1040.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0028_auto_20170304_1040.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0031_auto_20170610_1744.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0031_auto_20170610_1744.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import sortedm2m.fields
 from django.db import migrations
 from sortedm2m.operations import AlterSortedManyToManyField
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0030_auto_20170509_1831"),
     ]
 
     operations = [
         AlterSortedManyToManyField(
             model_name="post",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0032_auto_20180109_0023.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0032_auto_20180109_0023.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 1.10.8 on 2018-01-08 23:23
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0031_auto_20170610_1744"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="blogcategorytranslation",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0037_auto_20190806_0743.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0037_auto_20190806_0743.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import parler.fields
 import taggit_autosuggest.managers
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("djangocms_blog", "0036_auto_20180913_1809"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorentriesplugin",
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/migrations/0038_post_media.py` & `djangocms-blog-2.0.0b1/djangocms_blog/migrations/0038_post_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import cms.models.fields
 import django.db.models.deletion
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("cms", "0020_old_tree_cleanup"),
         ("djangocms_blog", "0037_auto_20190806_0743"),
     ]
 
     operations = [
         migrations.AddField(
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/models.py` & `djangocms-blog-2.0.0b1/djangocms_blog/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django.db import models
 from django.db.models.signals import post_save, pre_delete
 from django.dispatch import receiver
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.encoding import force_bytes, force_str
 from django.utils.functional import cached_property
-from django.utils.html import escape, strip_tags
+from django.utils.html import strip_tags
 from django.utils.translation import get_language, gettext, gettext_lazy as _
 from djangocms_text_ckeditor.fields import HTMLField
 from filer.fields.image import FilerImageField
 from filer.models import ThumbnailOption
 from meta.models import ModelMeta
 from parler.models import TranslatableModel, TranslatedFields
 from parler.utils.context import switch_language
@@ -178,15 +178,15 @@
 
     def get_title(self):
         title = self.safe_translation_getter("name", any_language=True)
         return title.strip()
 
     def get_description(self):
         description = self.safe_translation_getter("meta_description", any_language=True)
-        return escape(strip_tags(description)).strip()
+        return strip_tags(description).strip()
 
 
 class Post(KnockerModel, BlogMetaMixin, TranslatableModel):
     """
     Blog post
     """
 
@@ -201,14 +201,15 @@
 
     date_created = models.DateTimeField(_("created"), auto_now_add=True)
     date_modified = models.DateTimeField(_("last modified"), auto_now=True)
     date_published = models.DateTimeField(_("published since"), null=True, blank=True)
     date_published_end = models.DateTimeField(_("published until"), null=True, blank=True)
     date_featured = models.DateTimeField(_("featured date"), null=True, blank=True)
     publish = models.BooleanField(_("publish"), default=False)
+    include_in_rss = models.BooleanField(_("include in RSS feed"), default=True)
     categories = models.ManyToManyField(
         "djangocms_blog.BlogCategory", verbose_name=_("category"), related_name="blog_posts", blank=True
     )
     main_image = FilerImageField(
         verbose_name=_("main image"),
         blank=True,
         null=True,
@@ -244,15 +245,17 @@
             "visible in all the configured sites."
         ),
     )
     app_config = AppHookConfigField(BlogConfig, null=True, verbose_name=_("app. config"))
 
     translations = TranslatedFields(
         title=models.CharField(_("title"), max_length=752),
-        slug=models.SlugField(_("slug"), max_length=752, blank=True, db_index=True, allow_unicode=True),
+        slug=models.SlugField(
+            _("slug"), max_length=752, blank=True, db_index=True, allow_unicode=get_setting("UNICODE_SLUGS")
+        ),
         subtitle=models.CharField(verbose_name=_("subtitle"), max_length=767, blank=True, default=""),
         abstract=HTMLField(_("abstract"), blank=True, default="", configuration="BLOG_ABSTRACT_CKEDITOR"),
         meta_description=models.TextField(verbose_name=_("post meta description"), blank=True, default=""),
         meta_keywords=models.TextField(verbose_name=_("post meta keywords"), blank=True, default=""),
         meta_title=models.CharField(
             verbose_name=_("post meta title"),
             help_text=_("used in title tag and social sharing"),
@@ -390,15 +393,15 @@
         """
         return self.safe_translation_getter("meta_keywords", default="").strip().split(",")
 
     def get_description(self):
         description = self.safe_translation_getter("meta_description", any_language=True)
         if not description:
             description = self.safe_translation_getter("abstract", any_language=True)
-        return escape(strip_tags(description)).strip()
+        return strip_tags(description).strip()
 
     def get_image_full_url(self):
         if self.main_image:
             return self.build_absolute_uri(self.main_image.url)
         return ""
 
     def get_image_width(self):
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/settings.py` & `djangocms-blog-2.0.0b1/djangocms_blog/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,22 @@
 )
 """
 .. _PERMALINKS:
 
 Permalinks styles.
 """
 
+BLOG_UNICODE_SLUGS = True
+"""
+.. _UNICODE_SLUGS:
+
+Allow unicode chars in auto-generated slugs.
+"""
+
+
 PERMALINKS_URLS = {  # noqa
     PERMALINK_TYPE_FULL_DATE: "<int:year>/<int:month>/<int:day>/<str:slug>/",
     PERMALINK_TYPE_SHORT_DATE: "<int:year>/<int:month>/<str:slug>/",
     PERMALINK_TYPE_CATEGORY: "<str:category>/<str:slug>/",
     PERMALINK_TYPE_SLUG: "<str:slug>/",
 }
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/sitemaps/__init__.py` & `djangocms-blog-2.0.0b1/djangocms_blog/sitemaps/__init__.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/static/djangocms_blog/css/djangocms_blog_admin.css` & `djangocms-blog-2.0.0b1/djangocms_blog/static/djangocms_blog/css/djangocms_blog_admin.css`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/base.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/includes/blog_item.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/includes/blog_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/includes/blog_meta.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/includes/blog_meta.html`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     </li>
     {% endif %}
 </ul>
 <ul class="post-detail tags">
     {% if post.categories.exists %}
         {% for category in post.categories.all %}
             {% if category.slug %}
-                <li class="category_{{ forloop.counter }}"><a href="{% url 'djangocms_blog:posts-category' category=category.slug %}" class="blog-categories-{{ category.count }}">{{ category.name }}</a>{% if not forloop.last %}, {% endif %}</li>
+                <li class="category_{{ forloop.counter }}"><a href="{% url 'djangocms_blog:posts-category' category=category.slug %}" class="blog-categories-{{ category.count }} blog-categories-{{ category.slug }}">{{ category.name }}</a>{% if not forloop.last %}, {% endif %}</li>
             {% endif %}
         {% endfor %}
     {% endif %}
     {% if post.tags.exists %}
         {% for tag in post.tags.all %}
-            <li class="tag_{{ forloop.counter }}"><a href="{% url 'djangocms_blog:posts-tagged' tag=tag.slug %}" class="blog-tag blog-tag-{{ tag.count }}">{{ tag.name }}</a>{% if not forloop.last %}, {% endif %}</li>
+            <li class="tag_{{ forloop.counter }}"><a href="{% url 'djangocms_blog:posts-tagged' tag=tag.slug %}" class="blog-tag blog-tag-{{ tag.count }} blog-tag-{{ tag.slug }}">{{ tag.name }}</a>{% if not forloop.last %}, {% endif %}</li>
         {% endfor %}
     {% endif %}
 </ul>
```

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/archive.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/archive.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/authors.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/authors.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/authors_posts.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/authors_posts.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/categories.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/categories.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/plugins/tags.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/plugins/tags.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/post_detail.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/post_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/post_instant_article.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/post_instant_article.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templates/djangocms_blog/post_list.html` & `djangocms-blog-2.0.0b1/djangocms_blog/templates/djangocms_blog/post_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/templatetags/djangocms_blog.py` & `djangocms-blog-2.0.0b1/djangocms_blog/templatetags/djangocms_blog.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/urls.py` & `djangocms-blog-2.0.0b1/djangocms_blog/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog/views.py` & `djangocms-blog-2.0.0b1/djangocms_blog/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-1.2.3/djangocms_blog.egg-info/SOURCES.txt` & `djangocms-blog-2.0.0b1/djangocms_blog.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 djangocms_blog/cms_toolbars.py
 djangocms_blog/cms_wizards.py
 djangocms_blog/feeds.py
 djangocms_blog/fields.py
 djangocms_blog/forms.py
 djangocms_blog/managers.py
 djangocms_blog/models.py
-djangocms_blog/search_indexes.py
 djangocms_blog/settings.py
 djangocms_blog/taggit_urls.py
 djangocms_blog/urls.py
 djangocms_blog/views.py
 djangocms_blog.egg-info/PKG-INFO
 djangocms_blog.egg-info/SOURCES.txt
 djangocms_blog.egg-info/dependency_links.txt
@@ -43,15 +42,14 @@
 djangocms_blog/liveblog/migrations/0002_liveblog_title.py
 djangocms_blog/liveblog/migrations/0003_auto_20160917_0123.py
 djangocms_blog/liveblog/migrations/__init__.py
 djangocms_blog/liveblog/static/liveblog/js/liveblog.js
 djangocms_blog/liveblog/static/liveblog/js/reconnecting-websocket.min.js
 djangocms_blog/liveblog/templates/liveblog/includes/post_detail.html
 djangocms_blog/liveblog/templates/liveblog/plugins/liveblog.html
-djangocms_blog/liveblog/templates/liveblog/plugins/unpublished.html
 djangocms_blog/locale/ar/LC_MESSAGES/django.mo
 djangocms_blog/locale/ar/LC_MESSAGES/django.po
 djangocms_blog/locale/de/LC_MESSAGES/django.mo
 djangocms_blog/locale/de/LC_MESSAGES/django.po
 djangocms_blog/locale/en/LC_MESSAGES/django.mo
 djangocms_blog/locale/en/LC_MESSAGES/django.po
 djangocms_blog/locale/es/LC_MESSAGES/django.mo
@@ -117,14 +115,15 @@
 djangocms_blog/migrations/0033_auto_20180226_1410.py
 djangocms_blog/migrations/0034_merge.py
 djangocms_blog/migrations/0035_posttranslation_subtitle.py
 djangocms_blog/migrations/0036_auto_20180913_1809.py
 djangocms_blog/migrations/0037_auto_20190806_0743.py
 djangocms_blog/migrations/0038_post_media.py
 djangocms_blog/migrations/0039_auto_20200331_2227.py
+djangocms_blog/migrations/0040_post_include_in_rss.py
 djangocms_blog/migrations/__init__.py
 djangocms_blog/sitemaps/__init__.py
 djangocms_blog/static/djangocms_blog/css/djangocms_blog.css
 djangocms_blog/static/djangocms_blog/css/djangocms_blog_admin.css
 djangocms_blog/templates/djangocms_blog/base.html
 djangocms_blog/templates/djangocms_blog/post_archive.html
 djangocms_blog/templates/djangocms_blog/post_detail.html
@@ -135,8 +134,20 @@
 djangocms_blog/templates/djangocms_blog/plugins/archive.html
 djangocms_blog/templates/djangocms_blog/plugins/authors.html
 djangocms_blog/templates/djangocms_blog/plugins/authors_posts.html
 djangocms_blog/templates/djangocms_blog/plugins/categories.html
 djangocms_blog/templates/djangocms_blog/plugins/latest_entries.html
 djangocms_blog/templates/djangocms_blog/plugins/tags.html
 djangocms_blog/templatetags/__init__.py
-djangocms_blog/templatetags/djangocms_blog.py
+djangocms_blog/templatetags/djangocms_blog.py
+tests/test_extension.py
+tests/test_indexing.py
+tests/test_liveblog.py
+tests/test_media.py
+tests/test_menu.py
+tests/test_models.py
+tests/test_namespace.py
+tests/test_plugins.py
+tests/test_setup.py
+tests/test_toolbar.py
+tests/test_views.py
+tests/test_wizards.py
```

### Comparing `djangocms-blog-1.2.3/setup.cfg` & `djangocms-blog-2.0.0b1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-[bumpversion]
-current_version = 1.2.3
-parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.?)(?P<release>[a-z]*)(?P<relver>\d*)
-serialize = 
-	{major}.{minor}.{patch}.{release}{relver}
-	{major}.{minor}.{patch}
-commit = True
-tag = True
-sign_tags = True
-tag_name = {new_version}
-message = Release {new_version}
-
-[bumpversion:part:release]
-optional_value = gamma
-values = 
-	dev
-	a
-	b
-	rc
-	gamma
-
-[bumpversion:file:djangocms_blog/__init__.py]
-
 [metadata]
 name = djangocms-blog
 version = attr: djangocms_blog.__version__
 url = https://github.com/nephila/djangocms-blog
 project_urls = 
 	Documentation = https://djangocms-blog.readthedocs.io/
 author = Iacopo Spalletti
@@ -34,45 +11,46 @@
 long_description_content_type = text/x-rst
 license = BSD
 license_file = LICENSE
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
-	Framework :: Django :: 2.2
-	Framework :: Django :: 3.0
-	Framework :: Django :: 3.1
+	Framework :: Django :: 3.2
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 install_requires = 
 	django-parler>=2.0
-	django-cms>=3.7
+	django-cms>=3.9
 	django-taggit>=1.0
-	django-filer>=1.4
+	django-filer>=2.0
 	pytz
 	django-taggit-templatetags
 	django-taggit-autosuggest
 	djangocms-text-ckeditor>=3.9
 	easy-thumbnails>=2.4.1
 	django-meta>=2.0
 	aldryn-apphooks-config>=0.5
 	djangocms-apphook-setup
 	django-sortedm2m
 	lxml
 setup_requires = 
 	setuptools
 packages = djangocms_blog
-python_requires = >=3.6
+python_requires = >=3.7
 test_suite = cms_helper.run
 zip_safe = False
 keywords = 
 	djangocms-blog
 	blog
 	django
 	wordpress
@@ -80,21 +58,17 @@
 	django-app-enabler addon
 
 [options.package_data]
 * = *.txt, *.rst
 djangocms_blog = *.html *.png *.gif *js *jpg *jpeg *svg *py *mo *po
 
 [options.extras_require]
-search = aldryn-search
 taggit-helpers = django-taggit-helpers
 docs = 
-	django<3.1
-
-[upload]
-repository = https://upload.pypi.org/legacy/
+	django<5.0
 
 [sdist]
 formats = zip
 
 [bdist_wheel]
 universal = 1
```

