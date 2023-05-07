# Comparing `tmp/aldryn-apphooks-config-0.6.0.tar.gz` & `tmp/aldryn-apphooks-config-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aldryn-apphooks-config-0.6.0.tar", last modified: Tue May 12 16:36:48 2020, max compression
+gzip compressed data, was "aldryn-apphooks-config-0.7.0.tar", last modified: Sun May  7 16:06:07 2023, max compression
```

## Comparing `aldryn-apphooks-config-0.6.0.tar` & `aldryn-apphooks-config-0.7.0.tar`

### file list

```diff
@@ -1,99 +1,76 @@
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      588 2016-02-12 06:17:37.000000 aldryn-apphooks-config-0.6.0/.coveragerc
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      268 2015-10-18 07:55:16.000000 aldryn-apphooks-config-0.6.0/.editorconfig
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      413 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/.gitignore
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1137 2020-05-12 16:33:53.000000 aldryn-apphooks-config-0.6.0/.travis.yml
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/.tx/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      258 2017-03-04 08:09:24.000000 aldryn-apphooks-config-0.6.0/.tx/config
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     2215 2020-05-12 16:34:38.000000 aldryn-apphooks-config-0.6.0/CHANGELOG.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     3325 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/CONTRIBUTING.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1485 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/LICENSE
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      242 2017-11-01 14:31:28.000000 aldryn-apphooks-config-0.6.0/MANIFEST.in
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1281 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/Makefile
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     8761 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/PKG-INFO
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     6184 2020-05-12 16:33:53.000000 aldryn-apphooks-config-0.6.0/README.rst
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       46 2020-05-12 16:35:08.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     6509 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/admin.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      926 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/app_base.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1303 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/fields.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/de/
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1685 2017-03-04 08:09:24.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     2164 2017-03-04 08:09:24.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/en/
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/en/LC_MESSAGES/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      378 2017-03-04 08:09:24.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1499 2017-03-04 08:09:24.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/en/LC_MESSAGES/django.po
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/managers/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      168 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/managers/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     2199 2017-03-04 08:09:24.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/managers/base.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1577 2017-01-06 10:09:55.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/managers/parler.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      960 2017-11-01 15:00:44.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/mixins.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1617 2020-05-12 16:33:53.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/models.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/css/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/css/aldryn_apphooks_config.css
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/img/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/img/.gitignore
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/js/
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/js/aldryn_apphooks_config/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1164 2018-11-10 11:40:12.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/js/aldryn_apphooks_config/aldryn_apphooks_config.js
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templates/
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/admin/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      509 2018-11-10 11:39:58.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/admin/apphook_config_widget.html
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      661 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/base.html
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templatetags/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       24 2015-10-18 07:55:16.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templatetags/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1877 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templatetags/apphooks_config_tags.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       24 2018-02-20 17:16:06.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)    20758 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/test_config.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      973 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/test_migrations.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       24 2018-02-20 17:16:06.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/__init__.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       24 2018-02-20 17:16:06.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1180 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/admin.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      876 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/cms_appconfig.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      729 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/cms_apps.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/migrations/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     6543 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/migrations/0001_initial.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      651 2019-10-18 22:17:42.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/migrations/0002_auto_20191012_2339.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2016-04-12 20:44:26.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/migrations/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1287 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/models.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/templates/
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/templates/app1/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      111 2015-03-04 06:20:13.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/templates/app1/article_detail.html
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      163 2015-03-04 06:20:13.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/templates/app1/article_list.html
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/templates/app2/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      111 2015-03-04 06:20:13.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/templates/app2/article_detail.html
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      163 2015-03-04 06:20:13.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/templates/app2/article_list.html
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      766 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/views.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     3443 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/utils.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1023 2019-10-18 22:17:42.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/widgets.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config.egg-info/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     8761 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config.egg-info/PKG-INFO
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     2731 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config.egg-info/SOURCES.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config.egg-info/dependency_links.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2019-10-19 14:07:45.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config.egg-info/not-zip-safe
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       38 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config.egg-info/requires.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       23 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/aldryn_apphooks_config.egg-info/top_level.txt
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/docs/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     6777 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/docs/Makefile
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       27 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/docs/authors.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     8358 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/docs/conf.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       32 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/docs/contributing.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       30 2017-11-01 14:31:28.000000 aldryn-apphooks-config-0.6.0/docs/history.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      452 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/docs/index.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      235 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/docs/installation.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     6466 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/docs/make.bat
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       26 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/docs/readme.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      104 2014-12-17 17:38:56.000000 aldryn-apphooks-config-0.6.0/docs/usage.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      648 2020-05-12 16:36:48.000000 aldryn-apphooks-config-0.6.0/setup.cfg
--rwxrwxr-x   0 yakky     (1000) yakky     (1000)     1556 2020-05-12 16:34:49.000000 aldryn-apphooks-config-0.6.0/setup.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      235 2019-03-07 20:37:05.000000 aldryn-apphooks-config-0.6.0/test_requirements.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      865 2018-03-10 20:51:45.000000 aldryn-apphooks-config-0.6.0/test_settings.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      748 2020-05-12 16:33:53.000000 aldryn-apphooks-config-0.6.0/tox.ini
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     2285 2023-05-07 16:05:42.000000 aldryn-apphooks-config-0.7.0/CHANGELOG.rst
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     3322 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/CONTRIBUTING.rst
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1486 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/LICENSE
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      242 2023-02-12 10:56:40.000000 aldryn-apphooks-config-0.7.0/MANIFEST.in
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     9803 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/PKG-INFO
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     6216 2023-05-07 16:04:07.000000 aldryn-apphooks-config-0.7.0/README.rst
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)       22 2023-05-07 16:05:37.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     6447 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/admin.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      768 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/app_base.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1063 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/fields.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/de/
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1685 2023-02-12 10:56:40.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     2163 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/en/
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      378 2023-02-12 10:56:40.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1499 2023-02-12 10:56:40.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/managers/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)       70 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/managers/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1981 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/managers/base.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1471 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/managers/parler.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      815 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/mixins.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1425 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/models.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/static/
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/static/css/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2023-02-12 10:56:40.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/static/css/aldryn_apphooks_config.css
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/static/js/
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/static/js/aldryn_apphooks_config/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1165 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/static/js/aldryn_apphooks_config/aldryn_apphooks_config.js
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templates/
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/admin/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      509 2023-02-12 10:56:40.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/admin/apphook_config_widget.html
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      661 2023-02-12 10:56:40.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/base.html
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templatetags/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templatetags/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1768 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templatetags/apphooks_config_tags.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)    19824 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/test_config.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/__init__.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      983 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/admin.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      778 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/cms_appconfig.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      716 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/cms_apps.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/migrations/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     9041 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/migrations/0001_initial.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      681 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/migrations/0002_auto_20191012_2339.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2023-02-12 10:56:40.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/migrations/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1166 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/models.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/templates/
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/templates/app1/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      112 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/templates/app1/article_detail.html
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      164 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/templates/app1/article_list.html
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/templates/app2/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      112 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/templates/app2/article_detail.html
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      164 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/templates/app2/article_list.html
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      647 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/views.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     3322 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/utils.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      909 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/widgets.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:06:07.953178 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config.egg-info/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     9803 2023-05-07 16:06:07.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config.egg-info/PKG-INFO
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     2372 2023-05-07 16:06:07.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2023-05-07 16:06:07.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2023-02-12 11:14:09.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config.egg-info/not-zip-safe
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)       38 2023-05-07 16:06:07.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config.egg-info/requires.txt
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)       23 2023-05-07 16:06:07.000000 aldryn-apphooks-config-0.7.0/aldryn_apphooks_config.egg-info/top_level.txt
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      496 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/pyproject.toml
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1619 2023-05-07 16:06:07.957178 aldryn-apphooks-config-0.7.0/setup.cfg
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)       38 2023-05-07 16:03:52.000000 aldryn-apphooks-config-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aldryn-apphooks-config-0.6.0/CHANGELOG.rst` & `aldryn-apphooks-config-0.7.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Changelog
 =========
 
 
+0.7.0 (2023-05-07)
+==================
+
+* Add Django 3.2+ support
+
 0.6.0 (2020-05-12)
 ==================
 
 * Add Django 3.0 support
 
 0.5.3 (2019-10-19)
 ==================
 
 * Fix media asset declaration on django 2.2+
 
 0.5.2 (2019-01-02)
 ==================
 
-* Changed deprecated `rel.to` to `remote_field.model`
+* Changed deprecated ``rel.to`` to ``remote_field.model``
 * Fixed migration for example app
 * Fixed issues for Django 2.0 and up
 
 
 0.5.1 (2018-12-18)
 ==================
```

### Comparing `aldryn-apphooks-config-0.6.0/CONTRIBUTING.rst` & `aldryn-apphooks-config-0.7.0/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ============
 Contributing
 ============
 
 Contributions are welcome, and they are greatly appreciated! Every
-little bit helps, and credit will always be given. 
+little bit helps, and credit will always be given.
 
 You can contribute in many ways:
 
 Types of Contributions
 ----------------------
 
 Report Bugs
@@ -32,15 +32,15 @@
 
 Look through the GitHub issues for features. Anything tagged with "feature"
 is open to whoever wants to implement it.
 
 Write Documentation
 ~~~~~~~~~~~~~~~~~~~
 
-aldryn-apphooks-config could always use more documentation, whether as part of the 
+aldryn-apphooks-config could always use more documentation, whether as part of the
 official aldryn-apphooks-config docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
 The best way to send feedback is to file an issue at https://github.com/nephila/aldryn-apphooks-config/issues.
@@ -77,15 +77,15 @@
 5. When you're done making changes, check that your changes pass flake8 and the
 tests, including testing other Python versions with tox::
 
     $ flake8 aldryn_apphooks_config tests
     $ python setup.py test
     $ tox
 
-To get flake8 and tox, just pip install them into your virtualenv. 
+To get flake8 and tox, just pip install them into your virtualenv.
 
 6. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
 
@@ -96,17 +96,17 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 2.6, 2.7, and 3.3, and for PyPy. Check 
+3. The pull request should work for Python 2.6, 2.7, and 3.3, and for PyPy. Check
    https://travis-ci.org/nephila/aldryn-apphooks-config/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
 
