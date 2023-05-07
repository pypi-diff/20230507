# Comparing `tmp/django-data-browser-4.1.0.tar.gz` & `tmp/django-data-browser-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-data-browser-4.1.0.tar", last modified: Mon May  1 19:30:11 2023, max compression
+gzip compressed data, was "django-data-browser-4.1.1.tar", last modified: Sun May  7 09:31:28 2023, max compression
```

## Comparing `django-data-browser-4.1.0.tar` & `django-data-browser-4.1.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.833860 django-data-browser-4.1.0/
--rw-rw-rw-   0        0        0     1885 2023-03-30 21:24:18.000000 django-data-browser-4.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0    14913 2021-12-12 20:01:39.000000 django-data-browser-4.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1522 2020-03-29 21:09:45.000000 django-data-browser-4.1.0/LICENSE
--rw-rw-rw-   0        0        0      605 2022-01-04 07:58:07.000000 django-data-browser-4.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    61435 2023-05-01 19:30:11.832863 django-data-browser-4.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    60312 2023-05-01 19:29:28.000000 django-data-browser-4.1.0/README.rst
--rw-rw-rw-   0        0        0      508 2021-09-26 12:42:44.000000 django-data-browser-4.1.0/build.sh
--rw-rw-rw-   0        0        0      243 2020-10-18 11:05:29.000000 django-data-browser-4.1.0/build_fe.sh
--rw-rw-rw-   0        0        0      209 2020-11-28 10:32:50.000000 django-data-browser-4.1.0/build_whl.sh
--rw-rw-rw-   0        0        0      105 2020-10-18 11:05:29.000000 django-data-browser-4.1.0/clean.sh
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.715178 django-data-browser-4.1.0/data_browser/
--rw-rw-rw-   0        0        0       18 2023-05-01 19:29:34.000000 django-data-browser-4.1.0/data_browser/__init__.py
--rw-rw-rw-   0        0        0     1741 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/data_browser/admin.py
--rw-rw-rw-   0        0        0     5338 2023-05-01 18:59:01.000000 django-data-browser-4.1.0/data_browser/api.py
--rw-rw-rw-   0        0        0      206 2022-02-07 19:45:31.000000 django-data-browser-4.1.0/data_browser/apps.py
--rw-rw-rw-   0        0        0     3142 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/data_browser/common.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.718169 django-data-browser-4.1.0/data_browser/fe_build/
--rw-rw-rw-   0        0        0      374 2023-05-01 19:30:00.000000 django-data-browser-4.1.0/data_browser/fe_build/asset-manifest.json
--rw-rw-rw-   0        0        0     2400 2023-05-01 19:30:00.000000 django-data-browser-4.1.0/data_browser/fe_build/index.html
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.657333 django-data-browser-4.1.0/data_browser/fe_build/static/
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.719167 django-data-browser-4.1.0/data_browser/fe_build/static/css/
--rw-rw-rw-   0        0        0     7039 2023-05-01 19:30:00.000000 django-data-browser-4.1.0/data_browser/fe_build/static/css/main.6e6fbe98.css
--rw-rw-rw-   0        0        0    10284 2023-05-01 19:30:00.000000 django-data-browser-4.1.0/data_browser/fe_build/static/css/main.6e6fbe98.css.map
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.728143 django-data-browser-4.1.0/data_browser/fe_build/static/js/
--rw-rw-rw-   0        0        0   327813 2023-05-01 19:30:00.000000 django-data-browser-4.1.0/data_browser/fe_build/static/js/main.b4d189f0.js
--rw-rw-rw-   0        0        0     1447 2023-05-01 19:30:00.000000 django-data-browser-4.1.0/data_browser/fe_build/static/js/main.b4d189f0.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1220114 2023-05-01 19:30:00.000000 django-data-browser-4.1.0/data_browser/fe_build/static/js/main.b4d189f0.js.map
--rw-rw-rw-   0        0        0     1741 2021-03-13 16:54:43.000000 django-data-browser-4.1.0/data_browser/format_csv.py
--rw-rw-rw-   0        0        0     5819 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/helpers.py
--rw-rw-rw-   0        0        0     2574 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/data_browser/migration_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.750084 django-data-browser-4.1.0/data_browser/migrations/
--rw-rw-rw-   0        0        0     1629 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      536 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/migrations/0002_auto_20200331_1842.py
--rw-rw-rw-   0        0        0      263 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/migrations/0003_remove_view_app.py
--rw-rw-rw-   0        0        0      325 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/migrations/0004_auto_20200501_0903.py
--rw-rw-rw-   0        0        0      463 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/migrations/0005_auto_20200516_1726.py
--rw-rw-rw-   0        0        0      592 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/migrations/0006_auto_20200531_1450.py
--rw-rw-rw-   0        0        0      440 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/migrations/0007_view_public_slug.py
--rw-rw-rw-   0        0        0      344 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/migrations/0008_view_limit.py
--rw-rw-rw-   0        0        0      469 2020-12-01 19:24:08.000000 django-data-browser-4.1.0/data_browser/migrations/0009_migrate_saved_views.py
--rw-rw-rw-   0        0        0      350 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/data_browser/migrations/0010_shared.py
--rw-rw-rw-   0        0        0      502 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/data_browser/migrations/0011_folder.py
--rw-rw-rw-   0        0        0      529 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/data_browser/migrations/0012_can_share.py
--rw-rw-rw-   0        0        0        0 2020-03-31 16:35:44.000000 django-data-browser-4.1.0/data_browser/migrations/__init__.py
--rw-rw-rw-   0        0        0     2657 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/data_browser/models.py
--rw-rw-rw-   0        0        0    15088 2023-03-30 21:24:18.000000 django-data-browser-4.1.0/data_browser/orm_admin.py
--rw-rw-rw-   0        0        0     3923 2023-03-06 07:51:43.000000 django-data-browser-4.1.0/data_browser/orm_aggregates.py
--rw-rw-rw-   0        0        0     2471 2021-12-31 10:44:42.000000 django-data-browser-4.1.0/data_browser/orm_debug.py
--rw-rw-rw-   0        0        0     8291 2023-04-30 12:59:04.000000 django-data-browser-4.1.0/data_browser/orm_fields.py
--rw-rw-rw-   0        0        0     4992 2023-03-30 22:40:08.000000 django-data-browser-4.1.0/data_browser/orm_functions.py
--rw-rw-rw-   0        0        0     1729 2022-01-03 10:46:07.000000 django-data-browser-4.1.0/data_browser/orm_lookups.py
--rw-rw-rw-   0        0        0     9368 2023-04-05 21:52:54.000000 django-data-browser-4.1.0/data_browser/orm_results.py
--rw-rw-rw-   0        0        0     3525 2023-03-30 22:40:08.000000 django-data-browser-4.1.0/data_browser/orm_types.py
--rw-rw-rw-   0        0        0     9111 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/data_browser/query.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.658330 django-data-browser-4.1.0/data_browser/templates/
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.751082 django-data-browser-4.1.0/data_browser/templates/data_browser/
--rw-rw-rw-   0        0        0     2400 2023-05-01 19:30:00.000000 django-data-browser-4.1.0/data_browser/templates/data_browser/index.html
--rw-rw-rw-   0        0        0    16949 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/data_browser/types.py
--rw-rw-rw-   0        0        0     1684 2021-12-31 10:46:26.000000 django-data-browser-4.1.0/data_browser/urls.py
--rw-rw-rw-   0        0        0      349 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/data_browser/util.py
--rw-rw-rw-   0        0        0    13143 2023-05-01 18:59:45.000000 django-data-browser-4.1.0/data_browser/views.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.760058 django-data-browser-4.1.0/data_browser/web_root/
--rw-rw-rw-   0        0        0     5221 2020-07-01 20:11:06.000000 django-data-browser-4.1.0/data_browser/web_root/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    17683 2020-07-01 20:11:06.000000 django-data-browser-4.1.0/data_browser/web_root/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     4613 2020-07-01 20:11:06.000000 django-data-browser-4.1.0/data_browser/web_root/apple-touch-icon.png
--rw-rw-rw-   0        0        0      333 2020-07-01 20:11:06.000000 django-data-browser-4.1.0/data_browser/web_root/favicon-16x16.png
--rw-rw-rw-   0        0        0      648 2020-07-01 20:11:06.000000 django-data-browser-4.1.0/data_browser/web_root/favicon-32x32.png
--rw-rw-rw-   0        0        0    15406 2020-07-01 20:11:06.000000 django-data-browser-4.1.0/data_browser/web_root/favicon.ico
--rw-rw-rw-   0        0        0      424 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/data_browser/web_root/site.webmanifest
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.766041 django-data-browser-4.1.0/django_data_browser.egg-info/
--rw-rw-rw-   0        0        0    61435 2023-05-01 19:30:11.000000 django-data-browser-4.1.0/django_data_browser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3438 2023-05-01 19:30:11.000000 django-data-browser-4.1.0/django_data_browser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 19:30:11.000000 django-data-browser-4.1.0/django_data_browser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-01 19:30:11.000000 django-data-browser-4.1.0/django_data_browser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 19:30:11.000000 django-data-browser-4.1.0/django_data_browser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.771028 django-data-browser-4.1.0/frontend/
--rw-rw-rw-   0        0        0     2891 2020-04-22 19:19:40.000000 django-data-browser-4.1.0/frontend/README.md
--rw-rw-rw-   0        0        0  1009738 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/frontend/package-lock.json
--rw-rw-rw-   0        0        0     1000 2022-04-10 12:41:54.000000 django-data-browser-4.1.0/frontend/package.json
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.773023 django-data-browser-4.1.0/frontend/public/
--rw-rw-rw-   0        0        0     3304 2023-03-06 21:38:15.000000 django-data-browser-4.1.0/frontend/public/index.html
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.791973 django-data-browser-4.1.0/frontend/src/
--rw-rw-rw-   0        0        0     1298 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/frontend/src/App.js
--rw-rw-rw-   0        0        0     7309 2023-05-01 19:00:32.000000 django-data-browser-4.1.0/frontend/src/App.scss
--rw-rw-rw-   0        0        0      280 2020-04-22 19:19:40.000000 django-data-browser-4.1.0/frontend/src/App.test.js
--rw-rw-rw-   0        0        0       85 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/frontend/src/Config.js
--rw-rw-rw-   0        0        0     2678 2021-12-29 21:35:30.000000 django-data-browser-4.1.0/frontend/src/ContextMenu.js
--rw-rw-rw-   0        0        0      551 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/frontend/src/CurrentSavedView.js
--rw-rw-rw-   0        0        0     4278 2023-05-01 19:00:44.000000 django-data-browser-4.1.0/frontend/src/HomePage.js
--rw-rw-rw-   0        0        0     9454 2023-05-01 18:59:45.000000 django-data-browser-4.1.0/frontend/src/Query.js
--rw-rw-rw-   0        0        0      144 2020-06-27 10:10:01.000000 django-data-browser-4.1.0/frontend/src/Query.test.js
--rw-rw-rw-   0        0        0    14845 2023-05-01 18:59:45.000000 django-data-browser-4.1.0/frontend/src/QueryPage.js
--rw-rw-rw-   0        0        0     9360 2021-12-29 21:35:30.000000 django-data-browser-4.1.0/frontend/src/Results.js
--rw-rw-rw-   0        0        0     6645 2023-05-01 19:01:07.000000 django-data-browser-4.1.0/frontend/src/SavedViewPage.js
--rw-rw-rw-   0        0        0     1649 2021-12-30 00:35:29.000000 django-data-browser-4.1.0/frontend/src/Tooltip.js
--rw-rw-rw-   0        0        0    12431 2023-05-01 19:01:07.000000 django-data-browser-4.1.0/frontend/src/Util.js
--rw-rw-rw-   0        0        0      591 2021-12-12 20:01:39.000000 django-data-browser-4.1.0/frontend/src/WindowDimensions.js
--rw-rw-rw-   0        0        0      733 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/frontend/src/index.js
--rw-rw-rw-   0        0        0      366 2020-04-22 19:19:40.000000 django-data-browser-4.1.0/frontend/src/index.scss
--rw-rw-rw-   0        0        0     2671 2020-04-22 19:19:40.000000 django-data-browser-4.1.0/frontend/src/logo.svg
--rw-rw-rw-   0        0        0      255 2020-04-22 19:19:40.000000 django-data-browser-4.1.0/frontend/src/setupTests.js
--rw-rw-rw-   0        0        0     2837 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      260 2023-03-06 20:00:37.000000 django-data-browser-4.1.0/requirements.txt
--rw-rw-rw-   0        0        0   112598 2021-03-13 16:54:43.000000 django-data-browser-4.1.0/screenshot.png
--rw-rw-rw-   0        0        0       42 2023-05-01 19:30:11.834858 django-data-browser-4.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1092 2023-03-30 22:40:08.000000 django-data-browser-4.1.0/setup.py
--rw-rw-rw-   0        0        0    35837 2020-06-27 10:10:01.000000 django-data-browser-4.1.0/structure.svg
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.816905 django-data-browser-4.1.0/tests/
--rw-rw-rw-   0        0        0        0 2019-07-20 09:57:44.000000 django-data-browser-4.1.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.818900 django-data-browser-4.1.0/tests/array/
--rw-rw-rw-   0        0        0        0 2020-10-24 10:26:31.000000 django-data-browser-4.1.0/tests/array/__init__.py
--rw-rw-rw-   0        0        0      617 2021-12-31 10:07:16.000000 django-data-browser-4.1.0/tests/array/models.py
--rw-rw-rw-   0        0        0     2343 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.821893 django-data-browser-4.1.0/tests/core/
--rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.1.0/tests/core/__init__.py
--rw-rw-rw-   0        0        0     4422 2021-12-31 10:49:19.000000 django-data-browser-4.1.0/tests/core/admin.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.826879 django-data-browser-4.1.0/tests/core/migrations/
--rw-rw-rw-   0        0        0    10069 2023-03-06 08:08:57.000000 django-data-browser-4.1.0/tests/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2021-12-29 23:58:51.000000 django-data-browser-4.1.0/tests/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     4303 2021-12-31 10:48:59.000000 django-data-browser-4.1.0/tests/core/models.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.828873 django-data-browser-4.1.0/tests/json/
--rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.1.0/tests/json/__init__.py
--rw-rw-rw-   0        0        0       98 2023-03-30 22:40:08.000000 django-data-browser-4.1.0/tests/json/models.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:30:11.830869 django-data-browser-4.1.0/tests/snapshots/
--rw-rw-rw-   0        0        0        0 2020-06-27 10:10:01.000000 django-data-browser-4.1.0/tests/snapshots/__init__.py
--rw-rw-rw-   0        0        0   436829 2023-05-01 18:51:44.000000 django-data-browser-4.1.0/tests/snapshots/snap_test_views.py
--rw-rw-rw-   0        0        0     5231 2023-04-25 17:09:12.000000 django-data-browser-4.1.0/tests/test_admin.py
--rw-rw-rw-   0        0        0    20223 2023-05-01 18:59:01.000000 django-data-browser-4.1.0/tests/test_api.py
--rw-rw-rw-   0        0        0     7162 2022-02-07 21:31:16.000000 django-data-browser-4.1.0/tests/test_array_field.py
--rw-rw-rw-   0        0        0      919 2020-09-09 18:29:41.000000 django-data-browser-4.1.0/tests/test_common.py
--rw-rw-rw-   0        0        0     3693 2022-05-03 21:04:24.000000 django-data-browser-4.1.0/tests/test_helpers.py
--rw-rw-rw-   0        0        0     6081 2023-03-30 22:40:08.000000 django-data-browser-4.1.0/tests/test_json_field.py
--rw-rw-rw-   0        0        0     4483 2021-12-12 21:09:42.000000 django-data-browser-4.1.0/tests/test_migrations.py
--rw-rw-rw-   0        0        0     1240 2020-07-06 07:50:49.000000 django-data-browser-4.1.0/tests/test_models.py
--rw-rw-rw-   0        0        0    35026 2023-03-30 22:40:08.000000 django-data-browser-4.1.0/tests/test_orm.py
--rw-rw-rw-   0        0        0      878 2023-03-30 22:40:08.000000 django-data-browser-4.1.0/tests/test_orm_debug.py
--rw-rw-rw-   0        0        0    25081 2023-03-30 21:24:18.000000 django-data-browser-4.1.0/tests/test_query.py
--rw-rw-rw-   0        0        0      165 2020-10-22 20:32:07.000000 django-data-browser-4.1.0/tests/test_tests.py
--rw-rw-rw-   0        0        0    18139 2023-05-01 18:59:45.000000 django-data-browser-4.1.0/tests/test_views.py
--rw-rw-rw-   0        0        0      184 2020-10-22 18:16:38.000000 django-data-browser-4.1.0/tests/urls.py
--rw-rw-rw-   0        0        0      366 2023-03-30 21:24:18.000000 django-data-browser-4.1.0/tests/util.py
--rw-rw-rw-   0        0        0      574 2023-03-30 22:40:08.000000 django-data-browser-4.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.713739 django-data-browser-4.1.1/
+-rw-rw-rw-   0        0        0     1885 2023-03-30 21:24:18.000000 django-data-browser-4.1.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0    14913 2021-12-12 20:01:39.000000 django-data-browser-4.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1522 2020-03-29 21:09:45.000000 django-data-browser-4.1.1/LICENSE
+-rw-rw-rw-   0        0        0      605 2022-01-04 07:58:07.000000 django-data-browser-4.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    61701 2023-05-07 09:31:28.712741 django-data-browser-4.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    60576 2023-05-07 09:30:09.000000 django-data-browser-4.1.1/README.rst
+-rw-rw-rw-   0        0        0      508 2021-09-26 12:42:44.000000 django-data-browser-4.1.1/build.sh
+-rw-rw-rw-   0        0        0      243 2020-10-18 11:05:29.000000 django-data-browser-4.1.1/build_fe.sh
+-rw-rw-rw-   0        0        0      209 2020-11-28 10:32:50.000000 django-data-browser-4.1.1/build_whl.sh
+-rw-rw-rw-   0        0        0      105 2020-10-18 11:05:29.000000 django-data-browser-4.1.1/clean.sh
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.603034 django-data-browser-4.1.1/data_browser/
+-rw-rw-rw-   0        0        0       18 2023-05-07 09:30:21.000000 django-data-browser-4.1.1/data_browser/__init__.py
+-rw-rw-rw-   0        0        0     1741 2023-05-01 18:51:44.000000 django-data-browser-4.1.1/data_browser/admin.py
+-rw-rw-rw-   0        0        0     5338 2023-05-01 18:59:01.000000 django-data-browser-4.1.1/data_browser/api.py
+-rw-rw-rw-   0        0        0      206 2022-02-07 19:45:31.000000 django-data-browser-4.1.1/data_browser/apps.py
+-rw-rw-rw-   0        0        0     3287 2023-05-07 09:17:35.000000 django-data-browser-4.1.1/data_browser/common.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.604031 django-data-browser-4.1.1/data_browser/fe_build/
+-rw-rw-rw-   0        0        0      374 2023-05-07 09:31:20.000000 django-data-browser-4.1.1/data_browser/fe_build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2400 2023-05-07 09:31:20.000000 django-data-browser-4.1.1/data_browser/fe_build/index.html
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.561147 django-data-browser-4.1.1/data_browser/fe_build/static/
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.606026 django-data-browser-4.1.1/data_browser/fe_build/static/css/
+-rw-rw-rw-   0        0        0     7039 2023-05-07 09:31:20.000000 django-data-browser-4.1.1/data_browser/fe_build/static/css/main.6e6fbe98.css
+-rw-rw-rw-   0        0        0    10284 2023-05-07 09:31:20.000000 django-data-browser-4.1.1/data_browser/fe_build/static/css/main.6e6fbe98.css.map
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.610016 django-data-browser-4.1.1/data_browser/fe_build/static/js/
+-rw-rw-rw-   0        0        0   327813 2023-05-07 09:31:20.000000 django-data-browser-4.1.1/data_browser/fe_build/static/js/main.b4d189f0.js
+-rw-rw-rw-   0        0        0     1447 2023-05-07 09:31:20.000000 django-data-browser-4.1.1/data_browser/fe_build/static/js/main.b4d189f0.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1220114 2023-05-07 09:31:20.000000 django-data-browser-4.1.1/data_browser/fe_build/static/js/main.b4d189f0.js.map
+-rw-rw-rw-   0        0        0     1741 2021-03-13 16:54:43.000000 django-data-browser-4.1.1/data_browser/format_csv.py
+-rw-rw-rw-   0        0        0     5819 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/helpers.py
+-rw-rw-rw-   0        0        0     2574 2023-05-01 18:51:44.000000 django-data-browser-4.1.1/data_browser/migration_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.623978 django-data-browser-4.1.1/data_browser/migrations/
+-rw-rw-rw-   0        0        0     1629 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      536 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/migrations/0002_auto_20200331_1842.py
+-rw-rw-rw-   0        0        0      263 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/migrations/0003_remove_view_app.py
+-rw-rw-rw-   0        0        0      325 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/migrations/0004_auto_20200501_0903.py
+-rw-rw-rw-   0        0        0      463 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/migrations/0005_auto_20200516_1726.py
+-rw-rw-rw-   0        0        0      592 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/migrations/0006_auto_20200531_1450.py
+-rw-rw-rw-   0        0        0      440 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/migrations/0007_view_public_slug.py
+-rw-rw-rw-   0        0        0      344 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/migrations/0008_view_limit.py
+-rw-rw-rw-   0        0        0      469 2020-12-01 19:24:08.000000 django-data-browser-4.1.1/data_browser/migrations/0009_migrate_saved_views.py
+-rw-rw-rw-   0        0        0      350 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/data_browser/migrations/0010_shared.py
+-rw-rw-rw-   0        0        0      502 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/data_browser/migrations/0011_folder.py
+-rw-rw-rw-   0        0        0      529 2023-05-01 18:51:44.000000 django-data-browser-4.1.1/data_browser/migrations/0012_can_share.py
+-rw-rw-rw-   0        0        0        0 2020-03-31 16:35:44.000000 django-data-browser-4.1.1/data_browser/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2657 2023-05-01 18:51:44.000000 django-data-browser-4.1.1/data_browser/models.py
+-rw-rw-rw-   0        0        0    15088 2023-03-30 21:24:18.000000 django-data-browser-4.1.1/data_browser/orm_admin.py
+-rw-rw-rw-   0        0        0     3923 2023-03-06 07:51:43.000000 django-data-browser-4.1.1/data_browser/orm_aggregates.py
+-rw-rw-rw-   0        0        0     2471 2021-12-31 10:44:42.000000 django-data-browser-4.1.1/data_browser/orm_debug.py
+-rw-rw-rw-   0        0        0     8291 2023-04-30 12:59:04.000000 django-data-browser-4.1.1/data_browser/orm_fields.py
+-rw-rw-rw-   0        0        0     4992 2023-03-30 22:40:08.000000 django-data-browser-4.1.1/data_browser/orm_functions.py
+-rw-rw-rw-   0        0        0     1729 2022-01-03 10:46:07.000000 django-data-browser-4.1.1/data_browser/orm_lookups.py
+-rw-rw-rw-   0        0        0     9368 2023-04-05 21:52:54.000000 django-data-browser-4.1.1/data_browser/orm_results.py
+-rw-rw-rw-   0        0        0     3525 2023-03-30 22:40:08.000000 django-data-browser-4.1.1/data_browser/orm_types.py
+-rw-rw-rw-   0        0        0     9111 2023-05-01 18:51:44.000000 django-data-browser-4.1.1/data_browser/query.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.562144 django-data-browser-4.1.1/data_browser/templates/
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.625973 django-data-browser-4.1.1/data_browser/templates/data_browser/
+-rw-rw-rw-   0        0        0     2400 2023-05-07 09:31:21.000000 django-data-browser-4.1.1/data_browser/templates/data_browser/index.html
+-rw-rw-rw-   0        0        0    16949 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/data_browser/types.py
+-rw-rw-rw-   0        0        0     1684 2021-12-31 10:46:26.000000 django-data-browser-4.1.1/data_browser/urls.py
+-rw-rw-rw-   0        0        0      349 2023-05-01 18:51:44.000000 django-data-browser-4.1.1/data_browser/util.py
+-rw-rw-rw-   0        0        0    13143 2023-05-01 18:59:45.000000 django-data-browser-4.1.1/data_browser/views.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.634949 django-data-browser-4.1.1/data_browser/web_root/
+-rw-rw-rw-   0        0        0     5221 2020-07-01 20:11:06.000000 django-data-browser-4.1.1/data_browser/web_root/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    17683 2020-07-01 20:11:06.000000 django-data-browser-4.1.1/data_browser/web_root/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     4613 2020-07-01 20:11:06.000000 django-data-browser-4.1.1/data_browser/web_root/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      333 2020-07-01 20:11:06.000000 django-data-browser-4.1.1/data_browser/web_root/favicon-16x16.png
+-rw-rw-rw-   0        0        0      648 2020-07-01 20:11:06.000000 django-data-browser-4.1.1/data_browser/web_root/favicon-32x32.png
+-rw-rw-rw-   0        0        0    15406 2020-07-01 20:11:06.000000 django-data-browser-4.1.1/data_browser/web_root/favicon.ico
+-rw-rw-rw-   0        0        0      424 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/data_browser/web_root/site.webmanifest
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.645920 django-data-browser-4.1.1/django_data_browser.egg-info/
+-rw-rw-rw-   0        0        0    61701 2023-05-07 09:31:28.000000 django-data-browser-4.1.1/django_data_browser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3438 2023-05-07 09:31:28.000000 django-data-browser-4.1.1/django_data_browser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 09:31:28.000000 django-data-browser-4.1.1/django_data_browser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-07 09:31:28.000000 django-data-browser-4.1.1/django_data_browser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 09:31:28.000000 django-data-browser-4.1.1/django_data_browser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.652901 django-data-browser-4.1.1/frontend/
+-rw-rw-rw-   0        0        0     2891 2020-04-22 19:19:40.000000 django-data-browser-4.1.1/frontend/README.md
+-rw-rw-rw-   0        0        0  1009738 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/frontend/package-lock.json
+-rw-rw-rw-   0        0        0     1000 2022-04-10 12:41:54.000000 django-data-browser-4.1.1/frontend/package.json
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.653898 django-data-browser-4.1.1/frontend/public/
+-rw-rw-rw-   0        0        0     3304 2023-03-06 21:38:15.000000 django-data-browser-4.1.1/frontend/public/index.html
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.676837 django-data-browser-4.1.1/frontend/src/
+-rw-rw-rw-   0        0        0     1298 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/frontend/src/App.js
+-rw-rw-rw-   0        0        0     7309 2023-05-01 19:00:32.000000 django-data-browser-4.1.1/frontend/src/App.scss
+-rw-rw-rw-   0        0        0      280 2020-04-22 19:19:40.000000 django-data-browser-4.1.1/frontend/src/App.test.js
+-rw-rw-rw-   0        0        0       85 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/frontend/src/Config.js
+-rw-rw-rw-   0        0        0     2678 2021-12-29 21:35:30.000000 django-data-browser-4.1.1/frontend/src/ContextMenu.js
+-rw-rw-rw-   0        0        0      551 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/frontend/src/CurrentSavedView.js
+-rw-rw-rw-   0        0        0     4278 2023-05-01 19:00:44.000000 django-data-browser-4.1.1/frontend/src/HomePage.js
+-rw-rw-rw-   0        0        0     9454 2023-05-01 18:59:45.000000 django-data-browser-4.1.1/frontend/src/Query.js
+-rw-rw-rw-   0        0        0      144 2020-06-27 10:10:01.000000 django-data-browser-4.1.1/frontend/src/Query.test.js
+-rw-rw-rw-   0        0        0    14845 2023-05-01 18:59:45.000000 django-data-browser-4.1.1/frontend/src/QueryPage.js
+-rw-rw-rw-   0        0        0     9360 2021-12-29 21:35:30.000000 django-data-browser-4.1.1/frontend/src/Results.js
+-rw-rw-rw-   0        0        0     6645 2023-05-01 19:01:07.000000 django-data-browser-4.1.1/frontend/src/SavedViewPage.js
+-rw-rw-rw-   0        0        0     1649 2021-12-30 00:35:29.000000 django-data-browser-4.1.1/frontend/src/Tooltip.js
+-rw-rw-rw-   0        0        0    12431 2023-05-01 19:01:07.000000 django-data-browser-4.1.1/frontend/src/Util.js
+-rw-rw-rw-   0        0        0      591 2021-12-12 20:01:39.000000 django-data-browser-4.1.1/frontend/src/WindowDimensions.js
+-rw-rw-rw-   0        0        0      733 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/frontend/src/index.js
+-rw-rw-rw-   0        0        0      366 2020-04-22 19:19:40.000000 django-data-browser-4.1.1/frontend/src/index.scss
+-rw-rw-rw-   0        0        0     2671 2020-04-22 19:19:40.000000 django-data-browser-4.1.1/frontend/src/logo.svg
+-rw-rw-rw-   0        0        0      255 2020-04-22 19:19:40.000000 django-data-browser-4.1.1/frontend/src/setupTests.js
+-rw-rw-rw-   0        0        0     2837 2023-05-01 18:51:44.000000 django-data-browser-4.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      260 2023-03-06 20:00:37.000000 django-data-browser-4.1.1/requirements.txt
+-rw-rw-rw-   0        0        0   112598 2021-03-13 16:54:43.000000 django-data-browser-4.1.1/screenshot.png
+-rw-rw-rw-   0        0        0       42 2023-05-07 09:31:28.713739 django-data-browser-4.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2023-03-30 22:40:08.000000 django-data-browser-4.1.1/setup.py
+-rw-rw-rw-   0        0        0    35837 2020-06-27 10:10:01.000000 django-data-browser-4.1.1/structure.svg
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.697781 django-data-browser-4.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2019-07-20 09:57:44.000000 django-data-browser-4.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.699776 django-data-browser-4.1.1/tests/array/
+-rw-rw-rw-   0        0        0        0 2020-10-24 10:26:31.000000 django-data-browser-4.1.1/tests/array/__init__.py
+-rw-rw-rw-   0        0        0      617 2021-12-31 10:07:16.000000 django-data-browser-4.1.1/tests/array/models.py
+-rw-rw-rw-   0        0        0     2343 2023-05-07 09:14:15.000000 django-data-browser-4.1.1/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.702768 django-data-browser-4.1.1/tests/core/
+-rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.1.1/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     4422 2021-12-31 10:49:19.000000 django-data-browser-4.1.1/tests/core/admin.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.704762 django-data-browser-4.1.1/tests/core/migrations/
+-rw-rw-rw-   0        0        0    10069 2023-03-06 08:08:57.000000 django-data-browser-4.1.1/tests/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2021-12-29 23:58:51.000000 django-data-browser-4.1.1/tests/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4303 2021-12-31 10:48:59.000000 django-data-browser-4.1.1/tests/core/models.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.705760 django-data-browser-4.1.1/tests/json/
+-rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.1.1/tests/json/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-03-30 22:40:08.000000 django-data-browser-4.1.1/tests/json/models.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:31:28.709749 django-data-browser-4.1.1/tests/snapshots/
+-rw-rw-rw-   0        0        0        0 2020-06-27 10:10:01.000000 django-data-browser-4.1.1/tests/snapshots/__init__.py
+-rw-rw-rw-   0        0        0   436829 2023-05-01 18:51:44.000000 django-data-browser-4.1.1/tests/snapshots/snap_test_views.py
+-rw-rw-rw-   0        0        0     5231 2023-04-25 17:09:12.000000 django-data-browser-4.1.1/tests/test_admin.py
+-rw-rw-rw-   0        0        0    20582 2023-05-07 09:13:51.000000 django-data-browser-4.1.1/tests/test_api.py
+-rw-rw-rw-   0        0        0     7162 2022-02-07 21:31:16.000000 django-data-browser-4.1.1/tests/test_array_field.py
+-rw-rw-rw-   0        0        0      919 2020-09-09 18:29:41.000000 django-data-browser-4.1.1/tests/test_common.py
+-rw-rw-rw-   0        0        0     3693 2022-05-03 21:04:24.000000 django-data-browser-4.1.1/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     6081 2023-03-30 22:40:08.000000 django-data-browser-4.1.1/tests/test_json_field.py
+-rw-rw-rw-   0        0        0     4483 2021-12-12 21:09:42.000000 django-data-browser-4.1.1/tests/test_migrations.py
+-rw-rw-rw-   0        0        0     1240 2020-07-06 07:50:49.000000 django-data-browser-4.1.1/tests/test_models.py
+-rw-rw-rw-   0        0        0    35026 2023-03-30 22:40:08.000000 django-data-browser-4.1.1/tests/test_orm.py
+-rw-rw-rw-   0        0        0      878 2023-03-30 22:40:08.000000 django-data-browser-4.1.1/tests/test_orm_debug.py
+-rw-rw-rw-   0        0        0    25081 2023-03-30 21:24:18.000000 django-data-browser-4.1.1/tests/test_query.py
+-rw-rw-rw-   0        0        0      165 2020-10-22 20:32:07.000000 django-data-browser-4.1.1/tests/test_tests.py
+-rw-rw-rw-   0        0        0    18139 2023-05-01 18:59:45.000000 django-data-browser-4.1.1/tests/test_views.py
+-rw-rw-rw-   0        0        0      184 2020-10-22 18:16:38.000000 django-data-browser-4.1.1/tests/urls.py
+-rw-rw-rw-   0        0        0      366 2023-03-30 21:24:18.000000 django-data-browser-4.1.1/tests/util.py
+-rw-rw-rw-   0        0        0      574 2023-03-30 22:40:08.000000 django-data-browser-4.1.1/tox.ini
```

### Comparing `django-data-browser-4.1.0/.pre-commit-config.yaml` & `django-data-browser-4.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/CONTRIBUTING.rst` & `django-data-browser-4.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/LICENSE` & `django-data-browser-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/MANIFEST.in` & `django-data-browser-4.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/PKG-INFO` & `django-data-browser-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-browser
-Version: 4.1.0
+Version: 4.1.1
 Summary: Interactive user-friendly database explorer.
 Home-page: https://github.com/tolomea/django-data-browser
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -365,14 +365,16 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.1.1   | 2023-05-07 | Fix bug with shared views when using multiple authentication backends.                                   |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.0   | 2023-05-01 | | Support sharing of saved views between users.                                                          |
 |         |            | | Allow mixing of folders and views in the saved views section.                                          |
 |         |            | | Fix bug where an invalid filter causes the query page to fail to render.                               |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.0.17  | 2023-04-25 | Fix bug with admin actions only working on the first column (introduced in 4.0.14).                      |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.0.16  | 2023-04-16 | | Group homepage model list into collapsible sections by app.                                            |
