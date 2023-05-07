# Comparing `tmp/osxphotos-0.59.3.tar.gz` & `tmp/osxphotos-0.60.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.59.3.tar", last modified: Tue Apr 11 02:05:45 2023, max compression
+gzip compressed data, was "osxphotos-0.60.0.tar", last modified: Sun May  7 14:48:43 2023, max compression
```

## Comparing `osxphotos-0.59.3.tar` & `osxphotos-0.60.0.tar`

### file list

```diff
@@ -1,231 +1,232 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.052886 osxphotos-0.59.3/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.59.3/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.59.3/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-11 02:05:45.052663 osxphotos-0.59.3/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   223845 2023-04-11 02:05:33.000000 osxphotos-0.59.3/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.59.3/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:44.999197 osxphotos-0.59.3/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1850 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.59.3/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15928 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-04-11 02:05:26.000000 osxphotos-0.59.3/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.59.3/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.010712 osxphotos-0.59.3/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3482 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.59.3/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6838 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9875 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3628 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    26501 2023-04-08 21:34:18.000000 osxphotos-0.59.3/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8517 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.59.3/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      433 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3457 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   106667 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    21765 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61618 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.59.3/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9663 2023-04-08 20:57:19.000000 osxphotos-0.59.3/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20532 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5361 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     7033 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23014 2023-04-10 18:30:56.000000 osxphotos-0.59.3/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.59.3/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3324 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26903 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.59.3/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28013 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.59.3/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      633 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.59.3/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5058 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.59.3/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-03-24 13:39:33.000000 osxphotos-0.59.3/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.011189 osxphotos-0.59.3/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.59.3/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1466350 2023-04-11 02:05:41.000000 osxphotos-0.59.3/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.59.3/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.59.3/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.59.3/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51732 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10002 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5048 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.59.3/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2906 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    88952 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    80371 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46166 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     5511 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5283 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.013615 osxphotos-0.59.3/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.59.3/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10370 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149077 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.59.3/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-04-11 02:05:33.000000 osxphotos-0.59.3/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78831 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.59.3/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21857 2023-03-24 13:39:33.000000 osxphotos-0.59.3/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.59.3/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.014494 osxphotos-0.59.3/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.59.3/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.59.3/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.59.3/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.59.3/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.59.3/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.59.3/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-03-24 13:39:33.000000 osxphotos-0.59.3/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.015090 osxphotos-0.59.3/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.59.3/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3201 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.59.3/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1682 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)    27026 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    18282 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:44.999936 osxphotos-0.59.3/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6319 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-04-11 02:05:45.052923 osxphotos-0.59.3/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.59.3/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.051583 osxphotos-0.59.3/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.052296 osxphotos-0.59.3/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.59.3/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.59.3/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.59.3/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.59.3/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.59.3/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54621 2023-04-11 02:03:56.000000 osxphotos-0.59.3/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   269538 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1693 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4469 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2125 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6692 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.59.3/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.59.3/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    29889 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.59.3/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3345 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.59.3/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.59.3/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.59.3/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1931 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.59.3/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.59.3/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.59.3/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18530 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.59.3/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.59.3/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5864 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.59.3/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.59.3/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.59.3/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.59.3/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5059 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.59.3/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.59.3/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.59.3/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.59.3/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.59.3/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.59.3/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18366 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.59.3/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50347 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.59.3/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.59.3/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13297 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.59.3/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.59.3/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.59.3/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.59.3/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.59.3/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.59.3/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.59.3/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.59.3/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.59.3/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.59.3/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.59.3/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.59.3/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.59.3/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.59.3/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.59.3/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    49786 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2324 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     1867 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    47877 2023-04-11 02:03:56.000000 osxphotos-0.59.3/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.569779 osxphotos-0.60.0/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.0/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.0/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-05-07 14:48:43.569088 osxphotos-0.60.0/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   224064 2023-05-07 14:48:33.000000 osxphotos-0.60.0/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.0/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.507659 osxphotos-0.60.0/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.0/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15945 2023-05-07 14:44:48.000000 osxphotos-0.60.0/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-05-07 14:38:45.000000 osxphotos-0.60.0/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.0/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.0/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.527845 osxphotos-0.60.0/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.0/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26594 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.0/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      713 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   106908 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.0/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7833 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.0/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.0/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.0/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.60.0/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.0/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.528403 osxphotos-0.60.0/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.0/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1459529 2023-05-07 14:48:39.000000 osxphotos-0.60.0/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.0/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.0/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.0/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51732 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.0/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    89066 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    80700 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5542 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.535350 osxphotos-0.60.0/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.60.0/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149146 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.0/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.0/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-05-07 14:48:32.000000 osxphotos-0.60.0/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.0/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.0/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.537111 osxphotos-0.60.0/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.0/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.0/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.0/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.0/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.0/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.0/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.538126 osxphotos-0.60.0/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.0/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.60.0/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.510165 osxphotos-0.60.0/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6344 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-05-07 14:48:43.569822 osxphotos-0.60.0/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.0/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.567919 osxphotos-0.60.0/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.568686 osxphotos-0.60.0/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.0/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.0/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.60.0/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.60.0/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.60.0/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-05-07 14:25:27.000000 osxphotos-0.60.0/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.0/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.0/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.60.0/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.0/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.0/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.0/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.0/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.60.0/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.60.0/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.0/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.60.0/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.60.0/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.0/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.60.0/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.60.0/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.60.0/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.60.0/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.0/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.60.0/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.0/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.60.0/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.60.0/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.0/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.60.0/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.60.0/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.60.0/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.60.0/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.0/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.0/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.0/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.0/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.60.0/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.60.0/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.60.0/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.60.0/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.60.0/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.0/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.60.0/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.0/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.0/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.0/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.0/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.0/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.59.3/LICENSE` & `osxphotos-0.60.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/PKG-INFO` & `osxphotos-0.60.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.59.3
+Version: 0.60.0
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.59.3/README.md` & `osxphotos-0.60.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osxphotos)
 [![Downloads](https://static.pepy.tech/personalized-badge/osxphotos?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/osxphotos)
 [![subreddit](https://img.shields.io/reddit/subreddit-subscribers/osxphotos?style=social)](https://www.reddit.com/r/osxphotos/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-59-orange.svg?style=flat)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
-OSXPhotos provides the ability to interact with and query Apple's Photos.app library on macOS. You can query the Photos library database — for example, file name, file path, and metadata such as keywords/tags, persons/faces, albums, etc. You can also easily export both the original and edited photos.
+OSXPhotos provides the ability to interact with and query Apple's Photos.app library on macOS and Linux. You can query the Photos library database — for example, file name, file path, and metadata such as keywords/tags, persons/faces, albums, etc. You can also easily export both the original and edited photos.
 
 <p align="center"><img src="docs/screencast/demo.gif?raw=true" width="713" height="430"/></p>
 
 # Table of Contents
 
 * [Supported operating systems](#supported-operating-systems)
 * [Installation](#installation)
@@ -29,28 +29,32 @@
 * [Contributing](#contributing)
 * [Known Bugs and Limitations](#known-bugs-and-limitations)
 * [Implementation Notes](#implementation-notes)
 * [Acknowledgements](#acknowledgements)
 
 ## Supported operating systems
 
-Only works on macOS (aka Mac OS X). Tested on macOS Sierra (10.12.6) through macOS Monterey (12.0.1).  Tested on both x86 and Apple silicon (M1).
+Tested on Ubuntu Linux and macOS. Many features are only available on macOS.
+
+On Linux, macOS-specific features of the CLI will not be available (these will not be shown in the help output).
+The export and query CLI commands as well as the Python API will work on Linux which enables you to export photos
+from a Photos library on a Linux machine.
+
+Tested on macOS Sierra (10.12.6) through macOS Ventura (13.3). Tested on both x86 and Apple silicon (M1).
 
 | macOS Version     | macOS name | Photos.app version |
 | ----------------- |------------|:-------------------|
-| 13.0              | Ventura    | 8.0 ✅ *           |
-| 12.0 - 12.6       | Monterey   | 7.0 ✅ *           |
+| 13.0 - 13.3       | Ventura    | 8.0 ✅             |
+| 12.0 - 12.6       | Monterey   | 7.0 ✅             |
 | 10.16, 11.0-11.4  | Big Sur    | 6.0 ✅             |
 | 10.15.1 - 10.15.7 | Catalina   | 5.0 ✅             |
 | 10.14.5, 10.14.6  | Mojave     | 4.0 ✅             |
 | 10.13.6           | High Sierra| 3.0 ✅             |
 | 10.12.6           | Sierra     | 2.0 ✅             |
 
-\* Some features may not be fully supported on Monterey and Ventura. Notably, `--use-photokit` and `--download-missing` may or may not work depending on your configuration; this is a known issue that will be fixed if I can find a solution.  Many users successfully use OSXPhotos on Monterey without problem.
-
 This package will read Photos databases for any supported version on any supported macOS version.  E.g. you can read a database created with Photos 5.0 on MacOS 10.15 on a machine running macOS 10.12 and vice versa.
 
 Requires python >= `3.9`.
 
 ## Installation
 
 If you are new to python, I recommend you to install using pipx. See other advanced options below.
@@ -1436,30 +1440,31 @@
 for updating the library. You can always run export without the --update
 option to re-export the entire library thus rebuilding the
 '.osxphotos_export.db' database.
 
 
                              Extended Attributes                              
 
-Some options (currently '--finder-tag-template', '--finder-tag-keywords',
-'-xattr-template') write additional metadata accessible by Spotlight to
-facilitate searching.  For example, --finder-tag-keyword writes all keywords
-(including any specified by '--keyword-template' or other options) to Finder
-tags that are searchable in Spotlight using the syntax: 'tag:tagname'. For
-example, if you have images with keyword "Travel" then using '--finder-tag-
-keywords' you could quickly find those images in the Finder by typing
-'tag:Travel' in the Spotlight search bar. Finder tags are written to the
-'com.apple.metadata:_kMDItemUserTags' extended attribute. Unlike EXIF
-metadata, extended attributes do not modify the actual file; the metadata is
-written to extended attributes associated with the file and the Spotlight
-metadata database.  Most cloud storage services do not synch extended
-attributes.  Dropbox does sync them and any changes to a file's extended
-attributes will cause Dropbox to re-sync the files.
+    Some options (currently '--finder-tag-template', '--finder-tag-keywords',
+    '-xattr-template') write     additional metadata accessible by Spotlight
+    to facilitate searching.      For example, --finder-tag-keyword writes all
+    keywords (including any specified by '--keyword-template'     or other
+    options) to Finder tags that are searchable in Spotlight using the syntax:
+    'tag:tagname'.     For example, if you have images with keyword "Travel"
+    then using '--finder-tag-keywords' you could quickly     find those images
+    in the Finder by typing 'tag:Travel' in the Spotlight search bar.
+    Finder tags are written to the 'com.apple.metadata:_kMDItemUserTags'
+    extended attribute.     Unlike EXIF metadata, extended attributes do not
+    modify the actual file;     the metadata is written to extended attributes
+    associated with the file and the Spotlight metadata database.      Most
+    cloud storage services do not synch extended attributes.      Dropbox does
+    sync them and any changes to a file's extended attributes     will cause
+    Dropbox to re-sync the files.
 
-The following attributes may be used with '--xattr-template':
+    The following attributes may be used with '--xattr-template':
 
 
 Attribute      Description
 authors        kMDItemAuthors; com.apple.metadata:kMDItemAuthors; The
                author, or authors, of the contents of the file.; list of
                strings
 comment        kMDItemComment; com.apple.metadata:kMDItemComment; A comment
@@ -2090,15 +2095,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.59.3'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.0'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2577,15 +2582,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.59.3'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.0'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
@@ -2697,15 +2702,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://eecue.com/"><img src="https://avatars.githubusercontent.com/u/532536?v=4?s=75" width="75px;" alt="Dave Bullock"/><br /><sub><b>Dave Bullock</b></sub></a><br /><a href="#ideas-eecue" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-eecue" title="User Testing">📓</a> <a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aeecue" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pweaver"><img src="https://avatars.githubusercontent.com/u/611620?v=4?s=75" width="75px;" alt="Pweaver"/><br /><sub><b>Pweaver</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Apweaver" title="Bug reports">🐛</a> <a href="#ideas-pweaver" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aa599"><img src="https://avatars.githubusercontent.com/u/37746269?v=4?s=75" width="75px;" alt="aa599"/><br /><sub><b>aa599</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aaa599" title="Bug reports">🐛</a> <a href="#ideas-aa599" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/swduncan"><img src="https://avatars.githubusercontent.com/u/2053195?v=4?s=75" width="75px;" alt="Steve Duncan"/><br /><sub><b>Steve Duncan</b></sub></a><br /><a href="#ideas-swduncan" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.projany.com"><img src="https://avatars.githubusercontent.com/u/15144745?v=4?s=75" width="75px;" alt="Ian Moir"/><br /><sub><b>Ian Moir</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aianmmoir" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pekingduck"><img src="https://avatars.githubusercontent.com/u/2597142?v=4?s=75" width="75px;" alt="Peking Duck"/><br /><sub><b>Peking Duck</b></sub></a><br /><a href="#ideas-pekingduck" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pekingduck"><img src="https://avatars.githubusercontent.com/u/2597142?v=4?s=75" width="75px;" alt="Peking Duck"/><br /><sub><b>Peking Duck</b></sub></a><br /><a href="#ideas-pekingduck" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Apekingduck" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.patreon.com/cclauss"><img src="https://avatars.githubusercontent.com/u/3709715?v=4?s=75" width="75px;" alt="Christian Clauss"/><br /><sub><b>Christian Clauss</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=cclauss" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dvdkon"><img src="https://avatars.githubusercontent.com/u/3526303?v=4?s=75" width="75px;" alt="dvdkon"/><br /><sub><b>dvdkon</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=dvdkon" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/wernerzj"><img src="https://avatars.githubusercontent.com/u/130370930?v=4?s=75" width="75px;" alt="wernerzj"/><br /><sub><b>wernerzj</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Awernerzj" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/rajscode"><img src="https://avatars.githubusercontent.com/u/99123253?v=4?s=75" width="75px;" alt="rajscode"/><br /><sub><b>rajscode</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Arajscode" title="Bug reports">🐛</a></td>
     </tr>
```

### Comparing `osxphotos-0.59.3/README.rst` & `osxphotos-0.60.0/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/__init__.py` & `osxphotos-0.60.0/osxphotos/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,26 @@
 from .exiftool import ExifTool
 from .export_db import ExportDB, ExportDBTemp
 from .fileutil import FileUtil, FileUtilNoOp
 from .momentinfo import MomentInfo
 from .personinfo import PersonInfo
 from .photoexporter import ExportOptions, ExportResults, PhotoExporter
 from .photoinfo import PhotoInfo
-from .photosalbum import PhotosAlbum, PhotosAlbumPhotoScript
 from .photosdb import PhotosDB
 from .photosdb._photosdb_process_comments import CommentInfo, LikeInfo
+from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate
 from .placeinfo import PlaceInfo
 from .queryoptions import QueryOptions
 from .scoreinfo import ScoreInfo
 from .searchinfo import SearchInfo
+from .utils import is_macos
+
+if is_macos:
+    from .photosalbum import PhotosAlbum, PhotosAlbumPhotoScript
 
 # configure logging; every module in osxphotos should use this logger
 logging.basicConfig(
     level=logging.DEBUG,
     format="%(asctime)s - %(name)s - %(levelname)s - %(filename)s - %(lineno)d - %(message)s",
 )
 logger: logging.Logger = logging.getLogger("osxphotos")
@@ -49,14 +53,15 @@
     "FolderInfo",
     "ImportInfo",
     "LikeInfo",
     "MomentInfo",
     "PersonInfo",
     "PhotoExporter",
     "PhotoInfo",
+    "PhotoTables",
     "PhotoTemplate",
     "PhotosAlbum",
     "PhotosAlbumPhotoScript",
     "PhotosDB",
     "PlaceInfo",
     "ProjectInfo",
     "QueryOptions",
```

### Comparing `osxphotos-0.59.3/osxphotos/_constants.py` & `osxphotos-0.60.0/osxphotos/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     ("12", "3"),
     ("12", "4"),
     ("12", "5"),
     ("12", "6"),
     ("13", "0"),
     ("13", "1"),
     ("13", "2"),
+    ("13", "3"),
 ]
 
 # Photos 5 has persons who are empty string if unidentified face
 _UNKNOWN_PERSON = "_UNKNOWN_"
 
 # photos with no reverse geolocation info (place)
 _UNKNOWN_PLACE = "_UNKNOWN_"
```

### Comparing `osxphotos-0.59.3/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.0/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/albuminfo.py` & `osxphotos-0.60.0/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/__init__.py` & `osxphotos-0.60.0/osxphotos/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """cli package for osxphotos"""
 
 import sys
 
 from rich import print
 from rich.traceback import install as install_traceback
 
+from osxphotos.utils import is_macos
 from osxphotos.debug import (
     debug_breakpoint,
     debug_watch,
     get_debug_flags,
     get_debug_options,
     set_debug,
     wrap_function,
@@ -40,17 +41,15 @@
 
 args = get_debug_flags(["--debug"], sys.argv)
 if args.get("--debug", False):
     set_debug(True)
     print("Debugging enabled", file=sys.stderr)
 
 from .about import about
-from .add_locations import add_locations
 from .albums import albums
-from .batch_edit import batch_edit
 from .cli import cli_main
 from .cli_commands import (
     abort,
     echo,
     echo_error,
     logger,
     query_command,
@@ -63,36 +62,40 @@
 from .docs import docs_command
 from .dump import dump
 from .exiftool_cli import exiftool
 from .export import export
 from .exportdb import exportdb
 from .grep import grep
 from .help import help
-from .import_cli import import_cli
 from .info import info
 from .install_uninstall_run import install, run, uninstall
 from .keywords import keywords
 from .kvstore import kvstore
 from .labels import labels
 from .list import _list_libraries, list_libraries
 from .orphans import orphans
 from .persons import persons
-from .photo_inspect import photo_inspect
 from .places import places
 from .query import query
 from .repl import repl
-from .show_command import show
 from .snap_diff import diff, snap
-from .sync import sync
 from .theme import theme
-from .timewarp import timewarp
 from .tutorial import tutorial
-from .uuid import uuid
 from .version import version
 
+if is_macos:
+    from .add_locations import add_locations
+    from .batch_edit import batch_edit
+    from .import_cli import import_cli
+    from .photo_inspect import photo_inspect
+    from .show_command import show
+    from .sync import sync
+    from .timewarp import timewarp
+    from .uuid import uuid
+
 install_traceback()
 
 __all__ = [
     "abort",
     "about",
     "add_locations",
     "albums",
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/about.py` & `osxphotos-0.60.0/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/add_locations.py` & `osxphotos-0.60.0/osxphotos/cli/add_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Add missing location data to photos in Photos.app using nearest neighbor."""
 
 from __future__ import annotations
 
 import datetime
 
 import click
-import photoscript
 
 import osxphotos
 from osxphotos.queryoptions import IncompatibleQueryOptions, query_options_from_kwargs
-from osxphotos.utils import pluralize
+from osxphotos.utils import assert_macos, pluralize
 
 from .cli_params import QUERY_OPTIONS, THEME_OPTION, TIMESTAMP_OPTION, VERBOSE_OPTION
 from .click_rich_echo import rich_click_echo as echo
 from .click_rich_echo import rich_echo_error as echo_error
 from .param_types import TimeOffset
 from .rich_progress import rich_progress
 from .verbose import get_verbose_console, verbose_print
 
+assert_macos()
+
+import photoscript
+
 
 def get_location(
     photos: list[osxphotos.PhotoInfo], idx: int, window: datetime.timedelta
 ) -> osxphotos.PhotoInfo | None:
     """Find nearest neighbor with location data within window of time.
 
     Args:
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/albums.py` & `osxphotos-0.60.0/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.0/osxphotos/cli/batch_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 from __future__ import annotations
 
 import functools
 import json
 import sys
 
 import click
-import photoscript
 
 import osxphotos
 from osxphotos.phototemplate import RenderOptions
 from osxphotos.sqlitekvstore import SQLiteKVStore
+from osxphotos.utils import assert_macos
+
+assert_macos()
+
+import photoscript
 
 from .cli_commands import echo, echo_error, selection_command, verbose
 from .kvstore import kvstore
 from .param_types import Latitude, Longitude, TemplateString
 
 
 @selection_command(name="batch-edit")
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/cli.py` & `osxphotos-0.60.0/osxphotos/cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,50 +5,53 @@
 import io
 import pstats
 
 import click
 
 from osxphotos._constants import PROFILE_SORT_KEYS
 from osxphotos._version import __version__
+from osxphotos.utils import is_macos
 
 from .about import about
-from .add_locations import add_locations
 from .albums import albums
-from .batch_edit import batch_edit
 from .cli_params import DB_OPTION, DEBUG_OPTIONS, JSON_OPTION, VERSION_OPTION
 from .common import OSXPHOTOS_HIDDEN
 from .debug_dump import debug_dump
 from .docs import docs_command
 from .dump import dump
 from .exiftool_cli import exiftool
 from .export import export
 from .exportdb import exportdb
 from .grep import grep
 from .help import help
-from .import_cli import import_cli
 from .info import info
 from .install_uninstall_run import install, run, uninstall
 from .keywords import keywords
 from .labels import labels
 from .list import list_libraries
 from .orphans import orphans
 from .persons import persons
-from .photo_inspect import photo_inspect
 from .places import places
 from .query import query
 from .repl import repl
-from .show_command import show
 from .snap_diff import diff, snap
-from .sync import sync
 from .theme import theme
-from .timewarp import timewarp
 from .tutorial import tutorial
-from .uuid import uuid
 from .version import version
 
+if is_macos:
+    from .add_locations import add_locations
+    from .batch_edit import batch_edit
+    from .import_cli import import_cli
+    from .photo_inspect import photo_inspect
+    from .show_command import show
+    from .sync import sync
+    from .timewarp import timewarp
+    from .uuid import uuid
+
 
 # Click CLI object & context settings
 class CLI_Obj:
     def __init__(self, db=None, json=False, debug=False, group=None):
         self.db = db
         self.json = json
         self.group = group
@@ -102,45 +105,51 @@
             ).print_stats()
             click.echo(s.getvalue())
 
         atexit.register(at_exit)
 
 
 # install CLI commands
-for command in [
+commands = [
     about,
-    add_locations,
     albums,
-    batch_edit,
     debug_dump,
     diff,
     docs_command,
     dump,
     exiftool,
     export,
     exportdb,
     grep,
     help,
-    import_cli,
     info,
     install,
     keywords,
     labels,
     list_libraries,
     orphans,
     persons,
-    photo_inspect,
     places,
     query,
     repl,
     run,
-    show,
     snap,
-    sync,
     theme,
-    timewarp,
     tutorial,
     uninstall,
-    uuid,
     version,
-]:
+]
+
+if is_macos:
+    commands += [
+        add_locations,
+        batch_edit,
+        import_cli,
+        photo_inspect,
+        show,
+        sync,
+        timewarp,
+        uuid,
+    ]
+
+for command in commands:
     cli_main.add_command(command)
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.0/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/cli_params.py` & `osxphotos-0.60.0/osxphotos/cli/cli_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from __future__ import annotations
 
 import functools
 from typing import Any, Callable
 import click
 import contextlib
 from textwrap import dedent
+
+from ..utils import is_macos
 from .common import OSXPHOTOS_HIDDEN, print_version
 from .param_types import *
 
 __all__ = [
     "DB_ARGUMENT",
     "DB_OPTION",
     "DEBUG_OPTIONS",
@@ -638,14 +640,17 @@
         + "Your function will be passed a list of PhotoInfo objects and is expected to return a filtered list of PhotoInfo objects. "
         + "You may use more than one function by repeating the --query-function option with a different value. "
         + "Your query function will be called after all other query options have been evaluated. "
         + "See https://github.com/RhetTbull/osxphotos/blob/master/examples/query_function.py for example of how to use this option.",
     ),
 }
 
+if not is_macos:
+    del _QUERY_PARAMETERS_DICT["--selected"]
+
 
 def QUERY_OPTIONS(
     wrapped=None, *, exclude: list[str] | None = None
 ) -> Callable[..., Any]:
     """Function decorator to add query options to a click command.
 
     Args:
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.0/osxphotos/cli/click_rich_echo.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,17 @@
             echo_args[arg] = val
 
     width = kwargs.pop("width", None)
     if width is None and OSXPHOTOS_IS_TESTING:
         # if not outputting to terminal, use a huge width to avoid wrapping
         # otherwise tests fail
         width = 10_000
-    console = get_rich_console() or Console(theme=theme or get_rich_theme(), width=width)
+    console = get_rich_console() or Console(
+        theme=theme or get_rich_theme(), width=width
+    )
     if markdown:
         message = Markdown(message)
         # Markdown always adds a new line so disable unless explicitly specified
     global _timestamp
     if _timestamp:
         message = time_stamp() + message
     console.print(message, highlight=highlight, **kwargs)
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/color_themes.py` & `osxphotos-0.60.0/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/common.py` & `osxphotos-0.60.0/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.0/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/docs.py` & `osxphotos-0.60.0/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/dump.py` & `osxphotos-0.60.0/osxphotos/cli/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     deleted_only,
     field,
     json_,
     photos_library,
     print_template,
 ):
     """Print list of all photos & associated info from the Photos library.
-    
-    NOTE: dump is DEPRECATED and will be removed in a future release. 
+
+    NOTE: dump is DEPRECATED and will be removed in a future release.
     Use `osxphotos query` instead.
     """
 
     # below needed for to make CliRunner work for testing
     cli_db = cli_obj.db if cli_obj is not None else None
     cli_json = cli_obj.json if cli_obj is not None else None
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.0/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/export.py` & `osxphotos-0.60.0/osxphotos/cli/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,21 +8,14 @@
 import shlex
 import subprocess
 import sys
 import time
 from typing import Iterable, List, Optional, Tuple
 
 import click
-from osxmetadata import (
-    MDITEM_ATTRIBUTE_DATA,
-    MDITEM_ATTRIBUTE_SHORT_NAMES,
-    OSXMetaData,
-    Tag,
-)
-from osxmetadata.constants import _TAGS_NAMES
 
 import osxphotos
 from osxphotos._constants import (
     _EXIF_TOOL_URL,
     _OSXPHOTOS_NONE_SENTINEL,
     DEFAULT_EDITED_SUFFIX,
     DEFAULT_JPEG_QUALITY,
@@ -43,34 +36,45 @@
     ConfigOptionsLoadError,
 )
 from osxphotos.crash_reporter import crash_reporter, set_crash_data
 from osxphotos.datetime_formatter import DateTimeFormatter
 from osxphotos.debug import is_debug
 from osxphotos.exiftool import get_exiftool_path
 from osxphotos.export_db import ExportDB, ExportDBInMemory
-from osxphotos.fileutil import FileUtil, FileUtilNoOp, FileUtilShUtil
+from osxphotos.fileutil import FileUtilMacOS, FileUtilNoOp, FileUtilShUtil
 from osxphotos.path_utils import is_valid_filepath, sanitize_filename, sanitize_filepath
 from osxphotos.photoexporter import ExportOptions, ExportResults, PhotoExporter
 from osxphotos.photoinfo import PhotoInfoNone
-from osxphotos.photokit import (
-    check_photokit_authorization,
-    request_photokit_authorization,
-)
-from osxphotos.photosalbum import PhotosAlbum
 from osxphotos.phototemplate import PhotoTemplate, RenderOptions
 from osxphotos.queryoptions import load_uuid_from_file, query_options_from_kwargs
 from osxphotos.uti import get_preferred_uti_extension
 from osxphotos.utils import (
     format_sec_to_hhmmss,
     get_macos_version,
+    is_macos,
     normalize_fs_path,
     pluralize,
     under_test,
 )
 
+if is_macos:
+    from osxmetadata import (
+        MDITEM_ATTRIBUTE_DATA,
+        MDITEM_ATTRIBUTE_SHORT_NAMES,
+        OSXMetaData,
+        Tag,
+    )
+    from osxmetadata.constants import _TAGS_NAMES
+
+    from osxphotos.photokit import (
+        check_photokit_authorization,
+        request_photokit_authorization,
+    )
+    from osxphotos.photosalbum import PhotosAlbum
+
 from .cli_commands import logger
 from .cli_params import (
     DB_ARGUMENT,
     DB_OPTION,
     DELETED_OPTIONS,
     JSON_OPTION,
     QUERY_OPTIONS,
@@ -847,15 +851,14 @@
     ramdb,
     regex,
     replace_keywords,
     report,
     retry,
     save_config,
     screenshot,
-    selected,
     selfie,
     shared,
     sidecar,
     sidecar_drop_ext,
     skip_bursts,
     skip_edited,
     skip_live,
@@ -879,14 +882,15 @@
     use_photos_export,
     uti,
     uuid,
     uuid_from_file,
     verbose_flag,
     xattr_template,
     year,
+    selected=False,  # Isn't provided on unsupported platforms
     # debug,  # debug, watch, breakpoint handled in cli/__init__.py
     # watch,
     # breakpoint,
 ):
     """Export photos from the Photos database.
     Export path DEST is required.
 
@@ -1107,15 +1111,18 @@
         verbose = verbose_print(verbose=verbose_flag, timestamp=timestamp, theme=theme)
         verbose(f"Loaded options from file [filepath]{load_config}")
 
         set_crash_data("cfg", cfg.asdict())
 
     verbose(f"osxphotos version: {__version__}")
     verbose(f"Python version: {sys.version}")
-    verbose(f"Platform: {platform.platform()}, {'.'.join(get_macos_version())}")
+    if is_macos:
+        verbose(f"Platform: {platform.platform()}, {'.'.join(get_macos_version())}")
+    else:
+        verbose(f"Platform: {platform.platform()}")
     verbose(f"Verbose level: {verbose_flag}")
 
     # validate options
     exclusive_options = [
         ("burst", "not_burst"),
         ("cloudasset", "not_cloudasset"),
         ("deleted", "deleted_only"),
@@ -1321,15 +1328,15 @@
         fileutil = FileUtilNoOp
     else:
         export_db = (
             ExportDBInMemory(dbfile=export_db_path, export_dir=dest)
             if ramdb
             else ExportDB(dbfile=export_db_path, export_dir=dest)
         )
-        fileutil = FileUtilShUtil if alt_copy else FileUtil
+        fileutil = FileUtilShUtil if alt_copy or not is_macos else FileUtilMacOS
 
     if verbose:
         if export_db.was_created:
             verbose(f"Created export database [filepath]{export_db_path}")
         else:
             verbose(f"Using export database [filepath]{export_db_path}")
         upgraded = export_db.was_upgraded
@@ -1709,15 +1716,15 @@
     filename_template=None,
     export_raw=None,
     album_keyword=None,
     person_keyword=None,
     keyword_template=None,
     description_template=None,
     export_db=None,
-    fileutil=FileUtil,
+    fileutil=FileUtilShUtil,
     dry_run=None,
     touch_file=None,
     edited_suffix="_edited",
     original_suffix="",
     use_photos_export=False,
     convert_to_jpeg=False,
     jpeg_quality=1.0,
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/exportdb.py` & `osxphotos-0.60.0/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/grep.py` & `osxphotos-0.60.0/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/help.py` & `osxphotos-0.60.0/osxphotos/cli/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Help text helper class for osxphotos CLI """
 
 import inspect
 import re
 import typing as t
 
 import click
-from osxmetadata import MDITEM_ATTRIBUTE_DATA, MDITEM_ATTRIBUTE_SHORT_NAMES
 from rich.console import Console
 from rich.markdown import Markdown
 
 from osxphotos._constants import (
     EXTENDED_ATTRIBUTE_NAMES,
     EXTENDED_ATTRIBUTE_NAMES_QUOTED,
     OSXPHOTOS_EXPORT_DB,
@@ -17,14 +16,18 @@
 )
 from osxphotos.phototemplate import (
     TEMPLATE_SUBSTITUTIONS,
     TEMPLATE_SUBSTITUTIONS_MULTI_VALUED,
     TEMPLATE_SUBSTITUTIONS_PATHLIB,
     get_template_help,
 )
+from osxphotos.utils import is_macos
+
+if is_macos:
+    from osxmetadata import MDITEM_ATTRIBUTE_DATA, MDITEM_ATTRIBUTE_SHORT_NAMES
 
 from .click_rich_echo import rich_echo_via_pager
 from .color_themes import get_theme
 from .common import OSXPHOTOS_HIDDEN
 
 HELP_WIDTH = 110
 HIGHLIGHT_COLOR = "yellow"
@@ -245,76 +248,81 @@
             + "The signature includes size, modification time, and filename.  In order to minimize "
             + "run time, --update does not do a full comparison (diff) of the files nor does it compare "
             + "hashes of the files.  In normal usage, this is sufficient for updating the library. "
             + "You can always run export without the --update option to re-export the entire library thus "
             + f"rebuilding the '{OSXPHOTOS_EXPORT_DB}' database."
         )
         formatter.write("\n")
-        formatter.write(
-            rich_text("## Extended Attributes", width=formatter.width, markdown=True)
-        )
-        formatter.write("\n")
-        formatter.write_text(
-            """
-Some options (currently '--finder-tag-template', '--finder-tag-keywords', '-xattr-template') write
-additional metadata accessible by Spotlight to facilitate searching. 
-For example, --finder-tag-keyword writes all keywords (including any specified by '--keyword-template'
-or other options) to Finder tags that are searchable in Spotlight using the syntax: 'tag:tagname'.
-For example, if you have images with keyword "Travel" then using '--finder-tag-keywords' you could quickly
-find those images in the Finder by typing 'tag:Travel' in the Spotlight search bar.
-Finder tags are written to the 'com.apple.metadata:_kMDItemUserTags' extended attribute.
-Unlike EXIF metadata, extended attributes do not modify the actual file;
-the metadata is written to extended attributes associated with the file and the Spotlight metadata database. 
-Most cloud storage services do not synch extended attributes. 
-Dropbox does sync them and any changes to a file's extended attributes
-will cause Dropbox to re-sync the files.
 
-The following attributes may be used with '--xattr-template':
+        if is_macos:
+            formatter.write(
+                rich_text(
+                    "## Extended Attributes", width=formatter.width, markdown=True
+                )
+            )
+            formatter.write("\n")
+            formatter.write_text(
+                """
+    Some options (currently '--finder-tag-template', '--finder-tag-keywords', '-xattr-template') write
+    additional metadata accessible by Spotlight to facilitate searching. 
+    For example, --finder-tag-keyword writes all keywords (including any specified by '--keyword-template'
+    or other options) to Finder tags that are searchable in Spotlight using the syntax: 'tag:tagname'.
+    For example, if you have images with keyword "Travel" then using '--finder-tag-keywords' you could quickly
+    find those images in the Finder by typing 'tag:Travel' in the Spotlight search bar.
+    Finder tags are written to the 'com.apple.metadata:_kMDItemUserTags' extended attribute.
+    Unlike EXIF metadata, extended attributes do not modify the actual file;
+    the metadata is written to extended attributes associated with the file and the Spotlight metadata database. 
+    Most cloud storage services do not synch extended attributes. 
+    Dropbox does sync them and any changes to a file's extended attributes
+    will cause Dropbox to re-sync the files.
 
-            """
-        )
+    The following attributes may be used with '--xattr-template':
 
-        # build help text from all the attribute names
-        # passed to click.HelpFormatter.write_dl for formatting
-        attr_tuples = [
-            (
-                rich_text("[bold]Attribute[/bold]", width=formatter.width),
-                rich_text("[bold]Description[/bold]", width=formatter.width),
+                """
             )
-        ]
-        for attr_key in sorted(EXTENDED_ATTRIBUTE_NAMES):
-            # get short and long name
-            attr = MDITEM_ATTRIBUTE_SHORT_NAMES[attr_key]
-            short_name = MDITEM_ATTRIBUTE_DATA[attr]["short_name"]
-            long_name = MDITEM_ATTRIBUTE_DATA[attr]["name"]
-            constant = MDITEM_ATTRIBUTE_DATA[attr]["xattr_constant"]
-
-            # get help text
-            description = MDITEM_ATTRIBUTE_DATA[attr]["description"]
-            type_ = MDITEM_ATTRIBUTE_DATA[attr]["help_type"]
-            attr_help = f"{long_name}; {constant}; {description}; {type_}"
 
-            # add to list
-            attr_tuples.append((short_name, attr_help))
+            # build help text from all the attribute names
+            # passed to click.HelpFormatter.write_dl for formatting
+            attr_tuples = [
+                (
+                    rich_text("[bold]Attribute[/bold]", width=formatter.width),
+                    rich_text("[bold]Description[/bold]", width=formatter.width),
+                )
+            ]
+            for attr_key in sorted(EXTENDED_ATTRIBUTE_NAMES):
+                # get short and long name
+                attr = MDITEM_ATTRIBUTE_SHORT_NAMES[attr_key]
+                short_name = MDITEM_ATTRIBUTE_DATA[attr]["short_name"]
+                long_name = MDITEM_ATTRIBUTE_DATA[attr]["name"]
+                constant = MDITEM_ATTRIBUTE_DATA[attr]["xattr_constant"]
+
+                # get help text
+                description = MDITEM_ATTRIBUTE_DATA[attr]["description"]
+                type_ = MDITEM_ATTRIBUTE_DATA[attr]["help_type"]
+                attr_help = f"{long_name}; {constant}; {description}; {type_}"
+
+                # add to list
+                attr_tuples.append((short_name, attr_help))
+
+            formatter.write_dl(attr_tuples)
+            formatter.write("\n")
+            formatter.write_text(
+                "For additional information on extended attributes see: https://developer.apple.com/documentation/coreservices/file_metadata/mditem/common_metadata_attribute_keys"
+            )
+            formatter.write("\n")
+            formatter.write(
+                rich_text("## Templating System", width=formatter.width, markdown=True)
+            )
+            formatter.write("\n")
+            help_text += formatter.getvalue()
+            help_text += template_help(width=formatter.width)
+            formatter = click.HelpFormatter(width=HELP_WIDTH)
 
-        formatter.write_dl(attr_tuples)
-        formatter.write("\n")
-        formatter.write_text(
-            "For additional information on extended attributes see: https://developer.apple.com/documentation/coreservices/file_metadata/mditem/common_metadata_attribute_keys"
-        )
-        formatter.write("\n")
-        formatter.write(
-            rich_text("## Templating System", width=formatter.width, markdown=True)
-        )
-        formatter.write("\n")
-        help_text += formatter.getvalue()
-        help_text += template_help(width=formatter.width)
-        formatter = click.HelpFormatter(width=HELP_WIDTH)
+            formatter.write("\n")
 
-        formatter.write("\n")
         formatter.write_text(
             "With the --directory and --filename options you may specify a template for the "
             + "export directory or filename, respectively. "
             + "The directory will be appended to the export path specified "
             + "in the export DEST argument to export.  For example, if template is "
             + "'{created.year}/{created.month}', and export destination DEST is "
             + "'/Users/maria/Pictures/export', "
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/import_cli.py` & `osxphotos-0.60.0/osxphotos/cli/import_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from contextlib import suppress
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
 from textwrap import dedent
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import click
-from photoscript import Photo, PhotosLibrary
 from rich.console import Console
 from rich.markdown import Markdown
 from strpdatetime import strpdatetime
 
 from osxphotos._constants import _OSXPHOTOS_NONE_SENTINEL, SQLITE_CHECK_SAME_THREAD
 from osxphotos._version import __version__
 from osxphotos.cli.cli_params import TIMESTAMP_OPTION, VERBOSE_OPTION
@@ -39,15 +38,19 @@
     datetime_utc_to_local,
 )
 from osxphotos.exiftool import ExifToolCaching, get_exiftool_path
 from osxphotos.photoinfo import PhotoInfoNone
 from osxphotos.photosalbum import PhotosAlbumPhotoScript
 from osxphotos.phototemplate import PhotoTemplate, RenderOptions
 from osxphotos.sqlitekvstore import SQLiteKVStore
-from osxphotos.utils import pluralize
+from osxphotos.utils import assert_macos, pluralize
+
+assert_macos()
+
+from photoscript import Photo, PhotosLibrary
 
 from .cli_params import THEME_OPTION
 from .click_rich_echo import rich_click_echo, rich_echo_error
 from .rich_progress import rich_progress
 from .verbose import get_verbose_console, verbose_print
 
 # Note: the style in this module is a bit different than much of the other osxphotos code
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/info.py` & `osxphotos-0.60.0/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.0/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/keywords.py` & `osxphotos-0.60.0/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/kvstore.py` & `osxphotos-0.60.0/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/labels.py` & `osxphotos-0.60.0/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/list.py` & `osxphotos-0.60.0/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/orphans.py` & `osxphotos-0.60.0/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/param_types.py` & `osxphotos-0.60.0/osxphotos/cli/param_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,29 +64,27 @@
         super().__init__(*args, **kwargs)
 
     def convert(self, value, param, ctx):
         return value if value == "-" else super().convert(value, param, ctx)
 
 
 class DateTimeISO8601(click.ParamType):
-
     name = "DATETIME"
 
     def convert(self, value, param, ctx):
         try:
             return datetime.datetime.fromisoformat(value)
         except Exception:
             self.fail(
                 f"Invalid datetime format {value}. "
                 "Valid format: YYYY-MM-DD[*HH[:MM[:SS[.fff[fff]]]][+HH:MM[:SS[.ffffff]]]]"
             )
 
 
 class BitMathSize(click.ParamType):
-
     name = "BITMATH"
 
     def convert(self, value, param, ctx):
         try:
             value = bitmath.parse_string(value)
         except ValueError:
             # no units specified
@@ -98,15 +96,14 @@
                     f"{value} must be specified as bytes or using SI/NIST units. "
                     + "For example, the following are all valid and equivalent sizes: '1048576' '1.048576MB', '1 MiB'."
                 )
         return value
 
 
 class TimeISO8601(click.ParamType):
-
     name = "TIME"
 
     def convert(self, value, param, ctx):
         try:
             return datetime.time.fromisoformat(value).replace(tzinfo=None)
         except Exception:
             self.fail(
@@ -137,15 +134,14 @@
         except Exception as e:
             self.fail(f"Could not load function {funcname} from {filename_validated}")
 
         return (function, value)
 
 
 class ExportDBType(click.ParamType):
-
     name = "EXPORTDB"
 
     def convert(self, value, param, ctx):
         try:
             export_db_name = pathlib.Path(value)
             if export_db_name.is_dir():
                 raise click.BadParameter(f"{value} is a directory")
@@ -275,15 +271,14 @@
             ):
                 self.fail(f"Invalid strpdatetime format string: {value}. {e}")
             else:
                 return value
 
 
 class Latitude(click.ParamType):
-
     name = "Latitude"
 
     def convert(self, value, param, ctx):
         try:
             latitude = float(value)
             if latitude < -90 or latitude > 90:
                 raise ValueError
@@ -291,15 +286,14 @@
         except Exception:
             self.fail(
                 f"Invalid latitude {value}. Must be a floating point number between -90 and 90."
             )
 
 
 class Longitude(click.ParamType):
-
     name = "Longitude"
 
     def convert(self, value, param, ctx):
         try:
             longitude = float(value)
             if longitude < -180 or longitude > 180:
                 raise ValueError
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/persons.py` & `osxphotos-0.60.0/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.0/osxphotos/cli/photo_inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,30 @@
 from multiprocessing import Process, Queue
 from queue import Empty
 from time import gmtime, sleep, strftime
 from typing import Generator, List, Optional, Tuple
 
 import bitmath
 import click
-from applescript import ScriptError
-from photoscript import PhotosLibrary
 from rich.console import Console
 from rich.layout import Layout
 from rich.live import Live
 from rich.panel import Panel
 
 from osxphotos import PhotoInfo, PhotosDB
 from osxphotos._constants import _UNKNOWN_PERSON, search_category_factory
 from osxphotos.rich_utils import add_rich_markup_tag
+from osxphotos.utils import assert_macos, dd_to_dms_str
+
+assert_macos()
+
+from applescript import ScriptError
+from photoscript import PhotosLibrary
+
 from osxphotos.text_detection import detect_text as detect_text_in_photo
-from osxphotos.utils import dd_to_dms_str
 
 from .cli_params import DB_OPTION, THEME_OPTION
 from .color_themes import get_theme
 from .common import get_photos_db
 
 # global that tracks UUID being inspected
 CURRENT_UUID = None
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/places.py` & `osxphotos-0.60.0/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.0/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/query.py` & `osxphotos-0.60.0/osxphotos/cli/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 """query command for osxphotos CLI"""
 
+import sys
 import click
 
 import osxphotos
 from osxphotos.cli.click_rich_echo import (
     rich_click_echo,
     set_rich_console,
     set_rich_theme,
 )
 from osxphotos.debug import set_debug
-from osxphotos.photosalbum import PhotosAlbum
 from osxphotos.phototemplate import RenderOptions
 from osxphotos.queryoptions import query_options_from_kwargs
+from osxphotos.utils import assert_macos, is_macos
+
+if is_macos:
+    from osxphotos.photosalbum import PhotosAlbum
 
 from .cli_params import (
     DB_ARGUMENT,
     DB_OPTION,
     DELETED_OPTIONS,
     FIELD_OPTION,
     JSON_OPTION,
     QUERY_OPTIONS,
+    make_click_option_decorator,
 )
 from .color_themes import get_default_theme
 from .common import CLI_COLOR_ERROR, CLI_COLOR_WARNING, OSXPHOTOS_HIDDEN, get_photos_db
 from .list import _list_libraries
 from .print_photo_info import print_photo_fields, print_photo_info
 from .verbose import get_verbose_console
 
+MACOS_OPTIONS = make_click_option_decorator(
+    *[
+        click.Option(
+            ["--add-to-album"],
+            metavar="ALBUM",
+            help="Add all photos from query to album ALBUM in Photos. Album ALBUM will be created "
+            "if it doesn't exist.  All photos in the query results will be added to this album. "
+            "This only works if the Photos library being queried is the last-opened (default) library in Photos. "
+            "This feature is currently experimental.  I don't know how well it will work on large query sets.",
+        ),
+    ]
+    if is_macos
+    else []
+)
+
 
 @click.command()
 @DB_OPTION
 @JSON_OPTION
 @QUERY_OPTIONS
 @DELETED_OPTIONS
-@click.option(
-    "--add-to-album",
-    metavar="ALBUM",
-    help="Add all photos from query to album ALBUM in Photos. Album ALBUM will be created "
-    "if it doesn't exist.  All photos in the query results will be added to this album. "
-    "This only works if the Photos library being queried is the last-opened (default) library in Photos. "
-    "This feature is currently experimental.  I don't know how well it will work on large query sets.",
-)
+@MACOS_OPTIONS
 @click.option(
     "--quiet",
     is_flag=True,
     help="Quiet output; doesn't actually print query results. "
     "Useful with --print and --add-to-album if you don't want to see the actual query results.",
 )
 @FIELD_OPTION
@@ -66,16 +79,16 @@
     ctx,
     cli_obj,
     db,
     field,
     json_,
     print_template,
     quiet,
-    add_to_album,
     photos_library,
+    add_to_album=False,
     **kwargs,
 ):
     """Query the Photos database using 1 or more search options;
     if more than one different option is provided, they are treated as "AND"
     (e.g. search for photos matching all options).
     If the same query option is provided multiple times, they are treated as
     "OR" (e.g. search for photos matching any of the options).
@@ -120,14 +133,16 @@
             "query_eval", f"Invalid query-eval CRITERIA: {msg}"
         ) from e
 
     # below needed for to make CliRunner work for testing
     cli_json = cli_obj.json if cli_obj is not None else None
 
     if add_to_album and photos:
+        assert_macos()
+
         album_query = PhotosAlbum(add_to_album, verbose=None)
         photo_len = len(photos)
         photo_word = "photos" if photo_len > 1 else "photo"
         click.echo(
             f"Adding {photo_len} {photo_word} to album '{album_query.name}'. Note: Photos may prompt you to confirm this action.",
             err=True,
         )
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/repl.py` & `osxphotos-0.60.0/osxphotos/cli/repl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 """repl command for osxphotos CLI"""
+from __future__ import annotations
 
 import os
 import os.path
 import pathlib
+import re
 import sys
 import time
 from typing import List
 
 import click
-import photoscript
 from rich import pretty, print
 
 import osxphotos
 from osxphotos._constants import _PHOTOS_4_VERSION
 from osxphotos.cli.click_rich_echo import rich_echo_error as echo_error
 from osxphotos.photoinfo import PhotoInfo
 from osxphotos.photosdb import PhotosDB
 from osxphotos.pyrepl import embed_repl
 from osxphotos.queryoptions import (
     IncompatibleQueryOptions,
     QueryOptions,
     query_options_from_kwargs,
 )
+from osxphotos.utils import assert_macos, is_macos
+
+if is_macos:
+    import photoscript
+    from applescript import ScriptError
 
 from .cli_params import DB_ARGUMENT, DB_OPTION, DELETED_OPTIONS, QUERY_OPTIONS
 from .common import get_photos_db
 
 
 @click.command(name="repl")
 @DB_OPTION
@@ -48,15 +54,17 @@
 @QUERY_OPTIONS
 @DELETED_OPTIONS
 def repl(ctx, cli_obj, db, emacs, beta, **kwargs):
     """Run interactive osxphotos REPL shell (useful for debugging, prototyping, and inspecting your Photos library)"""
     import logging
 
     from objexplore import explore
-    from photoscript import Album, Photo, PhotosLibrary
+
+    if is_macos:
+        from photoscript import Album, Photo, PhotosLibrary
     from rich import inspect as _inspect
 
     from osxphotos import ExifTool, PhotoInfo, PhotosDB
     from osxphotos.albuminfo import AlbumInfo
     from osxphotos.momentinfo import MomentInfo
     from osxphotos.photoexporter import ExportOptions, ExportResults, PhotoExporter
     from osxphotos.placeinfo import PlaceInfo
@@ -187,23 +195,31 @@
     return photos
 
 
 def _get_selected(photosdb):
     """get list of PhotoInfo objects for photos selected in Photos"""
 
     def get_selected():
-        selected = photoscript.PhotosLibrary().selection
-        if not selected:
-            return []
-        return photosdb.photos(uuid=[p.uuid for p in selected])
+        assert_macos()
+        try:
+            selected = photoscript.PhotosLibrary().selection
+        except ScriptError as e:
+            # some photos (e.g. shared items) can't be selected and raise ScriptError:
+            # applescript.ScriptError: Photos got an error: Can’t get media item id "34C26DFA-0CEA-4DB7-8FDA-B87789B3209D/L0/001". (-1728) app='Photos' range=16820-16873
+            # In this case, we can parse the UUID from the error (though this only works for a single selected item)
+            if match := re.match(r".*Can’t get media item id \"(.*)\".*", str(e)):
+                uuid = match[1].split("/")[0]
+                return photosdb.photos(uuid=[uuid])
+        return photosdb.photos(uuid=[p.uuid for p in selected]) if selected else []
 
     return get_selected
 
 
 def _spotlight_photo(photo: PhotoInfo):
+    assert_macos()
     photo_ = photoscript.Photo(photo.uuid)
     photo_.spotlight()
 
 
 def _query_photos(photosdb: PhotosDB, query_options: QueryOptions) -> List:
     """Query photos given a QueryOptions instance"""
     try:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/report_writer.py` & `osxphotos-0.60.0/osxphotos/cli/report_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,17 @@
         self.output_file = output_file
         self.append = append
 
         if not append:
             with suppress(FileNotFoundError):
                 os.unlink(self.output_file)
 
-        self._conn = sqlite3.connect(self.output_file, check_same_thread=SQLITE_CHECK_SAME_THREAD)
+        self._conn = sqlite3.connect(
+            self.output_file, check_same_thread=SQLITE_CHECK_SAME_THREAD
+        )
         self._create_tables()
         self.report_id = self._generate_report_id()
 
     def write(self, export_results: ExportResults):
         """Write results to the output file"""
 
         all_results = prepare_export_results_for_writing(export_results)
@@ -530,15 +532,17 @@
         self.output_file = output_file
         self.append = append
 
         if not append:
             with suppress(FileNotFoundError):
                 os.unlink(self.output_file)
 
-        self._conn = sqlite3.connect(self.output_file, check_same_thread=SQLITE_CHECK_SAME_THREAD)
+        self._conn = sqlite3.connect(
+            self.output_file, check_same_thread=SQLITE_CHECK_SAME_THREAD
+        )
         self._create_tables()
         self.report_id = self._generate_report_id()
 
     def write(self, results: SyncResults):
         """Write results to the output file"""
 
         # insert rows of values into sqlite report table
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.0/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/show_command.py` & `osxphotos-0.60.0/osxphotos/cli/show_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 import pathlib
 import re
 
 import click
 
 from osxphotos._constants import UUID_PATTERN
 from osxphotos.export_db_utils import get_uuid_for_filepath
+from osxphotos.photosdb.photosdb_utils import get_photos_library_version
+from osxphotos.utils import get_last_library_path, assert_macos
+
+assert_macos()
+
 from osxphotos.photoscript_utils import (
     photoscript_object_from_name,
     photoscript_object_from_uuid,
 )
-from osxphotos.photosdb.photosdb_utils import get_photos_library_version
-from osxphotos.utils import get_last_library_path
 
 from .cli_commands import echo, echo_error
 from .cli_params import DB_OPTION
 from .click_rich_echo import set_rich_theme
 
 
 @click.command(name="show")
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.0/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/sync.py` & `osxphotos-0.60.0/osxphotos/cli/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 import datetime
 import json
 import os
 import pathlib
 from typing import Any, Callable, Literal
 
 import click
-import photoscript
 
 from osxphotos import PhotoInfo, PhotosDB, __version__
 from osxphotos.photoinfo import PhotoInfoNone
 from osxphotos.photosalbum import PhotosAlbum
 from osxphotos.photosdb.photosdb_utils import get_db_version
 from osxphotos.phototemplate import PhotoTemplate, RenderOptions
 from osxphotos.queryoptions import (
     IncompatibleQueryOptions,
     QueryOptions,
     query_options_from_kwargs,
 )
 from osxphotos.sqlitekvstore import SQLiteKVStore
-from osxphotos.utils import pluralize
+from osxphotos.utils import assert_macos, pluralize
+
+assert_macos()
+
+import photoscript
 
 from .cli_params import (
     DB_OPTION,
     QUERY_OPTIONS,
     THEME_OPTION,
     TIMESTAMP_OPTION,
     VERBOSE_OPTION,
@@ -163,14 +166,15 @@
                         photos_dict[k] = sorted(list(set(photos_dict[k]) | set(v)))
                     else:
                         if v:
                             if not photos_dict[k]:
                                 photos_dict[k] = v
                             elif photos_dict[k] and v != photos_dict[k]:
                                 photos_dict[k] = f"{photos_dict[k]} {v}"
+
     # convert photos_dict to JSON string
     # wouldn't it be nice if json encoder handled datetimes...
     def default(o):
         if isinstance(o, (datetime.date, datetime.datetime)):
             return o.isoformat()
 
     return json.dumps(photos_dict, sort_keys=True, default=default)
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/sync_results.py` & `osxphotos-0.60.0/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/theme.py` & `osxphotos-0.60.0/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/timewarp.py` & `osxphotos-0.60.0/osxphotos/cli/timewarp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import annotations
 
 import sys
 from functools import partial
 from textwrap import dedent
 
 import click
-from photoscript import PhotosLibrary
 from rich.console import Console
 
 from osxphotos._constants import APP_NAME
 from osxphotos._version import __version__
 from osxphotos.compare_exif import PhotoCompare
 from osxphotos.crash_reporter import crash_reporter, set_crash_data
 from osxphotos.datetime_utils import datetime_naive_to_local, datetime_to_new_tz
@@ -21,17 +20,21 @@
     get_photo_date_added,
     set_photo_date_added,
     set_photo_date_from_filename,
     update_photo_date_time,
     update_photo_from_function,
     update_photo_time_for_new_timezone,
 )
-from osxphotos.photosalbum import PhotosAlbumPhotoScript
 from osxphotos.phototz import PhotoTimeZone, PhotoTimeZoneUpdater
-from osxphotos.utils import noop, pluralize
+from osxphotos.utils import assert_macos, noop, pluralize
+
+assert_macos()
+
+from photoscript import PhotosLibrary
+from osxphotos.photosalbum import PhotosAlbumPhotoScript
 
 from .cli_params import THEME_OPTION, TIMESTAMP_OPTION, VERBOSE_OPTION
 from .click_rich_echo import rich_click_echo as echo
 from .click_rich_echo import rich_echo_error as echo_error
 from .color_themes import get_theme
 from .common import OSXPHOTOS_CRASH_LOG
 from .darkmode import is_dark_mode
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/tutorial.py` & `osxphotos-0.60.0/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/uuid.py` & `osxphotos-0.60.0/osxphotos/cli/uuid.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """uuid command for osxphotos CLI"""
 
 import click
+
+from osxphotos.utils import assert_macos
+
+assert_macos()
+
 import photoscript
 
 
 @click.command(name="uuid")
 @click.pass_obj
 @click.pass_context
 @click.option(
```

### Comparing `osxphotos-0.59.3/osxphotos/cli/verbose.py` & `osxphotos-0.60.0/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/cli/version.py` & `osxphotos-0.60.0/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/compare_exif.py` & `osxphotos-0.60.0/osxphotos/compare_exif.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """ PhotoCompare class to compare date/time/timezone in Photos to the exif data """
 
 from collections import namedtuple
 from typing import Callable, List, Optional, Tuple
 
 from osxphotos import PhotosDB
 from osxphotos.exiftool import ExifTool
-from photoscript import Photo
 
 from .datetime_utils import datetime_naive_to_local, datetime_to_new_tz
+from .utils import assert_macos, noop
+
+assert_macos()
+
+from photoscript import Photo
 from .exif_datetime_updater import get_exif_date_time_offset
 from .phototz import PhotoTimeZone
-from .utils import noop
 
 ExifDiff = namedtuple(
     "ExifDiff",
     [
         "diff",
         "photos_date",
         "photos_time",
```

### Comparing `osxphotos-0.59.3/osxphotos/configoptions.py` & `osxphotos-0.60.0/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/crash_reporter.py` & `osxphotos-0.60.0/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/datetime_formatter.py` & `osxphotos-0.60.0/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/datetime_utils.py` & `osxphotos-0.60.0/osxphotos/datetime_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "datetime_to_new_tz",
     "datetime_tz_to_utc",
     "datetime_utc_to_local",
     "get_local_tz",
     "utc_offset_seconds",
 ]
 
+
 # TODO: look at https://github.com/regebro/tzlocal for more robust implementation
 def get_local_tz(dt: datetime.datetime) -> datetime.tzinfo:
     """Return local timezone as datetime.timezone tzinfo for dt
 
     Args:
         dt: datetime.datetime
 
@@ -203,8 +204,7 @@
         ValueError if dt does not have timezone information
     """
 
     if dt.tzinfo is not None and dt.tzinfo.utcoffset(dt) is not None:
         return dt.tzinfo.utcoffset(dt).total_seconds()
     else:
         raise ValueError("dt does not have timezone info")
-
```

### Comparing `osxphotos-0.59.3/osxphotos/debug.py` & `osxphotos-0.60.0/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/docs/docs.zip` & `osxphotos-0.60.0/osxphotos/docs/docs.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1466350 bytes, number of entries: 99
+Zip file size: 1459529 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Apr-11 02:05 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-May-07 14:48 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
--rw-r--r--  3.0 unx   317210 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/photoexporter.html
--rw-r--r--  3.0 unx   296574 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/phototemplate.html
+-rw-r--r--  3.0 unx   317579 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photoexporter.html
+-rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
 -rw-r--r--  3.0 unx   200939 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
--rw-r--r--  3.0 unx    49029 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   298462 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx    52325 tx defN 23-May-07 14:38 docs/_modules/osxphotos/fileutil.html
+-rw-r--r--  3.0 unx   299834 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
 -rw-r--r--  3.0 unx    29240 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   522689 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/photosdb/photosdb.html
--rw-r--r--  3.0 unx    36121 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photosalbum.html
--rw-r--r--  3.0 unx    92801 tx defN 23-Apr-01 16:39 docs/_modules/osxphotos/placeinfo.html
+-rw-r--r--  3.0 unx   523106 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx    36244 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photosalbum.html
+-rw-r--r--  3.0 unx    92802 tx defN 23-May-07 14:38 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    59723 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
--rw-r--r--  3.0 unx    61696 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/_constants.html
+-rw-r--r--  3.0 unx    61850 tx defN 23-May-07 14:48 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Apr-11 02:05 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-May-07 14:38 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Apr-11 02:05 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-May-07 14:48 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Apr-11 02:05 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-May-07 14:48 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Apr-11 02:05 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-May-07 14:48 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Apr-11 02:05 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-May-07 14:48 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Apr-11 02:05 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-May-07 14:48 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   414459 tx defN 23-Apr-11 02:05 docs/cli.html
+-rw-r--r--  3.0 unx   414459 tx defN 23-May-07 14:38 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   243757 tx defN 23-Apr-11 02:05 docs/genindex.html
--rw-r--r--  3.0 unx   103771 tx defN 23-Apr-11 02:05 docs/index.html
+-rw-r--r--  3.0 unx   243869 tx defN 23-May-07 14:48 docs/genindex.html
+-rw-r--r--  3.0 unx   103976 tx defN 23-May-07 14:48 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9391 bx stor 23-Apr-11 02:05 docs/objects.inv
+-rw-r--r--  3.0 unx     9396 bx stor 23-May-07 14:48 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Apr-11 02:05 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Apr-11 02:05 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Apr-11 02:05 docs/py-modindex.html
--rw-r--r--  3.0 unx   437653 tx defN 23-Apr-11 02:05 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-May-07 14:38 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-May-07 14:38 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-May-07 14:48 docs/py-modindex.html
+-rw-r--r--  3.0 unx   438606 tx defN 23-May-07 14:48 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Apr-11 02:05 docs/search.html
--rw-r--r--  3.0 unx   215837 tx defN 23-Apr-11 02:05 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Apr-11 02:05 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Apr-11 02:05 docs/tutorial.html
-99 files, 6895891 bytes uncompressed, 1447618 bytes compressed:  79.0%
+-rw-r--r--  3.0 unx    10567 tx defN 23-May-07 14:48 docs/search.html
+-rw-r--r--  3.0 unx   146510 tx defN 23-May-07 14:48 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-May-07 14:48 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-May-07 14:48 docs/tutorial.html
+99 files, 6833436 bytes uncompressed, 1440797 bytes compressed:  78.9%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.59.3 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoexporter.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoexporter - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos.photoexporter - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -200,22 +200,22 @@
 
 <span class="kn">import</span> <span class="nn">dataclasses</span>
 <span class="kn">import</span> <span class="nn">json</span>
 <span class="kn">import</span> <span class="nn">logging</span>
 <span class="kn">import</span> <span class="nn">os</span>
 <span class="kn">import</span> <span class="nn">pathlib</span>
 <span class="kn">import</span> <span class="nn">re</span>
+<span class="kn">import</span> <span class="nn">sys</span>
 <span class="kn">import</span> <span class="nn">typing</span> <span class="k">as</span> <span class="nn">t</span>
 <span class="kn">from</span> <span class="nn">collections</span> <span class="kn">import</span> <span class="n">namedtuple</span>  <span class="c1"># pylint: disable=syntax-error</span>
 <span class="kn">from</span> <span class="nn">dataclasses</span> <span class="kn">import</span> <span class="n">asdict</span><span class="p">,</span> <span class="n">dataclass</span>
 <span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span>
 <span class="kn">from</span> <span class="nn">enum</span> <span class="kn">import</span> <span class="n">Enum</span>
 <span class="kn">from</span> <span class="nn">types</span> <span class="kn">import</span> <span class="n">SimpleNamespace</span>
 
-<span class="kn">import</span> <span class="nn">photoscript</span>
 <span class="kn">from</span> <span class="nn">mako.template</span> <span class="kn">import</span> <span class="n">Template</span>
 
 <span class="kn">from</span> <span class="nn">._constants</span> <span class="kn">import</span> <span class="p">(</span>
     <span class="n">_MAX_IPTC_KEYWORD_LEN</span><span class="p">,</span>
     <span class="n">_OSXPHOTOS_NONE_SENTINEL</span><span class="p">,</span>
     <span class="n">_TEMPLATE_DIR</span><span class="p">,</span>
     <span class="n">_UNKNOWN_PERSON</span><span class="p">,</span>
@@ -228,34 +228,41 @@
     <span class="n">SIDECAR_XMP</span><span class="p">,</span>
 <span class="p">)</span>
 <span class="kn">from</span> <span class="nn">._version</span> <span class="kn">import</span> <span class="n">__version__</span>
 <span class="kn">from</span> <span class="nn">.datetime_utils</span> <span class="kn">import</span> <span class="n">datetime_tz_to_utc</span>
 <span class="kn">from</span> <span class="nn">.exiftool</span> <span class="kn">import</span> <span class="n">ExifTool</span><span class="p">,</span> <span class="n">ExifToolCaching</span><span class="p">,</span> <span class="n">exiftool_can_write</span><span class="p">,</span> <span class="n">get_exiftool_path</span>
 <span class="kn">from</span> <span class="nn">.export_db</span> <span class="kn">import</span> <span class="n">ExportDB</span><span class="p">,</span> <span class="n">ExportDBTemp</span>
 <span class="kn">from</span> <span class="nn">.fileutil</span> <span class="kn">import</span> <span class="n">FileUtil</span>
-<span class="kn">from</span> <span class="nn">.photokit</span> <span class="kn">import</span> <span class="p">(</span>
-    <span class="n">PHOTOS_VERSION_CURRENT</span><span class="p">,</span>
-    <span class="n">PHOTOS_VERSION_ORIGINAL</span><span class="p">,</span>
-    <span class="n">PHOTOS_VERSION_UNADJUSTED</span><span class="p">,</span>
-    <span class="n">PhotoKitFetchFailed</span><span class="p">,</span>
-    <span class="n">PhotoLibrary</span><span class="p">,</span>
-<span class="p">)</span>
 <span class="kn">from</span> <span class="nn">.phototemplate</span> <span class="kn">import</span> <span class="n">RenderOptions</span>
 <span class="kn">from</span> <span class="nn">.rich_utils</span> <span class="kn">import</span> <span class="n">add_rich_markup_tag</span>
 <span class="kn">from</span> <span class="nn">.uti</span> <span class="kn">import</span> <span class="n">get_preferred_uti_extension</span>
 <span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="p">(</span>
+    <span class="n">is_macos</span><span class="p">,</span>
     <span class="n">hexdigest</span><span class="p">,</span>
     <span class="n">increment_filename</span><span class="p">,</span>
     <span class="n">increment_filename_with_count</span><span class="p">,</span>
     <span class="n">lineno</span><span class="p">,</span>
     <span class="n">list_directory</span><span class="p">,</span>
     <span class="n">lock_filename</span><span class="p">,</span>
+    <span class="n">normalize_fs_path</span><span class="p">,</span>
     <span class="n">unlock_filename</span><span class="p">,</span>
 <span class="p">)</span>
 
+<span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
+    <span class="kn">import</span> <span class="nn">photoscript</span>
+
+    <span class="kn">from</span> <span class="nn">.photokit</span> <span class="kn">import</span> <span class="p">(</span>
+        <span class="n">PHOTOS_VERSION_CURRENT</span><span class="p">,</span>
+        <span class="n">PHOTOS_VERSION_ORIGINAL</span><span class="p">,</span>
+        <span class="n">PHOTOS_VERSION_UNADJUSTED</span><span class="p">,</span>
+        <span class="n">PhotoKitFetchFailed</span><span class="p">,</span>
+        <span class="n">PhotoLibrary</span><span class="p">,</span>
+    <span class="p">)</span>
+
+
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span>
     <span class="s2">&quot;ExportError&quot;</span><span class="p">,</span>
     <span class="s2">&quot;ExportOptions&quot;</span><span class="p">,</span>
     <span class="s2">&quot;ExportResults&quot;</span><span class="p">,</span>
     <span class="s2">&quot;PhotoExporter&quot;</span><span class="p">,</span>
     <span class="s2">&quot;rename_jpeg_files&quot;</span><span class="p">,</span>
 <span class="p">]</span>
@@ -914,15 +921,14 @@
         <span class="n">_lock_filename</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">dest</span>
 
     <span class="k">def</span> <span class="nf">_should_update_photo</span><span class="p">(</span>
         <span class="bp">self</span><span class="p">,</span> <span class="n">src</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">dest</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span>
     <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">t</span><span class="o">.</span><span class="n">Literal</span><span class="p">[</span><span class="kc">True</span><span class="p">,</span> <span class="kc">False</span><span class="p">]:</span>
         <span class="sd">&quot;&quot;&quot;Return True if photo should be updated, else False&quot;&quot;&quot;</span>
-
         <span class="c1"># NOTE: The order of certain checks is important</span>
         <span class="c1"># read the comments below to understand why before changing</span>
 
         <span class="n">export_db</span> <span class="o">=</span> <span class="n">options</span><span class="o">.</span><span class="n">export_db</span>
         <span class="n">fileutil</span> <span class="o">=</span> <span class="n">options</span><span class="o">.</span><span class="n">fileutil</span>
 
         <span class="n">file_record</span> <span class="o">=</span> <span class="n">export_db</span><span class="o">.</span><span class="n">get_file_record</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
@@ -1374,15 +1380,15 @@
                     <span class="n">exif_results</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">write_exiftool_metadata_to_file</span><span class="p">(</span>
                         <span class="n">src</span><span class="p">,</span> <span class="n">dest</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="n">options</span>
                     <span class="p">)</span>
 
                 <span class="k">try</span><span class="p">:</span>
                     <span class="n">fileutil</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">dest_str</span><span class="p">)</span>
                     <span class="n">verbose</span><span class="p">(</span>
-                        <span class="sa">f</span><span class="s2">&quot;Exported </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filename</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">original_filename</span><span class="p">)</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filepath</span><span class="p">(</span><span class="n">dest_str</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+                        <span class="sa">f</span><span class="s2">&quot;Exported </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filename</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">original_filename</span><span class="p">)</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filepath</span><span class="p">(</span><span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">dest_str</span><span class="p">))</span><span class="si">}</span><span class="s2">&quot;</span>
                     <span class="p">)</span>
                 <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
                     <span class="k">raise</span> <span class="n">ExportError</span><span class="p">(</span>
                         <span class="sa">f</span><span class="s2">&quot;Error copying file </span><span class="si">{</span><span class="n">src</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="n">dest_str</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">lineno</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
                     <span class="p">)</span> <span class="kn">from</span> <span class="nn">e</span>
 
         <span class="n">results</span> <span class="o">=</span> <span class="n">ExportResults</span><span class="p">(</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -41,22 +41,22 @@
 
 import dataclasses
 import json
 import logging
 import os
 import pathlib
 import re
+import sys
 import typing as t
 from collections import namedtuple  # pylint: disable=syntax-error
 from dataclasses import asdict, dataclass
 from datetime import datetime
 from enum import Enum
 from types import SimpleNamespace
 
-import photoscript
 from mako.template import Template
 
 from ._constants import (
     _MAX_IPTC_KEYWORD_LEN,
     _OSXPHOTOS_NONE_SENTINEL,
     _TEMPLATE_DIR,
     _UNKNOWN_PERSON,
@@ -70,34 +70,41 @@
 )
 from ._version import __version__
 from .datetime_utils import datetime_tz_to_utc
 from .exiftool import ExifTool, ExifToolCaching, exiftool_can_write,
 get_exiftool_path
 from .export_db import ExportDB, ExportDBTemp
 from .fileutil import FileUtil
-from .photokit import (
-    PHOTOS_VERSION_CURRENT,
-    PHOTOS_VERSION_ORIGINAL,
-    PHOTOS_VERSION_UNADJUSTED,
-    PhotoKitFetchFailed,
-    PhotoLibrary,
-)
 from .phototemplate import RenderOptions
 from .rich_utils import add_rich_markup_tag
 from .uti import get_preferred_uti_extension
 from .utils import (
+    is_macos,
     hexdigest,
     increment_filename,
     increment_filename_with_count,
     lineno,
     list_directory,
     lock_filename,
+    normalize_fs_path,
     unlock_filename,
 )
 
+if is_macos:
+    import photoscript
+
+    from .photokit import (
+        PHOTOS_VERSION_CURRENT,
+        PHOTOS_VERSION_ORIGINAL,
+        PHOTOS_VERSION_UNADJUSTED,
+        PhotoKitFetchFailed,
+        PhotoLibrary,
+    )
+
+
 __all__ = [
     "ExportError",
     "ExportOptions",
     "ExportResults",
     "PhotoExporter",
     "rename_jpeg_files",
 ]
@@ -862,15 +869,14 @@
         _lock_filename(dest)
         return dest
 
     def _should_update_photo(
         self, src: pathlib.Path, dest: pathlib.Path, options: ExportOptions
     ) -> t.Literal[True, False]:
         """Return True if photo should be updated, else False"""
-
         # NOTE: The order of certain checks is important
         # read the comments below to understand why before changing
 
         export_db = options.export_db
         fileutil = options.fileutil
 
         file_record = export_db.get_file_record(dest)
@@ -1362,15 +1368,16 @@
                         src, dest, options=options
                     )
 
                 try:
                     fileutil.copy(src, dest_str)
                     verbose(
                         f"Exported {self._filename
-(self.photo.original_filename)} to {self._filepath(dest_str)}"
+(self.photo.original_filename)} to {self._filepath(normalize_fs_path
+(dest_str))}"
                     )
                 except Exception as e:
                     raise ExportError(
                         f"Error copying file {src} to {dest_str}: {e} ({lineno
 (__file__)})"
                     ) from e
```

#### docs/_modules/osxphotos/phototemplate.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.phototemplate - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos.phototemplate - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -214,15 +214,14 @@
 <span class="kn">import</span> <span class="nn">osxphotos.template_counter</span> <span class="k">as</span> <span class="nn">counter</span>
 
 <span class="kn">from</span> <span class="nn">._constants</span> <span class="kn">import</span> <span class="n">_UNKNOWN_PERSON</span><span class="p">,</span> <span class="n">TEXT_DETECTION_CONFIDENCE_THRESHOLD</span>
 <span class="kn">from</span> <span class="nn">._version</span> <span class="kn">import</span> <span class="n">__version__</span>
 <span class="kn">from</span> <span class="nn">.datetime_formatter</span> <span class="kn">import</span> <span class="n">DateTimeFormatter</span>
 <span class="kn">from</span> <span class="nn">.exiftool</span> <span class="kn">import</span> <span class="n">ExifToolCaching</span>
 <span class="kn">from</span> <span class="nn">.path_utils</span> <span class="kn">import</span> <span class="n">sanitize_dirname</span><span class="p">,</span> <span class="n">sanitize_filename</span><span class="p">,</span> <span class="n">sanitize_pathpart</span>
-<span class="kn">from</span> <span class="nn">.text_detection</span> <span class="kn">import</span> <span class="n">detect_text</span>
 <span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">expand_and_validate_filepath</span><span class="p">,</span> <span class="n">load_function</span><span class="p">,</span> <span class="n">uuid_to_shortuuid</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span>
     <span class="s2">&quot;RenderOptions&quot;</span><span class="p">,</span>
     <span class="s2">&quot;PhotoTemplateParser&quot;</span><span class="p">,</span>
     <span class="s2">&quot;PhotoTemplate&quot;</span><span class="p">,</span>
     <span class="s2">&quot;parse_default_kv&quot;</span><span class="p">,</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -56,15 +56,14 @@
 import osxphotos.template_counter as counter
 
 from ._constants import _UNKNOWN_PERSON, TEXT_DETECTION_CONFIDENCE_THRESHOLD
 from ._version import __version__
 from .datetime_formatter import DateTimeFormatter
 from .exiftool import ExifToolCaching
 from .path_utils import sanitize_dirname, sanitize_filename, sanitize_pathpart
-from .text_detection import detect_text
 from .utils import expand_and_validate_filepath, load_function,
 uuid_to_shortuuid
 
 __all__ = [
     "RenderOptions",
     "PhotoTemplateParser",
     "PhotoTemplate",
```

#### docs/_modules/osxphotos/fileutil.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.fileutil - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos.fileutil - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -202,17 +202,19 @@
 <span class="kn">import</span> <span class="nn">shutil</span>
 <span class="kn">import</span> <span class="nn">stat</span>
 <span class="kn">import</span> <span class="nn">tempfile</span>
 <span class="kn">import</span> <span class="nn">typing</span> <span class="k">as</span> <span class="nn">t</span>
 <span class="kn">from</span> <span class="nn">abc</span> <span class="kn">import</span> <span class="n">ABC</span><span class="p">,</span> <span class="n">abstractmethod</span>
 <span class="kn">from</span> <span class="nn">tempfile</span> <span class="kn">import</span> <span class="n">TemporaryDirectory</span>
 
-<span class="kn">import</span> <span class="nn">Foundation</span>
-
 <span class="kn">from</span> <span class="nn">.imageconverter</span> <span class="kn">import</span> <span class="n">ImageConverter</span>
+<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">is_macos</span><span class="p">,</span> <span class="n">normalize_fs_path</span>
+
+<span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
+    <span class="kn">import</span> <span class="nn">Foundation</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;FileUtilABC&quot;</span><span class="p">,</span> <span class="s2">&quot;FileUtilMacOS&quot;</span><span class="p">,</span> <span class="s2">&quot;FileUtilShUtil&quot;</span><span class="p">,</span> <span class="s2">&quot;FileUtil&quot;</span><span class="p">,</span> <span class="s2">&quot;FileUtilNoOp&quot;</span><span class="p">]</span>
 
 
 <span class="k">class</span> <span class="nc">FileUtilABC</span><span class="p">(</span><span class="n">ABC</span><span class="p">):</span>
     <span class="sd">&quot;&quot;&quot;Abstract base class for FileUtil&quot;&quot;&quot;</span>
 
@@ -283,14 +285,17 @@
 <span class="sd">        src: source path as string</span>
 <span class="sd">        dest: destination path as string</span>
 <span class="sd">        Raises exception if linking fails or either path is None&quot;&quot;&quot;</span>
 
         <span class="k">if</span> <span class="n">src</span> <span class="ow">is</span> <span class="kc">None</span> <span class="ow">or</span> <span class="n">dest</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;src and dest must not be None&quot;</span><span class="p">,</span> <span class="n">src</span><span class="p">,</span> <span class="n">dest</span><span class="p">)</span>
 
+        <span class="n">src</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">src</span><span class="p">)</span>
+        <span class="n">dest</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
+
         <span class="k">if</span> <span class="ow">not</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">src</span><span class="p">):</span>
             <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="s2">&quot;src file does not appear to exist&quot;</span><span class="p">,</span> <span class="n">src</span><span class="p">)</span>
 
         <span class="k">try</span><span class="p">:</span>
             <span class="n">os</span><span class="o">.</span><span class="n">link</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">dest</span><span class="p">)</span>
         <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
             <span class="k">raise</span> <span class="n">e</span> <span class="kn">from</span> <span class="nn">e</span>
@@ -308,14 +313,17 @@
 <span class="sd">        Returns:</span>
 <span class="sd">            True if copy succeeded</span>
 
 <span class="sd">        Raises:</span>
 <span class="sd">            OSError if copy fails</span>
 <span class="sd">            TypeError if either path is None</span>
 <span class="sd">        &quot;&quot;&quot;</span>
+        <span class="n">src</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">src</span><span class="p">)</span>
+        <span class="n">dest</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
+
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">):</span>
             <span class="n">src</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">src</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">dest</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">):</span>
             <span class="n">dest</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">dest</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
@@ -328,30 +336,33 @@
         <span class="k">if</span> <span class="ow">not</span> <span class="n">error</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
             <span class="k">raise</span> <span class="ne">OSError</span><span class="p">(</span><span class="n">error</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
         <span class="k">return</span> <span class="kc">True</span>
 
     <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">unlink</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">filepath</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;unlink filepath; if it&#39;s pathlib.Path, use Path.unlink, otherwise use os.unlink&quot;&quot;&quot;</span>
+        <span class="n">filepath</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">filepath</span><span class="p">)</span>
         <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">filepath</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">):</span>
             <span class="n">filepath</span><span class="o">.</span><span class="n">unlink</span><span class="p">()</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">os</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">filepath</span><span class="p">)</span>
 
     <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">rmdir</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">dirpath</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;remove directory filepath; dirpath must be empty&quot;&quot;&quot;</span>
+        <span class="n">dirpath</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">dirpath</span><span class="p">)</span>
         <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">dirpath</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">):</span>
             <span class="n">dirpath</span><span class="o">.</span><span class="n">rmdir</span><span class="p">()</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">os</span><span class="o">.</span><span class="n">rmdir</span><span class="p">(</span><span class="n">dirpath</span><span class="p">)</span>
 
     <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">utime</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">path</span><span class="p">,</span> <span class="n">times</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Set the access and modified time of path.&quot;&quot;&quot;</span>
+        <span class="n">path</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
         <span class="n">os</span><span class="o">.</span><span class="n">utime</span><span class="p">(</span><span class="n">path</span><span class="p">,</span> <span class="n">times</span><span class="o">=</span><span class="n">times</span><span class="p">)</span>
 
     <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">cmp</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">f1</span><span class="p">,</span> <span class="n">f2</span><span class="p">,</span> <span class="n">mtime1</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Does shallow compare (file signatures) of f1 to file f2.</span>
 <span class="sd">        Arguments:</span>
 <span class="sd">        f1 --  File name</span>
@@ -359,14 +370,17 @@
 <span class="sd">        mtime1 -- optional, pass alternate file modification timestamp for f1; will be converted to int</span>
 
 <span class="sd">        Return value:</span>
 <span class="sd">        True if the file signatures as returned by stat are the same, False otherwise.</span>
 <span class="sd">        Does not do a byte-by-byte comparison.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
 
+        <span class="n">f1</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">f1</span><span class="p">)</span>
+        <span class="n">f2</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">f2</span><span class="p">)</span>
+
         <span class="n">s1</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_sig</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">stat</span><span class="p">(</span><span class="n">f1</span><span class="p">))</span>
         <span class="k">if</span> <span class="n">mtime1</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">s1</span> <span class="o">=</span> <span class="p">(</span><span class="n">s1</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">s1</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="nb">int</span><span class="p">(</span><span class="n">mtime1</span><span class="p">))</span>
         <span class="n">s2</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_sig</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">stat</span><span class="p">(</span><span class="n">f2</span><span class="p">))</span>
         <span class="k">if</span> <span class="n">s1</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="n">stat</span><span class="o">.</span><span class="n">S_IFREG</span> <span class="ow">or</span> <span class="n">s2</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="n">stat</span><span class="o">.</span><span class="n">S_IFREG</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">False</span>
         <span class="k">return</span> <span class="n">s1</span> <span class="o">==</span> <span class="n">s2</span>
@@ -381,36 +395,40 @@
 <span class="sd">        Return value:</span>
 <span class="sd">        True if the files are the same, False otherwise.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="n">s2</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">False</span>
 
+        <span class="n">f1</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">f1</span><span class="p">)</span>
         <span class="n">s1</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_sig</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">stat</span><span class="p">(</span><span class="n">f1</span><span class="p">))</span>
         <span class="k">if</span> <span class="n">s1</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="n">stat</span><span class="o">.</span><span class="n">S_IFREG</span> <span class="ow">or</span> <span class="n">s2</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="n">stat</span><span class="o">.</span><span class="n">S_IFREG</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">False</span>
         <span class="k">return</span> <span class="n">s1</span> <span class="o">==</span> <span class="n">s2</span>
 
     <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">file_sig</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">f1</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;return os.stat signature for file f1 as tuple of (mode, size, mtime)&quot;&quot;&quot;</span>
+        <span class="n">f1</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">f1</span><span class="p">)</span>
         <span class="k">return</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_sig</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">stat</span><span class="p">(</span><span class="n">f1</span><span class="p">))</span>
 
     <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">convert_to_jpeg</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">src_file</span><span class="p">,</span> <span class="n">dest_file</span><span class="p">,</span> <span class="n">compression_quality</span><span class="o">=</span><span class="mf">1.0</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;converts image file src_file to jpeg format as dest_file</span>
 
 <span class="sd">        Args:</span>
 <span class="sd">            src_file: image file to convert</span>
 <span class="sd">            dest_file: destination path to write converted file to</span>
 <span class="sd">            compression quality: JPEG compression quality in range 0.0 &lt;= compression_quality &lt;= 1.0; default 1.0 (best quality)</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">            True if success, otherwise False</span>
 <span class="sd">        &quot;&quot;&quot;</span>
+        <span class="n">src_file</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">src_file</span><span class="p">)</span>
+        <span class="n">dest_file</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">dest_file</span><span class="p">)</span>
         <span class="n">converter</span> <span class="o">=</span> <span class="n">ImageConverter</span><span class="p">()</span>
         <span class="k">return</span> <span class="n">converter</span><span class="o">.</span><span class="n">write_jpeg</span><span class="p">(</span>
             <span class="n">src_file</span><span class="p">,</span> <span class="n">dest_file</span><span class="p">,</span> <span class="n">compression_quality</span><span class="o">=</span><span class="n">compression_quality</span>
         <span class="p">)</span>
 
     <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">rename</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">src</span><span class="p">,</span> <span class="n">dest</span><span class="p">):</span>
@@ -420,14 +438,16 @@
 <span class="sd">            src: path to source file</span>
 <span class="sd">            dest: path to destination file</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">            Name of renamed file (dest)</span>
 
 <span class="sd">        &quot;&quot;&quot;</span>
+        <span class="n">src</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">src</span><span class="p">)</span>
+        <span class="n">dest</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
         <span class="n">os</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">src</span><span class="p">),</span> <span class="nb">str</span><span class="p">(</span><span class="n">dest</span><span class="p">))</span>
         <span class="k">return</span> <span class="n">dest</span>
 
     <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">tmpdir</span><span class="p">(</span>
         <span class="bp">cls</span><span class="p">,</span> <span class="n">prefix</span><span class="p">:</span> <span class="n">t</span><span class="o">.</span><span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="nb">dir</span><span class="p">:</span> <span class="n">t</span><span class="o">.</span><span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">tempfile</span><span class="o">.</span><span class="n">TemporaryDirectory</span><span class="p">:</span>
@@ -464,14 +484,17 @@
 <span class="sd">        Returns:</span>
 <span class="sd">            True if copy succeeded</span>
 
 <span class="sd">        Raises:</span>
 <span class="sd">            OSError if copy fails</span>
 <span class="sd">            TypeError if either path is None</span>
 <span class="sd">        &quot;&quot;&quot;</span>
+        <span class="n">src</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">src</span><span class="p">)</span>
+        <span class="n">dest</span> <span class="o">=</span> <span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
+
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">):</span>
             <span class="n">src</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">src</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">dest</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">):</span>
             <span class="n">dest</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">dest</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
@@ -481,15 +504,15 @@
             <span class="n">shutil</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">src</span><span class="p">),</span> <span class="nb">str</span><span class="p">(</span><span class="n">dest</span><span class="p">))</span>
         <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
             <span class="k">raise</span> <span class="ne">OSError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error copying </span><span class="si">{</span><span class="n">src</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="n">dest</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span> <span class="kn">from</span> <span class="nn">e</span>
 
         <span class="k">return</span> <span class="kc">True</span>
 
 
-<div class="viewcode-block" id="FileUtil"><a class="viewcode-back" href="../../reference.html#osxphotos.FileUtil">[docs]</a><span class="k">class</span> <span class="nc">FileUtil</span><span class="p">(</span><span class="n">FileUtilMacOS</span><span class="p">):</span>
+<div class="viewcode-block" id="FileUtil"><a class="viewcode-back" href="../../reference.html#osxphotos.FileUtil">[docs]</a><span class="k">class</span> <span class="nc">FileUtil</span><span class="p">(</span><span class="n">FileUtilShUtil</span><span class="p">):</span>
     <span class="sd">&quot;&quot;&quot;Various file utilities&quot;&quot;&quot;</span>
 
     <span class="k">pass</span></div>
 
 
 <div class="viewcode-block" id="FileUtilNoOp"><a class="viewcode-back" href="../../reference.html#osxphotos.FileUtilNoOp">[docs]</a><span class="k">class</span> <span class="nc">FileUtilNoOp</span><span class="p">(</span><span class="n">FileUtil</span><span class="p">):</span>
     <span class="sd">&quot;&quot;&quot;No-Op implementation of FileUtil for testing / dry-run mode</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -43,17 +43,19 @@
 import shutil
 import stat
 import tempfile
 import typing as t
 from abc import ABC, abstractmethod
 from tempfile import TemporaryDirectory
 
-import Foundation
-
 from .imageconverter import ImageConverter
+from .utils import is_macos, normalize_fs_path
+
+if is_macos:
+    import Foundation
 
 __all__ = ["FileUtilABC", "FileUtilMacOS", "FileUtilShUtil", "FileUtil",
 "FileUtilNoOp"]
 
 
 class FileUtilABC(ABC):
     """Abstract base class for FileUtil"""
@@ -125,14 +127,17 @@
         src: source path as string
         dest: destination path as string
         Raises exception if linking fails or either path is None"""
 
         if src is None or dest is None:
             raise ValueError("src and dest must not be None", src, dest)
 
+        src = normalize_fs_path(src)
+        dest = normalize_fs_path(dest)
+
         if not os.path.isfile(src):
             raise FileNotFoundError("src file does not appear to exist", src)
 
         try:
             os.link(src, dest)
         except Exception as e:
             raise e from e
@@ -151,14 +156,17 @@
         Returns:
             True if copy succeeded
 
         Raises:
             OSError if copy fails
             TypeError if either path is None
         """
+        src = normalize_fs_path(src)
+        dest = normalize_fs_path(dest)
+
         if not isinstance(src, pathlib.Path):
             src = pathlib.Path(src)
 
         if not isinstance(dest, pathlib.Path):
             dest = pathlib.Path(dest)
 
         if dest.is_dir():
@@ -172,30 +180,33 @@
             raise OSError(error[1])
         return True
 
     @classmethod
     def unlink(cls, filepath):
         """unlink filepath; if it's pathlib.Path, use Path.unlink, otherwise
 use os.unlink"""
+        filepath = normalize_fs_path(filepath)
         if isinstance(filepath, pathlib.Path):
             filepath.unlink()
         else:
             os.unlink(filepath)
 
     @classmethod
     def rmdir(cls, dirpath):
         """remove directory filepath; dirpath must be empty"""
+        dirpath = normalize_fs_path(dirpath)
         if isinstance(dirpath, pathlib.Path):
             dirpath.rmdir()
         else:
             os.rmdir(dirpath)
 
     @classmethod
     def utime(cls, path, times):
         """Set the access and modified time of path."""
+        path = normalize_fs_path(path)
         os.utime(path, times=times)
 
     @classmethod
     def cmp(cls, f1, f2, mtime1=None):
         """Does shallow compare (file signatures) of f1 to file f2.
         Arguments:
         f1 --  File name
@@ -205,14 +216,17 @@
 
         Return value:
         True if the file signatures as returned by stat are the same, False
 otherwise.
         Does not do a byte-by-byte comparison.
         """
 
+        f1 = normalize_fs_path(f1)
+        f2 = normalize_fs_path(f2)
+
         s1 = cls._sig(os.stat(f1))
         if mtime1 is not None:
             s1 = (s1[0], s1[1], int(mtime1))
         s2 = cls._sig(os.stat(f2))
         if s1[0] != stat.S_IFREG or s2[0] != stat.S_IFREG:
             return False
         return s1 == s2
@@ -227,23 +241,25 @@
         Return value:
         True if the files are the same, False otherwise.
         """
 
         if not s2:
             return False
 
+        f1 = normalize_fs_path(f1)
         s1 = cls._sig(os.stat(f1))
         if s1[0] != stat.S_IFREG or s2[0] != stat.S_IFREG:
             return False
         return s1 == s2
 
     @classmethod
     def file_sig(cls, f1):
         """return os.stat signature for file f1 as tuple of (mode, size,
 mtime)"""
+        f1 = normalize_fs_path(f1)
         return cls._sig(os.stat(f1))
 
     @classmethod
     def convert_to_jpeg(cls, src_file, dest_file, compression_quality=1.0):
         """converts image file src_file to jpeg format as dest_file
 
         Args:
@@ -251,14 +267,16 @@
             dest_file: destination path to write converted file to
             compression quality: JPEG compression quality in range 0.0 <=
 compression_quality <= 1.0; default 1.0 (best quality)
 
         Returns:
             True if success, otherwise False
         """
+        src_file = normalize_fs_path(src_file)
+        dest_file = normalize_fs_path(dest_file)
         converter = ImageConverter()
         return converter.write_jpeg(
             src_file, dest_file, compression_quality=compression_quality
         )
 
     @classmethod
     def rename(cls, src, dest):
@@ -268,14 +286,16 @@
             src: path to source file
             dest: path to destination file
 
         Returns:
             Name of renamed file (dest)
 
         """
+        src = normalize_fs_path(src)
+        dest = normalize_fs_path(dest)
         os.rename(str(src), str(dest))
         return dest
 
     @classmethod
     def tmpdir(
         cls, prefix: t.Optional[str] = None, dir: t.Optional[str] = None
     ) -> tempfile.TemporaryDirectory:
@@ -318,14 +338,17 @@
         Returns:
             True if copy succeeded
 
         Raises:
             OSError if copy fails
             TypeError if either path is None
         """
+        src = normalize_fs_path(src)
+        dest = normalize_fs_path(dest)
+
         if not isinstance(src, pathlib.Path):
             src = pathlib.Path(src)
 
         if not isinstance(dest, pathlib.Path):
             dest = pathlib.Path(dest)
 
         if dest.is_dir():
@@ -335,15 +358,15 @@
             shutil.copy(str(src), str(dest))
         except Exception as e:
             raise OSError(f"Error copying {src} to {dest}: {e}") from e
 
         return True
 
 
-[docs]class FileUtil(FileUtilMacOS):
+[docs]class FileUtil(FileUtilShUtil):
     """Various file utilities"""
 
     pass
 
 
 
 [docs]class FileUtilNoOp(FileUtil):
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoinfo - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos.photoinfo - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -213,15 +213,14 @@
 <span class="kn">import</span> <span class="nn">re</span>
 <span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">timedelta</span><span class="p">,</span> <span class="n">timezone</span>
 <span class="kn">from</span> <span class="nn">functools</span> <span class="kn">import</span> <span class="n">cached_property</span>
 <span class="kn">from</span> <span class="nn">types</span> <span class="kn">import</span> <span class="n">SimpleNamespace</span>
 <span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span><span class="p">,</span> <span class="n">Dict</span><span class="p">,</span> <span class="n">Optional</span>
 
 <span class="kn">import</span> <span class="nn">yaml</span>
-<span class="kn">from</span> <span class="nn">osxmetadata</span> <span class="kn">import</span> <span class="n">OSXMetaData</span>
 
 <span class="kn">import</span> <span class="nn">osxphotos</span>
 
 <span class="kn">from</span> <span class="nn">._constants</span> <span class="kn">import</span> <span class="p">(</span>
     <span class="n">_DB_TABLE_NAMES</span><span class="p">,</span>
     <span class="n">_MOVIE_TYPE</span><span class="p">,</span>
     <span class="n">_PHOTO_TYPE</span><span class="p">,</span>
@@ -252,22 +251,26 @@
 <span class="kn">from</span> <span class="nn">.adjustmentsinfo</span> <span class="kn">import</span> <span class="n">AdjustmentsInfo</span>
 <span class="kn">from</span> <span class="nn">.albuminfo</span> <span class="kn">import</span> <span class="n">AlbumInfo</span><span class="p">,</span> <span class="n">ImportInfo</span><span class="p">,</span> <span class="n">ProjectInfo</span>
 <span class="kn">from</span> <span class="nn">.exifinfo</span> <span class="kn">import</span> <span class="n">ExifInfo</span>
 <span class="kn">from</span> <span class="nn">.exiftool</span> <span class="kn">import</span> <span class="n">ExifToolCaching</span><span class="p">,</span> <span class="n">get_exiftool_path</span>
 <span class="kn">from</span> <span class="nn">.momentinfo</span> <span class="kn">import</span> <span class="n">MomentInfo</span>
 <span class="kn">from</span> <span class="nn">.personinfo</span> <span class="kn">import</span> <span class="n">FaceInfo</span><span class="p">,</span> <span class="n">PersonInfo</span>
 <span class="kn">from</span> <span class="nn">.photoexporter</span> <span class="kn">import</span> <span class="n">ExportOptions</span><span class="p">,</span> <span class="n">PhotoExporter</span>
+<span class="kn">from</span> <span class="nn">.phototables</span> <span class="kn">import</span> <span class="n">PhotoTables</span>
 <span class="kn">from</span> <span class="nn">.phototemplate</span> <span class="kn">import</span> <span class="n">PhotoTemplate</span><span class="p">,</span> <span class="n">RenderOptions</span>
 <span class="kn">from</span> <span class="nn">.placeinfo</span> <span class="kn">import</span> <span class="n">PlaceInfo4</span><span class="p">,</span> <span class="n">PlaceInfo5</span>
 <span class="kn">from</span> <span class="nn">.query_builder</span> <span class="kn">import</span> <span class="n">get_query</span>
 <span class="kn">from</span> <span class="nn">.scoreinfo</span> <span class="kn">import</span> <span class="n">ScoreInfo</span>
 <span class="kn">from</span> <span class="nn">.searchinfo</span> <span class="kn">import</span> <span class="n">SearchInfo</span>
-<span class="kn">from</span> <span class="nn">.text_detection</span> <span class="kn">import</span> <span class="n">detect_text</span>
 <span class="kn">from</span> <span class="nn">.uti</span> <span class="kn">import</span> <span class="n">get_preferred_uti_extension</span><span class="p">,</span> <span class="n">get_uti_for_extension</span>
-<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">_get_resource_loc</span><span class="p">,</span> <span class="n">hexdigest</span><span class="p">,</span> <span class="n">list_directory</span>
+<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">_get_resource_loc</span><span class="p">,</span> <span class="n">assert_macos</span><span class="p">,</span> <span class="n">is_macos</span><span class="p">,</span> <span class="n">hexdigest</span><span class="p">,</span> <span class="n">list_directory</span>
+
+<span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
+    <span class="kn">from</span> <span class="nn">osxmetadata</span> <span class="kn">import</span> <span class="n">OSXMetaData</span>
+    <span class="kn">from</span> <span class="nn">.text_detection</span> <span class="kn">import</span> <span class="n">detect_text</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;PhotoInfo&quot;</span><span class="p">,</span> <span class="s2">&quot;PhotoInfoNone&quot;</span><span class="p">,</span> <span class="s2">&quot;frozen_photoinfo_factory&quot;</span><span class="p">]</span>
 
 <span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s2">&quot;osxphotos&quot;</span><span class="p">)</span>
 
 
 <div class="viewcode-block" id="PhotoInfo"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo">[docs]</a><span class="k">class</span> <span class="nc">PhotoInfo</span><span class="p">:</span>
@@ -1653,14 +1656,16 @@
                 <span class="k">for</span> <span class="n">text</span><span class="p">,</span> <span class="n">confidence</span> <span class="ow">in</span> <span class="n">detected_text</span>
                 <span class="k">if</span> <span class="n">confidence</span> <span class="o">&gt;=</span> <span class="n">confidence_threshold</span>
             <span class="p">]</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_detected_text_cache</span><span class="p">[</span><span class="n">confidence_threshold</span><span class="p">]</span></div>
 
     <span class="k">def</span> <span class="nf">_detected_text</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;detect text in photo, either from cached extended attribute or by attempting text detection&quot;&quot;&quot;</span>
+        <span class="n">assert_macos</span><span class="p">()</span>
+
         <span class="n">path</span> <span class="o">=</span> <span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">path_edited</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">hasadjustments</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_edited</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">path</span>
         <span class="p">)</span>
         <span class="n">path</span> <span class="o">=</span> <span class="n">path</span> <span class="ow">or</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_derivatives</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_derivatives</span> <span class="k">else</span> <span class="kc">None</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
             <span class="k">return</span> <span class="p">[]</span>
 
@@ -2086,14 +2091,18 @@
             <span class="c1"># but do not sort certain items like location</span>
             <span class="k">if</span> <span class="n">k</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;location&quot;</span><span class="p">]:</span>
                 <span class="k">continue</span>
             <span class="k">if</span> <span class="n">v</span> <span class="ow">and</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">v</span><span class="p">,</span> <span class="p">(</span><span class="nb">list</span><span class="p">,</span> <span class="nb">tuple</span><span class="p">))</span> <span class="ow">and</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">v</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="nb">dict</span><span class="p">):</span>
                 <span class="n">dict_data</span><span class="p">[</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">v</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">v</span><span class="p">:</span> <span class="n">v</span> <span class="k">if</span> <span class="n">v</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="k">else</span> <span class="s2">&quot;&quot;</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">dict_data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">)</span></div>
 
+<div class="viewcode-block" id="PhotoInfo.tables"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo.tables">[docs]</a>    <span class="k">def</span> <span class="nf">tables</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">PhotoTables</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Return PhotoTables object to provide access database tables associated with this photo (Photos 5+)&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="kc">None</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_photos_ver</span> <span class="o">&lt;</span> <span class="mi">5</span> <span class="k">else</span> <span class="n">PhotoTables</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span></div>
+
     <span class="k">def</span> <span class="nf">_json_hexdigest</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;JSON for use by hexdigest()&quot;&quot;&quot;</span>
 
         <span class="c1"># This differs from json() because hexdigest must not change if metadata changed</span>
         <span class="c1"># With json(), sort order of lists of dicts is not consistent but these aren&#39;t needed</span>
         <span class="c1"># for computing hexdigest so we can ignore them</span>
         <span class="c1"># also don&#39;t use visible because it changes based on Photos UI state</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -55,15 +55,14 @@
 import re
 from datetime import timedelta, timezone
 from functools import cached_property
 from types import SimpleNamespace
 from typing import Any, Dict, Optional
 
 import yaml
-from osxmetadata import OSXMetaData
 
 import osxphotos
 
 from ._constants import (
     _DB_TABLE_NAMES,
     _MOVIE_TYPE,
     _PHOTO_TYPE,
@@ -94,22 +93,27 @@
 from .adjustmentsinfo import AdjustmentsInfo
 from .albuminfo import AlbumInfo, ImportInfo, ProjectInfo
 from .exifinfo import ExifInfo
 from .exiftool import ExifToolCaching, get_exiftool_path
 from .momentinfo import MomentInfo
 from .personinfo import FaceInfo, PersonInfo
 from .photoexporter import ExportOptions, PhotoExporter
+from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate, RenderOptions
 from .placeinfo import PlaceInfo4, PlaceInfo5
 from .query_builder import get_query
 from .scoreinfo import ScoreInfo
 from .searchinfo import SearchInfo
-from .text_detection import detect_text
 from .uti import get_preferred_uti_extension, get_uti_for_extension
-from .utils import _get_resource_loc, hexdigest, list_directory
+from .utils import _get_resource_loc, assert_macos, is_macos, hexdigest,
+list_directory
+
+if is_macos:
+    from osxmetadata import OSXMetaData
+    from .text_detection import detect_text
 
 __all__ = ["PhotoInfo", "PhotoInfoNone", "frozen_photoinfo_factory"]
 
 logger = logging.getLogger("osxphotos")
 
 
 [docs]class PhotoInfo:
@@ -1604,14 +1608,16 @@
             ]
             return self._detected_text_cache[confidence_threshold]
 
 
     def _detected_text(self):
         """detect text in photo, either from cached extended attribute or by
 attempting text detection"""
+        assert_macos()
+
         path = (
             self.path_edited if self.hasadjustments and self.path_edited else
 self.path
         )
         path = path or self.path_derivatives[0] if self.path_derivatives else
 None
         if not path:
@@ -2088,14 +2094,20 @@
 dict):
                 dict_data[k] = sorted(v, key=lambda v: v if v is not None else
 "")
         return json.dumps(dict_data, sort_keys=True, default=default,
 indent=indent)
 
 
+[docs]    def tables(self) -> PhotoTables:
+        """Return PhotoTables object to provide access database tables
+associated with this photo (Photos 5+)"""
+        return None if self._db._photos_ver < 5 else PhotoTables(self)
+
+
     def _json_hexdigest(self):
         """JSON for use by hexdigest()"""
 
         # This differs from json() because hexdigest must not change if
 metadata changed
         # With json(), sort order of lists of dicts is not consistent but these
 aren't needed
```

#### docs/_modules/osxphotos/photosdb/photosdb.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb.photosdb - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -214,15 +214,14 @@
 <span class="kn">from</span> <span class="nn">collections</span> <span class="kn">import</span> <span class="n">OrderedDict</span>
 <span class="kn">from</span> <span class="nn">collections.abc</span> <span class="kn">import</span> <span class="n">Iterable</span>
 <span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span><span class="p">,</span> <span class="n">timedelta</span><span class="p">,</span> <span class="n">timezone</span>
 <span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span><span class="p">,</span> <span class="n">List</span><span class="p">,</span> <span class="n">Optional</span>
 <span class="kn">from</span> <span class="nn">unicodedata</span> <span class="kn">import</span> <span class="n">normalize</span>
 
 <span class="kn">import</span> <span class="nn">bitmath</span>
-<span class="kn">import</span> <span class="nn">photoscript</span>
 <span class="kn">from</span> <span class="nn">rich</span> <span class="kn">import</span> <span class="nb">print</span>
 
 <span class="kn">from</span> <span class="nn">.._constants</span> <span class="kn">import</span> <span class="p">(</span>
     <span class="n">_DB_TABLE_NAMES</span><span class="p">,</span>
     <span class="n">_MOVIE_TYPE</span><span class="p">,</span>
     <span class="n">_PHOTO_TYPE</span><span class="p">,</span>
     <span class="n">_PHOTOS_3_VERSION</span><span class="p">,</span>
@@ -255,21 +254,25 @@
 <span class="kn">from</span> <span class="nn">..photoinfo</span> <span class="kn">import</span> <span class="n">PhotoInfo</span>
 <span class="kn">from</span> <span class="nn">..phototemplate</span> <span class="kn">import</span> <span class="n">RenderOptions</span>
 <span class="kn">from</span> <span class="nn">..queryoptions</span> <span class="kn">import</span> <span class="n">QueryOptions</span>
 <span class="kn">from</span> <span class="nn">..rich_utils</span> <span class="kn">import</span> <span class="n">add_rich_markup_tag</span>
 <span class="kn">from</span> <span class="nn">..sqlite_utils</span> <span class="kn">import</span> <span class="n">sqlite_db_is_locked</span><span class="p">,</span> <span class="n">sqlite_open_ro</span>
 <span class="kn">from</span> <span class="nn">..utils</span> <span class="kn">import</span> <span class="p">(</span>
     <span class="n">_check_file_exists</span><span class="p">,</span>
+    <span class="n">is_macos</span><span class="p">,</span>
     <span class="n">get_macos_version</span><span class="p">,</span>
     <span class="n">get_last_library_path</span><span class="p">,</span>
     <span class="n">noop</span><span class="p">,</span>
     <span class="n">normalize_unicode</span><span class="p">,</span>
 <span class="p">)</span>
 <span class="kn">from</span> <span class="nn">.photosdb_utils</span> <span class="kn">import</span> <span class="n">get_db_model_version</span><span class="p">,</span> <span class="n">get_db_version</span>
 
+<span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
+    <span class="kn">import</span> <span class="nn">photoscript</span>
+
 <span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s2">&quot;osxphotos&quot;</span><span class="p">)</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;PhotosDB&quot;</span><span class="p">]</span>
 
 <span class="c1"># TODO: Add test for imageTimeZoneOffsetSeconds = None</span>
 <span class="c1"># TODO: Add test for __str__</span>
 <span class="c1"># TODO: Add special albums and magic albums</span>
@@ -311,16 +314,16 @@
 <span class="sd">        Raises:</span>
 <span class="sd">            FileNotFoundError if dbfile is not a valid Photos library.</span>
 <span class="sd">            TypeError if verbose is not None and not callable.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
 
         <span class="c1"># Check OS version</span>
         <span class="n">system</span> <span class="o">=</span> <span class="n">platform</span><span class="o">.</span><span class="n">system</span><span class="p">()</span>
-        <span class="p">(</span><span class="n">ver</span><span class="p">,</span> <span class="n">major</span><span class="p">,</span> <span class="n">_</span><span class="p">)</span> <span class="o">=</span> <span class="n">get_macos_version</span><span class="p">()</span>
-        <span class="k">if</span> <span class="n">system</span> <span class="o">!=</span> <span class="s2">&quot;Darwin&quot;</span> <span class="ow">or</span> <span class="p">((</span><span class="n">ver</span><span class="p">,</span> <span class="n">major</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">_TESTED_OS_VERSIONS</span><span class="p">):</span>
+        <span class="p">(</span><span class="n">ver</span><span class="p">,</span> <span class="n">major</span><span class="p">,</span> <span class="n">_</span><span class="p">)</span> <span class="o">=</span> <span class="n">get_macos_version</span><span class="p">()</span> <span class="k">if</span> <span class="n">is_macos</span> <span class="k">else</span> <span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="kc">None</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+        <span class="k">if</span> <span class="n">system</span> <span class="o">==</span> <span class="s2">&quot;Darwin&quot;</span> <span class="ow">and</span> <span class="p">((</span><span class="n">ver</span><span class="p">,</span> <span class="n">major</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">_TESTED_OS_VERSIONS</span><span class="p">):</span>
             <span class="n">logging</span><span class="o">.</span><span class="n">warning</span><span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;WARNING: This module has only been tested with macOS versions &quot;</span>
                 <span class="sa">f</span><span class="s2">&quot;[</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">v</span><span class="si">}</span><span class="s1">.</span><span class="si">{</span><span class="n">m</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="p">(</span><span class="n">v</span><span class="p">,</span> <span class="n">m</span><span class="p">)</span> <span class="ow">in</span> <span class="n">_TESTED_OS_VERSIONS</span><span class="p">)</span><span class="si">}</span><span class="s2">]: &quot;</span>
                 <span class="sa">f</span><span class="s2">&quot;you have </span><span class="si">{</span><span class="n">system</span><span class="si">}</span><span class="s2">, OS version: </span><span class="si">{</span><span class="n">ver</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">major</span><span class="si">}</span><span class="s2">&quot;</span>
             <span class="p">)</span>
 
         <span class="k">if</span> <span class="n">verbose</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -55,15 +55,14 @@
 from collections import OrderedDict
 from collections.abc import Iterable
 from datetime import datetime, timedelta, timezone
 from typing import Any, List, Optional
 from unicodedata import normalize
 
 import bitmath
-import photoscript
 from rich import print
 
 from .._constants import (
     _DB_TABLE_NAMES,
     _MOVIE_TYPE,
     _PHOTO_TYPE,
     _PHOTOS_3_VERSION,
@@ -96,21 +95,25 @@
 from ..photoinfo import PhotoInfo
 from ..phototemplate import RenderOptions
 from ..queryoptions import QueryOptions
 from ..rich_utils import add_rich_markup_tag
 from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
 from ..utils import (
     _check_file_exists,
+    is_macos,
     get_macos_version,
     get_last_library_path,
     noop,
     normalize_unicode,
 )
 from .photosdb_utils import get_db_model_version, get_db_version
 
+if is_macos:
+    import photoscript
+
 logger = logging.getLogger("osxphotos")
 
 __all__ = ["PhotosDB"]
 
 # TODO: Add test for imageTimeZoneOffsetSeconds = None
 # TODO: Add test for __str__
 # TODO: Add special albums and magic albums
@@ -157,16 +160,17 @@
         Raises:
             FileNotFoundError if dbfile is not a valid Photos library.
             TypeError if verbose is not None and not callable.
         """
 
         # Check OS version
         system = platform.system()
-        (ver, major, _) = get_macos_version()
-        if system != "Darwin" or ((ver, major) not in _TESTED_OS_VERSIONS):
+        (ver, major, _) = get_macos_version() if is_macos else (None, None,
+None)
+        if system == "Darwin" and ((ver, major) not in _TESTED_OS_VERSIONS):
             logging.warning(
                 f"WARNING: This module has only been tested with macOS versions
 "
                 f"[{', '.join(f'{v}.{m}' for (v, m) in _TESTED_OS_VERSIONS)}]:
 "
                 f"you have {system}, OS version: {ver}.{major}"
             )
```

#### docs/_modules/osxphotos/photosalbum.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosalbum - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos.photosalbum - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -195,20 +195,23 @@
         </div>
         <article role="main">
           <h1>Source code for osxphotos.photosalbum</h1><div class="highlight"><pre>
 <span></span><span class="sd">&quot;&quot;&quot; PhotosAlbum class to create an album in default Photos library and add photos to it &quot;&quot;&quot;</span>
 
 <span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">List</span><span class="p">,</span> <span class="n">Optional</span>
 
-<span class="kn">import</span> <span class="nn">photoscript</span>
 <span class="kn">from</span> <span class="nn">more_itertools</span> <span class="kn">import</span> <span class="n">chunked</span>
-<span class="kn">from</span> <span class="nn">photoscript</span> <span class="kn">import</span> <span class="n">Album</span><span class="p">,</span> <span class="n">Folder</span><span class="p">,</span> <span class="n">Photo</span><span class="p">,</span> <span class="n">PhotosLibrary</span>
 
 <span class="kn">from</span> <span class="nn">.photoinfo</span> <span class="kn">import</span> <span class="n">PhotoInfo</span>
-<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">noop</span><span class="p">,</span> <span class="n">pluralize</span>
+<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">assert_macos</span><span class="p">,</span> <span class="n">noop</span><span class="p">,</span> <span class="n">pluralize</span>
+
+<span class="n">assert_macos</span><span class="p">()</span>
+
+<span class="kn">import</span> <span class="nn">photoscript</span>
+<span class="kn">from</span> <span class="nn">photoscript</span> <span class="kn">import</span> <span class="n">Album</span><span class="p">,</span> <span class="n">Folder</span><span class="p">,</span> <span class="n">Photo</span><span class="p">,</span> <span class="n">PhotosLibrary</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;PhotosAlbum&quot;</span><span class="p">,</span> <span class="s2">&quot;PhotosAlbumPhotoScript&quot;</span><span class="p">]</span>
 
 
 <span class="k">def</span> <span class="nf">folder_by_path</span><span class="p">(</span><span class="n">folders</span><span class="p">:</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">verbose</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">callable</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Folder</span><span class="p">:</span>
     <span class="sd">&quot;&quot;&quot;Get (and create if necessary) a Photos Folder by path (passed as list of folder names)&quot;&quot;&quot;</span>
     <span class="n">library</span> <span class="o">=</span> <span class="n">PhotosLibrary</span><span class="p">()</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -37,20 +37,23 @@
 
 ****** Source code for osxphotos.photosalbum ******
 """ PhotosAlbum class to create an album in default Photos library and add
 photos to it """
 
 from typing import List, Optional
 
-import photoscript
 from more_itertools import chunked
-from photoscript import Album, Folder, Photo, PhotosLibrary
 
 from .photoinfo import PhotoInfo
-from .utils import noop, pluralize
+from .utils import assert_macos, noop, pluralize
+
+assert_macos()
+
+import photoscript
+from photoscript import Album, Folder, Photo, PhotosLibrary
 
 __all__ = ["PhotosAlbum", "PhotosAlbumPhotoScript"]
 
 
 def folder_by_path(folders: List[str], verbose: Optional[callable] = None) -
 > Folder:
     """Get (and create if necessary) a Photos Folder by path (passed as list of
```

#### docs/_modules/osxphotos/placeinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.placeinfo - osxphotos 0.59.0 documentation</title>
+        <title>osxphotos.placeinfo - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -264,14 +264,15 @@
         <span class="s2">&quot;field15&quot;</span><span class="p">,</span>
         <span class="s2">&quot;field16&quot;</span><span class="p">,</span>
         <span class="s2">&quot;street_address&quot;</span><span class="p">,</span>  <span class="c1"># throughfare, The street address associated with the placemark.</span>
         <span class="s2">&quot;body_of_water&quot;</span><span class="p">,</span>  <span class="c1"># RKPlace.type == 44, appears to be any body of water (ocean or inland)</span>
     <span class="p">],</span>
 <span class="p">)</span>
 
+
 <span class="c1"># The following classes represent Photo Library Reverse Geolocation Info as stored</span>
 <span class="c1"># in ZADDITIONALASSETATTRIBUTES.ZREVERSELOCATIONDATA</span>
 <span class="c1"># These classes are used by bpylist.archiver to unarchive the serialized objects</span>
 <span class="k">class</span> <span class="nc">PLRevGeoLocationInfo</span><span class="p">:</span>
     <span class="sd">&quot;&quot;&quot;The top level reverse geolocation object&quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.0_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.0_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -113,14 +113,15 @@
         "street_address",  # throughfare, The street address associated with
 the placemark.
         "body_of_water",  # RKPlace.type == 44, appears to be any body of water
 (ocean or inland)
     ],
 )
 
+
 # The following classes represent Photo Library Reverse Geolocation Info as
 stored
 # in ZADDITIONALASSETATTRIBUTES.ZREVERSELOCATIONDATA
 # These classes are used by bpylist.archiver to unarchive the serialized
 objects
 class PLRevGeoLocationInfo:
     """The top level reverse geolocation object"""
```

#### docs/_modules/osxphotos/_constants.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos._constants - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos._constants - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -321,14 +321,15 @@
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;6&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;0&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;1&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">),</span>
+    <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">),</span>
 <span class="p">]</span>
 
 <span class="c1"># Photos 5 has persons who are empty string if unidentified face</span>
 <span class="n">_UNKNOWN_PERSON</span> <span class="o">=</span> <span class="s2">&quot;_UNKNOWN_&quot;</span>
 
 <span class="c1"># photos with no reverse geolocation info (place)</span>
 <span class="n">_UNKNOWN_PLACE</span> <span class="o">=</span> <span class="s2">&quot;_UNKNOWN_&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -164,14 +164,15 @@
     ("12", "3"),
     ("12", "4"),
     ("12", "5"),
     ("12", "6"),
     ("13", "0"),
     ("13", "1"),
     ("13", "2"),
+    ("13", "3"),
 ]
 
 # Photos 5 has persons who are empty string if unidentified face
 _UNKNOWN_PERSON = "_UNKNOWN_"
 
 # photos with no reverse geolocation info (place)
 _UNKNOWN_PLACE = "_UNKNOWN_"
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.59.3'
+     - The osxphotos version, e.g. '0.60.0'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.59.3',
+    VERSION: '0.60.0',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.59.3 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.59.3 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.0 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -5707,14 +5707,16 @@
   </tr></table>
 </section>
 
 <section id="T" class="genindex-section">
   <h2>T</h2>
   <table style="width: 100%" class="indextable genindextable"><tr>
     <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.PhotoInfo.tables">tables() (osxphotos.PhotoInfo method)</a>
+</li>
         <li><a href="reference.html#osxphotos.SearchInfo.text_found">text_found (osxphotos.SearchInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.time_lapse">time_lapse (osxphotos.PhotoInfo property)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.QueryOptions.time_lapse">(osxphotos.QueryOptions attribute)</a>
 </li>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1769,31 +1769,33 @@
       method)                                 property)
     * shared_(osxphotos.PhotoInfo           * SUBTOPIC
       property)                                   o osxphotos-help_command_line
           o (osxphotos.QueryOptions                 option
             attribute)
 
 ***** T *****
+    * tables()_(osxphotos.PhotoInfo
+      method)
     * text_found_(osxphotos.SearchInfo
       property)
-    * time_lapse_(osxphotos.PhotoInfo
-      property)                            * tmpdir_(osxphotos.ExportOptions
-          o (osxphotos.QueryOptions          attribute)
-            attribute)                     * tmpdir()_(osxphotos.FileUtilNoOp
-    * timeout_(osxphotos.ExportOptions       class_method)
-      attribute)                           * to_date_(osxphotos.QueryOptions
-    * title_(osxphotos.AlbumInfo             attribute)
-      property)                            * TOPIC
-          o (osxphotos.FolderInfo                o osxphotos-help_command_line
-            property)                              option
-          o (osxphotos.ImportInfo          * touch_file_
-            property)                        (osxphotos.ExportOptions
-          o (osxphotos.MomentInfo            attribute)
-            property)                      * tzoffset_(osxphotos.PhotoInfo
-          o (osxphotos.PhotoInfo             property)
+    * time_lapse_(osxphotos.PhotoInfo      * tmpdir_(osxphotos.ExportOptions
+      property)                              attribute)
+          o (osxphotos.QueryOptions        * tmpdir()_(osxphotos.FileUtilNoOp
+            attribute)                       class_method)
+    * timeout_(osxphotos.ExportOptions     * to_date_(osxphotos.QueryOptions
+      attribute)                             attribute)
+    * title_(osxphotos.AlbumInfo           * TOPIC
+      property)                                  o osxphotos-help_command_line
+          o (osxphotos.FolderInfo                  option
+            property)                      * touch_file_
+          o (osxphotos.ImportInfo            (osxphotos.ExportOptions
+            property)                        attribute)
+          o (osxphotos.MomentInfo          * tzoffset_(osxphotos.PhotoInfo
+            property)                        property)
+          o (osxphotos.PhotoInfo
             property)
           o (osxphotos.QueryOptions
             attribute)
 
 ***** U *****
     * unlink()_(osxphotos.FileUtilNoOp
       class_method)
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.59.3 documentation</title>
+        <title>osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -520,14 +520,15 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.score"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.score</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.screenshot"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.screenshot</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.search_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.search_info_normalized"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info_normalized</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.selfie"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.selfie</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.shared"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.shared</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.slow_mo"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.slow_mo</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.tables"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tables()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.time_lapse"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.time_lapse</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.title"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.title</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.tzoffset"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tzoffset</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.uti"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.uti_edited"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_edited</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.uti_original"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_original</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.uti_raw"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_raw</span></code></a></li>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -324,14 +324,15 @@
                 # PhotoInfo.score
                 # PhotoInfo.screenshot
                 # PhotoInfo.search_info
                 # PhotoInfo.search_info_normalized
                 # PhotoInfo.selfie
                 # PhotoInfo.shared
                 # PhotoInfo.slow_mo
+                # PhotoInfo.tables()
                 # PhotoInfo.time_lapse
                 # PhotoInfo.title
                 # PhotoInfo.tzoffset
                 # PhotoInfo.uti
                 # PhotoInfo.uti_edited
                 # PhotoInfo.uti_original
                 # PhotoInfo.uti_raw
```

#### docs/objects.inv

##### Sphinx inventory

```diff
@@ -219,14 +219,15 @@
 osxphotos.PhotoInfo.score py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.screenshot py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.search_info py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.search_info_normalized py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.selfie py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.shared py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.slow_mo py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.tables py:method 1 reference.html#$ -
 osxphotos.PhotoInfo.time_lapse py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.title py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.tzoffset py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.uti py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.uti_edited py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.uti_original py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.uti_raw py:property 1 reference.html#$ -
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.59.3 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.59.3 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.59.3 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.0 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.59.3 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1096,15 +1096,15 @@
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.FileUtilNoOp.copy">
 <em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">copy</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">src</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dest</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/fileutil.html#FileUtilNoOp.copy"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.FileUtilNoOp.copy" title="Permalink to this definition">#</a></dt>
-<dd><p>Copies a file from src path to dest path</p>
+<dd><p>Copies a file from src path to dest path using shutil.copy</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>src</strong> – source path as string; must be a valid file path</p></li>
 <li><p><strong>dest</strong> – destination path as string
 dest may be either directory or file; in either case, src file must not exist in dest</p></li>
 <li><p><strong>Note</strong> – src and dest may be either a string or a pathlib.Path object</p></li>
@@ -2080,14 +2080,20 @@
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.slow_mo">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">slow_mo</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.slow_mo" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns True if photo is a slow motion video, otherwise False</p>
 </dd></dl>
 
+<dl class="py method">
+<dt class="sig sig-object py" id="osxphotos.PhotoInfo.tables">
+<span class="sig-name descname"><span class="pre">tables</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">PhotoTables</span></span></span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.tables"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.tables" title="Permalink to this definition">#</a></dt>
+<dd><p>Return PhotoTables object to provide access database tables associated with this photo (Photos 5+)</p>
+</dd></dl>
+
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.time_lapse">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">time_lapse</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.time_lapse" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns True if photo is a time lapse video, otherwise False</p>
 </dd></dl>
 
 <dl class="py property">
@@ -3970,14 +3976,15 @@
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.score"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.score</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.screenshot"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.screenshot</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.search_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.search_info_normalized"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info_normalized</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.selfie"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.selfie</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.shared"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.shared</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.slow_mo"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.slow_mo</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PhotoInfo.tables"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tables()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.time_lapse"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.time_lapse</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.title"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.title</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.tzoffset"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tzoffset</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.uti"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.uti_edited"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_edited</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.uti_original"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_original</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.uti_raw"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_raw</span></code></a></li>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -470,15 +470,15 @@
                         to
                       * quality (compression) â JPEG compression quality in
                         range 0.0 <= compression_quality <= 1.0; default 1.0
                         (best quality)
               Returns:
                   True if success, otherwise False
         classmethodcopy(src, dest)[source]#
-            Copies a file from src path to dest path
+            Copies a file from src path to dest path using shutil.copy
               Parameters:
                       * src â source path as string; must be a valid file
                         path
                       * dest â destination path as string dest may be either
                         directory or file; in either case, src file must not
                         exist in dest
                       * Note â src and dest may be either a string or a
@@ -987,14 +987,17 @@
             Returns True if photo is a selfie (front facing camera), otherwise
             False
         propertyshared#
             returns True if photos is in a shared iCloud album otherwise false
             Only valid on Photos 5; returns None on older versions
         propertyslow_mo#
             Returns True if photo is a slow motion video, otherwise False
+        tables() &#x2192; PhotoTables[source]#
+            Return PhotoTables object to provide access database tables
+            associated with this photo (Photos 5+)
         propertytime_lapse#
             Returns True if photo is a time lapse video, otherwise False
         propertytitle#
             name / title of picture
         propertytzoffset#
             timezone offset from UTC in seconds
         propertyuti#
@@ -1911,14 +1914,15 @@
                 # PhotoInfo.score
                 # PhotoInfo.screenshot
                 # PhotoInfo.search_info
                 # PhotoInfo.search_info_normalized
                 # PhotoInfo.selfie
                 # PhotoInfo.shared
                 # PhotoInfo.slow_mo
+                # PhotoInfo.tables()
                 # PhotoInfo.time_lapse
                 # PhotoInfo.title
                 # PhotoInfo.tzoffset
                 # PhotoInfo.uti
                 # PhotoInfo.uti_edited
                 # PhotoInfo.uti_original
                 # PhotoInfo.uti_raw
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.59.3 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.0 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -2243,17 +2243,20 @@
         "restor": 0,
         "scan": 0,
         "midnight": 0,
         "batch": 1,
         "58": [],
         "cd": 5,
         "da": 5,
-        "59": 5,
+        "59": [],
         "indent": 4,
-        "shallow": 4
+        "shallow": 4,
+        "shutil": 4,
+        "photot": 4,
+        "60": 5
     },
     "objects": {
         "": [
             [4, 0, 0, "-", "osxphotos"]
         ],
         "osxphotos": [
             [4, 1, 1, "", "AlbumInfo"],
@@ -2511,14 +2514,15 @@
             [4, 3, 1, "", "score"],
             [4, 3, 1, "", "screenshot"],
             [4, 3, 1, "", "search_info"],
             [4, 3, 1, "", "search_info_normalized"],
             [4, 3, 1, "", "selfie"],
             [4, 3, 1, "", "shared"],
             [4, 3, 1, "", "slow_mo"],
+            [4, 2, 1, "", "tables"],
             [4, 3, 1, "", "time_lapse"],
             [4, 3, 1, "", "title"],
             [4, 3, 1, "", "tzoffset"],
             [4, 3, 1, "", "uti"],
             [4, 3, 1, "", "uti_edited"],
             [4, 3, 1, "", "uti_original"],
             [4, 3, 1, "", "uti_raw"],
@@ -4078,2028 +4082,14 @@
             [6, "color-themes"]
         ],
         "Conclusion": [
             [6, "conclusion"]
         ]
     },
     "indexentries": {
-        "--add-exported-to-album": [
-            [0, "cmdoption-osxphotos-export-add-exported-to-album"]
-        ],
-        "--add-missing-to-album": [
-            [0, "cmdoption-osxphotos-export-add-missing-to-album"]
-        ],
-        "--add-skipped-to-album": [
-            [0, "cmdoption-osxphotos-export-add-skipped-to-album"]
-        ],
-        "--add-to-album": [
-            [0, "cmdoption-osxphotos-query-add-to-album"],
-            [0, "cmdoption-osxphotos-timewarp-a"]
-        ],
-        "--added-after": [
-            [0, "cmdoption-osxphotos-add-locations-added-after"],
-            [0, "cmdoption-osxphotos-export-added-after"],
-            [0, "cmdoption-osxphotos-query-added-after"],
-            [0, "cmdoption-osxphotos-repl-added-after"],
-            [0, "cmdoption-osxphotos-sync-added-after"]
-        ],
-        "--added-before": [
-            [0, "cmdoption-osxphotos-add-locations-added-before"],
-            [0, "cmdoption-osxphotos-export-added-before"],
-            [0, "cmdoption-osxphotos-query-added-before"],
-            [0, "cmdoption-osxphotos-repl-added-before"],
-            [0, "cmdoption-osxphotos-sync-added-before"]
-        ],
-        "--added-in-last": [
-            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
-            [0, "cmdoption-osxphotos-export-added-in-last"],
-            [0, "cmdoption-osxphotos-query-added-in-last"],
-            [0, "cmdoption-osxphotos-repl-added-in-last"],
-            [0, "cmdoption-osxphotos-sync-added-in-last"]
-        ],
-        "--album": [
-            [0, "cmdoption-osxphotos-add-locations-album"],
-            [0, "cmdoption-osxphotos-export-album"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-query-album"],
-            [0, "cmdoption-osxphotos-repl-album"],
-            [0, "cmdoption-osxphotos-sync-album"]
-        ],
-        "--album-keyword": [
-            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
-            [0, "cmdoption-osxphotos-export-album-keyword"]
-        ],
-        "--alt-copy": [
-            [0, "cmdoption-osxphotos-export-alt-copy"]
-        ],
-        "--append": [
-            [0, "cmdoption-osxphotos-exiftool-append"],
-            [0, "cmdoption-osxphotos-export-append"],
-            [0, "cmdoption-osxphotos-exportdb-append"],
-            [0, "cmdoption-osxphotos-import-append"],
-            [0, "cmdoption-osxphotos-sync-A"]
-        ],
-        "--burst": [
-            [0, "cmdoption-osxphotos-add-locations-burst"],
-            [0, "cmdoption-osxphotos-export-burst"],
-            [0, "cmdoption-osxphotos-query-burst"],
-            [0, "cmdoption-osxphotos-repl-burst"],
-            [0, "cmdoption-osxphotos-sync-burst"]
-        ],
-        "--check-signatures": [
-            [0, "cmdoption-osxphotos-exportdb-check-signatures"]
-        ],
-        "--check-templates": [
-            [0, "cmdoption-osxphotos-import-check-templates"]
-        ],
-        "--cleanup": [
-            [0, "cmdoption-osxphotos-export-cleanup"]
-        ],
-        "--clear-location": [
-            [0, "cmdoption-osxphotos-import-L"]
-        ],
-        "--clear-metadata": [
-            [0, "cmdoption-osxphotos-import-C"]
-        ],
-        "--clone": [
-            [0, "cmdoption-osxphotos-theme-clone"]
-        ],
-        "--cloudasset": [
-            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
-            [0, "cmdoption-osxphotos-export-cloudasset"],
-            [0, "cmdoption-osxphotos-query-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-cloudasset"]
-        ],
-        "--compare-exif": [
-            [0, "cmdoption-osxphotos-timewarp-c"]
-        ],
-        "--config": [
-            [0, "cmdoption-osxphotos-theme-config"]
-        ],
-        "--config-only": [
-            [0, "cmdoption-osxphotos-export-config-only"]
-        ],
-        "--convert-to-jpeg": [
-            [0, "cmdoption-osxphotos-export-convert-to-jpeg"]
-        ],
-        "--current-name": [
-            [0, "cmdoption-osxphotos-export-current-name"]
-        ],
-        "--date": [
-            [0, "cmdoption-osxphotos-timewarp-d"]
-        ],
-        "--date-added": [
-            [0, "cmdoption-osxphotos-timewarp-date-added"]
-        ],
-        "--date-added-from-photo": [
-            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"]
-        ],
-        "--date-delta": [
-            [0, "cmdoption-osxphotos-timewarp-D"]
-        ],
-        "--db": [
-            [0, "cmdoption-osxphotos-albums-library"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-info-library"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-keywords-library"],
-            [0, "cmdoption-osxphotos-labels-library"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-persons-library"],
-            [0, "cmdoption-osxphotos-places-library"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-show-library"],
-            [0, "cmdoption-osxphotos-snap-library"],
-            [0, "cmdoption-osxphotos-sync-library"]
-        ],
-        "--db-config": [
-            [0, "cmdoption-osxphotos-exiftool-db-config"]
-        ],
-        "--default": [
-            [0, "cmdoption-osxphotos-theme-default"]
-        ],
-        "--delete": [
-            [0, "cmdoption-osxphotos-theme-delete"]
-        ],
-        "--delete-file": [
-            [0, "cmdoption-osxphotos-exportdb-delete-file"]
-        ],
-        "--delete-uuid": [
-            [0, "cmdoption-osxphotos-exportdb-delete-uuid"]
-        ],
-        "--deleted": [
-            [0, "cmdoption-osxphotos-dump-deleted"],
-            [0, "cmdoption-osxphotos-export-deleted"],
-            [0, "cmdoption-osxphotos-query-deleted"],
-            [0, "cmdoption-osxphotos-repl-deleted"]
-        ],
-        "--deleted-only": [
-            [0, "cmdoption-osxphotos-dump-deleted-only"],
-            [0, "cmdoption-osxphotos-export-deleted-only"],
-            [0, "cmdoption-osxphotos-query-deleted-only"],
-            [0, "cmdoption-osxphotos-repl-deleted-only"]
-        ],
-        "--description": [
-            [0, "cmdoption-osxphotos-add-locations-description"],
-            [0, "cmdoption-osxphotos-batch-edit-description"],
-            [0, "cmdoption-osxphotos-export-description"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-query-description"],
-            [0, "cmdoption-osxphotos-repl-description"],
-            [0, "cmdoption-osxphotos-sync-description"]
-        ],
-        "--description-template": [
-            [0, "cmdoption-osxphotos-exiftool-description-template"],
-            [0, "cmdoption-osxphotos-export-description-template"]
-        ],
-        "--detect-text": [
-            [0, "cmdoption-osxphotos-inspect-t"]
-        ],
-        "--directory": [
-            [0, "cmdoption-osxphotos-export-directory"]
-        ],
-        "--download-missing": [
-            [0, "cmdoption-osxphotos-export-download-missing"]
-        ],
-        "--dry-run": [
-            [0, "cmdoption-osxphotos-add-locations-dry-run"],
-            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
-            [0, "cmdoption-osxphotos-exiftool-dry-run"],
-            [0, "cmdoption-osxphotos-export-dry-run"],
-            [0, "cmdoption-osxphotos-exportdb-dry-run"],
-            [0, "cmdoption-osxphotos-sync-dry-run"]
-        ],
-        "--dup-check": [
-            [0, "cmdoption-osxphotos-import-D"]
-        ],
-        "--duplicate": [
-            [0, "cmdoption-osxphotos-add-locations-duplicate"],
-            [0, "cmdoption-osxphotos-export-duplicate"],
-            [0, "cmdoption-osxphotos-query-duplicate"],
-            [0, "cmdoption-osxphotos-repl-duplicate"],
-            [0, "cmdoption-osxphotos-sync-duplicate"]
-        ],
-        "--edit": [
-            [0, "cmdoption-osxphotos-theme-edit"]
-        ],
-        "--edited": [
-            [0, "cmdoption-osxphotos-add-locations-edited"],
-            [0, "cmdoption-osxphotos-export-edited"],
-            [0, "cmdoption-osxphotos-query-edited"],
-            [0, "cmdoption-osxphotos-repl-edited"],
-            [0, "cmdoption-osxphotos-sync-edited"]
-        ],
-        "--edited-suffix": [
-            [0, "cmdoption-osxphotos-export-edited-suffix"]
-        ],
-        "--emacs": [
-            [0, "cmdoption-osxphotos-repl-emacs"]
-        ],
-        "--errors": [
-            [0, "cmdoption-osxphotos-exportdb-errors"]
-        ],
-        "--exif": [
-            [0, "cmdoption-osxphotos-add-locations-exif"],
-            [0, "cmdoption-osxphotos-export-exif"],
-            [0, "cmdoption-osxphotos-query-exif"],
-            [0, "cmdoption-osxphotos-repl-exif"],
-            [0, "cmdoption-osxphotos-sync-exif"]
-        ],
-        "--exiftool": [
-            [0, "cmdoption-osxphotos-export-exiftool"],
-            [0, "cmdoption-osxphotos-import-e"]
-        ],
-        "--exiftool-merge-keywords": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"]
-        ],
-        "--exiftool-merge-persons": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"]
-        ],
-        "--exiftool-option": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
-            [0, "cmdoption-osxphotos-export-exiftool-option"]
-        ],
-        "--exiftool-path": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
-            [0, "cmdoption-osxphotos-export-exiftool-path"],
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-timewarp-e"]
-        ],
-        "--export": [
-            [0, "cmdoption-osxphotos-orphans-export"],
-            [0, "cmdoption-osxphotos-sync-e"]
-        ],
-        "--export-as-hardlink": [
-            [0, "cmdoption-osxphotos-export-export-as-hardlink"]
-        ],
-        "--export-by-date": [
-            [0, "cmdoption-osxphotos-export-export-by-date"]
-        ],
-        "--export-dir": [
-            [0, "cmdoption-osxphotos-exportdb-export-dir"]
-        ],
-        "--exportdb": [
-            [0, "cmdoption-osxphotos-exiftool-exportdb"],
-            [0, "cmdoption-osxphotos-export-exportdb"]
-        ],
-        "--external-edit": [
-            [0, "cmdoption-osxphotos-add-locations-external-edit"],
-            [0, "cmdoption-osxphotos-export-external-edit"],
-            [0, "cmdoption-osxphotos-query-external-edit"],
-            [0, "cmdoption-osxphotos-repl-external-edit"],
-            [0, "cmdoption-osxphotos-sync-external-edit"]
-        ],
-        "--favorite": [
-            [0, "cmdoption-osxphotos-add-locations-favorite"],
-            [0, "cmdoption-osxphotos-export-favorite"],
-            [0, "cmdoption-osxphotos-query-favorite"],
-            [0, "cmdoption-osxphotos-repl-favorite"],
-            [0, "cmdoption-osxphotos-sync-favorite"]
-        ],
-        "--favorite-rating": [
-            [0, "cmdoption-osxphotos-export-favorite-rating"]
-        ],
-        "--field": [
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-query-f"]
-        ],
-        "--filename": [
-            [0, "cmdoption-osxphotos-export-filename"],
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "--finder-tag-keywords": [
-            [0, "cmdoption-osxphotos-export-finder-tag-keywords"]
-        ],
-        "--finder-tag-template": [
-            [0, "cmdoption-osxphotos-export-finder-tag-template"]
-        ],
-        "--folder": [
-            [0, "cmdoption-osxphotos-add-locations-folder"],
-            [0, "cmdoption-osxphotos-export-folder"],
-            [0, "cmdoption-osxphotos-query-folder"],
-            [0, "cmdoption-osxphotos-repl-folder"],
-            [0, "cmdoption-osxphotos-sync-folder"]
-        ],
-        "--force": [
-            [0, "cmdoption-osxphotos-timewarp-force"]
-        ],
-        "--force-update": [
-            [0, "cmdoption-osxphotos-export-force-update"]
-        ],
-        "--from-date": [
-            [0, "cmdoption-osxphotos-add-locations-from-date"],
-            [0, "cmdoption-osxphotos-export-from-date"],
-            [0, "cmdoption-osxphotos-query-from-date"],
-            [0, "cmdoption-osxphotos-repl-from-date"],
-            [0, "cmdoption-osxphotos-sync-from-date"]
-        ],
-        "--from-time": [
-            [0, "cmdoption-osxphotos-add-locations-from-time"],
-            [0, "cmdoption-osxphotos-export-from-time"],
-            [0, "cmdoption-osxphotos-query-from-time"],
-            [0, "cmdoption-osxphotos-repl-from-time"],
-            [0, "cmdoption-osxphotos-sync-from-time"]
-        ],
-        "--function": [
-            [0, "cmdoption-osxphotos-timewarp-F"]
-        ],
-        "--glob": [
-            [0, "cmdoption-osxphotos-import-g"]
-        ],
-        "--has-comment": [
-            [0, "cmdoption-osxphotos-add-locations-has-comment"],
-            [0, "cmdoption-osxphotos-export-has-comment"],
-            [0, "cmdoption-osxphotos-query-has-comment"],
-            [0, "cmdoption-osxphotos-repl-has-comment"],
-            [0, "cmdoption-osxphotos-sync-has-comment"]
-        ],
-        "--has-likes": [
-            [0, "cmdoption-osxphotos-add-locations-has-likes"],
-            [0, "cmdoption-osxphotos-export-has-likes"],
-            [0, "cmdoption-osxphotos-query-has-likes"],
-            [0, "cmdoption-osxphotos-repl-has-likes"],
-            [0, "cmdoption-osxphotos-sync-has-likes"]
-        ],
-        "--has-raw": [
-            [0, "cmdoption-osxphotos-add-locations-has-raw"],
-            [0, "cmdoption-osxphotos-export-has-raw"],
-            [0, "cmdoption-osxphotos-query-has-raw"],
-            [0, "cmdoption-osxphotos-repl-has-raw"],
-            [0, "cmdoption-osxphotos-sync-has-raw"]
-        ],
-        "--hdr": [
-            [0, "cmdoption-osxphotos-add-locations-hdr"],
-            [0, "cmdoption-osxphotos-export-hdr"],
-            [0, "cmdoption-osxphotos-query-hdr"],
-            [0, "cmdoption-osxphotos-repl-hdr"],
-            [0, "cmdoption-osxphotos-sync-hdr"]
-        ],
-        "--help": [
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "--hidden": [
-            [0, "cmdoption-osxphotos-add-locations-hidden"],
-            [0, "cmdoption-osxphotos-export-hidden"],
-            [0, "cmdoption-osxphotos-query-hidden"],
-            [0, "cmdoption-osxphotos-repl-hidden"],
-            [0, "cmdoption-osxphotos-sync-hidden"]
-        ],
-        "--ignore-case": [
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-sync-0"]
-        ],
-        "--ignore-date-modified": [
-            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-export-ignore-date-modified"]
-        ],
-        "--ignore-signature": [
-            [0, "cmdoption-osxphotos-export-ignore-signature"]
-        ],
-        "--import": [
-            [0, "cmdoption-osxphotos-sync-i"]
-        ],
-        "--in-album": [
-            [0, "cmdoption-osxphotos-add-locations-in-album"],
-            [0, "cmdoption-osxphotos-export-in-album"],
-            [0, "cmdoption-osxphotos-query-in-album"],
-            [0, "cmdoption-osxphotos-repl-in-album"],
-            [0, "cmdoption-osxphotos-sync-in-album"]
-        ],
-        "--incloud": [
-            [0, "cmdoption-osxphotos-add-locations-incloud"],
-            [0, "cmdoption-osxphotos-export-incloud"],
-            [0, "cmdoption-osxphotos-query-incloud"],
-            [0, "cmdoption-osxphotos-repl-incloud"],
-            [0, "cmdoption-osxphotos-sync-incloud"]
-        ],
-        "--info": [
-            [0, "cmdoption-osxphotos-exportdb-info"]
-        ],
-        "--inspect": [
-            [0, "cmdoption-osxphotos-timewarp-i"]
-        ],
-        "--is-reference": [
-            [0, "cmdoption-osxphotos-add-locations-is-reference"],
-            [0, "cmdoption-osxphotos-export-is-reference"],
-            [0, "cmdoption-osxphotos-query-is-reference"],
-            [0, "cmdoption-osxphotos-repl-is-reference"],
-            [0, "cmdoption-osxphotos-sync-is-reference"]
-        ],
-        "--jpeg-ext": [
-            [0, "cmdoption-osxphotos-export-jpeg-ext"]
-        ],
-        "--jpeg-quality": [
-            [0, "cmdoption-osxphotos-export-jpeg-quality"]
-        ],
-        "--json": [
-            [0, "cmdoption-osxphotos-albums-json"],
-            [0, "cmdoption-osxphotos-dump-json"],
-            [0, "cmdoption-osxphotos-info-json"],
-            [0, "cmdoption-osxphotos-json"],
-            [0, "cmdoption-osxphotos-keywords-json"],
-            [0, "cmdoption-osxphotos-labels-json"],
-            [0, "cmdoption-osxphotos-list-json"],
-            [0, "cmdoption-osxphotos-persons-json"],
-            [0, "cmdoption-osxphotos-places-json"],
-            [0, "cmdoption-osxphotos-query-json"]
-        ],
-        "--keep": [
-            [0, "cmdoption-osxphotos-export-keep"]
-        ],
-        "--keyword": [
-            [0, "cmdoption-osxphotos-add-locations-keyword"],
-            [0, "cmdoption-osxphotos-batch-edit-keyword"],
-            [0, "cmdoption-osxphotos-export-keyword"],
-            [0, "cmdoption-osxphotos-import-k"],
-            [0, "cmdoption-osxphotos-query-keyword"],
-            [0, "cmdoption-osxphotos-repl-keyword"],
-            [0, "cmdoption-osxphotos-sync-keyword"]
-        ],
-        "--keyword-template": [
-            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
-            [0, "cmdoption-osxphotos-export-keyword-template"]
-        ],
-        "--label": [
-            [0, "cmdoption-osxphotos-add-locations-label"],
-            [0, "cmdoption-osxphotos-export-label"],
-            [0, "cmdoption-osxphotos-query-label"],
-            [0, "cmdoption-osxphotos-repl-label"],
-            [0, "cmdoption-osxphotos-sync-label"]
-        ],
-        "--last-errors": [
-            [0, "cmdoption-osxphotos-exportdb-last-errors"]
-        ],
-        "--last-run": [
-            [0, "cmdoption-osxphotos-exportdb-last-run"]
-        ],
-        "--library": [
-            [0, "cmdoption-osxphotos-albums-library"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-info-library"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-keywords-library"],
-            [0, "cmdoption-osxphotos-labels-library"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-persons-library"],
-            [0, "cmdoption-osxphotos-places-library"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-show-library"],
-            [0, "cmdoption-osxphotos-snap-library"],
-            [0, "cmdoption-osxphotos-sync-library"],
-            [0, "cmdoption-osxphotos-timewarp-L"]
-        ],
-        "--limit": [
-            [0, "cmdoption-osxphotos-export-limit"]
-        ],
-        "--list": [
-            [0, "cmdoption-osxphotos-theme-list"]
-        ],
-        "--live": [
-            [0, "cmdoption-osxphotos-add-locations-live"],
-            [0, "cmdoption-osxphotos-export-live"],
-            [0, "cmdoption-osxphotos-query-live"],
-            [0, "cmdoption-osxphotos-repl-live"],
-            [0, "cmdoption-osxphotos-sync-live"]
-        ],
-        "--load-config": [
-            [0, "cmdoption-osxphotos-exiftool-load-config"],
-            [0, "cmdoption-osxphotos-export-load-config"]
-        ],
-        "--location": [
-            [0, "cmdoption-osxphotos-add-locations-location"],
-            [0, "cmdoption-osxphotos-batch-edit-location"],
-            [0, "cmdoption-osxphotos-export-location"],
-            [0, "cmdoption-osxphotos-import-l"],
-            [0, "cmdoption-osxphotos-query-location"],
-            [0, "cmdoption-osxphotos-repl-location"],
-            [0, "cmdoption-osxphotos-sync-location"]
-        ],
-        "--match-time": [
-            [0, "cmdoption-osxphotos-timewarp-0"]
-        ],
-        "--max-size": [
-            [0, "cmdoption-osxphotos-add-locations-max-size"],
-            [0, "cmdoption-osxphotos-export-max-size"],
-            [0, "cmdoption-osxphotos-query-max-size"],
-            [0, "cmdoption-osxphotos-repl-max-size"],
-            [0, "cmdoption-osxphotos-sync-max-size"]
-        ],
-        "--merge": [
-            [0, "cmdoption-osxphotos-sync-m"]
-        ],
-        "--merge-keywords": [
-            [0, "cmdoption-osxphotos-import-m"]
-        ],
-        "--migrate": [
-            [0, "cmdoption-osxphotos-exportdb-migrate"]
-        ],
-        "--migrate-photos-library": [
-            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"]
-        ],
-        "--min-size": [
-            [0, "cmdoption-osxphotos-add-locations-min-size"],
-            [0, "cmdoption-osxphotos-export-min-size"],
-            [0, "cmdoption-osxphotos-query-min-size"],
-            [0, "cmdoption-osxphotos-repl-min-size"],
-            [0, "cmdoption-osxphotos-sync-min-size"]
-        ],
-        "--missing": [
-            [0, "cmdoption-osxphotos-add-locations-missing"],
-            [0, "cmdoption-osxphotos-export-missing"],
-            [0, "cmdoption-osxphotos-query-missing"],
-            [0, "cmdoption-osxphotos-repl-missing"],
-            [0, "cmdoption-osxphotos-sync-missing"]
-        ],
-        "--name": [
-            [0, "cmdoption-osxphotos-add-locations-name"],
-            [0, "cmdoption-osxphotos-export-name"],
-            [0, "cmdoption-osxphotos-query-name"],
-            [0, "cmdoption-osxphotos-repl-name"],
-            [0, "cmdoption-osxphotos-sync-name"]
-        ],
-        "--no-comment": [
-            [0, "cmdoption-osxphotos-add-locations-no-comment"],
-            [0, "cmdoption-osxphotos-export-no-comment"],
-            [0, "cmdoption-osxphotos-query-no-comment"],
-            [0, "cmdoption-osxphotos-repl-no-comment"],
-            [0, "cmdoption-osxphotos-sync-no-comment"]
-        ],
-        "--no-description": [
-            [0, "cmdoption-osxphotos-add-locations-no-description"],
-            [0, "cmdoption-osxphotos-export-no-description"],
-            [0, "cmdoption-osxphotos-query-no-description"],
-            [0, "cmdoption-osxphotos-repl-no-description"],
-            [0, "cmdoption-osxphotos-sync-no-description"]
-        ],
-        "--no-keyword": [
-            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
-            [0, "cmdoption-osxphotos-export-no-keyword"],
-            [0, "cmdoption-osxphotos-query-no-keyword"],
-            [0, "cmdoption-osxphotos-repl-no-keyword"],
-            [0, "cmdoption-osxphotos-sync-no-keyword"]
-        ],
-        "--no-likes": [
-            [0, "cmdoption-osxphotos-add-locations-no-likes"],
-            [0, "cmdoption-osxphotos-export-no-likes"],
-            [0, "cmdoption-osxphotos-query-no-likes"],
-            [0, "cmdoption-osxphotos-repl-no-likes"],
-            [0, "cmdoption-osxphotos-sync-no-likes"]
-        ],
-        "--no-location": [
-            [0, "cmdoption-osxphotos-add-locations-no-location"],
-            [0, "cmdoption-osxphotos-export-no-location"],
-            [0, "cmdoption-osxphotos-query-no-location"],
-            [0, "cmdoption-osxphotos-repl-no-location"],
-            [0, "cmdoption-osxphotos-sync-no-location"]
-        ],
-        "--no-place": [
-            [0, "cmdoption-osxphotos-add-locations-no-place"],
-            [0, "cmdoption-osxphotos-export-no-place"],
-            [0, "cmdoption-osxphotos-query-no-place"],
-            [0, "cmdoption-osxphotos-repl-no-place"],
-            [0, "cmdoption-osxphotos-sync-no-place"]
-        ],
-        "--no-progress": [
-            [0, "cmdoption-osxphotos-export-no-progress"],
-            [0, "cmdoption-osxphotos-import-no-progress"]
-        ],
-        "--no-title": [
-            [0, "cmdoption-osxphotos-add-locations-no-title"],
-            [0, "cmdoption-osxphotos-export-no-title"],
-            [0, "cmdoption-osxphotos-query-no-title"],
-            [0, "cmdoption-osxphotos-repl-no-title"],
-            [0, "cmdoption-osxphotos-sync-no-title"]
-        ],
-        "--not-burst": [
-            [0, "cmdoption-osxphotos-add-locations-not-burst"],
-            [0, "cmdoption-osxphotos-export-not-burst"],
-            [0, "cmdoption-osxphotos-query-not-burst"],
-            [0, "cmdoption-osxphotos-repl-not-burst"],
-            [0, "cmdoption-osxphotos-sync-not-burst"]
-        ],
-        "--not-cloudasset": [
-            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
-            [0, "cmdoption-osxphotos-export-not-cloudasset"],
-            [0, "cmdoption-osxphotos-query-not-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-not-cloudasset"]
-        ],
-        "--not-edited": [
-            [0, "cmdoption-osxphotos-add-locations-not-edited"],
-            [0, "cmdoption-osxphotos-export-not-edited"],
-            [0, "cmdoption-osxphotos-query-not-edited"],
-            [0, "cmdoption-osxphotos-repl-not-edited"],
-            [0, "cmdoption-osxphotos-sync-not-edited"]
-        ],
-        "--not-favorite": [
-            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
-            [0, "cmdoption-osxphotos-export-not-favorite"],
-            [0, "cmdoption-osxphotos-query-not-favorite"],
-            [0, "cmdoption-osxphotos-repl-not-favorite"],
-            [0, "cmdoption-osxphotos-sync-not-favorite"]
-        ],
-        "--not-hdr": [
-            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
-            [0, "cmdoption-osxphotos-export-not-hdr"],
-            [0, "cmdoption-osxphotos-query-not-hdr"],
-            [0, "cmdoption-osxphotos-repl-not-hdr"],
-            [0, "cmdoption-osxphotos-sync-not-hdr"]
-        ],
-        "--not-hidden": [
-            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
-            [0, "cmdoption-osxphotos-export-not-hidden"],
-            [0, "cmdoption-osxphotos-query-not-hidden"],
-            [0, "cmdoption-osxphotos-repl-not-hidden"],
-            [0, "cmdoption-osxphotos-sync-not-hidden"]
-        ],
-        "--not-in-album": [
-            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
-            [0, "cmdoption-osxphotos-export-not-in-album"],
-            [0, "cmdoption-osxphotos-query-not-in-album"],
-            [0, "cmdoption-osxphotos-repl-not-in-album"],
-            [0, "cmdoption-osxphotos-sync-not-in-album"]
-        ],
-        "--not-incloud": [
-            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
-            [0, "cmdoption-osxphotos-export-not-incloud"],
-            [0, "cmdoption-osxphotos-query-not-incloud"],
-            [0, "cmdoption-osxphotos-repl-not-incloud"],
-            [0, "cmdoption-osxphotos-sync-not-incloud"]
-        ],
-        "--not-live": [
-            [0, "cmdoption-osxphotos-add-locations-not-live"],
-            [0, "cmdoption-osxphotos-export-not-live"],
-            [0, "cmdoption-osxphotos-query-not-live"],
-            [0, "cmdoption-osxphotos-repl-not-live"],
-            [0, "cmdoption-osxphotos-sync-not-live"]
-        ],
-        "--not-missing": [
-            [0, "cmdoption-osxphotos-add-locations-not-missing"],
-            [0, "cmdoption-osxphotos-export-not-missing"],
-            [0, "cmdoption-osxphotos-query-not-missing"],
-            [0, "cmdoption-osxphotos-repl-not-missing"],
-            [0, "cmdoption-osxphotos-sync-not-missing"]
-        ],
-        "--not-panorama": [
-            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
-            [0, "cmdoption-osxphotos-export-not-panorama"],
-            [0, "cmdoption-osxphotos-query-not-panorama"],
-            [0, "cmdoption-osxphotos-repl-not-panorama"],
-            [0, "cmdoption-osxphotos-sync-not-panorama"]
-        ],
-        "--not-portrait": [
-            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
-            [0, "cmdoption-osxphotos-export-not-portrait"],
-            [0, "cmdoption-osxphotos-query-not-portrait"],
-            [0, "cmdoption-osxphotos-repl-not-portrait"],
-            [0, "cmdoption-osxphotos-sync-not-portrait"]
-        ],
-        "--not-reference": [
-            [0, "cmdoption-osxphotos-add-locations-not-reference"],
-            [0, "cmdoption-osxphotos-export-not-reference"],
-            [0, "cmdoption-osxphotos-query-not-reference"],
-            [0, "cmdoption-osxphotos-repl-not-reference"],
-            [0, "cmdoption-osxphotos-sync-not-reference"]
-        ],
-        "--not-screenshot": [
-            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
-            [0, "cmdoption-osxphotos-export-not-screenshot"],
-            [0, "cmdoption-osxphotos-query-not-screenshot"],
-            [0, "cmdoption-osxphotos-repl-not-screenshot"],
-            [0, "cmdoption-osxphotos-sync-not-screenshot"]
-        ],
-        "--not-selfie": [
-            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
-            [0, "cmdoption-osxphotos-export-not-selfie"],
-            [0, "cmdoption-osxphotos-query-not-selfie"],
-            [0, "cmdoption-osxphotos-repl-not-selfie"],
-            [0, "cmdoption-osxphotos-sync-not-selfie"]
-        ],
-        "--not-shared": [
-            [0, "cmdoption-osxphotos-add-locations-not-shared"],
-            [0, "cmdoption-osxphotos-export-not-shared"],
-            [0, "cmdoption-osxphotos-query-not-shared"],
-            [0, "cmdoption-osxphotos-repl-not-shared"]
-        ],
-        "--not-slow-mo": [
-            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
-            [0, "cmdoption-osxphotos-export-not-slow-mo"],
-            [0, "cmdoption-osxphotos-query-not-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-not-slow-mo"]
-        ],
-        "--not-time-lapse": [
-            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
-            [0, "cmdoption-osxphotos-export-not-time-lapse"],
-            [0, "cmdoption-osxphotos-query-not-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-not-time-lapse"]
-        ],
-        "--only-movies": [
-            [0, "cmdoption-osxphotos-add-locations-only-movies"],
-            [0, "cmdoption-osxphotos-export-only-movies"],
-            [0, "cmdoption-osxphotos-query-only-movies"],
-            [0, "cmdoption-osxphotos-repl-only-movies"],
-            [0, "cmdoption-osxphotos-sync-only-movies"]
-        ],
-        "--only-new": [
-            [0, "cmdoption-osxphotos-export-only-new"]
-        ],
-        "--only-photos": [
-            [0, "cmdoption-osxphotos-add-locations-only-photos"],
-            [0, "cmdoption-osxphotos-export-only-photos"],
-            [0, "cmdoption-osxphotos-query-only-photos"],
-            [0, "cmdoption-osxphotos-repl-only-photos"],
-            [0, "cmdoption-osxphotos-sync-only-photos"]
-        ],
-        "--original-suffix": [
-            [0, "cmdoption-osxphotos-export-original-suffix"]
-        ],
-        "--overwrite": [
-            [0, "cmdoption-osxphotos-export-overwrite"]
-        ],
-        "--panorama": [
-            [0, "cmdoption-osxphotos-add-locations-panorama"],
-            [0, "cmdoption-osxphotos-export-panorama"],
-            [0, "cmdoption-osxphotos-query-panorama"],
-            [0, "cmdoption-osxphotos-repl-panorama"],
-            [0, "cmdoption-osxphotos-sync-panorama"]
-        ],
-        "--parse-date": [
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-timewarp-M"]
-        ],
-        "--person": [
-            [0, "cmdoption-osxphotos-add-locations-person"],
-            [0, "cmdoption-osxphotos-export-person"],
-            [0, "cmdoption-osxphotos-query-person"],
-            [0, "cmdoption-osxphotos-repl-person"],
-            [0, "cmdoption-osxphotos-sync-person"]
-        ],
-        "--person-keyword": [
-            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
-            [0, "cmdoption-osxphotos-export-person-keyword"]
-        ],
-        "--place": [
-            [0, "cmdoption-osxphotos-add-locations-place"],
-            [0, "cmdoption-osxphotos-export-place"],
-            [0, "cmdoption-osxphotos-query-place"],
-            [0, "cmdoption-osxphotos-repl-place"],
-            [0, "cmdoption-osxphotos-sync-place"]
-        ],
-        "--plain": [
-            [0, "cmdoption-osxphotos-timewarp-plain"]
-        ],
-        "--portrait": [
-            [0, "cmdoption-osxphotos-add-locations-portrait"],
-            [0, "cmdoption-osxphotos-export-portrait"],
-            [0, "cmdoption-osxphotos-query-portrait"],
-            [0, "cmdoption-osxphotos-repl-portrait"],
-            [0, "cmdoption-osxphotos-sync-portrait"]
-        ],
-        "--post-command": [
-            [0, "cmdoption-osxphotos-export-post-command"]
-        ],
-        "--post-function": [
-            [0, "cmdoption-osxphotos-export-post-function"],
-            [0, "cmdoption-osxphotos-import-post-function"]
-        ],
-        "--preview": [
-            [0, "cmdoption-osxphotos-export-preview"],
-            [0, "cmdoption-osxphotos-theme-preview"]
-        ],
-        "--preview-if-missing": [
-            [0, "cmdoption-osxphotos-export-preview-if-missing"]
-        ],
-        "--preview-suffix": [
-            [0, "cmdoption-osxphotos-export-preview-suffix"]
-        ],
-        "--print": [
-            [0, "cmdoption-osxphotos-dump-print"],
-            [0, "cmdoption-osxphotos-export-print"],
-            [0, "cmdoption-osxphotos-query-print"]
-        ],
-        "--pull-exif": [
-            [0, "cmdoption-osxphotos-timewarp-P"]
-        ],
-        "--push-exif": [
-            [0, "cmdoption-osxphotos-timewarp-p"]
-        ],
-        "--query-eval": [
-            [0, "cmdoption-osxphotos-add-locations-query-eval"],
-            [0, "cmdoption-osxphotos-export-query-eval"],
-            [0, "cmdoption-osxphotos-query-query-eval"],
-            [0, "cmdoption-osxphotos-repl-query-eval"],
-            [0, "cmdoption-osxphotos-sync-query-eval"]
-        ],
-        "--query-function": [
-            [0, "cmdoption-osxphotos-add-locations-query-function"],
-            [0, "cmdoption-osxphotos-export-query-function"],
-            [0, "cmdoption-osxphotos-query-query-function"],
-            [0, "cmdoption-osxphotos-repl-query-function"],
-            [0, "cmdoption-osxphotos-sync-query-function"]
-        ],
-        "--quiet": [
-            [0, "cmdoption-osxphotos-query-quiet"]
-        ],
-        "--ramdb": [
-            [0, "cmdoption-osxphotos-export-ramdb"]
-        ],
-        "--raw-output": [
-            [0, "cmdoption-osxphotos-diff-r"]
-        ],
-        "--regex": [
-            [0, "cmdoption-osxphotos-add-locations-regex"],
-            [0, "cmdoption-osxphotos-export-regex"],
-            [0, "cmdoption-osxphotos-query-regex"],
-            [0, "cmdoption-osxphotos-repl-regex"],
-            [0, "cmdoption-osxphotos-sync-regex"]
-        ],
-        "--relative-to": [
-            [0, "cmdoption-osxphotos-import-r"]
-        ],
-        "--replace-keywords": [
-            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
-            [0, "cmdoption-osxphotos-export-replace-keywords"]
-        ],
-        "--report": [
-            [0, "cmdoption-osxphotos-exiftool-report"],
-            [0, "cmdoption-osxphotos-export-report"],
-            [0, "cmdoption-osxphotos-exportdb-report"],
-            [0, "cmdoption-osxphotos-import-report"],
-            [0, "cmdoption-osxphotos-sync-R"]
-        ],
-        "--resume": [
-            [0, "cmdoption-osxphotos-import-R"]
-        ],
-        "--retry": [
-            [0, "cmdoption-osxphotos-export-retry"]
-        ],
-        "--run": [
-            [0, "cmdoption-osxphotos-version-run"]
-        ],
-        "--save-config": [
-            [0, "cmdoption-osxphotos-exiftool-save-config"],
-            [0, "cmdoption-osxphotos-export-save-config"],
-            [0, "cmdoption-osxphotos-exportdb-save-config"]
-        ],
-        "--screenshot": [
-            [0, "cmdoption-osxphotos-add-locations-screenshot"],
-            [0, "cmdoption-osxphotos-export-screenshot"],
-            [0, "cmdoption-osxphotos-query-screenshot"],
-            [0, "cmdoption-osxphotos-repl-screenshot"],
-            [0, "cmdoption-osxphotos-sync-screenshot"]
-        ],
-        "--selected": [
-            [0, "cmdoption-osxphotos-add-locations-selected"],
-            [0, "cmdoption-osxphotos-export-selected"],
-            [0, "cmdoption-osxphotos-query-selected"],
-            [0, "cmdoption-osxphotos-repl-selected"],
-            [0, "cmdoption-osxphotos-sync-selected"]
-        ],
-        "--selfie": [
-            [0, "cmdoption-osxphotos-add-locations-selfie"],
-            [0, "cmdoption-osxphotos-export-selfie"],
-            [0, "cmdoption-osxphotos-query-selfie"],
-            [0, "cmdoption-osxphotos-repl-selfie"],
-            [0, "cmdoption-osxphotos-sync-selfie"]
-        ],
-        "--set": [
-            [0, "cmdoption-osxphotos-sync-s"]
-        ],
-        "--shared": [
-            [0, "cmdoption-osxphotos-add-locations-shared"],
-            [0, "cmdoption-osxphotos-export-shared"],
-            [0, "cmdoption-osxphotos-query-shared"],
-            [0, "cmdoption-osxphotos-repl-shared"]
-        ],
-        "--sidecar": [
-            [0, "cmdoption-osxphotos-export-sidecar"]
-        ],
-        "--sidecar-drop-ext": [
-            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"]
-        ],
-        "--skip-bursts": [
-            [0, "cmdoption-osxphotos-export-skip-bursts"]
-        ],
-        "--skip-edited": [
-            [0, "cmdoption-osxphotos-export-skip-edited"]
-        ],
-        "--skip-live": [
-            [0, "cmdoption-osxphotos-export-skip-live"]
-        ],
-        "--skip-original-if-edited": [
-            [0, "cmdoption-osxphotos-export-skip-original-if-edited"]
-        ],
-        "--skip-raw": [
-            [0, "cmdoption-osxphotos-export-skip-raw"]
-        ],
-        "--skip-uuid": [
-            [0, "cmdoption-osxphotos-export-skip-uuid"]
-        ],
-        "--skip-uuid-from-file": [
-            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"]
-        ],
-        "--slow-mo": [
-            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
-            [0, "cmdoption-osxphotos-export-slow-mo"],
-            [0, "cmdoption-osxphotos-query-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-slow-mo"]
-        ],
-        "--split-folder": [
-            [0, "cmdoption-osxphotos-import-f"]
-        ],
-        "--sql": [
-            [0, "cmdoption-osxphotos-exportdb-sql"]
-        ],
-        "--strip": [
-            [0, "cmdoption-osxphotos-export-strip"]
-        ],
-        "--style": [
-            [0, "cmdoption-osxphotos-diff-s"]
-        ],
-        "--template": [
-            [0, "cmdoption-osxphotos-inspect-T"]
-        ],
-        "--theme": [
-            [0, "cmdoption-osxphotos-add-locations-theme"],
-            [0, "cmdoption-osxphotos-batch-edit-theme"],
-            [0, "cmdoption-osxphotos-exiftool-theme"],
-            [0, "cmdoption-osxphotos-export-theme"],
-            [0, "cmdoption-osxphotos-exportdb-theme"],
-            [0, "cmdoption-osxphotos-import-theme"],
-            [0, "cmdoption-osxphotos-inspect-theme"],
-            [0, "cmdoption-osxphotos-orphans-theme"],
-            [0, "cmdoption-osxphotos-sync-theme"],
-            [0, "cmdoption-osxphotos-timewarp-theme"]
-        ],
-        "--time": [
-            [0, "cmdoption-osxphotos-timewarp-t"]
-        ],
-        "--time-delta": [
-            [0, "cmdoption-osxphotos-timewarp-T"]
-        ],
-        "--time-lapse": [
-            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
-            [0, "cmdoption-osxphotos-export-time-lapse"],
-            [0, "cmdoption-osxphotos-query-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-time-lapse"]
-        ],
-        "--timestamp": [
-            [0, "cmdoption-osxphotos-add-locations-timestamp"],
-            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
-            [0, "cmdoption-osxphotos-diff-timestamp"],
-            [0, "cmdoption-osxphotos-exiftool-timestamp"],
-            [0, "cmdoption-osxphotos-export-timestamp"],
-            [0, "cmdoption-osxphotos-exportdb-timestamp"],
-            [0, "cmdoption-osxphotos-import-timestamp"],
-            [0, "cmdoption-osxphotos-orphans-timestamp"],
-            [0, "cmdoption-osxphotos-sync-timestamp"],
-            [0, "cmdoption-osxphotos-timewarp-2"],
-            [0, "cmdoption-osxphotos-timewarp-timestamp"]
-        ],
-        "--timezone": [
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "--title": [
-            [0, "cmdoption-osxphotos-add-locations-title"],
-            [0, "cmdoption-osxphotos-batch-edit-title"],
-            [0, "cmdoption-osxphotos-export-title"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-query-title"],
-            [0, "cmdoption-osxphotos-repl-title"],
-            [0, "cmdoption-osxphotos-sync-title"]
-        ],
-        "--tmpdir": [
-            [0, "cmdoption-osxphotos-export-tmpdir"]
-        ],
-        "--to-date": [
-            [0, "cmdoption-osxphotos-add-locations-to-date"],
-            [0, "cmdoption-osxphotos-export-to-date"],
-            [0, "cmdoption-osxphotos-query-to-date"],
-            [0, "cmdoption-osxphotos-repl-to-date"],
-            [0, "cmdoption-osxphotos-sync-to-date"]
-        ],
-        "--to-time": [
-            [0, "cmdoption-osxphotos-add-locations-to-time"],
-            [0, "cmdoption-osxphotos-export-to-time"],
-            [0, "cmdoption-osxphotos-query-to-time"],
-            [0, "cmdoption-osxphotos-repl-to-time"],
-            [0, "cmdoption-osxphotos-sync-to-time"]
-        ],
-        "--touch-file": [
-            [0, "cmdoption-osxphotos-export-touch-file"],
-            [0, "cmdoption-osxphotos-exportdb-touch-file"]
-        ],
-        "--undo": [
-            [0, "cmdoption-osxphotos-batch-edit-undo"]
-        ],
-        "--unmatched": [
-            [0, "cmdoption-osxphotos-sync-U"]
-        ],
-        "--update": [
-            [0, "cmdoption-osxphotos-export-update"]
-        ],
-        "--update-errors": [
-            [0, "cmdoption-osxphotos-export-update-errors"]
-        ],
-        "--update-signatures": [
-            [0, "cmdoption-osxphotos-exportdb-update-signatures"]
-        ],
-        "--upgrade": [
-            [0, "cmdoption-osxphotos-install-U"]
-        ],
-        "--use-file-time": [
-            [0, "cmdoption-osxphotos-timewarp-1"]
-        ],
-        "--use-photokit": [
-            [0, "cmdoption-osxphotos-export-use-photokit"]
-        ],
-        "--use-photos-export": [
-            [0, "cmdoption-osxphotos-export-use-photos-export"]
-        ],
-        "--uti": [
-            [0, "cmdoption-osxphotos-add-locations-uti"],
-            [0, "cmdoption-osxphotos-export-uti"],
-            [0, "cmdoption-osxphotos-query-uti"],
-            [0, "cmdoption-osxphotos-repl-uti"],
-            [0, "cmdoption-osxphotos-sync-uti"]
-        ],
-        "--uuid": [
-            [0, "cmdoption-osxphotos-add-locations-uuid"],
-            [0, "cmdoption-osxphotos-export-uuid"],
-            [0, "cmdoption-osxphotos-query-uuid"],
-            [0, "cmdoption-osxphotos-repl-uuid"],
-            [0, "cmdoption-osxphotos-sync-uuid"]
-        ],
-        "--uuid-files": [
-            [0, "cmdoption-osxphotos-exportdb-uuid-files"]
-        ],
-        "--uuid-from-file": [
-            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-uuid-from-file"],
-            [0, "cmdoption-osxphotos-query-uuid-from-file"],
-            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
-            [0, "cmdoption-osxphotos-sync-uuid-from-file"]
-        ],
-        "--uuid-info": [
-            [0, "cmdoption-osxphotos-exportdb-uuid-info"]
-        ],
-        "--vacuum": [
-            [0, "cmdoption-osxphotos-exportdb-vacuum"]
-        ],
-        "--verbose": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-timewarp-V"]
-        ],
-        "--version": [
-            [0, "cmdoption-osxphotos-exportdb-version"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "--walk": [
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "--window": [
-            [0, "cmdoption-osxphotos-add-locations-w"]
-        ],
-        "--xattr-template": [
-            [0, "cmdoption-osxphotos-export-xattr-template"]
-        ],
-        "--year": [
-            [0, "cmdoption-osxphotos-add-locations-year"],
-            [0, "cmdoption-osxphotos-export-year"],
-            [0, "cmdoption-osxphotos-query-year"],
-            [0, "cmdoption-osxphotos-repl-year"],
-            [0, "cmdoption-osxphotos-sync-year"]
-        ],
-        "--yes": [
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "-a": [
-            [0, "cmdoption-osxphotos-sync-A"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-timewarp-a"]
-        ],
-        "-c": [
-            [0, "cmdoption-osxphotos-import-C"],
-            [0, "cmdoption-osxphotos-timewarp-c"]
-        ],
-        "-d": [
-            [0, "cmdoption-osxphotos-import-D"],
-            [0, "cmdoption-osxphotos-timewarp-D"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-timewarp-d"]
-        ],
-        "-f": [
-            [0, "cmdoption-osxphotos-timewarp-F"],
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-import-f"],
-            [0, "cmdoption-osxphotos-query-f"],
-            [0, "cmdoption-osxphotos-timewarp-1"],
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "-l": [
-            [0, "cmdoption-osxphotos-import-L"],
-            [0, "cmdoption-osxphotos-timewarp-L"],
-            [0, "cmdoption-osxphotos-import-l"]
-        ],
-        "-m": [
-            [0, "cmdoption-osxphotos-timewarp-M"],
-            [0, "cmdoption-osxphotos-import-m"],
-            [0, "cmdoption-osxphotos-sync-m"],
-            [0, "cmdoption-osxphotos-timewarp-0"]
-        ],
-        "-p": [
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-timewarp-P"],
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-timewarp-p"]
-        ],
-        "-r": [
-            [0, "cmdoption-osxphotos-import-R"],
-            [0, "cmdoption-osxphotos-sync-R"],
-            [0, "cmdoption-osxphotos-diff-r"],
-            [0, "cmdoption-osxphotos-import-r"]
-        ],
-        "-t": [
-            [0, "cmdoption-osxphotos-inspect-T"],
-            [0, "cmdoption-osxphotos-timewarp-T"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-inspect-t"],
-            [0, "cmdoption-osxphotos-timewarp-t"]
-        ],
-        "-u": [
-            [0, "cmdoption-osxphotos-install-U"],
-            [0, "cmdoption-osxphotos-sync-U"]
-        ],
-        "-v": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-timewarp-V"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "-e": [
-            [0, "cmdoption-osxphotos-import-e"],
-            [0, "cmdoption-osxphotos-sync-e"],
-            [0, "cmdoption-osxphotos-timewarp-e"]
-        ],
-        "-g": [
-            [0, "cmdoption-osxphotos-import-g"]
-        ],
-        "-h": [
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "-i": [
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-sync-0"],
-            [0, "cmdoption-osxphotos-sync-i"],
-            [0, "cmdoption-osxphotos-timewarp-i"]
-        ],
-        "-k": [
-            [0, "cmdoption-osxphotos-import-k"]
-        ],
-        "-s": [
-            [0, "cmdoption-osxphotos-diff-s"],
-            [0, "cmdoption-osxphotos-sync-s"]
-        ],
-        "-w": [
-            [0, "cmdoption-osxphotos-add-locations-w"],
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "-y": [
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "-z": [
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "args": [
-            [0, "cmdoption-osxphotos-run-arg-ARGS"]
-        ],
-        "db2": [
-            [0, "cmdoption-osxphotos-diff-arg-DB2"]
-        ],
-        "dest": [
-            [0, "cmdoption-osxphotos-export-arg-DEST"]
-        ],
-        "export_database": [
-            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"]
-        ],
-        "export_directory": [
-            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"]
-        ],
-        "files": [
-            [0, "cmdoption-osxphotos-import-arg-FILES"]
-        ],
-        "packages": [
-            [0, "cmdoption-osxphotos-install-arg-PACKAGES"],
-            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"]
-        ],
-        "photos_library": [
-            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"]
-        ],
-        "python_file": [
-            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"]
-        ],
-        "subtopic": [
-            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"]
-        ],
-        "topic": [
-            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
-        ],
-        "uuid_or_name": [
-            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"]
-        ],
-        "width": [
-            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
-        ],
-        "osxphotos command line option": [
-            [0, "cmdoption-osxphotos-json"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "osxphotos-add-locations command line option": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-add-locations-added-after"],
-            [0, "cmdoption-osxphotos-add-locations-added-before"],
-            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
-            [0, "cmdoption-osxphotos-add-locations-album"],
-            [0, "cmdoption-osxphotos-add-locations-burst"],
-            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
-            [0, "cmdoption-osxphotos-add-locations-description"],
-            [0, "cmdoption-osxphotos-add-locations-dry-run"],
-            [0, "cmdoption-osxphotos-add-locations-duplicate"],
-            [0, "cmdoption-osxphotos-add-locations-edited"],
-            [0, "cmdoption-osxphotos-add-locations-exif"],
-            [0, "cmdoption-osxphotos-add-locations-external-edit"],
-            [0, "cmdoption-osxphotos-add-locations-favorite"],
-            [0, "cmdoption-osxphotos-add-locations-folder"],
-            [0, "cmdoption-osxphotos-add-locations-from-date"],
-            [0, "cmdoption-osxphotos-add-locations-from-time"],
-            [0, "cmdoption-osxphotos-add-locations-has-comment"],
-            [0, "cmdoption-osxphotos-add-locations-has-likes"],
-            [0, "cmdoption-osxphotos-add-locations-has-raw"],
-            [0, "cmdoption-osxphotos-add-locations-hdr"],
-            [0, "cmdoption-osxphotos-add-locations-hidden"],
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-add-locations-in-album"],
-            [0, "cmdoption-osxphotos-add-locations-incloud"],
-            [0, "cmdoption-osxphotos-add-locations-is-reference"],
-            [0, "cmdoption-osxphotos-add-locations-keyword"],
-            [0, "cmdoption-osxphotos-add-locations-label"],
-            [0, "cmdoption-osxphotos-add-locations-live"],
-            [0, "cmdoption-osxphotos-add-locations-location"],
-            [0, "cmdoption-osxphotos-add-locations-max-size"],
-            [0, "cmdoption-osxphotos-add-locations-min-size"],
-            [0, "cmdoption-osxphotos-add-locations-missing"],
-            [0, "cmdoption-osxphotos-add-locations-name"],
-            [0, "cmdoption-osxphotos-add-locations-no-comment"],
-            [0, "cmdoption-osxphotos-add-locations-no-description"],
-            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
-            [0, "cmdoption-osxphotos-add-locations-no-likes"],
-            [0, "cmdoption-osxphotos-add-locations-no-location"],
-            [0, "cmdoption-osxphotos-add-locations-no-place"],
-            [0, "cmdoption-osxphotos-add-locations-no-title"],
-            [0, "cmdoption-osxphotos-add-locations-not-burst"],
-            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
-            [0, "cmdoption-osxphotos-add-locations-not-edited"],
-            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
-            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
-            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
-            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
-            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
-            [0, "cmdoption-osxphotos-add-locations-not-live"],
-            [0, "cmdoption-osxphotos-add-locations-not-missing"],
-            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
-            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
-            [0, "cmdoption-osxphotos-add-locations-not-reference"],
-            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
-            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
-            [0, "cmdoption-osxphotos-add-locations-not-shared"],
-            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
-            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
-            [0, "cmdoption-osxphotos-add-locations-only-movies"],
-            [0, "cmdoption-osxphotos-add-locations-only-photos"],
-            [0, "cmdoption-osxphotos-add-locations-panorama"],
-            [0, "cmdoption-osxphotos-add-locations-person"],
-            [0, "cmdoption-osxphotos-add-locations-place"],
-            [0, "cmdoption-osxphotos-add-locations-portrait"],
-            [0, "cmdoption-osxphotos-add-locations-query-eval"],
-            [0, "cmdoption-osxphotos-add-locations-query-function"],
-            [0, "cmdoption-osxphotos-add-locations-regex"],
-            [0, "cmdoption-osxphotos-add-locations-screenshot"],
-            [0, "cmdoption-osxphotos-add-locations-selected"],
-            [0, "cmdoption-osxphotos-add-locations-selfie"],
-            [0, "cmdoption-osxphotos-add-locations-shared"],
-            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
-            [0, "cmdoption-osxphotos-add-locations-theme"],
-            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
-            [0, "cmdoption-osxphotos-add-locations-timestamp"],
-            [0, "cmdoption-osxphotos-add-locations-title"],
-            [0, "cmdoption-osxphotos-add-locations-to-date"],
-            [0, "cmdoption-osxphotos-add-locations-to-time"],
-            [0, "cmdoption-osxphotos-add-locations-uti"],
-            [0, "cmdoption-osxphotos-add-locations-uuid"],
-            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
-            [0, "cmdoption-osxphotos-add-locations-w"],
-            [0, "cmdoption-osxphotos-add-locations-year"]
-        ],
-        "osxphotos-albums command line option": [
-            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-albums-json"],
-            [0, "cmdoption-osxphotos-albums-library"]
-        ],
-        "osxphotos-batch-edit command line option": [
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-batch-edit-description"],
-            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
-            [0, "cmdoption-osxphotos-batch-edit-keyword"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-batch-edit-location"],
-            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
-            [0, "cmdoption-osxphotos-batch-edit-theme"],
-            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
-            [0, "cmdoption-osxphotos-batch-edit-title"],
-            [0, "cmdoption-osxphotos-batch-edit-undo"]
-        ],
-        "osxphotos-diff command line option": [
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-diff-arg-DB2"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-diff-r"],
-            [0, "cmdoption-osxphotos-diff-s"],
-            [0, "cmdoption-osxphotos-diff-timestamp"]
-        ],
-        "osxphotos-dump command line option": [
-            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-dump-deleted"],
-            [0, "cmdoption-osxphotos-dump-deleted-only"],
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-dump-json"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-dump-print"]
-        ],
-        "osxphotos-exiftool command line option": [
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
-            [0, "cmdoption-osxphotos-exiftool-append"],
-            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"],
-            [0, "cmdoption-osxphotos-exiftool-db-config"],
-            [0, "cmdoption-osxphotos-exiftool-description-template"],
-            [0, "cmdoption-osxphotos-exiftool-dry-run"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
-            [0, "cmdoption-osxphotos-exiftool-exportdb"],
-            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-exiftool-load-config"],
-            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
-            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-report"],
-            [0, "cmdoption-osxphotos-exiftool-save-config"],
-            [0, "cmdoption-osxphotos-exiftool-theme"],
-            [0, "cmdoption-osxphotos-exiftool-timestamp"]
-        ],
-        "osxphotos-export command line option": [
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-export-add-exported-to-album"],
-            [0, "cmdoption-osxphotos-export-add-missing-to-album"],
-            [0, "cmdoption-osxphotos-export-add-skipped-to-album"],
-            [0, "cmdoption-osxphotos-export-added-after"],
-            [0, "cmdoption-osxphotos-export-added-before"],
-            [0, "cmdoption-osxphotos-export-added-in-last"],
-            [0, "cmdoption-osxphotos-export-album"],
-            [0, "cmdoption-osxphotos-export-album-keyword"],
-            [0, "cmdoption-osxphotos-export-alt-copy"],
-            [0, "cmdoption-osxphotos-export-append"],
-            [0, "cmdoption-osxphotos-export-arg-DEST"],
-            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-export-burst"],
-            [0, "cmdoption-osxphotos-export-cleanup"],
-            [0, "cmdoption-osxphotos-export-cloudasset"],
-            [0, "cmdoption-osxphotos-export-config-only"],
-            [0, "cmdoption-osxphotos-export-convert-to-jpeg"],
-            [0, "cmdoption-osxphotos-export-current-name"],
-            [0, "cmdoption-osxphotos-export-deleted"],
-            [0, "cmdoption-osxphotos-export-deleted-only"],
-            [0, "cmdoption-osxphotos-export-description"],
-            [0, "cmdoption-osxphotos-export-description-template"],
-            [0, "cmdoption-osxphotos-export-directory"],
-            [0, "cmdoption-osxphotos-export-download-missing"],
-            [0, "cmdoption-osxphotos-export-dry-run"],
-            [0, "cmdoption-osxphotos-export-duplicate"],
-            [0, "cmdoption-osxphotos-export-edited"],
-            [0, "cmdoption-osxphotos-export-edited-suffix"],
-            [0, "cmdoption-osxphotos-export-exif"],
-            [0, "cmdoption-osxphotos-export-exiftool"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-export-exiftool-option"],
-            [0, "cmdoption-osxphotos-export-exiftool-path"],
-            [0, "cmdoption-osxphotos-export-export-as-hardlink"],
-            [0, "cmdoption-osxphotos-export-export-by-date"],
-            [0, "cmdoption-osxphotos-export-exportdb"],
-            [0, "cmdoption-osxphotos-export-external-edit"],
-            [0, "cmdoption-osxphotos-export-favorite"],
-            [0, "cmdoption-osxphotos-export-favorite-rating"],
-            [0, "cmdoption-osxphotos-export-filename"],
-            [0, "cmdoption-osxphotos-export-finder-tag-keywords"],
-            [0, "cmdoption-osxphotos-export-finder-tag-template"],
-            [0, "cmdoption-osxphotos-export-folder"],
-            [0, "cmdoption-osxphotos-export-force-update"],
-            [0, "cmdoption-osxphotos-export-from-date"],
-            [0, "cmdoption-osxphotos-export-from-time"],
-            [0, "cmdoption-osxphotos-export-has-comment"],
-            [0, "cmdoption-osxphotos-export-has-likes"],
-            [0, "cmdoption-osxphotos-export-has-raw"],
-            [0, "cmdoption-osxphotos-export-hdr"],
-            [0, "cmdoption-osxphotos-export-hidden"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-export-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-export-ignore-signature"],
-            [0, "cmdoption-osxphotos-export-in-album"],
-            [0, "cmdoption-osxphotos-export-incloud"],
-            [0, "cmdoption-osxphotos-export-is-reference"],
-            [0, "cmdoption-osxphotos-export-jpeg-ext"],
-            [0, "cmdoption-osxphotos-export-jpeg-quality"],
-            [0, "cmdoption-osxphotos-export-keep"],
-            [0, "cmdoption-osxphotos-export-keyword"],
-            [0, "cmdoption-osxphotos-export-keyword-template"],
-            [0, "cmdoption-osxphotos-export-label"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-export-limit"],
-            [0, "cmdoption-osxphotos-export-live"],
-            [0, "cmdoption-osxphotos-export-load-config"],
-            [0, "cmdoption-osxphotos-export-location"],
-            [0, "cmdoption-osxphotos-export-max-size"],
-            [0, "cmdoption-osxphotos-export-min-size"],
-            [0, "cmdoption-osxphotos-export-missing"],
-            [0, "cmdoption-osxphotos-export-name"],
-            [0, "cmdoption-osxphotos-export-no-comment"],
-            [0, "cmdoption-osxphotos-export-no-description"],
-            [0, "cmdoption-osxphotos-export-no-keyword"],
-            [0, "cmdoption-osxphotos-export-no-likes"],
-            [0, "cmdoption-osxphotos-export-no-location"],
-            [0, "cmdoption-osxphotos-export-no-place"],
-            [0, "cmdoption-osxphotos-export-no-progress"],
-            [0, "cmdoption-osxphotos-export-no-title"],
-            [0, "cmdoption-osxphotos-export-not-burst"],
-            [0, "cmdoption-osxphotos-export-not-cloudasset"],
-            [0, "cmdoption-osxphotos-export-not-edited"],
-            [0, "cmdoption-osxphotos-export-not-favorite"],
-            [0, "cmdoption-osxphotos-export-not-hdr"],
-            [0, "cmdoption-osxphotos-export-not-hidden"],
-            [0, "cmdoption-osxphotos-export-not-in-album"],
-            [0, "cmdoption-osxphotos-export-not-incloud"],
-            [0, "cmdoption-osxphotos-export-not-live"],
-            [0, "cmdoption-osxphotos-export-not-missing"],
-            [0, "cmdoption-osxphotos-export-not-panorama"],
-            [0, "cmdoption-osxphotos-export-not-portrait"],
-            [0, "cmdoption-osxphotos-export-not-reference"],
-            [0, "cmdoption-osxphotos-export-not-screenshot"],
-            [0, "cmdoption-osxphotos-export-not-selfie"],
-            [0, "cmdoption-osxphotos-export-not-shared"],
-            [0, "cmdoption-osxphotos-export-not-slow-mo"],
-            [0, "cmdoption-osxphotos-export-not-time-lapse"],
-            [0, "cmdoption-osxphotos-export-only-movies"],
-            [0, "cmdoption-osxphotos-export-only-new"],
-            [0, "cmdoption-osxphotos-export-only-photos"],
-            [0, "cmdoption-osxphotos-export-original-suffix"],
-            [0, "cmdoption-osxphotos-export-overwrite"],
-            [0, "cmdoption-osxphotos-export-panorama"],
-            [0, "cmdoption-osxphotos-export-person"],
-            [0, "cmdoption-osxphotos-export-person-keyword"],
-            [0, "cmdoption-osxphotos-export-place"],
-            [0, "cmdoption-osxphotos-export-portrait"],
-            [0, "cmdoption-osxphotos-export-post-command"],
-            [0, "cmdoption-osxphotos-export-post-function"],
-            [0, "cmdoption-osxphotos-export-preview"],
-            [0, "cmdoption-osxphotos-export-preview-if-missing"],
-            [0, "cmdoption-osxphotos-export-preview-suffix"],
-            [0, "cmdoption-osxphotos-export-print"],
-            [0, "cmdoption-osxphotos-export-query-eval"],
-            [0, "cmdoption-osxphotos-export-query-function"],
-            [0, "cmdoption-osxphotos-export-ramdb"],
-            [0, "cmdoption-osxphotos-export-regex"],
-            [0, "cmdoption-osxphotos-export-replace-keywords"],
-            [0, "cmdoption-osxphotos-export-report"],
-            [0, "cmdoption-osxphotos-export-retry"],
-            [0, "cmdoption-osxphotos-export-save-config"],
-            [0, "cmdoption-osxphotos-export-screenshot"],
-            [0, "cmdoption-osxphotos-export-selected"],
-            [0, "cmdoption-osxphotos-export-selfie"],
-            [0, "cmdoption-osxphotos-export-shared"],
-            [0, "cmdoption-osxphotos-export-sidecar"],
-            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
-            [0, "cmdoption-osxphotos-export-skip-bursts"],
-            [0, "cmdoption-osxphotos-export-skip-edited"],
-            [0, "cmdoption-osxphotos-export-skip-live"],
-            [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
-            [0, "cmdoption-osxphotos-export-skip-raw"],
-            [0, "cmdoption-osxphotos-export-skip-uuid"],
-            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-slow-mo"],
-            [0, "cmdoption-osxphotos-export-strip"],
-            [0, "cmdoption-osxphotos-export-theme"],
-            [0, "cmdoption-osxphotos-export-time-lapse"],
-            [0, "cmdoption-osxphotos-export-timestamp"],
-            [0, "cmdoption-osxphotos-export-title"],
-            [0, "cmdoption-osxphotos-export-tmpdir"],
-            [0, "cmdoption-osxphotos-export-to-date"],
-            [0, "cmdoption-osxphotos-export-to-time"],
-            [0, "cmdoption-osxphotos-export-touch-file"],
-            [0, "cmdoption-osxphotos-export-update"],
-            [0, "cmdoption-osxphotos-export-update-errors"],
-            [0, "cmdoption-osxphotos-export-use-photokit"],
-            [0, "cmdoption-osxphotos-export-use-photos-export"],
-            [0, "cmdoption-osxphotos-export-uti"],
-            [0, "cmdoption-osxphotos-export-uuid"],
-            [0, "cmdoption-osxphotos-export-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-xattr-template"],
-            [0, "cmdoption-osxphotos-export-year"]
-        ],
-        "osxphotos-exportdb command line option": [
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-exportdb-append"],
-            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"],
-            [0, "cmdoption-osxphotos-exportdb-check-signatures"],
-            [0, "cmdoption-osxphotos-exportdb-delete-file"],
-            [0, "cmdoption-osxphotos-exportdb-delete-uuid"],
-            [0, "cmdoption-osxphotos-exportdb-dry-run"],
-            [0, "cmdoption-osxphotos-exportdb-errors"],
-            [0, "cmdoption-osxphotos-exportdb-export-dir"],
-            [0, "cmdoption-osxphotos-exportdb-info"],
-            [0, "cmdoption-osxphotos-exportdb-last-errors"],
-            [0, "cmdoption-osxphotos-exportdb-last-run"],
-            [0, "cmdoption-osxphotos-exportdb-migrate"],
-            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"],
-            [0, "cmdoption-osxphotos-exportdb-report"],
-            [0, "cmdoption-osxphotos-exportdb-save-config"],
-            [0, "cmdoption-osxphotos-exportdb-sql"],
-            [0, "cmdoption-osxphotos-exportdb-theme"],
-            [0, "cmdoption-osxphotos-exportdb-timestamp"],
-            [0, "cmdoption-osxphotos-exportdb-touch-file"],
-            [0, "cmdoption-osxphotos-exportdb-update-signatures"],
-            [0, "cmdoption-osxphotos-exportdb-uuid-files"],
-            [0, "cmdoption-osxphotos-exportdb-uuid-info"],
-            [0, "cmdoption-osxphotos-exportdb-vacuum"],
-            [0, "cmdoption-osxphotos-exportdb-version"]
-        ],
-        "osxphotos-help command line option": [
-            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"],
-            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
-        ],
-        "osxphotos-import command line option": [
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-import-C"],
-            [0, "cmdoption-osxphotos-import-D"],
-            [0, "cmdoption-osxphotos-import-L"],
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-import-R"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-import-append"],
-            [0, "cmdoption-osxphotos-import-arg-FILES"],
-            [0, "cmdoption-osxphotos-import-check-templates"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-import-e"],
-            [0, "cmdoption-osxphotos-import-f"],
-            [0, "cmdoption-osxphotos-import-g"],
-            [0, "cmdoption-osxphotos-import-k"],
-            [0, "cmdoption-osxphotos-import-l"],
-            [0, "cmdoption-osxphotos-import-m"],
-            [0, "cmdoption-osxphotos-import-no-progress"],
-            [0, "cmdoption-osxphotos-import-post-function"],
-            [0, "cmdoption-osxphotos-import-r"],
-            [0, "cmdoption-osxphotos-import-report"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-import-theme"],
-            [0, "cmdoption-osxphotos-import-timestamp"],
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "osxphotos-info command line option": [
-            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-info-json"],
-            [0, "cmdoption-osxphotos-info-library"]
-        ],
-        "osxphotos-inspect command line option": [
-            [0, "cmdoption-osxphotos-inspect-T"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-inspect-t"],
-            [0, "cmdoption-osxphotos-inspect-theme"]
-        ],
-        "osxphotos-install command line option": [
-            [0, "cmdoption-osxphotos-install-U"],
-            [0, "cmdoption-osxphotos-install-arg-PACKAGES"]
-        ],
-        "osxphotos-keywords command line option": [
-            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-keywords-json"],
-            [0, "cmdoption-osxphotos-keywords-library"]
-        ],
-        "osxphotos-labels command line option": [
-            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-labels-json"],
-            [0, "cmdoption-osxphotos-labels-library"]
-        ],
-        "osxphotos-list command line option": [
-            [0, "cmdoption-osxphotos-list-json"]
-        ],
-        "osxphotos-orphans command line option": [
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-orphans-export"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-orphans-theme"],
-            [0, "cmdoption-osxphotos-orphans-timestamp"]
-        ],
-        "osxphotos-persons command line option": [
-            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-persons-json"],
-            [0, "cmdoption-osxphotos-persons-library"]
-        ],
-        "osxphotos-places command line option": [
-            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-places-json"],
-            [0, "cmdoption-osxphotos-places-library"]
-        ],
-        "osxphotos-query command line option": [
-            [0, "cmdoption-osxphotos-query-add-to-album"],
-            [0, "cmdoption-osxphotos-query-added-after"],
-            [0, "cmdoption-osxphotos-query-added-before"],
-            [0, "cmdoption-osxphotos-query-added-in-last"],
-            [0, "cmdoption-osxphotos-query-album"],
-            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-query-burst"],
-            [0, "cmdoption-osxphotos-query-cloudasset"],
-            [0, "cmdoption-osxphotos-query-deleted"],
-            [0, "cmdoption-osxphotos-query-deleted-only"],
-            [0, "cmdoption-osxphotos-query-description"],
-            [0, "cmdoption-osxphotos-query-duplicate"],
-            [0, "cmdoption-osxphotos-query-edited"],
-            [0, "cmdoption-osxphotos-query-exif"],
-            [0, "cmdoption-osxphotos-query-external-edit"],
-            [0, "cmdoption-osxphotos-query-f"],
-            [0, "cmdoption-osxphotos-query-favorite"],
-            [0, "cmdoption-osxphotos-query-folder"],
-            [0, "cmdoption-osxphotos-query-from-date"],
-            [0, "cmdoption-osxphotos-query-from-time"],
-            [0, "cmdoption-osxphotos-query-has-comment"],
-            [0, "cmdoption-osxphotos-query-has-likes"],
-            [0, "cmdoption-osxphotos-query-has-raw"],
-            [0, "cmdoption-osxphotos-query-hdr"],
-            [0, "cmdoption-osxphotos-query-hidden"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-query-in-album"],
-            [0, "cmdoption-osxphotos-query-incloud"],
-            [0, "cmdoption-osxphotos-query-is-reference"],
-            [0, "cmdoption-osxphotos-query-json"],
-            [0, "cmdoption-osxphotos-query-keyword"],
-            [0, "cmdoption-osxphotos-query-label"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-query-live"],
-            [0, "cmdoption-osxphotos-query-location"],
-            [0, "cmdoption-osxphotos-query-max-size"],
-            [0, "cmdoption-osxphotos-query-min-size"],
-            [0, "cmdoption-osxphotos-query-missing"],
-            [0, "cmdoption-osxphotos-query-name"],
-            [0, "cmdoption-osxphotos-query-no-comment"],
-            [0, "cmdoption-osxphotos-query-no-description"],
-            [0, "cmdoption-osxphotos-query-no-keyword"],
-            [0, "cmdoption-osxphotos-query-no-likes"],
-            [0, "cmdoption-osxphotos-query-no-location"],
-            [0, "cmdoption-osxphotos-query-no-place"],
-            [0, "cmdoption-osxphotos-query-no-title"],
-            [0, "cmdoption-osxphotos-query-not-burst"],
-            [0, "cmdoption-osxphotos-query-not-cloudasset"],
-            [0, "cmdoption-osxphotos-query-not-edited"],
-            [0, "cmdoption-osxphotos-query-not-favorite"],
-            [0, "cmdoption-osxphotos-query-not-hdr"],
-            [0, "cmdoption-osxphotos-query-not-hidden"],
-            [0, "cmdoption-osxphotos-query-not-in-album"],
-            [0, "cmdoption-osxphotos-query-not-incloud"],
-            [0, "cmdoption-osxphotos-query-not-live"],
-            [0, "cmdoption-osxphotos-query-not-missing"],
-            [0, "cmdoption-osxphotos-query-not-panorama"],
-            [0, "cmdoption-osxphotos-query-not-portrait"],
-            [0, "cmdoption-osxphotos-query-not-reference"],
-            [0, "cmdoption-osxphotos-query-not-screenshot"],
-            [0, "cmdoption-osxphotos-query-not-selfie"],
-            [0, "cmdoption-osxphotos-query-not-shared"],
-            [0, "cmdoption-osxphotos-query-not-slow-mo"],
-            [0, "cmdoption-osxphotos-query-not-time-lapse"],
-            [0, "cmdoption-osxphotos-query-only-movies"],
-            [0, "cmdoption-osxphotos-query-only-photos"],
-            [0, "cmdoption-osxphotos-query-panorama"],
-            [0, "cmdoption-osxphotos-query-person"],
-            [0, "cmdoption-osxphotos-query-place"],
-            [0, "cmdoption-osxphotos-query-portrait"],
-            [0, "cmdoption-osxphotos-query-print"],
-            [0, "cmdoption-osxphotos-query-query-eval"],
-            [0, "cmdoption-osxphotos-query-query-function"],
-            [0, "cmdoption-osxphotos-query-quiet"],
-            [0, "cmdoption-osxphotos-query-regex"],
-            [0, "cmdoption-osxphotos-query-screenshot"],
-            [0, "cmdoption-osxphotos-query-selected"],
-            [0, "cmdoption-osxphotos-query-selfie"],
-            [0, "cmdoption-osxphotos-query-shared"],
-            [0, "cmdoption-osxphotos-query-slow-mo"],
-            [0, "cmdoption-osxphotos-query-time-lapse"],
-            [0, "cmdoption-osxphotos-query-title"],
-            [0, "cmdoption-osxphotos-query-to-date"],
-            [0, "cmdoption-osxphotos-query-to-time"],
-            [0, "cmdoption-osxphotos-query-uti"],
-            [0, "cmdoption-osxphotos-query-uuid"],
-            [0, "cmdoption-osxphotos-query-uuid-from-file"],
-            [0, "cmdoption-osxphotos-query-year"]
-        ],
-        "osxphotos-repl command line option": [
-            [0, "cmdoption-osxphotos-repl-added-after"],
-            [0, "cmdoption-osxphotos-repl-added-before"],
-            [0, "cmdoption-osxphotos-repl-added-in-last"],
-            [0, "cmdoption-osxphotos-repl-album"],
-            [0, "cmdoption-osxphotos-repl-burst"],
-            [0, "cmdoption-osxphotos-repl-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-deleted"],
-            [0, "cmdoption-osxphotos-repl-deleted-only"],
-            [0, "cmdoption-osxphotos-repl-description"],
-            [0, "cmdoption-osxphotos-repl-duplicate"],
-            [0, "cmdoption-osxphotos-repl-edited"],
-            [0, "cmdoption-osxphotos-repl-emacs"],
-            [0, "cmdoption-osxphotos-repl-exif"],
-            [0, "cmdoption-osxphotos-repl-external-edit"],
-            [0, "cmdoption-osxphotos-repl-favorite"],
-            [0, "cmdoption-osxphotos-repl-folder"],
-            [0, "cmdoption-osxphotos-repl-from-date"],
-            [0, "cmdoption-osxphotos-repl-from-time"],
-            [0, "cmdoption-osxphotos-repl-has-comment"],
-            [0, "cmdoption-osxphotos-repl-has-likes"],
-            [0, "cmdoption-osxphotos-repl-has-raw"],
-            [0, "cmdoption-osxphotos-repl-hdr"],
-            [0, "cmdoption-osxphotos-repl-hidden"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-repl-in-album"],
-            [0, "cmdoption-osxphotos-repl-incloud"],
-            [0, "cmdoption-osxphotos-repl-is-reference"],
-            [0, "cmdoption-osxphotos-repl-keyword"],
-            [0, "cmdoption-osxphotos-repl-label"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-repl-live"],
-            [0, "cmdoption-osxphotos-repl-location"],
-            [0, "cmdoption-osxphotos-repl-max-size"],
-            [0, "cmdoption-osxphotos-repl-min-size"],
-            [0, "cmdoption-osxphotos-repl-missing"],
-            [0, "cmdoption-osxphotos-repl-name"],
-            [0, "cmdoption-osxphotos-repl-no-comment"],
-            [0, "cmdoption-osxphotos-repl-no-description"],
-            [0, "cmdoption-osxphotos-repl-no-keyword"],
-            [0, "cmdoption-osxphotos-repl-no-likes"],
-            [0, "cmdoption-osxphotos-repl-no-location"],
-            [0, "cmdoption-osxphotos-repl-no-place"],
-            [0, "cmdoption-osxphotos-repl-no-title"],
-            [0, "cmdoption-osxphotos-repl-not-burst"],
-            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-not-edited"],
-            [0, "cmdoption-osxphotos-repl-not-favorite"],
-            [0, "cmdoption-osxphotos-repl-not-hdr"],
-            [0, "cmdoption-osxphotos-repl-not-hidden"],
-            [0, "cmdoption-osxphotos-repl-not-in-album"],
-            [0, "cmdoption-osxphotos-repl-not-incloud"],
-            [0, "cmdoption-osxphotos-repl-not-live"],
-            [0, "cmdoption-osxphotos-repl-not-missing"],
-            [0, "cmdoption-osxphotos-repl-not-panorama"],
-            [0, "cmdoption-osxphotos-repl-not-portrait"],
-            [0, "cmdoption-osxphotos-repl-not-reference"],
-            [0, "cmdoption-osxphotos-repl-not-screenshot"],
-            [0, "cmdoption-osxphotos-repl-not-selfie"],
-            [0, "cmdoption-osxphotos-repl-not-shared"],
-            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-only-movies"],
-            [0, "cmdoption-osxphotos-repl-only-photos"],
-            [0, "cmdoption-osxphotos-repl-panorama"],
-            [0, "cmdoption-osxphotos-repl-person"],
-            [0, "cmdoption-osxphotos-repl-place"],
-            [0, "cmdoption-osxphotos-repl-portrait"],
-            [0, "cmdoption-osxphotos-repl-query-eval"],
-            [0, "cmdoption-osxphotos-repl-query-function"],
-            [0, "cmdoption-osxphotos-repl-regex"],
-            [0, "cmdoption-osxphotos-repl-screenshot"],
-            [0, "cmdoption-osxphotos-repl-selected"],
-            [0, "cmdoption-osxphotos-repl-selfie"],
-            [0, "cmdoption-osxphotos-repl-shared"],
-            [0, "cmdoption-osxphotos-repl-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-title"],
-            [0, "cmdoption-osxphotos-repl-to-date"],
-            [0, "cmdoption-osxphotos-repl-to-time"],
-            [0, "cmdoption-osxphotos-repl-uti"],
-            [0, "cmdoption-osxphotos-repl-uuid"],
-            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
-            [0, "cmdoption-osxphotos-repl-year"]
-        ],
-        "osxphotos-run command line option": [
-            [0, "cmdoption-osxphotos-run-arg-ARGS"],
-            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"],
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "osxphotos-show command line option": [
-            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"],
-            [0, "cmdoption-osxphotos-show-library"]
-        ],
-        "osxphotos-snap command line option": [
-            [0, "cmdoption-osxphotos-snap-library"]
-        ],
-        "osxphotos-sync command line option": [
-            [0, "cmdoption-osxphotos-sync-0"],
-            [0, "cmdoption-osxphotos-sync-A"],
-            [0, "cmdoption-osxphotos-sync-R"],
-            [0, "cmdoption-osxphotos-sync-U"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-sync-added-after"],
-            [0, "cmdoption-osxphotos-sync-added-before"],
-            [0, "cmdoption-osxphotos-sync-added-in-last"],
-            [0, "cmdoption-osxphotos-sync-album"],
-            [0, "cmdoption-osxphotos-sync-burst"],
-            [0, "cmdoption-osxphotos-sync-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-description"],
-            [0, "cmdoption-osxphotos-sync-dry-run"],
-            [0, "cmdoption-osxphotos-sync-duplicate"],
-            [0, "cmdoption-osxphotos-sync-e"],
-            [0, "cmdoption-osxphotos-sync-edited"],
-            [0, "cmdoption-osxphotos-sync-exif"],
-            [0, "cmdoption-osxphotos-sync-external-edit"],
-            [0, "cmdoption-osxphotos-sync-favorite"],
-            [0, "cmdoption-osxphotos-sync-folder"],
-            [0, "cmdoption-osxphotos-sync-from-date"],
-            [0, "cmdoption-osxphotos-sync-from-time"],
-            [0, "cmdoption-osxphotos-sync-has-comment"],
-            [0, "cmdoption-osxphotos-sync-has-likes"],
-            [0, "cmdoption-osxphotos-sync-has-raw"],
-            [0, "cmdoption-osxphotos-sync-hdr"],
-            [0, "cmdoption-osxphotos-sync-hidden"],
-            [0, "cmdoption-osxphotos-sync-i"],
-            [0, "cmdoption-osxphotos-sync-in-album"],
-            [0, "cmdoption-osxphotos-sync-incloud"],
-            [0, "cmdoption-osxphotos-sync-is-reference"],
-            [0, "cmdoption-osxphotos-sync-keyword"],
-            [0, "cmdoption-osxphotos-sync-label"],
-            [0, "cmdoption-osxphotos-sync-library"],
-            [0, "cmdoption-osxphotos-sync-live"],
-            [0, "cmdoption-osxphotos-sync-location"],
-            [0, "cmdoption-osxphotos-sync-m"],
-            [0, "cmdoption-osxphotos-sync-max-size"],
-            [0, "cmdoption-osxphotos-sync-min-size"],
-            [0, "cmdoption-osxphotos-sync-missing"],
-            [0, "cmdoption-osxphotos-sync-name"],
-            [0, "cmdoption-osxphotos-sync-no-comment"],
-            [0, "cmdoption-osxphotos-sync-no-description"],
-            [0, "cmdoption-osxphotos-sync-no-keyword"],
-            [0, "cmdoption-osxphotos-sync-no-likes"],
-            [0, "cmdoption-osxphotos-sync-no-location"],
-            [0, "cmdoption-osxphotos-sync-no-place"],
-            [0, "cmdoption-osxphotos-sync-no-title"],
-            [0, "cmdoption-osxphotos-sync-not-burst"],
-            [0, "cmdoption-osxphotos-sync-not-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-not-edited"],
-            [0, "cmdoption-osxphotos-sync-not-favorite"],
-            [0, "cmdoption-osxphotos-sync-not-hdr"],
-            [0, "cmdoption-osxphotos-sync-not-hidden"],
-            [0, "cmdoption-osxphotos-sync-not-in-album"],
-            [0, "cmdoption-osxphotos-sync-not-incloud"],
-            [0, "cmdoption-osxphotos-sync-not-live"],
-            [0, "cmdoption-osxphotos-sync-not-missing"],
-            [0, "cmdoption-osxphotos-sync-not-panorama"],
-            [0, "cmdoption-osxphotos-sync-not-portrait"],
-            [0, "cmdoption-osxphotos-sync-not-reference"],
-            [0, "cmdoption-osxphotos-sync-not-screenshot"],
-            [0, "cmdoption-osxphotos-sync-not-selfie"],
-            [0, "cmdoption-osxphotos-sync-not-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-not-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-only-movies"],
-            [0, "cmdoption-osxphotos-sync-only-photos"],
-            [0, "cmdoption-osxphotos-sync-panorama"],
-            [0, "cmdoption-osxphotos-sync-person"],
-            [0, "cmdoption-osxphotos-sync-place"],
-            [0, "cmdoption-osxphotos-sync-portrait"],
-            [0, "cmdoption-osxphotos-sync-query-eval"],
-            [0, "cmdoption-osxphotos-sync-query-function"],
-            [0, "cmdoption-osxphotos-sync-regex"],
-            [0, "cmdoption-osxphotos-sync-s"],
-            [0, "cmdoption-osxphotos-sync-screenshot"],
-            [0, "cmdoption-osxphotos-sync-selected"],
-            [0, "cmdoption-osxphotos-sync-selfie"],
-            [0, "cmdoption-osxphotos-sync-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-theme"],
-            [0, "cmdoption-osxphotos-sync-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-timestamp"],
-            [0, "cmdoption-osxphotos-sync-title"],
-            [0, "cmdoption-osxphotos-sync-to-date"],
-            [0, "cmdoption-osxphotos-sync-to-time"],
-            [0, "cmdoption-osxphotos-sync-uti"],
-            [0, "cmdoption-osxphotos-sync-uuid"],
-            [0, "cmdoption-osxphotos-sync-uuid-from-file"],
-            [0, "cmdoption-osxphotos-sync-year"]
-        ],
-        "osxphotos-theme command line option": [
-            [0, "cmdoption-osxphotos-theme-clone"],
-            [0, "cmdoption-osxphotos-theme-config"],
-            [0, "cmdoption-osxphotos-theme-default"],
-            [0, "cmdoption-osxphotos-theme-delete"],
-            [0, "cmdoption-osxphotos-theme-edit"],
-            [0, "cmdoption-osxphotos-theme-list"],
-            [0, "cmdoption-osxphotos-theme-preview"]
-        ],
-        "osxphotos-timewarp command line option": [
-            [0, "cmdoption-osxphotos-timewarp-0"],
-            [0, "cmdoption-osxphotos-timewarp-1"],
-            [0, "cmdoption-osxphotos-timewarp-2"],
-            [0, "cmdoption-osxphotos-timewarp-D"],
-            [0, "cmdoption-osxphotos-timewarp-F"],
-            [0, "cmdoption-osxphotos-timewarp-L"],
-            [0, "cmdoption-osxphotos-timewarp-M"],
-            [0, "cmdoption-osxphotos-timewarp-P"],
-            [0, "cmdoption-osxphotos-timewarp-T"],
-            [0, "cmdoption-osxphotos-timewarp-V"],
-            [0, "cmdoption-osxphotos-timewarp-a"],
-            [0, "cmdoption-osxphotos-timewarp-c"],
-            [0, "cmdoption-osxphotos-timewarp-d"],
-            [0, "cmdoption-osxphotos-timewarp-date-added"],
-            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"],
-            [0, "cmdoption-osxphotos-timewarp-e"],
-            [0, "cmdoption-osxphotos-timewarp-force"],
-            [0, "cmdoption-osxphotos-timewarp-i"],
-            [0, "cmdoption-osxphotos-timewarp-p"],
-            [0, "cmdoption-osxphotos-timewarp-plain"],
-            [0, "cmdoption-osxphotos-timewarp-t"],
-            [0, "cmdoption-osxphotos-timewarp-theme"],
-            [0, "cmdoption-osxphotos-timewarp-timestamp"],
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "osxphotos-tutorial command line option": [
-            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
-        ],
-        "osxphotos-uninstall command line option": [
-            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"],
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "osxphotos-uuid command line option": [
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "osxphotos-version command line option": [
-            [0, "cmdoption-osxphotos-version-run"]
-        ],
         "albuminfo (class in osxphotos)": [
             [4, "osxphotos.AlbumInfo"]
         ],
         "albumsortorder (class in osxphotos)": [
             [4, "osxphotos.AlbumSortOrder"]
         ],
         "commentinfo (class in osxphotos)": [
@@ -7154,14 +5144,17 @@
         ],
         "subfolders (osxphotos.folderinfo property)": [
             [4, "osxphotos.FolderInfo.subfolders"]
         ],
         "subtitle (osxphotos.momentinfo property)": [
             [4, "osxphotos.MomentInfo.subtitle"]
         ],
+        "tables() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.tables"]
+        ],
         "text_found (osxphotos.searchinfo property)": [
             [4, "osxphotos.SearchInfo.text_found"]
         ],
         "time_lapse (osxphotos.photoinfo property)": [
             [4, "osxphotos.PhotoInfo.time_lapse"]
         ],
         "time_lapse (osxphotos.queryoptions attribute)": [
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.59.3 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.59.3’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.0’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.59.3â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.0â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.59.3 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.3_documentation
+osxphotos_0.60.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.59.3/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.0/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/exifinfo.py` & `osxphotos-0.60.0/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/exiftool.py` & `osxphotos-0.60.0/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.0/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/export_db.py` & `osxphotos-0.60.0/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/export_db_utils.py` & `osxphotos-0.60.0/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/fileutil.py` & `osxphotos-0.60.0/osxphotos/fileutil.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import shutil
 import stat
 import tempfile
 import typing as t
 from abc import ABC, abstractmethod
 from tempfile import TemporaryDirectory
 
-import Foundation
-
 from .imageconverter import ImageConverter
+from .utils import is_macos, normalize_fs_path
+
+if is_macos:
+    import Foundation
 
 __all__ = ["FileUtilABC", "FileUtilMacOS", "FileUtilShUtil", "FileUtil", "FileUtilNoOp"]
 
 
 class FileUtilABC(ABC):
     """Abstract base class for FileUtil"""
 
@@ -86,14 +88,17 @@
         src: source path as string
         dest: destination path as string
         Raises exception if linking fails or either path is None"""
 
         if src is None or dest is None:
             raise ValueError("src and dest must not be None", src, dest)
 
+        src = normalize_fs_path(src)
+        dest = normalize_fs_path(dest)
+
         if not os.path.isfile(src):
             raise FileNotFoundError("src file does not appear to exist", src)
 
         try:
             os.link(src, dest)
         except Exception as e:
             raise e from e
@@ -111,14 +116,17 @@
         Returns:
             True if copy succeeded
 
         Raises:
             OSError if copy fails
             TypeError if either path is None
         """
+        src = normalize_fs_path(src)
+        dest = normalize_fs_path(dest)
+
         if not isinstance(src, pathlib.Path):
             src = pathlib.Path(src)
 
         if not isinstance(dest, pathlib.Path):
             dest = pathlib.Path(dest)
 
         if dest.is_dir():
@@ -131,30 +139,33 @@
         if not error[0]:
             raise OSError(error[1])
         return True
 
     @classmethod
     def unlink(cls, filepath):
         """unlink filepath; if it's pathlib.Path, use Path.unlink, otherwise use os.unlink"""
+        filepath = normalize_fs_path(filepath)
         if isinstance(filepath, pathlib.Path):
             filepath.unlink()
         else:
             os.unlink(filepath)
 
     @classmethod
     def rmdir(cls, dirpath):
         """remove directory filepath; dirpath must be empty"""
+        dirpath = normalize_fs_path(dirpath)
         if isinstance(dirpath, pathlib.Path):
             dirpath.rmdir()
         else:
             os.rmdir(dirpath)
 
     @classmethod
     def utime(cls, path, times):
         """Set the access and modified time of path."""
+        path = normalize_fs_path(path)
         os.utime(path, times=times)
 
     @classmethod
     def cmp(cls, f1, f2, mtime1=None):
         """Does shallow compare (file signatures) of f1 to file f2.
         Arguments:
         f1 --  File name
@@ -162,14 +173,17 @@
         mtime1 -- optional, pass alternate file modification timestamp for f1; will be converted to int
 
         Return value:
         True if the file signatures as returned by stat are the same, False otherwise.
         Does not do a byte-by-byte comparison.
         """
 
+        f1 = normalize_fs_path(f1)
+        f2 = normalize_fs_path(f2)
+
         s1 = cls._sig(os.stat(f1))
         if mtime1 is not None:
             s1 = (s1[0], s1[1], int(mtime1))
         s2 = cls._sig(os.stat(f2))
         if s1[0] != stat.S_IFREG or s2[0] != stat.S_IFREG:
             return False
         return s1 == s2
@@ -184,36 +198,40 @@
         Return value:
         True if the files are the same, False otherwise.
         """
 
         if not s2:
             return False
 
+        f1 = normalize_fs_path(f1)
         s1 = cls._sig(os.stat(f1))
         if s1[0] != stat.S_IFREG or s2[0] != stat.S_IFREG:
             return False
         return s1 == s2
 
     @classmethod
     def file_sig(cls, f1):
         """return os.stat signature for file f1 as tuple of (mode, size, mtime)"""
+        f1 = normalize_fs_path(f1)
         return cls._sig(os.stat(f1))
 
     @classmethod
     def convert_to_jpeg(cls, src_file, dest_file, compression_quality=1.0):
         """converts image file src_file to jpeg format as dest_file
 
         Args:
             src_file: image file to convert
             dest_file: destination path to write converted file to
             compression quality: JPEG compression quality in range 0.0 <= compression_quality <= 1.0; default 1.0 (best quality)
 
         Returns:
             True if success, otherwise False
         """
+        src_file = normalize_fs_path(src_file)
+        dest_file = normalize_fs_path(dest_file)
         converter = ImageConverter()
         return converter.write_jpeg(
             src_file, dest_file, compression_quality=compression_quality
         )
 
     @classmethod
     def rename(cls, src, dest):
@@ -223,14 +241,16 @@
             src: path to source file
             dest: path to destination file
 
         Returns:
             Name of renamed file (dest)
 
         """
+        src = normalize_fs_path(src)
+        dest = normalize_fs_path(dest)
         os.rename(str(src), str(dest))
         return dest
 
     @classmethod
     def tmpdir(
         cls, prefix: t.Optional[str] = None, dir: t.Optional[str] = None
     ) -> tempfile.TemporaryDirectory:
@@ -267,14 +287,17 @@
         Returns:
             True if copy succeeded
 
         Raises:
             OSError if copy fails
             TypeError if either path is None
         """
+        src = normalize_fs_path(src)
+        dest = normalize_fs_path(dest)
+
         if not isinstance(src, pathlib.Path):
             src = pathlib.Path(src)
 
         if not isinstance(dest, pathlib.Path):
             dest = pathlib.Path(dest)
 
         if dest.is_dir():
@@ -284,15 +307,15 @@
             shutil.copy(str(src), str(dest))
         except Exception as e:
             raise OSError(f"Error copying {src} to {dest}: {e}") from e
 
         return True
 
 
-class FileUtil(FileUtilMacOS):
+class FileUtil(FileUtilShUtil):
     """Various file utilities"""
 
     pass
 
 
 class FileUtilNoOp(FileUtil):
     """No-Op implementation of FileUtil for testing / dry-run mode
```

### Comparing `osxphotos-0.59.3/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.0/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/imageconverter.py` & `osxphotos-0.60.0/osxphotos/imageconverter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """ ImageConverter class
     Convert an image to JPEG using CoreImage --
     for example, RAW to JPEG.  Only works if Mac equipped with GPU. """
 
 # reference: https://stackoverflow.com/questions/59330149/coreimage-ciimage-write-jpg-is-shifting-colors-macos/59334308#59334308
 
 import pathlib
-
-import objc
-import Metal
-import Quartz
-from Cocoa import NSURL
-from Foundation import NSDictionary
+import sys
 
 # needed to capture system-level stderr
 from wurlitzer import pipes
 
+from .utils import is_macos
+
+if is_macos:
+    import objc
+    import Metal
+    import Quartz
+    from Cocoa import NSURL
+    from Foundation import NSDictionary
+
 __all__ = ["ImageConversionError", "ImageConverter"]
 
 
 class ImageConversionError(Exception):
     """Base class for exceptions in this module."""
 
     pass
```

### Comparing `osxphotos-0.59.3/osxphotos/momentinfo.py` & `osxphotos-0.60.0/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/path_utils.py` & `osxphotos-0.60.0/osxphotos/path_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,24 @@
-""" utility functions for validating/sanitizing path components """
+""" utility functions for validating/sanitizing path components
+
+This module also performs Unicode normalization. For a quick summary, there are
+multiple ways to write more complex characters in Unicode. This causes problems
+when e.g. checking if a file already exists and you have multiple sources for
+the same string with different encodings. This sadly happens in Photos, but
+isn't a problem on macOS, since macOS does normalization behind-the-scenes (see
+https://eclecticlight.co/2021/05/08/explainer-unicode-normalization-and-apfs/).
+This causes problems on other platforms, so we normalize as part of filename
+sanitization functions and rely on them being called every time a unique
+filename is needed.
+"""
 
 import pathvalidate
 
+from osxphotos.utils import normalize_unicode
+
 from ._constants import MAX_DIRNAME_LEN, MAX_FILENAME_LEN
 
 __all__ = [
     "sanitize_filepath",
     "is_valid_filepath",
     "sanitize_filename",
     "sanitize_dirname",
@@ -20,25 +33,26 @@
 
 def is_valid_filepath(filepath):
     """returns True if a filepath is valid otherwise False"""
     return pathvalidate.is_valid_filepath(filepath, platform="macos")
 
 
 def sanitize_filename(filename, replacement=":"):
-    """replace any illegal characters in a filename and truncate filename if needed
+    """replace any illegal characters in a filename, truncate filename if needed and normalize Unicode to NFC form
 
     Args:
         filename: str, filename to sanitze
         replacement: str, value to replace any illegal characters with; default = ":"
 
     Returns:
         filename with any illegal characters replaced by replacement and truncated if necessary
     """
 
     if filename:
+        filename = normalize_unicode(filename)
         filename = filename.replace("/", replacement)
         if len(filename) > MAX_FILENAME_LEN:
             parts = filename.split(".")
             drop = len(filename) - MAX_FILENAME_LEN
             if len(parts) > 1:
                 # has an extension
                 ext = parts.pop(-1)
@@ -50,39 +64,40 @@
                 filename = f"{stem}.{ext}"
             else:
                 filename = filename[:-drop]
     return filename
 
 
 def sanitize_dirname(dirname, replacement=":"):
-    """replace any illegal characters in a directory name and truncate directory name if needed
+    """replace any illegal characters in a directory name, truncate directory name if needed, and normalize Unicode to NFC form
 
     Args:
         dirname: str, directory name to sanitize
         replacement: str, value to replace any illegal characters with; default = ":"; if None, no replacement occurs
 
     Returns:
         dirname with any illegal characters replaced by replacement and truncated if necessary
     """
     if dirname:
         dirname = sanitize_pathpart(dirname, replacement=replacement)
     return dirname
 
 
 def sanitize_pathpart(pathpart, replacement=":"):
-    """replace any illegal characters in a path part (either directory or filename without extension) and truncate name if needed
+    """replace any illegal characters in a path part (either directory or filename without extension), truncate name if needed, and normalize Unicode to NFC form
 
     Args:
         pathpart: str, path part to sanitize
         replacement: str, value to replace any illegal characters with; default = ":"; if None, no replacement occurs
 
     Returns:
         pathpart with any illegal characters replaced by replacement and truncated if necessary
     """
     if pathpart:
         pathpart = (
             pathpart.replace("/", replacement) if replacement is not None else pathpart
         )
+        pathpart = normalize_unicode(pathpart)
         if len(pathpart) > MAX_DIRNAME_LEN:
             drop = len(pathpart) - MAX_DIRNAME_LEN
             pathpart = pathpart[:-drop]
     return pathpart
```

### Comparing `osxphotos-0.59.3/osxphotos/personinfo.py` & `osxphotos-0.60.0/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/photodates.py` & `osxphotos-0.60.0/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/photoexporter.py` & `osxphotos-0.60.0/osxphotos/photoexporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 import dataclasses
 import json
 import logging
 import os
 import pathlib
 import re
+import sys
 import typing as t
 from collections import namedtuple  # pylint: disable=syntax-error
 from dataclasses import asdict, dataclass
 from datetime import datetime
 from enum import Enum
 from types import SimpleNamespace
 
-import photoscript
 from mako.template import Template
 
 from ._constants import (
     _MAX_IPTC_KEYWORD_LEN,
     _OSXPHOTOS_NONE_SENTINEL,
     _TEMPLATE_DIR,
     _UNKNOWN_PERSON,
@@ -31,34 +31,41 @@
     SIDECAR_XMP,
 )
 from ._version import __version__
 from .datetime_utils import datetime_tz_to_utc
 from .exiftool import ExifTool, ExifToolCaching, exiftool_can_write, get_exiftool_path
 from .export_db import ExportDB, ExportDBTemp
 from .fileutil import FileUtil
-from .photokit import (
-    PHOTOS_VERSION_CURRENT,
-    PHOTOS_VERSION_ORIGINAL,
-    PHOTOS_VERSION_UNADJUSTED,
-    PhotoKitFetchFailed,
-    PhotoLibrary,
-)
 from .phototemplate import RenderOptions
 from .rich_utils import add_rich_markup_tag
 from .uti import get_preferred_uti_extension
 from .utils import (
+    is_macos,
     hexdigest,
     increment_filename,
     increment_filename_with_count,
     lineno,
     list_directory,
     lock_filename,
+    normalize_fs_path,
     unlock_filename,
 )
 
+if is_macos:
+    import photoscript
+
+    from .photokit import (
+        PHOTOS_VERSION_CURRENT,
+        PHOTOS_VERSION_ORIGINAL,
+        PHOTOS_VERSION_UNADJUSTED,
+        PhotoKitFetchFailed,
+        PhotoLibrary,
+    )
+
+
 __all__ = [
     "ExportError",
     "ExportOptions",
     "ExportResults",
     "PhotoExporter",
     "rename_jpeg_files",
 ]
@@ -717,15 +724,14 @@
         _lock_filename(dest)
         return dest
 
     def _should_update_photo(
         self, src: pathlib.Path, dest: pathlib.Path, options: ExportOptions
     ) -> t.Literal[True, False]:
         """Return True if photo should be updated, else False"""
-
         # NOTE: The order of certain checks is important
         # read the comments below to understand why before changing
 
         export_db = options.export_db
         fileutil = options.fileutil
 
         file_record = export_db.get_file_record(dest)
@@ -1177,15 +1183,15 @@
                     exif_results = self.write_exiftool_metadata_to_file(
                         src, dest, options=options
                     )
 
                 try:
                     fileutil.copy(src, dest_str)
                     verbose(
-                        f"Exported {self._filename(self.photo.original_filename)} to {self._filepath(dest_str)}"
+                        f"Exported {self._filename(self.photo.original_filename)} to {self._filepath(normalize_fs_path(dest_str))}"
                     )
                 except Exception as e:
                     raise ExportError(
                         f"Error copying file {src} to {dest_str}: {e} ({lineno(__file__)})"
                     ) from e
 
         results = ExportResults(
```

### Comparing `osxphotos-0.59.3/osxphotos/photoinfo.py` & `osxphotos-0.60.0/osxphotos/photoinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import re
 from datetime import timedelta, timezone
 from functools import cached_property
 from types import SimpleNamespace
 from typing import Any, Dict, Optional
 
 import yaml
-from osxmetadata import OSXMetaData
 
 import osxphotos
 
 from ._constants import (
     _DB_TABLE_NAMES,
     _MOVIE_TYPE,
     _PHOTO_TYPE,
@@ -55,22 +54,26 @@
 from .adjustmentsinfo import AdjustmentsInfo
 from .albuminfo import AlbumInfo, ImportInfo, ProjectInfo
 from .exifinfo import ExifInfo
 from .exiftool import ExifToolCaching, get_exiftool_path
 from .momentinfo import MomentInfo
 from .personinfo import FaceInfo, PersonInfo
 from .photoexporter import ExportOptions, PhotoExporter
+from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate, RenderOptions
 from .placeinfo import PlaceInfo4, PlaceInfo5
 from .query_builder import get_query
 from .scoreinfo import ScoreInfo
 from .searchinfo import SearchInfo
-from .text_detection import detect_text
 from .uti import get_preferred_uti_extension, get_uti_for_extension
-from .utils import _get_resource_loc, hexdigest, list_directory
+from .utils import _get_resource_loc, assert_macos, is_macos, hexdigest, list_directory
+
+if is_macos:
+    from osxmetadata import OSXMetaData
+    from .text_detection import detect_text
 
 __all__ = ["PhotoInfo", "PhotoInfoNone", "frozen_photoinfo_factory"]
 
 logger = logging.getLogger("osxphotos")
 
 
 class PhotoInfo:
@@ -1456,14 +1459,16 @@
                 for text, confidence in detected_text
                 if confidence >= confidence_threshold
             ]
             return self._detected_text_cache[confidence_threshold]
 
     def _detected_text(self):
         """detect text in photo, either from cached extended attribute or by attempting text detection"""
+        assert_macos()
+
         path = (
             self.path_edited if self.hasadjustments and self.path_edited else self.path
         )
         path = path or self.path_derivatives[0] if self.path_derivatives else None
         if not path:
             return []
 
@@ -1889,14 +1894,18 @@
             # but do not sort certain items like location
             if k in ["location"]:
                 continue
             if v and isinstance(v, (list, tuple)) and not isinstance(v[0], dict):
                 dict_data[k] = sorted(v, key=lambda v: v if v is not None else "")
         return json.dumps(dict_data, sort_keys=True, default=default, indent=indent)
 
+    def tables(self) -> PhotoTables:
+        """Return PhotoTables object to provide access database tables associated with this photo (Photos 5+)"""
+        return None if self._db._photos_ver < 5 else PhotoTables(self)
+
     def _json_hexdigest(self):
         """JSON for use by hexdigest()"""
 
         # This differs from json() because hexdigest must not change if metadata changed
         # With json(), sort order of lists of dicts is not consistent but these aren't needed
         # for computing hexdigest so we can ignore them
         # also don't use visible because it changes based on Photos UI state
```

### Comparing `osxphotos-0.59.3/osxphotos/photokit.py` & `osxphotos-0.60.0/osxphotos/photokit.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 # TODO:
 # BUG: LivePhotoAsset.export always exports edited version if Live Photo has been edited, even if other version requested
 # add original=False to export instead of version= (and maybe others like path())
 # make burst/live methods get uuid from self instead of passing as arg
 
 import copy
 import pathlib
+import sys
 import threading
 import time
 
+assert sys.platform == "darwin"
+
 import AVFoundation
 import CoreServices
 import Foundation
 import objc
 import Photos
 import Quartz
 from Foundation import NSNotificationCenter, NSObject
@@ -80,14 +83,15 @@
 
 # notification that gets sent to Notification Center
 PHOTOKIT_NOTIFICATION_FINISHED_REQUEST = "PyPhotoKitNotificationFinishedRequest"
 
 # minimum amount to sleep while waiting for export
 MIN_SLEEP = 0.015
 
+
 ### utility functions
 def NSURL_to_path(url):
     """Convert URL string as represented by NSURL to a path string"""
     nsurl = Foundation.NSURL.alloc().initWithString_(
         Foundation.NSString.alloc().initWithString_(str(url))
     )
     path = nsurl.fileSystemRepresentation().decode("utf-8")
@@ -622,15 +626,16 @@
                 Photos.PHImageRequestOptionsDeliveryModeHighQualityFormat
             )
             requestdata = ImageData()
             event = threading.Event()
 
             def handler(imageData, dataUTI, orientation, info):
                 """result handler for requestImageDataAndOrientationForAsset_options_resultHandler_
-                all returned by the request is set as properties of nonlocal data (Fetchdata object)"""
+                all returned by the request is set as properties of nonlocal data (Fetchdata object)
+                """
 
                 nonlocal requestdata
 
                 options = {Quartz.kCGImageSourceShouldCache: Foundation.kCFBooleanFalse}
                 imgSrc = Quartz.CGImageSourceCreateWithData(imageData, options)
                 requestdata.metadata = Quartz.CGImageSourceCopyPropertiesAtIndex(
                     imgSrc, 0, options
@@ -669,15 +674,16 @@
             options.setNetworkAccessAllowed_(True)
 
             requestdata = PHAssetResourceData()
             event = threading.Event()
 
             def handler(data):
                 """result handler for requestImageDataAndOrientationForAsset_options_resultHandler_
-                all returned by the request is set as properties of nonlocal data (Fetchdata object)"""
+                all returned by the request is set as properties of nonlocal data (Fetchdata object)
+                """
 
                 nonlocal requestdata
 
                 requestdata.data += data
 
             def completion_handler(error):
                 if error:
@@ -706,15 +712,16 @@
         Following call to requestImageDataAndOrientationForAsset_options_resultHandler_,
         data will hold data from the fetch"""
 
         event = threading.Event()
 
         def handler(imageData, dataUTI, orientation, info):
             """result handler for requestImageDataAndOrientationForAsset_options_resultHandler_
-            all returned by the request is set as properties of nonlocal data (Fetchdata object)"""
+            all returned by the request is set as properties of nonlocal data (Fetchdata object)
+            """
 
             nonlocal data
 
             options = {Quartz.kCGImageSourceShouldCache: Foundation.kCFBooleanFalse}
             imgSrc = Quartz.CGImageSourceCreateWithData(imageData, options)
             data.metadata = Quartz.CGImageSourceCopyPropertiesAtIndex(
                 imgSrc, 0, options
```

### Comparing `osxphotos-0.59.3/osxphotos/photosalbum.py` & `osxphotos-0.60.0/osxphotos/photosalbum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """ PhotosAlbum class to create an album in default Photos library and add photos to it """
 
 from typing import List, Optional
 
-import photoscript
 from more_itertools import chunked
-from photoscript import Album, Folder, Photo, PhotosLibrary
 
 from .photoinfo import PhotoInfo
-from .utils import noop, pluralize
+from .utils import assert_macos, noop, pluralize
+
+assert_macos()
+
+import photoscript
+from photoscript import Album, Folder, Photo, PhotosLibrary
 
 __all__ = ["PhotosAlbum", "PhotosAlbumPhotoScript"]
 
 
 def folder_by_path(folders: List[str], verbose: Optional[callable] = None) -> Folder:
     """Get (and create if necessary) a Photos Folder by path (passed as list of folder names)"""
     library = PhotosLibrary()
```

### Comparing `osxphotos-0.59.3/osxphotos/photoscript_utils.py` & `osxphotos-0.60.0/osxphotos/photoscript_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Utilities for creating photoscript objects from a name or UUID"""
 
 from __future__ import annotations
 
 import sqlite3
 
+from .utils import assert_macos
+
+assert_macos()
+
 import photoscript
 
 from ._constants import _DB_TABLE_NAMES, _PHOTOS_5_ALBUM_KIND, _PHOTOS_5_FOLDER_KIND
 from .photosdb.photosdb_utils import get_db_path_for_library, get_photos_library_version
 from .sqlite_utils import sqlite_open_ro
```

### Comparing `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,17 @@
         face["mouthx"] = row[29]
         face["mouthy"] = row[30]
         face["quality"] = row[32]
         face["righteyex"] = row[33]
         face["righteyey"] = row[34]
         face["roll"] = row[35]
         face["size"] = row[36]
-        face["yaw"] = 0 # Photos 4 only (this is in Photos 5-7, but dropped in Ventura so just don't support it)
+        face[
+            "yaw"
+        ] = 0  # Photos 4 only (this is in Photos 5-7, but dropped in Ventura so just don't support it)
         face["pitch"] = 0  # not defined in Photos 5
 
         photosdb._db_faceinfo_pk[pk] = face
 
         try:
             photosdb._db_faceinfo_uuid[asset_uuid].append(pk)
         except KeyError:
```

### Comparing `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.0/osxphotos/photosdb/photosdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from collections import OrderedDict
 from collections.abc import Iterable
 from datetime import datetime, timedelta, timezone
 from typing import Any, List, Optional
 from unicodedata import normalize
 
 import bitmath
-import photoscript
 from rich import print
 
 from .._constants import (
     _DB_TABLE_NAMES,
     _MOVIE_TYPE,
     _PHOTO_TYPE,
     _PHOTOS_3_VERSION,
@@ -58,21 +57,25 @@
 from ..photoinfo import PhotoInfo
 from ..phototemplate import RenderOptions
 from ..queryoptions import QueryOptions
 from ..rich_utils import add_rich_markup_tag
 from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
 from ..utils import (
     _check_file_exists,
+    is_macos,
     get_macos_version,
     get_last_library_path,
     noop,
     normalize_unicode,
 )
 from .photosdb_utils import get_db_model_version, get_db_version
 
+if is_macos:
+    import photoscript
+
 logger = logging.getLogger("osxphotos")
 
 __all__ = ["PhotosDB"]
 
 # TODO: Add test for imageTimeZoneOffsetSeconds = None
 # TODO: Add test for __str__
 # TODO: Add special albums and magic albums
@@ -114,16 +117,16 @@
         Raises:
             FileNotFoundError if dbfile is not a valid Photos library.
             TypeError if verbose is not None and not callable.
         """
 
         # Check OS version
         system = platform.system()
-        (ver, major, _) = get_macos_version()
-        if system != "Darwin" or ((ver, major) not in _TESTED_OS_VERSIONS):
+        (ver, major, _) = get_macos_version() if is_macos else (None, None, None)
+        if system == "Darwin" and ((ver, major) not in _TESTED_OS_VERSIONS):
             logging.warning(
                 f"WARNING: This module has only been tested with macOS versions "
                 f"[{', '.join(f'{v}.{m}' for (v, m) in _TESTED_OS_VERSIONS)}]: "
                 f"you have {system}, OS version: {ver}.{major}"
             )
 
         if verbose is None:
```

### Comparing `osxphotos-0.59.3/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.0/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.0/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/phototemplate.md` & `osxphotos-0.60.0/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/phototemplate.py` & `osxphotos-0.60.0/osxphotos/phototemplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import osxphotos.template_counter as counter
 
 from ._constants import _UNKNOWN_PERSON, TEXT_DETECTION_CONFIDENCE_THRESHOLD
 from ._version import __version__
 from .datetime_formatter import DateTimeFormatter
 from .exiftool import ExifToolCaching
 from .path_utils import sanitize_dirname, sanitize_filename, sanitize_pathpart
-from .text_detection import detect_text
 from .utils import expand_and_validate_filepath, load_function, uuid_to_shortuuid
 
 __all__ = [
     "RenderOptions",
     "PhotoTemplateParser",
     "PhotoTemplate",
     "parse_default_kv",
```

### Comparing `osxphotos-0.59.3/osxphotos/phototemplate.tx` & `osxphotos-0.60.0/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/phototz.py` & `osxphotos-0.60.0/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/placeinfo.py` & `osxphotos-0.60.0/osxphotos/placeinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         "field15",
         "field16",
         "street_address",  # throughfare, The street address associated with the placemark.
         "body_of_water",  # RKPlace.type == 44, appears to be any body of water (ocean or inland)
     ],
 )
 
+
 # The following classes represent Photo Library Reverse Geolocation Info as stored
 # in ZADDITIONALASSETATTRIBUTES.ZREVERSELOCATIONDATA
 # These classes are used by bpylist.archiver to unarchive the serialized objects
 class PLRevGeoLocationInfo:
     """The top level reverse geolocation object"""
 
     def __init__(
```

### Comparing `osxphotos-0.59.3/osxphotos/pyrepl.py` & `osxphotos-0.60.0/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.0/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/query_builder.py` & `osxphotos-0.60.0/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/queryoptions.py` & `osxphotos-0.60.0/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/scoreinfo.py` & `osxphotos-0.60.0/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/searchinfo.py` & `osxphotos-0.60.0/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/sqlgrep.py` & `osxphotos-0.60.0/osxphotos/sqlgrep.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     Returns:
         Generator which yields list of [table, column, row_id, value]
     """
     flags = re.IGNORECASE if ignore_case else 0
     try:
         with sqlite3.connect(f"file:{filename}?mode=ro", uri=True) as conn:
-            regex = re.compile(f'({pattern})', flags=flags)
+            regex = re.compile(f"({pattern})", flags=flags)
             filename_header = f"{filename}: " if print_filename else ""
             conn.row_factory = sqlite3.Row
             cursor = conn.cursor()
             cursor.execute("SELECT name FROM sqlite_master WHERE type='table'")
             for tablerow in cursor.fetchall():
                 table = tablerow[0]
                 cursor.execute("SELECT * FROM {t}".format(t=table))
```

### Comparing `osxphotos-0.59.3/osxphotos/sqlite_utils.py` & `osxphotos-0.60.0/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.0/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/template_counter.py` & `osxphotos-0.60.0/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.0/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.0/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/text_detection.py` & `osxphotos-0.60.0/osxphotos/text_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """ Use Apple's Vision Framework via PyObjC to perform text detection on images (macOS 10.15+ only) """
 
 import logging
+import sys
 from typing import List, Optional
 
+from .utils import assert_macos, get_macos_version
+
+assert_macos()
+
 import objc
 import Quartz
 from Cocoa import NSURL
 from Foundation import NSDictionary
 
 # needed to capture system-level stderr
 from wurlitzer import pipes
 
-from .utils import get_macos_version
-
 __all__ = ["detect_text", "make_request_handler"]
 
 ver, major, minor = get_macos_version()
 if ver == "10" and int(major) < 15:
     vision = False
 else:
     import Vision
```

### Comparing `osxphotos-0.59.3/osxphotos/timeutils.py` & `osxphotos-0.60.0/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/tutorial.md` & `osxphotos-0.60.0/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/osxphotos/uti.py` & `osxphotos-0.60.0/osxphotos/uti.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """ get UTI for a given file extension and the preferred extension for a given UTI
 
-Implementation note: runs only on macOS
-
     On macOS <= 11 (Big Sur), uses objective C CoreServices methods 
     UTTypeCopyPreferredTagWithClass and UTTypeCreatePreferredIdentifierForTag to retrieve the 
     UTI and the extension.  These are deprecated in 10.15 (Catalina) and no longer supported on Monterey.
 
     On Monterey, these calls are replaced with Swift methods that I can't call from python so 
     this code uses a cached dict of UTI values.  The code first checks to see if the extension or UTI 
     is available in the cache and if so, returns it. If not, it performs a subprocess call to `mdls` to 
     retrieve the UTI (by creating a temp file with the correct extension) and returns the UTI.  This only 
     works for the extension -> UTI lookup. On Monterey, if there is no cached value for UTI -> extension lookup, 
     returns None.
 
+    Outside of macOS uses only the hardcoded list of UTIs.
+
     It's a bit hacky but best I can think of to make this robust on different versions of macOS.  PRs welcome.
 """
 
 from __future__ import annotations
 
 import csv
 import re
 import subprocess
+import sys
 import tempfile
 
-import CoreServices
-import objc
+from .utils import assert_macos, is_macos, get_macos_version
 
-from .utils import get_macos_version
+if is_macos:
+    import CoreServices
+    import objc
 
 __all__ = ["get_preferred_uti_extension", "get_uti_for_extension"]
 
 # cached values of all the UTIs (< 6 chars long) known to my Mac running macOS 10.15.7
 UTI_CSV = """extension,UTI,preferred_extension,MIME_type
 c,public.c-source,c,None
 f,public.fortran-source,f,None
@@ -518,24 +520,29 @@
         EXT_UTI_DICT[row["extension"]] = row["UTI"]
         UTI_EXT_DICT[row["UTI"]] = row["preferred_extension"]
 
 
 _load_uti_dict()
 
 # OS version for determining which methods can be used
-OS_VER, OS_MAJOR, _ = (int(x) for x in get_macos_version())
+OS_VER, OS_MAJOR, _ = (
+    (int(x) for x in get_macos_version()) if is_macos else (None, None, None)
+)
 
 
 def _get_uti_from_mdls(extension):
     """use mdls to get the UTI for a given extension on systems that don't support UTTypeCreatePreferredIdentifierForTag
     Returns: UTI or None if UTI cannot be determined"""
 
     # mdls -name kMDItemContentType foo.3fr
     # kMDItemContentType = "com.hasselblad.3fr-raw-image"
 
+    if not is_macos:
+        return None
+
     try:
         with tempfile.NamedTemporaryFile(suffix="." + extension) as temp:
             output = subprocess.check_output(
                 [
                     "/usr/bin/mdls",
                     "-name",
                     "kMDItemContentType",
@@ -569,15 +576,15 @@
 
 
 def get_preferred_uti_extension(uti: str) -> str | None:
     """get preferred extension for a UTI type
     uti: UTI str, e.g. 'public.jpeg'
     returns: preferred extension as str or None if cannot be determined"""
 
-    if (OS_VER, OS_MAJOR) <= (10, 16):
+    if is_macos and (OS_VER, OS_MAJOR) <= (10, 16):
         # reference: https://developer.apple.com/documentation/coreservices/1442744-uttypecopypreferredtagwithclass?language=objc
         # deprecated in Catalina+, likely won't work at all on macOS 12
         with objc.autorelease_pool():
             extension = CoreServices.UTTypeCopyPreferredTagWithClass(
                 uti, CoreServices.kUTTagClassFilenameExtension
             )
             if extension:
@@ -598,15 +605,15 @@
     if not extension:
         return None
 
     # accepts extension with or without leading 0
     if extension[0] == ".":
         extension = extension[1:]
 
-    if (OS_VER, OS_MAJOR) <= (10, 16):
+    if is_macos and (OS_VER, OS_MAJOR) <= (10, 16):
         # https://developer.apple.com/documentation/coreservices/1448939-uttypecreatepreferredidentifierf
         with objc.autorelease_pool():
             uti = CoreServices.UTTypeCreatePreferredIdentifierForTag(
                 CoreServices.kUTTagClassFilenameExtension, extension, None
             )
             if uti:
                 return uti
```

### Comparing `osxphotos-0.59.3/osxphotos/utils.py` & `osxphotos-0.60.0/osxphotos/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 import platform
 import re
 import subprocess
 import sys
 import unicodedata
 import urllib.parse
 from plistlib import load as plistload
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Any, Callable, List, Optional, Tuple, TypeVar, Union
 from uuid import UUID
 
-import CoreFoundation
 import requests
 import shortuuid
 
 from ._constants import UNICODE_FORMAT
 
 logger = logging.getLogger("osxphotos")
 
 __all__ = [
+    "is_macos",
+    "assert_macos",
     "dd_to_dms_str",
     "expand_and_validate_filepath",
     "get_last_library_path",
     "get_macos_version",
     "get_system_library_path",
     "hexdigest",
     "increment_filename_with_count",
@@ -49,28 +50,40 @@
     "uuid_to_shortuuid",
 ]
 
 
 VERSION_INFO_URL = "https://pypi.org/pypi/osxphotos/json"
 
 
+is_macos = sys.platform == "darwin"
+
+
+def assert_macos():
+    assert is_macos, "This feature only runs on macOS"
+
+
+if is_macos:
+    import CoreFoundation
+
+
 def noop(*args, **kwargs):
     """do nothing (no operation)"""
     pass
 
 
 def lineno(filename):
     """Returns string with filename and current line number in caller as '(filename): line_num'
     Will trim filename to just the name, dropping path, if any."""
     line = inspect.currentframe().f_back.f_lineno
     filename = pathlib.Path(filename).name
     return f"{filename}: {line}"
 
 
 def get_macos_version():
+    assert_macos()
     # returns tuple of str containing OS version
     # e.g. 10.13.6 = ("10", "13", "6")
     version = platform.mac_ver()[0].split(".")
     if len(version) == 2:
         (ver, major) = version
         minor = "0"
     elif len(version) == 3:
@@ -162,14 +175,16 @@
     return lat_str, lon_str
 
 
 def get_system_library_path():
     """return the path to the system Photos library as string"""
     """ only works on MacOS 10.15 """
     """ on earlier versions, returns None """
+    if not is_macos:
+        return None
     _, major, _ = get_macos_version()
     if int(major) < 15:
         logger.debug(
             f"get_system_library_path not implemented for MacOS < 10.15: you have {major}"
         )
         return None
 
@@ -237,14 +252,16 @@
         logger.debug("Could not get path to Photos database")
         return None
 
 
 def list_photo_libraries():
     """returns list of Photos libraries found on the system"""
     """ on MacOS < 10.15, this may omit some libraries """
+    if not is_macos:
+        return []
 
     # On 10.15, mdfind appears to find all libraries
     # On older MacOS versions, mdfind appears to ignore some libraries
     # glob to find libraries in ~/Pictures then mdfind to find all the others
     # TODO: make this more robust
     lib_list = list_directory(
         f"{pathlib.Path.home()}/Pictures/", glob="*.photoslibrary"
@@ -259,19 +276,24 @@
     ).splitlines()
     for lib in output:
         lib_list.append(lib.decode("utf-8"))
     lib_list = sorted(set(lib_list))
     return lib_list
 
 
-def normalize_fs_path(path: str) -> str:
+T = TypeVar("T", bound=Union[str, pathlib.Path])
+
+
+def normalize_fs_path(path: T) -> T:
     """Normalize filesystem paths with unicode in them"""
-    # macOS HFS+ uses NFD, APFS doesn't normalize but stick with NFD
-    # ref: https://eclecticlight.co/2021/05/08/explainer-unicode-normalization-and-apfs/
-    return unicodedata.normalize("NFD", path)
+    form = "NFD" if is_macos else "NFC"
+    if isinstance(path, pathlib.Path):
+        return pathlib.Path(unicodedata.normalize(form, str(path)))
+    else:
+        return unicodedata.normalize(form, path)
 
 
 # def findfiles(pattern, path):
 #     """Returns list of filenames from path matched by pattern
 #     shell pattern. Matching is case-insensitive.
 #     If 'path_' is invalid/doesn't exist, returns []."""
 #     if not os.path.isdir(path):
@@ -352,15 +374,15 @@
         files = [os.path.join(directory, f) for f in files]
     if is_pathlib:
         files = [pathlib.Path(f) for f in files]
 
     return files
 
 
-def normalize_unicode(value):
+def normalize_unicode(value) -> Any:
     """normalize unicode data"""
     if value is None:
         return None
     if isinstance(value, (tuple, list)):
         return tuple(unicodedata.normalize(UNICODE_FORMAT, v) for v in value)
     elif isinstance(value, str):
         return unicodedata.normalize(UNICODE_FORMAT, value)
```

### Comparing `osxphotos-0.59.3/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.0/osxphotos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.59.3
+Version: 0.60.0
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.59.3/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.0/osxphotos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 osxphotos/personinfo.py
 osxphotos/photodates.py
 osxphotos/photoexporter.py
 osxphotos/photoinfo.py
 osxphotos/photokit.py
 osxphotos/photosalbum.py
 osxphotos/photoscript_utils.py
+osxphotos/phototables.py
 osxphotos/phototemplate.cog.md
 osxphotos/phototemplate.md
 osxphotos/phototemplate.py
 osxphotos/phototemplate.tx
 osxphotos/phototz.py
 osxphotos/placeinfo.py
 osxphotos/pyrepl.py
```

### Comparing `osxphotos-0.59.3/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.0/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/setup.py` & `osxphotos-0.60.0/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_10_12_6.py` & `osxphotos-0.60.0/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.0/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.0/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.0/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.0/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.0/tests/test_catalina_10_15_7.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from collections import Counter, namedtuple
 
 import pytest
 
 import osxphotos
 from osxphotos._constants import _UNKNOWN_PERSON
 from osxphotos.photoexporter import PhotoExporter
-from osxphotos.utils import get_macos_version
+from osxphotos.utils import is_macos, get_macos_version
 
-OS_VERSION = get_macos_version()
+OS_VERSION = get_macos_version() if is_macos else (None, None, None)
 SKIP_TEST = "OSXPHOTOS_TEST_EXPORT" not in os.environ or OS_VERSION[1] != "15"
 PHOTOS_DB_LOCAL = os.path.expanduser("~/Pictures/Photos Library.photoslibrary")
 
 PHOTOS_DB = "tests/Test-10.15.7.photoslibrary/database/photos.db"
 PHOTOS_DB_PATH = "/Test-10.15.7.photoslibrary/database/photos.db"
 PHOTOS_LIBRARY_PATH = "/Test-10.15.7.photoslibrary"
 
@@ -1444,14 +1444,15 @@
 def test_multi_uuid(photosdb):
     """test photos() with multiple uuids"""
     photos = photosdb.photos(uuid=[UUID_DICT["favorite"], UUID_DICT["not_favorite"]])
 
     assert len(photos) == 2
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_detected_text(photosdb):
     """test PhotoInfo.detected_text"""
     for uuid, expected_text in UUID_DETECTED_TEXT.items():
         photo = photosdb.get_photo(uuid=uuid)
         detected_text = " ".join(text for text, conf in photo.detected_text())
         if expected_text is not None:
             assert expected_text in detected_text
```

### Comparing `osxphotos-0.59.3/tests/test_cli.py` & `osxphotos-0.60.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import re
 import shutil
 import sqlite3
 import subprocess
 import tempfile
 import time
 from tempfile import TemporaryDirectory
+from bitmath import contextlib
 
 import pytest
 from click.testing import CliRunner
-from osxmetadata import OSXMetaData, Tag
 
 import osxphotos
 from osxphotos._constants import OSXPHOTOS_EXPORT_DB
 from osxphotos._version import __version__
 from osxphotos.cli import (
     about,
     albums,
@@ -32,17 +32,27 @@
     labels,
     persons,
     places,
     query,
 )
 from osxphotos.exiftool import ExifTool, get_exiftool_path
 from osxphotos.fileutil import FileUtil
-from osxphotos.utils import noop, normalize_fs_path, normalize_unicode
+from osxphotos.utils import is_macos, noop, normalize_fs_path, normalize_unicode
+
+if is_macos:
+    from osxmetadata import OSXMetaData, Tag
 
 from .conftest import copy_photos_library_to_path
+from .locale_util import setlocale
+
+
+def _normalize_fs_paths(paths):
+    """Small helper to prepare path strings for test"""
+    return [normalize_fs_path(p) for p in paths]
+
 
 CLI_PHOTOS_DB = "tests/Test-10.15.7.photoslibrary"
 LIVE_PHOTOS_DB = "tests/Test-Cloud-10.15.1.photoslibrary"
 RAW_PHOTOS_DB = "tests/Test-RAW-10.15.1.photoslibrary"
 COMMENTS_PHOTOS_DB = "tests/Test-Cloud-10.15.6.photoslibrary"
 PLACES_PHOTOS_DB = "tests/Test-Places-Catalina-10_15_1.photoslibrary"
 PLACES_PHOTOS_DB_13 = "tests/Test-Places-High-Sierra-10.13.6.photoslibrary"
@@ -62,237 +72,255 @@
 UUID_DOWNLOAD_MISSING = "C6C712C5-9316-408D-A3C3-125661422DA9"  # IMG_8844.JPG
 
 UUID_FILE = "tests/uuid_from_file.txt"
 SKIP_UUID_FILE = "tests/skip_uuid_from_file.txt"
 
 CLI_OUTPUT_QUERY_UUID = '[{"uuid": "D79B8D77-BFFC-460B-9312-034F2877D35B", "filename": "D79B8D77-BFFC-460B-9312-034F2877D35B.jpeg", "original_filename": "Pumkins2.jpg", "date": "2018-09-28T16:07:07-04:00", "description": "Girl holding pumpkin", "title": "I found one!", "keywords": ["Kids"], "albums": ["Pumpkin Farm", "Test Album", "Multi Keyword"], "persons": ["Katie"], "path": "/tests/Test-10.15.7.photoslibrary/originals/D/D79B8D77-BFFC-460B-9312-034F2877D35B.jpeg", "ismissing": false, "hasadjustments": false, "external_edit": false, "favorite": false, "hidden": false, "latitude": 41.256566, "longitude": -95.940257, "path_edited": null, "shared": false, "isphoto": true, "ismovie": false, "uti": "public.jpeg", "burst": false, "live_photo": false, "path_live_photo": null, "iscloudasset": false, "incloud": null}]'
 
-CLI_EXPORT_FILENAMES = [
-    "[2020-08-29] AAF035 (1).jpg",
-    "[2020-08-29] AAF035 (2).jpg",
-    "[2020-08-29] AAF035 (3).jpg",
-    "[2020-08-29] AAF035.jpg",
-    "DSC03584.dng",
-    "Frítest (1).jpg",
-    "Frítest (2).jpg",
-    "Frítest (3).jpg",
-    "Frítest_edited (1).jpeg",
-    "Frítest_edited.jpeg",
-    "Frítest.jpg",
-    "IMG_1693.tif",
-    "IMG_1994.cr2",
-    "IMG_1994.JPG",
-    "IMG_1997.cr2",
-    "IMG_1997.JPG",
-    "IMG_3092_edited.jpeg",
-    "IMG_3092.heic",
-    "IMG_4547.jpg",
-    "Jellyfish.MOV",
-    "Jellyfish1.mp4",
-    "Pumkins1.jpg",
-    "Pumkins2.jpg",
-    "Pumpkins3.jpg",
-    "screenshot-really-a-png.jpeg",
-    "St James Park_edited.jpeg",
-    "St James Park.jpg",
-    "Tulips_edited.jpeg",
-    "Tulips.jpg",
-    "wedding_edited.jpeg",
-    "wedding.jpg",
-    "winebottle (1).jpeg",
-    "winebottle.jpeg",
-]
+CLI_EXPORT_FILENAMES = _normalize_fs_paths(
+    [
+        "[2020-08-29] AAF035 (1).jpg",
+        "[2020-08-29] AAF035 (2).jpg",
+        "[2020-08-29] AAF035 (3).jpg",
+        "[2020-08-29] AAF035.jpg",
+        "DSC03584.dng",
+        "Frítest (1).jpg",
+        "Frítest (2).jpg",
+        "Frítest (3).jpg",
+        "Frítest_edited (1).jpeg",
+        "Frítest_edited.jpeg",
+        "Frítest.jpg",
+        "IMG_1693.tif",
+        "IMG_1994.cr2",
+        "IMG_1994.JPG",
+        "IMG_1997.cr2",
+        "IMG_1997.JPG",
+        "IMG_3092_edited.jpeg",
+        "IMG_3092.heic",
+        "IMG_4547.jpg",
+        "Jellyfish.MOV",
+        "Jellyfish1.mp4",
+        "Pumkins1.jpg",
+        "Pumkins2.jpg",
+        "Pumpkins3.jpg",
+        "screenshot-really-a-png.jpeg",
+        "St James Park_edited.jpeg",
+        "St James Park.jpg",
+        "Tulips_edited.jpeg",
+        "Tulips.jpg",
+        "wedding_edited.jpeg",
+        "wedding.jpg",
+        "winebottle (1).jpeg",
+        "winebottle.jpeg",
+    ]
+)
 
 
-CLI_EXPORT_FILENAMES_DRY_RUN = [
-    "[2020-08-29] AAF035.jpg",
-    "DSC03584.dng",
-    "Frítest_edited.jpeg",
-    "Frítest.jpg",
-    "IMG_1693.tif",
-    "IMG_1994.cr2",
-    "IMG_1994.JPG",
-    "IMG_1997.cr2",
-    "IMG_1997.JPG",
-    "IMG_3092_edited.jpeg",
-    "IMG_3092.heic",
-    "IMG_4547.jpg",
-    "Jellyfish.MOV",
-    "Jellyfish1.mp4",
-    "Pumkins1.jpg",
-    "Pumkins2.jpg",
-    "Pumpkins3.jpg",
-    "screenshot-really-a-png.jpeg",
-    "St James Park_edited.jpeg",
-    "St James Park.jpg",
-    "Tulips_edited.jpeg",
-    "Tulips.jpg",
-    "wedding_edited.jpeg",
-    "wedding.jpg",
-    "winebottle.jpeg",
-    "winebottle.jpeg",
-]
+CLI_EXPORT_FILENAMES_DRY_RUN = _normalize_fs_paths(
+    [
+        "[2020-08-29] AAF035.jpg",
+        "DSC03584.dng",
+        "Frítest_edited.jpeg",
+        "Frítest.jpg",
+        "IMG_1693.tif",
+        "IMG_1994.cr2",
+        "IMG_1994.JPG",
+        "IMG_1997.cr2",
+        "IMG_1997.JPG",
+        "IMG_3092_edited.jpeg",
+        "IMG_3092.heic",
+        "IMG_4547.jpg",
+        "Jellyfish.MOV",
+        "Jellyfish1.mp4",
+        "Pumkins1.jpg",
+        "Pumkins2.jpg",
+        "Pumpkins3.jpg",
+        "screenshot-really-a-png.jpeg",
+        "St James Park_edited.jpeg",
+        "St James Park.jpg",
+        "Tulips_edited.jpeg",
+        "Tulips.jpg",
+        "wedding_edited.jpeg",
+        "wedding.jpg",
+        "winebottle.jpeg",
+        "winebottle.jpeg",
+    ]
+)
 
-CLI_EXPORT_IGNORE_SIGNATURE_FILENAMES = ["Tulips.jpg", "wedding.jpg"]
+CLI_EXPORT_IGNORE_SIGNATURE_FILENAMES = _normalize_fs_paths(
+    ["Tulips.jpg", "wedding.jpg"]
+)
 
-CLI_EXPORT_FILENAMES_ALBUM = ["Pumkins1.jpg", "Pumkins2.jpg", "Pumpkins3.jpg"]
+CLI_EXPORT_FILENAMES_ALBUM = _normalize_fs_paths(
+    ["Pumkins1.jpg", "Pumkins2.jpg", "Pumpkins3.jpg"]
+)
 
-CLI_EXPORT_FILENAMES_ALBUM_UNICODE = ["IMG_4547.jpg"]
+CLI_EXPORT_FILENAMES_ALBUM_UNICODE = _normalize_fs_paths(["IMG_4547.jpg"])
 
-CLI_EXPORT_FILENAMES_DELETED_TWIN = ["wedding.jpg", "wedding_edited.jpeg"]
+CLI_EXPORT_FILENAMES_DELETED_TWIN = _normalize_fs_paths(
+    ["wedding.jpg", "wedding_edited.jpeg"]
+)
 
 CLI_EXPORT_EDITED_SUFFIX = "_bearbeiten"
 CLI_EXPORT_EDITED_SUFFIX_TEMPLATE = "{edited?_edited,}"
 CLI_EXPORT_ORIGINAL_SUFFIX = "_original"
 CLI_EXPORT_ORIGINAL_SUFFIX_TEMPLATE = "{edited?_original,}"
 CLI_EXPORT_PREVIEW_SUFFIX = "_lowres"
 
-CLI_EXPORT_FILENAMES_EDITED_SUFFIX = [
-    "[2020-08-29] AAF035 (1).jpg",
-    "[2020-08-29] AAF035 (2).jpg",
-    "[2020-08-29] AAF035 (3).jpg",
-    "[2020-08-29] AAF035.jpg",
-    "DSC03584.dng",
-    "Frítest (1).jpg",
-    "Frítest (2).jpg",
-    "Frítest (3).jpg",
-    "Frítest_bearbeiten (1).jpeg",
-    "Frítest_bearbeiten.jpeg",
-    "Frítest.jpg",
-    "IMG_1693.tif",
-    "IMG_1994.cr2",
-    "IMG_1994.JPG",
-    "IMG_1997.cr2",
-    "IMG_1997.JPG",
-    "IMG_3092_bearbeiten.jpeg",
-    "IMG_3092.heic",
-    "IMG_4547.jpg",
-    "Jellyfish.MOV",
-    "Jellyfish1.mp4",
-    "Pumkins1.jpg",
-    "Pumkins2.jpg",
-    "Pumpkins3.jpg",
-    "screenshot-really-a-png.jpeg",
-    "St James Park_bearbeiten.jpeg",
-    "St James Park.jpg",
-    "Tulips_bearbeiten.jpeg",
-    "Tulips.jpg",
-    "wedding_bearbeiten.jpeg",
-    "wedding.jpg",
-    "winebottle (1).jpeg",
-    "winebottle.jpeg",
-]
+CLI_EXPORT_FILENAMES_EDITED_SUFFIX = _normalize_fs_paths(
+    [
+        "[2020-08-29] AAF035 (1).jpg",
+        "[2020-08-29] AAF035 (2).jpg",
+        "[2020-08-29] AAF035 (3).jpg",
+        "[2020-08-29] AAF035.jpg",
+        "DSC03584.dng",
+        "Frítest (1).jpg",
+        "Frítest (2).jpg",
+        "Frítest (3).jpg",
+        "Frítest_bearbeiten (1).jpeg",
+        "Frítest_bearbeiten.jpeg",
+        "Frítest.jpg",
+        "IMG_1693.tif",
+        "IMG_1994.cr2",
+        "IMG_1994.JPG",
+        "IMG_1997.cr2",
+        "IMG_1997.JPG",
+        "IMG_3092_bearbeiten.jpeg",
+        "IMG_3092.heic",
+        "IMG_4547.jpg",
+        "Jellyfish.MOV",
+        "Jellyfish1.mp4",
+        "Pumkins1.jpg",
+        "Pumkins2.jpg",
+        "Pumpkins3.jpg",
+        "screenshot-really-a-png.jpeg",
+        "St James Park_bearbeiten.jpeg",
+        "St James Park.jpg",
+        "Tulips_bearbeiten.jpeg",
+        "Tulips.jpg",
+        "wedding_bearbeiten.jpeg",
+        "wedding.jpg",
+        "winebottle (1).jpeg",
+        "winebottle.jpeg",
+    ]
+)
 
-CLI_EXPORT_FILENAMES_EDITED_SUFFIX_TEMPLATE = [
-    "[2020-08-29] AAF035 (1).jpg",
-    "[2020-08-29] AAF035 (2).jpg",
-    "[2020-08-29] AAF035 (3).jpg",
-    "[2020-08-29] AAF035.jpg",
-    "DSC03584.dng",
-    "Frítest (1).jpg",
-    "Frítest (2).jpg",
-    "Frítest (3).jpg",
-    "Frítest_edited (1).jpeg",
-    "Frítest_edited.jpeg",
-    "Frítest.jpg",
-    "IMG_1693.tif",
-    "IMG_1994.cr2",
-    "IMG_1994.JPG",
-    "IMG_1997.cr2",
-    "IMG_1997.JPG",
-    "IMG_3092_edited.jpeg",
-    "IMG_3092.heic",
-    "IMG_4547.jpg",
-    "Jellyfish.MOV",
-    "Jellyfish1.mp4",
-    "Pumkins1.jpg",
-    "Pumkins2.jpg",
-    "Pumpkins3.jpg",
-    "screenshot-really-a-png.jpeg",
-    "St James Park_edited.jpeg",
-    "St James Park.jpg",
-    "Tulips_edited.jpeg",
-    "Tulips.jpg",
-    "wedding_edited.jpeg",
-    "wedding.jpg",
-    "winebottle (1).jpeg",
-    "winebottle.jpeg",
-]
+CLI_EXPORT_FILENAMES_EDITED_SUFFIX_TEMPLATE = _normalize_fs_paths(
+    [
+        "[2020-08-29] AAF035 (1).jpg",
+        "[2020-08-29] AAF035 (2).jpg",
+        "[2020-08-29] AAF035 (3).jpg",
+        "[2020-08-29] AAF035.jpg",
+        "DSC03584.dng",
+        "Frítest (1).jpg",
+        "Frítest (2).jpg",
+        "Frítest (3).jpg",
+        "Frítest_edited (1).jpeg",
+        "Frítest_edited.jpeg",
+        "Frítest.jpg",
+        "IMG_1693.tif",
+        "IMG_1994.cr2",
+        "IMG_1994.JPG",
+        "IMG_1997.cr2",
+        "IMG_1997.JPG",
+        "IMG_3092_edited.jpeg",
+        "IMG_3092.heic",
+        "IMG_4547.jpg",
+        "Jellyfish.MOV",
+        "Jellyfish1.mp4",
+        "Pumkins1.jpg",
+        "Pumkins2.jpg",
+        "Pumpkins3.jpg",
+        "screenshot-really-a-png.jpeg",
+        "St James Park_edited.jpeg",
+        "St James Park.jpg",
+        "Tulips_edited.jpeg",
+        "Tulips.jpg",
+        "wedding_edited.jpeg",
+        "wedding.jpg",
+        "winebottle (1).jpeg",
+        "winebottle.jpeg",
+    ]
+)
 
-CLI_EXPORT_FILENAMES_ORIGINAL_SUFFIX = [
-    "[2020-08-29] AAF035_original (1).jpg",
-    "[2020-08-29] AAF035_original (2).jpg",
-    "[2020-08-29] AAF035_original (3).jpg",
-    "[2020-08-29] AAF035_original.jpg",
-    "DSC03584_original.dng",
-    "Frítest_edited (1).jpeg",
-    "Frítest_edited.jpeg",
-    "Frítest_original (1).jpg",
-    "Frítest_original (2).jpg",
-    "Frítest_original (3).jpg",
-    "Frítest_original.jpg",
-    "IMG_1693_original.tif",
-    "IMG_1994_original.cr2",
-    "IMG_1994_original.JPG",
-    "IMG_1997_original.cr2",
-    "IMG_1997_original.JPG",
-    "IMG_3092_edited.jpeg",
-    "IMG_3092_original.heic",
-    "IMG_4547_original.jpg",
-    "Jellyfish_original.MOV",
-    "Jellyfish1_original.mp4",
-    "Pumkins1_original.jpg",
-    "Pumkins2_original.jpg",
-    "Pumpkins3_original.jpg",
-    "screenshot-really-a-png_original.jpeg",
-    "St James Park_edited.jpeg",
-    "St James Park_original.jpg",
-    "Tulips_edited.jpeg",
-    "Tulips_original.jpg",
-    "wedding_edited.jpeg",
-    "wedding_original.jpg",
-    "winebottle_original (1).jpeg",
-    "winebottle_original.jpeg",
-]
+CLI_EXPORT_FILENAMES_ORIGINAL_SUFFIX = _normalize_fs_paths(
+    [
+        "[2020-08-29] AAF035_original (1).jpg",
+        "[2020-08-29] AAF035_original (2).jpg",
+        "[2020-08-29] AAF035_original (3).jpg",
+        "[2020-08-29] AAF035_original.jpg",
+        "DSC03584_original.dng",
+        "Frítest_edited (1).jpeg",
+        "Frítest_edited.jpeg",
+        "Frítest_original (1).jpg",
+        "Frítest_original (2).jpg",
+        "Frítest_original (3).jpg",
+        "Frítest_original.jpg",
+        "IMG_1693_original.tif",
+        "IMG_1994_original.cr2",
+        "IMG_1994_original.JPG",
+        "IMG_1997_original.cr2",
+        "IMG_1997_original.JPG",
+        "IMG_3092_edited.jpeg",
+        "IMG_3092_original.heic",
+        "IMG_4547_original.jpg",
+        "Jellyfish_original.MOV",
+        "Jellyfish1_original.mp4",
+        "Pumkins1_original.jpg",
+        "Pumkins2_original.jpg",
+        "Pumpkins3_original.jpg",
+        "screenshot-really-a-png_original.jpeg",
+        "St James Park_edited.jpeg",
+        "St James Park_original.jpg",
+        "Tulips_edited.jpeg",
+        "Tulips_original.jpg",
+        "wedding_edited.jpeg",
+        "wedding_original.jpg",
+        "winebottle_original (1).jpeg",
+        "winebottle_original.jpeg",
+    ]
+)
 
-CLI_EXPORT_FILENAMES_ORIGINAL_SUFFIX_TEMPLATE = [
-    "[2020-08-29] AAF035 (1).jpg",
-    "[2020-08-29] AAF035 (2).jpg",
-    "[2020-08-29] AAF035 (3).jpg",
-    "[2020-08-29] AAF035.jpg",
-    "DSC03584.dng",
-    "Frítest (1).jpg",
-    "Frítest_edited (1).jpeg",
-    "Frítest_edited.jpeg",
-    "Frítest_original (1).jpg",
-    "Frítest_original.jpg",
-    "Frítest.jpg",
-    "IMG_1693.tif",
-    "IMG_1994.cr2",
-    "IMG_1994.JPG",
-    "IMG_1997.cr2",
-    "IMG_1997.JPG",
-    "IMG_3092_edited.jpeg",
-    "IMG_3092_original.heic",
-    "IMG_4547.jpg",
-    "Jellyfish.MOV",
-    "Jellyfish1.mp4",
-    "Pumkins1.jpg",
-    "Pumkins2.jpg",
-    "Pumpkins3.jpg",
-    "screenshot-really-a-png.jpeg",
-    "St James Park_edited.jpeg",
-    "St James Park_original.jpg",
-    "Tulips_edited.jpeg",
-    "Tulips_original.jpg",
-    "wedding_edited.jpeg",
-    "wedding_original.jpg",
-    "winebottle (1).jpeg",
-    "winebottle.jpeg",
-]
+CLI_EXPORT_FILENAMES_ORIGINAL_SUFFIX_TEMPLATE = _normalize_fs_paths(
+    [
+        "[2020-08-29] AAF035 (1).jpg",
+        "[2020-08-29] AAF035 (2).jpg",
+        "[2020-08-29] AAF035 (3).jpg",
+        "[2020-08-29] AAF035.jpg",
+        "DSC03584.dng",
+        "Frítest (1).jpg",
+        "Frítest_edited (1).jpeg",
+        "Frítest_edited.jpeg",
+        "Frítest_original (1).jpg",
+        "Frítest_original.jpg",
+        "Frítest.jpg",
+        "IMG_1693.tif",
+        "IMG_1994.cr2",
+        "IMG_1994.JPG",
+        "IMG_1997.cr2",
+        "IMG_1997.JPG",
+        "IMG_3092_edited.jpeg",
+        "IMG_3092_original.heic",
+        "IMG_4547.jpg",
+        "Jellyfish.MOV",
+        "Jellyfish1.mp4",
+        "Pumkins1.jpg",
+        "Pumkins2.jpg",
+        "Pumpkins3.jpg",
+        "screenshot-really-a-png.jpeg",
+        "St James Park_edited.jpeg",
+        "St James Park_original.jpg",
+        "Tulips_edited.jpeg",
+        "Tulips_original.jpg",
+        "wedding_edited.jpeg",
+        "wedding_original.jpg",
+        "winebottle (1).jpeg",
+        "winebottle.jpeg",
+    ]
+)
 
 CLI_EXPORT_FILENAMES_CURRENT = [
     "1793FAAB-DE75-4E25-886C-2BD66C780D6A_edited.jpeg",  # Frítest.jpg
     "1793FAAB-DE75-4E25-886C-2BD66C780D6A.jpeg",  # Frítest.jpg
     "1EB2B765-0765-43BA-A90C-0D0580E6172C.jpeg",
     "2DFD33F1-A5D8-486F-A3A9-98C07995535A.jpeg",
     "35329C57-B963-48D6-BB75-6AFF9370CBBC.mov",
@@ -322,184 +350,206 @@
     "E2078879-A29C-4D6F-BACB-E3BBE6C3EB91.jpeg",
     "E9BC5C36-7CD1-40A1-A72B-8B8FAC227D51_edited.jpeg",
     "E9BC5C36-7CD1-40A1-A72B-8B8FAC227D51.jpeg",
     "F12384F6-CD17-4151-ACBA-AE0E3688539E.jpeg",
     "F207D5DE-EFAD-4217-8424-0764AAC971D0.jpeg",
 ]
 
-CLI_EXPORT_FILENAMES_CONVERT_TO_JPEG = [
-    "[2020-08-29] AAF035 (1).jpg",
-    "[2020-08-29] AAF035 (2).jpg",
-    "[2020-08-29] AAF035 (3).jpg",
-    "[2020-08-29] AAF035.jpg",
-    "DSC03584.jpeg",
-    "Frítest (1).jpg",
-    "Frítest (2).jpg",
-    "Frítest (3).jpg",
-    "Frítest_edited (1).jpeg",
-    "Frítest_edited.jpeg",
-    "Frítest.jpg",
-    "IMG_1693.jpeg",
-    "IMG_1994.cr2",
-    "IMG_1994.JPG",
-    "IMG_1997.cr2",
-    "IMG_1997.JPG",
-    "IMG_3092_edited.jpeg",
-    "IMG_3092.jpeg",
-    "IMG_4547.jpg",
-    "Jellyfish.MOV",
-    "Jellyfish1.mp4",
-    "Pumkins1.jpg",
-    "Pumkins2.jpg",
-    "Pumpkins3.jpg",
-    "screenshot-really-a-png.jpeg",
-    "St James Park_edited.jpeg",
-    "St James Park.jpg",
-    "Tulips_edited.jpeg",
-    "Tulips.jpg",
-    "wedding_edited.jpeg",
-    "wedding.jpg",
-    "winebottle (1).jpeg",
-    "winebottle.jpeg",
-]
+CLI_EXPORT_FILENAMES_CONVERT_TO_JPEG = _normalize_fs_paths(
+    [
+        "[2020-08-29] AAF035 (1).jpg",
+        "[2020-08-29] AAF035 (2).jpg",
+        "[2020-08-29] AAF035 (3).jpg",
+        "[2020-08-29] AAF035.jpg",
+        "DSC03584.jpeg",
+        "Frítest (1).jpg",
+        "Frítest (2).jpg",
+        "Frítest (3).jpg",
+        "Frítest_edited (1).jpeg",
+        "Frítest_edited.jpeg",
+        "Frítest.jpg",
+        "IMG_1693.jpeg",
+        "IMG_1994.cr2",
+        "IMG_1994.JPG",
+        "IMG_1997.cr2",
+        "IMG_1997.JPG",
+        "IMG_3092_edited.jpeg",
+        "IMG_3092.jpeg",
+        "IMG_4547.jpg",
+        "Jellyfish.MOV",
+        "Jellyfish1.mp4",
+        "Pumkins1.jpg",
+        "Pumkins2.jpg",
+        "Pumpkins3.jpg",
+        "screenshot-really-a-png.jpeg",
+        "St James Park_edited.jpeg",
+        "St James Park.jpg",
+        "Tulips_edited.jpeg",
+        "Tulips.jpg",
+        "wedding_edited.jpeg",
+        "wedding.jpg",
+        "winebottle (1).jpeg",
+        "winebottle.jpeg",
+    ]
+)
 
-CLI_EXPORT_FILENAMES_CONVERT_TO_JPEG_SKIP_RAW = [
-    "[2020-08-29] AAF035 (1).jpg",
-    "[2020-08-29] AAF035 (2).jpg",
-    "[2020-08-29] AAF035 (3).jpg",
-    "[2020-08-29] AAF035.jpg",
-    "DSC03584.jpeg",
-    "Frítest (1).jpg",
-    "Frítest (2).jpg",
-    "Frítest (3).jpg",
-    "Frítest_edited (1).jpeg",
-    "Frítest_edited.jpeg",
-    "Frítest.jpg",
-    "IMG_1693.jpeg",
-    "IMG_1994.JPG",
-    "IMG_1997.JPG",
-    "IMG_3092_edited.jpeg",
-    "IMG_3092.jpeg",
-    "IMG_4547.jpg",
-    "Jellyfish.MOV",
-    "Jellyfish1.mp4",
-    "Pumkins1.jpg",
-    "Pumkins2.jpg",
-    "Pumpkins3.jpg",
-    "screenshot-really-a-png.jpeg",
-    "St James Park_edited.jpeg",
-    "St James Park.jpg",
-    "Tulips_edited.jpeg",
-    "Tulips.jpg",
-    "wedding_edited.jpeg",
-    "wedding.jpg",
-    "winebottle (1).jpeg",
-    "winebottle.jpeg",
-]
+CLI_EXPORT_FILENAMES_CONVERT_TO_JPEG_SKIP_RAW = _normalize_fs_paths(
+    [
+        "[2020-08-29] AAF035 (1).jpg",
+        "[2020-08-29] AAF035 (2).jpg",
+        "[2020-08-29] AAF035 (3).jpg",
+        "[2020-08-29] AAF035.jpg",
+        "DSC03584.jpeg",
+        "Frítest (1).jpg",
+        "Frítest (2).jpg",
+        "Frítest (3).jpg",
+        "Frítest_edited (1).jpeg",
+        "Frítest_edited.jpeg",
+        "Frítest.jpg",
+        "IMG_1693.jpeg",
+        "IMG_1994.JPG",
+        "IMG_1997.JPG",
+        "IMG_3092_edited.jpeg",
+        "IMG_3092.jpeg",
+        "IMG_4547.jpg",
+        "Jellyfish.MOV",
+        "Jellyfish1.mp4",
+        "Pumkins1.jpg",
+        "Pumkins2.jpg",
+        "Pumpkins3.jpg",
+        "screenshot-really-a-png.jpeg",
+        "St James Park_edited.jpeg",
+        "St James Park.jpg",
+        "Tulips_edited.jpeg",
+        "Tulips.jpg",
+        "wedding_edited.jpeg",
+        "wedding.jpg",
+        "winebottle (1).jpeg",
+        "winebottle.jpeg",
+    ]
+)
 
 CLI_EXPORT_CONVERT_TO_JPEG_LARGE_FILE = "DSC03584.jpeg"
 
-CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES1 = [
-    "2019/April/wedding.jpg",
-    "2019/July/Tulips.jpg",
-    "2018/October/St James Park.jpg",
-    "2018/September/Pumpkins3.jpg",
-    "2018/September/Pumkins2.jpg",
-    "2018/September/Pumkins1.jpg",
-]
+CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES1 = _normalize_fs_paths(
+    [
+        "2019/April/wedding.jpg",
+        "2019/July/Tulips.jpg",
+        "2018/October/St James Park.jpg",
+        "2018/September/Pumpkins3.jpg",
+        "2018/September/Pumkins2.jpg",
+        "2018/September/Pumkins1.jpg",
+    ]
+)
 
-CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES_LOCALE = [
-    "2019/September/IMG_9975.JPEG",
-    "2020/Februar/IMG_1064.JPEG",
-    "2016/März/IMG_3984.JPEG",
-]
+CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES_LOCALE = _normalize_fs_paths(
+    [
+        "2019/September/IMG_9975.JPEG",
+        "2020/Februar/IMG_1064.JPEG",
+        "2016/März/IMG_3984.JPEG",
+    ]
+)
 
-CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES_ALBUM1 = [
-    "Multi Keyword/wedding.jpg",
-    "_/Tulips.jpg",
-    "_/St James Park.jpg",
-    "Pumpkin Farm/Pumpkins3.jpg",
-    "Pumpkin Farm/Pumkins2.jpg",
-    "Pumpkin Farm/Pumkins1.jpg",
-    "Test Album/Pumkins1.jpg",
-]
+CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES_ALBUM1 = _normalize_fs_paths(
+    [
+        "Multi Keyword/wedding.jpg",
+        "_/Tulips.jpg",
+        "_/St James Park.jpg",
+        "Pumpkin Farm/Pumpkins3.jpg",
+        "Pumpkin Farm/Pumkins2.jpg",
+        "Pumpkin Farm/Pumkins1.jpg",
+        "Test Album/Pumkins1.jpg",
+    ]
+)
 
-CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES_ALBUM2 = [
-    "Multi Keyword/wedding.jpg",
-    "NOALBUM/Tulips.jpg",
-    "NOALBUM/St James Park.jpg",
-    "Pumpkin Farm/Pumpkins3.jpg",
-    "Pumpkin Farm/Pumkins2.jpg",
-    "Pumpkin Farm/Pumkins1.jpg",
-    "Test Album/Pumkins1.jpg",
-]
+CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES_ALBUM2 = _normalize_fs_paths(
+    [
+        "Multi Keyword/wedding.jpg",
+        "NOALBUM/Tulips.jpg",
+        "NOALBUM/St James Park.jpg",
+        "Pumpkin Farm/Pumpkins3.jpg",
+        "Pumpkin Farm/Pumkins2.jpg",
+        "Pumpkin Farm/Pumkins1.jpg",
+        "Test Album/Pumkins1.jpg",
+    ]
+)
 
-CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES2 = [
-    "St James's Park, Great Britain, Westminster, England, United Kingdom/St James Park.jpg",
-    "_/Pumpkins3.jpg",
-    "Omaha, Nebraska, United States/Pumkins2.jpg",
-    "_/Pumkins1.jpg",
-    "_/Tulips.jpg",
-    "_/wedding.jpg",
-]
+CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES2 = _normalize_fs_paths(
+    [
+        "St James's Park, Great Britain, Westminster, England, United Kingdom/St James Park.jpg",
+        "_/Pumpkins3.jpg",
+        "Omaha, Nebraska, United States/Pumkins2.jpg",
+        "_/Pumkins1.jpg",
+        "_/Tulips.jpg",
+        "_/wedding.jpg",
+    ]
+)
 
-CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES3 = [
-    "2019/{foo}/wedding.jpg",
-    "2019/{foo}/Tulips.jpg",
-    "2018/{foo}/St James Park.jpg",
-    "2018/{foo}/Pumpkins3.jpg",
-    "2018/{foo}/Pumkins2.jpg",
-    "2018/{foo}/Pumkins1.jpg",
-]
+CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES3 = _normalize_fs_paths(
+    [
+        "2019/{foo}/wedding.jpg",
+        "2019/{foo}/Tulips.jpg",
+        "2018/{foo}/St James Park.jpg",
+        "2018/{foo}/Pumpkins3.jpg",
+        "2018/{foo}/Pumkins2.jpg",
+        "2018/{foo}/Pumkins1.jpg",
+    ]
+)
 
 
-CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES1 = [
-    "2019-wedding.jpg",
-    "2019-wedding_edited.jpeg",
-    "2019-Tulips.jpg",
-    "2018-St James Park.jpg",
-    "2018-St James Park_edited.jpeg",
-    "2018-Pumpkins3.jpg",
-    "2018-Pumkins2.jpg",
-    "2018-Pumkins1.jpg",
-]
+CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES1 = _normalize_fs_paths(
+    [
+        "2019-wedding.jpg",
+        "2019-wedding_edited.jpeg",
+        "2019-Tulips.jpg",
+        "2018-St James Park.jpg",
+        "2018-St James Park_edited.jpeg",
+        "2018-Pumpkins3.jpg",
+        "2018-Pumkins2.jpg",
+        "2018-Pumkins1.jpg",
+    ]
+)
 
-CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES2 = [
-    "Folder1_SubFolder2_AlbumInFolder-IMG_4547.jpg",
-    "Folder1_SubFolder2_AlbumInFolder-wedding.jpg",
-    "Folder1_SubFolder2_AlbumInFolder-wedding_edited.jpeg",
-    "Folder2_Raw-DSC03584.dng",
-    "Folder2_Raw-IMG_1994.cr2",
-    "Folder2_Raw-IMG_1994.JPG",
-    "Folder2_Raw-IMG_1997.cr2",
-    "Folder2_Raw-IMG_1997.JPG",
-    "None-St James Park.jpg",
-    "None-St James Park_edited.jpeg",
-    "None-Tulips.jpg",
-    "None-Tulips_edited.jpeg",
-    "Pumpkin Farm-Pumkins1.jpg",
-    "Pumpkin Farm-Pumkins2.jpg",
-    "Pumpkin Farm-Pumpkins3.jpg",
-    "Test Album-Pumkins1.jpg",
-    "Test Album-Pumkins2.jpg",
-    "None-IMG_1693.tif",
-    "I have a deleted twin-wedding.jpg",
-    "I have a deleted twin-wedding_edited.jpeg",
-]
+CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES2 = _normalize_fs_paths(
+    [
+        "Folder1_SubFolder2_AlbumInFolder-IMG_4547.jpg",
+        "Folder1_SubFolder2_AlbumInFolder-wedding.jpg",
+        "Folder1_SubFolder2_AlbumInFolder-wedding_edited.jpeg",
+        "Folder2_Raw-DSC03584.dng",
+        "Folder2_Raw-IMG_1994.cr2",
+        "Folder2_Raw-IMG_1994.JPG",
+        "Folder2_Raw-IMG_1997.cr2",
+        "Folder2_Raw-IMG_1997.JPG",
+        "None-St James Park.jpg",
+        "None-St James Park_edited.jpeg",
+        "None-Tulips.jpg",
+        "None-Tulips_edited.jpeg",
+        "Pumpkin Farm-Pumkins1.jpg",
+        "Pumpkin Farm-Pumkins2.jpg",
+        "Pumpkin Farm-Pumpkins3.jpg",
+        "Test Album-Pumkins1.jpg",
+        "Test Album-Pumkins2.jpg",
+        "None-IMG_1693.tif",
+        "I have a deleted twin-wedding.jpg",
+        "I have a deleted twin-wedding_edited.jpeg",
+    ]
+)
 
-CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES_PATHSEP = [
-    "2018-10 - Sponsion, Museum, Frühstück, Römermuseum/IMG_4547.jpg",
-    "Folder1/SubFolder2/AlbumInFolder/IMG_4547.jpg",
-    "2019-10:11 Paris Clermont/IMG_4547.jpg",
-]
+CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES_PATHSEP = _normalize_fs_paths(
+    [
+        "2018-10 - Sponsion, Museum, Frühstück, Römermuseum/IMG_4547.jpg",
+        "Folder1/SubFolder2/AlbumInFolder/IMG_4547.jpg",
+        "2019-10:11 Paris Clermont/IMG_4547.jpg",
+    ]
+)
 
 
-CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES_KEYWORD_PATHSEP = [
-    "foo:bar/foo:bar_IMG_3092.heic"
-]
+CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES_KEYWORD_PATHSEP = _normalize_fs_paths(
+    ["foo:bar/foo:bar_IMG_3092.heic"]
+)
 
 CLI_EXPORTED_FILENAME_TEMPLATE_LONG_DESCRIPTION = [
     "Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo"
     " ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis "
     "dis parturient montes, nascetu. Donec quam felis, ultricies nec, "
     "pellentesque eu, pretium q.tif"
 ]
@@ -515,54 +565,79 @@
 CLI_EXPORT_UUID_FILENAME_PREVIEW_TEMPLATE = "Pumkins2_lowres.jpeg"
 
 CLI_EXPORT_BY_DATE_TOUCH_UUID = [
     "1EB2B765-0765-43BA-A90C-0D0580E6172C",  # Pumpkins3.jpg
     "F12384F6-CD17-4151-ACBA-AE0E3688539E",  # Pumkins1.jpg
 ]
 CLI_EXPORT_BY_DATE_TOUCH_TIMES = [1538165373, 1538163349]
-CLI_EXPORT_BY_DATE_NEED_TOUCH = [
-    "2018/09/28/Pumkins2.jpg",
-    "2018/10/13/St James Park.jpg",
-]
+CLI_EXPORT_BY_DATE_NEED_TOUCH = _normalize_fs_paths(
+    [
+        "2018/09/28/Pumkins2.jpg",
+        "2018/10/13/St James Park.jpg",
+    ]
+)
 CLI_EXPORT_BY_DATE_NEED_TOUCH_UUID = [
     "D79B8D77-BFFC-460B-9312-034F2877D35B",
     "DC99FBDD-7A52-4100-A5BB-344131646C30",
 ]
 CLI_EXPORT_BY_DATE_NEED_TOUCH_TIMES = [1538165227, 1539436692]
-CLI_EXPORT_BY_DATE = ["2018/09/28/Pumpkins3.jpg", "2018/09/28/Pumkins1.jpg"]
+CLI_EXPORT_BY_DATE = _normalize_fs_paths(
+    [
+        "2018/09/28/Pumpkins3.jpg",
+        "2018/09/28/Pumkins1.jpg",
+    ]
+)
 
-CLI_EXPORT_SIDECAR_FILENAMES = ["Pumkins2.jpg", "Pumkins2.jpg.json", "Pumkins2.jpg.xmp"]
-CLI_EXPORT_SIDECAR_DROP_EXT_FILENAMES = [
-    "Pumkins2.jpg",
-    "Pumkins2.json",
-    "Pumkins2.xmp",
-]
+CLI_EXPORT_SIDECAR_FILENAMES = _normalize_fs_paths(
+    [
+        "Pumkins2.jpg",
+        "Pumkins2.jpg.json",
+        "Pumkins2.jpg.xmp",
+    ]
+)
+CLI_EXPORT_SIDECAR_DROP_EXT_FILENAMES = _normalize_fs_paths(
+    [
+        "Pumkins2.jpg",
+        "Pumkins2.json",
+        "Pumkins2.xmp",
+    ]
+)
 
 CLI_EXPORT_LIVE = [
     "51F2BEF7-431A-4D31-8AC1-3284A57826AE.jpeg",
     "51F2BEF7-431A-4D31-8AC1-3284A57826AE.mov",
 ]
 
-CLI_EXPORT_LIVE_ORIGINAL = ["IMG_0728.JPG", "IMG_0728.mov"]
+CLI_EXPORT_LIVE_ORIGINAL = _normalize_fs_paths(
+    [
+        "IMG_0728.JPG",
+        "IMG_0728.mov",
+    ]
+)
 
 CLI_EXPORT_RAW = ["441DFE2A-A69B-4C79-A69B-3F51D1B9B29C.cr2"]
-CLI_EXPORT_RAW_ORIGINAL = ["IMG_0476_2.CR2"]
+CLI_EXPORT_RAW_ORIGINAL = _normalize_fs_paths(["IMG_0476_2.CR2"])
 CLI_EXPORT_RAW_EDITED = [
     "441DFE2A-A69B-4C79-A69B-3F51D1B9B29C.cr2",
     "441DFE2A-A69B-4C79-A69B-3F51D1B9B29C_edited.jpeg",
 ]
-CLI_EXPORT_RAW_EDITED_ORIGINAL = ["IMG_0476_2.CR2", "IMG_0476_2_edited.jpeg"]
+CLI_EXPORT_RAW_EDITED_ORIGINAL = _normalize_fs_paths(
+    [
+        "IMG_0476_2.CR2",
+        "IMG_0476_2_edited.jpeg",
+    ]
+)
 
 CLI_UUID_DICT_15_7 = {
     "intrash": "71E3E212-00EB-430D-8A63-5E294B268554",
     "template": "F12384F6-CD17-4151-ACBA-AE0E3688539E",
 }
 
-CLI_TEMPLATE_SIDECAR_FILENAME = "Pumkins1.jpg.json"
-CLI_TEMPLATE_FILENAME = "Pumkins1.jpg"
+CLI_TEMPLATE_SIDECAR_FILENAME = normalize_fs_path("Pumkins1.jpg.json")
+CLI_TEMPLATE_FILENAME = normalize_fs_path("Pumkins1.jpg")
 
 CLI_UUID_DICT_14_6 = {"intrash": "3tljdX43R8+k6peNHVrJNQ"}
 
 PHOTOS_NOT_IN_TRASH_LEN_14_6 = 12
 PHOTOS_IN_TRASH_LEN_14_6 = 1
 PHOTOS_MISSING_14_6 = 1
 
@@ -956,20 +1031,22 @@
 UUID_UNICODE_TITLE = [
     "B13F4485-94E0-41CD-AF71-913095D62E31",  # Frítest.jpg
     "1793FAAB-DE75-4E25-886C-2BD66C780D6A",  # Frítest.jpg
     "A8266C97-9BAF-4AF4-99F3-0013832869B8",  # Frítest.jpg
     "D1D4040D-D141-44E8-93EA-E403D9F63E07",  # Frítest.jpg
 ]
 
-EXPORT_UNICODE_TITLE_FILENAMES = [
-    "Frítest.jpg",
-    "Frítest (1).jpg",
-    "Frítest (2).jpg",
-    "Frítest (3).jpg",
-]
+EXPORT_UNICODE_TITLE_FILENAMES = _normalize_fs_paths(
+    [
+        "Frítest.jpg",
+        "Frítest (1).jpg",
+        "Frítest (2).jpg",
+        "Frítest (3).jpg",
+    ]
+)
 
 # data for --report
 UUID_REPORT = [
     {
         "uuid": "4D521201-92AC-43E5-8F7C-59BC41C37A96",
         "filenames": ["IMG_1997.JPG", "IMG_1997.cr2"],
     },
@@ -983,20 +1060,22 @@
 QUERY_EXIF_DATA = [("EXIF:Make", "FUJIFILM", ["6191423D-8DB8-4D4C-92BE-9BBBA308AAC4"])]
 QUERY_EXIF_DATA_CASE_INSENSITIVE = [
     ("Make", "Fujifilm", ["6191423D-8DB8-4D4C-92BE-9BBBA308AAC4"])
 ]
 EXPORT_EXIF_DATA = [("EXIF:Make", "FUJIFILM", ["Tulips.jpg", "Tulips_edited.jpeg"])]
 
 UUID_LIVE_EDITED = "136A78FA-1B90-46CC-88A7-CCA3331F0353"  # IMG_4813.HEIC
-CLI_EXPORT_LIVE_EDITED = [
-    "IMG_4813.HEIC",
-    "IMG_4813.mov",
-    "IMG_4813_edited.jpeg",
-    "IMG_4813_edited.mov",
-]
+CLI_EXPORT_LIVE_EDITED = _normalize_fs_paths(
+    [
+        "IMG_4813.HEIC",
+        "IMG_4813.mov",
+        "IMG_4813_edited.jpeg",
+        "IMG_4813_edited.mov",
+    ]
+)
 
 UUID_FAVORITE = "E9BC5C36-7CD1-40A1-A72B-8B8FAC227D51"
 FILE_FAVORITE = "wedding.jpg"
 UUID_NOT_FAVORITE = "1EB2B765-0765-43BA-A90C-0D0580E6172C"
 FILE_NOT_FAVORITE = "Pumpkins3.jpg"
 
 # number of photos in test library with Make=Canon
@@ -1069,15 +1148,14 @@
         if photo.path_raw is not None:
             os.utime(photo.path_raw, (ts, ts))
         if photo.path_live_photo is not None:
             os.utime(photo.path_live_photo, (ts, ts))
 
 
 def test_osxphotos():
-
     runner = CliRunner()
     result = runner.invoke(cli_main, [])
 
     assert result.exit_code == 0
     assert "Print information about osxphotos" in result.output
 
 
@@ -1115,15 +1193,14 @@
     cwd = os.getcwd()
     result = runner.invoke(about, [])
     assert result.exit_code == 0
     assert "MIT License" in result.output
 
 
 def test_query_uuid():
-
     runner = CliRunner()
     cwd = os.getcwd()
     result = runner.invoke(
         query,
         [
             "--json",
             "--db",
@@ -1800,20 +1877,32 @@
             ],
         )
         assert result.exit_code == 0
         files = glob.glob("*")
         assert len(files) == 2  # preview + original
 
 
-def test_export_as_hardlink():
+@contextlib.contextmanager
+def isolated_filesystem_here():
+    cwd = os.getcwd()
+    tempdir = tempfile.mkdtemp(dir=cwd)  # type: ignore[type-var]
+    os.chdir(tempdir)
+
+    try:
+        yield tempdir
+    finally:
+        os.chdir(cwd)
+        shutil.rmtree(tempdir)
 
+
+def test_export_as_hardlink():
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
-    with runner.isolated_filesystem():
+    with isolated_filesystem_here():
         result = runner.invoke(
             export,
             [os.path.join(cwd, CLI_PHOTOS_DB), ".", "--export-as-hardlink", "-V"],
         )
         assert result.exit_code == 0
         files = glob.glob("*")
         assert sorted(files) == sorted(CLI_EXPORT_FILENAMES)
@@ -1825,15 +1914,15 @@
 
     runner = CliRunner()
     cwd = os.getcwd()
     photosdb = osxphotos.PhotosDB(dbfile=CLI_PHOTOS_DB)
     photo = photosdb.photos(uuid=[CLI_EXPORT_UUID])[0]
 
     # pylint: disable=not-context-manager
-    with runner.isolated_filesystem():
+    with isolated_filesystem_here():
         result = runner.invoke(
             export,
             [
                 os.path.join(cwd, CLI_PHOTOS_DB),
                 ".",
                 f"--uuid={CLI_EXPORT_UUID}",
                 "--export-as-hardlink",
@@ -1850,15 +1939,15 @@
 
     runner = CliRunner()
     cwd = os.getcwd()
     photosdb = osxphotos.PhotosDB(dbfile=CLI_PHOTOS_DB)
     photo = photosdb.photos(uuid=[CLI_EXPORT_UUID])[0]
 
     # pylint: disable=not-context-manager
-    with runner.isolated_filesystem():
+    with isolated_filesystem_here():
         result = runner.invoke(
             export,
             [
                 os.path.join(cwd, CLI_PHOTOS_DB),
                 ".",
                 f"--uuid={CLI_EXPORT_UUID}",
                 "--export-as-hardlink",
@@ -1867,43 +1956,40 @@
             ],
         )
         assert result.exit_code == 1
         assert "Incompatible export options" in result.output
 
 
 def test_export_current_name():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export, [os.path.join(cwd, PHOTOS_DB_15_7), ".", "--current-name", "-V"]
         )
         assert result.exit_code == 0
         files = glob.glob("*")
         assert sorted(files) == sorted(CLI_EXPORT_FILENAMES_CURRENT)
 
 
 def test_export_skip_edited():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export, [os.path.join(cwd, CLI_PHOTOS_DB), ".", "--skip-edited", "-V"]
         )
         assert result.exit_code == 0
         files = glob.glob("*")
         assert "St James Park_edited.jpeg" not in files
 
 
 def test_export_edited():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export, [os.path.join(cwd, CLI_PHOTOS_DB), ".", "--edited", "-V"]
         )
@@ -1912,15 +1998,14 @@
         # make sure edited versions did get exported
         assert "wedding_edited.jpeg" in files
         assert "Tulips_edited.jpeg" in files
         assert "St James Park_edited.jpeg" in files
 
 
 def test_export_not_edited():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export, [os.path.join(cwd, CLI_PHOTOS_DB), ".", "--not-edited", "-V"]
         )
@@ -1966,15 +2051,14 @@
 
         # make sure other originals did get exported
         assert "Pumkins2.jpg" in files
 
 
 @pytest.mark.skipif(exiftool is None, reason="exiftool not installed")
 def test_export_exiftool():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         for uuid in CLI_EXIFTOOL:
             result = runner.invoke(
                 export,
@@ -2178,15 +2262,14 @@
             assert re.search(r"Exported.*Canon", result.output)
 
     osxphotos.exiftool.get_exiftool_path = get_exiftool_path
 
 
 @pytest.mark.skipif(exiftool is None, reason="exiftool not installed")
 def test_export_exiftool_ignore_date_modified():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         for uuid in CLI_EXIFTOOL_IGNORE_DATE_MODIFIED:
             result = runner.invoke(
                 export,
@@ -3389,15 +3472,14 @@
         assert result.exit_code == 0
         assert "Writing exiftool sidecar" in result.output
         files = glob.glob("*.*")
         assert sorted(files) == sorted(CLI_EXPORT_SIDECAR_FILENAMES)
 
 
 def test_export_sidecar_templates():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             cli_main,
             [
@@ -3614,41 +3696,38 @@
             ],
         )
         assert result.exit_code != 0
         assert "cannot use --sidecar json with --sidecar exiftool" in result.output
 
 
 def test_export_live():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export, [os.path.join(cwd, LIVE_PHOTOS_DB), ".", "--live", "-V"]
         )
         files = glob.glob("*")
         assert sorted(files) == sorted(CLI_EXPORT_LIVE_ORIGINAL)
 
 
 def test_export_skip_live():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export, [os.path.join(cwd, LIVE_PHOTOS_DB), ".", "--skip-live", "-V"]
         )
         files = glob.glob("*")
         assert "img_0728.mov" not in [f.lower() for f in files]
 
 
 def test_export_raw():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
             [
@@ -3674,54 +3753,51 @@
 #         )
 #         files = glob.glob("*")
 #         for rawname in CLI_EXPORT_RAW:
 #             assert rawname.lower() not in [f.lower() for f in files]
 
 
 def test_export_raw_original():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export, [os.path.join(cwd, RAW_PHOTOS_DB), ".", "--skip-edited", "-V"]
         )
         files = glob.glob("*")
         assert sorted(files) == sorted(CLI_EXPORT_RAW_ORIGINAL)
 
 
 def test_export_raw_edited():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export, [os.path.join(cwd, RAW_PHOTOS_DB), ".", "--current-name", "-V"]
         )
         files = glob.glob("*")
         assert sorted(files) == sorted(CLI_EXPORT_RAW_EDITED)
 
 
 def test_export_raw_edited_original():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(export, [os.path.join(cwd, RAW_PHOTOS_DB), ".", "-V"])
         files = glob.glob("*")
         assert sorted(files) == sorted(CLI_EXPORT_RAW_EDITED_ORIGINAL)
 
 
 def test_export_directory_template_1():
     # test export using directory template
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
@@ -3833,15 +3909,15 @@
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         # set locale environment
         os.environ["LC_ALL"] = "de_DE.UTF-8"
-        locale.setlocale(locale.LC_ALL, "")
+        setlocale(locale.LC_ALL, "")
         result = runner.invoke(
             export,
             [
                 os.path.join(cwd, PLACES_PHOTOS_DB),
                 ".",
                 "-V",
                 "--directory",
@@ -3853,15 +3929,15 @@
         for filepath in CLI_EXPORTED_DIRECTORY_TEMPLATE_FILENAMES_LOCALE:
             assert os.path.isfile(os.path.join(workdir, filepath))
 
 
 def test_export_filename_template_1():
     """export photos using filename template"""
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
@@ -3878,15 +3954,15 @@
         for file in CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES1:
             assert file in files
 
 
 def test_export_filename_template_2():
     """export photos using filename template with folder_album and path_sep"""
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
@@ -3903,15 +3979,15 @@
         for file in CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES2:
             assert file in files
 
 
 def test_export_filename_template_strip():
     """export photos using filename template with --strip"""
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
@@ -3929,15 +4005,15 @@
         for file in CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES1:
             assert file in files
 
 
 def test_export_filename_template_pathsep_in_name_1():
     """export photos using filename template with folder_album and "/" in album name"""
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
@@ -3956,15 +4032,15 @@
             # assert fname in result.output
             assert pathlib.Path(fname).is_file()
 
 
 def test_export_filename_template_pathsep_in_name_2():
     """export photos using filename template with keyword and "/" in keyword"""
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
@@ -3984,15 +4060,15 @@
         for fname in CLI_EXPORTED_FILENAME_TEMPLATE_FILENAMES_KEYWORD_PATHSEP:
             assert pathlib.Path(fname).is_file()
 
 
 def test_export_filename_template_long_description():
     """export photos using filename template with description that exceeds max length"""
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
@@ -4232,15 +4308,14 @@
             [os.path.join(cwd, CLI_PHOTOS_DB), ".", "--exif", exiftag, exifvalue, "-V"],
         )
         files = glob.glob("*")
         assert sorted(files) == sorted(files_expected)
 
 
 def test_places():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             places, ["--db", os.path.join(cwd, PLACES_PHOTOS_DB), "--json"]
         )
@@ -4448,15 +4523,14 @@
         assert result.exit_code == 0
         json_got = json.loads(result.output)
         assert len(json_got) == 1  # single element
         assert json_got[0]["uuid"] == "15uNd7%8RguTEgNPKHfTWw"
 
 
 def test_export_sidecar_keyword_template():
-
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             cli_main,
             [
@@ -4660,15 +4734,14 @@
         )
 
         # run --force-update, nothing should export
         result = runner.invoke(
             export, [os.path.join(cwd, photos_db_path), ".", "--force-update"]
         )
         assert result.exit_code == 0
-        print(result.output)
         assert (
             f"Processed: {PHOTOS_NOT_IN_TRASH_LEN_15_7} photos, exported: 0, updated: 0, skipped: {PHOTOS_NOT_IN_TRASH_LEN_15_7+PHOTOS_EDITED_15_7}, updated EXIF data: 0, missing: 3, error: 0"
             in result.output
         )
 
 
 @pytest.mark.skipif(exiftool is None, reason="exiftool not installed")
@@ -4887,15 +4960,15 @@
 
     photosdb = osxphotos.PhotosDB(dbfile=CLI_PHOTOS_DB)
     photo = photosdb.photos(uuid=[CLI_EXPORT_UUID])[0]
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
-    with runner.isolated_filesystem():
+    with isolated_filesystem_here():
         # basic export
         result = runner.invoke(
             export,
             [os.path.join(cwd, CLI_PHOTOS_DB), ".", "-V", "--export-as-hardlink"],
         )
         assert result.exit_code == 0
         files = glob.glob("*")
@@ -4920,15 +4993,15 @@
 
     photosdb = osxphotos.PhotosDB(dbfile=CLI_PHOTOS_DB)
     photo = photosdb.photos(uuid=[CLI_EXPORT_UUID])[0]
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
-    with runner.isolated_filesystem():
+    with isolated_filesystem_here():
         # basic export
         result = runner.invoke(
             export,
             [os.path.join(cwd, CLI_PHOTOS_DB), ".", "-V", "--export-as-hardlink"],
         )
         assert result.exit_code == 0
         files = glob.glob("*")
@@ -5065,15 +5138,15 @@
 
     photosdb = osxphotos.PhotosDB(dbfile=CLI_PHOTOS_DB)
     photo = photosdb.photos(uuid=[CLI_EXPORT_UUID])[0]
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
-    with runner.isolated_filesystem():
+    with isolated_filesystem_here():
         # basic export
         result = runner.invoke(export, [os.path.join(cwd, CLI_PHOTOS_DB), ".", "-V"])
         assert result.exit_code == 0
         files = glob.glob("*")
         assert sorted(files) == sorted(CLI_EXPORT_FILENAMES)
         assert not os.path.samefile(CLI_EXPORT_UUID_FILENAME, photo.path)
 
@@ -5173,15 +5246,15 @@
         # make sure file didn't really get copied
         assert not os.path.isfile(CLI_EXPORT_BY_DATE[0])
 
 
 def test_export_directory_template_1_dry_run():
     """test export using directory template with dry-run flag"""
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
         result = runner.invoke(
             export,
@@ -5229,19 +5302,25 @@
         )
         assert result.exit_code == 0
 
         assert (
             f"exported: {PHOTOS_NOT_IN_TRASH_LEN_15_7+PHOTOS_EDITED_15_7}"
             in result.output
         )
-        assert (
-            f"touched date: {PHOTOS_NOT_IN_TRASH_LEN_15_7+PHOTOS_EDITED_15_7-2}"
-            in result.output
+
+        # on macOS there are two files that have the correct date and these don't get touched
+        # on other platforms, all files get touched
+        touched_files = (
+            PHOTOS_NOT_IN_TRASH_LEN_15_7 + PHOTOS_EDITED_15_7 - 2
+            if is_macos
+            else PHOTOS_NOT_IN_TRASH_LEN_15_7 + PHOTOS_EDITED_15_7
         )
 
+        assert f"touched date: {touched_files}" in result.output
+
         for fname, mtime in zip(CLI_EXPORT_BY_DATE, CLI_EXPORT_BY_DATE_TOUCH_TIMES):
             st = os.stat(fname)
             assert int(st.st_mtime) == int(mtime)
 
 
 def test_export_touch_files_update():
     """test complex export scenario with --update and --touch-files"""
@@ -5307,19 +5386,25 @@
             ],
         )
         assert result.exit_code == 0
         assert (
             f"skipped: {PHOTOS_NOT_IN_TRASH_LEN_15_7+PHOTOS_EDITED_15_7}"
             in result.output
         )
-        assert (
-            f"touched date: {PHOTOS_NOT_IN_TRASH_LEN_15_7+PHOTOS_EDITED_15_7-2}"
-            in result.output
+
+        # on macOS there are two files that have the correct date and these don't get touched
+        # on other platforms, all files get touched
+        touched_files = (
+            PHOTOS_NOT_IN_TRASH_LEN_15_7 + PHOTOS_EDITED_15_7 - 2
+            if is_macos
+            else PHOTOS_NOT_IN_TRASH_LEN_15_7 + PHOTOS_EDITED_15_7
         )
 
+        assert f"touched date: {touched_files}" in result.output
+
         for fname, mtime in zip(
             CLI_EXPORT_BY_DATE_NEED_TOUCH, CLI_EXPORT_BY_DATE_NEED_TOUCH_TIMES
         ):
             st = os.stat(fname)
             assert int(st.st_mtime) != int(mtime)
 
         # --update --touch-file
@@ -5334,18 +5419,15 @@
             ],
         )
         assert result.exit_code == 0
         assert (
             f"skipped: {PHOTOS_NOT_IN_TRASH_LEN_15_7+PHOTOS_EDITED_15_7}"
             in result.output
         )
-        assert (
-            f"touched date: {PHOTOS_NOT_IN_TRASH_LEN_15_7+PHOTOS_EDITED_15_7-2}"
-            in result.output
-        )
+        assert f"touched date: {touched_files}" in result.output
 
         for fname, mtime in zip(
             CLI_EXPORT_BY_DATE_NEED_TOUCH, CLI_EXPORT_BY_DATE_NEED_TOUCH_TIMES
         ):
             st = os.stat(fname)
             assert int(st.st_mtime) == int(mtime)
 
@@ -6048,15 +6130,15 @@
 
 def test_export_as_hardlink_download_missing():
     """test export with incompatible export options"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
-    with runner.isolated_filesystem():
+    with isolated_filesystem_here():
         result = runner.invoke(
             export,
             [
                 os.path.join(cwd, CLI_PHOTOS_DB),
                 ".",
                 "-V",
                 "--download-missing",
@@ -6873,14 +6955,15 @@
                     f"{uuid}",
                     "--dry-run",
                 ],
             )
             assert result.exit_code == 0
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_export_finder_tag_keywords():
     """test --finder-tag-keywords"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
@@ -6947,14 +7030,15 @@
             md = OSXMetaData(CLI_FINDER_TAGS[uuid]["File:FileName"])
             keywords = CLI_FINDER_TAGS[uuid]["IPTC:Keywords"]
             keywords = [keywords] if type(keywords) != list else keywords
             expected = [Tag(x, 0) for x in keywords]
             assert sorted(md.tags) == sorted(expected)
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_export_finder_tag_template():
     """test --finder-tag-template"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
@@ -7024,14 +7108,15 @@
             md = OSXMetaData(CLI_FINDER_TAGS[uuid]["File:FileName"])
             keywords = CLI_FINDER_TAGS[uuid]["XMP:PersonInImage"]
             keywords = [keywords] if type(keywords) != list else keywords
             expected = [Tag(x, 0) for x in keywords]
             assert sorted(md.tags) == sorted(expected)
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_export_finder_tag_template_multiple():
     """test --finder-tag-template used more than once"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
@@ -7057,14 +7142,15 @@
             keywords = [keywords] if type(keywords) != list else keywords
             persons = CLI_FINDER_TAGS[uuid]["XMP:PersonInImage"]
             persons = [persons] if type(persons) != list else persons
             expected = [Tag(x, 0) for x in set(keywords + persons)]
             assert sorted(md.tags) == sorted(expected)
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_export_finder_tag_template_keywords():
     """test --finder-tag-template with --finder-tag-keywords"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
@@ -7089,14 +7175,15 @@
             keywords = [keywords] if type(keywords) != list else keywords
             persons = CLI_FINDER_TAGS[uuid]["XMP:PersonInImage"]
             persons = [persons] if type(persons) != list else persons
             expected = [Tag(x, 0) for x in set(keywords + persons)]
             assert sorted(md.tags) == sorted(expected)
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_export_finder_tag_template_multi_field():
     """test --finder-tag-template with multiple fields (issue #422)"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
@@ -7153,14 +7240,15 @@
                     "--dry-run",
                 ],
             )
             assert result.exit_code == 0
             assert "Writing extended attribute" in result.output
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_export_xattr_template():
     """test --xattr template"""
 
     # Note: this test does not actually test that the metadata attributes get correctly
     # written by osxmetadata as osxmetadata doesn't work reliably when run by pytest
     # (but does appear to work correctly in practice)
     # Reference: https://github.com/RhetTbull/osxmetadata/issues/68
@@ -7651,22 +7739,22 @@
 def test_query_name_unicode():
     """test query --name with a unicode name"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     result = runner.invoke(
         query,
-        ["--json", "--db", os.path.join(cwd, PHOTOS_DB_15_7), "--name", "Frítest"],
+        ["--json", "--db", os.path.join(cwd, PHOTOS_DB_15_7), "--name", "Frítest"],
     )
     assert result.exit_code == 0
     json_got = json.loads(result.output)
 
     assert len(json_got) == 4
     assert normalize_unicode(json_got[0]["original_filename"]).startswith(
-        normalize_unicode("Frítest.jpg")
+        normalize_unicode("Frítest.jpg")
     )
 
 
 def test_query_name_i():
     """test query --name -i"""
 
     runner = CliRunner()
```

### Comparing `osxphotos-0.59.3/tests/test_cli_add_locations.py` & `osxphotos-0.60.0/tests/test_cli_add_locations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Test osxphotos add-locations command"""
 
-import photoscript
 import pytest
 from click.testing import CliRunner
 
-from osxphotos.cli.add_locations import add_locations
+from osxphotos.utils import is_macos
+if is_macos:
+    import photoscript
+    from osxphotos.cli.add_locations import add_locations
+else:
+    pytest.skip(allow_module_level=True)
 
 UUID_TEST_PHOTO_1 = "F12384F6-CD17-4151-ACBA-AE0E3688539E"  # Pumkins1.jpg
 UUID_TEST_PHOTO_LOCATION = "D79B8D77-BFFC-460B-9312-034F2877D35B"  # Pumkins2.jpg
 TEST_LOCATION = (41.26067, -95.94056)  # Omaha, NE
 
 
 @pytest.mark.test_add_locations
```

### Comparing `osxphotos-0.59.3/tests/test_cli_add_to_album.py` & `osxphotos-0.60.0/tests/test_cli_add_to_album.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """ Test --add-exported-to-album """
 
 import os
 
-import photoscript
 import pytest
 from click.testing import CliRunner
 
+from osxphotos.utils import is_macos
+if is_macos:
+    import photoscript
+else:
+    pytest.skip(allow_module_level=True)
+
 UUID_EXPORT = {"3DD2C897-F19E-4CA6-8C22-B027D5A71907": {"filename": "IMG_4547.jpg"}}
 UUID_MISSING = {
     "8E1D7BC9-9321-44F9-8CFB-4083F6B9232A": {"filename": "IMG_2000.JPGssss"}
 }
 
 # photos with matching names
 QUERY_NAME = "IMG_"
```

### Comparing `osxphotos-0.59.3/tests/test_cli_all_commands.py` & `osxphotos-0.60.0/tests/test_cli_all_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 TEST_RUN_SCRIPT = "examples/cli_example_1.py"
 
 
 @pytest.fixture(scope="module")
 def runner() -> CliRunner:
     return CliRunner()
 
-
 from osxphotos.cli import (
     about,
     albums,
     debug_dump,
     docs_command,
     dump,
     grep,
@@ -38,18 +37,22 @@
     labels,
     list_libraries,
     orphans,
     persons,
     places,
     theme,
     tutorial,
-    uuid,
     version,
 )
 
+from osxphotos.utils import is_macos
+
+if is_macos:
+    from osxphotos.cli import uuid
+
 
 def test_about(runner: CliRunner):
     with runner.isolated_filesystem():
         result = runner.invoke(about)
         assert result.exit_code == 0
 
 
@@ -64,17 +67,16 @@
         keywords,
         labels,
         list_libraries,
         orphans,
         persons,
         places,
         tutorial,
-        uuid,
         version,
-    ],
+    ] + ([uuid] if is_macos else []),
 )
 def test_cli_comands(runner: CliRunner, command: Callable[..., Any]):
     with runner.isolated_filesystem():
         result = runner.invoke(albums, ["--db", TEST_DB])
         assert result.exit_code == 0
```

### Comparing `osxphotos-0.59.3/tests/test_cli_batch_edit.py` & `osxphotos-0.60.0/tests/test_cli_batch_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """Test osxphotos batch-edit command"""
 
 from __future__ import annotations
 
 import os
 import time
 
-import photoscript
 import pytest
 from click.testing import CliRunner
 
 import osxphotos
-from osxphotos.cli.batch_edit import batch_edit
+from osxphotos.utils import is_macos
+
+if is_macos:
+    import photoscript
+    from osxphotos.cli.batch_edit import batch_edit
+else:
+    pytest.skip(allow_module_level=True)
 
 # set timezone to avoid issues with comparing dates
 os.environ["TZ"] = "US/Pacific"
 time.tzset()
 
 
 TEST_DATA_BATCH_EDIT = {
```

### Comparing `osxphotos-0.59.3/tests/test_cli_dump.py` & `osxphotos-0.60.0/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_exiftool.py` & `osxphotos-0.60.0/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_export_cloud.py` & `osxphotos-0.60.0/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_export_projects.py` & `osxphotos-0.60.0/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_exportdb.py` & `osxphotos-0.60.0/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_import.py` & `osxphotos-0.60.0/tests/test_cli_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,31 @@
 import sqlite3
 import time
 from datetime import datetime
 from tempfile import TemporaryDirectory
 from typing import Dict
 
 import pytest
+
 from click.testing import CliRunner
-from photoscript import Photo
 from pytest import MonkeyPatch, approx
 
 from osxphotos import PhotosDB, QueryOptions
 from osxphotos._constants import UUID_PATTERN
-from osxphotos.cli.import_cli import import_cli
 from osxphotos.datetime_utils import datetime_remove_tz
 from osxphotos.exiftool import get_exiftool_path
+from osxphotos.utils import is_macos
 from tests.conftest import get_os_version
 
+if is_macos:
+    from photoscript import Photo
+    from osxphotos.cli.import_cli import import_cli
+else:
+    pytest.skip(allow_module_level=True)
+
 TERMINAL_WIDTH = 250
 
 TEST_IMAGES_DIR = "tests/test-images"
 TEST_IMAGE_1 = "tests/test-images/IMG_4179.jpeg"
 TEST_IMAGE_2 = "tests/test-images/faceinfo/exif1.jpg"
 TEST_IMAGE_NO_EXIF = "tests/test-images/IMG_NO_EXIF.jpeg"
 TEST_VIDEO_1 = "tests/test-images/Jellyfish.mov"
```

### Comparing `osxphotos-0.59.3/tests/test_cli_orphans.py` & `osxphotos-0.60.0/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_param_types.py` & `osxphotos-0.60.0/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_sync.py` & `osxphotos-0.60.0/tests/test_cli_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Test osxphotos sync command"""
 
 import os
 import json
-import photoscript
 import pytest
 from click.testing import CliRunner
 
-from osxphotos.cli.sync import sync
+from osxphotos.utils import is_macos
+if is_macos:
+    import photoscript
+    from osxphotos.cli.sync import sync
+else:
+    pytest.skip(allow_module_level=True)
 
 UUID_TEST_PHOTO_1 = "D79B8D77-BFFC-460B-9312-034F2877D35B"  # Pumkins2.jpg
 UUID_TEST_PHOTO_2 = "E9BC5C36-7CD1-40A1-A72B-8B8FAC227D51"  # wedding.jpg
 
 TEST_ALBUM_NAME = "SyncTestAlbum"
```

### Comparing `osxphotos-0.59.3/tests/test_cli_timewarp.py` & `osxphotos-0.60.0/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_utils.py` & `osxphotos-0.60.0/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cli_verbose.py` & `osxphotos-0.60.0/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.0/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_comments.py` & `osxphotos-0.60.0/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_concurrent_export.py` & `osxphotos-0.60.0/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_configoptions.py` & `osxphotos-0.60.0/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_datetime_formatter.py` & `osxphotos-0.60.0/tests/test_datetime_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """ test datetime_formatter.DateTimeFormatter """
 import pytest
 
+from .locale_util import setlocale
+
 
 def test_datetime_formatter_1():
     """Test DateTimeFormatter """
     import datetime
     import locale
     from osxphotos.datetime_formatter import DateTimeFormatter
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     dt = datetime.datetime(2020, 5, 23, 12, 42, 33)
     dtf = DateTimeFormatter(dt)
 
     assert dtf.date == "2020-05-23"
     assert dtf.year == "2020"
     assert dtf.yy == "20"
@@ -28,15 +30,15 @@
 
 def test_datetime_formatter_2():
     """Test DateTimeFormatter with hour > 12 """
     import datetime
     import locale
     from osxphotos.datetime_formatter import DateTimeFormatter
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     dt = datetime.datetime(2020, 5, 23, 14, 42, 33)
     dtf = DateTimeFormatter(dt)
 
     assert dtf.date == "2020-05-23"
     assert dtf.year == "2020"
     assert dtf.yy == "20"
@@ -52,15 +54,15 @@
 
 def test_datetime_formatter_3():
     """Test DateTimeFormatter zero-padding  """
     import datetime
     import locale
     from osxphotos.datetime_formatter import DateTimeFormatter
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
 
     dt = datetime.datetime(2020, 5, 2, 9, 3, 6)
     dtf = DateTimeFormatter(dt)
 
     assert dtf.date == "2020-05-02"
     assert dtf.year == "2020"
     assert dtf.yy == "20"
```

### Comparing `osxphotos-0.59.3/tests/test_datetime_utils.py` & `osxphotos-0.60.0/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_debug.py` & `osxphotos-0.60.0/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_empty_library_4_0.py` & `osxphotos-0.60.0/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_exif_info.py` & `osxphotos-0.60.0/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_exiftool.py` & `osxphotos-0.60.0/tests/test_exiftool.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,21 +534,21 @@
 
     import osxphotos.exiftool
 
     exif1 = osxphotos.exiftool.ExifTool(TEST_FILE_ONE_KEYWORD)
 
     ps = subprocess.run(["ps"], capture_output=True)
     stdout = ps.stdout.decode("utf-8")
-    assert "exiftool -stay_open" in stdout
+    assert "exiftool" in stdout
 
     osxphotos.exiftool.terminate_exiftool()
 
     ps = subprocess.run(["ps"], capture_output=True)
     stdout = ps.stdout.decode("utf-8")
-    assert "exiftool -stay_open" not in stdout
+    assert "exiftool" not in stdout
 
     # verify we can create a new instance after termination
     exif2 = osxphotos.exiftool.ExifTool(TEST_FILE_ONE_KEYWORD)
     assert exif2.asdict()["IPTC:Keywords"] == "wedding"
 
 
 def test_unescape_str():
```

### Comparing `osxphotos-0.59.3/tests/test_exiftool_caching.py` & `osxphotos-0.60.0/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.0/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.0/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import pytest
 
 from osxphotos._constants import _UNKNOWN_PERSON
-from osxphotos.utils import get_macos_version
+from osxphotos.utils import is_macos, get_macos_version
 
-OS_VERSION = get_macos_version()
+OS_VERSION = get_macos_version() if is_macos else (None, None, None)
 SKIP_TEST = "OSXPHOTOS_TEST_EXPORT" not in os.environ or OS_VERSION[1] != "15"
 PHOTOS_DB = os.path.expanduser("~/Pictures/Photos Library.photoslibrary")
 pytestmark = pytest.mark.skipif(
     SKIP_TEST, reason="These tests only run against system photos library"
 )
 
 UUID_DICT = {
```

### Comparing `osxphotos-0.59.3/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.0/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_export_db.py` & `osxphotos-0.60.0/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.0/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.0/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_exportresults.py` & `osxphotos-0.60.0/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_faceinfo.py` & `osxphotos-0.60.0/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_fileutil.py` & `osxphotos-0.60.0/tests/test_fileutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,20 @@
     import os.path
     import tempfile
 
     from osxphotos.fileutil import FileUtil
 
     temp_dir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     src = "tests/test-images/wedding.jpg"
+    src2 = os.path.join(temp_dir.name, "wedding_src.jpg")
     dest = os.path.join(temp_dir.name, "wedding.jpg")
-    FileUtil.hardlink(src, dest)
+    FileUtil.copy(src, src2)
+    FileUtil.hardlink(src2, dest)
     assert os.path.isfile(dest)
-    assert os.path.samefile(src, dest)
+    assert os.path.samefile(src2, dest)
 
 
 def test_unlink_file():
     import os.path
     import tempfile
 
     from osxphotos.fileutil import FileUtil
```

### Comparing `osxphotos-0.59.3/tests/test_highsierra.py` & `osxphotos-0.60.0/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_image_converter.py` & `osxphotos-0.60.0/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.0/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.0/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.0/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.0/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.0/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.0/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.0/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.0/tests/test_mojave_10_14_6.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Test basic methods for Mojave 10.14.6 """
 
 import datetime
 from collections import namedtuple
 
 import pytest
 
+import osxphotos
 from osxphotos._constants import _UNKNOWN_PERSON
 
 PHOTOS_DB = "./tests/Test-10.14.6.photoslibrary/database/photos.db"
 PHOTOS_DB_PATH = "/Test-10.14.6.photoslibrary/database/photos.db"
 PHOTOS_LIBRARY_PATH = "/Test-10.14.6.photoslibrary"
 
 KEYWORDS = [
@@ -527,17 +528,18 @@
     ignore_keys = ["_tmp_db", "_tempdir", "_tempdir_name", "_db_connection"]
     assert {k: v for k, v in photosdb.__dict__.items() if k not in ignore_keys} == {
         k: v for k, v in photosdb2.__dict__.items() if k not in ignore_keys
     }
 
 
 def test_photosinfo_repr():
-    import osxphotos
     import datetime  # needed for eval to work
 
+    import osxphotos
+
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["favorite"]])
     photo = photos[0]
     photo2 = eval(repr(photo))
 
     assert {k: str(v).encode("utf-8") for k, v in photo.__dict__.items()} == {
         k: str(v).encode("utf-8") for k, v in photo2.__dict__.items()
@@ -685,7 +687,14 @@
 
 
 def test_fingerprint(photosdb):
     """Test fingerprint"""
     for uuid, fingerprint in UUID_FINGERPRINT.items():
         photo = photosdb.get_photo(uuid)
         assert photo.fingerprint == fingerprint
+
+
+def test_tables(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.tables"""
+    photo = photosdb.get_photo(UUID_DICT["favorite"])
+    tables = photo.tables()
+    assert tables is None
```

### Comparing `osxphotos-0.59.3/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.0/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.0/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.0/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from collections import Counter, namedtuple
 
 import pytest
 
 import osxphotos
 from osxphotos._constants import _UNKNOWN_PERSON
 from osxphotos.photoexporter import PhotoExporter
-from osxphotos.utils import get_macos_version
+from osxphotos.utils import is_macos, get_macos_version
 
-OS_VERSION = get_macos_version()
+OS_VERSION = get_macos_version() if is_macos else (None, None, None)
 # SKIP_TEST = "OSXPHOTOS_TEST_EXPORT" not in os.environ or OS_VERSION[1] != "17"
 SKIP_TEST = True  # don't run any of the local library tests
 PHOTOS_DB_LOCAL = os.path.expanduser("~/Pictures/Photos Library.photoslibrary")
 
 PHOTOS_DB = "tests/Test-12.0.0.dev-beta.photoslibrary/database/photos.db"
 PHOTOS_DB_PATH = "/Test-12.0.0.dev-beta.photoslibrary/database/photos.db"
 PHOTOS_LIBRARY_PATH = "/Test-12.0.0.dev-beta.photoslibrary"
```

### Comparing `osxphotos-0.59.3/tests/test_movies_4_0.py` & `osxphotos-0.60.0/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_movies_5_0.py` & `osxphotos-0.60.0/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_path_utils.py` & `osxphotos-0.60.0/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_personinfo.py` & `osxphotos-0.60.0/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_photokit.py` & `osxphotos-0.60.0/tests/test_photokit.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 import os
 import pathlib
 import tempfile
 
 import pytest
 
-from osxphotos.photokit import (
-    LivePhotoAsset,
-    PhotoAsset,
-    PhotoLibrary,
-    VideoAsset,
-    PHOTOS_VERSION_CURRENT,
-    PHOTOS_VERSION_ORIGINAL,
-    PHOTOS_VERSION_UNADJUSTED,
-)
+from osxphotos.utils import is_macos
+if is_macos:
+    from osxphotos.photokit import (
+        LivePhotoAsset,
+        PhotoAsset,
+        PhotoLibrary,
+        VideoAsset,
+        PHOTOS_VERSION_CURRENT,
+        PHOTOS_VERSION_ORIGINAL,
+        PHOTOS_VERSION_UNADJUSTED,
+    )
+else:
+    pytest.skip(allow_module_level=True)
 
 skip_test = "OSXPHOTOS_TEST_EXPORT" not in os.environ
 pytestmark = pytest.mark.skipif(
     skip_test, reason="Skip if not running with author's personal library."
 )
```

### Comparing `osxphotos-0.59.3/tests/test_photosdb_utils.py` & `osxphotos-0.60.0/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_placeinfo.py` & `osxphotos-0.60.0/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.0/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.0/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.0/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_projects_catalina.py` & `osxphotos-0.60.0/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_projects_sierra.py` & `osxphotos-0.60.0/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_score_info.py` & `osxphotos-0.60.0/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.0/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.0/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.0/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.0/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.0/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.0/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_sidecar_xmp.py` & `osxphotos-0.60.0/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.0/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.0/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.0/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.0/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_sqlitekvstore.py` & `osxphotos-0.60.0/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_template.py` & `osxphotos-0.60.0/tests/test_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     PUNCTUATION,
     TEMPLATE_SUBSTITUTIONS,
     TEMPLATE_SUBSTITUTIONS_MULTI_VALUED,
     PhotoTemplate,
     RenderOptions,
 )
 from osxphotos.photoinfo import PhotoInfoNone
+from osxphotos.utils import is_macos
 from .photoinfo_mock import PhotoInfoMock
+from .locale_util import setlocale
 
 try:
     exiftool = get_exiftool_path()
 except:
     exiftool = None
 
 PHOTOS_DB_PLACES = (
@@ -545,79 +547,84 @@
     photo = photosdb_places.photos(uuid=[UUID_DICT["place_dc"]])[0]
     template = PhotoTemplate(photo)
 
     for subst in TEMPLATE_SUBSTITUTIONS_MULTI_VALUED:
         lookup_str = re.match(r"\{([^\\,}]+)\}", subst).group(1)
         if subst in ["{exiftool}", "{photo}", "{function}", "{format}"]:
             continue
+        if subst == "{detected_text}" and not is_macos:
+            continue
         lookup = template.get_template_value_multi(
             lookup_str,
             path_sep=os.path.sep,
             default=[],
             subfield=None,
         )
         assert isinstance(lookup, list)
 
 
 def test_subst(photosdb_places):
     """Test that substitutions are correct"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb_places.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     for template in TEMPLATE_VALUES:
         rendered, _ = photo.render_template(template)
         assert rendered[0] == TEMPLATE_VALUES[template]
 
 
 def test_subst_date_modified(photosdb_places):
     """Test that substitutions are correct for date modified"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb_places.photos(uuid=[UUID_DICT["date_modified"]])[0]
 
     for template in TEMPLATE_VALUES_DATE_MODIFIED:
         rendered, _ = photo.render_template(template)
         assert rendered[0] == TEMPLATE_VALUES_DATE_MODIFIED[template]
 
 
 def test_subst_date_not_modified(photosdb_places):
     """Test that substitutions are correct for date modified when photo isn't modified"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb_places.photos(uuid=[UUID_DICT["date_not_modified"]])[0]
 
     for template in TEMPLATE_VALUES_DATE_NOT_MODIFIED:
         rendered, _ = photo.render_template(template)
         assert rendered[0] == TEMPLATE_VALUES_DATE_NOT_MODIFIED[template]
 
 
 def test_subst_locale_1(photosdb_places):
     """Test that substitutions are correct in user locale"""
     import locale
 
     # osxphotos.template sets local on load so set the environment first
     # set locale to DE
-    locale.setlocale(locale.LC_ALL, "de_DE.UTF-8")
+    setlocale(locale.LC_ALL, "de_DE.UTF-8")
 
     photo = photosdb_places.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     for template in TEMPLATE_VALUES_DEU:
         rendered, _ = photo.render_template(template)
         assert rendered[0] == TEMPLATE_VALUES_DEU[template]
 
 
 def test_subst_locale_2(photosdb_places):
     """Test that substitutions are correct in user locale"""
     import locale
     import os
 
+    # Check if locale is available
+    setlocale(locale.LC_ALL, "de_DE.UTF-8")
+
     # osxphotos.template sets local on load so set the environment first
     os.environ["LANG"] = "de_DE.UTF-8"
     os.environ["LC_COLLATE"] = "de_DE.UTF-8"
     os.environ["LC_CTYPE"] = "de_DE.UTF-8"
     os.environ["LC_MESSAGES"] = "de_DE.UTF-8"
     os.environ["LC_MONETARY"] = "de_DE.UTF-8"
     os.environ["LC_NUMERIC"] = "de_DE.UTF-8"
@@ -630,39 +637,39 @@
         assert rendered[0] == TEMPLATE_VALUES_DEU[template]
 
 
 def test_subst_default_val(photosdb_places):
     """Test substitution with default value specified"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb_places.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     template = "{place.name.area_of_interest,UNKNOWN}"
     rendered, _ = photo.render_template(template)
     assert rendered[0] == "UNKNOWN"
 
 
 def test_subst_default_val_2(photosdb_places):
     """Test substitution with ',' but no default value"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb_places.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     template = "{place.name.area_of_interest,}"
     rendered, _ = photo.render_template(template)
     assert rendered[0] == ""
 
 
 def test_subst_unknown_val(photosdb_places):
     """Test substitution with unknown value specified"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb_places.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     template = "{created.year}/{foo}"
     rendered, unknown = photo.render_template(template)
     # assert rendered[0] == "2020/{foo}"
     assert unknown == ["foo"]
 
@@ -678,15 +685,15 @@
 #     assert not unknown
 
 
 def test_subst_unknown_val_with_default(photosdb_places):
     """Test substitution with unknown value specified"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb_places.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     template = "{created.year}/{foo,bar}"
     rendered, unknown = photo.render_template(template)
     # assert rendered[0] == "2020/{foo,bar}"
     assert unknown == ["foo"]
 
@@ -925,15 +932,15 @@
     assert unknown == []
 
 
 def test_subst_strftime(photosdb_places):
     """Test that strftime substitutions are correct"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb_places.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     rendered, unmatched = photo.render_template("{created.strftime,%Y-%m-%d-%H%M%S}")
     assert rendered[0] == "2020-02-04-190738"
 
     rendered, unmatched = photo.render_template("{created.strftime}")
     assert rendered[0] == "_"
@@ -1283,14 +1290,15 @@
         album = UUID_ALBUM_SEQ[uuid]["album"]
         options = RenderOptions(dest_path=album)
         for template, value in UUID_ALBUM_SEQ[uuid]["templates"].items():
             rendered, _ = photo.render_template(template, options=options)
             assert rendered[0] == value
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_detected_text(photosdb):
     """Test {detected_text} template"""
     photo = photosdb.get_photo(UUID_DETECTED_TEXT)
     for template, value in TEMPLATE_VALUES_DETECTED_TEXT.items():
         rendered, _ = photo.render_template(template)
         assert value in "".join(rendered)
```

### Comparing `osxphotos-0.59.3/tests/test_template_counter.py` & `osxphotos-0.60.0/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_template_today.py` & `osxphotos-0.60.0/tests/test_template_today.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
 
 import pytest
 
 import osxphotos
 from osxphotos.phototemplate import RenderOptions
 
+from .locale_util import setlocale
+
 PHOTOS_DB_PLACES = (
     "./tests/Test-Places-Catalina-10_15_1.photoslibrary/database/photos.db"
 )
 
 DATETIME_TODAY = datetime.datetime(2020, 6, 21, 13, 0, 0)
 """ Used to patch osxphotos.phototemplate.TODAY for testing """
 
@@ -44,15 +46,15 @@
     return osxphotos.PhotosDB(dbfile=PHOTOS_DB_PLACES)
 
 
 def test_subst_today(photosdb):
     """Test that substitutions are correct for {today.x}"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     photo_template = osxphotos.PhotoTemplate(photo)
     photo_template.today = DATETIME_TODAY
 
     options = RenderOptions()
     for template in TODAY_VALUES:
@@ -60,15 +62,15 @@
         assert rendered[0] == TODAY_VALUES[template]
 
 
 def test_subst_strftime_today(photosdb):
     """Test that strftime substitutions are correct for {today.strftime}"""
     import locale
 
-    locale.setlocale(locale.LC_ALL, "en_US")
+    setlocale(locale.LC_ALL, "en_US")
     photo = photosdb.photos(uuid=[UUID_DICT["place_dc"]])[0]
 
     photo_template = osxphotos.PhotoTemplate(photo)
     photo_template.today = DATETIME_TODAY
     options = RenderOptions()
     rendered, unmatched = photo_template.render(
         "{today.strftime,%Y-%m-%d-%H%M%S}", options
```

### Comparing `osxphotos-0.59.3/tests/test_uti.py` & `osxphotos-0.60.0/tests/test_uti.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import osxphotos.uti
 from osxphotos.uti import (
     _get_uti_from_mdls,
     get_preferred_uti_extension,
     get_uti_for_extension,
 )
+from osxphotos.utils import is_macos
 
 EXT_DICT = {"heic": "public.heic", "jpg": "public.jpeg", ".jpg": "public.jpeg"}
 UTI_DICT = {"public.heic": "heic", "public.jpeg": "jpeg"}
 
 
 def test_get_preferred_uti_extension():
     """test get_preferred_uti_extension"""
@@ -39,20 +40,22 @@
     OLD_VER = osxphotos.uti.OS_VER
     osxphotos.uti.OS_VER = 12
     for ext in EXT_DICT:
         assert get_uti_for_extension(ext) == EXT_DICT[ext]
     osxphotos.uti.OS_VER = OLD_VER
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_get_uti_from_mdls():
     """get _get_uti_from_mdls"""
     for ext in EXT_DICT:
         assert _get_uti_from_mdls(ext) == EXT_DICT[ext]
 
 
+@pytest.mark.skipif(not is_macos, reason="Only works on macOS")
 def test_get_uti_not_in_dict():
     """get UTI when objc is not available and it's not in the EXT_UTI_DICT"""
     # monkey patch the EXT_UTI_DICT
     OLD_VER = osxphotos.uti.OS_VER
     osxphotos.uti.OS_VER = 12
     osxphotos.uti.EXT_UTI_DICT = {}
     osxphotos.uti.UTI_EXT_DICT = {}
```

### Comparing `osxphotos-0.59.3/tests/test_utils.py` & `osxphotos-0.60.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.3/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.0/tests/test_ventura_13_0_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1300,7 +1300,18 @@
 
 def test_photosdb_photos_by_uuid(photosdb: osxphotos.PhotosDB):
     """Test PhotosDB.photos_by_uuid"""
     photos = photosdb.photos_by_uuid(UUID_DICT.values())
     assert len(photos) == len(UUID_DICT)
     for photo in photos:
         assert photo.uuid in UUID_DICT.values()
+
+
+def test_tables(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.tables"""
+    photo = photosdb.get_photo(UUID_DICT["in_album"])
+    tables = photo.tables()
+    assert isinstance(tables, osxphotos.PhotoTables)
+    assert tables.ZASSET.ZUUID[0] == photo.uuid
+    assert tables.ZADDITIONALASSETATTRIBUTES.ZTITLE[0] == photo.title
+    assert len(tables.ZASSET.rows()) == 1
+    assert tables.ZASSET.rows_dict()[0]["ZUUID"] == photo.uuid
```

### Comparing `osxphotos-0.59.3/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.0/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

