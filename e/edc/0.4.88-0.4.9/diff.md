# Comparing `tmp/edc-0.4.88.tar.gz` & `tmp/edc-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.4.88.tar", last modified: Sun May  7 19:17:37 2023, max compression
+gzip compressed data, was "edc-0.4.9.tar", last modified: Mon Aug 15 01:45:03 2022, max compression
```

## Comparing `edc-0.4.88.tar` & `edc-0.4.9.tar`

### file list

```diff
@@ -1,75 +1,72 @@
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.129732 edc-0.4.88/
--rw-r--r--   0 jw         (502) staff       (20)     1410 2023-04-18 18:48:47.000000 edc-0.4.88/.gitignore
--rw-r--r--   0 jw         (502) staff       (20)     1076 2023-05-07 19:08:23.000000 edc-0.4.88/.pre-commit-config.yaml
--rw-r--r--   0 jw         (502) staff       (20)      291 2023-04-18 18:48:47.000000 edc-0.4.88/.yamllint
--rw-r--r--   0 jw         (502) staff       (20)        0 2023-04-18 18:48:47.000000 edc-0.4.88/AUTHORS
--rw-r--r--   0 jw         (502) staff       (20)    38851 2023-05-07 19:17:23.000000 edc-0.4.88/CHANGES
--rw-r--r--   0 jw         (502) staff       (20)    35147 2021-07-06 12:52:00.000000 edc-0.4.88/LICENSE
--rw-r--r--   0 jw         (502) staff       (20)      151 2021-07-06 12:52:00.000000 edc-0.4.88/MANIFEST.in
--rw-r--r--   0 jw         (502) staff       (20)    38295 2023-05-07 19:17:37.130082 edc-0.4.88/PKG-INFO
--rw-r--r--   0 jw         (502) staff       (20)    37432 2023-05-07 19:08:23.000000 edc-0.4.88/README.rst
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.082349 edc-0.4.88/bin/
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.091485 edc-0.4.88/bin/nginx/
--rw-r--r--   0 jw         (502) staff       (20)      350 2023-04-18 18:48:47.000000 edc-0.4.88/bin/nginx/edc-sites.conf
--rw-r--r--   0 jw         (502) staff       (20)      706 2023-04-18 18:48:47.000000 edc-0.4.88/bin/nginx/edc-uat.conf
--rw-r--r--   0 jw         (502) staff       (20)      656 2023-04-18 18:48:47.000000 edc-0.4.88/bin/nginx/edc.conf
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.094094 edc-0.4.88/bin/scripts/
--rw-r--r--   0 jw         (502) staff       (20)     2753 2023-04-18 18:48:47.000000 edc-0.4.88/bin/scripts/dev_repos.sh
--rw-r--r--   0 jw         (502) staff       (20)      276 2021-07-06 12:52:00.000000 edc-0.4.88/bin/scripts/list_db_files.sh
--rw-r--r--   0 jw         (502) staff       (20)      416 2021-07-06 12:52:00.000000 edc-0.4.88/bin/scripts/restore_db_file.sh
--rw-r--r--   0 jw         (502) staff       (20)     2408 2023-04-18 18:48:47.000000 edc-0.4.88/bin/scripts/update_edc.sh
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.099488 edc-0.4.88/bin/systemd/
--rw-r--r--   0 jw         (502) staff       (20)      835 2021-07-06 12:52:00.000000 edc-0.4.88/bin/systemd/celery-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      820 2021-07-06 12:52:00.000000 edc-0.4.88/bin/systemd/celery.service
--rw-r--r--   0 jw         (502) staff       (20)      501 2021-07-06 12:52:00.000000 edc-0.4.88/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      487 2021-07-06 12:52:00.000000 edc-0.4.88/bin/systemd/celerybeat.service
--rw-r--r--   0 jw         (502) staff       (20)      485 2021-07-06 12:52:00.000000 edc-0.4.88/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      121 2021-07-06 12:52:00.000000 edc-0.4.88/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 jw         (502) staff       (20)      474 2021-07-06 12:52:00.000000 edc-0.4.88/bin/systemd/gunicorn.service
--rw-r--r--   0 jw         (502) staff       (20)      111 2021-07-06 12:52:00.000000 edc-0.4.88/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.115069 edc-0.4.88/docs/
--rw-r--r--   0 jw         (502) staff       (20)      634 2023-04-18 18:48:47.000000 edc-0.4.88/docs/Makefile
--rw-r--r--   0 jw         (502) staff       (20)    12969 2023-05-07 19:08:23.000000 edc-0.4.88/docs/README.rst
--rw-r--r--   0 jw         (502) staff       (20)     4441 2023-04-18 18:48:47.000000 edc-0.4.88/docs/backup.rst
--rw-r--r--   0 jw         (502) staff       (20)     5437 2023-04-27 10:01:42.000000 edc-0.4.88/docs/celery.rst
--rw-r--r--   0 jw         (502) staff       (20)      580 2023-04-18 18:48:47.000000 edc-0.4.88/docs/conda.rst
--rw-r--r--   0 jw         (502) staff       (20)      975 2023-04-18 18:48:47.000000 edc-0.4.88/docs/conf.py
--rw-r--r--   0 jw         (502) staff       (20)     4806 2023-04-18 18:48:47.000000 edc-0.4.88/docs/configure_web_services.rst
--rw-r--r--   0 jw         (502) staff       (20)     3646 2023-04-18 18:48:47.000000 edc-0.4.88/docs/deploy_new_droplet.rst
--rw-r--r--   0 jw         (502) staff       (20)      163 2021-07-06 12:52:00.000000 edc-0.4.88/docs/dump_users.rst
--rw-r--r--   0 jw         (502) staff       (20)      845 2021-07-06 12:52:00.000000 edc-0.4.88/docs/exporting_encrypted_data.rst
--rw-r--r--   0 jw         (502) staff       (20)   258708 2023-04-18 18:48:47.000000 edc-0.4.88/docs/forms_reference.md
--rw-r--r--   0 jw         (502) staff       (20)      445 2023-04-18 18:48:47.000000 edc-0.4.88/docs/index.rst
--rw-r--r--   0 jw         (502) staff       (20)      778 2021-07-06 12:52:00.000000 edc-0.4.88/docs/landing_page.rst
--rw-r--r--   0 jw         (502) staff       (20)      765 2023-04-18 18:48:47.000000 edc-0.4.88/docs/make.bat
--rw-r--r--   0 jw         (502) staff       (20)        0 2021-07-06 12:52:00.000000 edc-0.4.88/docs/multisite_deployment.rst
--rw-r--r--   0 jw         (502) staff       (20)     3928 2023-04-18 18:48:47.000000 edc-0.4.88/docs/prepare_database.rst
--rw-r--r--   0 jw         (502) staff       (20)     1211 2023-04-18 18:48:47.000000 edc-0.4.88/docs/printing.rst
--rw-r--r--   0 jw         (502) staff       (20)      187 2021-07-06 12:52:00.000000 edc-0.4.88/docs/redis.rst
--rw-r--r--   0 jw         (502) staff       (20)      766 2021-07-06 12:52:00.000000 edc-0.4.88/docs/update_deployment.rst
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.118340 edc-0.4.88/edc.egg-info/
--rw-r--r--   0 jw         (502) staff       (20)    38295 2023-05-07 19:17:36.000000 edc-0.4.88/edc.egg-info/PKG-INFO
--rw-r--r--   0 jw         (502) staff       (20)     1508 2023-05-07 19:17:37.000000 edc-0.4.88/edc.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (502) staff       (20)        1 2023-05-07 19:17:36.000000 edc-0.4.88/edc.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (502) staff       (20)        1 2021-09-27 09:58:54.000000 edc-0.4.88/edc.egg-info/not-zip-safe
--rw-r--r--   0 jw         (502) staff       (20)     1922 2023-05-07 19:17:36.000000 edc-0.4.88/edc.egg-info/requires.txt
--rw-r--r--   0 jw         (502) staff       (20)        6 2023-05-07 19:17:36.000000 edc-0.4.88/edc.egg-info/top_level.txt
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.118806 edc-0.4.88/image/
--rw-r--r--   0 jw         (502) staff       (20)   160721 2021-08-24 11:21:23.000000 edc-0.4.88/image/icon-pycharm.png
--rw-r--r--   0 jw         (502) staff       (20)      162 2023-04-18 18:48:47.000000 edc-0.4.88/pyproject.toml
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.127876 edc-0.4.88/requirements.tests/
--rw-r--r--   0 jw         (502) staff       (20)       21 2023-04-18 18:48:47.000000 edc-0.4.88/requirements.tests/coverage.txt
--rw-r--r--   0 jw         (502) staff       (20)       14 2023-04-18 18:48:47.000000 edc-0.4.88/requirements.tests/docs.txt
--rw-r--r--   0 jw         (502) staff       (20)     1053 2023-05-07 19:16:29.000000 edc-0.4.88/requirements.tests/edc.txt
--rw-r--r--   0 jw         (502) staff       (20)     4100 2023-04-18 18:48:47.000000 edc-0.4.88/requirements.tests/edc_dev.txt
--rw-r--r--   0 jw         (502) staff       (20)       68 2021-07-06 12:52:00.000000 edc-0.4.88/requirements.tests/edc_offline.txt
--rw-r--r--   0 jw         (502) staff       (20)       54 2023-04-18 18:48:47.000000 edc-0.4.88/requirements.tests/lint.txt
--rw-r--r--   0 jw         (502) staff       (20)       11 2023-04-18 18:48:47.000000 edc-0.4.88/requirements.tests/mysql.txt
--rw-r--r--   0 jw         (502) staff       (20)       22 2021-07-06 12:52:00.000000 edc-0.4.88/requirements.tests/postgres.txt
--rw-r--r--   0 jw         (502) staff       (20)       86 2023-04-18 18:48:47.000000 edc-0.4.88/requirements.tests/test_utils.txt
--rw-r--r--   0 jw         (502) staff       (20)      238 2023-04-18 18:48:47.000000 edc-0.4.88/requirements.tests/third_party_dev.txt
--rw-r--r--   0 jw         (502) staff       (20)       50 2023-04-18 18:48:47.000000 edc-0.4.88/requirements.tests/tox.txt
--rw-r--r--   0 jw         (502) staff       (20)     2994 2023-05-07 19:17:37.131413 edc-0.4.88/setup.cfg
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-05-07 19:17:37.129056 edc-0.4.88/utils/
--rw-r--r--   0 jw         (502) staff       (20)        0 2021-07-06 12:52:00.000000 edc-0.4.88/utils/__init__.py
--rw-r--r--   0 jw         (502) staff       (20)      721 2023-04-18 18:48:47.000000 edc-0.4.88/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.020420 edc-0.4.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-12 15:19:56.000000 edc-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    24315 2022-08-15 01:44:54.000000 edc-0.4.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    36927 2022-08-15 01:45:03.020572 edc-0.4.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    35978 2022-08-15 01:30:02.000000 edc-0.4.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        5 2022-08-15 01:44:54.000000 edc-0.4.9/VERSION
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.006464 edc-0.4.9/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.009745 edc-0.4.9/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.9/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.9/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.9/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.010386 edc-0.4.9/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2778 2022-08-10 01:27:44.000000 edc-0.4.9/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.9/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.9/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.9/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.011571 edc-0.4.9/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.014346 edc-0.4.9/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)    11863 2022-07-30 01:15:42.000000 edc-0.4.9/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.9/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.9/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.9/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.9/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3625 2022-07-30 01:15:42.000000 edc-0.4.9/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.9/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.9/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.9/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.9/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.9/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3267 2022-07-30 01:15:42.000000 edc-0.4.9/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.9/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.9/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.9/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.015210 edc-0.4.9/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    36927 2022-08-15 01:45:02.000000 edc-0.4.9/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1460 2022-08-15 01:45:03.000000 edc-0.4.9/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-15 01:45:02.000000 edc-0.4.9/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.9/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1810 2022-08-15 01:45:02.000000 edc-0.4.9/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-15 01:45:02.000000 edc-0.4.9/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.015311 edc-0.4.9/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.9/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.9/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.019973 edc-0.4.9/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.9/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.9/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1009 2022-08-15 01:30:02.000000 edc-0.4.9/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4101 2022-08-15 01:30:02.000000 edc-0.4.9/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.9/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.9/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.9/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.9/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.9/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-08-10 01:27:44.000000 edc-0.4.9/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.9/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2941 2022-08-15 01:45:03.020986 edc-0.4.9/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.020261 edc-0.4.9/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.9/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.9/utils/get_edc_requirements.py
```

### Comparing `edc-0.4.88/.gitignore` & `edc-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/.pre-commit-config.yaml` & `edc-0.4.9/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,44 @@
     rev: 1.7.4
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 22.6.0
     hooks:
       - id: black
