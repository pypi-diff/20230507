# Comparing `tmp/intecomm-edc-0.1.8.tar.gz` & `tmp/intecomm-edc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intecomm-edc-0.1.8.tar", last modified: Fri Jan 27 03:45:22 2023, max compression
+gzip compressed data, was "intecomm-edc-0.1.9.tar", last modified: Mon Jan 30 02:26:37 2023, max compression
```

## Comparing `intecomm-edc-0.1.8.tar` & `intecomm-edc-0.1.9.tar`

### file list

```diff
@@ -1,735 +1,735 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.961958 intecomm-edc-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      129 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-13 15:16:15.000000 intecomm-edc-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.815436 intecomm-edc-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.829145 intecomm-edc-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2100 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1466 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1109 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      309 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2022-12-01 02:13:19.000000 intecomm-edc-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-11-22 15:26:51.000000 intecomm-edc-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1902 2023-01-27 03:45:22.962078 intecomm-edc-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1029 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-03-14 02:38:46.000000 intecomm-edc-0.1.8/VERSION
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.816234 intecomm-edc-0.1.8/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.829336 intecomm-edc-0.1.8/bin/nginx/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.830213 intecomm-edc-0.1.8/bin/nginx/conf/
--rw-r--r--   0 erikvw     (501) staff       (20)     1202 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/nginx/conf/intecomm_live.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      432 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/nginx/conf/intecomm_live_sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/nginx/conf/intecomm_uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      435 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/nginx/conf/intecomm_uat_sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/nginx/intecomm.clinicedc.org.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.815757 intecomm-edc-0.1.8/bin/nginx/www/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.816030 intecomm-edc-0.1.8/bin/nginx/www/html/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.830366 intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/
--rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.830615 intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     2297 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.830824 intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/
--rw-r--r--   0 erikvw     (501) staff       (20)     2281 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.831098 intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/
--rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.831306 intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     2334 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.831469 intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/
--rw-r--r--   0 erikvw     (501) staff       (20)     2318 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.832107 intecomm-edc-0.1.8/bin/systemd/
--rwxr-xr-x   0 erikvw     (501) staff       (20)      435 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/systemd/gunicorn-live.service
--rwxr-xr-x   0 erikvw     (501) staff       (20)      133 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/systemd/gunicorn-live.socket
--rwxr-xr-x   0 erikvw     (501) staff       (20)      433 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/systemd/gunicorn-uat.service
--rwxr-xr-x   0 erikvw     (501) staff       (20)      131 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/codecov.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     4590 2021-11-22 15:06:41.000000 intecomm-edc-0.1.8/env.sample
--rw-r--r--   0 erikvw     (501) staff       (20)     1048 2021-08-13 15:16:15.000000 intecomm-edc-0.1.8/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.833703 intecomm-edc-0.1.8/intecomm_ae/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7311 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.835297 intecomm-edc-0.1.8/intecomm_ae/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      460 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      424 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/admin/ae_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      774 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/admin/ae_initial_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      403 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/admin/ae_susar_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      389 2022-11-30 17:58:11.000000 intecomm-edc-0.1.8/intecomm_ae/admin/ae_tmg_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2191 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/admin/death_report_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      452 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/admin/death_report_tmg_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      482 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/admin/death_report_tmg_second_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4157 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-10-18 02:23:36.000000 intecomm-edc-0.1.8/intecomm_ae/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      292 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1154 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-04-11 18:27:09.000000 intecomm-edc-0.1.8/intecomm_ae/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       36 2022-04-11 18:27:09.000000 intecomm-edc-0.1.8/intecomm_ae/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.836842 intecomm-edc-0.1.8/intecomm_ae/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      330 2022-10-18 02:20:14.000000 intecomm-edc-0.1.8/intecomm_ae/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/forms/ae_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      292 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/forms/ae_initial_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      280 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/forms/ae_susar_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      268 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/forms/ae_tmg_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1425 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/forms/death_report_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      322 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/forms/death_report_tmg_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      340 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/forms/death_report_tmg_second_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      874 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/forms/modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1248 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.838222 intecomm-edc-0.1.8/intecomm_ae/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   144621 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_ae/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5272 2022-12-01 02:13:19.000000 intecomm-edc-0.1.8/intecomm_ae/migrations/0002_rename_narrative_aetmg_investigator_narrative_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1664 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_ae/migrations/0003_alter_deathreporttmg_cause_of_death_agreed_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.838690 intecomm-edc-0.1.8/intecomm_ae/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2020-05-15 02:40:42.000000 intecomm-edc-0.1.8/intecomm_ae/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2638 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/model_mixins/ae_review_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1799 2022-06-29 19:36:30.000000 intecomm-edc-0.1.8/intecomm_ae/model_mixins/death_report_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.840335 intecomm-edc-0.1.8/intecomm_ae/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      267 2022-10-18 02:17:22.000000 intecomm-edc-0.1.8/intecomm_ae/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/models/ae_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      343 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/models/ae_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      208 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/models/ae_susar.py
--rw-r--r--   0 erikvw     (501) staff       (20)      226 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/models/ae_tmg.py
--rw-r--r--   0 erikvw     (501) staff       (20)      442 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/models/death_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2021-07-05 19:24:26.000000 intecomm-edc-0.1.8/intecomm_ae/models/death_report_tmg.py
--rw-r--r--   0 erikvw     (501) staff       (20)      565 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/models/death_report_tmg_second.py
--rw-r--r--   0 erikvw     (501) staff       (20)      621 2022-06-29 19:36:30.000000 intecomm-edc-0.1.8/intecomm_ae/models/managers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.841037 intecomm-edc-0.1.8/intecomm_ae/pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)       70 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/pdf_reports/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/pdf_reports/ae_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      199 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/pdf_reports/death_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)       77 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/pdf_reports/pdf_report_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.816825 intecomm-edc-0.1.8/intecomm_ae/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.816879 intecomm-edc-0.1.8/intecomm_ae/templates/intecomm_ae/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.841193 intecomm-edc-0.1.8/intecomm_ae/templates/intecomm_ae/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      889 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/templates/intecomm_ae/bootstrap3/ae_initial_description.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.841520 intecomm-edc-0.1.8/intecomm_ae/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1154 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/templatetags/protocol_ae_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.841947 intecomm-edc-0.1.8/intecomm_ae/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_ae/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.842170 intecomm-edc-0.1.8/intecomm_ae/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.1.8/intecomm_ae/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      259 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_ae/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-10-18 02:24:15.000000 intecomm-edc-0.1.8/intecomm_ae/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.843032 intecomm-edc-0.1.8/intecomm_auth/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_auth/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      233 2022-03-12 18:30:44.000000 intecomm-edc-0.1.8/intecomm_auth/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      682 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_auth/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1733 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_auth/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_auth/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.852589 intecomm-edc-0.1.8/intecomm_consent/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_consent/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      764 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.854861 intecomm-edc-0.1.8/intecomm_consent/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_consent/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3162 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/intecomm_consent/admin/subject_consent_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2751 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/admin/subject_reconsent_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:54:16.000000 intecomm-edc-0.1.8/intecomm_consent/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-03-12 18:10:23.000000 intecomm-edc-0.1.8/intecomm_consent/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1257 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/consents.py
--rw-r--r--   0 erikvw     (501) staff       (20)       31 2021-10-27 22:32:32.000000 intecomm-edc-0.1.8/intecomm_consent/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.860550 intecomm-edc-0.1.8/intecomm_consent/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      139 2022-03-03 20:12:26.000000 intecomm-edc-0.1.8/intecomm_consent/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1498 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/intecomm_consent/forms/subject_consent_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_consent/forms/subject_reconsent_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.860759 intecomm-edc-0.1.8/intecomm_consent/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-03 20:12:26.000000 intecomm-edc-0.1.8/intecomm_consent/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.861214 intecomm-edc-0.1.8/intecomm_consent/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-03 20:12:26.000000 intecomm-edc-0.1.8/intecomm_consent/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/management/commands/create_missing_prescriptions.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.869249 intecomm-edc-0.1.8/intecomm_consent/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    69090 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_consent/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5397 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_consent/migrations/0002_remove_subjectconsent_intecomm_co_subject_145905_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1536 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/intecomm_consent/migrations/0003_alter_historicalsubjectconsent_language_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1952 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/intecomm_consent/migrations/0004_alter_historicalsubjectconsent_familiar_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1017 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_consent/migrations/0005_remove_subjectconsent_unique_consent_subject_id_and_version_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      697 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_consent/migrations/0006_historicalsubjectconsent_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_consent/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.870092 intecomm-edc-0.1.8/intecomm_consent/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      174 2021-08-09 19:25:29.000000 intecomm-edc-0.1.8/intecomm_consent/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_consent/models/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4389 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_consent/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5391 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_consent/models/subject_consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3631 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/models/subject_reconsent.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.817915 intecomm-edc-0.1.8/intecomm_consent/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.817981 intecomm-edc-0.1.8/intecomm_consent/templates/intecomm_consent/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.870337 intecomm-edc-0.1.8/intecomm_consent/templates/intecomm_consent/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     1420 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_consent/templates/intecomm_consent/admin/subjectconsent_change_list.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.870821 intecomm-edc-0.1.8/intecomm_consent/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_consent/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_consent/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.871319 intecomm-edc-0.1.8/intecomm_consent/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.1.8/intecomm_consent/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3459 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/tests/tests/test_form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/tests/tests/test_subject_consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)      924 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_consent/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.872626 intecomm-edc-0.1.8/intecomm_dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1948 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.872856 intecomm-edc-0.1.8/intecomm_dashboard/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.874167 intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/
--rw-r--r--   0 erikvw     (501) staff       (20)      401 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/ae_initial_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      379 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/death_report_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      492 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/patient_log_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      432 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/subject_consent_model_wrappers.py
--rw-r--r--   0 erikvw     (501) staff       (20)      411 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/subject_refusal_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1781 2023-01-23 13:57:43.000000 intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/subject_screening_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1853 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-06-24 09:14:59.000000 intecomm-edc-0.1.8/intecomm_dashboard/patterns.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.818587 intecomm-edc-0.1.8/intecomm_dashboard/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.818679 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.818937 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.875769 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/
--rw-r--r--   0 erikvw     (501) staff       (20)      466 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/add_consent_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      239 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/dashboard_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      401 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/eligibility_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/patient_group_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      365 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/patient_log_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      437 2022-10-20 00:50:06.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/refusal_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      341 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/screening_button.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.876061 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)     2986 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.876762 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)     2061 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/comm_listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.877006 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)      230 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard/top_bar.html
--rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-10-18 02:52:50.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1382 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/inte_listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.877338 intecomm-edc-0.1.8/intecomm_dashboard/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6019 2022-11-28 02:44:46.000000 intecomm-edc-0.1.8/intecomm_dashboard/templatetags/protocol_dashboard_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.878131 intecomm-edc-0.1.8/intecomm_dashboard/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      720 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/tests/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.878296 intecomm-edc-0.1.8/intecomm_dashboard/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2937 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_dashboard/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1517 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.878421 intecomm-edc-0.1.8/intecomm_dashboard/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.879115 intecomm-edc-0.1.8/intecomm_dashboard/views/ae/
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/ae/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      458 2022-10-18 02:53:29.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/ae/ae_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      496 2022-10-18 02:53:29.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/ae/death_report_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.879586 intecomm-edc-0.1.8/intecomm_dashboard/views/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2253 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/screening/listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.879764 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)      149 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.880197 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      477 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/dashboard/dashboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.880998 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/listboard/
--rw-r--r--   0 erikvw     (501) staff       (20)      176 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/listboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1202 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/listboard/comm_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      808 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/listboard/inte_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      786 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_dashboard/views/subject/listboard/subject_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.883008 intecomm-edc-0.1.8/intecomm_edc/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      927 2022-07-07 11:06:18.000000 intecomm-edc-0.1.8/intecomm_edc/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      382 2022-03-12 18:45:28.000000 intecomm-edc-0.1.8/intecomm_edc/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      793 2022-03-12 18:45:28.000000 intecomm-edc-0.1.8/intecomm_edc/celery.py
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-04 23:21:43.000000 intecomm-edc-0.1.8/intecomm_edc/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1309 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_edc/navbars.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.885116 intecomm-edc-0.1.8/intecomm_edc/settings/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-03 04:33:09.000000 intecomm-edc-0.1.8/intecomm_edc/settings/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      430 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_edc/settings/debug.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17573 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_edc/settings/defaults.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1065 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/settings/live.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1936 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/settings/logging.py
--rw-r--r--   0 erikvw     (501) staff       (20)      595 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/settings/minimal.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1302 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/settings/uat.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.820197 intecomm-edc-0.1.8/intecomm_edc/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.820253 intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.886063 intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2021-08-09 19:25:29.000000 intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/base.html
--rw-r--r--   0 erikvw     (501) staff       (20)     3191 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_comm.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2172 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_inte.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2759 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/grouping.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2543 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.886249 intecomm-edc-0.1.8/intecomm_edc/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 intecomm-edc-0.1.8/intecomm_edc/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.886488 intecomm-edc-0.1.8/intecomm_edc/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.1.8/intecomm_edc/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/tests/tests/test_endpoints.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3419 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_edc/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.887415 intecomm-edc-0.1.8/intecomm_edc/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      170 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      622 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/views/followup_comm_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      649 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_edc/views/followup_inte_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      518 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/views/grouping_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      502 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_edc/views/home_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      179 2022-03-12 18:45:28.000000 intecomm-edc-0.1.8/intecomm_edc/wsgi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-03-12 18:45:28.000000 intecomm-edc-0.1.8/intecomm_edc/wsgi_live.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:45:28.000000 intecomm-edc-0.1.8/intecomm_edc/wsgi_uat.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.883962 intecomm-edc-0.1.8/intecomm_edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1902 2023-01-27 03:45:22.000000 intecomm-edc-0.1.8/intecomm_edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    28083 2023-01-27 03:45:22.000000 intecomm-edc-0.1.8/intecomm_edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-01-27 03:45:22.000000 intecomm-edc-0.1.8/intecomm_edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-19 12:31:42.000000 intecomm-edc-0.1.8/intecomm_edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)      158 2023-01-27 03:45:22.000000 intecomm-edc-0.1.8/intecomm_edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      223 2023-01-27 03:45:22.000000 intecomm-edc-0.1.8/intecomm_edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.888578 intecomm-edc-0.1.8/intecomm_export/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_export/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_export/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-03-12 18:43:23.000000 intecomm-edc-0.1.8/intecomm_export/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-03-12 18:43:17.000000 intecomm-edc-0.1.8/intecomm_export/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_export/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-03-12 18:43:14.000000 intecomm-edc-0.1.8/intecomm_export/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_export/views.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.890216 intecomm-edc-0.1.8/intecomm_group/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.891822 intecomm-edc-0.1.8/intecomm_group/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_group/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/admin/autocomplete_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2709 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/admin/community_care_location_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      304 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3546 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/admin/patient_followup_call_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3808 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_group/admin/patient_group_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1914 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/admin/patient_group_appointment_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2032 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/admin/patient_group_meeting_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9250 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_group/admin/patient_log_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      292 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      800 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      100 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/exceptions.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.892698 intecomm-edc-0.1.8/intecomm_group/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/forms/community_care_location_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      372 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/forms/patient_group_appointment_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      497 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_group/forms/patient_group_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/forms/patient_group_meeting_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.894947 intecomm-edc-0.1.8/intecomm_group/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    29539 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3394 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0002_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      599 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0003_alter_historicalpatientgroup_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      666 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0004_alter_patientgroup_patients.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17785 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0005_patientfollowupcall_historicalpatientfollowupcall.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2953 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0006_remove_historicalpatientgroup_enforce_group_size_min_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3531 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0007_remove_historicalpatientfollowupcall_attend_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2555 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0008_patientgroup_dm_patients_patientgroup_hiv_patients_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1518 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0009_auto_20221126_0358.py
--rw-r--r--   0 erikvw     (501) staff       (20)      576 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_group/migrations/0010_alter_patientgroup_managers.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.896596 intecomm-edc-0.1.8/intecomm_group/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      536 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_group/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2278 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/models/community_care_location.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1214 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/models/patient_followup_call.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4070 2023-01-22 23:16:39.000000 intecomm-edc-0.1.8/intecomm_group/models/patient_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)      997 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/models/patient_group_appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1192 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/models/patient_group_meeting.py
--rw-r--r--   0 erikvw     (501) staff       (20)      150 2023-01-23 13:41:17.000000 intecomm-edc-0.1.8/intecomm_group/models/proxy_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2745 2022-12-06 23:12:40.000000 intecomm-edc-0.1.8/intecomm_group/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1946 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/models/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.821151 intecomm-edc-0.1.8/intecomm_group/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.821198 intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.897568 intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     1315 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/communitycarelocation_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1522 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/patientfollowupcall_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1354 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/patientgroup_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1475 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/patientgroupappointment_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1457 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/patientgroupmeeting_change_list.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.897848 intecomm-edc-0.1.8/intecomm_group/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.898006 intecomm-edc-0.1.8/intecomm_group/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_group/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1522 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_group/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.899722 intecomm-edc-0.1.8/intecomm_labs/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-02 03:53:00.000000 intecomm-edc-0.1.8/intecomm_labs/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       87 2021-07-05 19:24:26.000000 intecomm-edc-0.1.8/intecomm_labs/aliquot_types.py
--rw-r--r--   0 erikvw     (501) staff       (20)      209 2022-03-12 18:19:55.000000 intecomm-edc-0.1.8/intecomm_labs/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1011 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_labs/lab_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)      128 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_labs/labs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      481 2022-03-12 18:19:03.000000 intecomm-edc-0.1.8/intecomm_labs/list_data.py
--rw-r--r--   0 erikvw     (501) staff       (20)      500 2021-09-17 02:16:20.000000 intecomm-edc-0.1.8/intecomm_labs/processing_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)      516 2022-03-12 18:18:51.000000 intecomm-edc-0.1.8/intecomm_labs/reportables.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.900072 intecomm-edc-0.1.8/intecomm_labs/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_labs/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.900623 intecomm-edc-0.1.8/intecomm_labs/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_labs/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_labs/tests/tests/test_labs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      539 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_labs/tests/tests/test_reportables.py
--rw-r--r--   0 erikvw     (501) staff       (20)      116 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_labs/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.902486 intecomm-edc-0.1.8/intecomm_lists/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_lists/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      630 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_lists/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-03-14 02:24:52.000000 intecomm-edc-0.1.8/intecomm_lists/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-03-12 18:10:47.000000 intecomm-edc-0.1.8/intecomm_lists/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_lists/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_lists/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3529 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_lists/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.903630 intecomm-edc-0.1.8/intecomm_lists/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    77606 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_lists/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      466 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_lists/migrations/0002_delete_reasonsfortesting_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2718 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_lists/migrations/0003_dmmanagement_dmmanagement_intecomm_li_id_b4d41f_idx.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_lists/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4770 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_lists/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.903731 intecomm-edc-0.1.8/intecomm_lists/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_lists/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.903926 intecomm-edc-0.1.8/intecomm_lists/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_lists/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      212 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_lists/tests/tests/test_lists.py
--rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-03-12 18:05:17.000000 intecomm-edc-0.1.8/intecomm_lists/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.905555 intecomm-edc-0.1.8/intecomm_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_prn/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3105 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.907463 intecomm-edc-0.1.8/intecomm_prn/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      444 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4603 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_prn/admin/end_of_study_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1634 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_prn/admin/loss_to_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      354 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/admin/offschedule_comm_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1769 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/admin/offschedule_inte_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      286 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/admin/onschedule_comm_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1494 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/admin/onschedule_inte_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      781 2022-12-01 02:13:19.000000 intecomm-edc-0.1.8/intecomm_prn/admin/protocol_incident_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      659 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_prn/admin/subject_transfer_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-10-18 02:27:53.000000 intecomm-edc-0.1.8/intecomm_prn/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      288 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_prn/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3151 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_prn/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      104 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.908670 intecomm-edc-0.1.8/intecomm_prn/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      322 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      938 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_prn/forms/end_of_study_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1405 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_prn/forms/loss_to_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      960 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/forms/offschedule_comm_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      960 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/forms/offschedule_inte_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_prn/forms/protocol_incident_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      818 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_prn/forms/subject_transfer_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2336 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_prn/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.910388 intecomm-edc-0.1.8/intecomm_prn/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   149191 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_prn/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3534 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_prn/migrations/0002_remove_endofstudy_delivery_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1914 2022-12-01 02:13:19.000000 intecomm-edc-0.1.8/intecomm_prn/migrations/0003_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3193 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/migrations/0004_rename_historicaloffschedulebaseline_historicaloffschedulecomm_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3238 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/migrations/0005_rename_historicaloffschedulefollowup_historicaloffscheduleinte_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_prn/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.912274 intecomm-edc-0.1.8/intecomm_prn/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      356 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3359 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_prn/models/end_of_study.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2149 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_prn/models/loss_to_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      645 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/models/offschedule_comm.py
--rw-r--r--   0 erikvw     (501) staff       (20)      643 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/models/offschedule_inte.py
--rw-r--r--   0 erikvw     (501) staff       (20)      500 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/models/onschedule_comm.py
--rw-r--r--   0 erikvw     (501) staff       (20)      498 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_prn/models/onschedule_inte.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1088 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_prn/models/protocol_incident.py
--rw-r--r--   0 erikvw     (501) staff       (20)      266 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_prn/models/subject_transfer.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.912687 intecomm-edc-0.1.8/intecomm_prn/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_prn/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.912838 intecomm-edc-0.1.8/intecomm_prn/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_prn/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_prn/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-10-18 02:47:10.000000 intecomm-edc-0.1.8/intecomm_prn/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.915773 intecomm-edc-0.1.8/intecomm_screening/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_screening/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.918332 intecomm-edc-0.1.8/intecomm_screening/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      533 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2249 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/admin/health_facility_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2305 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/admin/health_talk_log_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5080 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4467 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/admin/patient_call_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2133 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/admin/patient_call_inlines.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8184 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/admin/patient_group_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13401 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/admin/patient_log_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      258 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/admin/site_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2178 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/admin/subject_refusal_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9586 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/intecomm_screening/admin/subject_screening_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2022-03-12 17:44:29.000000 intecomm-edc-0.1.8/intecomm_screening/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      553 2022-03-12 17:44:16.000000 intecomm-edc-0.1.8/intecomm_screening/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      549 2022-10-18 20:05:10.000000 intecomm-edc-0.1.8/intecomm_screening/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      402 2022-03-03 20:12:26.000000 intecomm-edc-0.1.8/intecomm_screening/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1065 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      597 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       33 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.919888 intecomm-edc-0.1.8/intecomm_screening/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      356 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      372 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/forms/health_facility_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      367 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/forms/health_talk_log_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      357 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/forms/patient_call_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      362 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/forms/patient_group_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      532 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/forms/patient_log_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1675 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/forms/subject_refusal_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1163 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/forms/subject_screening_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.923485 intecomm-edc-0.1.8/intecomm_screening/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   128990 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0002_remove_healthtalklog_unique_lower_name_report_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2758 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0003_site_remove_historicalpatientlog_patient_group_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1451 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0004_rename_name_historicalpatientlog_legal_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2034 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0005_historicalpatientcall_alt_contact_number_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3723 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0006_remove_historicalpatientcall_willing_to_attend_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2229 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0007_historicalpatientlog_last_4_contact_number_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7010 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0008_rename_last_routine_appt_date_historicalpatientlog_last_appt_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3259 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0009_historicalsubjectscreening_familiar_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      717 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0010_historicalpatientlog_age_in_years_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3940 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0011_rename_hf_identifier_historicalpatientlog_hospital_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1147 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0012_alter_historicalpatientcall_last_attend_clinic_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1893 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0013_alter_healthfacility_distance_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3542 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0014_alter_historicalpatientlog_familiar_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      561 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0015_remove_healthtalklog_unique_health_facility_report_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/0016_historicalpatientlog_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_screening/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.923783 intecomm-edc-0.1.8/intecomm_screening/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       60 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2649 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/model_mixins/patient_call_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.925443 intecomm-edc-0.1.8/intecomm_screening/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      461 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2259 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/models/health_facility.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1975 2022-12-01 03:07:11.000000 intecomm-edc-0.1.8/intecomm_screening/models/health_talk_log.py
--rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/models/location.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1186 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/models/patient_call.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6458 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/models/patient_log.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.926024 intecomm-edc-0.1.8/intecomm_screening/models/proxy_models/
--rw-r--r--   0 erikvw     (501) staff       (20)       63 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/models/proxy_models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      265 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/models/proxy_models/patient_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)      185 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/models/proxy_models/site.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2086 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2216 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/models/subject_refusal.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7895 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/models/subject_screening.py
--rw-r--r--   0 erikvw     (501) staff       (20)      135 2022-03-12 17:42:16.000000 intecomm-edc-0.1.8/intecomm_screening/offline_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.823003 intecomm-edc-0.1.8/intecomm_screening/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.927579 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.928614 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/healthfacility_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1270 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/healthtalklog_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1270 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/patientcall_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1270 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/patientgroup_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1270 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/patientlog_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)      719 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/subjectscreening_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)      240 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/change_list_appts.html
--rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/change_list_contacts.html
--rw-r--r--   0 erikvw     (501) staff       (20)       94 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/change_list_dx.html
--rw-r--r--   0 erikvw     (501) staff       (20)      176 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/change_list_group.html
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/change_list_hospital_identifier.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1424 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/change_list_screen_and_consent.html
--rw-r--r--   0 erikvw     (501) staff       (20)      462 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/change_list_talks.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1344 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/group_management.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.929140 intecomm-edc-0.1.8/intecomm_screening/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_screening/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_screening/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     6834 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/tests/intecomm_test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.929524 intecomm-edc-0.1.8/intecomm_screening/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 intecomm-edc-0.1.8/intecomm_screening/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2918 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/intecomm_screening/tests/tests/test_screening.py
--rw-r--r--   0 erikvw     (501) staff       (20)      579 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1701 2022-11-23 01:31:30.000000 intecomm-edc-0.1.8/intecomm_screening/utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1569 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_screening/views.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.930598 intecomm-edc-0.1.8/intecomm_sites/
--rw-r--r--   0 erikvw     (501) staff       (20)       43 2021-07-05 19:24:26.000000 intecomm-edc-0.1.8/intecomm_sites/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      943 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_sites/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      857 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_sites/intecomm_site.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.930819 intecomm-edc-0.1.8/intecomm_sites/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-12 18:03:07.000000 intecomm-edc-0.1.8/intecomm_sites/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_sites/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5871 2022-11-30 03:04:06.000000 intecomm-edc-0.1.8/intecomm_sites/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.931043 intecomm-edc-0.1.8/intecomm_sites/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_sites/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      346 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_sites/tests/site_test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.932648 intecomm-edc-0.1.8/intecomm_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-22 15:10:26.000000 intecomm-edc-0.1.8/intecomm_subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      512 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.938435 intecomm-edc-0.1.8/intecomm_subject/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     2046 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/arv_regimens_admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.939527 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      414 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      723 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_fbc_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      991 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_glu_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      785 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_hba1c_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      746 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_ins_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      746 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_lft_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      760 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_lipid_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4599 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_rft_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      584 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/cd4_result_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2139 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/clinical_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1708 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/clinical_review_baseline_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1556 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/complications_baseline_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1562 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/complications_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      755 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/concomitant_medication_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1547 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/admin/dm_initial_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      442 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/dm_medication_adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/dm_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      696 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/drug_refill_dm_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      771 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/drug_refill_hiv_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      707 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/drug_refill_htn_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1816 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/family_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      349 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1068 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/glucose_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      679 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/hba1c_result_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5682 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/admin/health_economics_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1862 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/hiv_initial_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/hiv_medication_adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/hiv_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      947 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/htn_initial_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/htn_medication_adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1031 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/htn_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      423 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/malaria_test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      816 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/medications_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1884 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2861 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/admin/other_baseline_data_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5264 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/admin/social_harms_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1738 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/subject_requisition_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1330 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/subject_visit_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1233 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/admin/subject_visit_missed_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1075 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/urine_dipstick_test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      968 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/urine_pregnancy_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      626 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/admin/viral_load_result_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2230 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/admin/vitals_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:18:07.000000 intecomm-edc-0.1.8/intecomm_subject/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-03-12 18:18:07.000000 intecomm-edc-0.1.8/intecomm_subject/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5928 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      435 2023-01-27 01:28:16.000000 intecomm-edc-0.1.8/intecomm_subject/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.943124 intecomm-edc-0.1.8/intecomm_subject/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)     1399 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/forms/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.944204 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      400 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      715 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_fbc_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      824 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_glu_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_hba1c_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      723 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_ins_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      715 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_lft_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      731 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_lipid_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1363 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_rft_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      646 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/cd4_result_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      685 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/clinical_review_baseline.py
--rw-r--r--   0 erikvw     (501) staff       (20)      921 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/forms/clinical_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      490 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/concomitant_medication_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      335 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/dm_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      355 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/drug_refill_dm_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/drug_refill_hiv_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/drug_refill_htn_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/drug_supply_dm_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      781 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/drug_supply_hiv_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      393 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/drug_supply_htn_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      371 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/forms/health_economics_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      340 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/hiv_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      340 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/htn_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/malaria_test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      268 2022-12-05 14:48:19.000000 intecomm-edc-0.1.8/intecomm_subject/forms/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/forms/social_harms_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      954 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/forms/subject_requisition_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      757 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/forms/subject_visit_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2277 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/forms/subject_visit_missed_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      829 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/urine_dipstick_test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/urine_pregnancy_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      682 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/forms/viral_load_result_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      343 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/forms/vitals_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.944609 intecomm-edc-0.1.8/intecomm_subject/metadata_rules/
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/metadata_rules/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4127 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/metadata_rules/metadata_rules.py
--rw-r--r--   0 erikvw     (501) staff       (20)      815 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/metadata_rules/predicates.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.948484 intecomm-edc-0.1.8/intecomm_subject/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)  1030443 2022-12-02 22:40:22.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    58038 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0002_remove_historicaldminitialreview_managed_by_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1792 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0003_alter_historicalsocialharms_coworkers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    24956 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0004_historicalsocialharms_employment_impact_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    82106 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0005_alter_historicalsocialharms_coworkers_impact_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1090 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0006_alter_healtheconomics_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1498 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0007_alter_historicalotherbaselinedata_alcohol_consumption_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    23862 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0008_historicalvitals_vitals_remove_indicators_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3555 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0009_remove_historicalvitals_bp_measured_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3178 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0010_remove_historicalvitals_weight_is_estmated_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1501 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0011_remove_clinicalreviewbaseline_complications_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/0012_alter_historicalvitals_heart_rate_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-12 18:03:07.000000 intecomm-edc-0.1.8/intecomm_subject/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.949682 intecomm-edc-0.1.8/intecomm_subject/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4828 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/model_mixins/clinical_review_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      248 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/model_mixins/crf_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/model_mixins/crf_with_action_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      560 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/model_mixins/followup_review_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/model_mixins/search_slug_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.956757 intecomm-edc-0.1.8/intecomm_subject/models/
--rw-r--r--   0 erikvw     (501) staff       (20)     1889 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/arv_regimens.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.958243 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      337 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1252 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_fbc.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1008 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_glu.py
--rw-r--r--   0 erikvw     (501) staff       (20)      958 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_hba1c.py
--rw-r--r--   0 erikvw     (501) staff       (20)      974 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_ins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1157 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_lft.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1090 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_lipid.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1568 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_rft.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1090 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/cd4_result.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4222 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/clinical_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/models/clinical_review_baseline.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4354 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/complications_baseline.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2831 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/complications_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      369 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/concomitant_medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1968 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/models/dm_initial_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      473 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/dm_medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)      404 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/dm_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/drug_refill_dm.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1429 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/drug_refill_hiv.py
--rw-r--r--   0 erikvw     (501) staff       (20)      591 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/drug_refill_htn.py
--rw-r--r--   0 erikvw     (501) staff       (20)      559 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/drug_supply_dm.py
--rw-r--r--   0 erikvw     (501) staff       (20)      617 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/drug_supply_hiv.py
--rw-r--r--   0 erikvw     (501) staff       (20)      573 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/drug_supply_htn.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3521 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/family_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)      335 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/glucose.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/hba1c_result.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18724 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/models/health_economics.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4525 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/hiv_initial_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      455 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/hiv_medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1062 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/hiv_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1677 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/htn_initial_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      482 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/htn_medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1463 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/htn_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1309 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/investigations.py
--rw-r--r--   0 erikvw     (501) staff       (20)      343 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/malaria_test.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1494 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/medications.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5356 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/models/other_baseline_data.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2708 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/patient_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1529 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/reason_for_visit.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.958752 intecomm-edc-0.1.8/intecomm_subject/models/social_harms/
--rw-r--r--   0 erikvw     (501) staff       (20)       38 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/models/social_harms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3281 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/models/social_harms/model_factories.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_subject/models/social_harms/social_harms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      321 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/subject_requisition.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2930 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/subject_visit.py
--rw-r--r--   0 erikvw     (501) staff       (20)      752 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/subject_visit_missed.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1179 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/urine_dipstick_test.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1180 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/models/urine_pregnancy.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1290 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/models/viral_load_result.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2386 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_subject/models/vitals.py
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_subject/reference_model_configs.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.958911 intecomm-edc-0.1.8/intecomm_subject/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.959039 intecomm-edc-0.1.8/intecomm_subject/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_subject/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-03-14 02:25:40.000000 intecomm-edc-0.1.8/intecomm_subject/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.959820 intecomm-edc-0.1.8/intecomm_visit_schedule/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-07 23:18:25.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      172 2022-03-12 18:22:09.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      120 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.959949 intecomm-edc-0.1.8/intecomm_visit_schedule/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.960201 intecomm-edc-0.1.8/intecomm_visit_schedule/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.960607 intecomm-edc-0.1.8/intecomm_visit_schedule/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       79 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/tests/tests/test_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      116 2020-03-15 03:34:20.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-27 03:45:22.961791 intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/
--rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-11-20 02:36:08.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      819 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/comm_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17847 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/crfs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/inte_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2012 2022-11-29 06:19:20.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/requisitions.py
--rw-r--r--   0 erikvw     (501) staff       (20)      525 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5285 2023-01-27 03:45:15.000000 intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/visits.py
--rwxr-xr-x   0 erikvw     (501) staff       (20)      789 2021-11-22 15:06:01.000000 intecomm-edc-0.1.8/manage.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1908 2023-01-25 03:04:55.000000 intecomm-edc-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     6882 2023-01-18 00:12:58.000000 intecomm-edc-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1356 2023-01-27 03:45:22.962491 intecomm-edc-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.721067 intecomm-edc-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      129 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-13 15:16:15.000000 intecomm-edc-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.586579 intecomm-edc-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.602569 intecomm-edc-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2100 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1466 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1109 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      309 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2022-12-01 02:13:19.000000 intecomm-edc-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-11-22 15:26:51.000000 intecomm-edc-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1902 2023-01-30 02:26:37.721173 intecomm-edc-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1029 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-03-14 02:38:46.000000 intecomm-edc-0.1.9/VERSION
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.587366 intecomm-edc-0.1.9/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.602755 intecomm-edc-0.1.9/bin/nginx/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.603620 intecomm-edc-0.1.9/bin/nginx/conf/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1202 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/nginx/conf/intecomm_live.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      432 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/nginx/conf/intecomm_live_sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/nginx/conf/intecomm_uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      435 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/nginx/conf/intecomm_uat_sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/nginx/intecomm.clinicedc.org.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.586893 intecomm-edc-0.1.9/bin/nginx/www/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.587162 intecomm-edc-0.1.9/bin/nginx/www/html/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.603771 intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.604024 intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2297 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.604225 intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2281 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.604492 intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.604713 intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2334 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.604952 intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2318 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.605736 intecomm-edc-0.1.9/bin/systemd/
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      435 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/systemd/gunicorn-live.service
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      133 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/systemd/gunicorn-live.socket
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      433 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/systemd/gunicorn-uat.service
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      131 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/codecov.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     4590 2021-11-22 15:06:41.000000 intecomm-edc-0.1.9/env.sample
+-rw-r--r--   0 erikvw     (501) staff       (20)     1048 2021-08-13 15:16:15.000000 intecomm-edc-0.1.9/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.608885 intecomm-edc-0.1.9/intecomm_ae/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7311 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.610636 intecomm-edc-0.1.9/intecomm_ae/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      460 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      424 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/admin/ae_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      774 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/admin/ae_initial_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      403 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/admin/ae_susar_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      389 2022-11-30 17:58:11.000000 intecomm-edc-0.1.9/intecomm_ae/admin/ae_tmg_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2191 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/admin/death_report_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      452 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/admin/death_report_tmg_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      482 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/admin/death_report_tmg_second_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4157 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-10-18 02:23:36.000000 intecomm-edc-0.1.9/intecomm_ae/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      292 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1154 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-04-11 18:27:09.000000 intecomm-edc-0.1.9/intecomm_ae/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       36 2022-04-11 18:27:09.000000 intecomm-edc-0.1.9/intecomm_ae/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.612209 intecomm-edc-0.1.9/intecomm_ae/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      330 2022-10-18 02:20:14.000000 intecomm-edc-0.1.9/intecomm_ae/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/forms/ae_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      292 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/forms/ae_initial_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      280 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/forms/ae_susar_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      268 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/forms/ae_tmg_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1425 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/forms/death_report_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      322 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/forms/death_report_tmg_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      340 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/forms/death_report_tmg_second_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      874 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/forms/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1248 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.613479 intecomm-edc-0.1.9/intecomm_ae/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   144621 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_ae/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5272 2022-12-01 02:13:19.000000 intecomm-edc-0.1.9/intecomm_ae/migrations/0002_rename_narrative_aetmg_investigator_narrative_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1664 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_ae/migrations/0003_alter_deathreporttmg_cause_of_death_agreed_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.613953 intecomm-edc-0.1.9/intecomm_ae/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2020-05-15 02:40:42.000000 intecomm-edc-0.1.9/intecomm_ae/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2638 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/model_mixins/ae_review_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1799 2022-06-29 19:36:30.000000 intecomm-edc-0.1.9/intecomm_ae/model_mixins/death_report_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.615532 intecomm-edc-0.1.9/intecomm_ae/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      267 2022-10-18 02:17:22.000000 intecomm-edc-0.1.9/intecomm_ae/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/models/ae_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      343 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/models/ae_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      208 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/models/ae_susar.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      226 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/models/ae_tmg.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      442 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/models/death_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2021-07-05 19:24:26.000000 intecomm-edc-0.1.9/intecomm_ae/models/death_report_tmg.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      565 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/models/death_report_tmg_second.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      621 2022-06-29 19:36:30.000000 intecomm-edc-0.1.9/intecomm_ae/models/managers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.616170 intecomm-edc-0.1.9/intecomm_ae/pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)       70 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/pdf_reports/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/pdf_reports/ae_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      199 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/pdf_reports/death_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       77 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/pdf_reports/pdf_report_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.590670 intecomm-edc-0.1.9/intecomm_ae/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.590734 intecomm-edc-0.1.9/intecomm_ae/templates/intecomm_ae/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.616314 intecomm-edc-0.1.9/intecomm_ae/templates/intecomm_ae/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      889 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/templates/intecomm_ae/bootstrap3/ae_initial_description.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.616625 intecomm-edc-0.1.9/intecomm_ae/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1154 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/templatetags/protocol_ae_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.617042 intecomm-edc-0.1.9/intecomm_ae/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_ae/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.617188 intecomm-edc-0.1.9/intecomm_ae/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.1.9/intecomm_ae/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      259 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_ae/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-10-18 02:24:15.000000 intecomm-edc-0.1.9/intecomm_ae/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.617986 intecomm-edc-0.1.9/intecomm_auth/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_auth/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      233 2022-03-12 18:30:44.000000 intecomm-edc-0.1.9/intecomm_auth/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      682 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_auth/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1733 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_auth/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_auth/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.619429 intecomm-edc-0.1.9/intecomm_consent/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_consent/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      764 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.620132 intecomm-edc-0.1.9/intecomm_consent/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_consent/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3162 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/intecomm_consent/admin/subject_consent_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2751 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/admin/subject_reconsent_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:54:16.000000 intecomm-edc-0.1.9/intecomm_consent/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-03-12 18:10:23.000000 intecomm-edc-0.1.9/intecomm_consent/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1257 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       31 2021-10-27 22:32:32.000000 intecomm-edc-0.1.9/intecomm_consent/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.620684 intecomm-edc-0.1.9/intecomm_consent/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      139 2022-03-03 20:12:26.000000 intecomm-edc-0.1.9/intecomm_consent/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1498 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/intecomm_consent/forms/subject_consent_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_consent/forms/subject_reconsent_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.620854 intecomm-edc-0.1.9/intecomm_consent/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-03 20:12:26.000000 intecomm-edc-0.1.9/intecomm_consent/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.621056 intecomm-edc-0.1.9/intecomm_consent/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-03 20:12:26.000000 intecomm-edc-0.1.9/intecomm_consent/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/management/commands/create_missing_prescriptions.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.622862 intecomm-edc-0.1.9/intecomm_consent/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    69090 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_consent/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5397 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_consent/migrations/0002_remove_subjectconsent_intecomm_co_subject_145905_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1536 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/intecomm_consent/migrations/0003_alter_historicalsubjectconsent_language_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1952 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/intecomm_consent/migrations/0004_alter_historicalsubjectconsent_familiar_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1017 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_consent/migrations/0005_remove_subjectconsent_unique_consent_subject_id_and_version_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      697 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_consent/migrations/0006_historicalsubjectconsent_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_consent/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.623710 intecomm-edc-0.1.9/intecomm_consent/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      174 2021-08-09 19:25:29.000000 intecomm-edc-0.1.9/intecomm_consent/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_consent/models/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4389 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_consent/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5391 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_consent/models/subject_consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3631 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/models/subject_reconsent.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.591691 intecomm-edc-0.1.9/intecomm_consent/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.591748 intecomm-edc-0.1.9/intecomm_consent/templates/intecomm_consent/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.623974 intecomm-edc-0.1.9/intecomm_consent/templates/intecomm_consent/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1420 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_consent/templates/intecomm_consent/admin/subjectconsent_change_list.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.624456 intecomm-edc-0.1.9/intecomm_consent/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_consent/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_consent/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.624954 intecomm-edc-0.1.9/intecomm_consent/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.1.9/intecomm_consent/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3459 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/tests/tests/test_form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/tests/tests/test_subject_consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      924 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_consent/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.625793 intecomm-edc-0.1.9/intecomm_dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1948 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.626027 intecomm-edc-0.1.9/intecomm_dashboard/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.627313 intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/
+-rw-r--r--   0 erikvw     (501) staff       (20)      401 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/ae_initial_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      379 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/death_report_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      492 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/patient_log_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      432 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/subject_consent_model_wrappers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      411 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/subject_refusal_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1781 2023-01-23 13:57:43.000000 intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/subject_screening_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1853 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-06-24 09:14:59.000000 intecomm-edc-0.1.9/intecomm_dashboard/patterns.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.592221 intecomm-edc-0.1.9/intecomm_dashboard/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.592272 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.592471 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.629437 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/
+-rw-r--r--   0 erikvw     (501) staff       (20)      466 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/add_consent_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      239 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/dashboard_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      401 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/eligibility_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/patient_group_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      365 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/patient_log_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      437 2022-10-20 00:50:06.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/refusal_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      341 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/screening_button.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.629769 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2986 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.630574 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2061 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/comm_listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.630866 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)      230 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard/top_bar.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-10-18 02:52:50.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1382 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/inte_listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.631255 intecomm-edc-0.1.9/intecomm_dashboard/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6019 2022-11-28 02:44:46.000000 intecomm-edc-0.1.9/intecomm_dashboard/templatetags/protocol_dashboard_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.632122 intecomm-edc-0.1.9/intecomm_dashboard/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      720 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/tests/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.632269 intecomm-edc-0.1.9/intecomm_dashboard/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2937 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_dashboard/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1517 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.632364 intecomm-edc-0.1.9/intecomm_dashboard/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.633026 intecomm-edc-0.1.9/intecomm_dashboard/views/ae/
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/ae/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      458 2022-10-18 02:53:29.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/ae/ae_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      496 2022-10-18 02:53:29.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/ae/death_report_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.633514 intecomm-edc-0.1.9/intecomm_dashboard/views/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/screening/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2253 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/screening/listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.633695 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)      149 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.634181 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      477 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/dashboard/dashboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.634958 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/listboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)      176 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/listboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1202 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/listboard/comm_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      808 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/listboard/inte_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      786 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_dashboard/views/subject/listboard/subject_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.636788 intecomm-edc-0.1.9/intecomm_edc/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      927 2022-07-07 11:06:18.000000 intecomm-edc-0.1.9/intecomm_edc/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      382 2022-03-12 18:45:28.000000 intecomm-edc-0.1.9/intecomm_edc/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      793 2022-03-12 18:45:28.000000 intecomm-edc-0.1.9/intecomm_edc/celery.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-04 23:21:43.000000 intecomm-edc-0.1.9/intecomm_edc/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1309 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_edc/navbars.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.639013 intecomm-edc-0.1.9/intecomm_edc/settings/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-03 04:33:09.000000 intecomm-edc-0.1.9/intecomm_edc/settings/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      430 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_edc/settings/debug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17573 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_edc/settings/defaults.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1065 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/settings/live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1936 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/settings/logging.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      595 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/settings/minimal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1302 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/settings/uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.593639 intecomm-edc-0.1.9/intecomm_edc/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.593690 intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.639831 intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2021-08-09 19:25:29.000000 intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/base.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     3191 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_comm.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2172 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_inte.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2759 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/grouping.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2543 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.639973 intecomm-edc-0.1.9/intecomm_edc/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 intecomm-edc-0.1.9/intecomm_edc/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.640168 intecomm-edc-0.1.9/intecomm_edc/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.1.9/intecomm_edc/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/tests/tests/test_endpoints.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3419 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_edc/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.640991 intecomm-edc-0.1.9/intecomm_edc/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      170 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      622 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/views/followup_comm_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      649 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_edc/views/followup_inte_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      518 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/views/grouping_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      502 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_edc/views/home_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      179 2022-03-12 18:45:28.000000 intecomm-edc-0.1.9/intecomm_edc/wsgi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-03-12 18:45:28.000000 intecomm-edc-0.1.9/intecomm_edc/wsgi_live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:45:28.000000 intecomm-edc-0.1.9/intecomm_edc/wsgi_uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.637717 intecomm-edc-0.1.9/intecomm_edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1902 2023-01-30 02:26:37.000000 intecomm-edc-0.1.9/intecomm_edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    28083 2023-01-30 02:26:37.000000 intecomm-edc-0.1.9/intecomm_edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-01-30 02:26:37.000000 intecomm-edc-0.1.9/intecomm_edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-19 12:31:42.000000 intecomm-edc-0.1.9/intecomm_edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)      159 2023-01-30 02:26:37.000000 intecomm-edc-0.1.9/intecomm_edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      223 2023-01-30 02:26:37.000000 intecomm-edc-0.1.9/intecomm_edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.641915 intecomm-edc-0.1.9/intecomm_export/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_export/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_export/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-03-12 18:43:23.000000 intecomm-edc-0.1.9/intecomm_export/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-03-12 18:43:17.000000 intecomm-edc-0.1.9/intecomm_export/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_export/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-03-12 18:43:14.000000 intecomm-edc-0.1.9/intecomm_export/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_export/views.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.643350 intecomm-edc-0.1.9/intecomm_group/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.644766 intecomm-edc-0.1.9/intecomm_group/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_group/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/admin/autocomplete_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2709 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/admin/community_care_location_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      304 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3546 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/admin/patient_followup_call_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3808 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_group/admin/patient_group_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1914 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/admin/patient_group_appointment_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2032 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/admin/patient_group_meeting_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9250 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_group/admin/patient_log_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      292 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      800 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      100 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/exceptions.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.645600 intecomm-edc-0.1.9/intecomm_group/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/forms/community_care_location_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      372 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/forms/patient_group_appointment_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      497 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_group/forms/patient_group_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/forms/patient_group_meeting_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.647718 intecomm-edc-0.1.9/intecomm_group/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    29539 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3394 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0002_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      599 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0003_alter_historicalpatientgroup_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      666 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0004_alter_patientgroup_patients.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17785 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0005_patientfollowupcall_historicalpatientfollowupcall.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2953 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0006_remove_historicalpatientgroup_enforce_group_size_min_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3531 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0007_remove_historicalpatientfollowupcall_attend_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2555 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0008_patientgroup_dm_patients_patientgroup_hiv_patients_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1518 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0009_auto_20221126_0358.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      576 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_group/migrations/0010_alter_patientgroup_managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.649275 intecomm-edc-0.1.9/intecomm_group/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      536 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_group/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2278 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/models/community_care_location.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1214 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/models/patient_followup_call.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4070 2023-01-22 23:16:39.000000 intecomm-edc-0.1.9/intecomm_group/models/patient_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      997 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/models/patient_group_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1192 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/models/patient_group_meeting.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      150 2023-01-23 13:41:17.000000 intecomm-edc-0.1.9/intecomm_group/models/proxy_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2745 2022-12-06 23:12:40.000000 intecomm-edc-0.1.9/intecomm_group/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1946 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/models/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.594421 intecomm-edc-0.1.9/intecomm_group/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.594474 intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.650127 intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1315 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/communitycarelocation_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1522 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/patientfollowupcall_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1354 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/patientgroup_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1475 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/patientgroupappointment_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1457 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/patientgroupmeeting_change_list.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.650359 intecomm-edc-0.1.9/intecomm_group/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.650501 intecomm-edc-0.1.9/intecomm_group/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_group/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1522 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_group/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.651999 intecomm-edc-0.1.9/intecomm_labs/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-02 03:53:00.000000 intecomm-edc-0.1.9/intecomm_labs/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       87 2021-07-05 19:24:26.000000 intecomm-edc-0.1.9/intecomm_labs/aliquot_types.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      209 2022-03-12 18:19:55.000000 intecomm-edc-0.1.9/intecomm_labs/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1011 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_labs/lab_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      128 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_labs/labs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      481 2022-03-12 18:19:03.000000 intecomm-edc-0.1.9/intecomm_labs/list_data.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      500 2021-09-17 02:16:20.000000 intecomm-edc-0.1.9/intecomm_labs/processing_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      516 2022-03-12 18:18:51.000000 intecomm-edc-0.1.9/intecomm_labs/reportables.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.652325 intecomm-edc-0.1.9/intecomm_labs/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_labs/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.652885 intecomm-edc-0.1.9/intecomm_labs/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_labs/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_labs/tests/tests/test_labs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      539 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_labs/tests/tests/test_reportables.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      116 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_labs/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.654763 intecomm-edc-0.1.9/intecomm_lists/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_lists/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      630 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_lists/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-03-14 02:24:52.000000 intecomm-edc-0.1.9/intecomm_lists/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-03-12 18:10:47.000000 intecomm-edc-0.1.9/intecomm_lists/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_lists/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_lists/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3529 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_lists/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.655964 intecomm-edc-0.1.9/intecomm_lists/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    77606 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_lists/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      466 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_lists/migrations/0002_delete_reasonsfortesting_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2718 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_lists/migrations/0003_dmmanagement_dmmanagement_intecomm_li_id_b4d41f_idx.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_lists/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4770 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_lists/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.656070 intecomm-edc-0.1.9/intecomm_lists/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_lists/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.656275 intecomm-edc-0.1.9/intecomm_lists/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_lists/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      212 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_lists/tests/tests/test_lists.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-03-12 18:05:17.000000 intecomm-edc-0.1.9/intecomm_lists/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.657868 intecomm-edc-0.1.9/intecomm_prn/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_prn/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3105 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.659722 intecomm-edc-0.1.9/intecomm_prn/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      444 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4603 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_prn/admin/end_of_study_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1634 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_prn/admin/loss_to_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      354 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/admin/offschedule_comm_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1769 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/admin/offschedule_inte_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      286 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/admin/onschedule_comm_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1494 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/admin/onschedule_inte_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      781 2022-12-01 02:13:19.000000 intecomm-edc-0.1.9/intecomm_prn/admin/protocol_incident_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      659 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_prn/admin/subject_transfer_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-10-18 02:27:53.000000 intecomm-edc-0.1.9/intecomm_prn/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      288 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_prn/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3151 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_prn/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      104 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.660923 intecomm-edc-0.1.9/intecomm_prn/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      322 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      938 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_prn/forms/end_of_study_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1405 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_prn/forms/loss_to_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      960 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/forms/offschedule_comm_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      960 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/forms/offschedule_inte_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_prn/forms/protocol_incident_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      818 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_prn/forms/subject_transfer_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2336 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_prn/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.662501 intecomm-edc-0.1.9/intecomm_prn/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   149191 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_prn/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3534 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_prn/migrations/0002_remove_endofstudy_delivery_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1914 2022-12-01 02:13:19.000000 intecomm-edc-0.1.9/intecomm_prn/migrations/0003_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3193 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/migrations/0004_rename_historicaloffschedulebaseline_historicaloffschedulecomm_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3238 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/migrations/0005_rename_historicaloffschedulefollowup_historicaloffscheduleinte_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_prn/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.664205 intecomm-edc-0.1.9/intecomm_prn/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      356 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3359 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_prn/models/end_of_study.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2149 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_prn/models/loss_to_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      645 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/models/offschedule_comm.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      643 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/models/offschedule_inte.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      500 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/models/onschedule_comm.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      498 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_prn/models/onschedule_inte.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1088 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_prn/models/protocol_incident.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      266 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_prn/models/subject_transfer.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.664590 intecomm-edc-0.1.9/intecomm_prn/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_prn/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.664747 intecomm-edc-0.1.9/intecomm_prn/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_prn/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_prn/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-10-18 02:47:10.000000 intecomm-edc-0.1.9/intecomm_prn/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.667663 intecomm-edc-0.1.9/intecomm_screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_screening/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.670446 intecomm-edc-0.1.9/intecomm_screening/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      533 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2249 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/admin/health_facility_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2305 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/admin/health_talk_log_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5080 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4467 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/admin/patient_call_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2133 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/admin/patient_call_inlines.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8184 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/admin/patient_group_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13401 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/admin/patient_log_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      258 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/admin/site_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2178 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/admin/subject_refusal_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9586 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/intecomm_screening/admin/subject_screening_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2022-03-12 17:44:29.000000 intecomm-edc-0.1.9/intecomm_screening/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      553 2022-03-12 17:44:16.000000 intecomm-edc-0.1.9/intecomm_screening/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      549 2022-10-18 20:05:10.000000 intecomm-edc-0.1.9/intecomm_screening/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      402 2022-03-03 20:12:26.000000 intecomm-edc-0.1.9/intecomm_screening/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1065 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      597 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       33 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.671789 intecomm-edc-0.1.9/intecomm_screening/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      356 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      372 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/forms/health_facility_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      367 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/forms/health_talk_log_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      357 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/forms/patient_call_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      362 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/forms/patient_group_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      532 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/forms/patient_log_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1675 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/forms/subject_refusal_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1163 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/forms/subject_screening_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.677832 intecomm-edc-0.1.9/intecomm_screening/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   128990 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0002_remove_healthtalklog_unique_lower_name_report_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2758 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0003_site_remove_historicalpatientlog_patient_group_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1451 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0004_rename_name_historicalpatientlog_legal_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2034 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0005_historicalpatientcall_alt_contact_number_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3723 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0006_remove_historicalpatientcall_willing_to_attend_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2229 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0007_historicalpatientlog_last_4_contact_number_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7010 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0008_rename_last_routine_appt_date_historicalpatientlog_last_appt_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3259 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0009_historicalsubjectscreening_familiar_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      717 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0010_historicalpatientlog_age_in_years_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3940 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0011_rename_hf_identifier_historicalpatientlog_hospital_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1147 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0012_alter_historicalpatientcall_last_attend_clinic_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1893 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0013_alter_healthfacility_distance_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3542 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0014_alter_historicalpatientlog_familiar_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      561 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0015_remove_healthtalklog_unique_health_facility_report_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/0016_historicalpatientlog_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_screening/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.678084 intecomm-edc-0.1.9/intecomm_screening/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       60 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2649 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/model_mixins/patient_call_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.679849 intecomm-edc-0.1.9/intecomm_screening/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      461 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2259 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/models/health_facility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1975 2022-12-01 03:07:11.000000 intecomm-edc-0.1.9/intecomm_screening/models/health_talk_log.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/models/location.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1186 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/models/patient_call.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6458 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/models/patient_log.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.680389 intecomm-edc-0.1.9/intecomm_screening/models/proxy_models/
+-rw-r--r--   0 erikvw     (501) staff       (20)       63 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/models/proxy_models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      265 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/models/proxy_models/patient_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      185 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/models/proxy_models/site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2086 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2216 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/models/subject_refusal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7895 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/models/subject_screening.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      135 2022-03-12 17:42:16.000000 intecomm-edc-0.1.9/intecomm_screening/offline_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.596171 intecomm-edc-0.1.9/intecomm_screening/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.681958 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.682995 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/healthfacility_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1270 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/healthtalklog_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1270 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/patientcall_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1270 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/patientgroup_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1270 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/patientlog_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      719 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/subjectscreening_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      240 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/change_list_appts.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/change_list_contacts.html
+-rw-r--r--   0 erikvw     (501) staff       (20)       94 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/change_list_dx.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      176 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/change_list_group.html
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/change_list_hospital_identifier.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1424 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/change_list_screen_and_consent.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      462 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/change_list_talks.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1344 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/group_management.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.683502 intecomm-edc-0.1.9/intecomm_screening/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_screening/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_screening/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     6834 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/tests/intecomm_test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.683878 intecomm-edc-0.1.9/intecomm_screening/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 intecomm-edc-0.1.9/intecomm_screening/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2918 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/intecomm_screening/tests/tests/test_screening.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      579 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1701 2022-11-23 01:31:30.000000 intecomm-edc-0.1.9/intecomm_screening/utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1569 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_screening/views.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.684987 intecomm-edc-0.1.9/intecomm_sites/
+-rw-r--r--   0 erikvw     (501) staff       (20)       43 2021-07-05 19:24:26.000000 intecomm-edc-0.1.9/intecomm_sites/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      943 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_sites/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      857 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_sites/intecomm_site.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.685218 intecomm-edc-0.1.9/intecomm_sites/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-12 18:03:07.000000 intecomm-edc-0.1.9/intecomm_sites/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_sites/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5871 2022-11-30 03:04:06.000000 intecomm-edc-0.1.9/intecomm_sites/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.685459 intecomm-edc-0.1.9/intecomm_sites/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_sites/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      346 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_sites/tests/site_test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.687504 intecomm-edc-0.1.9/intecomm_subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-22 15:10:26.000000 intecomm-edc-0.1.9/intecomm_subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      512 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.694327 intecomm-edc-0.1.9/intecomm_subject/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2046 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/arv_regimens_admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.695522 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      414 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      723 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_fbc_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      991 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_glu_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      785 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_hba1c_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      746 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_ins_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      746 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_lft_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      760 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_lipid_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4599 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_rft_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      584 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/cd4_result_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2139 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/clinical_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1708 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/clinical_review_baseline_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1556 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/complications_baseline_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1562 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/complications_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      755 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/concomitant_medication_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1547 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/admin/dm_initial_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      442 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/dm_medication_adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/dm_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      696 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/drug_refill_dm_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      771 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/drug_refill_hiv_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      707 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/drug_refill_htn_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1816 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/family_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      349 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1068 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/glucose_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      679 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/hba1c_result_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5682 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/admin/health_economics_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1862 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/hiv_initial_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/hiv_medication_adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/hiv_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      947 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/htn_initial_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/htn_medication_adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1031 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/htn_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      423 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/malaria_test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      816 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/medications_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1884 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2861 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/admin/other_baseline_data_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5264 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/admin/social_harms_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1738 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/subject_requisition_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1330 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/subject_visit_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1233 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/admin/subject_visit_missed_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1075 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/urine_dipstick_test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      968 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/urine_pregnancy_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      626 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/admin/viral_load_result_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2230 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/admin/vitals_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:18:07.000000 intecomm-edc-0.1.9/intecomm_subject/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-03-12 18:18:07.000000 intecomm-edc-0.1.9/intecomm_subject/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5928 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      435 2023-01-27 01:28:16.000000 intecomm-edc-0.1.9/intecomm_subject/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.699739 intecomm-edc-0.1.9/intecomm_subject/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1399 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/forms/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.701015 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      400 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      715 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_fbc_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      824 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_glu_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_hba1c_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      723 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_ins_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      715 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_lft_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      731 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_lipid_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1363 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_rft_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      646 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/cd4_result_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      685 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/clinical_review_baseline.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      921 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/forms/clinical_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      490 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/concomitant_medication_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      335 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/dm_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      355 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/drug_refill_dm_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/drug_refill_hiv_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/drug_refill_htn_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/drug_supply_dm_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      781 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/drug_supply_hiv_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      393 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/drug_supply_htn_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      371 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/forms/health_economics_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      340 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/hiv_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      340 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/htn_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/malaria_test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      268 2022-12-05 14:48:19.000000 intecomm-edc-0.1.9/intecomm_subject/forms/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/forms/social_harms_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      954 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/forms/subject_requisition_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      757 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/forms/subject_visit_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2277 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/forms/subject_visit_missed_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      829 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/urine_dipstick_test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/urine_pregnancy_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      682 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/forms/viral_load_result_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      343 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/forms/vitals_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.701430 intecomm-edc-0.1.9/intecomm_subject/metadata_rules/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/metadata_rules/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4127 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/metadata_rules/metadata_rules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      815 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/metadata_rules/predicates.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.707631 intecomm-edc-0.1.9/intecomm_subject/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)  1030443 2022-12-02 22:40:22.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    58038 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0002_remove_historicaldminitialreview_managed_by_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1792 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0003_alter_historicalsocialharms_coworkers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    24956 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0004_historicalsocialharms_employment_impact_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    82106 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0005_alter_historicalsocialharms_coworkers_impact_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1090 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0006_alter_healtheconomics_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1498 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0007_alter_historicalotherbaselinedata_alcohol_consumption_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    23862 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0008_historicalvitals_vitals_remove_indicators_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3555 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0009_remove_historicalvitals_bp_measured_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3178 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0010_remove_historicalvitals_weight_is_estmated_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1501 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0011_remove_clinicalreviewbaseline_complications_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/0012_alter_historicalvitals_heart_rate_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-12 18:03:07.000000 intecomm-edc-0.1.9/intecomm_subject/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.708836 intecomm-edc-0.1.9/intecomm_subject/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4828 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/model_mixins/clinical_review_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      248 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/model_mixins/crf_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/model_mixins/crf_with_action_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      560 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/model_mixins/followup_review_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/model_mixins/search_slug_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.715599 intecomm-edc-0.1.9/intecomm_subject/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1889 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/arv_regimens.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.717183 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      337 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1252 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_fbc.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1008 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_glu.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      958 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_hba1c.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      974 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_ins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1157 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_lft.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1090 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_lipid.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1568 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_rft.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1090 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/cd4_result.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4222 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/clinical_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/models/clinical_review_baseline.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4354 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/complications_baseline.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2831 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/complications_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      369 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/concomitant_medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1968 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/models/dm_initial_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      473 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/dm_medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      404 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/dm_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/drug_refill_dm.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1429 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/drug_refill_hiv.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      591 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/drug_refill_htn.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      559 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/drug_supply_dm.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      617 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/drug_supply_hiv.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      573 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/drug_supply_htn.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3521 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/family_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      335 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/glucose.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/hba1c_result.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18724 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/models/health_economics.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4525 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/hiv_initial_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      455 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/hiv_medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1062 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/hiv_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1677 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/htn_initial_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      482 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/htn_medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1463 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/htn_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1309 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/investigations.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      343 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/malaria_test.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1494 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/medications.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5356 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/models/other_baseline_data.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2708 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/patient_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1529 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/reason_for_visit.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.717670 intecomm-edc-0.1.9/intecomm_subject/models/social_harms/
+-rw-r--r--   0 erikvw     (501) staff       (20)       38 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/models/social_harms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3281 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/models/social_harms/model_factories.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_subject/models/social_harms/social_harms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      321 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/subject_requisition.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2930 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/subject_visit.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      752 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/subject_visit_missed.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1179 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/urine_dipstick_test.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1180 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/models/urine_pregnancy.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1290 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/models/viral_load_result.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2386 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_subject/models/vitals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_subject/reference_model_configs.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.717840 intecomm-edc-0.1.9/intecomm_subject/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.717956 intecomm-edc-0.1.9/intecomm_subject/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_subject/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-03-14 02:25:40.000000 intecomm-edc-0.1.9/intecomm_subject/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.718779 intecomm-edc-0.1.9/intecomm_visit_schedule/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-07 23:18:25.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      172 2022-03-12 18:22:09.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      120 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.718893 intecomm-edc-0.1.9/intecomm_visit_schedule/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.719092 intecomm-edc-0.1.9/intecomm_visit_schedule/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.719491 intecomm-edc-0.1.9/intecomm_visit_schedule/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       79 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/tests/tests/test_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      116 2020-03-15 03:34:20.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-30 02:26:37.720924 intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/
+-rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-11-20 02:36:08.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      819 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/comm_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17847 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/crfs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/inte_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2012 2022-11-29 06:19:20.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/requisitions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      525 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5285 2023-01-27 03:45:15.000000 intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/visits.py
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      789 2021-11-22 15:06:01.000000 intecomm-edc-0.1.9/manage.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1908 2023-01-25 03:04:55.000000 intecomm-edc-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     6882 2023-01-18 00:12:58.000000 intecomm-edc-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1357 2023-01-30 02:26:37.721551 intecomm-edc-0.1.9/setup.cfg
```

### Comparing `intecomm-edc-0.1.8/.github/workflows/build.yml` & `intecomm-edc-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/.gitignore` & `intecomm-edc-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/.pre-commit-config.yaml` & `intecomm-edc-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/LICENSE` & `intecomm-edc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/PKG-INFO` & `intecomm-edc-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-edc
-Version: 0.1.8
+Version: 0.1.9
 Summary: INTECOMM Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 Home-page: https://github.com/intecomm-trial/intecomm-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-edc-0.1.8/README.rst` & `intecomm-edc-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/bin/nginx/conf/intecomm_live.conf` & `intecomm-edc-0.1.9/bin/nginx/conf/intecomm_live.conf`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/bin/nginx/conf/intecomm_uat.conf` & `intecomm-edc-0.1.9/bin/nginx/conf/intecomm_uat.conf`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/index.html` & `intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/index.html` & `intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/index.html` & `intecomm-edc-0.1.9/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/index.html` & `intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/index.html` & `intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/index.html` & `intecomm-edc-0.1.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/env.sample` & `intecomm-edc-0.1.9/env.sample`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/holidays.csv` & `intecomm-edc-0.1.9/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/action_items.py` & `intecomm-edc-0.1.9/intecomm_ae/action_items.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/admin/ae_initial_admin.py` & `intecomm-edc-0.1.9/intecomm_ae/admin/ae_initial_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/admin/death_report_admin.py` & `intecomm-edc-0.1.9/intecomm_ae/admin/death_report_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/admin/modeladmin_mixins.py` & `intecomm-edc-0.1.9/intecomm_ae/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/baker_recipes.py` & `intecomm-edc-0.1.9/intecomm_ae/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/choices.py` & `intecomm-edc-0.1.9/intecomm_ae/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/forms/death_report_form.py` & `intecomm-edc-0.1.9/intecomm_ae/forms/death_report_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/forms/modelform_mixins.py` & `intecomm-edc-0.1.9/intecomm_ae/forms/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/list_data.py` & `intecomm-edc-0.1.9/intecomm_ae/list_data.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/migrations/0001_initial.py` & `intecomm-edc-0.1.9/intecomm_ae/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/migrations/0002_rename_narrative_aetmg_investigator_narrative_and_more.py` & `intecomm-edc-0.1.9/intecomm_ae/migrations/0002_rename_narrative_aetmg_investigator_narrative_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/migrations/0003_alter_deathreporttmg_cause_of_death_agreed_and_more.py` & `intecomm-edc-0.1.9/intecomm_ae/migrations/0003_alter_deathreporttmg_cause_of_death_agreed_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/model_mixins/ae_review_model_mixin.py` & `intecomm-edc-0.1.9/intecomm_ae/model_mixins/ae_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/model_mixins/death_report_model_mixin.py` & `intecomm-edc-0.1.9/intecomm_ae/model_mixins/death_report_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/models/death_report_tmg_second.py` & `intecomm-edc-0.1.9/intecomm_ae/models/death_report_tmg_second.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/models/managers.py` & `intecomm-edc-0.1.9/intecomm_ae/models/managers.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/templates/intecomm_ae/bootstrap3/ae_initial_description.html` & `intecomm-edc-0.1.9/intecomm_ae/templates/intecomm_ae/bootstrap3/ae_initial_description.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/templatetags/protocol_ae_extras.py` & `intecomm-edc-0.1.9/intecomm_ae/templatetags/protocol_ae_extras.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_ae/tests/holidays.csv` & `intecomm-edc-0.1.9/intecomm_ae/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_auth/auth_objects.py` & `intecomm-edc-0.1.9/intecomm_auth/auth_objects.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_auth/auths.py` & `intecomm-edc-0.1.9/intecomm_auth/auths.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/action_items.py` & `intecomm-edc-0.1.9/intecomm_consent/action_items.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/admin/subject_consent_admin.py` & `intecomm-edc-0.1.9/intecomm_consent/admin/subject_consent_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/admin/subject_reconsent_admin.py` & `intecomm-edc-0.1.9/intecomm_consent/admin/subject_reconsent_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/baker_recipes.py` & `intecomm-edc-0.1.9/intecomm_consent/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/forms/subject_consent_form.py` & `intecomm-edc-0.1.9/intecomm_consent/forms/subject_consent_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/forms/subject_reconsent_form.py` & `intecomm-edc-0.1.9/intecomm_consent/forms/subject_reconsent_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/migrations/0001_initial.py` & `intecomm-edc-0.1.9/intecomm_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/migrations/0002_remove_subjectconsent_intecomm_co_subject_145905_idx_and_more.py` & `intecomm-edc-0.1.9/intecomm_consent/migrations/0002_remove_subjectconsent_intecomm_co_subject_145905_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/migrations/0003_alter_historicalsubjectconsent_language_and_more.py` & `intecomm-edc-0.1.9/intecomm_consent/migrations/0003_alter_historicalsubjectconsent_language_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/migrations/0004_alter_historicalsubjectconsent_familiar_name_and_more.py` & `intecomm-edc-0.1.9/intecomm_consent/migrations/0004_alter_historicalsubjectconsent_familiar_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/migrations/0005_remove_subjectconsent_unique_consent_subject_id_and_version_and_more.py` & `intecomm-edc-0.1.9/intecomm_consent/migrations/0005_remove_subjectconsent_unique_consent_subject_id_and_version_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/migrations/0006_historicalsubjectconsent_group_identifier_and_more.py` & `intecomm-edc-0.1.9/intecomm_consent/migrations/0006_historicalsubjectconsent_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/models/signals.py` & `intecomm-edc-0.1.9/intecomm_consent/models/signals.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/models/subject_consent.py` & `intecomm-edc-0.1.9/intecomm_consent/models/subject_consent.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/models/subject_reconsent.py` & `intecomm-edc-0.1.9/intecomm_consent/models/subject_reconsent.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/templates/intecomm_consent/admin/subjectconsent_change_list.html` & `intecomm-edc-0.1.9/intecomm_consent/templates/intecomm_consent/admin/subjectconsent_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/tests/holidays.csv` & `intecomm-edc-0.1.9/intecomm_consent/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/tests/tests/test_form_validators.py` & `intecomm-edc-0.1.9/intecomm_consent/tests/tests/test_form_validators.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_consent/tests/urls.py` & `intecomm-edc-0.1.9/intecomm_consent/tests/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/apps.py` & `intecomm-edc-0.1.9/intecomm_dashboard/apps.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/model_wrappers/subject_screening_model_wrapper.py` & `intecomm-edc-0.1.9/intecomm_dashboard/model_wrappers/subject_screening_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/navbars.py` & `intecomm-edc-0.1.9/intecomm_dashboard/navbars.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/listboard.html` & `intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/listboard.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/comm_listboard.html` & `intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/comm_listboard.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/inte_listboard.html` & `intecomm-edc-0.1.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/inte_listboard.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/templatetags/protocol_dashboard_extras.py` & `intecomm-edc-0.1.9/intecomm_dashboard/templatetags/protocol_dashboard_extras.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/tests/admin.py` & `intecomm-edc-0.1.9/intecomm_dashboard/tests/admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/tests/holidays.csv` & `intecomm-edc-0.1.9/intecomm_dashboard/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/tests/urls.py` & `intecomm-edc-0.1.9/intecomm_dashboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/urls.py` & `intecomm-edc-0.1.9/intecomm_dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/views/screening/listboard_view.py` & `intecomm-edc-0.1.9/intecomm_dashboard/views/screening/listboard_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/views/subject/listboard/comm_listboard_view.py` & `intecomm-edc-0.1.9/intecomm_dashboard/views/subject/listboard/comm_listboard_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/views/subject/listboard/inte_listboard_view.py` & `intecomm-edc-0.1.9/intecomm_dashboard/views/subject/listboard/inte_listboard_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_dashboard/views/subject/listboard/subject_listboard_view.py` & `intecomm-edc-0.1.9/intecomm_dashboard/views/subject/listboard/subject_listboard_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/admin.py` & `intecomm-edc-0.1.9/intecomm_edc/admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/celery.py` & `intecomm-edc-0.1.9/intecomm_edc/celery.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/navbars.py` & `intecomm-edc-0.1.9/intecomm_edc/navbars.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/settings/defaults.py` & `intecomm-edc-0.1.9/intecomm_edc/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/settings/live.py` & `intecomm-edc-0.1.9/intecomm_edc/settings/live.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/settings/logging.py` & `intecomm-edc-0.1.9/intecomm_edc/settings/logging.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/settings/minimal.py` & `intecomm-edc-0.1.9/intecomm_edc/settings/minimal.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/settings/uat.py` & `intecomm-edc-0.1.9/intecomm_edc/settings/uat.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_comm.html` & `intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_comm.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_inte.html` & `intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_inte.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/grouping.html` & `intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/grouping.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/templates/intecomm_edc/bootstrap3/home.html` & `intecomm-edc-0.1.9/intecomm_edc/templates/intecomm_edc/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/urls.py` & `intecomm-edc-0.1.9/intecomm_edc/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/views/followup_comm_view.py` & `intecomm-edc-0.1.9/intecomm_edc/views/followup_comm_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/views/followup_inte_view.py` & `intecomm-edc-0.1.9/intecomm_edc/views/followup_inte_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc/views/grouping_view.py` & `intecomm-edc-0.1.9/intecomm_edc/views/grouping_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_edc.egg-info/PKG-INFO` & `intecomm-edc-0.1.9/intecomm_edc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-edc
