# Comparing `tmp/djangosaml2-1.5.6.tar.gz` & `tmp/djangosaml2-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangosaml2-1.5.6.tar", last modified: Wed Apr  5 16:38:22 2023, max compression
+gzip compressed data, was "djangosaml2-1.5.7.tar", last modified: Sun May  7 19:41:51 2023, max compression
```

## Comparing `djangosaml2-1.5.6.tar` & `djangosaml2-1.5.7.tar`

### file list

```diff
@@ -1,1576 +1,1580 @@
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.377415 djangosaml2-1.5.6/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:01.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.273415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.273415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.273415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.273415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.277415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.281415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.281415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.281415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:02.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.281415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.285415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:04.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.285415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:32:55.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.289415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:01.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.289415 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:32:55.000000 djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django3.0/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.261415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.289415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:10.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.289415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.293415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.297415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.297415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.297415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:12.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.301415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.301415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:13.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.301415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:06.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.301415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:11.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.301415 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:06.000000 djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.301415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:20.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.305415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.305415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.305415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.305415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.305415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.309415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.309415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.309415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.309415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.309415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.309415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.309415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.309415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.313415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.313415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.313415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:21.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.317415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.317415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:23.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.317415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:16.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.317415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:20.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.317415 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:16.000000 djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.317415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.321415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.321415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.321415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.321415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.321415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.321415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.325415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.325415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.325415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.325415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.325415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.325415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.325415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.325415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.329415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.329415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:31.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.329415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.329415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:33.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.329415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:25.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.333415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:30.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.333415 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:25.000000 djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.333415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:39.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.333415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.333415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.333415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.333415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.337415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.341415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.341415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.341415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:40.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.265416 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.345415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.345415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:42.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.345415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:35.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.345415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:39.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.345415 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:35.000000 djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.345415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.349415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.349415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.349415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.349415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.349415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.349415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.349415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.349415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.353415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.353415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.353415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.353415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.353415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.353415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.357415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.357415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:50.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.357415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.361415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:52.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.361415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:44.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.361415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:49.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.361415 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:44.000000 djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.1/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.361415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:58.000000 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.365415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:54.000000 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.365415 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:54.000000 djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    13512 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/CHANGES
--rw-rw-r--   0 wert      (1000) wert      (1000)    11358 2021-01-23 23:44:15.000000 djangosaml2-1.5.6/COPYING
--rw-rw-r--   0 wert      (1000) wert      (1000)      164 2021-01-23 23:44:15.000000 djangosaml2-1.5.6/MANIFEST.in
--rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-04-05 16:38:22.377415 djangosaml2-1.5.6/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)     1681 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/README.md
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.365415 djangosaml2-1.5.6/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      190 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/apps.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    14380 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/backends.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2894 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/cache.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2568 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/conf.py
--rw-rw-r--   0 wert      (1000) wert      (1000)       51 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/exceptions.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     3511 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/middleware.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1045 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/overrides.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      726 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/signals.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.365415 djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.365415 djangosaml2-1.5.6/djangosaml2/templatetags/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/templatetags/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/templatetags/idplist.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.365415 djangosaml2-1.5.6/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)    42515 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/__init__.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.365415 djangosaml2-1.5.6/djangosaml2/tests/attribute-maps/
--rw-rw-r--   0 wert      (1000) wert      (1000)      555 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/attribute-maps/django_saml_uri.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    11106 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/attribute-maps/saml_uri.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     5095 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/auth_response.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     4177 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/conf.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13780 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3565 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3557 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10380 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2466 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/spcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-16 13:28:16.000000 djangosaml2-1.5.6/djangosaml2/tests/utils.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1190 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/urls.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     6333 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/utils.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    33169 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/djangosaml2/views.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.365415 djangosaml2-1.5.6/djangosaml2.egg-info/
--rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-04-05 16:38:21.000000 djangosaml2-1.5.6/djangosaml2.egg-info/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)   110649 2023-04-05 16:38:22.000000 djangosaml2-1.5.6/djangosaml2.egg-info/SOURCES.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-04-05 16:38:21.000000 djangosaml2-1.5.6/djangosaml2.egg-info/dependency_links.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-04-05 16:38:21.000000 djangosaml2-1.5.6/djangosaml2.egg-info/not-zip-safe
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:38:21.000000 djangosaml2-1.5.6/djangosaml2.egg-info/requires.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)       12 2023-04-05 16:38:21.000000 djangosaml2-1.5.6/djangosaml2.egg-info/top_level.txt
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/docs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/docs/build/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/docs/build/html/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/docs/build/html/contents/
--rw-rw-r--   0 wert      (1000) wert      (1000)    12974 2021-04-04 23:22:05.000000 djangosaml2-1.5.6/docs/build/html/contents/developer.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     7950 2021-04-04 23:22:05.000000 djangosaml2-1.5.6/docs/build/html/contents/faq.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    15144 2021-04-04 23:22:05.000000 djangosaml2-1.5.6/docs/build/html/contents/miscellanea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    54956 2021-04-05 09:22:50.000000 djangosaml2-1.5.6/docs/build/html/contents/setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     8497 2021-04-05 09:22:28.000000 djangosaml2-1.5.6/docs/build/html/contents/usage.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6153 2021-04-05 09:22:50.000000 djangosaml2-1.5.6/docs/build/html/genindex.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    11611 2021-04-05 09:22:50.000000 djangosaml2-1.5.6/docs/build/html/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6624 2021-04-05 09:22:50.000000 djangosaml2-1.5.6/docs/build/html/search.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/docs/source/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/docs/source/_templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/docs/source/_templates/pplnx_template/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1829 2021-04-04 22:43:59.000000 djangosaml2-1.5.6/docs/source/_templates/pplnx_template/footer.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1486 2021-04-04 22:43:59.000000 djangosaml2-1.5.6/docs/source/_templates/pplnx_template/layout.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   286370 2022-12-06 06:43:27.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1235 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1716 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2515 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6110 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      448 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3019 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3290 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1502 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      697 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/color_theme_toggle.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      453 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2539 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2241 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2580 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4086 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2200 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1849 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1899 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      486 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2136 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1257 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1093 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.369415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      339 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2096 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      745 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2428 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1366 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      869 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      196 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1587 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      360 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      865 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/div.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/
--rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/
--rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      119 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/div.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       88 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       85 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/ul.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      147 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/label.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      673 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      814 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      712 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      874 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/div.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      118 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/div.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       82 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       83 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/ul.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      122 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/label.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      684 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      825 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      723 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      426 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.373415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11184 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17662 2023-04-05 16:18:17.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.377415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/docutils-0.19.dist-info/
--rw-rw-r--   0 wert      (1000) wert      (1000)    26094 2022-12-06 06:43:27.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/docutils-0.19.dist-info/SOURCES.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2022-12-06 06:43:27.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/docutils-0.19.dist-info/dependency_links.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      969 2022-12-06 06:43:27.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/docutils-0.19.dist-info/top_level.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/jeepney/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.377415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/jeepney/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     4575 2022-12-06 06:43:27.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.377415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   286370 2022-12-06 06:43:14.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.377415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2023-04-05 16:18:18.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.269415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-04-05 16:38:22.377415 djangosaml2-1.5.6/env/lib/python3.10/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2022-12-06 06:43:14.000000 djangosaml2-1.5.6/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      439 2023-04-05 16:19:28.000000 djangosaml2-1.5.6/pyproject.toml
--rw-rw-r--   0 wert      (1000) wert      (1000)      197 2023-04-05 16:38:22.377415 djangosaml2-1.5.6/setup.cfg
--rw-rw-r--   0 wert      (1000) wert      (1000)     2436 2023-04-05 16:21:35.000000 djangosaml2-1.5.6/setup.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.254062 djangosaml2-1.5.7/.tox/py3.6-django2.2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.254062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.254062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:01.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.254062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:32:55.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:01.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:32:55.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:10.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:06.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:06.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:20.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:16.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:20.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:16.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:25.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:25.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:39.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:35.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:39.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:35.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:44.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:44.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:58.000000 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:54.000000 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:54.000000 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13512 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/CHANGES
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11358 2021-01-23 23:44:15.000000 djangosaml2-1.5.7/COPYING
+-rw-rw-r--   0 wert      (1000) wert      (1000)      164 2021-01-23 23:44:15.000000 djangosaml2-1.5.7/MANIFEST.in
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/PKG-INFO
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1681 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/README.md
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/__init__.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)      190 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/apps.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    14380 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/backends.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2894 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/cache.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2568 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/conf.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)       51 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/exceptions.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3511 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/middleware.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1045 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/overrides.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)      726 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/signals.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/djangosaml2/templatetags/
+-rw-rw-r--   0 wert      (1000) wert      (1000)        0 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templatetags/__init__.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/templatetags/idplist.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    42515 2023-05-07 19:41:25.000000 djangosaml2-1.5.7/djangosaml2/tests/__init__.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      555 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/django_saml_uri.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11106 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/saml_uri.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     5095 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/auth_response.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4177 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/conf.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13780 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3565 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3557 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10380 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2466 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/spcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/utils.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1190 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/urls.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6333 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/utils.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    33757 2023-05-07 19:41:25.000000 djangosaml2-1.5.7/djangosaml2/views.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/djangosaml2.egg-info/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/PKG-INFO
+-rw-rw-r--   0 wert      (1000) wert      (1000)   110776 2023-05-07 19:41:51.000000 djangosaml2-1.5.7/djangosaml2.egg-info/SOURCES.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/dependency_links.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/not-zip-safe
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/requires.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)       12 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/top_level.txt
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/docs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/docs/build/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/docs/build/html/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/docs/build/html/contents/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    12974 2021-04-04 23:22:05.000000 djangosaml2-1.5.7/docs/build/html/contents/developer.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     7950 2021-04-04 23:22:05.000000 djangosaml2-1.5.7/docs/build/html/contents/faq.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    15144 2021-04-04 23:22:05.000000 djangosaml2-1.5.7/docs/build/html/contents/miscellanea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    54956 2021-04-05 09:22:50.000000 djangosaml2-1.5.7/docs/build/html/contents/setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     8497 2021-04-05 09:22:28.000000 djangosaml2-1.5.7/docs/build/html/contents/usage.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6153 2021-04-05 09:22:50.000000 djangosaml2-1.5.7/docs/build/html/genindex.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11611 2021-04-05 09:22:50.000000 djangosaml2-1.5.7/docs/build/html/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6624 2021-04-05 09:22:50.000000 djangosaml2-1.5.7/docs/build/html/search.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/docs/source/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/docs/source/_templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/docs/source/_templates/pplnx_template/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1829 2021-04-04 22:43:59.000000 djangosaml2-1.5.7/docs/source/_templates/pplnx_template/footer.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1486 2021-04-04 22:43:59.000000 djangosaml2-1.5.7/docs/source/_templates/pplnx_template/layout.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/coverage/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/coverage/htmlfiles/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     5400 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/coverage/htmlfiles/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6434 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/coverage/htmlfiles/pyfile.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      282 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      551 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/500.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1235 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/actions.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      389 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1716 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_list.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      320 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2515 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6110 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      448 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base_site.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3019 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      403 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3290 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1502 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_results.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      697 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/color_theme_toggle.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      453 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2539 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2241 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2580 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4086 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/filter.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2200 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      192 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1849 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      447 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1899 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/login.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      486 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2136 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/object_history.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      549 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/pagination.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      327 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/popup_response.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      209 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1257 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/search_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1093 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/submit_line.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      618 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      339 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2096 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      238 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      218 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      425 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/logged_out.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      745 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2428 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1366 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      588 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      612 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      869 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      786 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      928 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      196 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      111 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1587 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      683 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      360 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      865 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/div.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      119 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/div.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/p.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       88 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/table.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       85 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/ul.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      147 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/label.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      673 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/p.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      814 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/table.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      712 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      365 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      110 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      874 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/div.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      118 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/default.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/div.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       82 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/p.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/table.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       83 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/ul.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      122 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/label.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      684 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/p.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      825 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/table.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      723 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/ul.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/attrs.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/datetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/email.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/file.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      189 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      426 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      117 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/number.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/password.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      384 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_date.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      127 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_option.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/text.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/textarea.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/time.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/url.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11184 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/default_urlconf.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/technical_404.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)    17662 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/technical_500.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    26094 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/SOURCES.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/dependency_links.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      969 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/top_level.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/jeepney/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/jeepney/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4575 2023-05-07 19:41:47.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-01 09:54:29.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/data/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/data/templates/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      769 2023-05-01 09:55:04.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/data/templates/template_enc.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2023-05-01 09:54:28.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      439 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/pyproject.toml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      197 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/setup.cfg
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2436 2023-05-07 19:41:25.000000 djangosaml2-1.5.7/setup.py
```

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/default_urlconf.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/default_urlconf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_404.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_404.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_500.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_404.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_404.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_500.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/CHANGES` & `djangosaml2-1.5.7/CHANGES`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/COPYING` & `djangosaml2-1.5.7/COPYING`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/PKG-INFO` & `djangosaml2-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.5.6
+Version: 1.5.7
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.5.6/README.md` & `djangosaml2-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/backends.py` & `djangosaml2-1.5.7/djangosaml2/backends.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/cache.py` & `djangosaml2-1.5.7/djangosaml2/cache.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/conf.py` & `djangosaml2-1.5.7/djangosaml2/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/middleware.py` & `djangosaml2-1.5.7/djangosaml2/middleware.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/overrides.py` & `djangosaml2-1.5.7/djangosaml2/overrides.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/signals.py` & `djangosaml2-1.5.7/djangosaml2/signals.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/templatetags/idplist.py` & `djangosaml2-1.5.7/djangosaml2/templatetags/idplist.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/__init__.py` & `djangosaml2-1.5.7/djangosaml2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/attribute-maps/django_saml_uri.py` & `djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/django_saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/attribute-maps/saml_uri.py` & `djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/auth_response.py` & `djangosaml2-1.5.7/djangosaml2/tests/auth_response.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/conf.py` & `djangosaml2-1.5.7/djangosaml2/tests/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.5.7/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/idpcert.key` & `djangosaml2-1.5.7/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.5.7/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/mycert.csr` & `djangosaml2-1.5.7/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/mycert.key` & `djangosaml2-1.5.7/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/mycert.pem` & `djangosaml2-1.5.7/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.7/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.7/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/spcert.csr` & `djangosaml2-1.5.7/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/spcert.key` & `djangosaml2-1.5.7/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/tests/spcert.pem` & `djangosaml2-1.5.7/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/urls.py` & `djangosaml2-1.5.7/djangosaml2/urls.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/utils.py` & `djangosaml2-1.5.7/djangosaml2/utils.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/djangosaml2/views.py` & `djangosaml2-1.5.7/djangosaml2/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,47 +546,70 @@
                 break
 
         if callable(attribute_mapping):
             attribute_mapping = attribute_mapping()
         if callable(create_unknown_user):
             create_unknown_user = create_unknown_user()
 
+        try:
+            user = self.authenticate_user(
+                request,
+                session_info,
+                attribute_mapping,
+                create_unknown_user,
+                assertion_info
+            )
+        except PermissionDenied as e:
+            return self.handle_acs_failure(
+                request,
+                exception=e,
+                session_info=session_info,
+            )
+
+        relay_state = self.build_relay_state()
+        custom_redirect_url = self.custom_redirect(user, relay_state, session_info)
+        if custom_redirect_url:
+            return HttpResponseRedirect(custom_redirect_url)
+        relay_state = validate_referral_url(request, relay_state)
+        logger.debug("Redirecting to the RelayState: %s", relay_state)
+        return HttpResponseRedirect(relay_state)
+
+    def authenticate_user(
+            self,
+            request,
+            session_info,
+            attribute_mapping,
+            create_unknown_user,
+            assertion_info
+        ):
+        """Calls Django's authenticate method after the SAML response is verified"""
         logger.debug("Trying to authenticate the user. Session info: %s", session_info)
+
         user = auth.authenticate(
             request=request,
             session_info=session_info,
             attribute_mapping=attribute_mapping,
             create_unknown_user=create_unknown_user,
             assertion_info=assertion_info,
         )
         if user is None:
             logger.warning(
                 "Could not authenticate user received in SAML Assertion. Session info: %s",
                 session_info,
             )
-            return self.handle_acs_failure(
-                request,
-                exception=PermissionDenied("No user could be authenticated."),
-                session_info=session_info,
-            )
+            raise PermissionDenied("No user could be authenticated.")
 
         auth.login(self.request, user)
         _set_subject_id(request.saml_session, session_info["name_id"])
         logger.debug("User %s authenticated via SSO.", user)
 
         self.post_login_hook(request, user, session_info)
         self.customize_session(user, session_info)
 
-        relay_state = self.build_relay_state()
-        custom_redirect_url = self.custom_redirect(user, relay_state, session_info)
-        if custom_redirect_url:
-            return HttpResponseRedirect(custom_redirect_url)
-        relay_state = validate_referral_url(request, relay_state)
-        logger.debug("Redirecting to the RelayState: %s", relay_state)
-        return HttpResponseRedirect(relay_state)
+        return user
 
     def post_login_hook(
         self, request: HttpRequest, user: settings.AUTH_USER_MODEL, session_info: dict
     ) -> None:
         """If desired, a hook to add logic after a user has succesfully logged in."""
 
     def build_relay_state(self) -> str:
```