```

### Comparing `django-data-browser-4.1.0/README.rst` & `django-data-browser-4.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -351,14 +351,16 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.1.1   | 2023-05-07 | Fix bug with shared views when using multiple authentication backends.                                   |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.0   | 2023-05-01 | | Support sharing of saved views between users.                                                          |
 |         |            | | Allow mixing of folders and views in the saved views section.                                          |
 |         |            | | Fix bug where an invalid filter causes the query page to fail to render.                               |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.0.17  | 2023-04-25 | Fix bug with admin actions only working on the first column (introduced in 4.0.14).                      |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.0.16  | 2023-04-16 | | Group homepage model list into collapsible sections by app.                                            |
```

### Comparing `django-data-browser-4.1.0/data_browser/admin.py` & `django-data-browser-4.1.1/data_browser/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/api.py` & `django-data-browser-4.1.1/data_browser/api.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/common.py` & `django-data-browser-4.1.1/data_browser/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,59 @@
 from django import http
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Permission
 from django.contrib.contenttypes.models import ContentType
 
 from . import version
 
+
+class Settings:
+    _defaults = {
+        "DATA_BROWSER_ALLOW_PUBLIC": False,
+        "DATA_BROWSER_AUTH_USER_COMPAT": True,
+        "DATA_BROWSER_DEFAULT_ROW_LIMIT": 1000,
+        "DATA_BROWSER_DEV": False,
+        "DATA_BROWSER_FE_DSN": None,
+        "DATA_BROWSER_ADMIN_FIELD_NAME": "admin",
+        "DATA_BROWSER_USING_DB": "default",
+        "DATA_BROWSER_ADMIN_OPTIONS": {},
+        "DATA_BROWSER_APPS_EXPANDED": True,
+    }
+
+    def __getattr__(self, name):
+        from django.conf import settings
+
+        if hasattr(settings, name):
+            return getattr(settings, name)
+        return self._defaults[name]
+
+
+settings = Settings()
+
+
 PUBLIC_PERM = "make_view_public"
 SHARE_PERM = "share_view"
 
 
 def has_permission(user, permission):
     return user.has_perm(f"data_browser.{permission}")
 
 
 def users_with_permission(permission):
     from .models import View
 
     ct = ContentType.objects.get_for_model(View)
     perm = Permission.objects.get(codename=permission, content_type=ct)