-    $ python -m unittest tests.test_aldryn_apphooks_config
+    $ python -m unittest tests.test_aldryn_apphooks_config
```

### Comparing `aldryn-apphooks-config-0.6.0/LICENSE` & `aldryn-apphooks-config-0.7.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 
 * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
 * Neither the name of aldryn-apphooks-config nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `aldryn-apphooks-config-0.6.0/PKG-INFO` & `aldryn-apphooks-config-0.7.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,206 +1,334 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aldryn-apphooks-config
-Version: 0.6.0
+Version: 0.7.0
 Summary: Namespaces based configuration for Apphooks
 Home-page: https://github.com/aldryn/aldryn-apphooks-config
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.it
 License: BSD
-Description: |PyPI Version| |Build Status| |Coverage Status|
-        
-        ======================
-        aldryn-apphooks-config
-        ======================
-        
-        Namespaces based configuration for Apphooks
-        
-        Basic concepts
-        ==============
-        
-        The concept of apphooks-config is to store all the configuration
-        in an applications-specific model, and let the developer
-        specify the desired option in a form.
-        In the views the model instance specific for the current
-        application namespace is loaded (through a mixin) and it's
-        thus available in the view to provide the configuration for
-        the current namespace.
-        
-        Namespaces can be created on the fly in the ``Page`` admin
-        **Advanced settings** by following the steps above.
-        When creating an application configuration, you are in fact defining a
-        namespace, which is saved in the same field in the ``Page`` model as the
-        plain namespaces.
-        
-        
-        Contributing
-        ------------
-        
-        We're grateful to all contributors who have helped create and maintain this package.
-        
-        Contributors are listed at `contributions page
-        <https://github.com/divio/aldryn-apphooks-config/graphs/contributors>`_.
-        
-        
-        Supported versions
-        -----------------------------
-        
-        Python: 3.5, 3.6, 3.7, 3.8
-        Django: 1.11, 2.2, 3.0
-        django CMS: 3.5, 3.6, 3.7
-        
-        
-        Implementation step-guide
-        =========================
-        
-        * Define a AppHookConfig model in ``cms_appconfig.py``::
-        
-            from aldryn_apphooks_config.models import AppHookConfig
-        
-            class NewsBlogConfig(AppHookConfig):
-                pass
-        
-          Implementation can be completely empty as the schema is defined in the
-          parent (abstract) model
-        
-        * Use apphooks managers in your model::
-        
-            from aldryn_apphooks_config.managers import AppHookConfigManager
-        
-            class Article(models.Model):
-                title = models.CharField()
-        
-                objects = AppHookConfigManager()
-        
-        ``AppHookConfigManager`` adds ``namespace`` method to manager and queryset::
-        
-            Article.objects.namespace('foobar')
-        
-        There is also a proper queryset, the ``ApphooksConfigQueryset``. Parler
-        integrated variants can be found in ``aldryn_apphooks_config.managers.parler``.
-        Names are ``AppHookConfigTranslatableManager`` and
-        ``AppHookConfigTranslatableQueryset``.
-        
-        * Define a ConfigForm in ``cms_appconfig.py``::
-        
-            from app_data import AppDataForm
-            from django import forms
-            from aldryn_newsblog.models import NewsBlogConfig
-            from aldryn_apphooks_config.utils import setup_config
-        
-            class BlogOptionForm(AppDataForm):
-                # fields are totally arbitrary: any form field supported by
-                # django-appdata is supported
-                show_authors = forms.BooleanField(required=False)
-                ...
-        
-            # this function will register the provided form with the model created
-            # at the above step
-            setup_config(BlogOptionForm, NewsBlogConfig)
-        
-            # setup_config can be used as a decorator too, but the `model`
-            # attribute must be added to the form class
-            @setup_config
-            class BlogOptionForm(AppDataForm):
-                model = NewsBlogConfig
-        
-        
-        
-        
-        * Define an admin class for the AppHookConfig model (usually in ``admin.py``::
-        
-            from django.contrib import admin
-            from aldryn_apphooks_config.admin import BaseAppHookConfig
-        
-            class BlogConfigAdmin(BaseAppHookConfig):
-        
-                def get_config_fields(self):
-                    # this method **must** be implemented and **must** return the
-                    # fields defined in the above form, with the ``config`` prefix
-                    # This is dependent on the django-appdata API
-                    return ('config.show_authors', ...)
-        
-        * Define a CMSApp derived from CMSConfigApp provided by this application
-          (in ``cms_app.py``/``cms_apps.py``)::
-        
-            from aldryn_apphooks_config.app_base import CMSConfigApp
-            from cms.apphook_pool import apphook_pool
-            from django.utils.translation import ugettext_lazy as _
-            from .models import NewsBlogConfig
-        
-        
-            class NewsBlogApp(CMSConfigApp):
-                name = _('NewsBlogApp')
-                urls = ['aldryn_newsblog.urls']
-                app_name = 'aldryn_newsblog'
-                # this option is specific of CMSConfigApp, and links the
-                # CMSApp to a specific AppHookConfig model
-                app_config = NewsBlogConfig
-        
-            apphook_pool.register(NewsBlogApp)
-        
-        * Implements your views inheriting the ``AppConfigMixin``::
-        
-            from django.views.generic.detail import DetailView
-            from aldryn_apphooks_config.mixins import AppConfigMixin
-        
-            class ArticleDetail(AppConfigMixin, DetailView):
-                def get_queryset(self):
-                    return Article.objects.namespace(self.namespace)
-        
-          ``AppConfigMixin`` provides a complete support to namespaces, so the view
-          is not required to set anything specific to support them; the following
-          attributes are set for the view class instance:
-        
-          * current namespace in ``self.namespace``
-          * namespace configuration (the instance of NewsBlogConfig) in ``self.config``
-          * current application in the ``current_app`` parameter passed to the
-            Response class
-        
-        Test setup
-        ==========
-        
-        To properly setup the data for tests to run for a apphook-config enabled application,
-        make sure you add the following code to your TestCase::
-        
-            MyTestCase():
-        
-                def setUp(self):
-                    # This is the namespace represented by the AppHookConfig model instance
-                    self.ns_newsblog = NewsBlogConfig.objects.create(namespace='NBNS')
-                    self.page = api.create_page(
-                        'page', self.template, self.language, published=True,
-                        # this is the name of the apphook defined in the CMSApp class
-                        apphook='NewsBlogApp',
-                        # The namespace is the namespace field of the AppHookConfig instance created above
-                        apphook_namespace=self.ns_newsblog.namespace)
-                    # publish the page to make the apphook available
-                    self.page.publish(self.language)
-        
-        
-        .. |PyPI Version| image:: http://img.shields.io/pypi/v/aldryn-apphooks-config.svg
-           :target: https://pypi.python.org/pypi/aldryn-apphooks-config
-        .. |Build Status| image:: http://img.shields.io/travis/aldryn/aldryn-apphooks-config/master.svg
-           :target: https://travis-ci.org/aldryn/aldryn-apphooks-config
-        .. |Coverage Status| image:: http://img.shields.io/coveralls/aldryn/aldryn-apphooks-config/master.svg
-           :target: https://coveralls.io/r/aldryn/aldryn-apphooks-config?branch=master
-        
-Keywords: aldryn-apphooks-config
-Platform: UNKNOWN
+Project-URL: Documentation, https://aldryn-apphooks-config.readthedocs.io/
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+|PyPI Version| |Coverage Status|
+
+======================
+aldryn-apphooks-config
+======================
+
+Namespaces based configuration for Apphooks
+
+Basic concepts
+==============
+
+The concept of apphooks-config is to store all the configuration
+in an applications-specific model, and let the developer
+specify the desired option in a form.
+In the views the model instance specific for the current
+application namespace is loaded (through a mixin) and it's
+thus available in the view to provide the configuration for
+the current namespace.
+
+Namespaces can be created on the fly in the ``Page`` admin
+**Advanced settings** by following the steps above.
+When creating an application configuration, you are in fact defining a
+namespace, which is saved in the same field in the ``Page`` model as the
+plain namespaces.
+
+
+Contributing
+------------
+
+We're grateful to all contributors who have helped create and maintain this package.
+
+Contributors are listed at `contributions page
+<https://github.com/divio/aldryn-apphooks-config/graphs/contributors>`_.
+
+
+Supported versions
+-----------------------------
+
+Python: 3.9 - 3.11
+Django: 3.2 - 4.2
+django CMS: 3.9 - 3.11
+
+
+Implementation step-guide
+=========================
+
+* Define a AppHookConfig model in ``cms_appconfig.py``::
+
+    from aldryn_apphooks_config.models import AppHookConfig
+
+    class NewsBlogConfig(AppHookConfig):
+        pass
+
+  Implementation can be completely empty as the schema is defined in the
+  parent (abstract) model
+
+* Use apphooks managers in your model::
+
+    from aldryn_apphooks_config.managers import AppHookConfigManager
+
+    class Article(models.Model):
+        title = models.CharField()
+
+        objects = AppHookConfigManager()
+
+``AppHookConfigManager`` adds ``namespace`` method to manager and queryset::
+
+    Article.objects.namespace('foobar')
+
+There is also a proper queryset, the ``ApphooksConfigQueryset``. Parler
+integrated variants can be found in ``aldryn_apphooks_config.managers.parler``.
+Names are ``AppHookConfigTranslatableManager`` and
+``AppHookConfigTranslatableQueryset``.
+
+* Define a ConfigForm in ``cms_appconfig.py``::
+
+    from app_data import AppDataForm
+    from django import forms
+    from aldryn_newsblog.models import NewsBlogConfig
+    from aldryn_apphooks_config.utils import setup_config
+
+    class BlogOptionForm(AppDataForm):
+        # fields are totally arbitrary: any form field supported by
+        # django-appdata is supported
+        show_authors = forms.BooleanField(required=False)
+        ...
+
+    # this function will register the provided form with the model created
+    # at the above step
+    setup_config(BlogOptionForm, NewsBlogConfig)
+
+    # setup_config can be used as a decorator too, but the `model`
+    # attribute must be added to the form class
+    @setup_config
+    class BlogOptionForm(AppDataForm):
+        model = NewsBlogConfig
+
+
+
+
+* Define an admin class for the AppHookConfig model (usually in ``admin.py``::
+
+    from django.contrib import admin
+    from aldryn_apphooks_config.admin import BaseAppHookConfig
+
+    class BlogConfigAdmin(BaseAppHookConfig):
+
+        def get_config_fields(self):
+            # this method **must** be implemented and **must** return the
+            # fields defined in the above form, with the ``config`` prefix
+            # This is dependent on the django-appdata API
+            return ('config.show_authors', ...)
+
+* Define a CMSApp derived from CMSConfigApp provided by this application
+  (in ``cms_app.py``/``cms_apps.py``)::
+
+    from aldryn_apphooks_config.app_base import CMSConfigApp
+    from cms.apphook_pool import apphook_pool
+    from django.utils.translation import ugettext_lazy as _
+    from .models import NewsBlogConfig
+
+
+    class NewsBlogApp(CMSConfigApp):
+        name = _('NewsBlogApp')
+        urls = ['aldryn_newsblog.urls']
+        app_name = 'aldryn_newsblog'
+        # this option is specific of CMSConfigApp, and links the
+        # CMSApp to a specific AppHookConfig model
+        app_config = NewsBlogConfig
+
+    apphook_pool.register(NewsBlogApp)
+
+* Implements your views inheriting the ``AppConfigMixin``::
+
+    from django.views.generic.detail import DetailView
+    from aldryn_apphooks_config.mixins import AppConfigMixin
+
+    class ArticleDetail(AppConfigMixin, DetailView):
+        def get_queryset(self):
+            return Article.objects.namespace(self.namespace)
+
+  ``AppConfigMixin`` provides a complete support to namespaces, so the view
+  is not required to set anything specific to support them; the following
+  attributes are set for the view class instance:
+
+  * current namespace in ``self.namespace``
+  * namespace configuration (the instance of NewsBlogConfig) in ``self.config``
+  * current application in the ``current_app`` parameter passed to the
+    Response class
+
+Test setup
+==========
+
+To properly setup the data for tests to run for a apphook-config enabled application,
+make sure you add the following code to your TestCase::
+
+    MyTestCase():
+
+        def setUp(self):
+            # This is the namespace represented by the AppHookConfig model instance
+            self.ns_newsblog = NewsBlogConfig.objects.create(namespace='NBNS')
+            self.page = api.create_page(
+                'page', self.template, self.language, published=True,
+                # this is the name of the apphook defined in the CMSApp class
+                apphook='NewsBlogApp',
+                # The namespace is the namespace field of the AppHookConfig instance created above
+                apphook_namespace=self.ns_newsblog.namespace)
+            # publish the page to make the apphook available
+            self.page.publish(self.language)
+
+
+.. |PyPI Version| image:: http://img.shields.io/pypi/v/aldryn-apphooks-config.svg
+   :target: https://pypi.python.org/pypi/aldryn-apphooks-config
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/divio/aldryn-apphooks-config/test.yml?style=flat-square
+   :target: https://github.com/divio/aldryn-apphooks-config/actions/workflows/test.yml
+.. |Coverage Status| image:: http://img.shields.io/coveralls/aldryn/aldryn-apphooks-config/master.svg
+   :target: https://coveralls.io/r/aldryn/aldryn-apphooks-config?branch=master
+
+Changelog
+=========
+
+
+0.7.0 (2023-05-07)
+==================
+
+* Add Django 3.2+ support
+
+0.6.0 (2020-05-12)
+==================
+
+* Add Django 3.0 support
+
+0.5.3 (2019-10-19)
+==================
+
+* Fix media asset declaration on django 2.2+
+
+0.5.2 (2019-01-02)
+==================
+
+* Changed deprecated ``rel.to`` to ``remote_field.model``
+* Fixed migration for example app
+* Fixed issues for Django 2.0 and up
+
+
+0.5.1 (2018-12-18)
+==================
+
+* Added support for Django 2.0 and 2.1
+* Removed support for Django < 1.11
+* Adapted testing infrastructure (tox/travis) to incorporate django CMS 3.6
+* Fixed setup.py
+
+
+0.4.2 (2018-12-17)
+==================
+
+* Fixed issue with Django 1.10 and below in AppHookConfigWidget
+
+
+0.4.1 (2018-04-10)
+==================
+
+* django-appdata>=0.2.0 is now required
+
+
+0.4.0 (2018-03-19)
+==================
+
+* Added Django 1.11 compatibility
+* Added django CMS 3.5 compatibility
+* Implemented django-appdata 0.2 interface
+* Removed south migrations
+* Dropped support for django CMS 3.3 and below
+* Allowed use setup_config as decorators
+
+
+0.3.3 (2017-03-06)
+==================
+
+* Fixed MANIFEST.in typo
+
+
+0.3.2 (2017-03-06)
+==================
+
+* Fixed setup.py issue
+* Added locale files to MANIFEST.in
+
+
+0.3.1 (2017-03-02)
+==================
+
+* Added translation system
+* Added german translation
+
+
+0.3.0 (2017-01-06)
+==================
+
+* Allowed override AppHookConfigField attributes
+* Dropped Django 1.7 and below
+* Dropped django CMS 3.1 and below
+* Added Django 1.10 support
+
+
+0.2.7 (2016-03-03)
+==================
+
+* Set namespace as readonly
+* Added official Django 1.9 support
+* Updated readme
+* Used path_info instead of path in resolve
+
+
+0.2.6 (2015-10-05)
+==================
+
+* Added support for Python 3.5
+* Added support for Django 1.9a1
+* Code style cleanup and tests
+
+
+0.2.5 (2015-09-25)
+==================
+
+* Added support for Django 1.8, django CMS 3.2
+* AppHookConfigTranslatableManager.get_queryset should use queryset_class
+* Skipped overriding admin form if app_config field not present
+
+
+0.2.4 (2015-04-20)
+==================
+
+* Fixed issue where an apphook could not be changed, once set.
+* Added optional 'default' kwarg to namespace_url templatetag
+
+
+0.1.0 (2014-01-01)
+==================
+
+* Released first version on PyPI.
```

### Comparing `aldryn-apphooks-config-0.6.0/README.rst` & `aldryn-apphooks-config-0.7.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|PyPI Version| |Build Status| |Coverage Status|
+|PyPI Version| |Coverage Status|
 
 ======================
 aldryn-apphooks-config
 ======================
 
 Namespaces based configuration for Apphooks
 
@@ -32,17 +32,17 @@
 Contributors are listed at `contributions page
 <https://github.com/divio/aldryn-apphooks-config/graphs/contributors>`_.
 
 
 Supported versions
 -----------------------------
 
-Python: 3.5, 3.6, 3.7, 3.8
-Django: 1.11, 2.2, 3.0
-django CMS: 3.5, 3.6, 3.7
+Python: 3.9 - 3.11
+Django: 3.2 - 4.2
+django CMS: 3.9 - 3.11
 
 
 Implementation step-guide
 =========================
 
 * Define a AppHookConfig model in ``cms_appconfig.py``::
 
@@ -167,11 +167,11 @@
                 apphook_namespace=self.ns_newsblog.namespace)
             # publish the page to make the apphook available
             self.page.publish(self.language)
 
 
 .. |PyPI Version| image:: http://img.shields.io/pypi/v/aldryn-apphooks-config.svg
    :target: https://pypi.python.org/pypi/aldryn-apphooks-config
-.. |Build Status| image:: http://img.shields.io/travis/aldryn/aldryn-apphooks-config/master.svg
-   :target: https://travis-ci.org/aldryn/aldryn-apphooks-config
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/divio/aldryn-apphooks-config/test.yml?style=flat-square
+   :target: https://github.com/divio/aldryn-apphooks-config/actions/workflows/test.yml
 .. |Coverage Status| image:: http://img.shields.io/coveralls/aldryn/aldryn-apphooks-config/master.svg
    :target: https://coveralls.io/r/aldryn/aldryn-apphooks-config?branch=master
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/admin.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
 import copy
 
-from django.core.exceptions import ObjectDoesNotExist
-from django.utils.translation import ugettext_lazy as _
-
 from app_data.admin import AppDataModelAdmin
+from django.core.exceptions import ObjectDoesNotExist
+from django.utils.translation import gettext_lazy as _
 
 from .utils import get_apphook_model
 
 
 class BaseAppHookConfig(AppDataModelAdmin):
     """
     Base class for AppHookConfig admins
@@ -18,36 +14,37 @@
     The ModelAdmins for the AppHookConfig concrete models must:
 
     * Extends this class
     * Define a `get_config_fields` method that return a tuple of fields to be
       shown in the AppHookConfig fieldset. Every structure available in a single
       ModelAdmin fieldset `fields` definition can be returned by this method.
     """
-    readonly_fields = ('type',)
+
+    readonly_fields = ("type",)
 
     def get_fieldsets(self, request, obj):
         return [
-            (None, {'fields': ('type', 'namespace')}),
-            (_('Config'), {'fields': self.get_config_fields()})
+            (None, {"fields": ("type", "namespace")}),
+            (_("Config"), {"fields": self.get_config_fields()}),
         ]
 
     def get_config_fields(self):
         return ()
 
     def get_readonly_fields(self, request, obj=None):
         if obj and obj.pk:
-            return tuple(self.readonly_fields) + ('namespace',)
+            return tuple(self.readonly_fields) + ("namespace",)
         else:
             return self.readonly_fields
 
 
-class ModelAppHookConfig(object):
-    app_config_attribute = 'app_config'
-    app_config_selection_title = _('Select app config')
-    app_config_selection_desc = _('Select the app config for the new object')
+class ModelAppHookConfig:
+    app_config_attribute = "app_config"
+    app_config_selection_title = _("Select app config")
+    app_config_selection_desc = _("Select the app config for the new object")
     app_config_values = {}
 
     def _app_config_select(self, request, obj):
         """
         Return the select value for apphook configs
 
         :param request: request object
@@ -62,17 +59,15 @@
             if config_model.objects.count() == 1:
                 return config_model.objects.first()
             return None
         elif obj and getattr(obj, self.app_config_attribute, False):
             return getattr(obj, self.app_config_attribute)
         elif request.GET.get(self.app_config_attribute, False):
             config_model = get_apphook_model(self.model, self.app_config_attribute)
-            return config_model.objects.get(
-                pk=int(request.GET.get(self.app_config_attribute, False))
-            )
+            return config_model.objects.get(pk=int(request.GET.get(self.app_config_attribute, False)))
         return False
 
     def _set_config_defaults(self, request, form, obj=None):
         """
         Cycle through app_config_values and sets the form value according to the
         options in the current apphook config.
 
@@ -99,20 +94,26 @@
         If the apphook config must be selected first, returns a fieldset with just the
          app config field and help text
         :param request:
         :param obj:
         :return:
         """
         app_config_default = self._app_config_select(request, obj)
-        if app_config_default is None and request.method == 'GET':
-            return (_(self.app_config_selection_title),
-                    {'fields': (self.app_config_attribute, ),
-                     'description': _(self.app_config_selection_desc)}),
+        if app_config_default is None and request.method == "GET":
+            return (
+                (
+                    _(self.app_config_selection_title),
+                    {
+                        "fields": (self.app_config_attribute,),
+                        "description": _(self.app_config_selection_desc),
+                    },
+                ),
+            )
         else:
-            return super(ModelAppHookConfig, self).get_fieldsets(request, obj)
+            return super().get_fieldsets(request, obj)
 
     def get_config_data(self, request, obj, name):
         """
         Method that retrieves a configuration option for a specific AppHookConfig instance
 
         :param request: the request object
         :param obj: the model instance
@@ -142,23 +143,25 @@
         Provides a flexible way to get the right form according to the context
 
         For the add view it checks whether the app_config is set; if not, a special form
         to select the namespace is shown, which is reloaded after namespace selection.
         If only one namespace exists, the current is selected and the normal form
         is used.
         """
-        form = super(ModelAppHookConfig, self).get_form(request, obj, **kwargs)
+        form = super().get_form(request, obj, **kwargs)
         if self.app_config_attribute not in form.base_fields:
             return form
         app_config_default = self._app_config_select(request, obj)
         if app_config_default:
             form.base_fields[self.app_config_attribute].initial = app_config_default
             get = copy.copy(request.GET)
             get[self.app_config_attribute] = app_config_default.pk
             request.GET = get
-        elif app_config_default is None and request.method == 'GET':
+        elif app_config_default is None and request.method == "GET":
+
             class InitialForm(form):
                 class Meta(form.Meta):
                     fields = (self.app_config_attribute,)
+
             form = InitialForm
         form = self._set_config_defaults(request, form, obj)
         return form
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/app_base.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/app_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
+from cms.app_base import CMSApp
 from django.core.exceptions import ObjectDoesNotExist
 from django.urls import reverse
 
-from cms.app_base import CMSApp
-
 
 class CMSConfigApp(CMSApp):
-
     def get_configs(self):
         return self.app_config.objects.all()
 
     def get_config(self, namespace):
         try:
             return self.app_config.objects.get(namespace=namespace)
         except ObjectDoesNotExist:
             return None
 
     def get_config_add_url(self):
         try:
-            return reverse('admin:%s_%s_add' % (self.app_config._meta.app_label,
-                                                self.app_config._meta.model_name))
+            return reverse("admin:{}_{}_add".format(self.app_config._meta.app_label, self.app_config._meta.model_name))
         except AttributeError:  # pragma: no cover
-            return reverse('admin:%s_%s_add' % (self.app_config._meta.app_label,
-                                                self.app_config._meta.module_name))
+            return reverse(
+                "admin:{}_{}_add".format(self.app_config._meta.app_label, self.app_config._meta.module_name)
+            )
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/django.mo` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/django.po` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2017-03-02 10:09+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/locale/en/LC_MESSAGES/django.po` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/managers/base.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/managers/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,59 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
 from django.db.models import Manager
 from django.db.models.query import QuerySet
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from ..utils import get_apphook_field_names
 
 
-class QuerySetMixin(object):
-
+class QuerySetMixin:
     def namespace(self, namespace, to=None):
         """
         Filter by namespace. Try to guess which field to use in lookup.
         Accept 'to' argument if you need to specify.
         """
         fields = get_apphook_field_names(self.model)
         if not fields:
             raise ValueError(
-                ugettext(
-                    'Can\'t find any relation to an ApphookConfig model in {0}'
-                ).format(self.model.__name__)
+                gettext("Can't find any relation to an ApphookConfig model in {0}").format(self.model.__name__)
             )
         if to and to not in fields:
             raise ValueError(
-                ugettext(
-                    'Can\'t find relation to ApphookConfig model named '
-                    '"{0}" in "{1}"'
-                ).format(to, self.model.__name__)
+                gettext("Can't find relation to ApphookConfig model named " '"{0}" in "{1}"').format(
+                    to, self.model.__name__
+                )
             )
         if len(fields) > 1 and to not in fields:
             raise ValueError(
-                ugettext(
+                gettext(
                     '"{0}" has {1} relations to an ApphookConfig model.'
                     ' Please, specify which one to use in argument "to".'
-                    ' Choices are: {2}'
-                ).format(
-                    self.model.__name__, len(fields), ', '.join(fields)
-                )
+                    " Choices are: {2}"
+                ).format(self.model.__name__, len(fields), ", ".join(fields))
             )
         else:
             if not to:
                 to = fields[0]
 
-        lookup = '{0}__namespace'.format(to)
+        lookup = "{}__namespace".format(to)
         kwargs = {lookup: namespace}
         return self.filter(**kwargs)
 
 
-class ManagerMixin(object):
-
+class ManagerMixin:
     def namespace(self, namespace, to=None):
         return self.get_queryset().namespace(namespace, to=to)
 
 
 class AppHookConfigQuerySet(QuerySetMixin, QuerySet):
     pass
 
 
 class AppHookConfigManager(ManagerMixin, Manager):
     """
     Manager intended to use in models that has relations to apphooks
     configs. Add the namespace method to manager and queryset that should
     be used to filter objects by it namespace.
     """
+
     def get_queryset(self):
         return AppHookConfigQuerySet(self.model, using=self.db)
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/managers/parler.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/managers/parler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
 from aldryn_apphooks_config.managers.base import ManagerMixin, QuerySetMixin
 
 try:
     from parler.managers import TranslatableManager, TranslatableQuerySet
 except ImportError:  # pragma: no cover
     raise ImportError(
-        'Parler can not be found. Use pip install '
-        'aldryn-apphooks-config[parler] or just install django-parler.'
+        "Parler can not be found. Use pip install " "aldryn-apphooks-config[parler] or just install django-parler."
     )
 
 
 class AppHookConfigTranslatableQueryset(TranslatableQuerySet, QuerySetMixin):
-
     def create(self, **kwargs):
         # Pass language setting to the object, as people start assuming
         # things like .language('xx').create(..) which is a nice API
         # after all.
         #
         # TODO: this create is copy of TranslatableQuerySet.create which
         # in someway is not called when using .language('en').create(..)
         # and instead is called Django Manager.create. I not figured why
         # it is acting like that.
         if self._language:
-            kwargs['_current_language'] = self._language
+            kwargs["_current_language"] = self._language
         return super(TranslatableQuerySet, self).create(**kwargs)
 
 
 class AppHookConfigTranslatableManager(TranslatableManager, ManagerMixin):
     """
     Manager intended to use in TranslatableModels that has relations
     to apphooks configs. Add the namespace method to manager and queryset
     that should be used to filter objects by it namespace.
     """
+
     queryset_class = AppHookConfigTranslatableQueryset
 
     def get_queryset(self):
         return self.queryset_class(self.model, using=self.db)
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/static/js/aldryn_apphooks_config/aldryn_apphooks_config.js` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/static/js/aldryn_apphooks_config/aldryn_apphooks_config.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
 00000410: 7820 7265 7175 6573 742e 0a20 2020 2020  x request..     
 00000420: 2020 2020 2a2f 0a20 2020 2020 2020 206c      */.        l
 00000430: 6f63 6174 696f 6e2e 7365 6172 6368 203d  ocation.search =
 00000440: 2024 2e70 6172 616d 2871 7565 7279 5061   $.param(queryPa
 00000450: 7261 6d65 7465 7273 293b 202f 2f20 4361  rameters); // Ca
 00000460: 7573 6573 2070 6167 6520 746f 2072 656c  uses page to rel
 00000470: 6f61 640a 2020 2020 7d0a 7d29 2864 6a61  oad.    }.})(dja
-00000480: 6e67 6f2e 6a51 7565 7279 293b            ngo.jQuery);
+00000480: 6e67 6f2e 6a51 7565 7279 293b 0a         ngo.jQuery);.
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/base.html` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templates/aldryn_apphooks_config/base.html`

 * *Files identical despite different names*

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/templatetags/apphooks_config_tags.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/templatetags/apphooks_config_tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
 from functools import partial
 
 from django import template, urls
 
 from ..utils import get_app_instance
 
 register = template.Library()
@@ -23,36 +20,35 @@
 
     Normally, this tag will return whatever is returned by the ultimate call to
     reverse, which also means it will raise NoReverseMatch if reverse() cannot
     find a match. This behaviour can be override by suppling a 'default' kwarg
     with the value of what should be returned when no match is found.
     """
 
-    namespace = kwargs.pop('namespace', None)
+    namespace = kwargs.pop("namespace", None)
 
     if not namespace:
-        namespace, __ = get_app_instance(context['request'])
+        namespace, __ = get_app_instance(context["request"])
 
     if namespace:
-        namespace += ':'
+        namespace += ":"
 
-    reverse = partial(
-        urls.reverse, '{0:s}{1:s}'.format(namespace, view_name))
+    reverse = partial(urls.reverse, "{:s}{:s}".format(namespace, view_name))
 
     # We're explicitly NOT happy to just re-raise the exception, as that may
     # adversely affect stack traces.
-    if 'default' not in kwargs:
+    if "default" not in kwargs:
         if kwargs:
             return reverse(kwargs=kwargs)
         elif args:
             return reverse(args=args)
         else:
             return reverse()
 
-    default = kwargs.pop('default', None)
+    default = kwargs.pop("default", None)
     try:
         if kwargs:
             return reverse(kwargs=kwargs)
         elif args:
             return reverse(args=args)
         else:
             return reverse()
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/test_config.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,269 +1,263 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
 import os.path
 from copy import deepcopy
+from io import StringIO
 
+from app_helper.base_test import BaseTestCase
+from cms import api
+from cms.apphook_pool import apphook_pool
+from cms.utils.conf import get_cms_setting
 from django.conf import settings
 from django.http import SimpleCookie
 from django.template import RequestContext, Template
 from django.urls import reverse
-from django.utils.encoding import force_text
-from django.utils.six import StringIO
-
-from cms import api
-from cms.apphook_pool import apphook_pool
-from cms.utils.conf import get_cms_setting
-
-from djangocms_helper.base_test import BaseTestCase
+from django.utils.encoding import force_str
 
 from ..utils import get_app_instance, get_apphook_configs, get_apphook_field_names
 from .utils.example.models import (
-    AnotherExampleConfig, Article, ExampleConfig, News, NotApphookedModel, TranslatableArticle,
+    AnotherExampleConfig,
+    Article,
+    ExampleConfig,
+    News,
+    NotApphookedModel,
+    TranslatableArticle,
 )
 
 
 class AppHookConfigTestCase(BaseTestCase):
-
     def setUp(self):
-        self.template = get_cms_setting('TEMPLATES')[0][0]
+        self.template = get_cms_setting("TEMPLATES")[0][0]
         self.language = settings.LANGUAGES[0][0]
-        self.root_page = api.create_page(
-            'root page', self.template, self.language, published=True)
+        self.root_page = api.create_page("root page", self.template, self.language, published=True)
         # This is needed in django CMS 3.5+ to keep the same tree across
         # all django CMS versions
-        if hasattr(self.root_page, 'set_as_homepage'):
+        if hasattr(self.root_page, "set_as_homepage"):
             self.root_page.set_as_homepage()
 
-        self.ns_app_1 = ExampleConfig.objects.create(namespace='app1')
-        self.ns_app_1.app_data.config.property = 'app1_property'
+        self.ns_app_1 = ExampleConfig.objects.create(namespace="app1")
+        self.ns_app_1.app_data.config.property = "app1_property"
         self.ns_app_1.app_data.config.published_default = False
         self.ns_app_1.save()
-        self.ns_app_2 = ExampleConfig.objects.create(namespace='app2')
-        self.ns_app_2.app_data.config.property = 'app2_property'
+        self.ns_app_2 = ExampleConfig.objects.create(namespace="app2")
+        self.ns_app_2.app_data.config.property = "app2_property"
         self.ns_app_2.app_data.config.published_default = True
         self.ns_app_2.save()
-        self.ns_app_3 = AnotherExampleConfig.objects.create(namespace='app3')
-        self.ns_app_3.app_data.config.property = 'app3_property'
+        self.ns_app_3 = AnotherExampleConfig.objects.create(namespace="app3")
+        self.ns_app_3.app_data.config.property = "app3_property"
         self.ns_app_3.app_data.config.published_default = True
         self.ns_app_3.save()
 
         self.page_1 = api.create_page(
-            'page_1', self.template, self.language, published=True,
+            "page_1",
+            self.template,
+            self.language,
+            published=True,
             parent=self.root_page,
-            apphook='ExampleApp',
-            apphook_namespace=self.ns_app_1.namespace)
+            apphook="ExampleApp",
+            apphook_namespace=self.ns_app_1.namespace,
+        )
         self.page_2 = api.create_page(
-            'page_2', self.template, self.language, published=True,
+            "page_2",
+            self.template,
+            self.language,
+            published=True,
             parent=self.root_page,
-            apphook='ExampleApp',
-            apphook_namespace=self.ns_app_2.namespace)
+            apphook="ExampleApp",
+            apphook_namespace=self.ns_app_2.namespace,
+        )
         self.page_3 = api.create_page(
-            'page_3', self.template, self.language, published=True,
+            "page_3",
+            self.template,
+            self.language,
+            published=True,
             parent=self.root_page,
-            apphook='SampleApp')
+            apphook="SampleApp",
+        )
 
         for page in self.root_page, self.page_1, self.page_2:
             for language, _ in settings.LANGUAGES[1:]:
                 api.create_title(language, page.get_slug(), page)
                 page.publish(language)
         self.reload_urlconf()
 
     def test_configs(self):
         app = apphook_pool.get_apphook(self.page_1.application_urls)
         self.assertEqual(app.get_configs().count(), 2)
 
     def test_wrong_ns(self):
         app = apphook_pool.get_apphook(self.page_1.application_urls)