### Comparing `djangosaml2-1.5.6/djangosaml2.egg-info/PKG-INFO` & `djangosaml2-1.5.7/djangosaml2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.5.6
+Version: 1.5.7
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.5.6/djangosaml2.egg-info/SOURCES.txt` & `djangosaml2-1.5.7/djangosaml2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -958,14 +958,16 @@
 docs/build/html/contents/faq.html
 docs/build/html/contents/miscellanea.html
 docs/build/html/contents/setup.html
 docs/build/html/contents/usage.html
 docs/source/_templates/pplnx_template/footer.html
 docs/source/_templates/pplnx_template/layout.html
 env/lib/python3.10/site-packages/certifi/cacert.pem
+env/lib/python3.10/site-packages/coverage/htmlfiles/index.html
+env/lib/python3.10/site-packages/coverage/htmlfiles/pyfile.html
 env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/404.html
 env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/500.html
 env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/actions.html
 env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_index.html
 env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_list.html
 env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base.html
 env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base_site.html
```

### Comparing `djangosaml2-1.5.6/docs/build/html/contents/developer.html` & `djangosaml2-1.5.7/docs/build/html/contents/developer.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/build/html/contents/faq.html` & `djangosaml2-1.5.7/docs/build/html/contents/faq.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/build/html/contents/miscellanea.html` & `djangosaml2-1.5.7/docs/build/html/contents/miscellanea.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/build/html/contents/setup.html` & `djangosaml2-1.5.7/docs/build/html/contents/setup.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/build/html/contents/usage.html` & `djangosaml2-1.5.7/docs/build/html/contents/usage.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/build/html/genindex.html` & `djangosaml2-1.5.7/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/build/html/index.html` & `djangosaml2-1.5.7/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/build/html/search.html` & `djangosaml2-1.5.7/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/source/_templates/pplnx_template/footer.html` & `djangosaml2-1.5.7/docs/source/_templates/pplnx_template/footer.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/docs/source/_templates/pplnx_template/layout.html` & `djangosaml2-1.5.7/docs/source/_templates/pplnx_template/layout.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/certifi/cacert.pem`

 * *Files 2% similar despite different names*

```diff
@@ -632,45 +632,14 @@
 IC9Bi5HcSEW88cbeunZrM8gALTFGTO3nnc+IlP8zwFboJIYmuNg4ON8qa90SzMc/
 RxdMosIGlgnW2/4/PEZB31jiVg88O8EckzXZOFKs7sjsLjBOlDW0JB9LeGna8gI4
 zJVSk/BwJVmcIGfE7vmLV2H0knZ9P4SNVbfo5azV8fUZVqZa+5Acr5Pr5RzUZ5dd
 BA6+C4OmF4O5MBKgxTMVBbkN+8cFduPYSo38NBejxiEovjBFMR7HeL5YYTisO+IB
 ZQ==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Subject: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Label: "Network Solutions Certificate Authority"
