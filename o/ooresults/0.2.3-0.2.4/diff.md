# Comparing `tmp/ooresults-0.2.3.tar.gz` & `tmp/ooresults-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooresults-0.2.3.tar", last modified: Sun Apr 23 16:35:30 2023, max compression
+gzip compressed data, was "ooresults-0.2.4.tar", last modified: Sun May  7 16:09:25 2023, max compression
```

## Comparing `ooresults-0.2.3.tar` & `ooresults-0.2.4.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.453791 ooresults-0.2.3/
--rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.3/LICENSE
--rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.3/MANIFEST.in
--rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-04-23 16:35:30.453791 ooresults-0.2.3/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.3/README.rst
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.429791 ooresults-0.2.3/ooresults/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    11381 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/_server.py
--rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/configuration.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.433791 ooresults-0.2.3/ooresults/handler/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/handler/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     9134 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/build_results.py
--rw-r--r--   0 rainer    (1000) users      (100)     7873 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     2597 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)     4559 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/handler/competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     5824 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/demo_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    12416 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     3351 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/events.py
--rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/handler/handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    31886 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/model.py
--rw-r--r--   0 rainer    (1000) users      (100)     3536 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/results.py
--rw-r--r--   0 rainer    (1000) users      (100)     4892 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/handler/series.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.433791 ooresults-0.2.3/ooresults/pdf/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.437791 ooresults-0.2.3/ooresults/pdf/fonts/
--rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Bold.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Italic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Regular.ttf
--rw-r--r--   0 rainer    (1000) users      (100)     2806 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/pdf.py
--rw-r--r--   0 rainer    (1000) users      (100)    11206 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/pdf/result.py
--rw-r--r--   0 rainer    (1000) users      (100)     5283 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/pdf/series.py
--rw-r--r--   0 rainer    (1000) users      (100)    10007 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/pdf/splittimes.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.437791 ooresults-0.2.3/ooresults/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/plugins/__init__.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.429791 ooresults-0.2.3/ooresults/plugins/imports/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/plugins/imports/entries/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/plugins/imports/entries/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/plugins/imports/entries/text.py
--rw-r--r--   0 rainer    (1000) users      (100)     2813 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4068 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     5935 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     5184 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    10702 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/iof_result_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     7446 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/oe12.py
--rw-r--r--   0 rainer    (1000) users      (100)    14580 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/plugins/oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/reader.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2237 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/class_params.py
--rw-r--r--   0 rainer    (1000) users      (100)     7358 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/repo.py
--rw-r--r--   0 rainer    (1000) users      (100)    16171 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/result_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/series_type.py
--rw-r--r--   0 rainer    (1000) users      (100)    36849 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/repo/sqlite_repo.py
--rw-r--r--   0 rainer    (1000) users      (100)     1265 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/start_type.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/repo/update/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/update/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/update/update_008.py
--rw-r--r--   0 rainer    (1000) users      (100)     1890 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/repo/update/update_tables.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/schema/
--rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/schema/IOF.xsd
--rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/schema/cardreader_log.json
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/server.py
--rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/set_legacy_mode.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.441791 ooresults-0.2.3/ooresults/static/
--rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/static/style-tab.css
--rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/static/style.css
--rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/static/w3.js
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.445791 ooresults-0.2.3/ooresults/templates/
--rw-r--r--   0 rainer    (1000) users      (100)     5964 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/add_class.html
--rw-r--r--   0 rainer    (1000) users      (100)      883 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_club.html
--rw-r--r--   0 rainer    (1000) users      (100)     3093 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_competitor.html
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_course.html
--rw-r--r--   0 rainer    (1000) users      (100)     6139 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_entry.html
--rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_entry_competitors.html
--rw-r--r--   0 rainer    (1000) users      (100)     7204 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/add_entry_result.html
--rw-r--r--   0 rainer    (1000) users      (100)     2511 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/add_event.html
--rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/base.html
--rw-r--r--   0 rainer    (1000) users      (100)    11941 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/classes_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     2957 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/classes_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6858 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/clubs_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/clubs_table.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    11673 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/competitors_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1030 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/competitors_table.html
--rw-r--r--   0 rainer    (1000) users      (100)    11955 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/courses_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1386 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/courses_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.3/ooresults/templates/demo_reader.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    19221 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/entries_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     3006 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/entries_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     9445 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/events_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/events_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     5937 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/main.html
--rw-r--r--   0 rainer    (1000) users      (100)     5924 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/results_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     5390 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/results_table.html
--rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/root.html
--rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/select_event.html
--rw-r--r--   0 rainer    (1000) users      (100)     2500 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/series_settings.html
--rw-r--r--   0 rainer    (1000) users      (100)     8367 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/series_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1541 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/series_table.html
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.445791 ooresults-0.2.3/ooresults/templates/si/
--rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/si/si1_data.html
--rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/si/si1_error.html
--rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/si/si1_page.html
--rw-r--r--   0 rainer    (1000) users      (100)     4161 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/templates/si/si2_data.html
--rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/si/si2_page.html
--rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/templates/unauthorized.html
--rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/user.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.445791 ooresults-0.2.3/ooresults/utils/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/utils/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1666 2023-04-23 07:29:14.000000 ooresults-0.2.3/ooresults/utils/globals.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.449791 ooresults-0.2.3/ooresults/websocket_server/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/websocket_server/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1749 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/websocket_server/si.py
--rw-r--r--   0 rainer    (1000) users      (100)    14523 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/websocket_server/websocket_handler.py
--rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.3/ooresults/websocket_server/websocket_server.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.433791 ooresults-0.2.3/ooresults.egg-info/
--rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     4563 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/SOURCES.txt
--rw-r--r--   0 rainer    (1000) users      (100)        1 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/dependency_links.txt
--rw-r--r--   0 rainer    (1000) users      (100)      102 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/entry_points.txt
--rw-r--r--   0 rainer    (1000) users      (100)      152 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/requires.txt
--rw-r--r--   0 rainer    (1000) users      (100)       10 2023-04-23 16:35:30.000000 ooresults-0.2.3/ooresults.egg-info/top_level.txt
--rwxr-xr-x   0 rainer    (1000) users      (100)      977 2023-04-23 16:33:35.000000 ooresults-0.2.3/pyproject.toml
--rwxr-xr-x   0 rainer    (1000) users      (100)      616 2023-04-23 16:35:30.453791 ooresults-0.2.3/setup.cfg
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.449791 ooresults-0.2.3/tests/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1414 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/competitor.py
--rw-r--r--   0 rainer    (1000) users      (100)     2061 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/entry.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.449791 ooresults-0.2.3/tests/model/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/model/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     8015 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/model/test_build_series_result.py
--rw-r--r--   0 rainer    (1000) users      (100)    11820 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/model/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     6578 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/model/test_event_class_results.py
--rw-r--r--   0 rainer    (1000) users      (100)    16528 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/model/test_parse_cardreader_log.py
--rw-r--r--   0 rainer    (1000) users      (100)    27576 2023-04-23 07:11:17.000000 ooresults-0.2.3/tests/model/test_store_cardreader_result.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.449791 ooresults-0.2.3/tests/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)    13070 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_export_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_import_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)     2766 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4000 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    10229 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     8789 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    30446 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/plugins/test_plugin_iof_result_list.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-04-23 16:35:30.453791 ooresults-0.2.3/tests/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    11959 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/repo/test_classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     5314 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/repo/test_clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)    10687 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/repo/test_competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     7336 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/repo/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)    39686 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/repo/test_entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     7540 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/repo/test_events.py
--rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/repo/test_settings.py
--rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_compute_result_net.py
--rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_compute_result_score.py
--rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/test_compute_result_standard.py
--rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_configuration.py
--rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/test_globals.py
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    23885 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/test_ranking.py
--rw-r--r--   0 rainer    (1000) users      (100)    26132 2023-04-23 07:29:14.000000 ooresults-0.2.3/tests/test_series.py
--rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.3/tests/test_user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.155203 ooresults-0.2.4/
+-rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.4/LICENSE
+-rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.4/MANIFEST.in
+-rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-05-07 16:09:25.155203 ooresults-0.2.4/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.4/README.rst
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.127203 ooresults-0.2.4/ooresults/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11381 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/_server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/configuration.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.131203 ooresults-0.2.4/ooresults/handler/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/handler/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9134 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/build_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7873 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2597 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4559 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/handler/competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5824 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/demo_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    12416 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3351 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/handler/handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    31158 2023-05-07 16:05:24.000000 ooresults-0.2.4/ooresults/handler/model.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3536 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4892 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/series.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.131203 ooresults-0.2.4/ooresults/pdf/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.135203 ooresults-0.2.4/ooresults/pdf/fonts/
+-rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)     2806 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/pdf.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11206 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/pdf/result.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5283 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/series.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10007 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/pdf/splittimes.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/plugins/__init__.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.123203 ooresults-0.2.4/ooresults/plugins/imports/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/plugins/imports/entries/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/plugins/imports/entries/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/plugins/imports/entries/text.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2813 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4068 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5935 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5184 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10702 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_result_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7446 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/oe12.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14580 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/reader.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2237 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/class_params.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7358 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16754 2023-05-07 16:05:24.000000 ooresults-0.2.4/ooresults/repo/result_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/series_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)    36849 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/repo/sqlite_repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1265 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/start_type.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/repo/update/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/update/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/update/update_008.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1890 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/update/update_tables.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/schema/
+-rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/schema/IOF.xsd
+-rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/schema/cardreader_log.json
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/set_legacy_mode.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.143203 ooresults-0.2.4/ooresults/static/
+-rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/static/style-tab.css
+-rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/static/style.css
+-rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/static/w3.js
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.147203 ooresults-0.2.4/ooresults/templates/
+-rw-r--r--   0 rainer    (1000) users      (100)     5964 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/add_class.html
+-rw-r--r--   0 rainer    (1000) users      (100)      883 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_club.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3093 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_competitor.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_course.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6405 2023-05-07 16:05:24.000000 ooresults-0.2.4/ooresults/templates/add_entry.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_entry_competitors.html
+-rw-r--r--   0 rainer    (1000) users      (100)     7204 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/add_entry_result.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2511 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/base.html
+-rw-r--r--   0 rainer    (1000) users      (100)    11941 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/classes_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2957 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/classes_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6858 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/clubs_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/clubs_table.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    11673 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/competitors_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1030 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/competitors_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)    11955 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/courses_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1386 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/courses_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.4/ooresults/templates/demo_reader.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    19221 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/entries_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3006 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/entries_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     9445 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/events_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/events_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5937 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/main.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5924 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/results_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5390 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/results_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/root.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/select_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2500 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/series_settings.html
+-rw-r--r--   0 rainer    (1000) users      (100)     8367 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/series_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1541 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/series_table.html
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.147203 ooresults-0.2.4/ooresults/templates/si/
+-rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/si/si1_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/si/si1_error.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/si/si1_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)     4161 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/si/si2_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/si/si2_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/unauthorized.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.147203 ooresults-0.2.4/ooresults/utils/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/utils/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1666 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/utils/globals.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.151203 ooresults-0.2.4/ooresults/websocket_server/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/websocket_server/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1749 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/websocket_server/si.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14523 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/websocket_server/websocket_handler.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/websocket_server/websocket_server.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.127203 ooresults-0.2.4/ooresults.egg-info/
+-rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     4563 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/SOURCES.txt
+-rw-r--r--   0 rainer    (1000) users      (100)        1 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/dependency_links.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      102 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/entry_points.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      152 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/requires.txt
+-rw-r--r--   0 rainer    (1000) users      (100)       10 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/top_level.txt
+-rwxr-xr-x   0 rainer    (1000) users      (100)      977 2023-05-07 16:05:24.000000 ooresults-0.2.4/pyproject.toml
+-rwxr-xr-x   0 rainer    (1000) users      (100)      616 2023-05-07 16:09:25.155203 ooresults-0.2.4/setup.cfg
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.151203 ooresults-0.2.4/tests/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1414 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/competitor.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2061 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/entry.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.151203 ooresults-0.2.4/tests/model/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/model/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8015 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/model/test_build_series_result.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11820 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/model/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     6578 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/model/test_event_class_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16528 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/model/test_parse_cardreader_log.py
+-rw-r--r--   0 rainer    (1000) users      (100)    34026 2023-05-07 16:05:24.000000 ooresults-0.2.4/tests/model/test_store_cardreader_result.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.155203 ooresults-0.2.4/tests/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)    13070 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_export_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_import_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2766 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4000 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10229 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8789 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    30446 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_result_list.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.155203 ooresults-0.2.4/tests/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11959 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/repo/test_classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5314 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/repo/test_clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10687 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/repo/test_competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7336 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/repo/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)    39686 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/repo/test_entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7540 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/repo/test_events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/repo/test_settings.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_compute_result_net.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_compute_result_score.py
+-rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/test_compute_result_standard.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_configuration.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/test_globals.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    23885 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/test_ranking.py
+-rw-r--r--   0 rainer    (1000) users      (100)    26132 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/test_series.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_user.py
```

### Comparing `ooresults-0.2.3/LICENSE` & `ooresults-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/PKG-INFO` & `ooresults-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.3
+Version: 0.2.4
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooresults-0.2.3/README.rst` & `ooresults-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/__init__.py` & `ooresults-0.2.4/ooresults/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/_reader.py` & `ooresults-0.2.4/ooresults/_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/_server.py` & `ooresults-0.2.4/ooresults/_server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/configuration.py` & `ooresults-0.2.4/ooresults/configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/__init__.py` & `ooresults-0.2.4/ooresults/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/build_results.py` & `ooresults-0.2.4/ooresults/handler/build_results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/classes.py` & `ooresults-0.2.4/ooresults/handler/classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/clubs.py` & `ooresults-0.2.4/ooresults/handler/clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/competitors.py` & `ooresults-0.2.4/ooresults/handler/competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/courses.py` & `ooresults-0.2.4/ooresults/handler/courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/demo_reader.py` & `ooresults-0.2.4/ooresults/handler/demo_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/entries.py` & `ooresults-0.2.4/ooresults/handler/entries.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/events.py` & `ooresults-0.2.4/ooresults/handler/events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/handicap.py` & `ooresults-0.2.4/ooresults/handler/handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/model.py` & `ooresults-0.2.4/ooresults/handler/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -610,45 +610,78 @@
             if event_key != "" and e.key == event_key:
                 event = e
                 break
         else:
             raise EventNotFoundError(f'Event for key "{event_key}" not found')
 
         if item["entryType"] == "cardRead":