-        self.assertIsNone(app.get_config('no_app'))
+        self.assertIsNone(app.get_config("no_app"))
 
     def test_bad_property(self):
         with self.assertRaises(AttributeError):
             self.ns_app_1.no_property
 
     def test_app_no_ns(self):
         request = self.get_page_request(self.page_3, self.user)
         config = get_app_instance(request)
         # when config is requested on a non-config apphook, just return empty data
-        self.assertEqual(('', None), config)
+        self.assertEqual(("", None), config)
 
     def test_no_page(self):
-        request = self.request_factory.get('/en/sample/login/')
+        request = self.request("/en/sample/login/")
         request.user = self.user
         request.session = {}
         request.cookies = SimpleCookie()
         request.errors = StringIO()
 
         # when config is requested on a non-CMS url, just return empty data
-        with self.settings(ROOT_URLCONF='cms.test_utils.project.urls'):
+        with self.settings(ROOT_URLCONF="cms.test_utils.project.urls"):
             config = get_app_instance(request)
-            self.assertEqual(('', None), config)
+            self.assertEqual(("", None), config)
 
     def test_config_str(self):
         app = apphook_pool.get_apphook(self.page_1.application_urls)
-        self.assertEqual('%s / %s' % (force_text(app.name), self.ns_app_1.namespace), force_text(self.ns_app_1))
+        self.assertEqual(
+            "{} / {}".format(force_str(app.name), self.ns_app_1.namespace),
+            force_str(self.ns_app_1),
+        )
 
     def test_admin_url(self):
         app = apphook_pool.get_apphook(self.page_1.application_urls)
         url = app.get_config_add_url()
         try:
-            self.assertEqual(url, reverse('admin:%s_%s_add' % (ExampleConfig._meta.app_label,
-                                                               ExampleConfig._meta.model_name)))
+            self.assertEqual(
+                url,
+                reverse("admin:{}_{}_add".format(ExampleConfig._meta.app_label, ExampleConfig._meta.model_name)),
+            )
         except AttributeError:  # noqa
-            self.assertEqual(url, reverse('admin:%s_%s_add' % (ExampleConfig._meta.app_label,
-                                                               ExampleConfig._meta.module_name)))
+            self.assertEqual(
+                url,
+                reverse("admin:{}_{}_add".format(ExampleConfig._meta.app_label, ExampleConfig._meta.module_name)),
+            )
 
     def test_app_1_list_empty(self):
-        response = self.client.get('/en/page_1/')
-        self.assertContains(response, 'namespace:app1')
-        self.assertContains(response, 'property:app1_property')
-        self.assertContains(response, 'objects:0')
+        response = self.client.get("/en/page_1/")
+        self.assertContains(response, "namespace:app1")
+        self.assertContains(response, "property:app1_property")
+        self.assertContains(response, "objects:0")
 
     def test_app_2_list_empty(self):
-        response = self.client.get('/en/page_2/')
-        self.assertContains(response, 'namespace:app2')
-        self.assertContains(response, 'property:app2_property')
-        self.assertContains(response, 'objects:0')
+        response = self.client.get("/en/page_2/")
+        self.assertContains(response, "namespace:app2")
+        self.assertContains(response, "property:app2_property")
+        self.assertContains(response, "objects:0")
 
     def test_app_1_list_items(self):
