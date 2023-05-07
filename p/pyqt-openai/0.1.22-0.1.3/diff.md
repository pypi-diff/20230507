# Comparing `tmp/pyqt-openai-0.1.22.tar.gz` & `tmp/pyqt-openai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-openai-0.1.22.tar", last modified: Sat May  6 01:35:17 2023, max compression
+gzip compressed data, was "pyqt-openai-0.1.3.tar", last modified: Sun May  7 05:05:13 2023, max compression
```

## Comparing `pyqt-openai-0.1.22.tar` & `pyqt-openai-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.406271 pyqt-openai-0.1.22/
--rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.22/LICENSE
--rw-rw-rw-   0        0        0     5482 2023-05-06 01:35:17.405270 pyqt-openai-0.1.22/PKG-INFO
--rw-rw-rw-   0        0        0     5082 2023-05-06 01:32:51.000000 pyqt-openai-0.1.22/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.303224 pyqt-openai-0.1.22/pyqt_openai/
--rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/__init__.py
--rw-rw-rw-   0        0        0     6738 2023-04-09 06:45:06.000000 pyqt-openai-0.1.22/pyqt_openai/a.py
--rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/apiData.py
--rw-rw-rw-   0        0        0     6771 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/chatWidget.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.22/pyqt_openai/circleProfileImage.py
--rw-rw-rw-   0        0        0     8132 2023-04-08 11:47:46.000000 pyqt-openai-0.1.22/pyqt_openai/clickableTooltip.py
--rw-rw-rw-   0        0        0     5072 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/convListWidget.py
--rw-rw-rw-   0        0        0     7627 2023-05-06 01:32:51.000000 pyqt-openai-0.1.22/pyqt_openai/customizeDialog.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.365059 pyqt-openai-0.1.22/pyqt_openai/ico/
--rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.22/pyqt_openai/ico/__init__.py
--rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/add.svg
--rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.22/pyqt_openai/ico/close.svg
--rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.22/pyqt_openai/ico/customize.svg
--rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/delete.svg
--rw-rw-rw-   0        0        0      654 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/download.svg
--rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/help.svg
--rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.22/pyqt_openai/ico/openai.svg
--rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/ico/prompt.svg
--rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/search.svg
--rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/setting.svg
--rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.22/pyqt_openai/ico/sidebar.svg
--rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.22/pyqt_openai/ico/stackontop.svg
--rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.22/pyqt_openai/ico/user.svg
--rw-rw-rw-   0        0        0     1383 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/inputDialog.py
--rw-rw-rw-   0        0        0     3768 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/leftSideBar.py
--rw-rw-rw-   0        0        0    22532 2023-05-06 01:32:51.000000 pyqt-openai-0.1.22/pyqt_openai/main.py
--rw-rw-rw-   0        0        0     1788 2023-04-08 11:47:46.000000 pyqt-openai-0.1.22/pyqt_openai/modelTable.py
--rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.22/pyqt_openai/notifier.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.374035 pyqt-openai-0.1.22/pyqt_openai/prompt/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/prompt/__init__.py
--rw-rw-rw-   0        0        0     1721 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/prompt/promptGeneratorWidget.py
--rw-rw-rw-   0        0        0     1574 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/prompt/propPage.py
--rw-rw-rw-   0        0        0     3351 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/prompt/templatePage.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.386317 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/
--rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/__init__.py
--rw-rw-rw-   0        0        0     2220 2023-05-05 02:57:06.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
--rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/chatPage.py
--rw-rw-rw-   0        0        0    11101 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/completionPage.py
--rw-rw-rw-   0        0        0     1623 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/imagePage.py
--rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/searchBar.py
--rw-rw-rw-   0        0        0    21685 2023-05-06 01:32:51.000000 pyqt-openai-0.1.22/pyqt_openai/sqlite.py
--rw-rw-rw-   0        0        0     5931 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/svgButton.py
--rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.22/pyqt_openai/svgLabel.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.393302 pyqt-openai-0.1.22/pyqt_openai/test/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/test/__init__.py
--rw-rw-rw-   0        0        0     1425 2023-05-06 00:44:23.000000 pyqt-openai-0.1.22/pyqt_openai/test/dialog.py
--rw-rw-rw-   0        0        0     1773 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/test/htmlformat.py
--rw-rw-rw-   0        0        0     1280 2023-04-23 09:02:45.000000 pyqt-openai-0.1.22/pyqt_openai/test/rightSideBarTab.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.403276 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/
--rw-rw-rw-   0        0        0        0 2023-05-05 07:22:12.000000 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/__init__.py
--rw-rw-rw-   0        0        0      722 2023-05-05 12:31:35.000000 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/delete_model.py
--rw-rw-rw-   0        0        0     2559 2023-05-05 07:22:36.000000 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/make_model.py
--rw-rw-rw-   0        0        0      433 2023-05-05 08:36:36.000000 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/using_model.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.336141 pyqt-openai-0.1.22/pyqt_openai.egg-info/
--rw-rw-rw-   0        0        0     5482 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1683 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 01:35:17.406271 pyqt-openai-0.1.22/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-05-06 01:33:10.000000 pyqt-openai-0.1.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.863436 pyqt-openai-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5704 2023-05-07 05:05:13.862442 pyqt-openai-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5301 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.658283 pyqt-openai-0.1.3/pyqt_openai/
+-rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/__init__.py
+-rw-rw-rw-   0        0        0     6738 2023-04-09 06:45:06.000000 pyqt-openai-0.1.3/pyqt_openai/a.py
+-rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/apiData.py
+-rw-rw-rw-   0        0        0    10282 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/chatWidget.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.3/pyqt_openai/circleProfileImage.py
+-rw-rw-rw-   0        0        0     8132 2023-04-08 11:47:46.000000 pyqt-openai-0.1.3/pyqt_openai/clickableTooltip.py
+-rw-rw-rw-   0        0        0     5072 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/convListWidget.py
+-rw-rw-rw-   0        0        0     7627 2023-05-07 04:26:44.000000 pyqt-openai-0.1.3/pyqt_openai/customizeDialog.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.733666 pyqt-openai-0.1.3/pyqt_openai/ico/
+-rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.3/pyqt_openai/ico/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/add.svg
+-rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.3/pyqt_openai/ico/close.svg
+-rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.3/pyqt_openai/ico/customize.svg
+-rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/delete.svg
+-rw-rw-rw-   0        0        0      654 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/download.svg
+-rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/help.svg
+-rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.3/pyqt_openai/ico/openai.svg
+-rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/ico/prompt.svg
+-rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/search.svg
+-rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/ico/setting.svg
+-rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.3/pyqt_openai/ico/sidebar.svg
+-rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.3/pyqt_openai/ico/stackontop.svg
+-rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.3/pyqt_openai/ico/user.svg
+-rw-rw-rw-   0        0        0      432 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/ico/vertical_three_dots.svg
+-rw-rw-rw-   0        0        0     1383 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/inputDialog.py
+-rw-rw-rw-   0        0        0     3768 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/leftSideBar.py
+-rw-rw-rw-   0        0        0    22457 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/main.py
+-rw-rw-rw-   0        0        0     1788 2023-04-08 11:47:46.000000 pyqt-openai-0.1.3/pyqt_openai/modelTable.py
+-rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.3/pyqt_openai/notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.747629 pyqt-openai-0.1.3/pyqt_openai/prompt/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/prompt/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/prompt/promptGeneratorWidget.py
+-rw-rw-rw-   0        0        0     3775 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/prompt/propPage.py
+-rw-rw-rw-   0        0        0     4819 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/prompt/templatePage.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.793373 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/
+-rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/__init__.py
+-rw-rw-rw-   0        0        0     2220 2023-05-05 02:57:06.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
+-rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/chatPage.py
+-rw-rw-rw-   0        0        0    11101 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/completionPage.py
+-rw-rw-rw-   0        0        0     1623 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/right_sidebar/imagePage.py
+-rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/searchBar.py
+-rw-rw-rw-   0        0        0    21685 2023-05-07 04:26:44.000000 pyqt-openai-0.1.3/pyqt_openai/sqlite.py
+-rw-rw-rw-   0        0        0     5931 2023-04-22 00:05:31.000000 pyqt-openai-0.1.3/pyqt_openai/svgButton.py
+-rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.3/pyqt_openai/svgLabel.py
+-rw-rw-rw-   0        0        0     5935 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/pyqt_openai/svgToolButton.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.813564 pyqt-openai-0.1.3/pyqt_openai/test/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/test/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-05-05 02:56:55.000000 pyqt-openai-0.1.3/pyqt_openai/test/htmlformat.py
+-rw-rw-rw-   0        0        0     4417 2023-05-07 03:48:58.000000 pyqt-openai-0.1.3/pyqt_openai/test/prompt_autocomplete.py
+-rw-rw-rw-   0        0        0     1280 2023-04-23 09:02:45.000000 pyqt-openai-0.1.3/pyqt_openai/test/rightSideBarTab.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.859468 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/
+-rw-rw-rw-   0        0        0        0 2023-05-05 07:22:12.000000 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-05-05 12:31:35.000000 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/delete_model.py
+-rw-rw-rw-   0        0        0     2559 2023-05-05 07:22:36.000000 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/make_model.py
+-rw-rw-rw-   0        0        0      433 2023-05-05 08:36:36.000000 pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/using_model.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:05:13.697797 pyqt-openai-0.1.3/pyqt_openai.egg-info/
+-rw-rw-rw-   0        0        0     5704 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1765 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-07 05:05:13.000000 pyqt-openai-0.1.3/pyqt_openai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 05:05:13.863436 pyqt-openai-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1131 2023-05-07 05:04:02.000000 pyqt-openai-0.1.3/setup.py
```

### Comparing `pyqt-openai-0.1.22/LICENSE` & `pyqt-openai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/PKG-INFO` & `pyqt-openai-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.22
+Version: 0.1.3
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -49,43 +49,47 @@
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator
+* support prompt generator (manageable)
+* support beginning and ending part of the prompt
 * support image generation with DALL-E
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 
 ## Preview