-            entries = db.get_entries(event_id=event.id)
-            entries_controlcard = [
-                e
-                for e in entries
-                if e.class_id is not None and e.chip == item["controlCard"]
-            ]
             result = item["result"]
 
-            if len(entries_controlcard) == 1:
-                entry = entries_controlcard[0]
-                try:
-                    class_ = db.get_class(id=entry["class_id"])[0]
-                    course_id = class_["course_id"]
-                    class_params = class_["params"]
-                    controls = db.get_course(id=course_id)[0]["controls"]
-                except:
-                    class_params = ClassParams()
-                    controls = []
-
-                result.compute_result(
-                    controls=controls,
-                    class_params=class_params,
-                    start_time=entry.start.start_time,
-                    year=int(entry.get("year", None))
-                    if entry.get("year", None) is not None
-                    else None,
-                    gender=entry.get("gender", None),
-                )
+            entries = db.get_entries(event_id=event.id)
+            entries_controlcard = [e for e in entries if e.chip == item["controlCard"]]
+            assigned_entries = [e for e in entries_controlcard if e.class_ is not None]
+            unassigned_entries = [e for e in entries_controlcard if e.class_ is None]
+
+            for entry in assigned_entries:
+                r = entry["result"]
+                if r is not None and r.same_punches(other=result):
+                    # result exists and is assigned to a competitor => nothing to do
+                    res = {
+                        "entryTime": item["entryTime"],
+                        "eventId": event.id,
+                        "controlCard": entry["chip"],
+                        "firstName": entry["first_name"],
+                        "lastName": entry["last_name"],
+                        "club": entry["club"],
+                        "class": entry["class_"],
+                        "status": r["status"],
+                        "time": r.extensions.get("running_time", r["time"]),
+                        "error": None,
+                        "missingControls": missing_controls(result=r),
+                    }
+                    break
+            else:
+                # check if result is already read out
+                unassigned_entry = None
+                for entry in unassigned_entries:
+                    if entry["result"].same_punches(other=result):
+                        unassigned_entry = entry
+                        break
 