-        language_version: python3.9
+        language_version: python3.8
 
   - repo: https://github.com/pycqa/flake8
-    rev: 6.0.0
+    rev: 5.0.4
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.10.1
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.3.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.29.0
+    rev: v1.27.1
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-0.4.88/CHANGES` & `edc-0.4.9/CHANGES`

 * *Files 20% similar despite different names*

```diff
@@ -1,467 +1,9 @@
 Changes
--------
-
-0.4.88
-------
-- fix applicable_if_diagnosed validator (edc-dx)
-
-0.4.87
-------
-- add func to get appointment by datetime (edc-appointment)
-- move icecapa fields to model_mixin (edc-qol)
-
-0.4.86
-------
-- add NA option th choices (edc-lab)
-
-0.4.85
-------
-- accept site_id if known when creating identifiers. Useful
-  when creating identifiers in data migrations.
-  (edc-identifier)
-
-0.4.84
-------
-- fix comparison of db datetime with milliseconds vs django datetime without
-  (edc-appointment, edc-visit-schedule)
-- add new block to template for demographics title (edc-subject-dashboard)
-- render to response and just buffer (edc-pdf-report)
-- handle null identifier (edc-identifier)
-- add ICECAP-A version 2 (edc-qol)
-- add additional disease constants (edc-constants)
-
-0.4.83
-------
-- limit export of sensitive data to members of EXPORT_PII group. Only allow
-  users specified in settings to be added to EXPORT_PII group.
-  (edc-pdutils, edc-export)
-- add fieldset tuple to work with glucose model mixins (edc-glucose)
-- add NA option to rx_init (edc-dx-review)
-- fix validation issues with field `return_in_days` (edc-rx)
-
-0.4.82
-------
-- compare rx_init_date to report_datetime (edc-dx-review)
-
-0.4.81
-------
-- add additional fields and form logic to clinical review
-  baseline (edc-dx-review)
-- clean up unused test tags
-- setup configs
-
-0.4.80
-------
-- export by model (edc-pdutils)
-- other minor fixes (edc-dx-review, edc-form-validators)
-
-0.4.79
-------
-- bump to edc-dx-review 0.1.33
-
-0.4.78
-------
-- bump to django-crypto-fields 0.3.5
-
-0.4.77
-------
-- require edc-rx
-
-0.4.76
-------
-- simplify clinical baseline review, change initial review fields to be more
-  consistent. Use factories for model mixins. (edc-dx-review)
-- fix tests (edc-dx)
-- detect list models using ListUuidModelMixin (edc-pdutils)
-
-0.4.75
-------
-- additional features to export data (edc-pdutils)
-
-0.4.74
-------
-- add human readable identifier (edc-identifier)
-
-0.4.73
-----------
-- add more validation to ClinicalReviewFollowupFormValidatorMixin (edc-dx-review)
-- bump edc-rx
-
-0.4.72
-------
-- add signals to SubjectRefusal to update SubjectScreening model on add/delete (edc-refusal)
-
-0.4.71
-------
-- update neutrophil and lymphocyte model mixin settings (edc-lab-results)
-- trivial (edc-model-form)
-- add management command for CSV and STATA dataset export (edc-pdutils)
-
-0.4.70
-------
-- remove subject_consent_form_validator mixin from crf_form_validator.
-  Consent version and timing is verified in the modelform (edc-crf)
-- move model code to mixin (edc-data-manager)
-- trivial (edc-sites)
-
-0.4.69
-------
-- fix missing codename in DATA_MANAGER_SUPER group, on migrate (edc-data-manager)
-- add Python 3.11 support
-- drop Python 3.9 support
-
-0.4.68
-------
-- modeladmin mixin that selects the Form class conditionally by
-  user permission. Custom Form class removes all validation but
-  could be any Form class. (edc-model-admin)
-- add DATA_MANAGER_SUPER group, add codename tuple used by
-  modeladmin to select Form class by inspecting user perms.
-  (edc-data-manager)
-- add `special` to list of allowed codename prefixes (edc-auth)
-
-0.4.65
-------
-- ignore metadata rule if source model not in the current visits crfs
-  (edc-metadata)
-
-0.4.64
-------
-- add `HeartRateField` and `RespiratoryRateField` (edc-vitals)
-
-0.4.63
-------
-- add constants (edc-constants)
-- fix misspelled attr (edc-dx-review)
-
-0.4.62
-------
-- change `appointment.appt_type` model field to foreign key and
-  get choices from list_data. (edc-appointment)
-- add settings attributes for default appt_type choices, referenced
-  in list_data, and default value. (edc-appointment)
-- add fields familiar_name, full_name to registered subject
-  (edc-registration)
-- add late lower and upper to visit class (edc-visit-schedule)
-- now can customize name field and identity regex using class attrs
-  on SubjectListboardView (edc-listboard)
-- add option to customize identifier field name for utils and
-  other funcs. (edc-randomization)
-
-0.4.61
-------
-- remove 'None' choice from 'cause_of_death_agreed' in Death Report TMG (edc-adverse-event)
-- fix AE TMG Report readonly fields not pulling in ae_description,
-  ae_classification etc. (edc-adverse-event)
-
-0.4.60
-------
-- add missing migrations (edc-protocol-incident)
-- update docs on creation of MySQL users for connections from remote Django hosts
-
-0.4.59
-------
-- add option to withdraw AE after TMG review on AE followup (edc-adverse-event)
-- add investigator AE classification if not in agreement with initial
-  (edc-adverse-event)
- - add option to withdraw incident report (edc-protocol-incident)
-
-0.4.58
-------
-- add `language` to site class, `languages` to site_profile model
-  and intercept choices in modeladmin mixin (edc-sites)
-- update verbose_name and help_text on `familiar_name` field (edc-model)
-
-0.4.57
-------
-- move some respond mixins (edc-dx, edc-dx-review)
-
-0.4.56
-------
-- remove editable=False from eligibility model fields to show them as readonly
-  on modeladmin section (edc-screening)
-
-0.4.55
-------
-- fix missing method call in `get_changelist_url` (edc-model)
-- add new Names model mixin for legal_name, familiar_name (edc-model)
-- update consent to handle legal_name, familiar_name (edc-consent)
-- new attrs for modeladmin to add help and notes to custom changelist
-  (edc-model-admin)
-
-0.4.54
-------
-- allow to override criteria to select an unallocated registration instance
-  (edc-randomization)
-
-0.4.53
-------
-- add `get_changelist_url` to default model mixin (edc-model)
-- randomizer may identifier fields other than
-  `subject_identifier` (edc-randomization)
-- may use custom registration model (edc-registration)
-
-0.4.52
-------
-- fix regression in test sites following update to SingleSite init signature (edc-sites)
-- add PrnModelAdminMixin (edc-prn)
-- additional constants (edc-constants)
-
-0.4.51
-------
-- fix regressions causing list filter to always return an empty queryset
-  caused by not distinguishing `no date` (null) from filter not selected
-  (edc-model-admin, edc-constants)
-
-0.4.50
-------
-- * move list filter code as base class to edc-model-admin;
-  * ignore validation if appointment is cancelled;
-  * refactor missed appointment handling. (edc-appointment)
-
-0.4.49
-------
-- move reason updater to appointment (edc-appointment, edc-visit-tracking)
-- default offschedule action (edc-visit-schedule)
-- add current site to form class (edc-sites)
-- add mixins to query current site on screening form (edc-screening)
-
-0.4.48
-------
-- remove edc-egfr as a dependency
-
-0.4.47
-------
-- never export rando tables, even if user is unblinded (edc-export)
-- refactor blinded/unblined funcs (edc-randomization)
-- take code out of app_config and move to funcs in utils (edc-facility)
-- slight refactor, typing hints (edc-screening)
-
-0.4.46
-------
-- add css hack for wrapping radiolists in admin forms (edc-model-admin)
-- fix func signature (edc-form-describer)
-
-0.4.45
-------
-- fix regression that dropped linked to jQuery in edc base template
-  (edc-dashboard)
-- update rel.to to related_model for inlines (edc-crf)
-
-0.4.44
-------
-- add migration for help_text changes (edc-appointment)
-
-0.4.43
-------
-- change TabularInlineMixin to insert an inline before a fieldset
-  instead of after a field. Revert to using Django original
-  fieldset.html. Default to insert inlines before the audit
-  fieldset. (edc-model-admin)
-- move edc_protocol vars used in template context to middleware
-  (edc_protocol, edc-auth, edc-dashboard)
-- fix appointment radio widget missing class-radiolist
-- use new 4.1 template block to disable dark mode, update all
-  local admin templates (edc-model-admin)
-- set logout view to use default template. (edc-auth)
-- changes require you to run collectstatic and to clear
-  the cache on the browser to ensure jquery 3.6.0 loads.
-
-
-0.4.42
-------
-- drop mixin in favor of directly accessing func
-  `estimated_date_from_ago` (edc-dx-review)
-- fix signal attempting to delete unrleated action items
-  (edc-action-item)
-- remove code in AppConfig that auto creates export folders
-  (edc-export, edc-pdutils)
-- slight refactor (edc-timepoint)
-- clarify in exception message that edc-appointment has a reverse
-  relation to the related visit model (edc-appointment)
-- change blood result question prompt for field assay_datetime to
-  "Assay date and time" (edc-lab)
-- move save code to model method for consistency (edc-offstudy)
-- add additional unique_together constraint plus migration
-  (edc-appointment)
-- fix tests, test on py3.10 / DJ 4.1.1 primarily
-
-0.4.41
-------
-- add missing migration (edc-appointment)
-- fix import path (edc-glucose)
-
-0.4.40
-------
-- tighten up date validations across model/form/validators.
-- handle a number of regressions
-
-0.4.39
-------
-- update tests
-
-0.4.38
-------
-- update test models
-
-0.4.37
-------
-- handle a number of regressions
-- consolidate model managers and managers on model mixins
-  to make it easier to predict the _default_manager. Users
-  should add unitests to confirm concrete model classes
-  have the expected _default_manager (all with model mixins)
-- floor sec/microsec on datetimes when comparing in form
-  and form-validator validation (edc-appointment
-  edc-visit-schedule, edc-visit-tracking, edc-crf)
-- remove `SiteModelMixin` from default on/off schedule
-  model mixins. Add this mixin manually to the concrete
-  class.
-
-0.4.36
-------
-- add related visit methods to historical model (edc-model)
-- minor fixes to off/on schedule models
-
-0.4.35
-------
-- added base method to access offschedule_datetime, typing (edc-crf)
-- removed features/fields that create `next refill` on submission of
-  study medication report (edc-pharmacy)
-- trivial (edc-protocol-incident)
-- fixed issue that incorrectly compares int to str when confirming
-  that the grade from the user matches the grade from the evaluator
-  (edc-reportable)
-
-0.4.34
-------
-- rename module edc-protocol-deviation to edc-protocol-incident. This
-  requires manually renaming tables to reflect the app name and updating
-  the django_migration table app column with the new app name. Migrations
-  have been squashed for future users (edc-protocol-incident)
-- deprecate path form_validator_mixin for  form_validator_mixins
-  (edc-form-validator)
-
-0.4.31
-------
-- refactor modelform, model, and view mixins to derive subject_identifier,
-  report_datetime, related_visit_model_attr, related_visit in a consistent
-  manner. Changes added to most modules.
-  modules.
-- remove ContextMixin from view mixins. Add this to the concrete View.
-- add new typing hints in 3.10 style, convert existing ones to 3.10 style.
-- add form validation to compare user select grade with evaluated grade
-  (edc-reportable).
-- increase BMI upper bound to 75 (edc-reportable)
-- fix validation on modelform/validator mixin (edc-glucose)
-
-0.4.25
-------
-- fix issue where egfr calculator defaults to ethnicity = OTHER.
-- change rounding strategy (edc-utils and apps that round up).
-- add plural_name field to list models.
-
-0.4.24
-------
-- add data migrations to remove residual permissions
-  (edc-dashboard, edc-navbar).
-- minor update to group updater handling duplicates (edc-auth).
-
-0.4.21 - 0.4.23
----------------
-- refactor `visit_model_attr` to `related_visit_model_attr`
-- refactor model mixin method `visit` to avoid conflict with same
-  method name used in edc-visit-schedule. Use `related_visit` to
-  return a visit model instance and `visit` to return a schedule
-  visit object.
-- introduce py3.10 typing style
-- remove visit code/sequence link between study medication reports
-  and pharmacy refills (edc-pharmacy)
-- fix issue with pharmacy codenames not appearing in pharmacy
-  groups (edc-pharmacy)
-- enforce use of end date for a pharmacy refill. Adjust dates
-  if a refill is inserted between scheduled visits (edc-pharmacy)
-- confirm a group exists before adding to a role (edc-auth)
-
-0.4.20
-------
-- remove tracking identifier from all modules
-- make action_identifier nullable and blank=True (edc-action-item)
-- update custom tuple
-
-0.4.19
-------
-- minor updates (edc-utils, edc-appointment, edc-consent)
-
-0.4.18
-------
-- store custom permissions in owner app. default model is now
-  <app_label>.edcpermissions. Move away from storing all custom
-  permissions in edc-dashboard and edc-navbar. clean up auths
-  modules (most modules)
-- update references to perms in templates and navbars
-- add context-processors for apps that own constants
-  (edc-appointment, edc-constants, edc-visit-tracking)
-- add dashboard middleware (edc_review_dashboard)
-- add system checks to enforce context processors
-
-
-0.4.17
-------
-- fix regression deepcopy/copy (edc_form_validators)
-- add migrations for modules with models that use action_identifier
-
-0.4.15
-------
-- hold back support for Django 4.1 (problems with m2m on admin page)
-- move imports out of root __init__ in edc_model_admin
-- override delete_confirmation.html in admin
-
-0.4.14
-------
-
-0.4.13
-------
-- update breadcrumbs and branding for admin templates (edc-model-admin)
-- update and add fontawesomefree to requirements
-- require "fontawesomefree" in INSTALLED_APPS
-- add theme variables thru "edc_model_admin.context_processors.admin_theme"
-  if added to TEMPLATES context_processor
-- add simple themes configured from settings.EDC_MODEL_ADMIN_CSS_THEME
-- add attr to TemplateModelAdminMixin to override view_on_site and history
-  labels in object-tools
-- add TEST/LIVE badge, site name and number to admin templates
-- improve navigation between admin and edc
-- change topbar on subject dashboard to always show subject identifier
-- register auth models with edc_auth_admin, update urls
-
-0.4.12
-------
-- add to admin list_display, update imports (edc-auth)
-- carry over required fields from randomizer to importer
-  to verifier (edc-randomization)
-
-0.4.11
-------
-- refactor randomizer, verify on every import, add assignment description map,
-  add system check to validate blinded user list (edc-randomization).
-- remove formatted html from verbose names (edc-glucose)
-- rename get_subject_screening_model_name to get_subject_screening_model
-  (edc-consent)
-- add ActionItemModelAdminMixin to BloodResultsModelAdminMixin (edc-lab-results)
-- update admin templates to have consistent topbar (edc-model-admin)
-- remove coerce to datetime with astype() (edc-pdutil)
-
-0.4.10
------
-- add admin mixin, weight param (edc-egfr)
-- add func to 'get' references name (edc-reportable)
-- minor changes to update imports / lint (edc-data-manager, edc-lab-results,
-  edc-action, edc-timepoint, edc-registration, edc-metadata, edc-crf, edc-action-item)
+=======
 
 0.4.9
 -----
 - bump edc-egfr
 
 0.4.8
 -----