-    return get_user_model().objects.with_perm(perm)
+    User = get_user_model()
+
+    qs = User.objects.none()
+    for backend_path in settings.AUTHENTICATION_BACKENDS:
+        qs |= User.objects.with_perm(perm, backend=backend_path)
+
+    return qs
 
 
 def str_user(user):
     return (
         str(user) or user.get_username() or getattr(user, user.get_email_field_name())
     )
 
@@ -96,31 +127,7 @@
 
 def add_request_info(request, *, view=False):
     request.data_browser = {
         "public_view": view,
         "fields": set(),
         "calculated_fields": set(),
     }
-
-
-class Settings:
-    _defaults = {
-        "DATA_BROWSER_ALLOW_PUBLIC": False,
-        "DATA_BROWSER_AUTH_USER_COMPAT": True,
-        "DATA_BROWSER_DEFAULT_ROW_LIMIT": 1000,
-        "DATA_BROWSER_DEV": False,
-        "DATA_BROWSER_FE_DSN": None,
-        "DATA_BROWSER_ADMIN_FIELD_NAME": "admin",
-        "DATA_BROWSER_USING_DB": "default",
-        "DATA_BROWSER_ADMIN_OPTIONS": {},
-        "DATA_BROWSER_APPS_EXPANDED": True,
-    }
-
-    def __getattr__(self, name):
-        from django.conf import settings
-
-        if hasattr(settings, name):
-            return getattr(settings, name)
-        return self._defaults[name]
-
-
-settings = Settings()
```

### Comparing `django-data-browser-4.1.0/data_browser/fe_build/index.html` & `django-data-browser-4.1.1/data_browser/fe_build/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/fe_build/static/css/main.6e6fbe98.css` & `django-data-browser-4.1.1/data_browser/fe_build/static/css/main.6e6fbe98.css`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/fe_build/static/css/main.6e6fbe98.css.map` & `django-data-browser-4.1.1/data_browser/fe_build/static/css/main.6e6fbe98.css.map`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/fe_build/static/js/main.b4d189f0.js` & `django-data-browser-4.1.1/data_browser/fe_build/static/js/main.b4d189f0.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/fe_build/static/js/main.b4d189f0.js.LICENSE.txt` & `django-data-browser-4.1.1/data_browser/fe_build/static/js/main.b4d189f0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/fe_build/static/js/main.b4d189f0.js.map` & `django-data-browser-4.1.1/data_browser/fe_build/static/js/main.b4d189f0.js.map`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/format_csv.py` & `django-data-browser-4.1.1/data_browser/format_csv.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/helpers.py` & `django-data-browser-4.1.1/data_browser/helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/migration_helpers.py` & `django-data-browser-4.1.1/data_browser/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/migrations/0001_initial.py` & `django-data-browser-4.1.1/data_browser/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/migrations/0002_auto_20200331_1842.py` & `django-data-browser-4.1.1/data_browser/migrations/0002_auto_20200331_1842.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/migrations/0006_auto_20200531_1450.py` & `django-data-browser-4.1.1/data_browser/migrations/0006_auto_20200531_1450.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/migrations/0012_can_share.py` & `django-data-browser-4.1.1/data_browser/migrations/0012_can_share.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/models.py` & `django-data-browser-4.1.1/data_browser/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/orm_admin.py` & `django-data-browser-4.1.1/data_browser/orm_admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/orm_aggregates.py` & `django-data-browser-4.1.1/data_browser/orm_aggregates.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/orm_debug.py` & `django-data-browser-4.1.1/data_browser/orm_debug.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/orm_fields.py` & `django-data-browser-4.1.1/data_browser/orm_fields.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/orm_functions.py` & `django-data-browser-4.1.1/data_browser/orm_functions.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/orm_lookups.py` & `django-data-browser-4.1.1/data_browser/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/orm_results.py` & `django-data-browser-4.1.1/data_browser/orm_results.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/orm_types.py` & `django-data-browser-4.1.1/data_browser/orm_types.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/query.py` & `django-data-browser-4.1.1/data_browser/query.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/templates/data_browser/index.html` & `django-data-browser-4.1.1/data_browser/templates/data_browser/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/types.py` & `django-data-browser-4.1.1/data_browser/types.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/urls.py` & `django-data-browser-4.1.1/data_browser/urls.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/views.py` & `django-data-browser-4.1.1/data_browser/views.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/web_root/android-chrome-192x192.png` & `django-data-browser-4.1.1/data_browser/web_root/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/web_root/android-chrome-512x512.png` & `django-data-browser-4.1.1/data_browser/web_root/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/web_root/apple-touch-icon.png` & `django-data-browser-4.1.1/data_browser/web_root/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/web_root/favicon-32x32.png` & `django-data-browser-4.1.1/data_browser/web_root/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/data_browser/web_root/favicon.ico` & `django-data-browser-4.1.1/data_browser/web_root/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/django_data_browser.egg-info/PKG-INFO` & `django-data-browser-4.1.1/django_data_browser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-browser
-Version: 4.1.0
+Version: 4.1.1
 Summary: Interactive user-friendly database explorer.
 Home-page: https://github.com/tolomea/django-data-browser
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -365,14 +365,16 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.1.1   | 2023-05-07 | Fix bug with shared views when using multiple authentication backends.                                   |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.0   | 2023-05-01 | | Support sharing of saved views between users.                                                          |
 |         |            | | Allow mixing of folders and views in the saved views section.                                          |
 |         |            | | Fix bug where an invalid filter causes the query page to fail to render.                               |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.0.17  | 2023-04-25 | Fix bug with admin actions only working on the first column (introduced in 4.0.14).                      |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.0.16  | 2023-04-16 | | Group homepage model list into collapsible sections by app.                                            |
```