-                # do not update another existing result
-                if not entry.result.has_punches():
+                # result can be assigned to an entry if
+                #   (1) there is exactly one entry without result
+                #   (2) there is no unassigned entry or one unassigned entry with same result
+                if (
+                    len(assigned_entries) == 1
+                    and not assigned_entries[0]["result"].has_punches()
+                    and (
+                        len(unassigned_entries) == 0
+                        or len(unassigned_entries) == 1
+                        and unassigned_entries[0]["result"].same_punches(other=result)
+                    )
+                ):
+                    entry = assigned_entries[0]
+                    try:
+                        class_ = db.get_class(id=entry["class_id"])[0]
+                        course_id = class_["course_id"]
+                        class_params = class_["params"]
+                        controls = db.get_course(id=course_id)[0]["controls"]
+                    except:
+                        class_params = ClassParams()
+                        controls = []
+
+                    result.compute_result(
+                        controls=controls,
+                        class_params=class_params,
+                        start_time=entry.start.start_time,
+                        year=int(entry.get("year", None))
+                        if entry.get("year", None) is not None
+                        else None,
+                        gender=entry.get("gender", None),
+                    )
                     db.update_entry_result(
                         id=entry["id"],
                         chip=entry["chip"],
                         result=result,
                         start_time=entry["start"].start_time,
                     )
                     res = {
@@ -660,100 +693,46 @@
                         "club": entry["club"],
                         "class": entry["class_"],
                         "status": result["status"],
                         "time": result.extensions.get("running_time", result["time"]),
                         "error": None,
                         "missingControls": missing_controls(result=result),
                     }
+
+                    # if there is an unassigned entry with the same result, delete it
+                    if unassigned_entries == [unassigned_entry]:
+                        db.delete_entry(id=unassigned_entry.id)
+
                 else:
-                    # do not create a new entry if an entry with same result already exist
-                    if entry.result == result:
-                        res = {
-                            "entryTime": item["entryTime"],
-                            "eventId": event.id,
-                            "controlCard": entry["chip"],
-                            "firstName": entry["first_name"],
-                            "lastName": entry["last_name"],
-                            "club": entry["club"],
-                            "class": entry["class_"],
-                            "status": result["status"],
-                            "time": result.extensions.get(
-                                "running_time", result["time"]
-                            ),
-                            "error": None,
-                            "missingControls": missing_controls(result=result),
-                        }
-                    else:
-                        result.status = ResultStatus.FINISHED
-                        result.compute_result(controls=[], class_params=ClassParams())
+                    # create a new unassigned entry
+                    result.compute_result(controls=[], class_params=ClassParams())
+                    if unassigned_entry is None:
                         db.add_entry_result(
                             event_id=event.id,
                             chip=item["controlCard"],
                             result=result,
                             start_time=None,
                         )