-This is using GPT-3.5 turbo model by default.
+This is using GPT-3.5 turbo model by default. 
 
 ### Homepage
-![image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-b78ab8a1eb73.png)
+![image](https://user-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-b45401f8bb7c.png)
 <b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
 
 ### Overview
-![image](https://user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-e502a182264d.png)
+![image](https://user-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-4630010edd5b.png)
 
 ### Conversation preview
 #### Preview Image
 ![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
 #### Preview Video
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 
 ### Prompt Generator
+#### Preview 1 (v0.1.22)
 https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
+#### Preview 2 (v0.1.3)
+https://user-images.githubusercontent.com/55078043/236658468-9947a417-99b3-4e44-8849-a676308a0239.mp4
 
 So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
 
 ## How to play
 1. git clone ~
 2. from the root directory, type "cd pyqt_openai"
 3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.22 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.3 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot. Even though this
@@ -20,42 +20,45 @@
 software. It's not necessary to run this app (obviously), but it's good
 practice to manage database about conversation history with AI and to know how
 this works. ## Feature * basically this is desktop application version of
 ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
 past conversation * conversation management * add & delete conversations * save
 conversations * rename conversation * everything above is saved in an SQLite
 database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator * support image generation with DALL-E * you can run
-this in background application * notification will pop up when response is
-generated * you can make window stack on top or control its transparency ##
-Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
-using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-
-b78ab8a1eb73.png) You have to write your openai api key inside the red box. see
+* support prompt generator (manageable) * support beginning and ending part of
+the prompt * support image generation with DALL-E * you can run this in
+background application * notification will pop up when response is generated *
+you can make window stack on top or control its transparency ## Requirements *
+qtpy - the package allowing you to write code that works with both PyQt and
+PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is using GPT-3.5
+turbo model by default. ### Homepage ![image](https://user-
+images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-
+b45401f8bb7c.png) You have to write your openai api key inside the red box. see
 [How to play](#how-to-play) ### Overview ![image](https://user-
-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
-e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
+images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-
+4630010edd5b.png) ### Conversation preview #### Preview Image ![image](https://
 user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
 7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator https://user-images.githubusercontent.com/55078043/236584481-
-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
-lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
-~ 2. from the root directory, type "cd pyqt_openai" 3. You should put your api
-key in the line edit. You can get it in official_site of openai. Sign up and
-log in before you get it. By the way, this is free trial, not permanently free.
-See this after you have logged in. Be sure, this is a very important API key
-that belongs to you only, so you should remember it and keep it secure. 4.
-python main.py If installation doesn't work, check the troubleshooting below.
-## Troubleshooting If you see this error while installing the openai package
-``` subprocess-exited-with-error ``` you can shout a curse word and just
-download the package itself from pypi. Unzip it, access the package directory,
-type ``` python setup.py install ``` That will install the openai. ## TODO list
-* support Stable Diffusion * show the explanation of every model and terms
+Generator #### Preview 1 (v0.1.22) https://user-images.githubusercontent.com/
+55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 #### Preview 2
+(v0.1.3) https://user-images.githubusercontent.com/55078043/236658468-9947a417-
+99b3-4e44-8849-a676308a0239.mp4 So sorry to weak preview, but i have a lot of
+idea about this prompt generator! Just wait. ## How to play 1. git clone ~ 2.
+from the root directory, type "cd pyqt_openai" 3. You should put your api key
+in the line edit. You can get it in official_site of openai. Sign up and log in
+before you get it. By the way, this is free trial, not permanently free. See
+this after you have logged in. Be sure, this is a very important API key that
+belongs to you only, so you should remember it and keep it secure. 4. python
+main.py If installation doesn't work, check the troubleshooting below. ##
+Troubleshooting If you see this error while installing the openai package ```
+subprocess-exited-with-error ``` you can shout a curse word and just download
+the package itself from pypi. Unzip it, access the package directory, type ```
+python setup.py install ``` That will install the openai. ## TODO list *
+support Stable Diffusion * show the explanation of every model and terms
 related to AI (e.g. temperature, topp..) * save conversation history with other
 format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
 eventually) * support multiple language * use SQLAlchemy (maybe not) * show
 reason when the chat input is disabled for some reasons * add the basic example
 sources of making deep learning model with PyTorch (eventually) ## See Also *
 Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
 it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.22/README.md` & `pyqt-openai-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,43 +37,47 @@
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator
+* support prompt generator (manageable)
+* support beginning and ending part of the prompt
 * support image generation with DALL-E
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 
 ## Preview
-This is using GPT-3.5 turbo model by default.
+This is using GPT-3.5 turbo model by default. 
 
 ### Homepage
-![image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-b78ab8a1eb73.png)
+![image](https://user-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-b45401f8bb7c.png)
 <b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
 
 ### Overview
-![image](https://user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-e502a182264d.png)
+![image](https://user-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-4630010edd5b.png)
 
 ### Conversation preview
 #### Preview Image
 ![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
 #### Preview Video
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 
 ### Prompt Generator
+#### Preview 1 (v0.1.22)
 https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
+#### Preview 2 (v0.1.3)
+https://user-images.githubusercontent.com/55078043/236658468-9947a417-99b3-4e44-8849-a676308a0239.mp4
 
 So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
 
 ## How to play
 1. git clone ~
 2. from the root directory, type "cd pyqt_openai"
 3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
```

#### html2text {}

```diff
@@ -17,42 +17,45 @@
 software. It's not necessary to run this app (obviously), but it's good
 practice to manage database about conversation history with AI and to know how
 this works. ## Feature * basically this is desktop application version of
 ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
 past conversation * conversation management * add & delete conversations * save
 conversations * rename conversation * everything above is saved in an SQLite
 database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator * support image generation with DALL-E * you can run
-this in background application * notification will pop up when response is
-generated * you can make window stack on top or control its transparency ##
-Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
-using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-
-b78ab8a1eb73.png) You have to write your openai api key inside the red box. see
+* support prompt generator (manageable) * support beginning and ending part of
+the prompt * support image generation with DALL-E * you can run this in
+background application * notification will pop up when response is generated *
+you can make window stack on top or control its transparency ## Requirements *
+qtpy - the package allowing you to write code that works with both PyQt and
+PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is using GPT-3.5
+turbo model by default. ### Homepage ![image](https://user-
+images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-
+b45401f8bb7c.png) You have to write your openai api key inside the red box. see
 [How to play](#how-to-play) ### Overview ![image](https://user-
-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
-e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
+images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-
+4630010edd5b.png) ### Conversation preview #### Preview Image ![image](https://
 user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
 7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator https://user-images.githubusercontent.com/55078043/236584481-
-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
-lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
-~ 2. from the root directory, type "cd pyqt_openai" 3. You should put your api
-key in the line edit. You can get it in official_site of openai. Sign up and
-log in before you get it. By the way, this is free trial, not permanently free.
-See this after you have logged in. Be sure, this is a very important API key
-that belongs to you only, so you should remember it and keep it secure. 4.
-python main.py If installation doesn't work, check the troubleshooting below.
-## Troubleshooting If you see this error while installing the openai package
-``` subprocess-exited-with-error ``` you can shout a curse word and just
-download the package itself from pypi. Unzip it, access the package directory,
-type ``` python setup.py install ``` That will install the openai. ## TODO list
-* support Stable Diffusion * show the explanation of every model and terms
+Generator #### Preview 1 (v0.1.22) https://user-images.githubusercontent.com/
+55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 #### Preview 2
+(v0.1.3) https://user-images.githubusercontent.com/55078043/236658468-9947a417-
+99b3-4e44-8849-a676308a0239.mp4 So sorry to weak preview, but i have a lot of
+idea about this prompt generator! Just wait. ## How to play 1. git clone ~ 2.
+from the root directory, type "cd pyqt_openai" 3. You should put your api key
+in the line edit. You can get it in official_site of openai. Sign up and log in
+before you get it. By the way, this is free trial, not permanently free. See
+this after you have logged in. Be sure, this is a very important API key that
+belongs to you only, so you should remember it and keep it secure. 4. python
+main.py If installation doesn't work, check the troubleshooting below. ##
+Troubleshooting If you see this error while installing the openai package ```
+subprocess-exited-with-error ``` you can shout a curse word and just download
+the package itself from pypi. Unzip it, access the package directory, type ```
+python setup.py install ``` That will install the openai. ## TODO list *
+support Stable Diffusion * show the explanation of every model and terms
 related to AI (e.g. temperature, topp..) * save conversation history with other
 format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
 eventually) * support multiple language * use SQLAlchemy (maybe not) * show
 reason when the chat input is disabled for some reasons * add the basic example
 sources of making deep learning model with PyTorch (eventually) ## See Also *
 Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
 it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.22/pyqt_openai/a.py` & `pyqt-openai-0.1.3/pyqt_openai/a.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/apiData.py` & `pyqt-openai-0.1.3/pyqt_openai/apiData.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/chatWidget.py` & `pyqt-openai-0.1.3/pyqt_openai/svgButton.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,203 +1,159 @@
-import json
-import os
+import os.path, posixpath
 
-import requests
+from qtpy.QtGui import QColor, QPalette, qGray
+from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QPushButton
 
-from qtpy.QtCore import Qt, Signal
-from qtpy.QtGui import QPixmap, QFont
-from qtpy.QtWidgets import QScrollArea, QVBoxLayout, QWidget, QLabel, QHBoxLayout, QTextEdit, QStackedWidget
 
-
-class ChatBrowser(QScrollArea):
-    convUnitUpdated = Signal(int, int, str)
-
-    def __init__(self):
-        super().__init__()
+class SvgButton(QPushButton):
+    def __init__(self, base_widget: QWidget = None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.__baseWidget = base_widget
         self.__initVal()
-        self.__initUi()
+        self.__styleInit()
 
     def __initVal(self):
-        self.__cur_id = 0
-
-    def __initUi(self):
-        self.__homeWidget = QLabel('Home')
-        self.__homeWidget.setAlignment(Qt.AlignCenter)
-        self.__homeWidget.setFont(QFont('Arial', 32))
-
-        lay = QVBoxLayout()
-        lay.setAlignment(Qt.AlignTop)
-        lay.setSpacing(0)
-        lay.setContentsMargins(0, 0, 0, 0)
-
-        self.__chatWidget = QWidget()
-        self.__chatWidget.setLayout(lay)
-
-        widget = QStackedWidget()
-        widget.addWidget(self.__homeWidget)
-        widget.addWidget(self.__chatWidget)
-        self.setWidget(widget)
-        self.setWidgetResizable(True)
-
-    def getChatWidget(self):
-        return self.__chatWidget
-
-    def showLabel(self, text, user_f, stream_f, image_f):
-        if image_f:
-            self.showImage(text, user_f)
+        # to set size accordance with scale
+        sc = qApp.screens()[0]
+        sc.logicalDotsPerInchChanged.connect(self.__scaleChanged)
+        self.__size = sc.logicalDotsPerInch() // 4
+        self.__padding = self.__border_radius = self.__size // 10
+        self.__background_color = 'transparent'
+        self.__icon = ''
+        self.__animation = ''
+        self.installEventFilter(self)
+        if self.__baseWidget:
+            self.__baseWidget.installEventFilter(self)
+            self.__initColorByBaseWidget()
         else:
-            self.showText(text, stream_f, user_f)
-        if not stream_f:
-            # change user_f type from bool to int to insert in db
-            self.convUnitUpdated.emit(self.__cur_id, int(user_f), text)
-
-    def streamFinished(self):
-        self.convUnitUpdated.emit(self.__cur_id, 0, self.getLastResponse())
-
-    def showImage(self, image_url, user_f):
-        chatLbl = QLabel()
-        response = requests.get(image_url)
-        pixmap = QPixmap()
-        pixmap.loadFromData(response.content)
-        pixmap = pixmap.scaled(chatLbl.width(), chatLbl.height())
-        chatLbl.setPixmap(pixmap)
-        chatLbl.setStyleSheet('QLabel { background-color: #DDD; padding: 1em }')
-        self.getChatWidget().layout().addWidget(chatLbl)
-
-    def showText(self, text, stream_f, user_f):
-        if self.widget().currentWidget() == self.__chatWidget:
-            pass
+            self.__hover_color = '#DDDDDD'
+            self.__pressed_color = '#FFFFFF'
+            self.__checked_color = '#CCCCCC'
+            self.__text_color = '#AAAAAA'
+
+    def __initColorByBaseWidget(self):
+        self.__base_color = self.__baseWidget.palette().color(QPalette.Base)
+        self.__hover_color = self.__getHoverColor(self.__base_color)
+        self.__pressed_color = self.__getPressedColor(self.__base_color)
+        self.__checked_color = self.__getPressedColor(self.__base_color)
+        self.__text_color = self.__getButtonTextColor(self.__base_color)
+
+    def __getColorByFactor(self, base_color, factor):
+        r, g, b = base_color.red(), base_color.green(), base_color.blue()
+        gray = qGray(r, g, b)
+        if gray > 255 // 2:
+            color = base_color.darker(factor)
         else:
-            self.widget().setCurrentIndex(1)
-        self.__setLabel(text, stream_f, user_f)
+            color = base_color.lighter(factor)
+        return color
 
-    def __setLabel(self, text, stream_f, user_f):
-        chatLbl = QLabel(text)
-        chatLbl.setWordWrap(True)
-        chatLbl.setTextInteractionFlags(Qt.TextSelectableByMouse)
-        if user_f:
-            chatLbl.setStyleSheet('QLabel { padding: 1em }')
-            chatLbl.setAlignment(Qt.AlignRight)
-        else:
-            if stream_f:
-                lbl = self.getChatWidget().layout().itemAt(self.getChatWidget().layout().count()-1).widget()
-                if isinstance(lbl, QLabel) and lbl.alignment() == Qt.AlignLeft:
-                    lbl.setText(lbl.text()+text)
-                    return
-            chatLbl.setStyleSheet('QLabel { background-color: #DDD; padding: 1em }')
-            chatLbl.setAlignment(Qt.AlignLeft)
-            chatLbl.setOpenExternalLinks(True)
-        self.getChatWidget().layout().addWidget(chatLbl)
-
-    def event(self, e):
-        if e.type() == 43:
-            self.verticalScrollBar().setSliderPosition(self.verticalScrollBar().maximum())
-        return super().event(e)
-
-    # TODO distinguish the image response
-    def getAllText(self):
-        all_text_lst = []
-        lay = self.getChatWidget().layout()
-        if lay:
-            for i in range(lay.count()):
-                if lay.itemAt(i) and lay.itemAt(i).widget():
-                    widget = lay.itemAt(i).widget()
-                    if isinstance(widget, QLabel):
-                        prefix = 'User' if i % 2 == 0 else 'AI'
-                        all_text_lst.append(f'{prefix}: {widget.text()}')
-
-        return '\n'.join(all_text_lst)
-
-    def getLastResponse(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            i = lay.count()-1
-            if lay.itemAt(i) and lay.itemAt(i).widget():
-                widget = lay.itemAt(i).widget()
-                if isinstance(widget, QLabel):
-                    return widget.text()
-        return ''
-
-    def getEveryResponse(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            text_lst = []
-            for i in range(lay.count()):
-                item = lay.itemAt(i)
-                if item and item.widget():
-                    widget = item.widget()
-                    if isinstance(widget, QLabel) and i % 2 == 1:
-                        text_lst.append(widget.text())
-            return '\n'.join(text_lst)
+    def __getHoverColor(self, base_color):
+        hover_factor = 120
+        hover_color = self.__getColorByFactor(base_color, hover_factor)
+        return hover_color.name()
+
+    def __getPressedColor(self, base_color):
+        pressed_factor = 130
+        pressed_color = self.__getColorByFactor(base_color, pressed_factor)
+        return pressed_color.name()
+
+    def __getCheckedColor(self, base_color):
+        return self.__getPressedColor(base_color)
+
+    def __getButtonTextColor(self, base_color):
+        r, g, b = base_color.red() ^ 255, base_color.green() ^ 255, base_color.blue() ^ 255
+        if r == g == b:
+            text_color = QColor(r, g, b)
         else:
-            return ''
-
-    def clear(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            for i in range(lay.count()-1, -1, -1):
-                item = lay.itemAt(i)
-                if item and item.widget():
-                    lay.removeWidget(item.widget())
-        self.widget().setCurrentIndex(0)
-
-    def isNew(self):
-        return self.widget().currentIndex() == 0
-
-    def setCurId(self, id):
-        self.__cur_id = id
-
-    def resetChatWidget(self, id):
-        self.clear()
-        self.setCurId(id)
-
-    def replaceConv(self, id, conv_data):
-        self.clear()
-        self.setCurId(id)
-        self.widget().setCurrentIndex(1)
-        for i in range(len(conv_data)):
-            self.__setLabel(conv_data[i], False, not bool(i % 2))
-
-
-class TextEditPrompt(QTextEdit):
-    returnPressed = Signal()
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.__initUi()
-
-    def __initUi(self):
-        self.setStyleSheet('QTextEdit { border: 1px solid #AAA; } ')
-
-    def keyPressEvent(self, e):
-        if e.key() == Qt.Key_Return or e.key() == Qt.Key_Enter:
-            if e.modifiers() == Qt.ShiftModifier:
-                return super().keyPressEvent(e)
+            if qGray(r, g, b) > 255 // 2:
+                text_color = QColor(255, 255, 255)
             else:
-                self.returnPressed.emit()
-        else:
-            return super().keyPressEvent(e)
-
-
-class Prompt(QWidget):
-    def __init__(self):
-        super().__init__()
-        self.__initUi()
-
-    def __initUi(self):
-        self.__textEdit = TextEditPrompt()
-        self.__textEdit.textChanged.connect(self.updateHeight)
-        lay = QHBoxLayout()
-        lay.addWidget(self.__textEdit)
-        lay.setContentsMargins(0, 0, 0, 0)
-        self.setLayout(lay)
-        self.updateHeight()
-
-    def updateHeight(self):
-        document = self.__textEdit.document()
-        height = document.size().height()
-        self.setMaximumHeight(int(height+document.documentMargin()))
-
-    def getTextEdit(self):
-        return self.__textEdit
+                text_color = QColor(0, 0, 0)
+        return text_color.name()
 
+    def __styleInit(self):
+        self.__btn_style = f'''
+        QAbstractButton
+        {{
+        border: 0;
+        width: {self.__size};
+        height: {self.__size};
+        image: url({self.__icon});
+        background-color: {self.__background_color};
+        border-radius: {self.__border_radius};
+        padding: {self.__padding};
+        color: {self.__text_color};
+        }}
+        QAbstractButton:hover
+        {{
+        background-color: {self.__hover_color};
+        }}
+        QAbstractButton:pressed
+        {{
+        background-color: {self.__pressed_color};
+        }}
+        QAbstractButton:checked
+        {{
+        background-color: {self.__checked_color};
+        border: none;
+        }}
+        '''
+
+        self.setStyleSheet(self.__btn_style)
+
+    def setIcon(self, icon: str):
+        self.__icon = os.path.join(os.path.dirname(__file__), icon).replace(os.sep, posixpath.sep)
+        self.__styleInit()
+
+    def eventFilter(self, obj, e):
+        if obj == self:
+            # to change grayscale when button gets disabled
+            # if button get enabled/disabled EnableChange will emit
+            # so catch the EnabledChange
+            if e.type() == 98:
+                # change to enabled state
+                effect = QGraphicsColorizeEffect()
+                effect.setColor(QColor(255, 255, 255))
+                if self.isEnabled():
+                    effect.setStrength(0)
+                else:
+                    effect.setStrength(1)
+                    effect.setColor(QColor(150, 150, 150))
+                self.setGraphicsEffect(effect)
+        if obj == self.__baseWidget:
+            # catch the StyleChange event of base widget
+            if e.type() == 100:
+                # if base widget's background is transparent (#ffffff)
+                if self.__baseWidget.palette().color(QPalette.Base).name() == '#ffffff':
+                    # then check the parent widget's background
+                    if self.__baseWidget.parent():
+                        if self.__baseWidget.parent().palette().color(QPalette.Base).name() == '#ffffff':
+                            pass
+                        else:
+                            self.__baseWidget = self.__baseWidget.parent()
+                self.__initColorByBaseWidget()
+                self.__styleInit()
+        return super().eventFilter(obj, e)
+
+    def setPadding(self, padding: int):
+        self.__padding = padding
+        self.__styleInit()
+
+    def setBorderRadius(self, border_radius: int):
+        self.__border_radius = border_radius
+        self.__styleInit()
+
+    def setBackground(self, background=None):
+        if background:
+            self.__background_color = background
+        else:
+            self.__background_color = self.__base_color.name()
+        self.__styleInit()
 
+    def setAsCircle(self):
+        self.setBorderRadius(self.height() // 2)
+        self.__styleInit()
+
+    # to set size accordance with scale
+    def __scaleChanged(self, dpi):
+        self.__size = dpi // 4
+        self.__styleInit()
```

### Comparing `pyqt-openai-0.1.22/pyqt_openai/circleProfileImage.py` & `pyqt-openai-0.1.3/pyqt_openai/circleProfileImage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/clickableTooltip.py` & `pyqt-openai-0.1.3/pyqt_openai/clickableTooltip.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/convListWidget.py` & `pyqt-openai-0.1.3/pyqt_openai/convListWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/customizeDialog.py` & `pyqt-openai-0.1.3/pyqt_openai/customizeDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/close.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/close.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/customize.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/customize.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/download.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/download.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/help.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/help.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/openai.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/openai.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/search.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/search.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/setting.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/setting.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/stackontop.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/stackontop.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/ico/user.svg` & `pyqt-openai-0.1.3/pyqt_openai/ico/user.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/inputDialog.py` & `pyqt-openai-0.1.3/pyqt_openai/inputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/leftSideBar.py` & `pyqt-openai-0.1.3/pyqt_openai/leftSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/main.py` & `pyqt-openai-0.1.3/pyqt_openai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,14 @@
         self.__leftSideBarWidget.initHistory(self.__db)
         self.__leftSideBarWidget.added.connect(self.__addConv)
         self.__leftSideBarWidget.changed.connect(self.__changeConv)
         self.__leftSideBarWidget.deleted.connect(self.__deleteConv)
         self.__leftSideBarWidget.convUpdated.connect(self.__updateConv)
         self.__leftSideBarWidget.export.connect(self.__export)
 
-        self.__lineEdit.setPlaceholderText('Write some text...')
         self.__lineEdit.returnPressed.connect(self.__chat)
 
         self.__browser.convUnitUpdated.connect(self.__updateConvUnit)
 
         lay = QHBoxLayout()
         lay.addWidget(self.__prompt)
         lay.setSpacing(0)
@@ -423,15 +422,15 @@
 
     def __chat(self):
         info_dict = self.__db.selectInfo()
         is_img = info_dict['engine'] in ['DALL-E', 'midjourney', 'stable_diffusion']
         openai_arg = ''
         if is_img:
             openai_arg = {
-                "prompt": self.__lineEdit.toPlainText(),
+                "prompt": self.__prompt.getContent(),
                 "n": info_dict['n'],
                 "size": f"{info_dict['width']}x{info_dict['height']}"
             }
         else:
             if self.__remember_past_conv:
                 convs = []
                 with open('conv.json', 'r') as f:
@@ -442,15 +441,15 @@
             if info_dict['engine'] in ['gpt-3.5-turbo', 'gpt-3.5-turbo-0301', 'gpt-4']:
                 # "assistant" below is for making the AI remember the last question
                 openai_arg = {
                     'model': info_dict['engine'],
                     'messages': [
                         {"role": "system", "content": info_dict['system']},
                         {"role": "assistant", "content": self.__browser.getAllText()},
-                        {"role": "user", "content": self.__lineEdit.toPlainText()},
+                        {"role": "user", "content": self.__prompt.getContent()},
                     ],
                     # 'temperature': info_dict['temperature'],
 
                     # won't use max_tokens, this is set to infinite by default
                     # and i can't find any reason why should i limit the tokens currently
                     # https://platform.openai.com/docs/api-reference/chat/create
                     # 'max_tokens': self.__max_tokens,
@@ -467,15 +466,15 @@
             pass
         else:
             self.__addConv()
 
         self.__lineEdit.setEnabled(False)
         self.__leftSideBarWidget.setEnabled(False)
 
-        self.__browser.showLabel(self.__lineEdit.toPlainText(), True, False, False)
+        self.__browser.showLabel(self.__prompt.getContent(), True, False, False)
 
         self.__t = OpenAIThread(info_dict['engine'], openai_arg, is_img, self.__remember_past_conv)
         self.__t.replyGenerated.connect(self.__browser.showLabel)
         self.__t.streamFinished.connect(self.__browser.streamFinished)
         self.__lineEdit.clear()
         self.__t.start()
         self.__t.finished.connect(self.__afterGenerated)
```

### Comparing `pyqt-openai-0.1.22/pyqt_openai/modelTable.py` & `pyqt-openai-0.1.3/pyqt_openai/modelTable.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/notifier.py` & `pyqt-openai-0.1.3/pyqt_openai/notifier.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/prompt/promptGeneratorWidget.py` & `pyqt-openai-0.1.3/pyqt_openai/prompt/promptGeneratorWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/prompt/templatePage.py` & `pyqt-openai-0.1.3/pyqt_openai/prompt/templatePage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,40 @@
-from PyQt5.QtWidgets import QHeaderView, QTableWidgetItem, QAbstractItemView
-from qtpy.QtWidgets import QWidget, QTableWidget, QVBoxLayout
-from qtpy.QtCore import Signal
+from qtpy.QtWidgets import QWidget, QDialog, QTableWidget, QVBoxLayout, QHBoxLayout, QHeaderView, QTableWidgetItem, QAbstractItemView
+from qtpy.QtCore import Signal, Qt
+
+from pyqt_openai.inputDialog import InputDialog
+from pyqt_openai.svgButton import SvgButton
 
 
 class TemplatePage(QWidget):
     updated = Signal(str, str)
 
     def __init__(self):
         super().__init__()
         self.__initUi()
 
     def __initUi(self):
+        self.__addBtn = SvgButton()
+        self.__delBtn = SvgButton()
+
+        self.__addBtn.setIcon('ico/add.svg')
+        self.__delBtn.setIcon('ico/delete.svg')
+
+        self.__addBtn.clicked.connect(self.__add)
+        self.__delBtn.clicked.connect(self.__delete)
+
+        lay = QHBoxLayout()
+        lay.addWidget(self.__addBtn)
+        lay.addWidget(self.__delBtn)
+        lay.setAlignment(Qt.AlignRight)
+        lay.setContentsMargins(0, 0, 0, 0)
+
+        topWidget = QWidget()
+        topWidget.setLayout(lay)
+
         # this template has to be connected with db
         # QSqlTableModel
         self.__templateTable = QTableWidget()
         self.__templateTable.setColumnCount(2)
         self.__templateTable.setHorizontalHeaderLabels(['Content', 'Variables'])
         self.__templateTable.horizontalHeader().setSectionResizeMode(0, QHeaderView.Stretch)
         self.__templateTable.setSelectionBehavior(QAbstractItemView.SelectRows)
@@ -39,15 +59,34 @@
         for i in range(len(sampleTemplateItems)):
             content = sampleTemplateItems[i]
             self.__templateTable.setItem(i, 0, QTableWidgetItem(content))
             # variable = content.find()
             self.__templateTable.setItem(i, 1, QTableWidgetItem('topic or skill'))
 
         lay = QVBoxLayout()
+        lay.addWidget(topWidget)
         lay.addWidget(self.__templateTable)
 
         self.setLayout(lay)
 
     def __rowChanged(self, new_item: QTableWidgetItem, old_item: QTableWidgetItem):
         content = self.__templateTable.item(new_item.row(), 0).text() if new_item.column() == 1 else new_item.text()
         variable = self.__templateTable.item(new_item.row(), 1).text()
         self.updated.emit(content, variable)
+
+    def __add(self):
+        dialog = InputDialog('Content', '')
+        reply = dialog.exec()
+        if reply == QDialog.Accepted:
+            text = dialog.getText()
+            self.__templateTable.setRowCount(self.__templateTable.rowCount()+1)
+            item1 = QTableWidgetItem(text)
+            item1.setTextAlignment(Qt.AlignCenter)
+            self.__templateTable.setItem(self.__templateTable.rowCount()-1, 0, item1)
+
+            item2 = QTableWidgetItem('')
+            item2.setTextAlignment(Qt.AlignCenter)
+            self.__templateTable.setItem(self.__templateTable.rowCount()-1, 1, item2)
+
+    def __delete(self):
+        for i in sorted(set([i.row() for i in self.__templateTable.selectedIndexes()]), reverse=True):
+            self.__templateTable.removeRow(i)
```

### Comparing `pyqt-openai-0.1.22/pyqt_openai/right_sidebar/aiPlaygroundWidget.py` & `pyqt-openai-0.1.3/pyqt_openai/right_sidebar/aiPlaygroundWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/right_sidebar/chatPage.py` & `pyqt-openai-0.1.3/pyqt_openai/right_sidebar/chatPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/right_sidebar/completionPage.py` & `pyqt-openai-0.1.3/pyqt_openai/right_sidebar/completionPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/right_sidebar/imagePage.py` & `pyqt-openai-0.1.3/pyqt_openai/right_sidebar/imagePage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/searchBar.py` & `pyqt-openai-0.1.3/pyqt_openai/searchBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/sqlite.py` & `pyqt-openai-0.1.3/pyqt_openai/sqlite.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/svgButton.py` & `pyqt-openai-0.1.3/pyqt_openai/svgToolButton.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path, posixpath
 
 from qtpy.QtGui import QColor, QPalette, qGray
-from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QPushButton
+from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QToolButton
 
 
-class SvgButton(QPushButton):
+class SvgToolButton(QToolButton):
     def __init__(self, base_widget: QWidget = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__baseWidget = base_widget
         self.__initVal()
         self.__styleInit()
 
     def __initVal(self):
```

### Comparing `pyqt-openai-0.1.22/pyqt_openai/svgLabel.py` & `pyqt-openai-0.1.3/pyqt_openai/svgLabel.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/test/htmlformat.py` & `pyqt-openai-0.1.3/pyqt_openai/test/htmlformat.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/test/rightSideBarTab.py` & `pyqt-openai-0.1.3/pyqt_openai/test/rightSideBarTab.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/delete_model.py` & `pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/delete_model.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/make_model.py` & `pyqt-openai-0.1.3/pyqt_openai/test/stable_diffusion/make_model.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.22/pyqt_openai.egg-info/PKG-INFO` & `pyqt-openai-0.1.3/pyqt_openai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.22
+Version: 0.1.3
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -49,43 +49,47 @@
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator
+* support prompt generator (manageable)
+* support beginning and ending part of the prompt
 * support image generation with DALL-E
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 
 ## Preview
-This is using GPT-3.5 turbo model by default.
+This is using GPT-3.5 turbo model by default. 
 
 ### Homepage
-![image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-b78ab8a1eb73.png)
+![image](https://user-images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-b45401f8bb7c.png)
 <b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
 
 ### Overview
-![image](https://user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-e502a182264d.png)
+![image](https://user-images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-4630010edd5b.png)
 
 ### Conversation preview
 #### Preview Image
 ![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
 #### Preview Video
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 
 ### Prompt Generator
+#### Preview 1 (v0.1.22)
 https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
+#### Preview 2 (v0.1.3)
+https://user-images.githubusercontent.com/55078043/236658468-9947a417-99b3-4e44-8849-a676308a0239.mp4
 
 So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
 
 ## How to play
 1. git clone ~
 2. from the root directory, type "cd pyqt_openai"
 3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.22 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.3 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot. Even though this
@@ -20,42 +20,45 @@
 software. It's not necessary to run this app (obviously), but it's good
 practice to manage database about conversation history with AI and to know how
 this works. ## Feature * basically this is desktop application version of
 ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
 past conversation * conversation management * add & delete conversations * save
 conversations * rename conversation * everything above is saved in an SQLite
 database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator * support image generation with DALL-E * you can run
-this in background application * notification will pop up when response is
-generated * you can make window stack on top or control its transparency ##
-Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
-using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-
-b78ab8a1eb73.png) You have to write your openai api key inside the red box. see
+* support prompt generator (manageable) * support beginning and ending part of
+the prompt * support image generation with DALL-E * you can run this in
+background application * notification will pop up when response is generated *
+you can make window stack on top or control its transparency ## Requirements *
+qtpy - the package allowing you to write code that works with both PyQt and
+PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is using GPT-3.5
+turbo model by default. ### Homepage ![image](https://user-
+images.githubusercontent.com/55078043/236657804-bf299150-961a-4f80-9820-
+b45401f8bb7c.png) You have to write your openai api key inside the red box. see
 [How to play](#how-to-play) ### Overview ![image](https://user-
-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
-e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
+images.githubusercontent.com/55078043/236657785-69825ff8-8cce-4759-8468-
+4630010edd5b.png) ### Conversation preview #### Preview Image ![image](https://
 user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
 7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator https://user-images.githubusercontent.com/55078043/236584481-
-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
-lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
-~ 2. from the root directory, type "cd pyqt_openai" 3. You should put your api
-key in the line edit. You can get it in official_site of openai. Sign up and
-log in before you get it. By the way, this is free trial, not permanently free.
-See this after you have logged in. Be sure, this is a very important API key
-that belongs to you only, so you should remember it and keep it secure. 4.
-python main.py If installation doesn't work, check the troubleshooting below.
-## Troubleshooting If you see this error while installing the openai package
-``` subprocess-exited-with-error ``` you can shout a curse word and just
-download the package itself from pypi. Unzip it, access the package directory,
-type ``` python setup.py install ``` That will install the openai. ## TODO list
-* support Stable Diffusion * show the explanation of every model and terms
+Generator #### Preview 1 (v0.1.22) https://user-images.githubusercontent.com/
+55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 #### Preview 2
+(v0.1.3) https://user-images.githubusercontent.com/55078043/236658468-9947a417-
+99b3-4e44-8849-a676308a0239.mp4 So sorry to weak preview, but i have a lot of
+idea about this prompt generator! Just wait. ## How to play 1. git clone ~ 2.
+from the root directory, type "cd pyqt_openai" 3. You should put your api key
+in the line edit. You can get it in official_site of openai. Sign up and log in
+before you get it. By the way, this is free trial, not permanently free. See
+this after you have logged in. Be sure, this is a very important API key that
+belongs to you only, so you should remember it and keep it secure. 4. python
+main.py If installation doesn't work, check the troubleshooting below. ##
+Troubleshooting If you see this error while installing the openai package ```
+subprocess-exited-with-error ``` you can shout a curse word and just download
+the package itself from pypi. Unzip it, access the package directory, type ```
+python setup.py install ``` That will install the openai. ## TODO list *
+support Stable Diffusion * show the explanation of every model and terms
 related to AI (e.g. temperature, topp..) * save conversation history with other
 format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
 eventually) * support multiple language * use SQLAlchemy (maybe not) * show
 reason when the chat input is disabled for some reasons * add the basic example
 sources of making deep learning model with PyTorch (eventually) ## See Also *
 Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
 it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.22/pyqt_openai.egg-info/SOURCES.txt` & `pyqt-openai-0.1.3/pyqt_openai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 pyqt_openai/main.py
 pyqt_openai/modelTable.py
 pyqt_openai/notifier.py
 pyqt_openai/searchBar.py
 pyqt_openai/sqlite.py
 pyqt_openai/svgButton.py
 pyqt_openai/svgLabel.py
+pyqt_openai/svgToolButton.py
 pyqt_openai.egg-info/PKG-INFO
 pyqt_openai.egg-info/SOURCES.txt
 pyqt_openai.egg-info/dependency_links.txt
 pyqt_openai.egg-info/requires.txt
 pyqt_openai.egg-info/top_level.txt
 pyqt_openai/ico/__init__.py
 pyqt_openai/ico/add.svg
@@ -33,24 +34,25 @@
 pyqt_openai/ico/openai.svg
 pyqt_openai/ico/prompt.svg
 pyqt_openai/ico/search.svg
 pyqt_openai/ico/setting.svg
 pyqt_openai/ico/sidebar.svg
 pyqt_openai/ico/stackontop.svg
 pyqt_openai/ico/user.svg
+pyqt_openai/ico/vertical_three_dots.svg
 pyqt_openai/prompt/__init__.py
 pyqt_openai/prompt/promptGeneratorWidget.py
 pyqt_openai/prompt/propPage.py
 pyqt_openai/prompt/templatePage.py
 pyqt_openai/right_sidebar/__init__.py
 pyqt_openai/right_sidebar/aiPlaygroundWidget.py
 pyqt_openai/right_sidebar/chatPage.py
 pyqt_openai/right_sidebar/completionPage.py
 pyqt_openai/right_sidebar/imagePage.py
 pyqt_openai/test/__init__.py
-pyqt_openai/test/dialog.py
 pyqt_openai/test/htmlformat.py
+pyqt_openai/test/prompt_autocomplete.py
 pyqt_openai/test/rightSideBarTab.py
 pyqt_openai/test/stable_diffusion/__init__.py
 pyqt_openai/test/stable_diffusion/delete_model.py
 pyqt_openai/test/stable_diffusion/make_model.py
 pyqt_openai/test/stable_diffusion/using_model.py
```

### Comparing `pyqt-openai-0.1.22/setup.py` & `pyqt-openai-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-openai',
-    version='0.1.22',
+    version='0.1.3',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
     package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'help.svg', 'customize.svg', 'user.svg',
                                       'sidebar.svg', 'prompt.svg', 'download.svg', 'stackontop.svg',
-                                      'add.svg', 'delete.svg', 'setting.svg', 'search.svg']},
+                                      'add.svg', 'delete.svg', 'setting.svg', 'search.svg',
+                                      'vertical_three_dots.svg']},
     description='PyQt OpenAI example',
     url='https://github.com/yjg30737/pyqt-openai.git',
     long_description_content_type='text/markdown',
     long_description=long_description,
     install_requires=[
         'PyQt5>=5.14',
         'PySide6',
```