```

### Comparing `edc-0.4.88/LICENSE` & `edc-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/PKG-INFO` & `edc-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,47 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.88
+Version: 0.4.9
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |downloads|
 
-clinicedc
-=========
+Clinic EDC
+==========
 
-Here are a set of python modules that extend Django to empower you to build an EDC / eSource system to handle data
-collection and management for multi-site longitudinal clinical trials.
-
-Refer to the specific open projects listed below for example EDC systems built with these modules.
-The more recent the trial the better the example.
-
-The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
-the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
-`Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
-in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials have been related to HIV/AIDS research. Recent work with the
-`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM),
-Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
-three main chronic conditions -- HIV/DM/HTN.
+``Clinic EDC`` contains complete code for a set of core modules for clinical trial data management to build a trial EDC. Refer to the specific open projects listed below for example EDC systems built with these modules. The more recent the trial the better the example. The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__ in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__. Almost all trials have been related to HIV/AIDS research. Recent work with the `Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM), Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
 
-The ``clinicedc`` for each trial consists of a subset of trial-specific modules that reference this module.
+The ``Clinic EDC`` for each trial consists of a subset of trial-specific modules that reference this module.
 
-(python 3.10+ and Django 4.1, see setup.cfg)
+(python 3.9 and Django 3.2+ required, see setup.cfg)
 
 
 Projects that use the EDC
 -------------------------
 Recent examples of EDC's using this codebase:
 
 INTECOMM
@@ -144,15 +133,15 @@
 Start with main repo `bcpp`
 
 Contacts
 --------
 
 For further information go to https://github.com/erikvw.
 
-|django| |jet-brains|
+|django|
 
 =========================== ============================= ==================================
 edc-action-item_            |edc-action-item|             |pypi-edc-action-item|
 edc-adverse-event_          |edc-adverse-event|           |pypi-edc-adverse-event|
 edc-appointment_            |edc-appointment|             |pypi-edc-appointment|
 edc-auth_                   |edc-auth|                    |pypi-edc-auth|
 edc-call-manager_           |edc-call-manager|
@@ -186,15 +175,15 @@
 edc-model-wrapper_          |edc-model-wrapper|           |pypi-edc-model-wrapper|
 edc-navbar_                 |edc-navbar|                  |pypi-edc-navbar|
 edc-notification_           |edc-notification|            |pypi-edc-notification|
 edc-offstudy_               |edc-offstudy|                |pypi-edc-offstudy|
 edc-pdutils_                |edc-pdutils|                 |pypi-edc-pdutils|
 edc-prn_                    |edc-prn|                     |pypi-edc-prn|
 edc-protocol_               |edc-protocol|                |pypi-edc-protocol|
-edc-protocol-incident_      |edc-protocol-incident|       |pypi-edc-protocol-incident|
+edc-protocol-violation_     |edc-protocol-violation|      |pypi-edc-protocol-violation|
 edc-randomization_          |edc-randomization|           |pypi-edc-randomization|
 edc-reference_              |edc-reference|               |pypi-edc-reference|
 edc-registration_           |edc-registration|            |pypi-edc-registration|
 edc-reportable_             |edc-reportable|              |pypi-edc-reportable|
 edc-reports_                |edc-reports|                 |pypi-edc-reports|
 edc-review-dashboard_       |edc-review-dashboard|        |pypi-edc-review-dashboard|
 edc-screening_              |edc-screening|               |pypi-edc-screening|
@@ -213,21 +202,18 @@
 
 
 Contrib
 -------
 
 ========================== ============================== ==================================
 edc-adherence_              |edc-adherence|               |pypi-edc-adherence|
-edc-csf_                    |edc-csf|                     |pypi-edc-csf|
 edc-dx_                     |edc-dx|                      |pypi-edc-dx|
 edc-dx-review_              |edc-dx-review|               |pypi-edc-dx-review|
 edc-glucose_                |edc-glucose|                 |pypi-edc-glucose|
 edc-mnsi_                   |edc-mnsi|                    |pypi-edc-mnsi|
-edc-microbiology_           |edc-microbiology|            |pypi-edc-microbiology|
-edc-microscopy_             |edc-microscopy|              |pypi-edc-microscopy|
 edc-pharmacy_               |edc-pharmacy|                |pypi-edc-pharmacy|
 edc-pharmacy-dashboard_     |edc-pharmacy-dashboard|      |pypi-edc-pharmacy-dashboard|
 edc-vitals_                 |edc-vitals|                  |pypi-edc-vitals|
 ========================== ============================== ==================================
 
 Thanks to JetBrains for support with an opensource PyCharm IDE license. |jet-brains|
 
@@ -247,15 +233,14 @@
 .. _edc-adverse-event: https://github.com/clinicedc/edc-adverse-event
 .. _edc-appointment: https://github.com/clinicedc/edc-appointment
 .. _edc-auth: https://github.com/clinicedc/edc-auth
 .. _edc-call-manager: https://github.com/clinicedc/edc-call-manager
 .. _edc-consent: https://github.com/clinicedc/edc-consent
 .. _edc-constants: https://github.com/clinicedc/edc-constants
 .. _edc-crf: https://github.com/clinicedc/edc-crf
-.. _edc-csf: https://github.com/clinicedc/edc-csf
 .. _edc-dashboard: https://github.com/clinicedc/edc-dashboard
 .. _edc-data-manager: https://github.com/clinicedc/edc-data-manager
 .. _edc-device: https://github.com/clinicedc/edc-device
 .. _edc-dx: https://github.com/clinicedc/edc-dx
 .. _edc-dx-review: https://github.com/clinicedc/edc-dx-review
 .. _edc-egfr: https://github.com/clinicedc/edc-egfr
 .. _edc-export: https://github.com/clinicedc/edc-export
@@ -272,30 +257,28 @@
 .. _edc-lab-results: https://github.com/clinicedc/edc-lab-results
 .. _edc-label: https://github.com/clinicedc/edc-label
 .. _edc-list-data: https://github.com/clinicedc/edc-list-data
 .. _edc-locator: https://github.com/clinicedc/edc-locator
 .. _edc-ltfu: https://github.com/clinicedc/edc-ltfu
 .. _edc-metadata: https://github.com/clinicedc/edc-metadata
 .. _edc-mnsi: https://github.com/clinicedc/edc-mnsi
-.. _edc-microbiology: https://github.com/clinicedc/edc-microbiology
-.. _edc-microscopy: https://github.com/clinicedc/edc-microscopy
 .. _edc-model: https://github.com/clinicedc/edc-model
 .. _edc-model-admin: https://github.com/clinicedc/edc-model-admin
 .. _edc-model-fields: https://github.com/clinicedc/edc-model-fields
 .. _edc-model-form: https://github.com/clinicedc/edc-model-form
 .. _edc-model-wrapper: https://github.com/clinicedc/edc-model-wrapper
 .. _edc-navbar: https://github.com/clinicedc/edc-navbar
 .. _edc-notification: https://github.com/clinicedc/edc-notification
 .. _edc-offstudy: https://github.com/clinicedc/edc-offstudy
 .. _edc-pdutils: https://github.com/clinicedc/edc-pdutils
 .. _edc-pharmacy: https://github.com/clinicedc/edc-pharmacy
 .. _edc-pharmacy-dashboard: https://github.com/clinicedc/edc-pharmacy-dashboard
 .. _edc-prn: https://github.com/clinicedc/edc-prn
 .. _edc-protocol: https://github.com/clinicedc/edc-protocol
-.. _edc-protocol-incident: https://github.com/clinicedc/edc-protocol-incident
+.. _edc-protocol-violation: https://github.com/clinicedc/edc-protocol-violation
 .. _edc-randomization: https://github.com/clinicedc/edc-randomization
 .. _edc-reference: https://github.com/clinicedc/edc-reference
 .. _edc-refusal: https://github.com/clinicedc/edc-refusal
 .. _edc-registration: https://github.com/clinicedc/edc-registration
 .. _edc-reportable: https://github.com/clinicedc/edc-reportable
 .. _edc-reports: https://github.com/clinicedc/edc-reports
 .. _edc-review-dashboard: https://github.com/clinicedc/edc-review-dashboard
@@ -329,16 +312,14 @@
   :target: https://github.com/clinicedc/edc-call-manager/actions?query=workflow:build
 .. |edc-clinic| image:: https://github.com/clinicedc/edc-clinic/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-clinic/actions?query=workflow:build
 .. |edc-consent| image:: https://github.com/clinicedc/edc-consent/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-consent/actions?query=workflow:build
 .. |edc-crf| image:: https://github.com/clinicedc/edc-crf/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-crf/actions?query=workflow:build
-.. |edc-csf| image:: https://github.com/clinicedc/edc-csf/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-csf/actions?query=workflow:build
 .. |edc-dashboard| image:: https://github.com/clinicedc/edc-dashboard/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-dashboard/actions?query=workflow:build
 .. |edc-data-manager| image:: https://github.com/clinicedc/edc-data-manager/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-data-manager/actions?query=workflow:build
 .. |edc-device| image:: https://github.com/clinicedc/edc-device/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-device/actions?query=workflow:build
 .. |edc-dx| image:: https://github.com/clinicedc/edc-dx/workflows/build/badge.svg?branch=develop
@@ -379,18 +360,14 @@
   :target: https://github.com/clinicedc/edc-ltfu/actions?query=workflow:build
 .. |edc-metadata| image:: https://github.com/clinicedc/edc-metadata/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-metadata/actions?query=workflow:build
 .. |edc-metadata-rules| image:: https://github.com/clinicedc/edc-metadata-rules/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-metadata-rules/actions?query=workflow:build
 .. |edc-mnsi| image:: https://github.com/clinicedc/edc-mnsi/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-mnsi/actions?query=workflow:build
-.. |edc-microbiology| image:: https://github.com/clinicedc/edc-microbiology/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-microbiology/actions?query=workflow:build
-.. |edc-microscopy| image:: https://github.com/clinicedc/edc-microscopy/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-microscopy/actions?query=workflow:build
 .. |edc-model| image:: https://github.com/clinicedc/edc-model/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model/actions?query=workflow:build
 .. |edc-model-admin| image:: https://github.com/clinicedc/edc-model-admin/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model-admin/actions?query=workflow:build
 .. |edc-model-fields| image:: https://github.com/clinicedc/edc-model-fields/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model-fields/actions?query=workflow:build
 .. |edc-model-form| image:: https://github.com/clinicedc/edc-model-form/workflows/build/badge.svg?branch=develop
@@ -409,16 +386,16 @@
   :target: https://github.com/clinicedc/edc-pharmacy/actions?query=workflow:build
 .. |edc-pharmacy-dashboard| image:: https://github.com/clinicedc/edc-pharmacy-dashboard/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-pharmacy-dashboard/actions?query=workflow:build
 .. |edc-prn| image:: https://github.com/clinicedc/edc-prn/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-prn/actions?query=workflow:build
 .. |edc-protocol| image:: https://github.com/clinicedc/edc-protocol/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-protocol/actions?query=workflow:build
-.. |edc-protocol-incident| image:: https://github.com/clinicedc/edc-protocol-incident/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-protocol-incident/actions?query=workflow:build
+.. |edc-protocol-violation| image:: https://github.com/clinicedc/edc-protocol-violation/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-protocol-violation/actions?query=workflow:build
 .. |edc-randomization| image:: https://github.com/clinicedc/edc-randomization/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-randomization/actions?query=workflow:build
 .. |edc-reference| image:: https://github.com/clinicedc/edc-reference/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-reference/actions?query=workflow:build
 .. |edc-registration| image:: https://github.com/clinicedc/edc-registration/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-registration/actions?query=workflow:build
 .. |edc-reportable| image:: https://github.com/clinicedc/edc-reportable/workflows/build/badge.svg?branch=develop
@@ -468,16 +445,14 @@
     :target: https://pypi.python.org/pypi/edc-blood-results
 .. |pypi-edc-consent| image:: https://img.shields.io/pypi/v/edc-consent.svg
     :target: https://pypi.python.org/pypi/edc-consent
 .. |pypi-edc-constants| image:: https://img.shields.io/pypi/v/edc-constants.svg
     :target: https://pypi.python.org/pypi/edc-constants
 .. |pypi-edc-crf| image:: https://img.shields.io/pypi/v/edc-crf.svg
     :target: https://pypi.python.org/pypi/edc-crf
-.. |pypi-edc-csf| image:: https://img.shields.io/pypi/v/edc-csf.svg
-    :target: https://pypi.python.org/pypi/edc-csf
 .. |pypi-edc-dashboard| image:: https://img.shields.io/pypi/v/edc-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-dashboard
 .. |pypi-edc-data-manager| image:: https://img.shields.io/pypi/v/edc-data-manager.svg
     :target: https://pypi.python.org/pypi/edc-data-manager
 .. |pypi-edc-device| image:: https://img.shields.io/pypi/v/edc-device.svg
     :target: https://pypi.python.org/pypi/edc-device
 .. |pypi-edc-dx| image:: https://img.shields.io/pypi/v/edc-dx.svg
@@ -516,18 +491,14 @@
     :target: https://pypi.python.org/pypi/edc-locator
 .. |pypi-edc-ltfu| image:: https://img.shields.io/pypi/v/edc-ltfu.svg
     :target: https://pypi.python.org/pypi/edc-ltfu
 .. |pypi-edc-metadata| image:: https://img.shields.io/pypi/v/edc-metadata.svg
     :target: https://pypi.python.org/pypi/edc-metadata
 .. |pypi-edc-mnsi| image:: https://img.shields.io/pypi/v/edc-mnsi.svg
     :target: https://pypi.python.org/pypi/edc-mnsi
-.. |pypi-edc-microbiology| image:: https://img.shields.io/pypi/v/edc-microbiology.svg
-    :target: https://pypi.python.org/pypi/edc-microbiology
-.. |pypi-edc-microscopy| image:: https://img.shields.io/pypi/v/edc-microscopy.svg
-    :target: https://pypi.python.org/pypi/edc-microscopy
 .. |pypi-edc-model| image:: https://img.shields.io/pypi/v/edc-model.svg
     :target: https://pypi.python.org/pypi/edc-model
 .. |pypi-edc-model-admin| image:: https://img.shields.io/pypi/v/edc-model-admin.svg
     :target: https://pypi.python.org/pypi/edc-model-admin
 .. |pypi-edc-model-fields| image:: https://img.shields.io/pypi/v/edc-model-fields.svg
     :target: https://pypi.python.org/pypi/edc-model-fields
 .. |pypi-edc-model-form| image:: https://img.shields.io/pypi/v/edc-model-form.svg
@@ -546,16 +517,16 @@
     :target: https://pypi.python.org/pypi/edc-pharmacy
 .. |pypi-edc-pharmacy-dashboard| image:: https://img.shields.io/pypi/v/edc-pharmacy-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-pharmacy-dashboard
 .. |pypi-edc-prn| image:: https://img.shields.io/pypi/v/edc-prn.svg
     :target: https://pypi.python.org/pypi/edc-prn
 .. |pypi-edc-protocol| image:: https://img.shields.io/pypi/v/edc-protocol.svg
     :target: https://pypi.python.org/pypi/edc-protocol
-.. |pypi-edc-protocol-incident| image:: https://img.shields.io/pypi/v/edc-protocol-incident.svg
-    :target: https://pypi.python.org/pypi/edc-protocol-incident
+.. |pypi-edc-protocol-violation| image:: https://img.shields.io/pypi/v/edc-protocol-violation.svg
+    :target: https://pypi.python.org/pypi/edc-protocol-violation
 .. |pypi-edc-randomization| image:: https://img.shields.io/pypi/v/edc-randomization.svg
     :target: https://pypi.python.org/pypi/edc-randomization
 .. |pypi-edc-reference| image:: https://img.shields.io/pypi/v/edc-reference.svg
     :target: https://pypi.python.org/pypi/edc-reference
 .. |pypi-edc-registration| image:: https://img.shields.io/pypi/v/edc-registration.svg
     :target: https://pypi.python.org/pypi/edc-registration
 .. |pypi-edc-reportable| image:: https://img.shields.io/pypi/v/edc-reportable.svg
@@ -588,9 +559,9 @@
     :target: https://pypi.python.org/pypi/edc-visit-schedule
 .. |pypi-edc-visit-tracking| image:: https://img.shields.io/pypi/v/edc-visit-tracking.svg
     :target: https://pypi.python.org/pypi/edc-visit-tracking
 .. |pypi-edc-vitals| image:: https://img.shields.io/pypi/v/edc-vitals.svg
     :target: https://pypi.python.org/pypi/edc-vitals
 .. |jet-brains| image:: https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm_icon.png
     :target: https://jb.gg/OpenSource
-    :width: 25
+    :width: 120
     :alt: JetBrains PyCharm
```