-                        res = {
-                            "entryTime": item["entryTime"],
-                            "eventId": event.id,
-                            "controlCard": item["controlCard"],
-                            "firstName": None,
-                            "lastName": None,
-                            "club": None,
-                            "class": None,
-                            "status": result["status"],
-                            "time": None,
-                            "error": "There is already a result",
-                        }
-
-            else:
-                result.compute_result(controls=[], class_params=ClassParams())
-                # do not create a new entry if an entry with same results already exist
-                for entry in [
-                    e
-                    for e in entries
-                    if e.class_id is None and e.chip == item["controlCard"]
-                ]:
-                    if entry.result == result:
-                        res = {
-                            "entryTime": item["entryTime"],
-                            "eventId": event.id,
-                            "controlCard": entry["chip"],
-                            "firstName": entry["first_name"],
-                            "lastName": entry["last_name"],
-                            "club": entry["club"],
-                            "class": entry["class_"],
-                            "status": result["status"],
-                            "time": result.extensions.get(
-                                "running_time", result["time"]
-                            ),
-                            "missingControls": missing_controls(result=result),
-                        }
-                        break
-                else:
-                    db.add_entry_result(
-                        event_id=event.id,
-                        chip=item["controlCard"],
-                        result=result,
-                        start_time=None,
-                    )
                     res = {
                         "entryTime": item["entryTime"],
                         "eventId": event.id,
                         "controlCard": item["controlCard"],
                         "firstName": None,
                         "lastName": None,
                         "club": None,
                         "class": None,
                         "status": result["status"],
                         "time": None,
                     }
-                if entries_controlcard == []:
-                    res["error"] = "Control card unknown"
-                else:
-                    res["error"] = "Control card assigned several times"
+                    if len(assigned_entries) == 0:
+                        res["error"] = "Control card unknown"
+                    elif len(assigned_entries) >= 2:
+                        res["error"] = "There are several entries for this card"
+                    else:
+                        res["error"] = "There are other results for this card"
 
         elif item["entryType"] == "cardInserted":
             res = {"eventId": event.id, "controlCard": item["controlCard"]}
         else:
             res = {"eventId": event.id}
 
     return item["entryType"], event, res
```

### Comparing `ooresults-0.2.3/ooresults/handler/results.py` & `ooresults-0.2.4/ooresults/handler/results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/handler/series.py` & `ooresults-0.2.4/ooresults/handler/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Bold.ttf` & `ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/pdf/fonts/Carlito-BoldItalic.ttf` & `ooresults-0.2.4/ooresults/pdf/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Italic.ttf` & `ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/pdf/fonts/Carlito-Regular.ttf` & `ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/pdf/pdf.py` & `ooresults-0.2.4/ooresults/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/pdf/result.py` & `ooresults-0.2.4/ooresults/pdf/result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/pdf/series.py` & `ooresults-0.2.4/ooresults/pdf/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/pdf/splittimes.py` & `ooresults-0.2.4/ooresults/pdf/splittimes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/__init__.py` & `ooresults-0.2.4/ooresults/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/imports/entries/__init__.py` & `ooresults-0.2.4/ooresults/plugins/imports/entries/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/imports/entries/text.py` & `ooresults-0.2.4/ooresults/plugins/imports/entries/text.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/iof_class_list.py` & `ooresults-0.2.4/ooresults/plugins/iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/iof_competitor_list.py` & `ooresults-0.2.4/ooresults/plugins/iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/iof_course_data.py` & `ooresults-0.2.4/ooresults/plugins/iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/iof_entry_list.py` & `ooresults-0.2.4/ooresults/plugins/iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/iof_result_list.py` & `ooresults-0.2.4/ooresults/plugins/iof_result_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/oe12.py` & `ooresults-0.2.4/ooresults/plugins/oe12.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/plugins/oe2003.py` & `ooresults-0.2.4/ooresults/plugins/oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/reader.py` & `ooresults-0.2.4/ooresults/reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/__init__.py` & `ooresults-0.2.4/ooresults/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/class_params.py` & `ooresults-0.2.4/ooresults/repo/class_params.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/repo.py` & `ooresults-0.2.4/ooresults/repo/repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/result_type.py` & `ooresults-0.2.4/ooresults/repo/result_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
+from __future__ import annotations
+
 import dataclasses
 from datetime import datetime
 import enum
 from typing import List
 from typing import Optional
 from typing import Dict
 
@@ -110,14 +112,30 @@
     def has_punches(self) -> bool:
         return (
             self.punched_start_time is not None
             or self.punched_finish_time is not None
             or [p for p in self.split_times if p.status != "Missing"] != []
         )
 
+    def same_punches(self, other: PersonRaceResult) -> bool:
+        return (
+            self.punched_start_time == other.punched_start_time
+            and self.punched_finish_time == other.punched_finish_time
+            and [
+                (p.control_code, p.punch_time)
+                for p in self.split_times
+                if p.status != "Missing"
+            ]
+            == [
+                (p.control_code, p.punch_time)
+                for p in other.split_times
+                if p.status != "Missing"
+            ]
+        )
+
     def voided_legs(self) -> List[str]:
         voided_legs = []
         c1 = "S"
         for split_time in [s for s in self.split_times if s.status != "Additional"]:
             c2 = split_time.control_code
             if split_time.leg_voided and f"{c1}-{c2}" not in voided_legs:
                 voided_legs.append(f"{c1}-{c2}")
```

### Comparing `ooresults-0.2.3/ooresults/repo/series_type.py` & `ooresults-0.2.4/ooresults/repo/series_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/sqlite_repo.py` & `ooresults-0.2.4/ooresults/repo/sqlite_repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/start_type.py` & `ooresults-0.2.4/ooresults/repo/start_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/update/__init__.py` & `ooresults-0.2.4/ooresults/repo/update/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/update/update_008.py` & `ooresults-0.2.4/ooresults/repo/update/update_008.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/repo/update/update_tables.py` & `ooresults-0.2.4/ooresults/repo/update/update_tables.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/schema/IOF.xsd` & `ooresults-0.2.4/ooresults/schema/IOF.xsd`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/schema/cardreader_log.json` & `ooresults-0.2.4/ooresults/schema/cardreader_log.json`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/server.py` & `ooresults-0.2.4/ooresults/server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/set_legacy_mode.py` & `ooresults-0.2.4/ooresults/set_legacy_mode.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/static/style-tab.css` & `ooresults-0.2.4/ooresults/static/style-tab.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/static/style.css` & `ooresults-0.2.4/ooresults/static/style.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/static/w3.js` & `ooresults-0.2.4/ooresults/static/w3.js`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/add_class.html` & `ooresults-0.2.4/ooresults/templates/add_class.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/add_club.html` & `ooresults-0.2.4/ooresults/templates/add_club.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/add_competitor.html` & `ooresults-0.2.4/ooresults/templates/add_competitor.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/add_course.html` & `ooresults-0.2.4/ooresults/templates/add_course.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/add_entry.html` & `ooresults-0.2.4/ooresults/templates/add_entry.html`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,17 @@
             </tr>
             <tr>
                 <th class="input-header"><label for="year">Year</label></th>
                 <td><input id="year" name="year" type="number" min="1900" max="2099"
                            value="$(str(entry.year) if entry.year is not None else '')" onchange="mark_label(this)"/></td>
             </tr>
             <tr>