### Comparing `django-data-browser-4.1.0/django_data_browser.egg-info/SOURCES.txt` & `django-data-browser-4.1.1/django_data_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/README.md` & `django-data-browser-4.1.1/frontend/README.md`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/package-lock.json` & `django-data-browser-4.1.1/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/package.json` & `django-data-browser-4.1.1/frontend/package.json`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/public/index.html` & `django-data-browser-4.1.1/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/App.js` & `django-data-browser-4.1.1/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/App.scss` & `django-data-browser-4.1.1/frontend/src/App.scss`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/ContextMenu.js` & `django-data-browser-4.1.1/frontend/src/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/CurrentSavedView.js` & `django-data-browser-4.1.1/frontend/src/CurrentSavedView.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/HomePage.js` & `django-data-browser-4.1.1/frontend/src/HomePage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/Query.js` & `django-data-browser-4.1.1/frontend/src/Query.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/QueryPage.js` & `django-data-browser-4.1.1/frontend/src/QueryPage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/Results.js` & `django-data-browser-4.1.1/frontend/src/Results.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/SavedViewPage.js` & `django-data-browser-4.1.1/frontend/src/SavedViewPage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/Tooltip.js` & `django-data-browser-4.1.1/frontend/src/Tooltip.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/Util.js` & `django-data-browser-4.1.1/frontend/src/Util.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/WindowDimensions.js` & `django-data-browser-4.1.1/frontend/src/WindowDimensions.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/index.js` & `django-data-browser-4.1.1/frontend/src/index.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/frontend/src/logo.svg` & `django-data-browser-4.1.1/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/pyproject.toml` & `django-data-browser-4.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/screenshot.png` & `django-data-browser-4.1.1/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/setup.py` & `django-data-browser-4.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/structure.svg` & `django-data-browser-4.1.1/structure.svg`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/array/models.py` & `django-data-browser-4.1.1/tests/array/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/conftest.py` & `django-data-browser-4.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/core/admin.py` & `django-data-browser-4.1.1/tests/core/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/core/migrations/0001_initial.py` & `django-data-browser-4.1.1/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/core/models.py` & `django-data-browser-4.1.1/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/snapshots/snap_test_views.py` & `django-data-browser-4.1.1/tests/snapshots/snap_test_views.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_admin.py` & `django-data-browser-4.1.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_api.py` & `django-data-browser-4.1.1/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,23 @@
                     "can_edit": True,
                     "type": "view",
                 }
             ],
             "shared": [],
         }
 