### Comparing `edc-0.4.88/README.rst` & `edc-0.4.9/edc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,47 @@
-|pypi| |downloads|
-
-clinicedc
-=========
+Metadata-Version: 2.1
+Name: edc
+Version: 0.4.9
+Summary: EDC core modules for clinicedc/edc projects.
+Home-page: https://github.com/clinicedc/edc
+Author: Erik van Widenfelt
+Author-email: ew2789@gmail.com
+License: GPL license, see LICENSE
+Keywords: django edc clinical trials research
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
 
-Here are a set of python modules that extend Django to empower you to build an EDC / eSource system to handle data
-collection and management for multi-site longitudinal clinical trials.
+|pypi| |downloads|
 
-Refer to the specific open projects listed below for example EDC systems built with these modules.
-The more recent the trial the better the example.
+Clinic EDC
+==========
 
-The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
-the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
-`Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
-in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials have been related to HIV/AIDS research. Recent work with the
-`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM),
-Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
-three main chronic conditions -- HIV/DM/HTN.
+``Clinic EDC`` contains complete code for a set of core modules for clinical trial data management to build a trial EDC. Refer to the specific open projects listed below for example EDC systems built with these modules. The more recent the trial the better the example. The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__ in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__. Almost all trials have been related to HIV/AIDS research. Recent work with the `Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM), Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
 
-The ``clinicedc`` for each trial consists of a subset of trial-specific modules that reference this module.
+The ``Clinic EDC`` for each trial consists of a subset of trial-specific modules that reference this module.
 
-(python 3.10+ and Django 4.1, see setup.cfg)
+(python 3.9 and Django 3.2+ required, see setup.cfg)
 
 
 Projects that use the EDC
 -------------------------
 Recent examples of EDC's using this codebase:
 
 INTECOMM
@@ -120,15 +133,15 @@
 Start with main repo `bcpp`
 
 Contacts
 --------
 
 For further information go to https://github.com/erikvw.
 
-|django| |jet-brains|
+|django|
 
 =========================== ============================= ==================================
 edc-action-item_            |edc-action-item|             |pypi-edc-action-item|
 edc-adverse-event_          |edc-adverse-event|           |pypi-edc-adverse-event|
 edc-appointment_            |edc-appointment|             |pypi-edc-appointment|
 edc-auth_                   |edc-auth|                    |pypi-edc-auth|
 edc-call-manager_           |edc-call-manager|
@@ -162,15 +175,15 @@
 edc-model-wrapper_          |edc-model-wrapper|           |pypi-edc-model-wrapper|
 edc-navbar_                 |edc-navbar|                  |pypi-edc-navbar|
 edc-notification_           |edc-notification|            |pypi-edc-notification|
 edc-offstudy_               |edc-offstudy|                |pypi-edc-offstudy|
 edc-pdutils_                |edc-pdutils|                 |pypi-edc-pdutils|
 edc-prn_                    |edc-prn|                     |pypi-edc-prn|
 edc-protocol_               |edc-protocol|                |pypi-edc-protocol|
-edc-protocol-incident_      |edc-protocol-incident|       |pypi-edc-protocol-incident|
+edc-protocol-violation_     |edc-protocol-violation|      |pypi-edc-protocol-violation|
 edc-randomization_          |edc-randomization|           |pypi-edc-randomization|
 edc-reference_              |edc-reference|               |pypi-edc-reference|
 edc-registration_           |edc-registration|            |pypi-edc-registration|
 edc-reportable_             |edc-reportable|              |pypi-edc-reportable|
 edc-reports_                |edc-reports|                 |pypi-edc-reports|
 edc-review-dashboard_       |edc-review-dashboard|        |pypi-edc-review-dashboard|
 edc-screening_              |edc-screening|               |pypi-edc-screening|
@@ -189,21 +202,18 @@
 
 
 Contrib
 -------
 
 ========================== ============================== ==================================
 edc-adherence_              |edc-adherence|               |pypi-edc-adherence|
-edc-csf_                    |edc-csf|                     |pypi-edc-csf|
 edc-dx_                     |edc-dx|                      |pypi-edc-dx|
 edc-dx-review_              |edc-dx-review|               |pypi-edc-dx-review|
 edc-glucose_                |edc-glucose|                 |pypi-edc-glucose|
 edc-mnsi_                   |edc-mnsi|                    |pypi-edc-mnsi|
-edc-microbiology_           |edc-microbiology|            |pypi-edc-microbiology|
-edc-microscopy_             |edc-microscopy|              |pypi-edc-microscopy|
 edc-pharmacy_               |edc-pharmacy|                |pypi-edc-pharmacy|
 edc-pharmacy-dashboard_     |edc-pharmacy-dashboard|      |pypi-edc-pharmacy-dashboard|
 edc-vitals_                 |edc-vitals|                  |pypi-edc-vitals|
 ========================== ============================== ==================================
 
 Thanks to JetBrains for support with an opensource PyCharm IDE license. |jet-brains|
 
@@ -223,15 +233,14 @@
 .. _edc-adverse-event: https://github.com/clinicedc/edc-adverse-event
 .. _edc-appointment: https://github.com/clinicedc/edc-appointment
 .. _edc-auth: https://github.com/clinicedc/edc-auth
 .. _edc-call-manager: https://github.com/clinicedc/edc-call-manager
 .. _edc-consent: https://github.com/clinicedc/edc-consent
 .. _edc-constants: https://github.com/clinicedc/edc-constants
 .. _edc-crf: https://github.com/clinicedc/edc-crf
-.. _edc-csf: https://github.com/clinicedc/edc-csf
 .. _edc-dashboard: https://github.com/clinicedc/edc-dashboard
 .. _edc-data-manager: https://github.com/clinicedc/edc-data-manager
 .. _edc-device: https://github.com/clinicedc/edc-device
 .. _edc-dx: https://github.com/clinicedc/edc-dx
 .. _edc-dx-review: https://github.com/clinicedc/edc-dx-review
 .. _edc-egfr: https://github.com/clinicedc/edc-egfr
 .. _edc-export: https://github.com/clinicedc/edc-export
@@ -248,30 +257,28 @@
 .. _edc-lab-results: https://github.com/clinicedc/edc-lab-results
 .. _edc-label: https://github.com/clinicedc/edc-label
 .. _edc-list-data: https://github.com/clinicedc/edc-list-data
 .. _edc-locator: https://github.com/clinicedc/edc-locator
 .. _edc-ltfu: https://github.com/clinicedc/edc-ltfu
 .. _edc-metadata: https://github.com/clinicedc/edc-metadata
 .. _edc-mnsi: https://github.com/clinicedc/edc-mnsi
-.. _edc-microbiology: https://github.com/clinicedc/edc-microbiology
-.. _edc-microscopy: https://github.com/clinicedc/edc-microscopy
 .. _edc-model: https://github.com/clinicedc/edc-model
 .. _edc-model-admin: https://github.com/clinicedc/edc-model-admin
 .. _edc-model-fields: https://github.com/clinicedc/edc-model-fields
 .. _edc-model-form: https://github.com/clinicedc/edc-model-form
 .. _edc-model-wrapper: https://github.com/clinicedc/edc-model-wrapper
 .. _edc-navbar: https://github.com/clinicedc/edc-navbar
 .. _edc-notification: https://github.com/clinicedc/edc-notification
 .. _edc-offstudy: https://github.com/clinicedc/edc-offstudy
 .. _edc-pdutils: https://github.com/clinicedc/edc-pdutils
 .. _edc-pharmacy: https://github.com/clinicedc/edc-pharmacy
 .. _edc-pharmacy-dashboard: https://github.com/clinicedc/edc-pharmacy-dashboard
 .. _edc-prn: https://github.com/clinicedc/edc-prn
 .. _edc-protocol: https://github.com/clinicedc/edc-protocol
-.. _edc-protocol-incident: https://github.com/clinicedc/edc-protocol-incident
+.. _edc-protocol-violation: https://github.com/clinicedc/edc-protocol-violation
 .. _edc-randomization: https://github.com/clinicedc/edc-randomization
 .. _edc-reference: https://github.com/clinicedc/edc-reference
 .. _edc-refusal: https://github.com/clinicedc/edc-refusal
 .. _edc-registration: https://github.com/clinicedc/edc-registration
 .. _edc-reportable: https://github.com/clinicedc/edc-reportable
 .. _edc-reports: https://github.com/clinicedc/edc-reports
 .. _edc-review-dashboard: https://github.com/clinicedc/edc-review-dashboard
@@ -305,16 +312,14 @@
   :target: https://github.com/clinicedc/edc-call-manager/actions?query=workflow:build
 .. |edc-clinic| image:: https://github.com/clinicedc/edc-clinic/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-clinic/actions?query=workflow:build
 .. |edc-consent| image:: https://github.com/clinicedc/edc-consent/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-consent/actions?query=workflow:build
 .. |edc-crf| image:: https://github.com/clinicedc/edc-crf/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-crf/actions?query=workflow:build
-.. |edc-csf| image:: https://github.com/clinicedc/edc-csf/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-csf/actions?query=workflow:build
 .. |edc-dashboard| image:: https://github.com/clinicedc/edc-dashboard/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-dashboard/actions?query=workflow:build
 .. |edc-data-manager| image:: https://github.com/clinicedc/edc-data-manager/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-data-manager/actions?query=workflow:build
 .. |edc-device| image:: https://github.com/clinicedc/edc-device/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-device/actions?query=workflow:build
 .. |edc-dx| image:: https://github.com/clinicedc/edc-dx/workflows/build/badge.svg?branch=develop
@@ -355,18 +360,14 @@
   :target: https://github.com/clinicedc/edc-ltfu/actions?query=workflow:build
 .. |edc-metadata| image:: https://github.com/clinicedc/edc-metadata/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-metadata/actions?query=workflow:build
 .. |edc-metadata-rules| image:: https://github.com/clinicedc/edc-metadata-rules/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-metadata-rules/actions?query=workflow:build
 .. |edc-mnsi| image:: https://github.com/clinicedc/edc-mnsi/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-mnsi/actions?query=workflow:build
-.. |edc-microbiology| image:: https://github.com/clinicedc/edc-microbiology/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-microbiology/actions?query=workflow:build
-.. |edc-microscopy| image:: https://github.com/clinicedc/edc-microscopy/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-microscopy/actions?query=workflow:build
 .. |edc-model| image:: https://github.com/clinicedc/edc-model/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model/actions?query=workflow:build
 .. |edc-model-admin| image:: https://github.com/clinicedc/edc-model-admin/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model-admin/actions?query=workflow:build
 .. |edc-model-fields| image:: https://github.com/clinicedc/edc-model-fields/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model-fields/actions?query=workflow:build
 .. |edc-model-form| image:: https://github.com/clinicedc/edc-model-form/workflows/build/badge.svg?branch=develop
@@ -385,16 +386,16 @@
   :target: https://github.com/clinicedc/edc-pharmacy/actions?query=workflow:build
 .. |edc-pharmacy-dashboard| image:: https://github.com/clinicedc/edc-pharmacy-dashboard/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-pharmacy-dashboard/actions?query=workflow:build
 .. |edc-prn| image:: https://github.com/clinicedc/edc-prn/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-prn/actions?query=workflow:build
 .. |edc-protocol| image:: https://github.com/clinicedc/edc-protocol/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-protocol/actions?query=workflow:build
-.. |edc-protocol-incident| image:: https://github.com/clinicedc/edc-protocol-incident/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-protocol-incident/actions?query=workflow:build
+.. |edc-protocol-violation| image:: https://github.com/clinicedc/edc-protocol-violation/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-protocol-violation/actions?query=workflow:build
 .. |edc-randomization| image:: https://github.com/clinicedc/edc-randomization/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-randomization/actions?query=workflow:build
 .. |edc-reference| image:: https://github.com/clinicedc/edc-reference/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-reference/actions?query=workflow:build
 .. |edc-registration| image:: https://github.com/clinicedc/edc-registration/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-registration/actions?query=workflow:build
 .. |edc-reportable| image:: https://github.com/clinicedc/edc-reportable/workflows/build/badge.svg?branch=develop
@@ -444,16 +445,14 @@
     :target: https://pypi.python.org/pypi/edc-blood-results
 .. |pypi-edc-consent| image:: https://img.shields.io/pypi/v/edc-consent.svg
     :target: https://pypi.python.org/pypi/edc-consent
 .. |pypi-edc-constants| image:: https://img.shields.io/pypi/v/edc-constants.svg
     :target: https://pypi.python.org/pypi/edc-constants
 .. |pypi-edc-crf| image:: https://img.shields.io/pypi/v/edc-crf.svg
     :target: https://pypi.python.org/pypi/edc-crf
-.. |pypi-edc-csf| image:: https://img.shields.io/pypi/v/edc-csf.svg
-    :target: https://pypi.python.org/pypi/edc-csf
 .. |pypi-edc-dashboard| image:: https://img.shields.io/pypi/v/edc-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-dashboard
 .. |pypi-edc-data-manager| image:: https://img.shields.io/pypi/v/edc-data-manager.svg
     :target: https://pypi.python.org/pypi/edc-data-manager
 .. |pypi-edc-device| image:: https://img.shields.io/pypi/v/edc-device.svg
     :target: https://pypi.python.org/pypi/edc-device
 .. |pypi-edc-dx| image:: https://img.shields.io/pypi/v/edc-dx.svg
@@ -492,18 +491,14 @@
     :target: https://pypi.python.org/pypi/edc-locator
 .. |pypi-edc-ltfu| image:: https://img.shields.io/pypi/v/edc-ltfu.svg
     :target: https://pypi.python.org/pypi/edc-ltfu
 .. |pypi-edc-metadata| image:: https://img.shields.io/pypi/v/edc-metadata.svg
     :target: https://pypi.python.org/pypi/edc-metadata
 .. |pypi-edc-mnsi| image:: https://img.shields.io/pypi/v/edc-mnsi.svg
     :target: https://pypi.python.org/pypi/edc-mnsi
-.. |pypi-edc-microbiology| image:: https://img.shields.io/pypi/v/edc-microbiology.svg
-    :target: https://pypi.python.org/pypi/edc-microbiology
-.. |pypi-edc-microscopy| image:: https://img.shields.io/pypi/v/edc-microscopy.svg
-    :target: https://pypi.python.org/pypi/edc-microscopy
 .. |pypi-edc-model| image:: https://img.shields.io/pypi/v/edc-model.svg
     :target: https://pypi.python.org/pypi/edc-model
 .. |pypi-edc-model-admin| image:: https://img.shields.io/pypi/v/edc-model-admin.svg
     :target: https://pypi.python.org/pypi/edc-model-admin
 .. |pypi-edc-model-fields| image:: https://img.shields.io/pypi/v/edc-model-fields.svg
     :target: https://pypi.python.org/pypi/edc-model-fields
 .. |pypi-edc-model-form| image:: https://img.shields.io/pypi/v/edc-model-form.svg
@@ -522,16 +517,16 @@
     :target: https://pypi.python.org/pypi/edc-pharmacy
 .. |pypi-edc-pharmacy-dashboard| image:: https://img.shields.io/pypi/v/edc-pharmacy-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-pharmacy-dashboard
 .. |pypi-edc-prn| image:: https://img.shields.io/pypi/v/edc-prn.svg
     :target: https://pypi.python.org/pypi/edc-prn
 .. |pypi-edc-protocol| image:: https://img.shields.io/pypi/v/edc-protocol.svg
     :target: https://pypi.python.org/pypi/edc-protocol
-.. |pypi-edc-protocol-incident| image:: https://img.shields.io/pypi/v/edc-protocol-incident.svg
-    :target: https://pypi.python.org/pypi/edc-protocol-incident
+.. |pypi-edc-protocol-violation| image:: https://img.shields.io/pypi/v/edc-protocol-violation.svg
+    :target: https://pypi.python.org/pypi/edc-protocol-violation
 .. |pypi-edc-randomization| image:: https://img.shields.io/pypi/v/edc-randomization.svg
     :target: https://pypi.python.org/pypi/edc-randomization
 .. |pypi-edc-reference| image:: https://img.shields.io/pypi/v/edc-reference.svg
     :target: https://pypi.python.org/pypi/edc-reference
 .. |pypi-edc-registration| image:: https://img.shields.io/pypi/v/edc-registration.svg
     :target: https://pypi.python.org/pypi/edc-registration
 .. |pypi-edc-reportable| image:: https://img.shields.io/pypi/v/edc-reportable.svg
@@ -564,9 +559,9 @@
     :target: https://pypi.python.org/pypi/edc-visit-schedule
 .. |pypi-edc-visit-tracking| image:: https://img.shields.io/pypi/v/edc-visit-tracking.svg
     :target: https://pypi.python.org/pypi/edc-visit-tracking
 .. |pypi-edc-vitals| image:: https://img.shields.io/pypi/v/edc-vitals.svg
     :target: https://pypi.python.org/pypi/edc-vitals
 .. |jet-brains| image:: https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm_icon.png
     :target: https://jb.gg/OpenSource
-    :width: 25
+    :width: 120
     :alt: JetBrains PyCharm
```