+                $ readonly = "readonly" if [r for r in results if r['key'] == -1] else ""
                 <th class="input-header"><label for="chip">Chip</label></th>
-                <td><input id="chip" name="chip" type="text" value="$entry.chip" onchange="mark_label(this)"/></td>
+                <td><input id="chip" name="chip" type="text" value="$entry.chip" onchange="mark_label(this)" $readonly/></td>
             </tr>
             <tr>
                 <th class="input-header"><label for="club">Club</label></th>
                 <td>
                     <select id="club" name="club" onchange="mark_label(this)">
                     $if entry.club_id is None:
                         <option value="" selected></option>
@@ -86,19 +87,20 @@
             <tr>
                 <th class="input-header"><label for="start_time">Start time</label></th>
                 <td><input id="start_time" name="start_time" type="time" step="1" value="$(format_date(entry.start.get('start_time', None)))" onchange="mark_label(this)"/></td>
             </tr>
             <tr>
                 <th class="input-header"><label for="status">Status</label></th>
                 <td>
+                    $ has_no_result = [r for r in results if r['key'] == -1] == []
                     <select id="status" name="status" onchange="mark_label(this)">
                     $for status in list(ResultStatus):
                         $if status == entry.result.status:
                             <option value="$status.value" selected>$MAP_STATUS[status]</option>
-                        $else:
+                        $elif has_no_result or status not in (ResultStatus.INACTIVE, ResultStatus.DID_NOT_START):
                             <option value="$status.value">$MAP_STATUS[status]</option>
                     </select>
                 </td>
             </tr>
             $if results != []:
                 <tr>
                     <th class="input-header"><label for="result">Result</label></th>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 Last name *   [$entry.last_name    ]
               $for gender in ['', 'F', 'M']: $if str(gender) == str
               (entry.gender):
 Gender        $gender
               $else:
               $gender
 Year          [Unknown INPUT type]
-Chip          [$entry.chip         ]
+Chip          readonly/>
               $if entry.club_id is None:
               $else:
 Club          $for club in clubs: $if club.id == entry.club_id:
               $club.name
               $else:
               $club.name
               $for class_ in classes: $if class_.id == entry.class_id:
@@ -24,12 +24,13 @@
 $(fields[i])   name="$name" type="text" value="$entry.fields.get(i, '')"
               onchange="mark_label(this)"/>
 Not competing ('checked' if entry.not_competing else '')/>
 Start time    [Unknown INPUT type]
               $for status in list(ResultStatus): $if status ==
               entry.result.status:
 Status        $MAP_STATUS[status]
-              $else:
+              $elif has_no_result or status not in (ResultStatus.INACTIVE,
+              ResultStatus.DID_NOT_START):
               $MAP_STATUS[status]
 Result        $for r in results:
               $r['value']
 Save Cancel
```

### Comparing `ooresults-0.2.3/ooresults/templates/add_entry_competitors.html` & `ooresults-0.2.4/ooresults/templates/add_entry_competitors.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/add_entry_result.html` & `ooresults-0.2.4/ooresults/templates/add_entry_result.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/add_event.html` & `ooresults-0.2.4/ooresults/templates/add_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/classes_tab_content.html` & `ooresults-0.2.4/ooresults/templates/classes_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/classes_table.html` & `ooresults-0.2.4/ooresults/templates/classes_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/clubs_tab_content.html` & `ooresults-0.2.4/ooresults/templates/clubs_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/competitors_tab_content.html` & `ooresults-0.2.4/ooresults/templates/competitors_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/competitors_table.html` & `ooresults-0.2.4/ooresults/templates/competitors_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/courses_tab_content.html` & `ooresults-0.2.4/ooresults/templates/courses_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/courses_table.html` & `ooresults-0.2.4/ooresults/templates/courses_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/demo_reader.html` & `ooresults-0.2.4/ooresults/templates/demo_reader.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/entries_tab_content.html` & `ooresults-0.2.4/ooresults/templates/entries_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/entries_table.html` & `ooresults-0.2.4/ooresults/templates/entries_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/events_tab_content.html` & `ooresults-0.2.4/ooresults/templates/events_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/events_table.html` & `ooresults-0.2.4/ooresults/templates/events_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/main.html` & `ooresults-0.2.4/ooresults/templates/main.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/results_tab_content.html` & `ooresults-0.2.4/ooresults/templates/results_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/results_table.html` & `ooresults-0.2.4/ooresults/templates/results_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/root.html` & `ooresults-0.2.4/ooresults/templates/root.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/select_event.html` & `ooresults-0.2.4/ooresults/templates/select_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/series_settings.html` & `ooresults-0.2.4/ooresults/templates/series_settings.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/series_tab_content.html` & `ooresults-0.2.4/ooresults/templates/series_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/series_table.html` & `ooresults-0.2.4/ooresults/templates/series_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/si/si1_data.html` & `ooresults-0.2.4/ooresults/templates/si/si1_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/si/si1_page.html` & `ooresults-0.2.4/ooresults/templates/si/si1_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/si/si2_data.html` & `ooresults-0.2.4/ooresults/templates/si/si2_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/templates/si/si2_page.html` & `ooresults-0.2.4/ooresults/templates/si/si2_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/user.py` & `ooresults-0.2.4/ooresults/user.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/utils/__init__.py` & `ooresults-0.2.4/ooresults/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/utils/globals.py` & `ooresults-0.2.4/ooresults/utils/globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/websocket_server/__init__.py` & `ooresults-0.2.4/ooresults/websocket_server/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/websocket_server/si.py` & `ooresults-0.2.4/ooresults/websocket_server/si.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/websocket_server/websocket_handler.py` & `ooresults-0.2.4/ooresults/websocket_server/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults/websocket_server/websocket_server.py` & `ooresults-0.2.4/ooresults/websocket_server/websocket_server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/ooresults.egg-info/PKG-INFO` & `ooresults-0.2.4/ooresults.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.3
+Version: 0.2.4
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooresults-0.2.3/ooresults.egg-info/SOURCES.txt` & `ooresults-0.2.4/ooresults.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/pyproject.toml` & `ooresults-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ooresults"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   {name="Rainer Garus"},
 ]
 description = "A software for the evaluation of the results of orienteering events"
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
```

### Comparing `ooresults-0.2.3/setup.cfg` & `ooresults-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/__init__.py` & `ooresults-0.2.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/competitor.py` & `ooresults-0.2.4/tests/competitor.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/entry.py` & `ooresults-0.2.4/tests/entry.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/model/__init__.py` & `ooresults-0.2.4/tests/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/model/test_build_series_result.py` & `ooresults-0.2.4/tests/model/test_build_series_result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/model/test_courses.py` & `ooresults-0.2.4/tests/model/test_courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/model/test_event_class_results.py` & `ooresults-0.2.4/tests/model/test_event_class_results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/model/test_parse_cardreader_log.py` & `ooresults-0.2.4/tests/model/test_parse_cardreader_log.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/model/test_store_cardreader_result.py` & `ooresults-0.2.4/tests/model/test_store_cardreader_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -156,14 +156,44 @@
         start_time=None,
     )
     entry = db.get_entry(id=id)[0]
     return copy.deepcopy(entry)
 
 
 @pytest.fixture