-Version: 0.1.8
+Version: 0.1.9
 Summary: INTECOMM Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 Home-page: https://github.com/intecomm-trial/intecomm-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-edc-0.1.8/intecomm_edc.egg-info/SOURCES.txt` & `intecomm-edc-0.1.9/intecomm_edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/admin/community_care_location_admin.py` & `intecomm-edc-0.1.9/intecomm_group/admin/community_care_location_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/admin/patient_followup_call_admin.py` & `intecomm-edc-0.1.9/intecomm_group/admin/patient_followup_call_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/admin/patient_group_admin.py` & `intecomm-edc-0.1.9/intecomm_group/admin/patient_group_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/admin/patient_group_appointment_admin.py` & `intecomm-edc-0.1.9/intecomm_group/admin/patient_group_appointment_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/admin/patient_group_meeting_admin.py` & `intecomm-edc-0.1.9/intecomm_group/admin/patient_group_meeting_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/admin/patient_log_admin.py` & `intecomm-edc-0.1.9/intecomm_group/admin/patient_log_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/choices.py` & `intecomm-edc-0.1.9/intecomm_group/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0001_initial.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0002_initial.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0003_alter_historicalpatientgroup_group_identifier_and_more.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0003_alter_historicalpatientgroup_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0004_alter_patientgroup_patients.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0004_alter_patientgroup_patients.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0005_patientfollowupcall_historicalpatientfollowupcall.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0005_patientfollowupcall_historicalpatientfollowupcall.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0006_remove_historicalpatientgroup_enforce_group_size_min_and_more.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0006_remove_historicalpatientgroup_enforce_group_size_min_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0007_remove_historicalpatientfollowupcall_attend_date_and_more.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0007_remove_historicalpatientfollowupcall_attend_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0008_patientgroup_dm_patients_patientgroup_hiv_patients_and_more.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0008_patientgroup_dm_patients_patientgroup_hiv_patients_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0009_auto_20221126_0358.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0009_auto_20221126_0358.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/migrations/0010_alter_patientgroup_managers.py` & `intecomm-edc-0.1.9/intecomm_group/migrations/0010_alter_patientgroup_managers.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/models/__init__.py` & `intecomm-edc-0.1.9/intecomm_group/models/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/models/community_care_location.py` & `intecomm-edc-0.1.9/intecomm_group/models/community_care_location.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/models/patient_followup_call.py` & `intecomm-edc-0.1.9/intecomm_group/models/patient_followup_call.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/models/patient_group.py` & `intecomm-edc-0.1.9/intecomm_group/models/patient_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/models/patient_group_appointment.py` & `intecomm-edc-0.1.9/intecomm_group/models/patient_group_appointment.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/models/patient_group_meeting.py` & `intecomm-edc-0.1.9/intecomm_group/models/patient_group_meeting.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/models/signals.py` & `intecomm-edc-0.1.9/intecomm_group/models/signals.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/models/utils.py` & `intecomm-edc-0.1.9/intecomm_group/models/utils.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/communitycarelocation_change_list.html` & `intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/communitycarelocation_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/patientfollowupcall_change_list.html` & `intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/patientfollowupcall_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/patientgroup_change_list.html` & `intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/patientgroup_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/patientgroupappointment_change_list.html` & `intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/patientgroupappointment_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/templates/intecomm_group/admin/patientgroupmeeting_change_list.html` & `intecomm-edc-0.1.9/intecomm_group/templates/intecomm_group/admin/patientgroupmeeting_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/tests/holidays.csv` & `intecomm-edc-0.1.9/intecomm_group/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_group/utils.py` & `intecomm-edc-0.1.9/intecomm_group/utils.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_labs/lab_profiles.py` & `intecomm-edc-0.1.9/intecomm_labs/lab_profiles.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_labs/reportables.py` & `intecomm-edc-0.1.9/intecomm_labs/reportables.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_labs/tests/tests/test_labs.py` & `intecomm-edc-0.1.9/intecomm_labs/tests/tests/test_labs.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_labs/tests/tests/test_reportables.py` & `intecomm-edc-0.1.9/intecomm_labs/tests/tests/test_reportables.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_lists/admin.py` & `intecomm-edc-0.1.9/intecomm_lists/admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_lists/list_data.py` & `intecomm-edc-0.1.9/intecomm_lists/list_data.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_lists/migrations/0001_initial.py` & `intecomm-edc-0.1.9/intecomm_lists/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_lists/migrations/0003_dmmanagement_dmmanagement_intecomm_li_id_b4d41f_idx.py` & `intecomm-edc-0.1.9/intecomm_lists/migrations/0003_dmmanagement_dmmanagement_intecomm_li_id_b4d41f_idx.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_lists/models.py` & `intecomm-edc-0.1.9/intecomm_lists/models.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/action_items.py` & `intecomm-edc-0.1.9/intecomm_prn/action_items.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/admin/end_of_study_admin.py` & `intecomm-edc-0.1.9/intecomm_prn/admin/end_of_study_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/admin/loss_to_followup_admin.py` & `intecomm-edc-0.1.9/intecomm_prn/admin/loss_to_followup_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/admin/offschedule_inte_admin.py` & `intecomm-edc-0.1.9/intecomm_prn/admin/offschedule_inte_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/admin/onschedule_inte_admin.py` & `intecomm-edc-0.1.9/intecomm_prn/admin/onschedule_inte_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/admin/protocol_incident_admin.py` & `intecomm-edc-0.1.9/intecomm_prn/admin/protocol_incident_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/admin/subject_transfer_admin.py` & `intecomm-edc-0.1.9/intecomm_prn/admin/subject_transfer_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/choices.py` & `intecomm-edc-0.1.9/intecomm_prn/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/forms/end_of_study_form.py` & `intecomm-edc-0.1.9/intecomm_prn/forms/end_of_study_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/forms/loss_to_followup_form.py` & `intecomm-edc-0.1.9/intecomm_prn/forms/loss_to_followup_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/forms/offschedule_comm_form.py` & `intecomm-edc-0.1.9/intecomm_prn/forms/offschedule_comm_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/forms/offschedule_inte_form.py` & `intecomm-edc-0.1.9/intecomm_prn/forms/offschedule_inte_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/forms/subject_transfer_form.py` & `intecomm-edc-0.1.9/intecomm_prn/forms/subject_transfer_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/list_data.py` & `intecomm-edc-0.1.9/intecomm_prn/list_data.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/migrations/0001_initial.py` & `intecomm-edc-0.1.9/intecomm_prn/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/migrations/0002_remove_endofstudy_delivery_date_and_more.py` & `intecomm-edc-0.1.9/intecomm_prn/migrations/0002_remove_endofstudy_delivery_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/migrations/0003_historicalprotocolincident_reasons_withdrawn_and_more.py` & `intecomm-edc-0.1.9/intecomm_prn/migrations/0003_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/migrations/0004_rename_historicaloffschedulebaseline_historicaloffschedulecomm_and_more.py` & `intecomm-edc-0.1.9/intecomm_prn/migrations/0004_rename_historicaloffschedulebaseline_historicaloffschedulecomm_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/migrations/0005_rename_historicaloffschedulefollowup_historicaloffscheduleinte_and_more.py` & `intecomm-edc-0.1.9/intecomm_prn/migrations/0005_rename_historicaloffschedulefollowup_historicaloffscheduleinte_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/models/end_of_study.py` & `intecomm-edc-0.1.9/intecomm_prn/models/end_of_study.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/models/loss_to_followup.py` & `intecomm-edc-0.1.9/intecomm_prn/models/loss_to_followup.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/models/offschedule_comm.py` & `intecomm-edc-0.1.9/intecomm_prn/models/offschedule_comm.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/models/offschedule_inte.py` & `intecomm-edc-0.1.9/intecomm_prn/models/offschedule_inte.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_prn/models/protocol_incident.py` & `intecomm-edc-0.1.9/intecomm_prn/models/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/__init__.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/health_facility_admin.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/health_facility_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/health_talk_log_admin.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/health_talk_log_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/list_filters.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/list_filters.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/modeladmin_mixins.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/patient_call_admin.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/patient_call_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/patient_call_inlines.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/patient_call_inlines.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/patient_group_admin.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/patient_group_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/patient_log_admin.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/patient_log_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/subject_refusal_admin.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/subject_refusal_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/admin/subject_screening_admin.py` & `intecomm-edc-0.1.9/intecomm_screening/admin/subject_screening_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/apps.py` & `intecomm-edc-0.1.9/intecomm_screening/apps.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/auth_objects.py` & `intecomm-edc-0.1.9/intecomm_screening/auth_objects.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/baker_recipes.py` & `intecomm-edc-0.1.9/intecomm_screening/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/choices.py` & `intecomm-edc-0.1.9/intecomm_screening/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/forms/patient_log_form.py` & `intecomm-edc-0.1.9/intecomm_screening/forms/patient_log_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/forms/subject_refusal_form.py` & `intecomm-edc-0.1.9/intecomm_screening/forms/subject_refusal_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/forms/subject_screening_form.py` & `intecomm-edc-0.1.9/intecomm_screening/forms/subject_screening_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0001_initial.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0002_remove_healthtalklog_unique_lower_name_report_date_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0002_remove_healthtalklog_unique_lower_name_report_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0003_site_remove_historicalpatientlog_patient_group_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0003_site_remove_historicalpatientlog_patient_group_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0004_rename_name_historicalpatientlog_legal_name_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0004_rename_name_historicalpatientlog_legal_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0005_historicalpatientcall_alt_contact_number_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0005_historicalpatientcall_alt_contact_number_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0006_remove_historicalpatientcall_willing_to_attend_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0006_remove_historicalpatientcall_willing_to_attend_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0007_historicalpatientlog_last_4_contact_number_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0007_historicalpatientlog_last_4_contact_number_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0008_rename_last_routine_appt_date_historicalpatientlog_last_appt_date_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0008_rename_last_routine_appt_date_historicalpatientlog_last_appt_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0009_historicalsubjectscreening_familiar_name_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0009_historicalsubjectscreening_familiar_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0010_historicalpatientlog_age_in_years_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0010_historicalpatientlog_age_in_years_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0011_rename_hf_identifier_historicalpatientlog_hospital_identifier_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0011_rename_hf_identifier_historicalpatientlog_hospital_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0012_alter_historicalpatientcall_last_attend_clinic_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0012_alter_historicalpatientcall_last_attend_clinic_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0013_alter_healthfacility_distance_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0013_alter_healthfacility_distance_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0014_alter_historicalpatientlog_familiar_name_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0014_alter_historicalpatientlog_familiar_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0015_remove_healthtalklog_unique_health_facility_report_date_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0015_remove_healthtalklog_unique_health_facility_report_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/migrations/0016_historicalpatientlog_group_identifier_and_more.py` & `intecomm-edc-0.1.9/intecomm_screening/migrations/0016_historicalpatientlog_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/model_mixins/patient_call_model_mixin.py` & `intecomm-edc-0.1.9/intecomm_screening/model_mixins/patient_call_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/models/health_facility.py` & `intecomm-edc-0.1.9/intecomm_screening/models/health_facility.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/models/health_talk_log.py` & `intecomm-edc-0.1.9/intecomm_screening/models/health_talk_log.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/models/patient_call.py` & `intecomm-edc-0.1.9/intecomm_screening/models/patient_call.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/models/patient_log.py` & `intecomm-edc-0.1.9/intecomm_screening/models/patient_log.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/models/signals.py` & `intecomm-edc-0.1.9/intecomm_screening/models/signals.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/models/subject_refusal.py` & `intecomm-edc-0.1.9/intecomm_screening/models/subject_refusal.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/models/subject_screening.py` & `intecomm-edc-0.1.9/intecomm_screening/models/subject_screening.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/healthfacility_change_list.html` & `intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/healthfacility_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/healthtalklog_change_list.html` & `intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/healthtalklog_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/patientcall_change_list.html` & `intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/patientcall_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/patientgroup_change_list.html` & `intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/patientgroup_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/patientlog_change_list.html` & `intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/patientlog_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/admin/subjectscreening_change_list.html` & `intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/admin/subjectscreening_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/change_list_screen_and_consent.html` & `intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/change_list_screen_and_consent.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/templates/intecomm_screening/group_management.html` & `intecomm-edc-0.1.9/intecomm_screening/templates/intecomm_screening/group_management.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/tests/holidays.csv` & `intecomm-edc-0.1.9/intecomm_screening/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/tests/intecomm_test_case_mixin.py` & `intecomm-edc-0.1.9/intecomm_screening/tests/intecomm_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/tests/tests/test_screening.py` & `intecomm-edc-0.1.9/intecomm_screening/tests/tests/test_screening.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/urls.py` & `intecomm-edc-0.1.9/intecomm_screening/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/utils.py` & `intecomm-edc-0.1.9/intecomm_screening/utils.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_screening/views.py` & `intecomm-edc-0.1.9/intecomm_screening/views.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_sites/apps.py` & `intecomm-edc-0.1.9/intecomm_sites/apps.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_sites/intecomm_site.py` & `intecomm-edc-0.1.9/intecomm_sites/intecomm_site.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_sites/sites.py` & `intecomm-edc-0.1.9/intecomm_sites/sites.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/action_items.py` & `intecomm-edc-0.1.9/intecomm_subject/action_items.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/__init__.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_fbc_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_fbc_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_glu_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_glu_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_hba1c_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_hba1c_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_ins_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_ins_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_lft_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_lft_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_lipid_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_lipid_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/blood_results/blood_results_rft_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/blood_results/blood_results_rft_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/cd4_result_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/cd4_result_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/clinical_review_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/clinical_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/clinical_review_baseline_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/clinical_review_baseline_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/complications_baseline_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/complications_baseline_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/complications_followup_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/complications_followup_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/concomitant_medication_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/concomitant_medication_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/dm_initial_review_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/dm_initial_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/dm_review_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/dm_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/drug_refill_dm_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/drug_refill_dm_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/drug_refill_hiv_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/drug_refill_hiv_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/drug_refill_htn_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/drug_refill_htn_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/family_history_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/family_history_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/glucose_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/glucose_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/hba1c_result_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/hba1c_result_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/health_economics_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/health_economics_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/hiv_initial_review_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/hiv_initial_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/hiv_review_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/hiv_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/htn_initial_review_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/htn_initial_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/htn_review_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/htn_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/medications_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/medications_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/modeladmin_mixins.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/other_baseline_data_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/other_baseline_data_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/social_harms_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/social_harms_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/subject_requisition_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/subject_requisition_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/subject_visit_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/subject_visit_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/subject_visit_missed_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/subject_visit_missed_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/urine_dipstick_test_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/urine_dipstick_test_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/urine_pregnancy_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/urine_pregnancy_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/viral_load_result_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/viral_load_result_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/admin/vitals_admin.py` & `intecomm-edc-0.1.9/intecomm_subject/admin/vitals_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/choices.py` & `intecomm-edc-0.1.9/intecomm_subject/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/__init__.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_fbc_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_fbc_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_glu_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_glu_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_hba1c_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_hba1c_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_ins_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_ins_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_lft_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_lft_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_lipid_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_lipid_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/blood_results/blood_results_rft_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/blood_results/blood_results_rft_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/cd4_result_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/cd4_result_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/clinical_review_baseline.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/clinical_review_baseline.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/clinical_review_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/clinical_review_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/drug_supply_hiv_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/drug_supply_hiv_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/subject_requisition_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/subject_requisition_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/subject_visit_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/subject_visit_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/subject_visit_missed_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/subject_visit_missed_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/urine_dipstick_test_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/urine_dipstick_test_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/urine_pregnancy_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/urine_pregnancy_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/forms/viral_load_result_form.py` & `intecomm-edc-0.1.9/intecomm_subject/forms/viral_load_result_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/metadata_rules/metadata_rules.py` & `intecomm-edc-0.1.9/intecomm_subject/metadata_rules/metadata_rules.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/metadata_rules/predicates.py` & `intecomm-edc-0.1.9/intecomm_subject/metadata_rules/predicates.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0001_initial.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0002_remove_historicaldminitialreview_managed_by_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0002_remove_historicaldminitialreview_managed_by_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0003_alter_historicalsocialharms_coworkers_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0003_alter_historicalsocialharms_coworkers_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0004_historicalsocialharms_employment_impact_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0004_historicalsocialharms_employment_impact_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0005_alter_historicalsocialharms_coworkers_impact_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0005_alter_historicalsocialharms_coworkers_impact_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0006_alter_healtheconomics_options_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0006_alter_healtheconomics_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0007_alter_historicalotherbaselinedata_alcohol_consumption_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0007_alter_historicalotherbaselinedata_alcohol_consumption_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0008_historicalvitals_vitals_remove_indicators_site_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0008_historicalvitals_vitals_remove_indicators_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0009_remove_historicalvitals_bp_measured_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0009_remove_historicalvitals_bp_measured_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0010_remove_historicalvitals_weight_is_estmated_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0010_remove_historicalvitals_weight_is_estmated_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0011_remove_clinicalreviewbaseline_complications_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0011_remove_clinicalreviewbaseline_complications_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/migrations/0012_alter_historicalvitals_heart_rate_and_more.py` & `intecomm-edc-0.1.9/intecomm_subject/migrations/0012_alter_historicalvitals_heart_rate_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/model_mixins/clinical_review_model_mixins.py` & `intecomm-edc-0.1.9/intecomm_subject/model_mixins/clinical_review_model_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/model_mixins/followup_review_model_mixin.py` & `intecomm-edc-0.1.9/intecomm_subject/model_mixins/followup_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/__init__.py` & `intecomm-edc-0.1.9/intecomm_subject/models/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_fbc.py` & `intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_fbc.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_glu.py` & `intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_glu.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_hba1c.py` & `intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_hba1c.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_ins.py` & `intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_ins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_lft.py` & `intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_lft.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_lipid.py` & `intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_lipid.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/blood_results/blood_results_rft.py` & `intecomm-edc-0.1.9/intecomm_subject/models/blood_results/blood_results_rft.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/cd4_result.py` & `intecomm-edc-0.1.9/intecomm_subject/models/cd4_result.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/clinical_review.py` & `intecomm-edc-0.1.9/intecomm_subject/models/clinical_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/clinical_review_baseline.py` & `intecomm-edc-0.1.9/intecomm_subject/models/clinical_review_baseline.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/complications_baseline.py` & `intecomm-edc-0.1.9/intecomm_subject/models/complications_baseline.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/complications_followup.py` & `intecomm-edc-0.1.9/intecomm_subject/models/complications_followup.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/dm_initial_review.py` & `intecomm-edc-0.1.9/intecomm_subject/models/dm_initial_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/drug_refill_dm.py` & `intecomm-edc-0.1.9/intecomm_subject/models/drug_refill_dm.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/drug_refill_hiv.py` & `intecomm-edc-0.1.9/intecomm_subject/models/drug_refill_hiv.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/drug_refill_htn.py` & `intecomm-edc-0.1.9/intecomm_subject/models/drug_refill_htn.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/drug_supply_dm.py` & `intecomm-edc-0.1.9/intecomm_subject/models/drug_supply_dm.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/drug_supply_hiv.py` & `intecomm-edc-0.1.9/intecomm_subject/models/drug_supply_hiv.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/drug_supply_htn.py` & `intecomm-edc-0.1.9/intecomm_subject/models/drug_supply_htn.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/family_history.py` & `intecomm-edc-0.1.9/intecomm_subject/models/family_history.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/hba1c_result.py` & `intecomm-edc-0.1.9/intecomm_subject/models/hba1c_result.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/health_economics.py` & `intecomm-edc-0.1.9/intecomm_subject/models/health_economics.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/hiv_initial_review.py` & `intecomm-edc-0.1.9/intecomm_subject/models/hiv_initial_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/hiv_review.py` & `intecomm-edc-0.1.9/intecomm_subject/models/hiv_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/htn_initial_review.py` & `intecomm-edc-0.1.9/intecomm_subject/models/htn_initial_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/htn_review.py` & `intecomm-edc-0.1.9/intecomm_subject/models/htn_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/investigations.py` & `intecomm-edc-0.1.9/intecomm_subject/models/investigations.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/medications.py` & `intecomm-edc-0.1.9/intecomm_subject/models/medications.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/other_baseline_data.py` & `intecomm-edc-0.1.9/intecomm_subject/models/other_baseline_data.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/patient_history.py` & `intecomm-edc-0.1.9/intecomm_subject/models/patient_history.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/reason_for_visit.py` & `intecomm-edc-0.1.9/intecomm_subject/models/reason_for_visit.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/social_harms/model_factories.py` & `intecomm-edc-0.1.9/intecomm_subject/models/social_harms/model_factories.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/social_harms/social_harms.py` & `intecomm-edc-0.1.9/intecomm_subject/models/social_harms/social_harms.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/subject_visit.py` & `intecomm-edc-0.1.9/intecomm_subject/models/subject_visit.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/subject_visit_missed.py` & `intecomm-edc-0.1.9/intecomm_subject/models/subject_visit_missed.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/urine_dipstick_test.py` & `intecomm-edc-0.1.9/intecomm_subject/models/urine_dipstick_test.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/urine_pregnancy.py` & `intecomm-edc-0.1.9/intecomm_subject/models/urine_pregnancy.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/viral_load_result.py` & `intecomm-edc-0.1.9/intecomm_subject/models/viral_load_result.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_subject/models/vitals.py` & `intecomm-edc-0.1.9/intecomm_subject/models/vitals.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/comm_schedule.py` & `intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/comm_schedule.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/crfs.py` & `intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/crfs.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/requisitions.py` & `intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/requisitions.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/visit_schedule.py` & `intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/intecomm_visit_schedule/visit_schedules/visits.py` & `intecomm-edc-0.1.9/intecomm_visit_schedule/visit_schedules/visits.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/manage.py` & `intecomm-edc-0.1.9/manage.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/pyproject.toml` & `intecomm-edc-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/runtests.py` & `intecomm-edc-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.1.8/setup.cfg` & `intecomm-edc-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 
 [options]
 python_requires = >=3.10
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	edc==0.4.63
+	edc==0.4.64
 	beautifulsoup4
 	canned-views
 	edc-microscopy==0.1.0
 	edc-rx==0.1.1
 	intecomm-eligibility==0.1.3
-	intecomm-form-validators==0.1.9
+	intecomm-form-validators==0.1.10
 	intecomm-rando==0.1.4
 
 [options.packages.find]
 exclude = 
 	examples*
 	tools*
 	docs*
```