### Comparing `edc-0.4.88/bin/nginx/edc-uat.conf` & `edc-0.4.9/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/bin/nginx/edc.conf` & `edc-0.4.9/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/bin/scripts/dev_repos.sh` & `edc-0.4.9/bin/scripts/dev_repos.sh`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pip install gunicorn
 pip install inflect
 pip install mysqlclient
 pip install pyrabbit
 pip install python-dateutil
 pip install python-memcached
 pip install reportlab
+pip uninstall sentry_sdk
 pip install tqdm
 pip install django-environ
 pip install django-redis
 pip install django-audit-fields
 pip install django-celery-beat
 pip install django-celery-results
 pip install django-crypto-fields
```

### Comparing `edc-0.4.88/bin/scripts/update_edc.sh` & `edc-0.4.9/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/bin/systemd/celery-uat.service` & `edc-0.4.9/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/bin/systemd/celery.service` & `edc-0.4.9/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/backup.rst` & `edc-0.4.9/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/celery.rst` & `edc-0.4.9/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/conda.rst` & `edc-0.4.9/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/configure_web_services.rst` & `edc-0.4.9/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/deploy_new_droplet.rst` & `edc-0.4.9/docs/deploy_new_droplet.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 Update the DB
 =============
 
 Configure access to mysql on the db droplet
 +++++++++++++++++++++++++++++++++++++++++++
 