-        Article.objects.create(title='article_app_1',
-                               slug='article_app_1', section=self.ns_app_1)
-        response = self.client.get('/en/page_1/')
-        self.assertContains(response, 'namespace:app1')
-        self.assertContains(response, 'property:app1_property')
-        self.assertContains(response, 'objects:1')
+        Article.objects.create(title="article_app_1", slug="article_app_1", section=self.ns_app_1)
+        response = self.client.get("/en/page_1/")
+        self.assertContains(response, "namespace:app1")
+        self.assertContains(response, "property:app1_property")
+        self.assertContains(response, "objects:1")
 
     def test_app_2_list_items(self):
-        Article.objects.create(title='article_app_2',
-                               slug='article_app_2', section=self.ns_app_2)
-        response = self.client.get('/en/page_2/')
-        self.assertContains(response, 'namespace:app2')
-        self.assertContains(response, 'property:app2_property')
-        self.assertContains(response, 'objects:1')
+        Article.objects.create(title="article_app_2", slug="article_app_2", section=self.ns_app_2)
+        response = self.client.get("/en/page_2/")
+        self.assertContains(response, "namespace:app2")
+        self.assertContains(response, "property:app2_property")
+        self.assertContains(response, "objects:1")
 
     def test_apphook_manager_on_simple_model(self):
-        ns_app_3 = ExampleConfig.objects.create(namespace='app3')
-        ns_app_3.app_data.config.property = 'app3_property'
+        ns_app_3 = ExampleConfig.objects.create(namespace="app3")
+        ns_app_3.app_data.config.property = "app3_property"
         ns_app_3.save()
 
-        Article.objects.create(title='article_1_app_1',
-                               slug='article_1_app_1',
-                               section=self.ns_app_1)
-        Article.objects.create(title='article_2_app_1',
-                               slug='article_2_app_1',
-                               section=self.ns_app_1)
-        Article.objects.create(title='article_1_app_2',
-                               slug='article_1_app_2',
-                               section=self.ns_app_2)
-
-        self.assertEqual(
-            2, Article.objects.namespace(self.ns_app_1.namespace).count()
-        )
-        self.assertEqual(
-            1, Article.objects.namespace(self.ns_app_2.namespace).count()
-        )
-        self.assertEqual(
-            0, Article.objects.namespace(ns_app_3.namespace).count()
-        )
-        self.assertEqual(
-            0, Article.objects.namespace('').count()
-        )
+        Article.objects.create(title="article_1_app_1", slug="article_1_app_1", section=self.ns_app_1)
+        Article.objects.create(title="article_2_app_1", slug="article_2_app_1", section=self.ns_app_1)
+        Article.objects.create(title="article_1_app_2", slug="article_1_app_2", section=self.ns_app_2)
+
+        self.assertEqual(2, Article.objects.namespace(self.ns_app_1.namespace).count())
+        self.assertEqual(1, Article.objects.namespace(self.ns_app_2.namespace).count())
+        self.assertEqual(0, Article.objects.namespace(ns_app_3.namespace).count())
+        self.assertEqual(0, Article.objects.namespace("").count())
 
     def test_apphook_manager_on_model_with_two_configs(self):
-        ans_config_1 = AnotherExampleConfig.objects.create(namespace='config1')
-        ans_config_2 = AnotherExampleConfig.objects.create(namespace='config2')
-        News.objects.create(title='news_1_app_1_config1',
-                            slug='news_1_app_1_config1',
-                            section=self.ns_app_1,
-                            config=ans_config_1)
-        News.objects.create(title='news_2_app_1_config2',
-                            slug='news_2_app_1_config2',
-                            section=self.ns_app_1,
-                            config=ans_config_2)
-        msg = ('"{0}" has {1} relations to an ApphookConfig model.'
-               ' Please, specify which one to use in argument "to".'
-               ' Choices are: {2}'.format('News', '2', 'section, config'))
-        self.assertRaisesMessage(
-            ValueError, msg, News.objects.namespace, ans_config_1.namespace
-        )
-        self.assertEqual(
-            1, News.objects.namespace(ans_config_1.namespace,
-                                      to='config').count()
-        )
-        self.assertEqual(
-            2, News.objects.namespace(self.ns_app_1.namespace,
-                                      to='section').count()
-        )
+        ans_config_1 = AnotherExampleConfig.objects.create(namespace="config1")
+        ans_config_2 = AnotherExampleConfig.objects.create(namespace="config2")
+        News.objects.create(
+            title="news_1_app_1_config1",
+            slug="news_1_app_1_config1",
+            section=self.ns_app_1,
+            config=ans_config_1,
+        )
+        News.objects.create(
+            title="news_2_app_1_config2",
+            slug="news_2_app_1_config2",
+            section=self.ns_app_1,
+            config=ans_config_2,
+        )
+        msg = (
+            '"{}" has {} relations to an ApphookConfig model.'
+            ' Please, specify which one to use in argument "to".'
+            " Choices are: {}".format("News", "2", "section, config")
+        )
+        self.assertRaisesMessage(ValueError, msg, News.objects.namespace, ans_config_1.namespace)
+        self.assertEqual(1, News.objects.namespace(ans_config_1.namespace, to="config").count())
+        self.assertEqual(2, News.objects.namespace(self.ns_app_1.namespace, to="section").count())
 
     def test_translatable_apphook_manager(self):