-# Serial: 116697915152937497490437556386812487904
-# MD5 Fingerprint: d3:f3:a6:16:c0:fa:6b:1d:59:b1:2d:96:4d:0e:11:2e
-# SHA1 Fingerprint: 74:f8:a3:c3:ef:e7:b3:90:06:4b:83:90:3c:21:64:60:20:e5:df:ce
-# SHA256 Fingerprint: 15:f0:ba:00:a3:ac:7a:f3:ac:88:4c:07:2b:10:11:a0:77:bd:77:c0:97:f4:01:64:b2:f8:59:8a:bd:83:86:0c
------BEGIN CERTIFICATE-----
-MIID5jCCAs6gAwIBAgIQV8szb8JcFuZHFhfjkDFo4DANBgkqhkiG9w0BAQUFADBi
-MQswCQYDVQQGEwJVUzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMu
-MTAwLgYDVQQDEydOZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3Jp
-dHkwHhcNMDYxMjAxMDAwMDAwWhcNMjkxMjMxMjM1OTU5WjBiMQswCQYDVQQGEwJV
-UzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMuMTAwLgYDVQQDEydO
-ZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkwggEiMA0GCSqG
-SIb3DQEBAQUAA4IBDwAwggEKAoIBAQDkvH6SMG3G2I4rC7xGzuAnlt7e+foS0zwz
-c7MEL7xxjOWftiJgPl9dzgn/ggwbmlFQGiaJ3dVhXRncEg8tCqJDXRfQNJIg6nPP
-OCwGJgl6cvf6UDL4wpPTaaIjzkGxzOTVHzbRijr4jGPiFFlp7Q3Tf2vouAPlT2rl
-mGNpSAW+Lv8ztumXWWn4Zxmuk2GWRBXTcrA/vGp97Eh/jcOrqnErU2lBUzS1sLnF
-BgrEsEX1QV1uiUV7PTsmjHTC5dLRfbIR1PtYMiKagMnc/Qzpf14Dl847ABSHJ3A4
-qY5usyd2mFHgBeMhqxrVhSI8KbWaFsWAqPS7azCPL0YCorEMIuDTAgMBAAGjgZcw
-gZQwHQYDVR0OBBYEFCEwyfsA106Y2oeqKtCnLrFAMadMMA4GA1UdDwEB/wQEAwIB
-BjAPBgNVHRMBAf8EBTADAQH/MFIGA1UdHwRLMEkwR6BFoEOGQWh0dHA6Ly9jcmwu
-bmV0c29sc3NsLmNvbS9OZXR3b3JrU29sdXRpb25zQ2VydGlmaWNhdGVBdXRob3Jp
-dHkuY3JsMA0GCSqGSIb3DQEBBQUAA4IBAQC7rkvnt1frf6ott3NHhWrB5KUd5Oc8
-6fRZZXe1eltajSU24HqXLjjAV2CDmAaDn7l2em5Q4LqILPxFzBiwmZVRDuwduIj/
-h1AcgsLj4DKAv6ALR8jDMe+ZZzKATxcheQxpXN5eNK4CtSbqUN9/GGUsyfJj4akH
-/nxxH2szJGoeBfcFaMBqEssuXmHLrijTfsK0ZpEmXzwuJF/LWA/rKOyvEZbz3Htv
-wKeI8lN3s2Berq4o2jUsbzRF0ybh3uxbTydrFny9RAQYgrOJeRcQcT16ohZO9QHN
-pGxlaKFJdlxDydi8NmdspZS11My5vWo1ViHe2MPr+8ukYEywVaCge1ey
------END CERTIFICATE-----
-
 # Issuer: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Subject: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Label: "COMODO ECC Certification Authority"
 # Serial: 41578283867086692638256921589707938090
 # MD5 Fingerprint: 7c:62:ff:74:9d:31:53:5e:68:4a:d5:78:aa:1e:bf:23
 # SHA1 Fingerprint: 9f:74:4e:9f:2b:4d:ba:ec:0f:31:2c:50:b6:56:3b:8e:2d:93:c3:11
 # SHA256 Fingerprint: 17:93:92:7a:06:14:54:97:89:ad:ce:2f:8f:34:f7:f0:b6:6d:0f:3a:e3:a3:b8:4d:21:ec:15:db:ba:4f:ad:c7
@@ -2200,54 +2169,14 @@
 hOvRnkmSh5SHDDqFSmafnVmTTZdhBoZKo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYD
 VR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUPeYpSJvqB8ohREom3m7e0oPQn1kwCgYI
 KoZIzj0EAwMDaAAwZQIxAOVpEslu28YxuglB4Zf4+/2a4n0Sye18ZNPLBSWLVtmg
 515dTguDnFt2KaAJJiFqYgIwcdK1j1zqO+F4CYWodZI7yFz9SO8NdCKoCOJuxUnO
 xwy8p2Fp8fc74SrL+SvzZpA3
 -----END CERTIFICATE-----
 