-To allow the new droplet to access the database, you need to configure both the firewall and the ``mysql`` database permissions.
+To allow the new droplet to access the database, you need to confugre both the firewall and the ``mysql`` database permissions.
 
 Log in to the ``db`` droplet
 
 Update ``mysql`` USER and privileges
 
 .. code-block:: bash
 
-  mysql> CREATE USER 'edc-<host-desc>'@'x.x.x.x' IDENTIFIED BY 'password'; FLUSH PRIVILEGES;
+  mysql> CREATE USER 'edc'@'x.x.x.x' IDENTIFIED BY 'password'; FLUSH PRIVILEGES;
   Query OK, 0 rows affected (0.00 sec)
 
-  mysql> GRANT ALL PRIVILEGES ON `<database_name>`.* TO 'edc-<host-desc>'@'x.x.x.x';
+  mysql> GRANT ALL PRIVILEGES ON *.* TO 'edc'@'x.x.x.x' WITH GRANT OPTION;
   Query OK, 0 rows affected (0.00 sec)
 
 
 Open the DO firewall on the ``db`` to allow access from this droplet on its private IP.
 
 Switch back to your new droplet and confirm that you can connect to mysql:
 
@@ -154,7 +154,9 @@
   $ sudo nginx -t
 
 Restart nginx
 
 .. code-block:: bash
 
   $ sudo systemctl reload nginx
+
+
```

### Comparing `edc-0.4.88/docs/exporting_encrypted_data.rst` & `edc-0.4.9/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/forms_reference.md` & `edc-0.4.9/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/landing_page.rst` & `edc-0.4.9/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/printing.rst` & `edc-0.4.9/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/docs/update_deployment.rst` & `edc-0.4.9/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/edc.egg-info/PKG-INFO` & `edc-0.4.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,21 @@
-Metadata-Version: 2.1
-Name: edc
-Version: 0.4.88
-Summary: EDC core modules for clinicedc/edc projects.
-Home-page: https://github.com/clinicedc/edc
-Author: Erik van Widenfelt
-Author-email: ew2789@gmail.com
-License: GPL license, see LICENSE
-Keywords: django edc clinical trials research
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS
-
 |pypi| |downloads|
 
-clinicedc
-=========
-
-Here are a set of python modules that extend Django to empower you to build an EDC / eSource system to handle data
-collection and management for multi-site longitudinal clinical trials.
-
-Refer to the specific open projects listed below for example EDC systems built with these modules.
-The more recent the trial the better the example.
+Clinic EDC
+==========
 