+def entry_2_with_result(db, event_id, class_id, entry_2):
+    db.update_entry_result(
+        id=entry_2["id"],
+        chip=entry_2["chip"],
+        start_time=entry_2["start"].start_time,
+        result=PersonRaceResult(
+            status=ResultStatus.OK,
+            start_time=s1,
+            finish_time=f1,
+            punched_start_time=s1,
+            punched_finish_time=f1,
+            time=t(s1, f1),
+            split_times=[
+                SplitTime(
+                    control_code="101", punch_time=c1, time=t(s1, c1), status="OK"
+                ),
+                SplitTime(
+                    control_code="102", punch_time=c2, time=t(s1, c2), status="OK"
+                ),
+                SplitTime(
+                    control_code="103", punch_time=c3, time=t(s1, c3), status="OK"
+                ),
+            ],
+        ),
+    )
+    entry = db.get_entry(id=entry_2["id"])[0]
+    return copy.deepcopy(entry)
+
+
+@pytest.fixture
 def entry_3(db, event_id, class_id):
     id = db.add_entry(
         event_id=event_id,
         competitor_id=None,
         first_name="Angela",
         last_name="Merkel",
         gender="F",
@@ -177,53 +207,31 @@
         start_time=None,
     )
     entry = db.get_entry(id=id)[0]
     return copy.deepcopy(entry)
 
 
 @pytest.fixture