-# Issuer: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Subject: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Label: "Staat der Nederlanden EV Root CA"
-# Serial: 10000013
-# MD5 Fingerprint: fc:06:af:7b:e8:1a:f1:9a:b4:e8:d2:70:1f:c0:f5:ba
-# SHA1 Fingerprint: 76:e2:7e:c1:4f:db:82:c1:c0:a6:75:b5:05:be:3d:29:b4:ed:db:bb
-# SHA256 Fingerprint: 4d:24:91:41:4c:fe:95:67:46:ec:4c:ef:a6:cf:6f:72:e2:8a:13:29:43:2f:9d:8a:90:7a:c4:cb:5d:ad:c1:5a
------BEGIN CERTIFICATE-----
-MIIFcDCCA1igAwIBAgIEAJiWjTANBgkqhkiG9w0BAQsFADBYMQswCQYDVQQGEwJO
-TDEeMBwGA1UECgwVU3RhYXQgZGVyIE5lZGVybGFuZGVuMSkwJwYDVQQDDCBTdGFh
-dCBkZXIgTmVkZXJsYW5kZW4gRVYgUm9vdCBDQTAeFw0xMDEyMDgxMTE5MjlaFw0y
-MjEyMDgxMTEwMjhaMFgxCzAJBgNVBAYTAk5MMR4wHAYDVQQKDBVTdGFhdCBkZXIg
-TmVkZXJsYW5kZW4xKTAnBgNVBAMMIFN0YWF0IGRlciBOZWRlcmxhbmRlbiBFViBS
-b290IENBMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA48d+ifkkSzrS
-M4M1LGns3Amk41GoJSt5uAg94JG6hIXGhaTK5skuU6TJJB79VWZxXSzFYGgEt9nC
-UiY4iKTWO0Cmws0/zZiTs1QUWJZV1VD+hq2kY39ch/aO5ieSZxeSAgMs3NZmdO3d
-Z//BYY1jTw+bbRcwJu+r0h8QoPnFfxZpgQNH7R5ojXKhTbImxrpsX23Wr9GxE46p
-rfNeaXUmGD5BKyF/7otdBwadQ8QpCiv8Kj6GyzyDOvnJDdrFmeK8eEEzduG/L13l
-pJhQDBXd4Pqcfzho0LKmeqfRMb1+ilgnQ7O6M5HTp5gVXJrm0w912fxBmJc+qiXb
-j5IusHsMX/FjqTf5m3VpTCgmJdrV8hJwRVXj33NeN/UhbJCONVrJ0yPr08C+eKxC
-KFhmpUZtcALXEPlLVPxdhkqHz3/KRawRWrUgUY0viEeXOcDPusBCAUCZSCELa6fS
-/ZbV0b5GnUngC6agIk440ME8MLxwjyx1zNDFjFE7PZQIZCZhfbnDZY8UnCHQqv0X
-cgOPvZuM5l5Tnrmd74K74bzickFbIZTTRTeU0d8JOV3nI6qaHcptqAqGhYqCvkIH
-1vI4gnPah1vlPNOePqc7nvQDs/nxfRN0Av+7oeX6AHkcpmZBiFxgV6YuCcS6/ZrP
-px9Aw7vMWgpVSzs4dlG4Y4uElBbmVvMCAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB
-/zAOBgNVHQ8BAf8EBAMCAQYwHQYDVR0OBBYEFP6rAJCYniT8qcwaivsnuL8wbqg7
-MA0GCSqGSIb3DQEBCwUAA4ICAQDPdyxuVr5Os7aEAJSrR8kN0nbHhp8dB9O2tLsI
-eK9p0gtJ3jPFrK3CiAJ9Brc1AsFgyb/E6JTe1NOpEyVa/m6irn0F3H3zbPB+po3u
-2dfOWBfoqSmuc0iH55vKbimhZF8ZE/euBhD/UcabTVUlT5OZEAFTdfETzsemQUHS
-v4ilf0X8rLiltTMMgsT7B/Zq5SWEXwbKwYY5EdtYzXc7LMJMD16a4/CrPmEbUCTC
-wPTxGfARKbalGAKb12NMcIxHowNDXLldRqANb/9Zjr7dn3LDWyvfjFvO5QxGbJKy
-CqNMVEIYFRIYvdr8unRu/8G2oGTYqV9Vrp9canaW2HNnh/tNf1zuacpzEPuKqf2e
-vTY4SUmH9A4U8OmHuD+nT3pajnnUk+S7aFKErGzp85hwVXIy+TSrK0m1zSBi5Dp6
-Z2Orltxtrpfs/J92VoguZs9btsmksNcFuuEnL5O7Jiqik7Ab846+HUCjuTaPPoIa
-Gl6I6lD4WeKDRikL40Rc4ZW2aZCaFG+XroHPaO+Zmr615+F/+PoTRxZMzG0IQOeL
-eG9QgkRQP2YGiqtDhFZKDyAthg710tvSeopLzaXoTvFeJiUBWSOgftL2fiFX1ye8
-FVdMpEbB4IMeDExNH08GGeL5qPQ6gqGyeUN51q1veieQA6TqJIc/2b3Z6fJfUEkc
-7uzXLg==
------END CERTIFICATE-----
-
 # Issuer: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Subject: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Label: "IdenTrust Commercial Root CA 1"
 # Serial: 13298821034946342390520003877796839426
 # MD5 Fingerprint: b3:3e:77:73:75:ee:a0:d3:e3:7e:49:63:49:59:bb:c7
 # SHA1 Fingerprint: df:71:7e:aa:4a:d9:4e:c9:55:84:99:60:2d:48:de:5f:bc:f0:3a:25
 # SHA256 Fingerprint: 5d:56:49:9b:e4:d2:e0:8b:cf:ca:d0:8a:3e:38:72:3d:50:50:3b:de:70:69:48:e4:2f:55:60:30:19:e5:28:ae
@@ -2847,124 +2776,14 @@
 2c9Si1vIY9RCPqAzekYu9wogRlR+ak8x8YF+QnQ4ZXMn7sZ8uI7XpTrXmKGcjBBV
 09tL7ECQ8s1uV9JiDnxXk7Gnbc2dg7sq5+W2O3FYrf3RRbxake5TFW/TRQl1brqQ
 XR4EzzffHqhmsYzmIGrv/EhOdJhCrylvLmrH+33RZjEizIYAfmaDDEL0vTSSwxrq
 T8p+ck0LcIymSLumoRT2+1hEmRSuqguTaaApJUqlyyvdimYHFngVV3Eb7PVHhPOe
 MTd61X8kreS8/f3MboPoDKi3QWwH3b08hpcv0g==
 -----END CERTIFICATE-----
 