-The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
-the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
-`Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
-in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials have been related to HIV/AIDS research. Recent work with the
-`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM),
-Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
-three main chronic conditions -- HIV/DM/HTN.
+``Clinic EDC`` contains complete code for a set of core modules for clinical trial data management to build a trial EDC. Refer to the specific open projects listed below for example EDC systems built with these modules. The more recent the trial the better the example. The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__ in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__. Almost all trials have been related to HIV/AIDS research. Recent work with the `Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM), Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
 
-The ``clinicedc`` for each trial consists of a subset of trial-specific modules that reference this module.
+The ``Clinic EDC`` for each trial consists of a subset of trial-specific modules that reference this module.
 
-(python 3.10+ and Django 4.1, see setup.cfg)
+(python 3.9 and Django 3.2+ required, see setup.cfg)
 
 
 Projects that use the EDC
 -------------------------
 Recent examples of EDC's using this codebase:
 
 INTECOMM
@@ -144,15 +107,15 @@
 Start with main repo `bcpp`
 
 Contacts
 --------
 
 For further information go to https://github.com/erikvw.
 
-|django| |jet-brains|
+|django|
 
 =========================== ============================= ==================================
 edc-action-item_            |edc-action-item|             |pypi-edc-action-item|
 edc-adverse-event_          |edc-adverse-event|           |pypi-edc-adverse-event|
 edc-appointment_            |edc-appointment|             |pypi-edc-appointment|
 edc-auth_                   |edc-auth|                    |pypi-edc-auth|
 edc-call-manager_           |edc-call-manager|
@@ -186,15 +149,15 @@
 edc-model-wrapper_          |edc-model-wrapper|           |pypi-edc-model-wrapper|
 edc-navbar_                 |edc-navbar|                  |pypi-edc-navbar|
 edc-notification_           |edc-notification|            |pypi-edc-notification|
 edc-offstudy_               |edc-offstudy|                |pypi-edc-offstudy|
 edc-pdutils_                |edc-pdutils|                 |pypi-edc-pdutils|
 edc-prn_                    |edc-prn|                     |pypi-edc-prn|
 edc-protocol_               |edc-protocol|                |pypi-edc-protocol|
-edc-protocol-incident_      |edc-protocol-incident|       |pypi-edc-protocol-incident|
+edc-protocol-violation_     |edc-protocol-violation|      |pypi-edc-protocol-violation|
 edc-randomization_          |edc-randomization|           |pypi-edc-randomization|
 edc-reference_              |edc-reference|               |pypi-edc-reference|
 edc-registration_           |edc-registration|            |pypi-edc-registration|
 edc-reportable_             |edc-reportable|              |pypi-edc-reportable|
 edc-reports_                |edc-reports|                 |pypi-edc-reports|
 edc-review-dashboard_       |edc-review-dashboard|        |pypi-edc-review-dashboard|
 edc-screening_              |edc-screening|               |pypi-edc-screening|
@@ -213,21 +176,18 @@
 
 
 Contrib
 -------
 
 ========================== ============================== ==================================
 edc-adherence_              |edc-adherence|               |pypi-edc-adherence|
-edc-csf_                    |edc-csf|                     |pypi-edc-csf|
 edc-dx_                     |edc-dx|                      |pypi-edc-dx|
 edc-dx-review_              |edc-dx-review|               |pypi-edc-dx-review|
 edc-glucose_                |edc-glucose|                 |pypi-edc-glucose|
 edc-mnsi_                   |edc-mnsi|                    |pypi-edc-mnsi|
-edc-microbiology_           |edc-microbiology|            |pypi-edc-microbiology|
-edc-microscopy_             |edc-microscopy|              |pypi-edc-microscopy|
 edc-pharmacy_               |edc-pharmacy|                |pypi-edc-pharmacy|
 edc-pharmacy-dashboard_     |edc-pharmacy-dashboard|      |pypi-edc-pharmacy-dashboard|
 edc-vitals_                 |edc-vitals|                  |pypi-edc-vitals|
 ========================== ============================== ==================================
 
 Thanks to JetBrains for support with an opensource PyCharm IDE license. |jet-brains|
 
@@ -247,15 +207,14 @@
 .. _edc-adverse-event: https://github.com/clinicedc/edc-adverse-event
 .. _edc-appointment: https://github.com/clinicedc/edc-appointment
 .. _edc-auth: https://github.com/clinicedc/edc-auth
 .. _edc-call-manager: https://github.com/clinicedc/edc-call-manager
 .. _edc-consent: https://github.com/clinicedc/edc-consent
 .. _edc-constants: https://github.com/clinicedc/edc-constants
 .. _edc-crf: https://github.com/clinicedc/edc-crf
-.. _edc-csf: https://github.com/clinicedc/edc-csf
 .. _edc-dashboard: https://github.com/clinicedc/edc-dashboard
 .. _edc-data-manager: https://github.com/clinicedc/edc-data-manager
 .. _edc-device: https://github.com/clinicedc/edc-device
 .. _edc-dx: https://github.com/clinicedc/edc-dx
 .. _edc-dx-review: https://github.com/clinicedc/edc-dx-review
 .. _edc-egfr: https://github.com/clinicedc/edc-egfr
 .. _edc-export: https://github.com/clinicedc/edc-export
@@ -272,30 +231,28 @@
 .. _edc-lab-results: https://github.com/clinicedc/edc-lab-results
 .. _edc-label: https://github.com/clinicedc/edc-label
 .. _edc-list-data: https://github.com/clinicedc/edc-list-data
 .. _edc-locator: https://github.com/clinicedc/edc-locator
 .. _edc-ltfu: https://github.com/clinicedc/edc-ltfu
 .. _edc-metadata: https://github.com/clinicedc/edc-metadata
 .. _edc-mnsi: https://github.com/clinicedc/edc-mnsi
-.. _edc-microbiology: https://github.com/clinicedc/edc-microbiology
-.. _edc-microscopy: https://github.com/clinicedc/edc-microscopy
 .. _edc-model: https://github.com/clinicedc/edc-model
 .. _edc-model-admin: https://github.com/clinicedc/edc-model-admin
 .. _edc-model-fields: https://github.com/clinicedc/edc-model-fields
 .. _edc-model-form: https://github.com/clinicedc/edc-model-form
 .. _edc-model-wrapper: https://github.com/clinicedc/edc-model-wrapper
 .. _edc-navbar: https://github.com/clinicedc/edc-navbar
 .. _edc-notification: https://github.com/clinicedc/edc-notification
 .. _edc-offstudy: https://github.com/clinicedc/edc-offstudy
 .. _edc-pdutils: https://github.com/clinicedc/edc-pdutils
 .. _edc-pharmacy: https://github.com/clinicedc/edc-pharmacy
 .. _edc-pharmacy-dashboard: https://github.com/clinicedc/edc-pharmacy-dashboard
 .. _edc-prn: https://github.com/clinicedc/edc-prn
 .. _edc-protocol: https://github.com/clinicedc/edc-protocol
-.. _edc-protocol-incident: https://github.com/clinicedc/edc-protocol-incident
+.. _edc-protocol-violation: https://github.com/clinicedc/edc-protocol-violation
 .. _edc-randomization: https://github.com/clinicedc/edc-randomization
 .. _edc-reference: https://github.com/clinicedc/edc-reference
 .. _edc-refusal: https://github.com/clinicedc/edc-refusal
 .. _edc-registration: https://github.com/clinicedc/edc-registration
 .. _edc-reportable: https://github.com/clinicedc/edc-reportable
 .. _edc-reports: https://github.com/clinicedc/edc-reports
 .. _edc-review-dashboard: https://github.com/clinicedc/edc-review-dashboard
@@ -329,16 +286,14 @@
   :target: https://github.com/clinicedc/edc-call-manager/actions?query=workflow:build
 .. |edc-clinic| image:: https://github.com/clinicedc/edc-clinic/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-clinic/actions?query=workflow:build
 .. |edc-consent| image:: https://github.com/clinicedc/edc-consent/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-consent/actions?query=workflow:build
 .. |edc-crf| image:: https://github.com/clinicedc/edc-crf/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-crf/actions?query=workflow:build
-.. |edc-csf| image:: https://github.com/clinicedc/edc-csf/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-csf/actions?query=workflow:build
 .. |edc-dashboard| image:: https://github.com/clinicedc/edc-dashboard/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-dashboard/actions?query=workflow:build
 .. |edc-data-manager| image:: https://github.com/clinicedc/edc-data-manager/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-data-manager/actions?query=workflow:build
 .. |edc-device| image:: https://github.com/clinicedc/edc-device/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-device/actions?query=workflow:build
 .. |edc-dx| image:: https://github.com/clinicedc/edc-dx/workflows/build/badge.svg?branch=develop
@@ -379,18 +334,14 @@
   :target: https://github.com/clinicedc/edc-ltfu/actions?query=workflow:build
 .. |edc-metadata| image:: https://github.com/clinicedc/edc-metadata/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-metadata/actions?query=workflow:build
 .. |edc-metadata-rules| image:: https://github.com/clinicedc/edc-metadata-rules/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-metadata-rules/actions?query=workflow:build
 .. |edc-mnsi| image:: https://github.com/clinicedc/edc-mnsi/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-mnsi/actions?query=workflow:build
-.. |edc-microbiology| image:: https://github.com/clinicedc/edc-microbiology/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-microbiology/actions?query=workflow:build
-.. |edc-microscopy| image:: https://github.com/clinicedc/edc-microscopy/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-microscopy/actions?query=workflow:build
 .. |edc-model| image:: https://github.com/clinicedc/edc-model/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model/actions?query=workflow:build
 .. |edc-model-admin| image:: https://github.com/clinicedc/edc-model-admin/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model-admin/actions?query=workflow:build
 .. |edc-model-fields| image:: https://github.com/clinicedc/edc-model-fields/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-model-fields/actions?query=workflow:build
 .. |edc-model-form| image:: https://github.com/clinicedc/edc-model-form/workflows/build/badge.svg?branch=develop
@@ -409,16 +360,16 @@
   :target: https://github.com/clinicedc/edc-pharmacy/actions?query=workflow:build
 .. |edc-pharmacy-dashboard| image:: https://github.com/clinicedc/edc-pharmacy-dashboard/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-pharmacy-dashboard/actions?query=workflow:build
 .. |edc-prn| image:: https://github.com/clinicedc/edc-prn/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-prn/actions?query=workflow:build
 .. |edc-protocol| image:: https://github.com/clinicedc/edc-protocol/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-protocol/actions?query=workflow:build
-.. |edc-protocol-incident| image:: https://github.com/clinicedc/edc-protocol-incident/workflows/build/badge.svg?branch=develop
-  :target: https://github.com/clinicedc/edc-protocol-incident/actions?query=workflow:build
+.. |edc-protocol-violation| image:: https://github.com/clinicedc/edc-protocol-violation/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-protocol-violation/actions?query=workflow:build
 .. |edc-randomization| image:: https://github.com/clinicedc/edc-randomization/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-randomization/actions?query=workflow:build
 .. |edc-reference| image:: https://github.com/clinicedc/edc-reference/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-reference/actions?query=workflow:build
 .. |edc-registration| image:: https://github.com/clinicedc/edc-registration/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-registration/actions?query=workflow:build
 .. |edc-reportable| image:: https://github.com/clinicedc/edc-reportable/workflows/build/badge.svg?branch=develop
@@ -468,16 +419,14 @@
     :target: https://pypi.python.org/pypi/edc-blood-results
 .. |pypi-edc-consent| image:: https://img.shields.io/pypi/v/edc-consent.svg
     :target: https://pypi.python.org/pypi/edc-consent
 .. |pypi-edc-constants| image:: https://img.shields.io/pypi/v/edc-constants.svg
     :target: https://pypi.python.org/pypi/edc-constants
 .. |pypi-edc-crf| image:: https://img.shields.io/pypi/v/edc-crf.svg
     :target: https://pypi.python.org/pypi/edc-crf
-.. |pypi-edc-csf| image:: https://img.shields.io/pypi/v/edc-csf.svg
-    :target: https://pypi.python.org/pypi/edc-csf
 .. |pypi-edc-dashboard| image:: https://img.shields.io/pypi/v/edc-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-dashboard
 .. |pypi-edc-data-manager| image:: https://img.shields.io/pypi/v/edc-data-manager.svg
     :target: https://pypi.python.org/pypi/edc-data-manager
 .. |pypi-edc-device| image:: https://img.shields.io/pypi/v/edc-device.svg
     :target: https://pypi.python.org/pypi/edc-device
 .. |pypi-edc-dx| image:: https://img.shields.io/pypi/v/edc-dx.svg
@@ -516,18 +465,14 @@
     :target: https://pypi.python.org/pypi/edc-locator
 .. |pypi-edc-ltfu| image:: https://img.shields.io/pypi/v/edc-ltfu.svg
     :target: https://pypi.python.org/pypi/edc-ltfu
 .. |pypi-edc-metadata| image:: https://img.shields.io/pypi/v/edc-metadata.svg
     :target: https://pypi.python.org/pypi/edc-metadata
 .. |pypi-edc-mnsi| image:: https://img.shields.io/pypi/v/edc-mnsi.svg
     :target: https://pypi.python.org/pypi/edc-mnsi
-.. |pypi-edc-microbiology| image:: https://img.shields.io/pypi/v/edc-microbiology.svg
-    :target: https://pypi.python.org/pypi/edc-microbiology
-.. |pypi-edc-microscopy| image:: https://img.shields.io/pypi/v/edc-microscopy.svg
-    :target: https://pypi.python.org/pypi/edc-microscopy
 .. |pypi-edc-model| image:: https://img.shields.io/pypi/v/edc-model.svg
     :target: https://pypi.python.org/pypi/edc-model
 .. |pypi-edc-model-admin| image:: https://img.shields.io/pypi/v/edc-model-admin.svg
     :target: https://pypi.python.org/pypi/edc-model-admin
 .. |pypi-edc-model-fields| image:: https://img.shields.io/pypi/v/edc-model-fields.svg
     :target: https://pypi.python.org/pypi/edc-model-fields
 .. |pypi-edc-model-form| image:: https://img.shields.io/pypi/v/edc-model-form.svg
@@ -546,16 +491,16 @@
     :target: https://pypi.python.org/pypi/edc-pharmacy
 .. |pypi-edc-pharmacy-dashboard| image:: https://img.shields.io/pypi/v/edc-pharmacy-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-pharmacy-dashboard
 .. |pypi-edc-prn| image:: https://img.shields.io/pypi/v/edc-prn.svg
     :target: https://pypi.python.org/pypi/edc-prn
 .. |pypi-edc-protocol| image:: https://img.shields.io/pypi/v/edc-protocol.svg
     :target: https://pypi.python.org/pypi/edc-protocol
-.. |pypi-edc-protocol-incident| image:: https://img.shields.io/pypi/v/edc-protocol-incident.svg
-    :target: https://pypi.python.org/pypi/edc-protocol-incident
+.. |pypi-edc-protocol-violation| image:: https://img.shields.io/pypi/v/edc-protocol-violation.svg
+    :target: https://pypi.python.org/pypi/edc-protocol-violation
 .. |pypi-edc-randomization| image:: https://img.shields.io/pypi/v/edc-randomization.svg
     :target: https://pypi.python.org/pypi/edc-randomization
 .. |pypi-edc-reference| image:: https://img.shields.io/pypi/v/edc-reference.svg
     :target: https://pypi.python.org/pypi/edc-reference
 .. |pypi-edc-registration| image:: https://img.shields.io/pypi/v/edc-registration.svg
     :target: https://pypi.python.org/pypi/edc-registration
 .. |pypi-edc-reportable| image:: https://img.shields.io/pypi/v/edc-reportable.svg
@@ -588,9 +533,9 @@
     :target: https://pypi.python.org/pypi/edc-visit-schedule
 .. |pypi-edc-visit-tracking| image:: https://img.shields.io/pypi/v/edc-visit-tracking.svg
     :target: https://pypi.python.org/pypi/edc-visit-tracking
 .. |pypi-edc-vitals| image:: https://img.shields.io/pypi/v/edc-vitals.svg
     :target: https://pypi.python.org/pypi/edc-vitals
 .. |jet-brains| image:: https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm_icon.png
     :target: https://jb.gg/OpenSource
-    :width: 25
+    :width: 120
     :alt: JetBrains PyCharm
```

### Comparing `edc-0.4.88/edc.egg-info/SOURCES.txt` & `edc-0.4.9/edc.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 .yamllint
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
+VERSION
 pyproject.toml
 setup.cfg
 bin/nginx/edc-sites.conf
 bin/nginx/edc-uat.conf
 bin/nginx/edc.conf
 bin/scripts/dev_repos.sh
 bin/scripts/list_db_files.sh
@@ -19,28 +20,24 @@
 bin/systemd/celery.service
 bin/systemd/celerybeat-uat.service
 bin/systemd/celerybeat.service
 bin/systemd/gunicorn-uat.service
 bin/systemd/gunicorn-uat.socket
 bin/systemd/gunicorn.service
 bin/systemd/gunicorn.socket
-docs/Makefile
 docs/README.rst
 docs/backup.rst
 docs/celery.rst
 docs/conda.rst
-docs/conf.py
 docs/configure_web_services.rst
 docs/deploy_new_droplet.rst
 docs/dump_users.rst
 docs/exporting_encrypted_data.rst
 docs/forms_reference.md
-docs/index.rst
 docs/landing_page.rst
-docs/make.bat
 docs/multisite_deployment.rst
 docs/prepare_database.rst
 docs/printing.rst
 docs/redis.rst
 docs/update_deployment.rst
 edc.egg-info/PKG-INFO
 edc.egg-info/SOURCES.txt
```

### Comparing `edc-0.4.88/edc.egg-info/requires.txt` & `edc-0.4.9/edc.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,90 +6,84 @@
 mysqlclient
 pycups
 pyrabbit
 python-dateutil
 python-memcached
 reportlab
 tqdm
-fontawesomefree
 django-environ
 django-redis
-django-audit-fields==0.3.9
-django-crypto-fields==0.3.5
+django-audit-fields>=0.3.8
+django-crypto-fields>=0.3.4
 django-defender
 django-extensions
 django-logentry-admin
 django-multisite-edc==2.0.0
-django-revision==0.3.6
+django-revision>=0.3.3
 django-simple-history>=3.1.1
 django-storages
 djangorestframework
-edc-action-item==0.3.51
-edc-adherence==0.1.20
-edc-adverse-event==0.3.47
-edc-appointment==0.3.70
-edc-auth==0.3.59
-edc-consent==0.3.44
-edc-constants==0.3.46
-edc-crf==0.3.41
-edc-dashboard==0.3.43
-edc-data-manager==0.3.52
-edc-device==0.3.10
-edc-document-status==0.1.3
-edc-dx==0.1.16
-edc-dx-review==0.1.37
-edc-egfr==0.1.10
-edc-export==0.3.25
-edc-facility==0.3.14
-edc-fieldsets==0.3.12
-edc-form-describer==0.3.12
-edc-form-label==0.3.8
-edc-form-validators==0.3.32
-edc-glucose==0.1.27
-edc-he==0.1.5
-edc-identifier==0.3.22
-edc-lab==0.3.42
-edc-lab-dashboard==0.3.10
-edc-lab-panel==0.1.14
-edc-lab-results==0.1.37
+edc-action-item==0.3.32
+edc-adherence==0.1.11
+edc-adverse-event==0.3.30
+edc-appointment==0.3.40
+edc-auth==0.3.44
+edc-consent==0.3.30
+edc-constants==0.3.31
+edc-crf==0.3.26
+edc-dashboard==0.3.23
+edc-data-manager==0.3.32
+edc-device==0.3.8
+edc-document-status==0.1.2
+edc-dx==0.1.9
+edc-dx-review==0.1.16
+edc-egfr==0.1.1
+edc-export==0.3.14
+edc-facility==0.3.11
+edc-fieldsets==0.3.8
+edc-form-describer==0.3.9
+edc-form-label==0.3.4
+edc-form-validators==0.3.20
+edc-glucose==0.1.18
+edc-identifier==0.3.15
+edc-lab==0.3.26
+edc-lab-dashboard==0.3.6
+edc-lab-panel==0.1.12
+edc-lab-results==0.1.28
 edc-label==0.3.11