+    def test_with_multiple_aut_backends(self, admin_client, admin_user, view, settings):
+        settings.AUTHENTICATION_BACKENDS = [
+            "django.contrib.auth.backends.ModelBackend",
+            "django.contrib.auth.backends.ModelBackend",
+        ]
+
+        resp = admin_client.get("/data_browser/api/views/")
+        assert resp.status_code == 200
+
     def test_get_with_folders_and_shared_views(
         self, view, multiple_views, admin_user, other_user, get_list_summary
     ):
         make_view(
             owner=other_user,
             name="shared_in_folder",
             shared=True,
```

### Comparing `django-data-browser-4.1.0/tests/test_array_field.py` & `django-data-browser-4.1.1/tests/test_array_field.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_common.py` & `django-data-browser-4.1.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_helpers.py` & `django-data-browser-4.1.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_json_field.py` & `django-data-browser-4.1.1/tests/test_json_field.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_migrations.py` & `django-data-browser-4.1.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_models.py` & `django-data-browser-4.1.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_orm.py` & `django-data-browser-4.1.1/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_orm_debug.py` & `django-data-browser-4.1.1/tests/test_orm_debug.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_query.py` & `django-data-browser-4.1.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tests/test_views.py` & `django-data-browser-4.1.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.1.0/tox.ini` & `django-data-browser-4.1.1/tox.ini`

 * *Files identical despite different names*