-# Issuer: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-1"
-# Serial: 15752444095811006489
-# MD5 Fingerprint: 6e:85:f1:dc:1a:00:d3:22:d5:b2:b2:ac:6b:37:05:45
-# SHA1 Fingerprint: ff:bd:cd:e7:82:c8:43:5e:3c:6f:26:86:5c:ca:a8:3a:45:5b:c3:0a
-# SHA256 Fingerprint: d4:0e:9c:86:cd:8f:e4:68:c1:77:69:59:f4:9e:a7:74:fa:54:86:84:b6:c4:06:f3:90:92:61:f4:dc:e2:57:5c
------BEGIN CERTIFICATE-----
-MIIEMDCCAxigAwIBAgIJANqb7HHzA7AZMA0GCSqGSIb3DQEBCwUAMIGkMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRydXN0Q29y
-IFJvb3RDZXJ0IENBLTEwHhcNMTYwMjA0MTIzMjE2WhcNMjkxMjMxMTcyMzE2WjCB
-pDELMAkGA1UEBhMCUEExDzANBgNVBAgMBlBhbmFtYTEUMBIGA1UEBwwLUGFuYW1h
-IENpdHkxJDAiBgNVBAoMG1RydXN0Q29yIFN5c3RlbXMgUy4gZGUgUi5MLjEnMCUG
-A1UECwweVHJ1c3RDb3IgQ2VydGlmaWNhdGUgQXV0aG9yaXR5MR8wHQYDVQQDDBZU
-cnVzdENvciBSb290Q2VydCBDQS0xMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
-CgKCAQEAv463leLCJhJrMxnHQFgKq1mqjQCj/IDHUHuO1CAmujIS2CNUSSUQIpid
-RtLByZ5OGy4sDjjzGiVoHKZaBeYei0i/mJZ0PmnK6bV4pQa81QBeCQryJ3pS/C3V
-seq0iWEk8xoT26nPUu0MJLq5nux+AHT6k61sKZKuUbS701e/s/OojZz0JEsq1pme
-9J7+wH5COucLlVPat2gOkEz7cD+PSiyU8ybdY2mplNgQTsVHCJCZGxdNuWxu72CV
-EY4hgLW9oHPY0LJ3xEXqWib7ZnZ2+AYfYW0PVcWDtxBWcgYHpfOxGgMFZA6dWorW
-hnAbJN7+KIor0Gqw/Hqi3LJ5DotlDwIDAQABo2MwYTAdBgNVHQ4EFgQU7mtJPHo/
-DeOxCbeKyKsZn3MzUOcwHwYDVR0jBBgwFoAU7mtJPHo/DeOxCbeKyKsZn3MzUOcw
-DwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYwDQYJKoZIhvcNAQELBQAD
-ggEBACUY1JGPE+6PHh0RU9otRCkZoB5rMZ5NDp6tPVxBb5UrJKF5mDo4Nvu7Zp5I
-/5CQ7z3UuJu0h3U/IJvOcs+hVcFNZKIZBqEHMwwLKeXx6quj7LUKdJDHfXLy11yf
-ke+Ri7fc7Waiz45mO7yfOgLgJ90WmMCV1Aqk5IGadZQ1nJBfiDcGrVmVCrDRZ9MZ
-yonnMlo2HD6CqFqTvsbQZJG2z9m2GM/bftJlo6bEjhcxwft+dtvTheNYsnd6djts
-L1Ac59v2Z3kf9YKVmgenFK+P3CghZwnS1k1aHBkcjndcw5QkPTJrS37UeJSDvjdN
-zl/HHk484IkzlQsPpTLWPFp5LBk=
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-2"
-# Serial: 2711694510199101698
-# MD5 Fingerprint: a2:e1:f8:18:0b:ba:45:d5:c7:41:2a:bb:37:52:45:64
-# SHA1 Fingerprint: b8:be:6d:cb:56:f1:55:b9:63:d4:12:ca:4e:06:34:c7:94:b2:1c:c0
-# SHA256 Fingerprint: 07:53:e9:40:37:8c:1b:d5:e3:83:6e:39:5d:ae:a5:cb:83:9e:50:46:f1:bd:0e:ae:19:51:cf:10:fe:c7:c9:65
------BEGIN CERTIFICATE-----
-MIIGLzCCBBegAwIBAgIIJaHfyjPLWQIwDQYJKoZIhvcNAQELBQAwgaQxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEfMB0GA1UEAwwWVHJ1c3RDb3Ig
-Um9vdENlcnQgQ0EtMjAeFw0xNjAyMDQxMjMyMjNaFw0zNDEyMzExNzI2MzlaMIGk
-MQswCQYDVQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEg
-Q2l0eTEkMCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYD
-VQQLDB5UcnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRy
-dXN0Q29yIFJvb3RDZXJ0IENBLTIwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIK
-AoICAQCnIG7CKqJiJJWQdsg4foDSq8GbZQWU9MEKENUCrO2fk8eHyLAnK0IMPQo+
-QVqedd2NyuCb7GgypGmSaIwLgQ5WoD4a3SwlFIIvl9NkRvRUqdw6VC0xK5mC8tkq
-1+9xALgxpL56JAfDQiDyitSSBBtlVkxs1Pu2YVpHI7TYabS3OtB0PAx1oYxOdqHp
-2yqlO/rOsP9+aij9JxzIsekp8VduZLTQwRVtDr4uDkbIXvRR/u8OYzo7cbrPb1nK
-DOObXUm4TOJXsZiKQlecdu/vvdFoqNL0Cbt3Nb4lggjEFixEIFapRBF37120Hape
-az6LMvYHL1cEksr1/p3C6eizjkxLAjHZ5DxIgif3GIJ2SDpxsROhOdUuxTTCHWKF
-3wP+TfSvPd9cW436cOGlfifHhi5qjxLGhF5DUVCcGZt45vz27Ud+ez1m7xMTiF88
-oWP7+ayHNZ/zgp6kPwqcMWmLmaSISo5uZk3vFsQPeSghYA2FFn3XVDjxklb9tTNM
-g9zXEJ9L/cb4Qr26fHMC4P99zVvh1Kxhe1fVSntb1IVYJ12/+CtgrKAmrhQhJ8Z3
-mjOAPF5GP/fDsaOGM8boXg25NSyqRsGFAnWAoOsk+xWq5Gd/bnc/9ASKL3x74xdh
-8N0JqSDIvgmk0H5Ew7IwSjiqqewYmgeCK9u4nBit2uBGF6zPXQIDAQABo2MwYTAd
-BgNVHQ4EFgQU2f4hQG6UnrybPZx9mCAZ5YwwYrIwHwYDVR0jBBgwFoAU2f4hQG6U
-nrybPZx9mCAZ5YwwYrIwDwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYw
-DQYJKoZIhvcNAQELBQADggIBAJ5Fngw7tu/hOsh80QA9z+LqBrWyOrsGS2h60COX
-dKcs8AjYeVrXWoSK2BKaG9l9XE1wxaX5q+WjiYndAfrs3fnpkpfbsEZC89NiqpX+
-MWcUaViQCqoL7jcjx1BRtPV+nuN79+TMQjItSQzL/0kMmx40/W5ulop5A7Zv2wnL
-/V9lFDfhOPXzYRZY5LVtDQsEGz9QLX+zx3oaFoBg+Iof6Rsqxvm6ARppv9JYx1RX
-CI/hOWB3S6xZhBqI8d3LT3jX5+EzLfzuQfogsL7L9ziUwOHQhQ+77Sxzq+3+knYa
-ZH9bDTMJBzN7Bj8RpFxwPIXAz+OQqIN3+tvmxYxoZxBnpVIt8MSZj3+/0WvitUfW
-2dCFmU2Umw9Lje4AWkcdEQOsQRivh7dvDDqPys/cA8GiCcjl/YBeyGBCARsaU1q7
-N6a3vLqE6R5sGtRk2tRD/pOLS/IseRYQ1JMLiI+h2IYURpFHmygk71dSTlxCnKr3
-Sewn6EAes6aJInKc9Q0ztFijMDvd1GpUk74aTfOTlPf8hAs/hCBcNANExdqtvArB
-As8e5ZTZ845b2EzwnexhF7sUMlQMAimTHpKG9n/v55IFDlndmQguLvqcAFLTxWYp
-5KeXRKQOKIETNcX2b2TmQcTVL8w0RSXPQQCWPUouwpaYT05KnJe32x+SMsj/D1Fu
-1uwJ
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor ECA-1"
-# Serial: 9548242946988625984
-# MD5 Fingerprint: 27:92:23:1d:0a:f5:40:7c:e9:e6:6b:9d:d8:f5:e7:6c
-# SHA1 Fingerprint: 58:d1:df:95:95:67:6b:63:c0:f0:5b:1c:17:4d:8b:84:0b:c8:78:bd
-# SHA256 Fingerprint: 5a:88:5d:b1:9c:01:d9:12:c5:75:93:88:93:8c:af:bb:df:03:1a:b2:d4:8e:91:ee:15:58:9b:42:97:1d:03:9c
------BEGIN CERTIFICATE-----
-MIIEIDCCAwigAwIBAgIJAISCLF8cYtBAMA0GCSqGSIb3DQEBCwUAMIGcMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxFzAVBgNVBAMMDlRydXN0Q29y
-IEVDQS0xMB4XDTE2MDIwNDEyMzIzM1oXDTI5MTIzMTE3MjgwN1owgZwxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEXMBUGA1UEAwwOVHJ1c3RDb3Ig
-RUNBLTEwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDPj+ARtZ+odnbb
-3w9U73NjKYKtR8aja+3+XzP4Q1HpGjORMRegdMTUpwHmspI+ap3tDvl0mEDTPwOA
-BoJA6LHip1GnHYMma6ve+heRK9jGrB6xnhkB1Zem6g23xFUfJ3zSCNV2HykVh0A5
-3ThFEXXQmqc04L/NyFIduUd+Dbi7xgz2c1cWWn5DkR9VOsZtRASqnKmcp0yJF4Ou
-owReUoCLHhIlERnXDH19MURB6tuvsBzvgdAsxZohmz3tQjtQJvLsznFhBmIhVE5/
-wZ0+fyCMgMsq2JdiyIMzkX2woloPV+g7zPIlstR8L+xNxqE6FXrntl019fZISjZF
-ZtS6mFjBAgMBAAGjYzBhMB0GA1UdDgQWBBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAf
-BgNVHSMEGDAWgBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAPBgNVHRMBAf8EBTADAQH/
-MA4GA1UdDwEB/wQEAwIBhjANBgkqhkiG9w0BAQsFAAOCAQEABT41XBVwm8nHc2Fv
-civUwo/yQ10CzsSUuZQRg2dd4mdsdXa/uwyqNsatR5Nj3B5+1t4u/ukZMjgDfxT2
-AHMsWbEhBuH7rBiVDKP/mZb3Kyeb1STMHd3BOuCYRLDE5D53sXOpZCz2HAF8P11F
-hcCF5yWPldwX8zyfGm6wyuMdKulMY/okYWLW2n62HGz1Ah3UKt1VkOsqEUc8Ll50
-soIipX1TH0XsJ5F95yIW6MBoNtjG8U+ARDL54dHRHareqKucBK+tIA5kmE2la8BI
-WJZpTdwHjFGTot+fDz2LYLSCjaoITmJF4PkL0uDgPFveXHEnJcLmA4GLEFPjx1Wi
-tJ/X5g==
------END CERTIFICATE-----
-
 # Issuer: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Subject: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Label: "SSL.com Root Certification Authority RSA"
 # Serial: 8875640296558310041
 # MD5 Fingerprint: 86:69:12:c0:70:f1:ec:ac:ac:c2:d5:bc:a5:5b:a1:29
 # SHA1 Fingerprint: b7:ab:33:08:d1:ea:44:77:ba:14:80:12:5a:6f:bd:a9:36:49:0c:bb
 # SHA256 Fingerprint: 85:66:6a:56:2e:e0:be:5c:e9:25:c1:d8:89:0a:6f:76:a8:7e:c1:6d:4d:7d:5f:29:ea:74:19:cf:20:12:3b:69