-edc-list-data==0.3.17
-edc-listboard==0.1.7
-edc-locator==0.3.21
-edc-ltfu==0.3.22
-edc-metadata==0.3.50
-edc-mnsi==0.1.15
-edc-model==0.3.29
-edc-model-admin==0.3.43
-edc-model-fields==0.3.6
-edc-model-form==0.1.10
-edc-model-wrapper==0.3.9
-edc-navbar==0.3.15
-edc-notification==0.3.16
-edc-offstudy==0.3.30
-edc-pdf-reports==0.3.11
-edc-pdutils==0.3.21
-edc-pharmacy==0.1.37
-edc-pharmacy-dashboard==0.1.2
-edc-prn==0.3.13
-edc-protocol==0.3.8
-edc-protocol-incident==0.1.24
-edc-qol==0.1.11
-edc-randomization==0.3.45
-edc-reference==0.3.14
-edc-refusal==0.1.10
-edc-registration==0.3.26
-edc-reportable==0.3.30
-edc-review-dashboard==0.3.18
-edc-rx==0.1.5
-edc-screening==0.3.31
-edc-search==0.3.6
-edc-sites==0.3.19
-edc-subject-dashboard==0.3.32
-edc-subject-model-wrappers==0.3.12
-edc-timepoint==0.3.10
-edc-transfer==0.3.13
-edc-unblinding==0.1.13
-edc-utils==0.3.19
-edc-visit-schedule==0.3.59
-edc-visit-tracking==0.3.50
-edc-vitals==0.1.10
+edc-list-data==0.3.14
+edc-locator==0.3.14
+edc-ltfu==0.3.16
+edc-metadata==0.3.39
+edc-model==0.3.19
+edc-model-admin==0.3.21
+edc-model-fields==0.3.4
+edc-model-form==0.1.2
+edc-model-wrapper==0.3.6
+edc-navbar==0.3.9
+edc-notification==0.3.14
+edc-offstudy==0.3.19
+edc-pdf-reports==0.3.9
+edc-pdutils==0.3.8
+edc-pharmacy==0.1.21
+edc-pharmacy-dashboard==0.1.1a14
+edc-prn==0.3.7
+edc-protocol==0.3.7
+edc-protocol-violation==0.1.11
+edc-randomization==0.3.32
+edc-reference==0.3.10
+edc-refusal==0.1.6
+edc-registration==0.3.19
+edc-reportable==0.3.23
+edc-review-dashboard==0.3.12
+edc-screening==0.3.22
+edc-search==0.3.5
+edc-sites==0.3.6
+edc-subject-dashboard==0.3.21
+edc-subject-model-wrappers==0.3.9
+edc-timepoint==0.3.6
+edc-transfer==0.3.9
+edc-unblinding==0.1.7
+edc-utils==0.3.12
+edc-visit-schedule==0.3.43
+edc-visit-tracking==0.3.37
+edc-vitals==0.1.7
```

### Comparing `edc-0.4.88/image/icon-pycharm.png` & `edc-0.4.9/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.4.88/requirements.tests/edc.txt` & `edc-0.4.9/requirements.tests/edc.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,50 +20,45 @@
 edc-export
 edc-facility
 edc-fieldsets
 edc-form-describer
 edc-form-label
 edc-form-validators
 edc-glucose
-edc-he
 edc-identifier
 edc-lab
 edc-lab-dashboard
 edc-lab-panel
 edc-lab-results
 edc-label
 edc-list-data
-edc-listboard
 edc-locator
 edc-ltfu
 edc-metadata
-edc-mnsi
 edc-model
 edc-model-admin
 edc-model-fields
 edc-model-form
 edc-model-wrapper
 edc-navbar
 edc-notification
 edc-offstudy
 edc-pdf-reports
 edc-pdutils
 edc-pharmacy
 edc-pharmacy-dashboard
 edc-prn
 edc-protocol
-edc-protocol-incident
-edc-qol
+edc-protocol-violation
 edc-randomization
 edc-reference
 edc-refusal
 edc-registration
 edc-reportable
 edc-review-dashboard
-edc-rx
 edc-screening
 edc-search
 edc-sites
 edc-subject-dashboard
 edc-subject-model-wrappers
 edc-timepoint
 edc-transfer
```

### Comparing `edc-0.4.88/requirements.tests/edc_dev.txt` & `edc-0.4.9/requirements.tests/edc_dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 https://github.com/clinicedc/edc-offstudy/tarball/develop
 https://github.com/clinicedc/edc-pdf-reports/tarball/develop
 https://github.com/clinicedc/edc-pdutils/tarball/develop
 https://github.com/clinicedc/edc-pharmacy/tarball/develop
 https://github.com/clinicedc/edc-pharmacy-dashboard/tarball/develop
 https://github.com/clinicedc/edc-prn/tarball/develop
 https://github.com/clinicedc/edc-protocol/tarball/develop
-https://github.com/clinicedc/edc-protocol-incident/tarball/develop
+https://github.com/clinicedc/edc-protocol-violation/tarball/develop
 https://github.com/clinicedc/edc-randomization/tarball/develop
 https://github.com/clinicedc/edc-reference/tarball/develop
 https://github.com/clinicedc/edc-refusal/tarball/develop
 https://github.com/clinicedc/edc-registration/tarball/develop
 https://github.com/clinicedc/edc-reportable/tarball/develop
 https://github.com/clinicedc/edc-review-dashboard/tarball/develop
 https://github.com/clinicedc/edc-screening/tarball/develop
```

### Comparing `edc-0.4.88/setup.cfg` & `edc-0.4.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 description = EDC core modules for clinicedc/edc projects.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django edc clinical trials research
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
+	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.10
+python_requires = >=3.9
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	argon2-cffi
 	boto3
 	celery
@@ -35,97 +37,91 @@
 	mysqlclient
 	pycups
 	pyrabbit
 	python-dateutil
 	python-memcached
 	reportlab
 	tqdm
-	fontawesomefree
 	django-environ
 	django-redis
-	django-audit-fields==0.3.9
-	django-crypto-fields==0.3.5
+	django-audit-fields>=0.3.8
+	django-crypto-fields>=0.3.4
 	django-defender
 	django-extensions
 	django-logentry-admin
 	django-multisite-edc==2.0.0
-	django-revision==0.3.6
+	django-revision>=0.3.3
 	django-simple-history>=3.1.1
 	django-storages
 	djangorestframework
-	edc-action-item==0.3.51
-	edc-adherence==0.1.20
-	edc-adverse-event==0.3.47
-	edc-appointment==0.3.70
-	edc-auth==0.3.59
-	edc-consent==0.3.44
-	edc-constants==0.3.46
-	edc-crf==0.3.41
-	edc-dashboard==0.3.43
-	edc-data-manager==0.3.52
-	edc-device==0.3.10
-	edc-document-status==0.1.3
-	edc-dx==0.1.16
-	edc-dx-review==0.1.37
-	edc-egfr==0.1.10
-	edc-export==0.3.25
-	edc-facility==0.3.14
-	edc-fieldsets==0.3.12
-	edc-form-describer==0.3.12
-	edc-form-label==0.3.8
-	edc-form-validators==0.3.32
-	edc-glucose==0.1.27
-	edc-he==0.1.5
-	edc-identifier==0.3.22
-	edc-lab==0.3.42
-	edc-lab-dashboard==0.3.10
-	edc-lab-panel==0.1.14
-	edc-lab-results==0.1.37
+	edc-action-item==0.3.32
+	edc-adherence==0.1.11
+	edc-adverse-event==0.3.30
+	edc-appointment==0.3.40
+	edc-auth==0.3.44
+	edc-consent==0.3.30
+	edc-constants==0.3.31
+	edc-crf==0.3.26
+	edc-dashboard==0.3.23
+	edc-data-manager==0.3.32
+	edc-device==0.3.8
+	edc-document-status==0.1.2
+	edc-dx==0.1.9
+	edc-dx-review==0.1.16
+	edc-egfr==0.1.1
+	edc-export==0.3.14
+	edc-facility==0.3.11
+	edc-fieldsets==0.3.8
+	edc-form-describer==0.3.9
+	edc-form-label==0.3.4
+	edc-form-validators==0.3.20
+	edc-glucose==0.1.18
+	edc-identifier==0.3.15
+	edc-lab==0.3.26
+	edc-lab-dashboard==0.3.6
+	edc-lab-panel==0.1.12
+	edc-lab-results==0.1.28
 	edc-label==0.3.11
-	edc-list-data==0.3.17
-	edc-listboard==0.1.7
-	edc-locator==0.3.21
-	edc-ltfu==0.3.22
-	edc-metadata==0.3.50
-	edc-mnsi==0.1.15
-	edc-model==0.3.29
-	edc-model-admin==0.3.43
-	edc-model-fields==0.3.6
-	edc-model-form==0.1.10
-	edc-model-wrapper==0.3.9
-	edc-navbar==0.3.15
-	edc-notification==0.3.16
-	edc-offstudy==0.3.30
-	edc-pdf-reports==0.3.11
-	edc-pdutils==0.3.21
-	edc-pharmacy==0.1.37
-	edc-pharmacy-dashboard==0.1.2
-	edc-prn==0.3.13
-	edc-protocol==0.3.8
-	edc-protocol-incident==0.1.24
-	edc-qol==0.1.11
-	edc-randomization==0.3.45
-	edc-reference==0.3.14
-	edc-refusal==0.1.10
-	edc-registration==0.3.26
-	edc-reportable==0.3.30
-	edc-review-dashboard==0.3.18
-	edc-rx==0.1.5
-	edc-screening==0.3.31
-	edc-search==0.3.6
-	edc-sites==0.3.19
-	edc-subject-dashboard==0.3.32
-	edc-subject-model-wrappers==0.3.12
-	edc-timepoint==0.3.10
-	edc-transfer==0.3.13
-	edc-unblinding==0.1.13
-	edc-utils==0.3.19
-	edc-visit-schedule==0.3.59
-	edc-visit-tracking==0.3.50
-	edc-vitals==0.1.10
+	edc-list-data==0.3.14
+	edc-locator==0.3.14
+	edc-ltfu==0.3.16
+	edc-metadata==0.3.39
+	edc-model==0.3.19
+	edc-model-admin==0.3.21
+	edc-model-fields==0.3.4
+	edc-model-form==0.1.2
+	edc-model-wrapper==0.3.6
+	edc-navbar==0.3.9
+	edc-notification==0.3.14
+	edc-offstudy==0.3.19
+	edc-pdf-reports==0.3.9
+	edc-pdutils==0.3.8
+	edc-pharmacy==0.1.21
+	edc-pharmacy-dashboard==0.1.1a14
+	edc-prn==0.3.7
+	edc-protocol==0.3.7
+	edc-protocol-violation==0.1.11
+	edc-randomization==0.3.32
+	edc-reference==0.3.10
+	edc-refusal==0.1.6
+	edc-registration==0.3.19
+	edc-reportable==0.3.23
+	edc-review-dashboard==0.3.12
+	edc-screening==0.3.22
+	edc-search==0.3.5
+	edc-sites==0.3.6
+	edc-subject-dashboard==0.3.21
+	edc-subject-model-wrappers==0.3.9
+	edc-timepoint==0.3.6
+	edc-transfer==0.3.9
+	edc-unblinding==0.1.7
+	edc-utils==0.3.12
+	edc-visit-schedule==0.3.43
+	edc-visit-tracking==0.3.37
+	edc-vitals==0.1.7
 
 [options.packages.find]
 exclude = 
 	examples*
 	tools*
 	docs*
 	bin*
```

### Comparing `edc-0.4.88/utils/get_edc_requirements.py` & `edc-0.4.9/utils/get_edc_requirements.py`

 * *Files identical despite different names*