-def entry_4(db, event_id, class_id):
-    id = db.add_entry(
-        event_id=event_id,
-        competitor_id=None,
-        first_name="Yogi",
-        last_name="Löw",
-        gender="N",
-        year=None,
-        class_id=class_id,
-        club_id=None,
-        not_competing=False,
-        chip="7410",
-        fields={},
-        status=ResultStatus.INACTIVE,
-        start_time=None,
+def unassigned_entry(db, event_id):
+    result = PersonRaceResult(
+        status=ResultStatus.FINISHED,
+        punched_start_time=s1,
+        punched_finish_time=f1,
+        time=None,
+        split_times=[
+            SplitTime(control_code="101", punch_time=c1, status="Additional"),
+            SplitTime(control_code="102", punch_time=c2, status="Additional"),
+            SplitTime(control_code="103", punch_time=c3, status="Additional"),
+        ],
     )
-    db.update_entry_result(
-        id=id,
+    id = db.add_entry_result(
+        event_id=event_id,
         chip="7410",
+        result=result,
         start_time=None,
-        result=PersonRaceResult(
-            status=ResultStatus.OK,
-            start_time=s1,
-            finish_time=f1,
-            punched_start_time=s1,
-            punched_finish_time=f1,
-            time=t(s1, f1),
-            split_times=[
-                SplitTime(
-                    control_code="101", punch_time=c1, time=t(s1, c1), status="OK"
-                ),
-                SplitTime(
-                    control_code="102", punch_time=c2, time=t(s1, c2), status="OK"
-                ),
-                SplitTime(
-                    control_code="103", punch_time=c3, time=t(s1, c3), status="OK"
-                ),
-            ],
-        ),
     )
     entry = db.get_entry(id=id)[0]
     return copy.deepcopy(entry)
 
 
 def assert_entries_are_equal(entry_a: Dict, entry_b: Dict) -> None:
     assert entry_a["id"] == entry_b["id"]
@@ -241,15 +249,15 @@
     assert entry_a["club_id"] == entry_b["club_id"]
     assert entry_a["club"] == entry_b["club"]
     assert entry_a["class_id"] == entry_b["class_id"]
     assert entry_a["class_"] == entry_b["class_"]
     assert entry_a.get("missingControls", None) == entry_b.get("missingControls", None)
 
 
-def test_store_cardreader_result_if_cardnumber_is_unique(
+def test_assign_to_entry_if_cardnumber_is_unique(
     db, event_id, entry_1, entry_2, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=f1,
         time=None,
@@ -302,15 +310,15 @@
     )
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=entry_1)
     assert_entries_are_equal(entry_a=entries[1], entry_b=entry_2)
     assert_entries_are_equal(entry_a=entries[2], entry_b=entry_3)
 
 
-def test_store_cardreader_result_if_cardnumber_is_unique_but_finish_time_is_missing(
+def test_assign_to_entry_if_cardnumber_is_unique_but_finish_time_is_missing(
     db, event_id, entry_1, entry_2, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=None,
         time=None,
@@ -363,15 +371,15 @@
     )
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=entry_1)
     assert_entries_are_equal(entry_a=entries[1], entry_b=entry_2)
     assert_entries_are_equal(entry_a=entries[2], entry_b=entry_3)
 
 
-def test_store_cardreader_result_if_cardnumber_is_unique_but_start_time_is_missing(
+def test_assign_to_entry_if_cardnumber_is_unique_but_start_time_is_missing(
     db, event_id, entry_1, entry_2, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=None,
         punched_finish_time=f1,
         time=None,
@@ -424,15 +432,15 @@
     )
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=entry_1)
     assert_entries_are_equal(entry_a=entries[1], entry_b=entry_2)
     assert_entries_are_equal(entry_a=entries[2], entry_b=entry_3)
 
 
-def test_store_cardreader_result_if_cardnumber_is_unique_but_controls_are_missing(
+def test_assign_to_entry_if_cardnumber_is_unique_but_controls_are_missing(
     db, event_id, entry_1, entry_2, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=f1,
         time=None,
@@ -483,15 +491,210 @@
     )
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=entry_1)
     assert_entries_are_equal(entry_a=entries[1], entry_b=entry_2)
     assert_entries_are_equal(entry_a=entries[2], entry_b=entry_3)
 
 
-def test_store_cardreader_result_if_cardnumber_is_unknown(
+def test_assign_to_entry_and_delete_unnamed_entry_with_same_result(
+    db, event_id, entry_1, entry_2, entry_3, unassigned_entry
+):
+    result = PersonRaceResult(
+        status=ResultStatus.FINISHED,
+        punched_start_time=s1,
+        punched_finish_time=f1,
+        time=None,
+        split_times=[
+            SplitTime(control_code="101", punch_time=c1, status="Additional"),
+            SplitTime(control_code="102", punch_time=c2, status="Additional"),
+            SplitTime(control_code="103", punch_time=c3, status="Additional"),
+        ],
+    )
+    item = {
+        "entryType": "cardRead",
+        "entryTime": entry_time,
+        "controlCard": "7410",
+        "result": result,
+    }
+
+    status, event, res = model.store_cardreader_result(event_key="4711", item=item)
+    print(res)
+
+    assert status == "cardRead"
+    assert event["id"] == event_id
+    assert res == {
+        "entryTime": entry_time,
+        "eventId": event_id,
+        "controlCard": "7410",
+        "firstName": "Yogi",
+        "lastName": "Löw",
+        "club": None,
+        "class": "Elite",
+        "status": ResultStatus.OK,
+        "time": t(s1, f1),
+        "error": None,
+        "missingControls": [],
+    }
+
+    entries = db.get_entries(event_id=event_id)
+    assert len(entries) == 3
+
+    entry_2["result"] = PersonRaceResult(
+        status=ResultStatus.OK,
+        start_time=s1,
+        finish_time=f1,
+        punched_start_time=s1,
+        punched_finish_time=f1,
+        time=t(s1, f1),
+        split_times=[
+            SplitTime(control_code="101", punch_time=c1, time=t(s1, c1), status="OK"),
+            SplitTime(control_code="102", punch_time=c2, time=t(s1, c2), status="OK"),
+            SplitTime(control_code="103", punch_time=c3, time=t(s1, c3), status="OK"),
+        ],
+    )
+
+    assert_entries_are_equal(entry_a=entries[0], entry_b=entry_1)
+    assert_entries_are_equal(entry_a=entries[1], entry_b=entry_2)
+    assert_entries_are_equal(entry_a=entries[2], entry_b=entry_3)
+
+
+def test_store_as_new_entry_if_another_result_exists(
+    db, event_id, entry_1, entry_2, entry_3, unassigned_entry
+):
+    result = PersonRaceResult(
+        status=ResultStatus.FINISHED,
+        punched_start_time=s1,
+        punched_finish_time=f1,
+        time=None,
+        split_times=[
+            SplitTime(control_code="101", punch_time=c1, status="Additional"),
+            SplitTime(control_code="103", punch_time=c3, status="Additional"),
+        ],
+    )
+    item = {
+        "entryType": "cardRead",
+        "entryTime": entry_time,
+        "controlCard": "7410",
+        "result": result,
+    }
+
+    status, event, res = model.store_cardreader_result(event_key="4711", item=item)
+
+    assert status == "cardRead"
+    assert event["id"] == event_id
+    assert res == {
+        "entryTime": entry_time,
+        "eventId": event_id,
+        "controlCard": "7410",
+        "firstName": None,
+        "lastName": None,
+        "club": None,
+        "class": None,
+        "status": ResultStatus.FINISHED,
+        "time": None,
+        "error": "There are other results for this card",
+    }
+
+    entries = db.get_entries(event_id=event_id)
+    assert len(entries) == 5
+
+    result = PersonRaceResult(
+        status=ResultStatus.FINISHED,
+        start_time=s1,
+        finish_time=f1,
+        punched_start_time=s1,
+        punched_finish_time=f1,
+        time=t(s1, f1),
+        split_times=[
+            SplitTime(
+                control_code="101", punch_time=c1, time=t(s1, c1), status="Additional"
+            ),
+            SplitTime(
+                control_code="103", punch_time=c3, time=t(s1, c3), status="Additional"
+            ),
+        ],
+    )
+    new_entry = {
+        "id": [
+            e["id"]
+            for e in entries
+            if e["id"]
+            not in [entry_1["id"], entry_2["id"], entry_3["id"], unassigned_entry["id"]]
+        ][0],
+        "event_id": event_id,
+        "first_name": None,
+        "last_name": None,
+        "gender": None,
+        "year": None,
+        "competitor_id": None,
+        "not_competing": False,
+        "chip": "7410",
+        "fields": {},
+        "result": result,
+        "start": PersonRaceStart(),
+        "club_id": None,
+        "club": None,
+        "class_id": None,
+        "class_": None,
+    }
+
+    assert_entries_are_equal(entry_a=entries[0], entry_b=unassigned_entry)
+    assert_entries_are_equal(entry_a=entries[1], entry_b=new_entry)
+    assert_entries_are_equal(entry_a=entries[2], entry_b=entry_1)
+    assert_entries_are_equal(entry_a=entries[3], entry_b=entry_2)
+    assert_entries_are_equal(entry_a=entries[4], entry_b=entry_3)
+
+
+def test_do_not_store_as_new_entry_if_result_already_exists(
+    db, event_id, entry_1, entry_3, unassigned_entry
+):
+    result = PersonRaceResult(
+        status=ResultStatus.FINISHED,
+        punched_start_time=s1,
+        punched_finish_time=f1,
+        time=None,
+        split_times=[
+            SplitTime(control_code="101", punch_time=c1, status="Additional"),
+            SplitTime(control_code="102", punch_time=c2, status="Additional"),
+            SplitTime(control_code="103", punch_time=c3, status="Additional"),
+        ],
+    )
+    item = {
+        "entryType": "cardRead",
+        "entryTime": entry_time,
+        "controlCard": "7410",
+        "result": result,
+    }
+
+    status, event, res = model.store_cardreader_result(event_key="4711", item=item)
+
+    assert status == "cardRead"
+    assert event["id"] == event_id
+    assert res == {
+        "entryTime": entry_time,
+        "eventId": event_id,
+        "controlCard": "7410",
+        "firstName": None,
+        "lastName": None,
+        "club": None,
+        "class": None,
+        "status": ResultStatus.FINISHED,
+        "time": None,
+        "error": "Control card unknown",
+    }
+
+    entries = db.get_entries(event_id=event_id)
+    assert len(entries) == 3
+
+    assert_entries_are_equal(entry_a=entries[0], entry_b=unassigned_entry)
+    assert_entries_are_equal(entry_a=entries[1], entry_b=entry_1)
+    assert_entries_are_equal(entry_a=entries[2], entry_b=entry_3)
+
+
+def test_store_as_new_entry_if_cardnumber_is_unknown(
     db, event_id, entry_1, entry_2, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=f1,
         time=None,
@@ -572,15 +775,15 @@
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=new_entry)
     assert_entries_are_equal(entry_a=entries[1], entry_b=entry_1)
     assert_entries_are_equal(entry_a=entries[2], entry_b=entry_2)
     assert_entries_are_equal(entry_a=entries[3], entry_b=entry_3)
 
 
-def test_store_cardreader_result_if_cardnumber_exist_several_times(
+def test_store_as_new_entry_if_cardnumber_exist_several_times(
     db, event_id, entry_1, entry_2, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=f1,
         time=None,
@@ -607,15 +810,15 @@
         "controlCard": "12734",
         "firstName": None,
         "lastName": None,
         "club": None,
         "class": None,
         "status": ResultStatus.FINISHED,
         "time": None,
-        "error": "Control card assigned several times",
+        "error": "There are several entries for this card",
     }
 
     entries = db.get_entries(event_id=event_id)
     assert len(entries) == 4
 
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
@@ -661,16 +864,16 @@
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=new_entry)
     assert_entries_are_equal(entry_a=entries[1], entry_b=entry_1)
     assert_entries_are_equal(entry_a=entries[2], entry_b=entry_2)
     assert_entries_are_equal(entry_a=entries[3], entry_b=entry_3)
 
 
-def test_store_cardreader_result_if_cardnumer_is_unique_with_same_result(
-    db, event_id, entry_1, entry_4, entry_3
+def test_use_already_assigned_entry_if_it_has_the_same_result(
+    db, event_id, entry_1, entry_2_with_result, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=f1,
         time=None,
         split_times=[
@@ -704,20 +907,20 @@
         "missingControls": [],
     }
 
     entries = db.get_entries(event_id=event_id)
     assert len(entries) == 3
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=entry_1)
-    assert_entries_are_equal(entry_a=entries[1], entry_b=entry_4)
+    assert_entries_are_equal(entry_a=entries[1], entry_b=entry_2_with_result)
     assert_entries_are_equal(entry_a=entries[2], entry_b=entry_3)
 
 
-def test_store_cardreader_result_if_cardnumber_is_unique_with_another_result(
-    db, event_id, entry_1, entry_4, entry_3
+def test_store_as_new_entry_if_cardnumber_is_unique_with_another_result(
+    db, event_id, entry_1, entry_2_with_result, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=f1,
         time=None,
         split_times=[
@@ -743,15 +946,15 @@
         "controlCard": "7410",
         "firstName": None,
         "lastName": None,
         "club": None,
         "class": None,
         "status": ResultStatus.FINISHED,
         "time": None,
-        "error": "There is already a result",
+        "error": "There are other results for this card",
     }
 
     entries = db.get_entries(event_id=event_id)
     assert len(entries) == 4
 
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
@@ -772,15 +975,15 @@
             ),
         ],
     )
     new_entry = {
         "id": [
             e["id"]
             for e in entries
-            if e["id"] not in [entry_1["id"], entry_4["id"], entry_3["id"]]
+            if e["id"] not in [entry_1["id"], entry_2_with_result["id"], entry_3["id"]]
         ][0],
         "event_id": event_id,
         "first_name": None,
         "last_name": None,
         "gender": None,
         "year": None,
         "competitor_id": None,
@@ -793,19 +996,19 @@
         "club": None,
         "class_id": None,
         "class_": None,
     }
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=new_entry)
     assert_entries_are_equal(entry_a=entries[1], entry_b=entry_1)
-    assert_entries_are_equal(entry_a=entries[2], entry_b=entry_4)
+    assert_entries_are_equal(entry_a=entries[2], entry_b=entry_2_with_result)
     assert_entries_are_equal(entry_a=entries[3], entry_b=entry_3)
 
 
-def test_store_cardreader_result_use_empty_control_list_if_course_is_undefined(
+def test_use_empty_control_list_if_course_is_undefined(
     db, event_id, entry_1_without_course
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=f1,
         time=None,
@@ -862,15 +1065,15 @@
             ),
         ],
     )
 
     assert_entries_are_equal(entry_a=entries[0], entry_b=entry_1_without_course)
 
 
-def test_store_cardreader_result_exception_if_eventkey_is_unknown(
+def test_raise_exception_if_event_key_is_unknown(
     db, event_id, entry_1, entry_2, entry_3
 ):
     result = PersonRaceResult(
         status=ResultStatus.FINISHED,
         punched_start_time=s1,
         punched_finish_time=f1,
         time=None,
```

### Comparing `ooresults-0.2.3/tests/plugins/test_export_competitors_oe2003.py` & `ooresults-0.2.4/tests/plugins/test_export_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/plugins/test_import_competitors_oe2003.py` & `ooresults-0.2.4/tests/plugins/test_import_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/plugins/test_plugin_iof_class_list.py` & `ooresults-0.2.4/tests/plugins/test_plugin_iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/plugins/test_plugin_iof_competitor_list.py` & `ooresults-0.2.4/tests/plugins/test_plugin_iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/plugins/test_plugin_iof_course_data.py` & `ooresults-0.2.4/tests/plugins/test_plugin_iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/plugins/test_plugin_iof_entry_list.py` & `ooresults-0.2.4/tests/plugins/test_plugin_iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/plugins/test_plugin_iof_result_list.py` & `ooresults-0.2.4/tests/plugins/test_plugin_iof_result_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/repo/__init__.py` & `ooresults-0.2.4/tests/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/repo/test_classes.py` & `ooresults-0.2.4/tests/repo/test_classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/repo/test_clubs.py` & `ooresults-0.2.4/tests/repo/test_clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/repo/test_competitors.py` & `ooresults-0.2.4/tests/repo/test_competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/repo/test_courses.py` & `ooresults-0.2.4/tests/repo/test_courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/repo/test_entries.py` & `ooresults-0.2.4/tests/repo/test_entries.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/repo/test_events.py` & `ooresults-0.2.4/tests/repo/test_events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/repo/test_settings.py` & `ooresults-0.2.4/tests/repo/test_settings.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_compute_result_net.py` & `ooresults-0.2.4/tests/test_compute_result_net.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_compute_result_score.py` & `ooresults-0.2.4/tests/test_compute_result_score.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_compute_result_standard.py` & `ooresults-0.2.4/tests/test_compute_result_standard.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_configuration.py` & `ooresults-0.2.4/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_globals.py` & `ooresults-0.2.4/tests/test_globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_handicap.py` & `ooresults-0.2.4/tests/test_handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_ranking.py` & `ooresults-0.2.4/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_series.py` & `ooresults-0.2.4/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.3/tests/test_user.py` & `ooresults-0.2.4/tests/test_user.py`

 * *Files identical despite different names*