```

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/500.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/actions.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_list.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_results.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/color_theme_toggle.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/color_theme_toggle.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/index.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/login.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/object_history.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/pagination.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/search_form.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/submit_line.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_done.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_form.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_done.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_email.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_form.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/index.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap.xml` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/div.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/div.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/p.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/p.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/table.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/table.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/ul.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/ul.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/div.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/div.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/p.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/p.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/table.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/table.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/forms/templates/django/forms/ul.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/ul.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/views/templates/default_urlconf.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/default_urlconf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/views/templates/technical_404.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/technical_404.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/django/views/templates/technical_500.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/technical_500.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/docutils-0.19.dist-info/SOURCES.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/SOURCES.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/docutils-0.19.dist-info/dependency_links.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/dependency_links.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/docutils-0.19.dist-info/top_level.html` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/top_level.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files 2% similar despite different names*

```diff
@@ -632,45 +632,14 @@
 IC9Bi5HcSEW88cbeunZrM8gALTFGTO3nnc+IlP8zwFboJIYmuNg4ON8qa90SzMc/
 RxdMosIGlgnW2/4/PEZB31jiVg88O8EckzXZOFKs7sjsLjBOlDW0JB9LeGna8gI4
 zJVSk/BwJVmcIGfE7vmLV2H0knZ9P4SNVbfo5azV8fUZVqZa+5Acr5Pr5RzUZ5dd
 BA6+C4OmF4O5MBKgxTMVBbkN+8cFduPYSo38NBejxiEovjBFMR7HeL5YYTisO+IB
 ZQ==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Subject: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Label: "Network Solutions Certificate Authority"
-# Serial: 116697915152937497490437556386812487904
-# MD5 Fingerprint: d3:f3:a6:16:c0:fa:6b:1d:59:b1:2d:96:4d:0e:11:2e
-# SHA1 Fingerprint: 74:f8:a3:c3:ef:e7:b3:90:06:4b:83:90:3c:21:64:60:20:e5:df:ce
-# SHA256 Fingerprint: 15:f0:ba:00:a3:ac:7a:f3:ac:88:4c:07:2b:10:11:a0:77:bd:77:c0:97:f4:01:64:b2:f8:59:8a:bd:83:86:0c
------BEGIN CERTIFICATE-----
-MIID5jCCAs6gAwIBAgIQV8szb8JcFuZHFhfjkDFo4DANBgkqhkiG9w0BAQUFADBi
-MQswCQYDVQQGEwJVUzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMu
-MTAwLgYDVQQDEydOZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3Jp
-dHkwHhcNMDYxMjAxMDAwMDAwWhcNMjkxMjMxMjM1OTU5WjBiMQswCQYDVQQGEwJV
-UzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMuMTAwLgYDVQQDEydO
-ZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkwggEiMA0GCSqG
-SIb3DQEBAQUAA4IBDwAwggEKAoIBAQDkvH6SMG3G2I4rC7xGzuAnlt7e+foS0zwz
-c7MEL7xxjOWftiJgPl9dzgn/ggwbmlFQGiaJ3dVhXRncEg8tCqJDXRfQNJIg6nPP
-OCwGJgl6cvf6UDL4wpPTaaIjzkGxzOTVHzbRijr4jGPiFFlp7Q3Tf2vouAPlT2rl
-mGNpSAW+Lv8ztumXWWn4Zxmuk2GWRBXTcrA/vGp97Eh/jcOrqnErU2lBUzS1sLnF
-BgrEsEX1QV1uiUV7PTsmjHTC5dLRfbIR1PtYMiKagMnc/Qzpf14Dl847ABSHJ3A4
-qY5usyd2mFHgBeMhqxrVhSI8KbWaFsWAqPS7azCPL0YCorEMIuDTAgMBAAGjgZcw
-gZQwHQYDVR0OBBYEFCEwyfsA106Y2oeqKtCnLrFAMadMMA4GA1UdDwEB/wQEAwIB
-BjAPBgNVHRMBAf8EBTADAQH/MFIGA1UdHwRLMEkwR6BFoEOGQWh0dHA6Ly9jcmwu
-bmV0c29sc3NsLmNvbS9OZXR3b3JrU29sdXRpb25zQ2VydGlmaWNhdGVBdXRob3Jp
-dHkuY3JsMA0GCSqGSIb3DQEBBQUAA4IBAQC7rkvnt1frf6ott3NHhWrB5KUd5Oc8
-6fRZZXe1eltajSU24HqXLjjAV2CDmAaDn7l2em5Q4LqILPxFzBiwmZVRDuwduIj/
-h1AcgsLj4DKAv6ALR8jDMe+ZZzKATxcheQxpXN5eNK4CtSbqUN9/GGUsyfJj4akH
-/nxxH2szJGoeBfcFaMBqEssuXmHLrijTfsK0ZpEmXzwuJF/LWA/rKOyvEZbz3Htv
-wKeI8lN3s2Berq4o2jUsbzRF0ybh3uxbTydrFny9RAQYgrOJeRcQcT16ohZO9QHN
-pGxlaKFJdlxDydi8NmdspZS11My5vWo1ViHe2MPr+8ukYEywVaCge1ey
------END CERTIFICATE-----
-
 # Issuer: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Subject: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Label: "COMODO ECC Certification Authority"
 # Serial: 41578283867086692638256921589707938090
 # MD5 Fingerprint: 7c:62:ff:74:9d:31:53:5e:68:4a:d5:78:aa:1e:bf:23
 # SHA1 Fingerprint: 9f:74:4e:9f:2b:4d:ba:ec:0f:31:2c:50:b6:56:3b:8e:2d:93:c3:11
 # SHA256 Fingerprint: 17:93:92:7a:06:14:54:97:89:ad:ce:2f:8f:34:f7:f0:b6:6d:0f:3a:e3:a3:b8:4d:21:ec:15:db:ba:4f:ad:c7
@@ -2200,54 +2169,14 @@
 hOvRnkmSh5SHDDqFSmafnVmTTZdhBoZKo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYD
 VR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUPeYpSJvqB8ohREom3m7e0oPQn1kwCgYI
 KoZIzj0EAwMDaAAwZQIxAOVpEslu28YxuglB4Zf4+/2a4n0Sye18ZNPLBSWLVtmg
 515dTguDnFt2KaAJJiFqYgIwcdK1j1zqO+F4CYWodZI7yFz9SO8NdCKoCOJuxUnO
 xwy8p2Fp8fc74SrL+SvzZpA3
 -----END CERTIFICATE-----
 