-        t1 = TranslatableArticle.objects.language('en').create(
-            title='article_1_app_1_en', slug='article_1_app_1_en',
-            section=self.ns_app_1
-        )
-        self.assertEqual(t1.get_current_language(), 'en')
-        t2 = TranslatableArticle.objects.language('de').create(
-            title='article_2_app_1_de', slug='article_2_app_1_de',
-            section=self.ns_app_1
+        t1 = TranslatableArticle.objects.language("en").create(
+            title="article_1_app_1_en", slug="article_1_app_1_en", section=self.ns_app_1
         )
-        self.assertEqual(t2.get_current_language(), 'de')
-
-        self.assertEqual(
-            2, TranslatableArticle.objects.namespace(self.ns_app_1.namespace)
-                                          .count()
+        self.assertEqual(t1.get_current_language(), "en")
+        t2 = TranslatableArticle.objects.language("de").create(
+            title="article_2_app_1_de", slug="article_2_app_1_de", section=self.ns_app_1
         )
+        self.assertEqual(t2.get_current_language(), "de")
+
+        self.assertEqual(2, TranslatableArticle.objects.namespace(self.ns_app_1.namespace).count())
         self.assertEqual(
             1,
-            TranslatableArticle.objects.namespace(self.ns_app_1.namespace)
-                                       .translated('en')
-                                       .count()
+            TranslatableArticle.objects.namespace(self.ns_app_1.namespace).translated("en").count(),
         )
         self.assertEqual(
             1,
-            TranslatableArticle.objects.namespace(self.ns_app_1.namespace)
-                                       .translated('de')
-                                       .count()
+            TranslatableArticle.objects.namespace(self.ns_app_1.namespace).translated("de").count(),
         )
 
     def test_get_config_data(self):
         from django.contrib import admin
 
-        article = Article.objects.create(title='news_1_app_1_config1',
-                                         slug='news_1_app_1_config1',
-                                         section=self.ns_app_1)
+        article = Article.objects.create(
+            title="news_1_app_1_config1",
+            slug="news_1_app_1_config1",
+            section=self.ns_app_1,
+        )
 
         admin.autodiscover()
 
         admin_instance = admin.site._registry[Article]
 
         # correct parameter passed by the request
         request = self.get_page_request(self.page_3, self.user)
         request.GET = deepcopy(request.GET)
-        request.GET['section'] = self.ns_app_1.pk
-        retrieved = admin_instance.get_config_data(request, article, 'property')
+        request.GET["section"] = self.ns_app_1.pk
+        retrieved = admin_instance.get_config_data(request, article, "property")
         self.assertEqual(retrieved, self.ns_app_1.property)
 
         # correct parameter passed by the request - no existing object
         request = self.get_page_request(self.page_3, self.user)
         request.GET = deepcopy(request.GET)
-        request.GET['section'] = self.ns_app_1.pk
-        retrieved = admin_instance.get_config_data(request, Article(), 'property')
+        request.GET["section"] = self.ns_app_1.pk
+        retrieved = admin_instance.get_config_data(request, Article(), "property")
         self.assertEqual(retrieved, self.ns_app_1.property)
 
         # no parameter from request - config retrieved form existing instance
         request = self.get_page_request(self.page_3, self.user)
-        retrieved = admin_instance.get_config_data(request, article, 'property')
+        retrieved = admin_instance.get_config_data(request, article, "property")
         self.assertEqual(retrieved, self.ns_app_1.property)
 
     def test_config_select(self):
         from django.contrib import admin
 
-        article = Article.objects.create(title='news_1_app_1_config1',
-                                         slug='news_1_app_1_config1',
-                                         section=self.ns_app_1)
+        article = Article.objects.create(
+            title="news_1_app_1_config1",
+            slug="news_1_app_1_config1",
+            section=self.ns_app_1,
+        )
 
         admin.autodiscover()
 
         admin_instance = admin.site._registry[Article]
 
         # no object is set, no parameter passed through the request, two namespaces
         request = self.get_page_request(self.page_3, self.user)
@@ -281,174 +275,178 @@
         request = self.get_page_request(self.page_3, self.user)
         value = admin_instance._app_config_select(request, None)
         self.assertEqual(value, self.ns_app_1)
 
     def test_get_config_form(self):
         from django.contrib import admin
 
-        article = Article.objects.create(title='news_1_app_1_config1',
-                                         slug='news_1_app_1_config1',
-                                         section=self.ns_app_1)
+        article = Article.objects.create(
+            title="news_1_app_1_config1",
+            slug="news_1_app_1_config1",
+            section=self.ns_app_1,
+        )
 
         admin.autodiscover()
 
         admin_instance = admin.site._registry[Article]
 
         # no object is set, no parameter passed through the request, two namespaces
         request = self.get_page_request(self.page_3, self.user)
         form = admin_instance.get_form(request, None)
-        self.assertEqual(list(form.base_fields.keys()), ['section'])
-        self.assertEqual(form.base_fields['section'].initial, None)
+        self.assertEqual(list(form.base_fields.keys()), ["section"])
+        self.assertEqual(form.base_fields["section"].initial, None)
 
         # object is set, normal form is used
         request = self.get_page_request(self.page_3, self.user)
         request.GET = deepcopy(request.GET)
-        request.GET['section'] = self.ns_app_1.pk
+        request.GET["section"] = self.ns_app_1.pk
         form = admin_instance.get_form(request, article)
-        self.assertEqual(list(form.base_fields.keys()), ['title', 'slug', 'section', 'published'])
-        self.assertEqual(form.base_fields['section'].initial, self.ns_app_1)
+        self.assertEqual(list(form.base_fields.keys()), ["title", "slug", "section", "published"])
+        self.assertEqual(form.base_fields["section"].initial, self.ns_app_1)
 
         # no object is set, parameter passed through the request
         request = self.get_page_request(self.page_3, self.user)
         request.GET = deepcopy(request.GET)
-        request.GET['section'] = self.ns_app_1.pk
+        request.GET["section"] = self.ns_app_1.pk
         form = admin_instance.get_form(request, None)
-        self.assertEqual(list(form.base_fields.keys()), ['title', 'slug', 'section', 'published'])
-        self.assertEqual(form.base_fields['section'].initial, self.ns_app_1)
+        self.assertEqual(list(form.base_fields.keys()), ["title", "slug", "section", "published"])
+        self.assertEqual(form.base_fields["section"].initial, self.ns_app_1)
 
         self.ns_app_2.delete()
         request = self.get_page_request(self.page_3, self.user)
         app_config_default = admin_instance._app_config_select(request, None)
         self.assertEqual(app_config_default, self.ns_app_1)
 
         # no object is set, no parameter passed through the request, one namespace
         request = self.get_page_request(self.page_3, self.user)
         form = admin_instance.get_form(request, None)
-        self.assertEqual(list(form.base_fields.keys()), ['title', 'slug', 'section', 'published'])
-        self.assertEqual(form.base_fields['section'].initial, self.ns_app_1)
+        self.assertEqual(list(form.base_fields.keys()), ["title", "slug", "section", "published"])
+        self.assertEqual(form.base_fields["section"].initial, self.ns_app_1)
 
     def test_apphook_admin(self):
         from django.contrib import admin
+
         admin.autodiscover()
 
         admin_instance = admin.site._registry[ExampleConfig]
         request = self.get_page_request(self.page_3, self.user)
 
         # Testing Readonly field
+        self.assertEqual(admin_instance.get_readonly_fields(request), ("type",))
         self.assertEqual(
-            admin_instance.get_readonly_fields(request), ('type',)
-        )
-        self.assertEqual(
-            admin_instance.get_readonly_fields(request, self.ns_app_1), ('type', 'namespace')
+            admin_instance.get_readonly_fields(request, self.ns_app_1),
+            ("type", "namespace"),
         )
 
         # Testing admin output for sample app specific implementation
         response = admin_instance.change_view(request, str(self.ns_app_1.pk))
         try:
             self.assertContains(
                 response,
-                '<div class="readonly">aldryn_apphooks_config.tests.utils.example.cms_appconfig.ExampleConfig</div>'
+                '<div class="readonly">aldryn_apphooks_config.tests.utils.example.cms_appconfig.ExampleConfig</div>',
             )
             self.assertContains(response, '<div class="readonly">app1</div>')
             self.assertContains(response, 'value="app1_property"')
         except AssertionError:
             self.assertContains(
                 response,
-                '<p>aldryn_apphooks_config.tests.utils.example.cms_appconfig.ExampleConfig</p>'
+                "<p>aldryn_apphooks_config.tests.utils.example.cms_appconfig.ExampleConfig</p>",
             )
-            self.assertContains(response, '<p>app1</p>')
+            self.assertContains(response, "<p>app1</p>")
             self.assertContains(response, 'name="config-property" type="text" value="app1_property"')
 
     def test_admin(self):
         from django.contrib import admin
+
         admin.autodiscover()
 
         admin_instance = admin.site._registry[Article]
 
         # testing behavior when more than 1 namespace instance exists - the selection form
         # should be shown
         request = self.get_page_request(self.page_3, self.user)
         response = admin_instance.add_view(request)
-        self.assertContains(response, '$(this).apphook_reload_admin')
-        self.assertContains(response, 'var sel = $(\'#id_section\');')
-        self.assertContains(response, 'aldryn_apphooks_config')
+        self.assertContains(response, "$(this).apphook_reload_admin")
+        self.assertContains(response, "var sel = $('#id_section');")
+        self.assertContains(response, "aldryn_apphooks_config")
         self.assertContains(response, '<option value="1">%s</option>' % self.ns_app_1)
         self.assertContains(response, '<option value="2">%s</option>' % self.ns_app_2)
-        self.assertContains(response, '<h2>Select app config</h2>')
+        self.assertContains(response, "<h2>Select app config</h2>")
 
         # only one namespace instance exists, the normal changeform is used
         self.ns_app_2.delete()
         response = admin_instance.add_view(request)
-        self.assertContains(response, '$(this).apphook_reload_admin')
-        self.assertContains(response, 'aldryn_apphooks_config')
-        self.assertRegexpMatches(
-            force_text(response.content),
-            '(<option value="1" selected="selected">%s</option>|<option value="1" selected>%s</option>)' % (
-                self.ns_app_1, self.ns_app_1
-            )
+        self.assertContains(response, "$(this).apphook_reload_admin")
+        self.assertContains(response, "aldryn_apphooks_config")
+        self.assertRegex(
+            force_str(response.content),
+            '(<option value="1" selected="selected">%s</option>|<option value="1" selected>%s</option>)'
+            % (self.ns_app_1, self.ns_app_1),
         )
         self.assertContains(response, 'id="id_published"')
 
         self.ns_app_1.app_data.config.published_default = True
         self.ns_app_1.save()
         response = admin_instance.add_view(request)
         response.render()
-        self.assertRegexpMatches(
-            force_text(response.content),
-            '(checked id="id_published"|id="id_published" checked|<input checked="checked" id="id_published")'
+        self.assertRegex(
+            force_str(response.content),
+            '(checked id="id_published"|id="id_published" checked|<input checked="checked" id="id_published")',
         )
 
     def test_templatetag(self):
-        article = Article.objects.create(title='news_1_app_1_config1',
-                                         slug='news_1_app_1_config1',
-                                         section=self.ns_app_1)
+        article = Article.objects.create(
+            title="news_1_app_1_config1",
+            slug="news_1_app_1_config1",
+            section=self.ns_app_1,
+        )
 
         request = self.get_page_request(self.page_1, self.user)
-        context = RequestContext(request, {'object': article, 'current_app': self.ns_app_1.namespace})
+        context = RequestContext(request, {"object": article, "current_app": self.ns_app_1.namespace})
 
         template = Template('{% load apphooks_config_tags %}{% namespace_url "example_detail" object.slug %}')
         response = template.render(context)
-        self.assertEqual(response, os.path.join(self.page_1.get_absolute_url(), article.slug, ''))
+        self.assertEqual(response, os.path.join(self.page_1.get_absolute_url(), article.slug, ""))
 
         template = Template('{% load apphooks_config_tags %}{% namespace_url "example_detail" slug=object.slug %}')
         response = template.render(context)
-        self.assertEqual(response, os.path.join(self.page_1.get_absolute_url(), article.slug, ''))
+        self.assertEqual(response, os.path.join(self.page_1.get_absolute_url(), article.slug, ""))
 
         template = Template('{% load apphooks_config_tags %}{% namespace_url "example_list" %}')
         response = template.render(context)
         self.assertEqual(response, self.page_1.get_absolute_url())
 
         request = self.get_page_request(self.page_2, self.user)
-        context = RequestContext(request, {'object': article, 'current_app': self.ns_app_2.namespace})
+        context = RequestContext(request, {"object": article, "current_app": self.ns_app_2.namespace})
         template = Template('{% load apphooks_config_tags %}{% namespace_url "example_list" %}')
         response = template.render(context)
         self.assertEqual(response, self.page_2.get_absolute_url())
 
     def test_apphook_field_name_discovery(self):
         field_names = get_apphook_field_names(Article)
-        self.assertEqual(field_names, ['section'])
+        self.assertEqual(field_names, ["section"])
 
         field_names = get_apphook_field_names(TranslatableArticle)
-        self.assertEqual(field_names, ['section'])
+        self.assertEqual(field_names, ["section"])
 
         field_names = get_apphook_field_names(News)
-        self.assertEqual(set(field_names), set(['config', 'section']))
+        self.assertEqual(set(field_names), {"config", "section"})
 
         field_names = get_apphook_field_names(NotApphookedModel)
         self.assertEqual(field_names, [])
 
     def test_apphook_field_name_discovery_from_objects(self):
         field_names = get_apphook_field_names(Article())
-        self.assertEqual(field_names, ['section'])
+        self.assertEqual(field_names, ["section"])
 
         field_names = get_apphook_field_names(TranslatableArticle())
-        self.assertEqual(field_names, ['section'])
+        self.assertEqual(field_names, ["section"])
 
         field_names = get_apphook_field_names(News())
-        self.assertEqual(set(field_names), set(['config', 'section']))
+        self.assertEqual(set(field_names), {"config", "section"})
 
         field_names = get_apphook_field_names(NotApphookedModel())
         self.assertEqual(field_names, [])
 
     def test_apphook_config_objects_discovery(self):
         obj = Article(section=self.ns_app_1)
         configs = get_apphook_configs(obj)
@@ -456,12 +454,12 @@
 
         obj = TranslatableArticle(section=self.ns_app_1)
         configs = get_apphook_configs(obj)
         self.assertEqual(configs, [self.ns_app_1])
 
         obj = News(section=self.ns_app_1, config=self.ns_app_3)
         configs = get_apphook_configs(obj)
-        self.assertEqual(set(configs), set([self.ns_app_1, self.ns_app_3]))
+        self.assertEqual(set(configs), {self.ns_app_1, self.ns_app_3})
 
         obj = NotApphookedModel()
         configs = get_apphook_configs(obj)
         self.assertEqual(configs, [])
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/cms_appconfig.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/cms_appconfig.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
+from app_data import AppDataForm
 from django import forms
 from django.db import models
 
-from app_data import AppDataForm
-
 from aldryn_apphooks_config.models import AppHookConfig
 from aldryn_apphooks_config.utils import setup_config
 
 
 class ExampleConfig(AppHookConfig):
     """Adds some translatable, per-app-instance fields."""
-    app_title = models.CharField('application title', max_length=234)
+
+    app_title = models.CharField("application title", max_length=234)
 
 
 class AnotherExampleConfig(AppHookConfig):
     max_entries = models.SmallIntegerField(default=5)
 
 
 @setup_config
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/migrations/0002_auto_20191012_2339.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/migrations/0002_auto_20191012_2339.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# -*- coding: utf-8 -*-
 # Generated by Django 1.11.25 on 2019-10-12 21:39
-from __future__ import unicode_literals
 
-from django.db import migrations
 import django.db.models.deletion
 import parler.fields
+from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('example', '0001_initial'),
+        ("example", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='translatablearticletranslation',
-            name='master',
-            field=parler.fields.TranslationsForeignKey(editable=False, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='translations', to='example.TranslatableArticle'),
+            model_name="translatablearticletranslation",
+            name="master",
+            field=parler.fields.TranslationsForeignKey(
+                editable=False,
+                null=True,
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name="translations",
+                to="example.TranslatableArticle",
+            ),
         ),
     ]
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/tests/utils/example/views.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/tests/utils/example/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
 from django.views.generic import DetailView, ListView
 
 from aldryn_apphooks_config.mixins import AppConfigMixin
 
 from .models import Article
 
 
 class ArticleDetail(AppConfigMixin, DetailView):
     model = Article
-    slug_field = 'slug'
+    slug_field = "slug"
 
     def get_template_names(self):
-        return '%s/article_detail.html' % self.config.namespace
+        return "%s/article_detail.html" % self.config.namespace
 
 
 class ArticleList(AppConfigMixin, ListView):
     """A complete list of articles."""
+
     model = Article
 
     def get_template_names(self):
-        return '%s/article_list.html' % self.config.namespace
+        return "%s/article_list.html" % self.config.namespace
 
     def get_queryset(self):
-        return Article.objects.all().filter(
-            section__namespace=self.namespace
-        )
+        return Article.objects.all().filter(section__namespace=self.namespace)
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config/utils.py` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
+from app_data import AppDataContainer, app_registry
+from cms.apphook_pool import apphook_pool
 from django.db.models import ForeignKey
 from django.urls import Resolver404, resolve
 from django.utils.translation import get_language_from_request, override
 
-from cms.apphook_pool import apphook_pool
-
-from app_data import AppDataContainer, app_registry
-
 # making key app/model specific to avoid inheritance issues
-APP_CONFIG_FIELDS_KEY = '_app_config_field_names_{app_label}_{model_name}'
+APP_CONFIG_FIELDS_KEY = "_app_config_field_names_{app_label}_{model_name}"
 
 
 def get_app_instance(request):
     """
     Returns a tuple containing the current namespace and the AppHookConfig instance
 
     :param request: request object
     :return: namespace, config
     """
     app = None
-    if getattr(request, 'current_page', None) and request.current_page.application_urls:
+    if getattr(request, "current_page", None) and request.current_page.application_urls:
         app = apphook_pool.get_apphook(request.current_page.application_urls)
     if app and app.app_config:
         try:
             config = None
             with override(get_language_from_request(request, check_path=True)):
                 namespace = resolve(request.path_info).namespace
                 config = app.get_config(namespace)
             return namespace, config
         except Resolver404:
             pass
-    return '', None
+    return "", None
 
 
 def setup_config(form_class, config_model=None):
     """
     Register the provided form as config form for the provided config model
 
     This can be used as a decorator by adding a `model` attribute to the config form::
@@ -49,40 +44,38 @@
     :param config_model: Model class derived from AppHookConfig
     :return:
     """
     # allow use as a decorator
     if config_model is None:
         return setup_config(form_class, form_class.model)
 
-    app_registry.register('config', AppDataContainer.from_form(form_class), config_model)
+    app_registry.register("config", AppDataContainer.from_form(form_class), config_model)
 
 
 def _get_apphook_field_names(model):
     """
     Return all foreign key field names for a AppHookConfig based model
     """
     from .models import AppHookConfig  # avoid circular dependencies
+
     fields = []
     for field in model._meta.fields:
         if isinstance(field, ForeignKey) and issubclass(field.remote_field.model, AppHookConfig):
             fields.append(field)
     return [field.name for field in fields]
 
 
 def get_apphook_field_names(model):
     """
     Cache app-hook field names on model
 
     :param model: model class or object
     :return: list of foreign key field names to AppHookConfigs
     """
-    key = APP_CONFIG_FIELDS_KEY.format(
-        app_label=model._meta.app_label,
-        model_name=model._meta.object_name
-    ).lower()
+    key = APP_CONFIG_FIELDS_KEY.format(app_label=model._meta.app_label, model_name=model._meta.object_name).lower()
     if not hasattr(model, key):
         field_names = _get_apphook_field_names(model)
         setattr(model, key, field_names)
     return getattr(model, key)
 
 
 def get_apphook_configs(obj):
```

### Comparing `aldryn-apphooks-config-0.6.0/aldryn_apphooks_config.egg-info/PKG-INFO` & `aldryn-apphooks-config-0.7.0/aldryn_apphooks_config.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,206 +1,334 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aldryn-apphooks-config
-Version: 0.6.0
+Version: 0.7.0
 Summary: Namespaces based configuration for Apphooks
 Home-page: https://github.com/aldryn/aldryn-apphooks-config
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.it
 License: BSD
-Description: |PyPI Version| |Build Status| |Coverage Status|
-        
-        ======================
-        aldryn-apphooks-config
-        ======================
-        
-        Namespaces based configuration for Apphooks
-        
-        Basic concepts
-        ==============
-        
-        The concept of apphooks-config is to store all the configuration
-        in an applications-specific model, and let the developer
-        specify the desired option in a form.
-        In the views the model instance specific for the current
-        application namespace is loaded (through a mixin) and it's
-        thus available in the view to provide the configuration for
-        the current namespace.
-        
-        Namespaces can be created on the fly in the ``Page`` admin
-        **Advanced settings** by following the steps above.
-        When creating an application configuration, you are in fact defining a
-        namespace, which is saved in the same field in the ``Page`` model as the
-        plain namespaces.
-        
-        
-        Contributing
-        ------------
-        
-        We're grateful to all contributors who have helped create and maintain this package.
-        
-        Contributors are listed at `contributions page
-        <https://github.com/divio/aldryn-apphooks-config/graphs/contributors>`_.
-        
-        
-        Supported versions
-        -----------------------------
-        
-        Python: 3.5, 3.6, 3.7, 3.8
-        Django: 1.11, 2.2, 3.0
-        django CMS: 3.5, 3.6, 3.7
-        
-        
-        Implementation step-guide
-        =========================
-        
-        * Define a AppHookConfig model in ``cms_appconfig.py``::
-        
-            from aldryn_apphooks_config.models import AppHookConfig
-        
-            class NewsBlogConfig(AppHookConfig):
-                pass
-        
-          Implementation can be completely empty as the schema is defined in the
-          parent (abstract) model
-        
-        * Use apphooks managers in your model::
-        
-            from aldryn_apphooks_config.managers import AppHookConfigManager
-        
-            class Article(models.Model):
-                title = models.CharField()
-        
-                objects = AppHookConfigManager()
-        
-        ``AppHookConfigManager`` adds ``namespace`` method to manager and queryset::
-        
-            Article.objects.namespace('foobar')
-        
-        There is also a proper queryset, the ``ApphooksConfigQueryset``. Parler
-        integrated variants can be found in ``aldryn_apphooks_config.managers.parler``.
-        Names are ``AppHookConfigTranslatableManager`` and
-        ``AppHookConfigTranslatableQueryset``.
-        
-        * Define a ConfigForm in ``cms_appconfig.py``::
-        
-            from app_data import AppDataForm
-            from django import forms
-            from aldryn_newsblog.models import NewsBlogConfig
-            from aldryn_apphooks_config.utils import setup_config
-        
-            class BlogOptionForm(AppDataForm):
-                # fields are totally arbitrary: any form field supported by
-                # django-appdata is supported
-                show_authors = forms.BooleanField(required=False)
-                ...
-        
-            # this function will register the provided form with the model created
-            # at the above step
-            setup_config(BlogOptionForm, NewsBlogConfig)
-        
-            # setup_config can be used as a decorator too, but the `model`
-            # attribute must be added to the form class
-            @setup_config
-            class BlogOptionForm(AppDataForm):
-                model = NewsBlogConfig
-        
-        
-        
-        
-        * Define an admin class for the AppHookConfig model (usually in ``admin.py``::
-        
-            from django.contrib import admin
-            from aldryn_apphooks_config.admin import BaseAppHookConfig
-        
-            class BlogConfigAdmin(BaseAppHookConfig):
-        
-                def get_config_fields(self):
-                    # this method **must** be implemented and **must** return the
-                    # fields defined in the above form, with the ``config`` prefix
-                    # This is dependent on the django-appdata API
-                    return ('config.show_authors', ...)
-        
-        * Define a CMSApp derived from CMSConfigApp provided by this application
-          (in ``cms_app.py``/``cms_apps.py``)::
-        
-            from aldryn_apphooks_config.app_base import CMSConfigApp
-            from cms.apphook_pool import apphook_pool
-            from django.utils.translation import ugettext_lazy as _
-            from .models import NewsBlogConfig
-        
-        
-            class NewsBlogApp(CMSConfigApp):
-                name = _('NewsBlogApp')
-                urls = ['aldryn_newsblog.urls']
-                app_name = 'aldryn_newsblog'
-                # this option is specific of CMSConfigApp, and links the
-                # CMSApp to a specific AppHookConfig model
-                app_config = NewsBlogConfig
-        
-            apphook_pool.register(NewsBlogApp)
-        
-        * Implements your views inheriting the ``AppConfigMixin``::
-        
-            from django.views.generic.detail import DetailView
-            from aldryn_apphooks_config.mixins import AppConfigMixin
-        
-            class ArticleDetail(AppConfigMixin, DetailView):
-                def get_queryset(self):
-                    return Article.objects.namespace(self.namespace)
-        
-          ``AppConfigMixin`` provides a complete support to namespaces, so the view
-          is not required to set anything specific to support them; the following
-          attributes are set for the view class instance:
-        
-          * current namespace in ``self.namespace``
-          * namespace configuration (the instance of NewsBlogConfig) in ``self.config``
-          * current application in the ``current_app`` parameter passed to the
-            Response class
-        
-        Test setup
-        ==========
-        
-        To properly setup the data for tests to run for a apphook-config enabled application,
-        make sure you add the following code to your TestCase::
-        
-            MyTestCase():
-        
-                def setUp(self):
-                    # This is the namespace represented by the AppHookConfig model instance
-                    self.ns_newsblog = NewsBlogConfig.objects.create(namespace='NBNS')
-                    self.page = api.create_page(
-                        'page', self.template, self.language, published=True,
-                        # this is the name of the apphook defined in the CMSApp class
-                        apphook='NewsBlogApp',
-                        # The namespace is the namespace field of the AppHookConfig instance created above
-                        apphook_namespace=self.ns_newsblog.namespace)
-                    # publish the page to make the apphook available
-                    self.page.publish(self.language)
-        
-        
-        .. |PyPI Version| image:: http://img.shields.io/pypi/v/aldryn-apphooks-config.svg
-           :target: https://pypi.python.org/pypi/aldryn-apphooks-config
-        .. |Build Status| image:: http://img.shields.io/travis/aldryn/aldryn-apphooks-config/master.svg
-           :target: https://travis-ci.org/aldryn/aldryn-apphooks-config
-        .. |Coverage Status| image:: http://img.shields.io/coveralls/aldryn/aldryn-apphooks-config/master.svg
-           :target: https://coveralls.io/r/aldryn/aldryn-apphooks-config?branch=master
-        
-Keywords: aldryn-apphooks-config
-Platform: UNKNOWN
+Project-URL: Documentation, https://aldryn-apphooks-config.readthedocs.io/
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+|PyPI Version| |Coverage Status|
+
+======================
+aldryn-apphooks-config
+======================
+
+Namespaces based configuration for Apphooks
+
+Basic concepts
+==============
+
+The concept of apphooks-config is to store all the configuration
+in an applications-specific model, and let the developer
+specify the desired option in a form.
+In the views the model instance specific for the current
+application namespace is loaded (through a mixin) and it's
+thus available in the view to provide the configuration for
+the current namespace.
+
+Namespaces can be created on the fly in the ``Page`` admin
+**Advanced settings** by following the steps above.
+When creating an application configuration, you are in fact defining a
+namespace, which is saved in the same field in the ``Page`` model as the
+plain namespaces.
+
+
+Contributing
+------------
+
+We're grateful to all contributors who have helped create and maintain this package.
+
+Contributors are listed at `contributions page
+<https://github.com/divio/aldryn-apphooks-config/graphs/contributors>`_.
+
+
+Supported versions
+-----------------------------
+
+Python: 3.9 - 3.11
+Django: 3.2 - 4.2
+django CMS: 3.9 - 3.11
+
+
+Implementation step-guide
+=========================
+
+* Define a AppHookConfig model in ``cms_appconfig.py``::
+
+    from aldryn_apphooks_config.models import AppHookConfig
+
+    class NewsBlogConfig(AppHookConfig):
+        pass
+
+  Implementation can be completely empty as the schema is defined in the
+  parent (abstract) model
+
+* Use apphooks managers in your model::
+
+    from aldryn_apphooks_config.managers import AppHookConfigManager
+
+    class Article(models.Model):
+        title = models.CharField()
+
+        objects = AppHookConfigManager()
+
+``AppHookConfigManager`` adds ``namespace`` method to manager and queryset::
+
+    Article.objects.namespace('foobar')
+
+There is also a proper queryset, the ``ApphooksConfigQueryset``. Parler
+integrated variants can be found in ``aldryn_apphooks_config.managers.parler``.
+Names are ``AppHookConfigTranslatableManager`` and
+``AppHookConfigTranslatableQueryset``.
+
+* Define a ConfigForm in ``cms_appconfig.py``::
+
+    from app_data import AppDataForm
+    from django import forms
+    from aldryn_newsblog.models import NewsBlogConfig
+    from aldryn_apphooks_config.utils import setup_config
+
+    class BlogOptionForm(AppDataForm):
+        # fields are totally arbitrary: any form field supported by
+        # django-appdata is supported
+        show_authors = forms.BooleanField(required=False)
+        ...
+
+    # this function will register the provided form with the model created
+    # at the above step
+    setup_config(BlogOptionForm, NewsBlogConfig)
+
+    # setup_config can be used as a decorator too, but the `model`
+    # attribute must be added to the form class
+    @setup_config
+    class BlogOptionForm(AppDataForm):
+        model = NewsBlogConfig
+
+
+
+
+* Define an admin class for the AppHookConfig model (usually in ``admin.py``::
+
+    from django.contrib import admin
+    from aldryn_apphooks_config.admin import BaseAppHookConfig
+
+    class BlogConfigAdmin(BaseAppHookConfig):
+
+        def get_config_fields(self):
+            # this method **must** be implemented and **must** return the
+            # fields defined in the above form, with the ``config`` prefix
+            # This is dependent on the django-appdata API
+            return ('config.show_authors', ...)
+
+* Define a CMSApp derived from CMSConfigApp provided by this application
+  (in ``cms_app.py``/``cms_apps.py``)::
+
+    from aldryn_apphooks_config.app_base import CMSConfigApp
+    from cms.apphook_pool import apphook_pool
+    from django.utils.translation import ugettext_lazy as _
+    from .models import NewsBlogConfig
+
+
+    class NewsBlogApp(CMSConfigApp):
+        name = _('NewsBlogApp')
+        urls = ['aldryn_newsblog.urls']
+        app_name = 'aldryn_newsblog'
+        # this option is specific of CMSConfigApp, and links the
+        # CMSApp to a specific AppHookConfig model
+        app_config = NewsBlogConfig
+
+    apphook_pool.register(NewsBlogApp)
+
+* Implements your views inheriting the ``AppConfigMixin``::
+
+    from django.views.generic.detail import DetailView
+    from aldryn_apphooks_config.mixins import AppConfigMixin
+
+    class ArticleDetail(AppConfigMixin, DetailView):
+        def get_queryset(self):
+            return Article.objects.namespace(self.namespace)
+
+  ``AppConfigMixin`` provides a complete support to namespaces, so the view
+  is not required to set anything specific to support them; the following
+  attributes are set for the view class instance:
+
+  * current namespace in ``self.namespace``
+  * namespace configuration (the instance of NewsBlogConfig) in ``self.config``
+  * current application in the ``current_app`` parameter passed to the
+    Response class
+
+Test setup
+==========
+
+To properly setup the data for tests to run for a apphook-config enabled application,
+make sure you add the following code to your TestCase::
+
+    MyTestCase():
+
+        def setUp(self):
+            # This is the namespace represented by the AppHookConfig model instance
+            self.ns_newsblog = NewsBlogConfig.objects.create(namespace='NBNS')
+            self.page = api.create_page(
+                'page', self.template, self.language, published=True,
+                # this is the name of the apphook defined in the CMSApp class
+                apphook='NewsBlogApp',
+                # The namespace is the namespace field of the AppHookConfig instance created above
+                apphook_namespace=self.ns_newsblog.namespace)
+            # publish the page to make the apphook available
+            self.page.publish(self.language)
+
+
+.. |PyPI Version| image:: http://img.shields.io/pypi/v/aldryn-apphooks-config.svg
+   :target: https://pypi.python.org/pypi/aldryn-apphooks-config
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/divio/aldryn-apphooks-config/test.yml?style=flat-square
+   :target: https://github.com/divio/aldryn-apphooks-config/actions/workflows/test.yml
+.. |Coverage Status| image:: http://img.shields.io/coveralls/aldryn/aldryn-apphooks-config/master.svg
+   :target: https://coveralls.io/r/aldryn/aldryn-apphooks-config?branch=master
+
+Changelog
+=========
+
+
+0.7.0 (2023-05-07)
+==================
+
+* Add Django 3.2+ support
+
+0.6.0 (2020-05-12)
+==================
+
+* Add Django 3.0 support
+
+0.5.3 (2019-10-19)
+==================
+
+* Fix media asset declaration on django 2.2+
+
+0.5.2 (2019-01-02)
+==================
+
+* Changed deprecated ``rel.to`` to ``remote_field.model``
+* Fixed migration for example app
+* Fixed issues for Django 2.0 and up
+
+
+0.5.1 (2018-12-18)
+==================
+
+* Added support for Django 2.0 and 2.1
+* Removed support for Django < 1.11
+* Adapted testing infrastructure (tox/travis) to incorporate django CMS 3.6
+* Fixed setup.py
+
+
+0.4.2 (2018-12-17)
+==================
+
+* Fixed issue with Django 1.10 and below in AppHookConfigWidget
+
+
+0.4.1 (2018-04-10)
+==================
+
+* django-appdata>=0.2.0 is now required
+
+
+0.4.0 (2018-03-19)
+==================
+
+* Added Django 1.11 compatibility
+* Added django CMS 3.5 compatibility
+* Implemented django-appdata 0.2 interface
+* Removed south migrations
+* Dropped support for django CMS 3.3 and below
+* Allowed use setup_config as decorators
+
+
+0.3.3 (2017-03-06)
+==================
+
+* Fixed MANIFEST.in typo
+
+
+0.3.2 (2017-03-06)
+==================
+
+* Fixed setup.py issue
+* Added locale files to MANIFEST.in
+
+
+0.3.1 (2017-03-02)
+==================
+
+* Added translation system
+* Added german translation
+
+
+0.3.0 (2017-01-06)
+==================
+
+* Allowed override AppHookConfigField attributes
+* Dropped Django 1.7 and below
+* Dropped django CMS 3.1 and below
+* Added Django 1.10 support
+
+
+0.2.7 (2016-03-03)
+==================
+
+* Set namespace as readonly
+* Added official Django 1.9 support
+* Updated readme
+* Used path_info instead of path in resolve
+
+
+0.2.6 (2015-10-05)
+==================
+
+* Added support for Python 3.5
+* Added support for Django 1.9a1
+* Code style cleanup and tests
+
+
+0.2.5 (2015-09-25)
+==================
+
+* Added support for Django 1.8, django CMS 3.2
+* AppHookConfigTranslatableManager.get_queryset should use queryset_class
+* Skipped overriding admin form if app_config field not present
+
+
+0.2.4 (2015-04-20)
+==================
+
+* Fixed issue where an apphook could not be changed, once set.
+* Added optional 'default' kwarg to namespace_url templatetag
+
+
+0.1.0 (2014-01-01)
+==================
+
+* Released first version on PyPI.
```