-# Issuer: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Subject: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Label: "Staat der Nederlanden EV Root CA"
-# Serial: 10000013
-# MD5 Fingerprint: fc:06:af:7b:e8:1a:f1:9a:b4:e8:d2:70:1f:c0:f5:ba
-# SHA1 Fingerprint: 76:e2:7e:c1:4f:db:82:c1:c0:a6:75:b5:05:be:3d:29:b4:ed:db:bb
-# SHA256 Fingerprint: 4d:24:91:41:4c:fe:95:67:46:ec:4c:ef:a6:cf:6f:72:e2:8a:13:29:43:2f:9d:8a:90:7a:c4:cb:5d:ad:c1:5a
------BEGIN CERTIFICATE-----
-MIIFcDCCA1igAwIBAgIEAJiWjTANBgkqhkiG9w0BAQsFADBYMQswCQYDVQQGEwJO
-TDEeMBwGA1UECgwVU3RhYXQgZGVyIE5lZGVybGFuZGVuMSkwJwYDVQQDDCBTdGFh
-dCBkZXIgTmVkZXJsYW5kZW4gRVYgUm9vdCBDQTAeFw0xMDEyMDgxMTE5MjlaFw0y
-MjEyMDgxMTEwMjhaMFgxCzAJBgNVBAYTAk5MMR4wHAYDVQQKDBVTdGFhdCBkZXIg
-TmVkZXJsYW5kZW4xKTAnBgNVBAMMIFN0YWF0IGRlciBOZWRlcmxhbmRlbiBFViBS
-b290IENBMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA48d+ifkkSzrS
-M4M1LGns3Amk41GoJSt5uAg94JG6hIXGhaTK5skuU6TJJB79VWZxXSzFYGgEt9nC
-UiY4iKTWO0Cmws0/zZiTs1QUWJZV1VD+hq2kY39ch/aO5ieSZxeSAgMs3NZmdO3d
-Z//BYY1jTw+bbRcwJu+r0h8QoPnFfxZpgQNH7R5ojXKhTbImxrpsX23Wr9GxE46p
-rfNeaXUmGD5BKyF/7otdBwadQ8QpCiv8Kj6GyzyDOvnJDdrFmeK8eEEzduG/L13l
-pJhQDBXd4Pqcfzho0LKmeqfRMb1+ilgnQ7O6M5HTp5gVXJrm0w912fxBmJc+qiXb
-j5IusHsMX/FjqTf5m3VpTCgmJdrV8hJwRVXj33NeN/UhbJCONVrJ0yPr08C+eKxC
-KFhmpUZtcALXEPlLVPxdhkqHz3/KRawRWrUgUY0viEeXOcDPusBCAUCZSCELa6fS
-/ZbV0b5GnUngC6agIk440ME8MLxwjyx1zNDFjFE7PZQIZCZhfbnDZY8UnCHQqv0X
-cgOPvZuM5l5Tnrmd74K74bzickFbIZTTRTeU0d8JOV3nI6qaHcptqAqGhYqCvkIH
-1vI4gnPah1vlPNOePqc7nvQDs/nxfRN0Av+7oeX6AHkcpmZBiFxgV6YuCcS6/ZrP
-px9Aw7vMWgpVSzs4dlG4Y4uElBbmVvMCAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB
-/zAOBgNVHQ8BAf8EBAMCAQYwHQYDVR0OBBYEFP6rAJCYniT8qcwaivsnuL8wbqg7
-MA0GCSqGSIb3DQEBCwUAA4ICAQDPdyxuVr5Os7aEAJSrR8kN0nbHhp8dB9O2tLsI
-eK9p0gtJ3jPFrK3CiAJ9Brc1AsFgyb/E6JTe1NOpEyVa/m6irn0F3H3zbPB+po3u
-2dfOWBfoqSmuc0iH55vKbimhZF8ZE/euBhD/UcabTVUlT5OZEAFTdfETzsemQUHS
-v4ilf0X8rLiltTMMgsT7B/Zq5SWEXwbKwYY5EdtYzXc7LMJMD16a4/CrPmEbUCTC
-wPTxGfARKbalGAKb12NMcIxHowNDXLldRqANb/9Zjr7dn3LDWyvfjFvO5QxGbJKy
-CqNMVEIYFRIYvdr8unRu/8G2oGTYqV9Vrp9canaW2HNnh/tNf1zuacpzEPuKqf2e
-vTY4SUmH9A4U8OmHuD+nT3pajnnUk+S7aFKErGzp85hwVXIy+TSrK0m1zSBi5Dp6
-Z2Orltxtrpfs/J92VoguZs9btsmksNcFuuEnL5O7Jiqik7Ab846+HUCjuTaPPoIa
-Gl6I6lD4WeKDRikL40Rc4ZW2aZCaFG+XroHPaO+Zmr615+F/+PoTRxZMzG0IQOeL
-eG9QgkRQP2YGiqtDhFZKDyAthg710tvSeopLzaXoTvFeJiUBWSOgftL2fiFX1ye8
-FVdMpEbB4IMeDExNH08GGeL5qPQ6gqGyeUN51q1veieQA6TqJIc/2b3Z6fJfUEkc
-7uzXLg==
------END CERTIFICATE-----
-
 # Issuer: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Subject: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Label: "IdenTrust Commercial Root CA 1"
 # Serial: 13298821034946342390520003877796839426
 # MD5 Fingerprint: b3:3e:77:73:75:ee:a0:d3:e3:7e:49:63:49:59:bb:c7
 # SHA1 Fingerprint: df:71:7e:aa:4a:d9:4e:c9:55:84:99:60:2d:48:de:5f:bc:f0:3a:25
 # SHA256 Fingerprint: 5d:56:49:9b:e4:d2:e0:8b:cf:ca:d0:8a:3e:38:72:3d:50:50:3b:de:70:69:48:e4:2f:55:60:30:19:e5:28:ae
@@ -2847,124 +2776,14 @@
 2c9Si1vIY9RCPqAzekYu9wogRlR+ak8x8YF+QnQ4ZXMn7sZ8uI7XpTrXmKGcjBBV
 09tL7ECQ8s1uV9JiDnxXk7Gnbc2dg7sq5+W2O3FYrf3RRbxake5TFW/TRQl1brqQ
 XR4EzzffHqhmsYzmIGrv/EhOdJhCrylvLmrH+33RZjEizIYAfmaDDEL0vTSSwxrq
 T8p+ck0LcIymSLumoRT2+1hEmRSuqguTaaApJUqlyyvdimYHFngVV3Eb7PVHhPOe
 MTd61X8kreS8/f3MboPoDKi3QWwH3b08hpcv0g==
 -----END CERTIFICATE-----
 
-# Issuer: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-1"
-# Serial: 15752444095811006489
-# MD5 Fingerprint: 6e:85:f1:dc:1a:00:d3:22:d5:b2:b2:ac:6b:37:05:45
-# SHA1 Fingerprint: ff:bd:cd:e7:82:c8:43:5e:3c:6f:26:86:5c:ca:a8:3a:45:5b:c3:0a
-# SHA256 Fingerprint: d4:0e:9c:86:cd:8f:e4:68:c1:77:69:59:f4:9e:a7:74:fa:54:86:84:b6:c4:06:f3:90:92:61:f4:dc:e2:57:5c
------BEGIN CERTIFICATE-----
-MIIEMDCCAxigAwIBAgIJANqb7HHzA7AZMA0GCSqGSIb3DQEBCwUAMIGkMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRydXN0Q29y
-IFJvb3RDZXJ0IENBLTEwHhcNMTYwMjA0MTIzMjE2WhcNMjkxMjMxMTcyMzE2WjCB
-pDELMAkGA1UEBhMCUEExDzANBgNVBAgMBlBhbmFtYTEUMBIGA1UEBwwLUGFuYW1h
-IENpdHkxJDAiBgNVBAoMG1RydXN0Q29yIFN5c3RlbXMgUy4gZGUgUi5MLjEnMCUG
-A1UECwweVHJ1c3RDb3IgQ2VydGlmaWNhdGUgQXV0aG9yaXR5MR8wHQYDVQQDDBZU
-cnVzdENvciBSb290Q2VydCBDQS0xMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
-CgKCAQEAv463leLCJhJrMxnHQFgKq1mqjQCj/IDHUHuO1CAmujIS2CNUSSUQIpid
-RtLByZ5OGy4sDjjzGiVoHKZaBeYei0i/mJZ0PmnK6bV4pQa81QBeCQryJ3pS/C3V
-seq0iWEk8xoT26nPUu0MJLq5nux+AHT6k61sKZKuUbS701e/s/OojZz0JEsq1pme
-9J7+wH5COucLlVPat2gOkEz7cD+PSiyU8ybdY2mplNgQTsVHCJCZGxdNuWxu72CV
-EY4hgLW9oHPY0LJ3xEXqWib7ZnZ2+AYfYW0PVcWDtxBWcgYHpfOxGgMFZA6dWorW
-hnAbJN7+KIor0Gqw/Hqi3LJ5DotlDwIDAQABo2MwYTAdBgNVHQ4EFgQU7mtJPHo/
-DeOxCbeKyKsZn3MzUOcwHwYDVR0jBBgwFoAU7mtJPHo/DeOxCbeKyKsZn3MzUOcw
-DwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYwDQYJKoZIhvcNAQELBQAD
-ggEBACUY1JGPE+6PHh0RU9otRCkZoB5rMZ5NDp6tPVxBb5UrJKF5mDo4Nvu7Zp5I
-/5CQ7z3UuJu0h3U/IJvOcs+hVcFNZKIZBqEHMwwLKeXx6quj7LUKdJDHfXLy11yf
-ke+Ri7fc7Waiz45mO7yfOgLgJ90WmMCV1Aqk5IGadZQ1nJBfiDcGrVmVCrDRZ9MZ
-yonnMlo2HD6CqFqTvsbQZJG2z9m2GM/bftJlo6bEjhcxwft+dtvTheNYsnd6djts
-L1Ac59v2Z3kf9YKVmgenFK+P3CghZwnS1k1aHBkcjndcw5QkPTJrS37UeJSDvjdN
-zl/HHk484IkzlQsPpTLWPFp5LBk=
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-2"
-# Serial: 2711694510199101698
-# MD5 Fingerprint: a2:e1:f8:18:0b:ba:45:d5:c7:41:2a:bb:37:52:45:64
-# SHA1 Fingerprint: b8:be:6d:cb:56:f1:55:b9:63:d4:12:ca:4e:06:34:c7:94:b2:1c:c0
-# SHA256 Fingerprint: 07:53:e9:40:37:8c:1b:d5:e3:83:6e:39:5d:ae:a5:cb:83:9e:50:46:f1:bd:0e:ae:19:51:cf:10:fe:c7:c9:65
------BEGIN CERTIFICATE-----
-MIIGLzCCBBegAwIBAgIIJaHfyjPLWQIwDQYJKoZIhvcNAQELBQAwgaQxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEfMB0GA1UEAwwWVHJ1c3RDb3Ig
-Um9vdENlcnQgQ0EtMjAeFw0xNjAyMDQxMjMyMjNaFw0zNDEyMzExNzI2MzlaMIGk
-MQswCQYDVQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEg
-Q2l0eTEkMCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYD
-VQQLDB5UcnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRy
-dXN0Q29yIFJvb3RDZXJ0IENBLTIwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIK
-AoICAQCnIG7CKqJiJJWQdsg4foDSq8GbZQWU9MEKENUCrO2fk8eHyLAnK0IMPQo+
-QVqedd2NyuCb7GgypGmSaIwLgQ5WoD4a3SwlFIIvl9NkRvRUqdw6VC0xK5mC8tkq
-1+9xALgxpL56JAfDQiDyitSSBBtlVkxs1Pu2YVpHI7TYabS3OtB0PAx1oYxOdqHp
-2yqlO/rOsP9+aij9JxzIsekp8VduZLTQwRVtDr4uDkbIXvRR/u8OYzo7cbrPb1nK
-DOObXUm4TOJXsZiKQlecdu/vvdFoqNL0Cbt3Nb4lggjEFixEIFapRBF37120Hape
-az6LMvYHL1cEksr1/p3C6eizjkxLAjHZ5DxIgif3GIJ2SDpxsROhOdUuxTTCHWKF
-3wP+TfSvPd9cW436cOGlfifHhi5qjxLGhF5DUVCcGZt45vz27Ud+ez1m7xMTiF88
-oWP7+ayHNZ/zgp6kPwqcMWmLmaSISo5uZk3vFsQPeSghYA2FFn3XVDjxklb9tTNM
-g9zXEJ9L/cb4Qr26fHMC4P99zVvh1Kxhe1fVSntb1IVYJ12/+CtgrKAmrhQhJ8Z3
-mjOAPF5GP/fDsaOGM8boXg25NSyqRsGFAnWAoOsk+xWq5Gd/bnc/9ASKL3x74xdh
-8N0JqSDIvgmk0H5Ew7IwSjiqqewYmgeCK9u4nBit2uBGF6zPXQIDAQABo2MwYTAd
-BgNVHQ4EFgQU2f4hQG6UnrybPZx9mCAZ5YwwYrIwHwYDVR0jBBgwFoAU2f4hQG6U
-nrybPZx9mCAZ5YwwYrIwDwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYw
-DQYJKoZIhvcNAQELBQADggIBAJ5Fngw7tu/hOsh80QA9z+LqBrWyOrsGS2h60COX
-dKcs8AjYeVrXWoSK2BKaG9l9XE1wxaX5q+WjiYndAfrs3fnpkpfbsEZC89NiqpX+
-MWcUaViQCqoL7jcjx1BRtPV+nuN79+TMQjItSQzL/0kMmx40/W5ulop5A7Zv2wnL
-/V9lFDfhOPXzYRZY5LVtDQsEGz9QLX+zx3oaFoBg+Iof6Rsqxvm6ARppv9JYx1RX
-CI/hOWB3S6xZhBqI8d3LT3jX5+EzLfzuQfogsL7L9ziUwOHQhQ+77Sxzq+3+knYa
-ZH9bDTMJBzN7Bj8RpFxwPIXAz+OQqIN3+tvmxYxoZxBnpVIt8MSZj3+/0WvitUfW
-2dCFmU2Umw9Lje4AWkcdEQOsQRivh7dvDDqPys/cA8GiCcjl/YBeyGBCARsaU1q7
-N6a3vLqE6R5sGtRk2tRD/pOLS/IseRYQ1JMLiI+h2IYURpFHmygk71dSTlxCnKr3
-Sewn6EAes6aJInKc9Q0ztFijMDvd1GpUk74aTfOTlPf8hAs/hCBcNANExdqtvArB
-As8e5ZTZ845b2EzwnexhF7sUMlQMAimTHpKG9n/v55IFDlndmQguLvqcAFLTxWYp
-5KeXRKQOKIETNcX2b2TmQcTVL8w0RSXPQQCWPUouwpaYT05KnJe32x+SMsj/D1Fu
-1uwJ
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor ECA-1"
-# Serial: 9548242946988625984
-# MD5 Fingerprint: 27:92:23:1d:0a:f5:40:7c:e9:e6:6b:9d:d8:f5:e7:6c
-# SHA1 Fingerprint: 58:d1:df:95:95:67:6b:63:c0:f0:5b:1c:17:4d:8b:84:0b:c8:78:bd
-# SHA256 Fingerprint: 5a:88:5d:b1:9c:01:d9:12:c5:75:93:88:93:8c:af:bb:df:03:1a:b2:d4:8e:91:ee:15:58:9b:42:97:1d:03:9c
------BEGIN CERTIFICATE-----
-MIIEIDCCAwigAwIBAgIJAISCLF8cYtBAMA0GCSqGSIb3DQEBCwUAMIGcMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxFzAVBgNVBAMMDlRydXN0Q29y
-IEVDQS0xMB4XDTE2MDIwNDEyMzIzM1oXDTI5MTIzMTE3MjgwN1owgZwxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEXMBUGA1UEAwwOVHJ1c3RDb3Ig
-RUNBLTEwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDPj+ARtZ+odnbb
-3w9U73NjKYKtR8aja+3+XzP4Q1HpGjORMRegdMTUpwHmspI+ap3tDvl0mEDTPwOA
-BoJA6LHip1GnHYMma6ve+heRK9jGrB6xnhkB1Zem6g23xFUfJ3zSCNV2HykVh0A5
-3ThFEXXQmqc04L/NyFIduUd+Dbi7xgz2c1cWWn5DkR9VOsZtRASqnKmcp0yJF4Ou
-owReUoCLHhIlERnXDH19MURB6tuvsBzvgdAsxZohmz3tQjtQJvLsznFhBmIhVE5/
-wZ0+fyCMgMsq2JdiyIMzkX2woloPV+g7zPIlstR8L+xNxqE6FXrntl019fZISjZF
-ZtS6mFjBAgMBAAGjYzBhMB0GA1UdDgQWBBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAf
-BgNVHSMEGDAWgBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAPBgNVHRMBAf8EBTADAQH/
-MA4GA1UdDwEB/wQEAwIBhjANBgkqhkiG9w0BAQsFAAOCAQEABT41XBVwm8nHc2Fv
-civUwo/yQ10CzsSUuZQRg2dd4mdsdXa/uwyqNsatR5Nj3B5+1t4u/ukZMjgDfxT2
-AHMsWbEhBuH7rBiVDKP/mZb3Kyeb1STMHd3BOuCYRLDE5D53sXOpZCz2HAF8P11F
-hcCF5yWPldwX8zyfGm6wyuMdKulMY/okYWLW2n62HGz1Ah3UKt1VkOsqEUc8Ll50
-soIipX1TH0XsJ5F95yIW6MBoNtjG8U+ARDL54dHRHareqKucBK+tIA5kmE2la8BI
-WJZpTdwHjFGTot+fDz2LYLSCjaoITmJF4PkL0uDgPFveXHEnJcLmA4GLEFPjx1Wi
-tJ/X5g==
------END CERTIFICATE-----
-
 # Issuer: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Subject: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Label: "SSL.com Root Certification Authority RSA"
 # Serial: 8875640296558310041
 # MD5 Fingerprint: 86:69:12:c0:70:f1:ec:ac:ac:c2:d5:bc:a5:5b:a1:29
 # SHA1 Fingerprint: b7:ab:33:08:d1:ea:44:77:ba:14:80:12:5a:6f:bd:a9:36:49:0c:bb
 # SHA256 Fingerprint: 85:66:6a:56:2e:e0:be:5c:e9:25:c1:d8:89:0a:6f:76:a8:7e:c1:6d:4d:7d:5f:29:ea:74:19:cf:20:12:3b:69
```

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/saml2/data/templates/template_enc.xml` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/data/templates/template_enc.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.7/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.6/setup.py` & `djangosaml2-1.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return codecs.open(
         os.path.join(os.path.dirname(__file__), *rnames), encoding="utf-8"
     ).read()
 
 
 setup(
     name="djangosaml2",
-    version="1.5.6",
+    version="1.5.7",
     description="pysaml2 integration for Django",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
```

