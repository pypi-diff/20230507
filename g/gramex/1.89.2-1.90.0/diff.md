# Comparing `tmp/gramex-1.89.2.tar.gz` & `tmp/gramex-1.90.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramex-1.89.2.tar", last modified: Tue Apr 11 12:21:52 2023, max compression
+gzip compressed data, was "gramex-1.90.0.tar", last modified: Sun May  7 15:53:06 2023, max compression
```

## Comparing `gramex-1.89.2.tar` & `gramex-1.90.0.tar`

### file list

```diff
@@ -1,411 +1,398 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.996815 gramex-1.89.2/
--rw-rw-rw-   0        0        0     1900 2023-04-10 11:33:47.000000 gramex-1.89.2/.gitignore
--rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.89.2/LICENSE
--rw-rw-rw-   0        0        0      641 2023-04-11 12:20:36.000000 gramex-1.89.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2956 2023-04-11 12:21:51.997818 gramex-1.89.2/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.89.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.781002 gramex-1.89.2/gramex/
--rw-rw-rw-   0        0        0    15368 2023-04-11 12:20:36.000000 gramex-1.89.2/gramex/__init__.py
--rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.89.2/gramex/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.840230 gramex-1.89.2/gramex/apps/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.89.2/gramex/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.843225 gramex-1.89.2/gramex/apps/admin/
--rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.89.2/gramex/apps/admin/.gitignore
--rw-rw-rw-   0        0        0      129 2023-01-03 16:10:30.000000 gramex-1.89.2/gramex/apps/admin/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.877013 gramex-1.89.2/gramex/apps/admin2/
--rw-rw-rw-   0        0        0      269 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/admin2/.eslintrc.js
--rw-rw-rw-   0        0        0      226 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/apps/admin2/.snyk
--rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.89.2/gramex/apps/admin2/admin.css
--rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/admin2/gramex.yaml
--rw-rw-rw-   0        0        0    12257 2022-11-23 04:49:14.000000 gramex-1.89.2/gramex/apps/admin2/gramexadmin.py
--rw-rw-rw-   0        0        0     8420 2022-03-03 08:20:09.000000 gramex-1.89.2/gramex/apps/admin2/index.html
--rw-rw-rw-   0        0        0    12293 2023-04-11 12:16:39.000000 gramex-1.89.2/gramex/apps/admin2/package-lock.json
--rw-rw-rw-   0        0        0      132 2022-02-19 10:03:02.000000 gramex-1.89.2/gramex/apps/admin2/package.json
--rw-rw-rw-   0        0        0      231 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/admin2/rollup.config.js
--rw-rw-rw-   0        0        0     4919 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/admin2/schedule.js
--rw-rw-rw-   0        0        0     2505 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/admin2/schedule.src.js
--rw-rw-rw-   0        0        0     3037 2022-02-19 10:03:02.000000 gramex-1.89.2/gramex/apps/admin2/schedule.template.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.893653 gramex-1.89.2/gramex/apps/capture/
--rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/capture/README.md
--rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/capture/capture.js
--rw-rw-rw-   0        0        0    12034 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/capture/chromecapture.js
--rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.89.2/gramex/apps/capture/index.html
--rw-rw-rw-   0        0        0   141593 2023-04-11 12:16:46.000000 gramex-1.89.2/gramex/apps/capture/package-lock.json
--rw-rw-rw-   0        0        0      863 2023-02-08 17:06:15.000000 gramex-1.89.2/gramex/apps/capture/package.json
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.922654 gramex-1.89.2/gramex/apps/filemanager/
--rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.89.2/gramex/apps/filemanager/.snyk
--rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.89.2/gramex/apps/filemanager/README.html
--rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.89.2/gramex/apps/filemanager/drivehandler-snippet.html
--rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.89.2/gramex/apps/filemanager/filemanager-snippet.html
--rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.89.2/gramex/apps/filemanager/filemanager.html
--rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/filemanager/filemanager.js
--rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.89.2/gramex/apps/filemanager/filemanager.py
--rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.89.2/gramex/apps/filemanager/gramex.yaml
--rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.89.2/gramex/apps/filemanager/index.html
--rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.89.2/gramex/apps/filemanager/navbar.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.657522 gramex-1.89.2/gramex/apps/init/
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.959230 gramex-1.89.2/gramex/apps/init/default/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:38.000000 gramex-1.89.2/gramex/apps/init/default/$appname.py
--rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/.flake8
--rw-rw-rw-   0        0        0      592 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.89.2/gramex/apps/init/default/.secrets.yaml
--rw-rw-rw-   0        0        0     1144 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/.stylelintrc.js
--rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.89.2/gramex/apps/init/default/.template.gitignore
--rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/README.template.md
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.961231 gramex-1.89.2/gramex/apps/init/default/assets/
--rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/assets/README.template.md
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.976586 gramex-1.89.2/gramex/apps/init/default/error/
--rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/error/400.html
--rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/error/401.html
--rw-rw-rw-   0        0        0     2374 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/error/403.html
--rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/error/404.html
--rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/error/500.html
--rw-rw-rw-   0        0        0    12057 2022-02-19 10:03:03.000000 gramex-1.89.2/gramex/apps/init/default/favicon.ico
--rw-rw-rw-   0        0        0     2992 2022-10-02 08:02:34.000000 gramex-1.89.2/gramex/apps/init/default/gramex.template.yaml
--rw-rw-rw-   0        0        0     2602 2022-03-03 08:20:09.000000 gramex-1.89.2/gramex/apps/init/default/index.template.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.979617 gramex-1.89.2/gramex/apps/init/default/js/
--rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/init/default/js/README.template.md
--rw-rw-rw-   0        0        0     2604 2022-02-19 10:03:03.000000 gramex-1.89.2/gramex/apps/init/default/login.template.html
--rw-rw-rw-   0        0        0      304 2022-02-19 10:03:03.000000 gramex-1.89.2/gramex/apps/init/default/package.template.json
--rw-rw-rw-   0        0        0       77 2022-03-03 08:20:09.000000 gramex-1.89.2/gramex/apps/init/default/style.scss
--rw-rw-rw-   0        0        0     2614 2022-02-19 10:03:03.000000 gramex-1.89.2/gramex/apps/init/default/template-navbar.template.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.988880 gramex-1.89.2/gramex/apps/init/ide/
--rw-rw-rw-   0        0        0      377 2023-02-08 17:06:15.000000 gramex-1.89.2/gramex/apps/init/ide/.gitlab-ci.template.yml
--rw-rw-rw-   0        0        0      199 2023-02-08 17:06:15.000000 gramex-1.89.2/gramex/apps/init/ide/gramex.template.yaml
--rw-rw-rw-   0        0        0      738 2023-02-08 17:06:15.000000 gramex-1.89.2/gramex/apps/init/ide/index.template.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.994091 gramex-1.89.2/gramex/apps/init/minimal/
--rw-rw-rw-   0        0        0      199 2022-02-19 10:03:03.000000 gramex-1.89.2/gramex/apps/init/minimal/gramex.template.yaml
--rw-rw-rw-   0        0        0      738 2022-03-03 08:20:09.000000 gramex-1.89.2/gramex/apps/init/minimal/index.template.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.001089 gramex-1.89.2/gramex/apps/languagetool/
--rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/languagetool/README.md
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.89.2/gramex/apps/languagetool/__init__.py
--rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/languagetool/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.042440 gramex-1.89.2/gramex/apps/logviewer/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.89.2/gramex/apps/logviewer/__init__.py
--rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/logviewer/config.yaml
--rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/logviewer/gramex.yaml
--rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.89.2/gramex/apps/logviewer/index.html
--rw-rw-rw-   0        0        0    13287 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/apps/logviewer/logviewer.py
--rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.89.2/gramex/apps/logviewer/lv-card-deck.html
--rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.89.2/gramex/apps/logviewer/lv-card.html
--rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.89.2/gramex/apps/logviewer/lv-datepicker.html
--rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.89.2/gramex/apps/logviewer/lv-dropdown.html
--rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.89.2/gramex/apps/logviewer/lv-filters.html
--rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.89.2/gramex/apps/logviewer/lv-header.html
--rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.89.2/gramex/apps/logviewer/lv-kpi.html
--rw-rw-rw-   0        0        0      775 2023-04-11 12:16:50.000000 gramex-1.89.2/gramex/apps/logviewer/package-lock.json
--rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.89.2/gramex/apps/logviewer/package.json
--rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/logviewer/render.js
--rw-rw-rw-   0        0        0     5390 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/apps/logviewer/script.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.050533 gramex-1.89.2/gramex/apps/mail/
--rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/mail/gramex.yaml
--rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.89.2/gramex/apps/mail/index.html
--rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.89.2/gramex/apps/mail/mailapp.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.052483 gramex-1.89.2/gramex/apps/mlhandler/
--rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.89.2/gramex/apps/mlhandler/template.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.065907 gramex-1.89.2/gramex/apps/pynode/
--rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.89.2/gramex/apps/pynode/.snyk
--rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.89.2/gramex/apps/pynode/README.md
--rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/pynode/index.js
--rw-rw-rw-   0        0        0     2953 2023-04-11 12:16:54.000000 gramex-1.89.2/gramex/apps/pynode/package-lock.json
--rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.89.2/gramex/apps/pynode/package.json
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.070904 gramex-1.89.2/gramex/apps/smartalerts/
--rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.89.2/gramex/apps/smartalerts/gramex.yaml
--rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.89.2/gramex/apps/smartalerts/index.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.099425 gramex-1.89.2/gramex/apps/ui/
--rw-rw-rw-   0        0        0     1019 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/apps/ui/.snyk
--rw-rw-rw-   0        0        0    12878 2022-12-20 15:16:57.000000 gramex-1.89.2/gramex/apps/ui/__init__.py
--rw-rw-rw-   0        0        0      648 2022-02-19 09:58:43.000000 gramex-1.89.2/gramex/apps/ui/bootstrap-theme.scss
--rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/config.yaml
--rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.89.2/gramex/apps/ui/gramex.yaml
--rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/gramexui.scss
--rw-rw-rw-   0        0        0   588284 2023-04-11 12:20:36.000000 gramex-1.89.2/gramex/apps/ui/package-lock.json
--rw-rw-rw-   0        0        0      341 2023-04-11 12:20:36.000000 gramex-1.89.2/gramex/apps/ui/package.json
--rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.89.2/gramex/apps/ui/setup.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.116908 gramex-1.89.2/gramex/apps/ui/theme/
--rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/bootstrap5.scss
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.476274 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/
--rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cerulean.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cerulean.scss
--rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cosmo.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cosmo.scss
--rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cyborg.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cyborg.scss
--rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/darkly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/darkly.scss
--rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/flatly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/flatly.scss
--rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/journal.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/journal.scss
--rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/litera.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/litera.scss
--rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/lumen.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/lumen.scss
--rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/lux.png
--rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/lux.scss
--rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/materia.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/materia.scss
--rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/minty.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/minty.scss
--rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/pulse.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/pulse.scss
--rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/sandstone.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/sandstone.scss
--rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/simplex.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/simplex.scss
--rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/sketchy.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/sketchy.scss
--rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/slate.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/slate.scss
--rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/solar.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/solar.scss
--rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/spacelab.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/spacelab.scss
--rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/superhero.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/superhero.scss
--rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/united.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/united.scss
--rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/yeti.png
--rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.89.2/gramex/apps/ui/theme/bootswatch/yeti.scss
--rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/default.png
--rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.89.2/gramex/apps/ui/theme/default.scss
--rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/index.html
--rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/sample.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.573953 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/
--rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/blue_voltage.png
--rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
--rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/boldstrap.png
--rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/boldstrap.scss
--rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
--rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
--rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/darkster.png
--rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/darkster.scss
--rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/fresca.png
--rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/fresca.scss
--rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/greyson.png
--rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/greyson.scss
--rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
--rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
--rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/herbie.png
--rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/herbie.scss
--rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/hootstrap.png
--rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/hootstrap.scss
--rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/lovey.png
--rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/lovey.scss
--rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/monotony.png
--rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/monotony.scss
--rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/poypull.png
--rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/poypull.scss
--rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/signal.png
--rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/signal.scss
--rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/tequila.png
--rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/ui/theme/themes-guide/tequila.scss
--rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.89.2/gramex/apps/ui/theme/themes.json
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.622418 gramex-1.89.2/gramex/apps/uifactory/
--rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.89.2/gramex/apps/uifactory/.eslintrc.js
--rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/.gitattributes
--rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.624750 gramex-1.89.2/gramex/apps/uifactory/assets/
--rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/assets/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.627165 gramex-1.89.2/gramex/apps/uifactory/assets/data/
--rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.89.2/gramex/apps/uifactory/assets/data/input.json
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.638026 gramex-1.89.2/gramex/apps/uifactory/assets/img/
--rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.89.2/gramex/apps/uifactory/assets/img/arrows-move.svg
--rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.89.2/gramex/apps/uifactory/assets/img/clipboard.svg
--rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
--rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.89.2/gramex/apps/uifactory/assets/img/trash.svg
--rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/create.html
--rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/edit.html
--rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/field-actions.html
--rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.89.2/gramex/apps/uifactory/form_builder.py
--rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/gramex.yaml
--rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/index.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.658005 gramex-1.89.2/gramex/apps/uifactory/js/
--rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/js/README.md
--rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/js/embed.js
--rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/js/fields.js
--rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/js/fork-form.js
--rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/js/index.js
--rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/js/script.js
--rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/js/utils.js
--rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/js/viewform.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.673428 gramex-1.89.2/gramex/apps/uifactory/modals/
--rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/modals/add-field.html
--rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/modals/embed.html
--rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/modals/remove.html
--rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/modals/rename.html
--rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/modals/themes.html
--rw-rw-rw-   0        0        0     5540 2023-04-11 12:17:09.000000 gramex-1.89.2/gramex/apps/uifactory/package-lock.json
--rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.89.2/gramex/apps/uifactory/package.json
--rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/popover-form.html
--rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/sample.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.679632 gramex-1.89.2/gramex/apps/uifactory/snippets/
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.682646 gramex-1.89.2/gramex/apps/uifactory/snippets/button/
--rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/button/bs4-button.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.686659 gramex-1.89.2/gramex/apps/uifactory/snippets/checkbox/
--rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.688937 gramex-1.89.2/gramex/apps/uifactory/snippets/email/
--rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/email/bs4-email.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.691938 gramex-1.89.2/gramex/apps/uifactory/snippets/hidden/
--rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.694934 gramex-1.89.2/gramex/apps/uifactory/snippets/html/
--rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/html/bs4-html.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.697935 gramex-1.89.2/gramex/apps/uifactory/snippets/multiselect/
--rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.701336 gramex-1.89.2/gramex/apps/uifactory/snippets/number/
--rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/number/bs4-number.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.704331 gramex-1.89.2/gramex/apps/uifactory/snippets/password/
--rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/password/bs4-password.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.707338 gramex-1.89.2/gramex/apps/uifactory/snippets/radio/
--rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/radio/bs4-radio.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.710348 gramex-1.89.2/gramex/apps/uifactory/snippets/range/
--rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/range/bs4-range.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.713492 gramex-1.89.2/gramex/apps/uifactory/snippets/select/
--rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/select/bs4-select.js
--rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/setup.js
--rw-rw-rw-   0        0        0        3 2023-01-07 08:41:00.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/snippets.json
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.715926 gramex-1.89.2/gramex/apps/uifactory/snippets/text/
--rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/text/bs4-text.js
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.718925 gramex-1.89.2/gramex/apps/uifactory/snippets/textarea/
--rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
--rw-rw-rw-   0        0        0     1766 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/uifactory/style.scss
--rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/template-navbar-view-form.html
--rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/template-navbar.html
--rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/toast.html
--rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.89.2/gramex/apps/uifactory/viewform.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.731496 gramex-1.89.2/gramex/apps/update/
--rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.89.2/gramex/apps/update/README.md
--rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/apps/update/gramex.yaml
--rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.89.2/gramex/apps/update/gramexupdate.py
--rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.89.2/gramex/apps/update/index.html
--rw-rw-rw-   0        0        0      391 2023-04-11 12:20:36.000000 gramex-1.89.2/gramex/apps.yaml
--rw-rw-rw-   0        0        0    56930 2023-01-03 16:10:30.000000 gramex-1.89.2/gramex/cache.py
--rw-rw-rw-   0        0        0    34362 2023-02-09 09:15:32.000000 gramex-1.89.2/gramex/config.py
--rw-rw-rw-   0        0        0    93430 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/data.py
--rw-rw-rw-   0        0        0     6353 2022-11-23 04:49:14.000000 gramex-1.89.2/gramex/debug.py
--rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/deploy.yaml
--rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/download.vega.js
--rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.89.2/gramex/favicon.ico
--rw-rw-rw-   0        0        0    16330 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/gramex.yaml
--rw-rw-rw-   0        0        0     2011 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/gramexfeatures.csv
--rw-rw-rw-   0        0        0    14445 2023-04-11 12:20:36.000000 gramex-1.89.2/gramex/gramexsize.csv
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.813123 gramex-1.89.2/gramex/handlers/
--rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/400.html
--rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/401.html
--rw-rw-rw-   0        0        0     2374 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/403.html
--rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/404.html
--rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/500.html
--rw-rw-rw-   0        0        0     2499 2022-11-23 03:19:44.000000 gramex-1.89.2/gramex/handlers/__init__.py
--rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/auth.recaptcha.template.html
--rw-rw-rw-   0        0        0    12772 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/auth.template.html
--rw-rw-rw-   0        0        0    17394 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/handlers/authhandler.py
--rw-rw-rw-   0        0        0    61031 2023-04-03 08:25:14.000000 gramex-1.89.2/gramex/handlers/basehandler.py
--rw-rw-rw-   0        0        0    15648 2022-12-20 15:16:57.000000 gramex-1.89.2/gramex/handlers/capturehandler.py
--rw-rw-rw-   0        0        0     1477 2022-11-06 08:24:25.000000 gramex-1.89.2/gramex/handlers/comichandler.py
--rw-rw-rw-   0        0        0     8922 2022-11-06 08:24:26.000000 gramex-1.89.2/gramex/handlers/drivehandler.py
--rw-rw-rw-   0        0        0    14849 2023-02-24 08:15:32.000000 gramex-1.89.2/gramex/handlers/filehandler.py
--rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.89.2/gramex/handlers/filehandler.template.html
--rw-rw-rw-   0        0        0      198 2023-01-03 16:10:30.000000 gramex-1.89.2/gramex/handlers/filterhandler.py
--rw-rw-rw-   0        0        0    13238 2023-01-03 16:10:30.000000 gramex-1.89.2/gramex/handlers/formhandler.py
--rw-rw-rw-   0        0        0     3774 2022-11-23 03:19:45.000000 gramex-1.89.2/gramex/handlers/functionhandler.py
--rw-rw-rw-   0        0        0     6622 2022-11-23 03:19:45.000000 gramex-1.89.2/gramex/handlers/jsonhandler.py
--rw-rw-rw-   0        0        0    16154 2022-11-23 04:49:14.000000 gramex-1.89.2/gramex/handlers/mlhandler.py
--rw-rw-rw-   0        0        0     7492 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/modelhandler.py
--rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/openapiconfig.yaml
--rw-rw-rw-   0        0        0     7193 2022-12-20 15:16:57.000000 gramex-1.89.2/gramex/handlers/openapihandler.py
--rw-rw-rw-   0        0        0      818 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/handlers/pptxhandler.py
--rw-rw-rw-   0        0        0     6216 2022-11-23 03:19:45.000000 gramex-1.89.2/gramex/handlers/processhandler.py
--rw-rw-rw-   0        0        0     7715 2022-11-23 03:19:45.000000 gramex-1.89.2/gramex/handlers/proxyhandler.py
--rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.89.2/gramex/handlers/queryhandler.template.html
--rw-rw-rw-   0        0        0    11443 2022-11-23 03:19:45.000000 gramex-1.89.2/gramex/handlers/socialhandler.py
--rw-rw-rw-   0        0        0     9415 2022-11-23 03:19:45.000000 gramex-1.89.2/gramex/handlers/uploadhandler.py
--rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.89.2/gramex/handlers/websockethandler.py
--rw-rw-rw-   0        0        0     1458 2022-11-23 04:49:14.000000 gramex-1.89.2/gramex/http.py
--rw-rw-rw-   0        0        0    34944 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/install.py
--rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.89.2/gramex/license.py
--rw-rw-rw-   0        0        0     2005 2023-02-08 17:06:16.000000 gramex-1.89.2/gramex/migrate.py
--rw-rw-rw-   0        0        0    18498 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/ml.py
--rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/ml_api.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.833072 gramex-1.89.2/gramex/pptgen/
--rw-rw-rw-   0        0        0     9976 2022-11-23 04:49:14.000000 gramex-1.89.2/gramex/pptgen/__init__.py
--rw-rw-rw-   0        0        0    18876 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/pptgen/color.py
--rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.89.2/gramex/pptgen/colors.json
--rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.89.2/gramex/pptgen/commands.py
--rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.89.2/gramex/pptgen/fonts.json
--rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/pptgen/fontwidth.py
--rw-rw-rw-   0        0        0    26306 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/pptgen/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.841079 gramex-1.89.2/gramex/pptgen2/
--rw-rw-rw-   0        0        0    23501 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/pptgen2/__init__.py
--rw-rw-rw-   0        0        0    34484 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/pptgen2/commands.py
--rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/pptgen2/config.yaml
--rw-rw-rw-   0        0        0     4208 2022-11-23 04:49:14.000000 gramex-1.89.2/gramex/pynode.py
--rw-rw-rw-   0        0        0     2985 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/scale.py
--rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/secrets.py
--rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/servicenow.yaml
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.859952 gramex-1.89.2/gramex/services/
--rw-rw-rw-   0        0        0    39415 2023-02-08 17:06:16.000000 gramex-1.89.2/gramex/services/__init__.py
--rw-rw-rw-   0        0        0    10911 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/services/emailer.py
--rw-rw-rw-   0        0        0     3615 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/services/rediscache.py
--rw-rw-rw-   0        0        0     7164 2023-02-08 17:06:16.000000 gramex-1.89.2/gramex/services/scheduler.py
--rw-rw-rw-   0        0        0     3668 2022-11-06 08:24:30.000000 gramex-1.89.2/gramex/services/sms.py
--rw-rw-rw-   0        0        0     6385 2022-11-23 04:49:14.000000 gramex-1.89.2/gramex/services/ttlcache.py
--rw-rw-rw-   0        0        0     4529 2022-11-06 08:24:30.000000 gramex-1.89.2/gramex/services/urlcache.py
--rw-rw-rw-   0        0        0     5762 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/services/watcher.py
--rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/sm_api.py
--rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/topcause.py
--rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/transformers.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.874971 gramex-1.89.2/gramex/transforms/
--rw-rw-rw-   0        0        0      777 2022-11-23 04:49:14.000000 gramex-1.89.2/gramex/transforms/__init__.py
--rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.89.2/gramex/transforms/auth.py
--rw-rw-rw-   0        0        0     3542 2022-11-02 08:06:18.000000 gramex-1.89.2/gramex/transforms/template.py
--rw-rw-rw-   0        0        0    32281 2023-04-10 11:33:47.000000 gramex-1.89.2/gramex/transforms/transforms.py
--rw-rw-rw-   0        0        0    10122 2022-11-06 08:24:30.000000 gramex-1.89.2/gramex/transforms/twitterstream.py
--rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.89.2/gramex/winservice.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:50.837299 gramex-1.89.2/gramex.egg-info/
--rw-rw-rw-   0        0        0     2956 2023-04-11 12:21:47.000000 gramex-1.89.2/gramex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12426 2023-04-11 12:21:50.000000 gramex-1.89.2/gramex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 12:21:47.000000 gramex-1.89.2/gramex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-04-11 12:21:47.000000 gramex-1.89.2/gramex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      945 2023-04-11 12:21:47.000000 gramex-1.89.2/gramex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 12:21:47.000000 gramex-1.89.2/gramex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5972 2023-04-11 12:20:36.000000 gramex-1.89.2/pyproject.toml
--rw-rw-rw-   0        0        0      540 2023-04-11 12:21:52.016842 gramex-1.89.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 12:21:51.994426 gramex-1.89.2/tests/
--rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.89.2/tests/test_admin.py
--rw-rw-rw-   0        0        0     9054 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_alerts.py
--rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.89.2/tests/test_args.py
--rw-rw-rw-   0        0        0    38922 2023-04-10 11:33:47.000000 gramex-1.89.2/tests/test_auth.py
--rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.89.2/tests/test_cache.py
--rw-rw-rw-   0        0        0    15062 2022-11-23 04:49:14.000000 gramex-1.89.2/tests/test_capturehandler.py
--rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.89.2/tests/test_comichandler.py
--rw-rw-rw-   0        0        0    11152 2022-11-06 08:24:20.000000 gramex-1.89.2/tests/test_drivehandler.py
--rw-rw-rw-   0        0        0    17841 2022-11-06 08:24:20.000000 gramex-1.89.2/tests/test_filehandler.py
--rw-rw-rw-   0        0        0     6797 2022-11-24 04:51:52.000000 gramex-1.89.2/tests/test_filterhandler.py
--rw-rw-rw-   0        0        0    35746 2023-01-03 16:10:30.000000 gramex-1.89.2/tests/test_formhandler.py
--rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.89.2/tests/test_functionhandler.py
--rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.89.2/tests/test_gramexlog.py
--rw-rw-rw-   0        0        0    15699 2022-11-23 04:49:14.000000 gramex-1.89.2/tests/test_handlers.py
--rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_init.py
--rw-rw-rw-   0        0        0     8931 2022-11-23 04:49:14.000000 gramex-1.89.2/tests/test_install.py
--rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.89.2/tests/test_jsonhandler.py
--rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.89.2/tests/test_ldapauth.py
--rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_logviewer.py
--rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.89.2/tests/test_mlhandler.py
--rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_modelhandler.py
--rw-rw-rw-   0        0        0     7082 2022-12-20 15:16:57.000000 gramex-1.89.2/tests/test_openapihandler.py
--rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_pptxhandler.py
--rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.89.2/tests/test_processhandler.py
--rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.89.2/tests/test_proxyhandler.py
--rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_pynode.py
--rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.89.2/tests/test_schedule.py
--rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.89.2/tests/test_secrets.py
--rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.89.2/tests/test_sms.py
--rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.89.2/tests/test_subapp.py
--rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_subprocess.py
--rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_translater.py
--rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.89.2/tests/test_twitterresthandler.py
--rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.89.2/tests/test_ui.py
--rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_update.py
--rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.89.2/tests/test_uploadhandler.py
--rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.89.2/tests/test_watcher.py
--rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.89.2/tests/test_websockethandler.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.808865 gramex-1.90.0/
+-rw-rw-rw-   0        0        0     1900 2023-04-10 11:33:47.000000 gramex-1.90.0/.gitignore
+-rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.90.0/LICENSE
+-rw-rw-rw-   0        0        0      641 2023-04-11 12:20:36.000000 gramex-1.90.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2956 2023-05-07 15:53:06.808865 gramex-1.90.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.90.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.110353 gramex-1.90.0/gramex/
+-rw-rw-rw-   0        0        0    15366 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/__init__.py
+-rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.90.0/gramex/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.194902 gramex-1.90.0/gramex/apps/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.90.0/gramex/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.202226 gramex-1.90.0/gramex/apps/admin/
+-rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.90.0/gramex/apps/admin/.gitignore
+-rw-rw-rw-   0        0        0      129 2023-01-03 16:10:30.000000 gramex-1.90.0/gramex/apps/admin/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.239841 gramex-1.90.0/gramex/apps/admin2/
+-rw-rw-rw-   0        0        0      226 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/apps/admin2/.snyk
+-rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.90.0/gramex/apps/admin2/admin.css
+-rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/admin2/gramex.yaml
+-rw-rw-rw-   0        0        0    12257 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/apps/admin2/gramexadmin.py
+-rw-rw-rw-   0        0        0     8420 2023-04-24 07:27:25.000000 gramex-1.90.0/gramex/apps/admin2/index.html
+-rw-rw-rw-   0        0        0     5216 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/admin2/schedule.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.260237 gramex-1.90.0/gramex/apps/capture/
+-rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/capture/README.md
+-rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/capture/capture.js
+-rw-rw-rw-   0        0        0    12034 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/capture/chromecapture.js
+-rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/capture/index.html
+-rw-rw-rw-   0        0        0   141595 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/capture/package-lock.json
+-rw-rw-rw-   0        0        0      863 2023-02-08 17:06:15.000000 gramex-1.90.0/gramex/apps/capture/package.json
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.291007 gramex-1.90.0/gramex/apps/filemanager/
+-rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.90.0/gramex/apps/filemanager/.snyk
+-rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.90.0/gramex/apps/filemanager/README.html
+-rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/filemanager/drivehandler-snippet.html
+-rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.90.0/gramex/apps/filemanager/filemanager-snippet.html
+-rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.90.0/gramex/apps/filemanager/filemanager.html
+-rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/filemanager/filemanager.js
+-rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.90.0/gramex/apps/filemanager/filemanager.py
+-rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/filemanager/gramex.yaml
+-rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/filemanager/index.html
+-rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/filemanager/navbar.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:04.945276 gramex-1.90.0/gramex/apps/init/
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.337348 gramex-1.90.0/gramex/apps/init/default/
+-rw-rw-rw-   0        0        0      578 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/.eslintrc.yml
+-rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/init/default/.flake8
+-rw-rw-rw-   0        0        0      756 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.90.0/gramex/apps/init/default/.secrets.yaml
+-rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.90.0/gramex/apps/init/default/.template.gitignore
+-rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/init/default/README.template.md
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.337348 gramex-1.90.0/gramex/apps/init/default/assets/
+-rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/init/default/assets/README.template.md
+-rw-rw-rw-   0        0        0     1756 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/gramex.template.yaml
+-rw-rw-rw-   0        0        0      694 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/index.template.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.337348 gramex-1.90.0/gramex/apps/init/default/js/
+-rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/init/default/js/README.template.md
+-rw-rw-rw-   0        0        0     2608 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/login.template.html
+-rw-rw-rw-   0        0        0      352 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/package.template.json
+-rw-rw-rw-   0        0        0       80 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/style.scss
+-rw-rw-rw-   0        0        0     3499 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/template-navbar.template.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.337348 gramex-1.90.0/gramex/apps/init/ide/
+-rw-rw-rw-   0        0        0      378 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/ide/.gitlab-ci.template.yml
+-rw-rw-rw-   0        0        0      244 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/ide/gramex.template.yaml
+-rw-rw-rw-   0        0        0      738 2023-04-24 06:54:58.000000 gramex-1.90.0/gramex/apps/init/ide/index.template.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.354087 gramex-1.90.0/gramex/apps/init/minimal/
+-rw-rw-rw-   0        0        0      247 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/minimal/gramex.template.yaml
+-rw-rw-rw-   0        0        0      757 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/minimal/index.template.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.368927 gramex-1.90.0/gramex/apps/languagetool/
+-rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/languagetool/README.md
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.90.0/gramex/apps/languagetool/__init__.py
+-rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/languagetool/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.429595 gramex-1.90.0/gramex/apps/logviewer/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.90.0/gramex/apps/logviewer/__init__.py
+-rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/logviewer/config.yaml
+-rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/logviewer/gramex.yaml
+-rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/logviewer/index.html
+-rw-rw-rw-   0        0        0    13287 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/apps/logviewer/logviewer.py
+-rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.90.0/gramex/apps/logviewer/lv-card-deck.html
+-rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-card.html
+-rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-datepicker.html
+-rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-dropdown.html
+-rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.90.0/gramex/apps/logviewer/lv-filters.html
+-rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-header.html
+-rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-kpi.html
+-rw-rw-rw-   0        0        0      775 2023-05-07 15:42:40.000000 gramex-1.90.0/gramex/apps/logviewer/package-lock.json
+-rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.90.0/gramex/apps/logviewer/package.json
+-rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/logviewer/render.js
+-rw-rw-rw-   0        0        0     5390 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/apps/logviewer/script.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.447178 gramex-1.90.0/gramex/apps/mail/
+-rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/mail/gramex.yaml
+-rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.90.0/gramex/apps/mail/index.html
+-rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.90.0/gramex/apps/mail/mailapp.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.447178 gramex-1.90.0/gramex/apps/mlhandler/
+-rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.90.0/gramex/apps/mlhandler/template.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.466873 gramex-1.90.0/gramex/apps/pynode/
+-rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.90.0/gramex/apps/pynode/.snyk
+-rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.90.0/gramex/apps/pynode/README.md
+-rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/pynode/index.js
+-rw-rw-rw-   0        0        0     2953 2023-05-07 15:42:44.000000 gramex-1.90.0/gramex/apps/pynode/package-lock.json
+-rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.90.0/gramex/apps/pynode/package.json
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.480425 gramex-1.90.0/gramex/apps/smartalerts/
+-rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.90.0/gramex/apps/smartalerts/gramex.yaml
+-rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.90.0/gramex/apps/smartalerts/index.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.511699 gramex-1.90.0/gramex/apps/ui/
+-rw-rw-rw-   0        0        0     1019 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/apps/ui/.snyk
+-rw-rw-rw-   0        0        0    12878 2022-12-20 15:16:57.000000 gramex-1.90.0/gramex/apps/ui/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-04-24 07:13:24.000000 gramex-1.90.0/gramex/apps/ui/bootstrap-theme.scss
+-rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/config.yaml
+-rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.90.0/gramex/apps/ui/gramex.yaml
+-rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/gramexui.scss
+-rw-rw-rw-   0        0        0   588333 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/ui/package-lock.json
+-rw-rw-rw-   0        0        0      341 2023-04-11 12:20:36.000000 gramex-1.90.0/gramex/apps/ui/package.json
+-rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.90.0/gramex/apps/ui/setup.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.524255 gramex-1.90.0/gramex/apps/ui/theme/
+-rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/bootstrap5.scss
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.736434 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/
+-rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cerulean.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cerulean.scss
+-rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cosmo.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cosmo.scss
+-rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cyborg.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cyborg.scss
+-rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/darkly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/darkly.scss
+-rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/flatly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/flatly.scss
+-rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/journal.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/journal.scss
+-rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/litera.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/litera.scss
+-rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lumen.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lumen.scss
+-rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lux.png
+-rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lux.scss
+-rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/materia.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/materia.scss
+-rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/minty.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/minty.scss
+-rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/pulse.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/pulse.scss
+-rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sandstone.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sandstone.scss
+-rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/simplex.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/simplex.scss
+-rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sketchy.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sketchy.scss
+-rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/slate.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/slate.scss
+-rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/solar.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/solar.scss
+-rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/spacelab.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/spacelab.scss
+-rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/superhero.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/superhero.scss
+-rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/united.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/united.scss
+-rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/yeti.png
+-rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/yeti.scss
+-rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/default.png
+-rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.90.0/gramex/apps/ui/theme/default.scss
+-rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/index.html
+-rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/sample.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.838240 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/
+-rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png
+-rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
+-rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/boldstrap.png
+-rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/boldstrap.scss
+-rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
+-rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
+-rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/darkster.png
+-rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/darkster.scss
+-rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/fresca.png
+-rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/fresca.scss
+-rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/greyson.png
+-rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/greyson.scss
+-rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
+-rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
+-rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/herbie.png
+-rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/herbie.scss
+-rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hootstrap.png
+-rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hootstrap.scss
+-rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/lovey.png
+-rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/lovey.scss
+-rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/monotony.png
+-rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/monotony.scss
+-rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/poypull.png
+-rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/poypull.scss
+-rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/signal.png
+-rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/signal.scss
+-rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/tequila.png
+-rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/tequila.scss
+-rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.90.0/gramex/apps/ui/theme/themes.json
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.952648 gramex-1.90.0/gramex/apps/uifactory/
+-rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/uifactory/.eslintrc.js
+-rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/.gitattributes
+-rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.952648 gramex-1.90.0/gramex/apps/uifactory/assets/
+-rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/assets/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.959658 gramex-1.90.0/gramex/apps/uifactory/assets/data/
+-rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.90.0/gramex/apps/uifactory/assets/data/input.json
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.959658 gramex-1.90.0/gramex/apps/uifactory/assets/img/
+-rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.90.0/gramex/apps/uifactory/assets/img/arrows-move.svg
+-rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.90.0/gramex/apps/uifactory/assets/img/clipboard.svg
+-rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
+-rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.90.0/gramex/apps/uifactory/assets/img/trash.svg
+-rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/create.html
+-rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/edit.html
+-rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/field-actions.html
+-rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.90.0/gramex/apps/uifactory/form_builder.py
+-rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/gramex.yaml
+-rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/index.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.993004 gramex-1.90.0/gramex/apps/uifactory/js/
+-rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/README.md
+-rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/embed.js
+-rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/fields.js
+-rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/fork-form.js
+-rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/index.js
+-rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/script.js
+-rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/utils.js
+-rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/viewform.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.010178 gramex-1.90.0/gramex/apps/uifactory/modals/
+-rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/add-field.html
+-rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/embed.html
+-rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/remove.html
+-rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/rename.html
+-rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/themes.html
+-rw-rw-rw-   0        0        0     5781 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/uifactory/package-lock.json
+-rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.90.0/gramex/apps/uifactory/package.json
+-rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/popover-form.html
+-rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/sample.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.017264 gramex-1.90.0/gramex/apps/uifactory/snippets/
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.021247 gramex-1.90.0/gramex/apps/uifactory/snippets/button/
+-rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/button/bs4-button.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.024264 gramex-1.90.0/gramex/apps/uifactory/snippets/checkbox/
+-rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.036034 gramex-1.90.0/gramex/apps/uifactory/snippets/email/
+-rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/email/bs4-email.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.038838 gramex-1.90.0/gramex/apps/uifactory/snippets/hidden/
+-rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.049232 gramex-1.90.0/gramex/apps/uifactory/snippets/html/
+-rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/html/bs4-html.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.049232 gramex-1.90.0/gramex/apps/uifactory/snippets/multiselect/
+-rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.057921 gramex-1.90.0/gramex/apps/uifactory/snippets/number/
+-rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/number/bs4-number.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.063055 gramex-1.90.0/gramex/apps/uifactory/snippets/password/
+-rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/password/bs4-password.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.067634 gramex-1.90.0/gramex/apps/uifactory/snippets/radio/
+-rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.075899 gramex-1.90.0/gramex/apps/uifactory/snippets/range/
+-rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/range/bs4-range.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.079284 gramex-1.90.0/gramex/apps/uifactory/snippets/select/
+-rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/select/bs4-select.js
+-rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/setup.js
+-rw-rw-rw-   0        0        0        3 2023-04-17 10:18:07.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/snippets.json
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.084684 gramex-1.90.0/gramex/apps/uifactory/snippets/text/
+-rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/text/bs4-text.js
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.091213 gramex-1.90.0/gramex/apps/uifactory/snippets/textarea/
+-rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
+-rw-rw-rw-   0        0        0     1815 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/uifactory/style.scss
+-rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/template-navbar-view-form.html
+-rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/template-navbar.html
+-rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/toast.html
+-rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/viewform.html
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.109236 gramex-1.90.0/gramex/apps/update/
+-rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.90.0/gramex/apps/update/README.md
+-rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/update/gramex.yaml
+-rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.90.0/gramex/apps/update/gramexupdate.py
+-rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.90.0/gramex/apps/update/index.html
+-rw-rw-rw-   0        0        0      277 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps.yaml
+-rw-rw-rw-   0        0        0    56930 2023-04-15 03:29:37.000000 gramex-1.90.0/gramex/cache.py
+-rw-rw-rw-   0        0        0    35221 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/config.py
+-rw-rw-rw-   0        0        0    93430 2023-04-20 06:58:42.000000 gramex-1.90.0/gramex/data.py
+-rw-rw-rw-   0        0        0     6353 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/debug.py
+-rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/deploy.yaml
+-rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/download.vega.js
+-rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.90.0/gramex/favicon.ico
+-rw-rw-rw-   0        0        0    16670 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/gramex.yaml
+-rw-rw-rw-   0        0        0     2011 2023-04-18 07:09:40.000000 gramex-1.90.0/gramex/gramexfeatures.csv
+-rw-rw-rw-   0        0        0    14445 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/gramexsize.csv
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.309057 gramex-1.90.0/gramex/handlers/
+-rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/400.html
+-rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/401.html
+-rw-rw-rw-   0        0        0     2374 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/403.html
+-rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/404.html
+-rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/500.html
+-rw-rw-rw-   0        0        0     2643 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/handlers/__init__.py
+-rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/auth.recaptcha.template.html
+-rw-rw-rw-   0        0        0     3862 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/handlers/auth.template.html
+-rw-rw-rw-   0        0        0    17394 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/handlers/authhandler.py
+-rw-rw-rw-   0        0        0    60917 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/handlers/basehandler.py
+-rw-rw-rw-   0        0        0    15648 2022-12-20 15:16:57.000000 gramex-1.90.0/gramex/handlers/capturehandler.py
+-rw-rw-rw-   0        0        0     1477 2022-11-06 08:24:25.000000 gramex-1.90.0/gramex/handlers/comichandler.py
+-rw-rw-rw-   0        0        0     8922 2022-11-06 08:24:26.000000 gramex-1.90.0/gramex/handlers/drivehandler.py
+-rw-rw-rw-   0        0        0    14849 2023-02-24 08:15:32.000000 gramex-1.90.0/gramex/handlers/filehandler.py
+-rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.90.0/gramex/handlers/filehandler.template.html
+-rw-rw-rw-   0        0        0      198 2023-01-03 16:10:30.000000 gramex-1.90.0/gramex/handlers/filterhandler.py
+-rw-rw-rw-   0        0        0    13238 2023-01-03 16:10:30.000000 gramex-1.90.0/gramex/handlers/formhandler.py
+-rw-rw-rw-   0        0        0     3774 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/functionhandler.py
+-rw-rw-rw-   0        0        0     6622 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/jsonhandler.py
+-rw-rw-rw-   0        0        0     6838 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/handlers/messagehandler.py
+-rw-rw-rw-   0        0        0    16154 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/handlers/mlhandler.py
+-rw-rw-rw-   0        0        0     7492 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/modelhandler.py
+-rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/openapiconfig.yaml
+-rw-rw-rw-   0        0        0     7193 2022-12-20 15:16:57.000000 gramex-1.90.0/gramex/handlers/openapihandler.py
+-rw-rw-rw-   0        0        0      818 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/pptxhandler.py
+-rw-rw-rw-   0        0        0     6216 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/processhandler.py
+-rw-rw-rw-   0        0        0     7715 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/proxyhandler.py
+-rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.90.0/gramex/handlers/queryhandler.template.html
+-rw-rw-rw-   0        0        0    11443 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/socialhandler.py
+-rw-rw-rw-   0        0        0     9415 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/uploadhandler.py
+-rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/websockethandler.py
+-rw-rw-rw-   0        0        0     1458 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/http.py
+-rw-rw-rw-   0        0        0    35070 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/install.py
+-rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.90.0/gramex/license.py
+-rw-rw-rw-   0        0        0     2005 2023-02-08 17:06:16.000000 gramex-1.90.0/gramex/migrate.py
+-rw-rw-rw-   0        0        0    18498 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/ml.py
+-rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/ml_api.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.542414 gramex-1.90.0/gramex/pptgen/
+-rw-rw-rw-   0        0        0     9976 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/pptgen/__init__.py
+-rw-rw-rw-   0        0        0    18876 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/pptgen/color.py
+-rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.90.0/gramex/pptgen/colors.json
+-rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/pptgen/commands.py
+-rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.90.0/gramex/pptgen/fonts.json
+-rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/pptgen/fontwidth.py
+-rw-rw-rw-   0        0        0    26306 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/pptgen/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.542414 gramex-1.90.0/gramex/pptgen2/
+-rw-rw-rw-   0        0        0    23501 2023-04-26 11:16:23.000000 gramex-1.90.0/gramex/pptgen2/__init__.py
+-rw-rw-rw-   0        0        0    34484 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/pptgen2/commands.py
+-rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/pptgen2/config.yaml
+-rw-rw-rw-   0        0        0     4208 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/pynode.py
+-rw-rw-rw-   0        0        0     2985 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/scale.py
+-rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/secrets.py
+-rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/servicenow.yaml
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.604612 gramex-1.90.0/gramex/services/
+-rw-rw-rw-   0        0        0    39493 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/services/__init__.py
+-rw-rw-rw-   0        0        0    11176 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/services/emailer.py
+-rw-rw-rw-   0        0        0     3615 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/services/rediscache.py
+-rw-rw-rw-   0        0        0     7164 2023-02-08 17:06:16.000000 gramex-1.90.0/gramex/services/scheduler.py
+-rw-rw-rw-   0        0        0     3668 2022-11-06 08:24:30.000000 gramex-1.90.0/gramex/services/sms.py
+-rw-rw-rw-   0        0        0     6385 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/services/ttlcache.py
+-rw-rw-rw-   0        0        0     4529 2022-11-06 08:24:30.000000 gramex-1.90.0/gramex/services/urlcache.py
+-rw-rw-rw-   0        0        0     5762 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/services/watcher.py
+-rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/sm_api.py
+-rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/topcause.py
+-rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/transformers.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.623721 gramex-1.90.0/gramex/transforms/
+-rw-rw-rw-   0        0        0      777 2023-04-14 07:12:43.000000 gramex-1.90.0/gramex/transforms/__init__.py
+-rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.90.0/gramex/transforms/auth.py
+-rw-rw-rw-   0        0        0     3542 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/transforms/template.py
+-rw-rw-rw-   0        0        0    32281 2023-04-14 04:57:01.000000 gramex-1.90.0/gramex/transforms/transforms.py
+-rw-rw-rw-   0        0        0    10122 2022-11-06 08:24:30.000000 gramex-1.90.0/gramex/transforms/twitterstream.py
+-rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.90.0/gramex/winservice.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.191893 gramex-1.90.0/gramex.egg-info/
+-rw-rw-rw-   0        0        0     2956 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11970 2023-05-07 15:53:04.000000 gramex-1.90.0/gramex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      945 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6088 2023-05-07 15:51:36.000000 gramex-1.90.0/pyproject.toml
+-rw-rw-rw-   0        0        0      540 2023-05-07 15:53:06.841813 gramex-1.90.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.808865 gramex-1.90.0/tests/
+-rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.90.0/tests/test_admin.py
+-rw-rw-rw-   0        0        0     9054 2023-04-18 08:45:54.000000 gramex-1.90.0/tests/test_alerts.py
+-rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.90.0/tests/test_args.py
+-rw-rw-rw-   0        0        0    39027 2023-05-07 15:51:36.000000 gramex-1.90.0/tests/test_auth.py
+-rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.90.0/tests/test_cache.py
+-rw-rw-rw-   0        0        0    15062 2022-11-23 04:49:14.000000 gramex-1.90.0/tests/test_capturehandler.py
+-rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.90.0/tests/test_comichandler.py
+-rw-rw-rw-   0        0        0    11152 2022-11-06 08:24:20.000000 gramex-1.90.0/tests/test_drivehandler.py
+-rw-rw-rw-   0        0        0    17841 2022-11-06 08:24:20.000000 gramex-1.90.0/tests/test_filehandler.py
+-rw-rw-rw-   0        0        0     6797 2022-11-24 04:51:52.000000 gramex-1.90.0/tests/test_filterhandler.py
+-rw-rw-rw-   0        0        0    35746 2023-01-03 16:10:30.000000 gramex-1.90.0/tests/test_formhandler.py
+-rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.90.0/tests/test_functionhandler.py
+-rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.90.0/tests/test_gramexlog.py
+-rw-rw-rw-   0        0        0    15699 2022-11-23 04:49:14.000000 gramex-1.90.0/tests/test_handlers.py
+-rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_init.py
+-rw-rw-rw-   0        0        0     8931 2022-11-23 04:49:14.000000 gramex-1.90.0/tests/test_install.py
+-rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.90.0/tests/test_jsonhandler.py
+-rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.90.0/tests/test_ldapauth.py
+-rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_logviewer.py
+-rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.90.0/tests/test_mlhandler.py
+-rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_modelhandler.py
+-rw-rw-rw-   0        0        0     7082 2022-12-20 15:16:57.000000 gramex-1.90.0/tests/test_openapihandler.py
+-rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_pptxhandler.py
+-rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_processhandler.py
+-rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_proxyhandler.py
+-rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_pynode.py
+-rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_schedule.py
+-rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.90.0/tests/test_secrets.py
+-rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.90.0/tests/test_sms.py
+-rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.90.0/tests/test_subapp.py
+-rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_subprocess.py
+-rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_translater.py
+-rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_twitterresthandler.py
+-rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_ui.py
+-rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_update.py
+-rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.90.0/tests/test_uploadhandler.py
+-rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_watcher.py
+-rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.90.0/tests/test_websockethandler.py
```

### Comparing `gramex-1.89.2/.gitignore` & `gramex-1.90.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/LICENSE` & `gramex-1.90.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/MANIFEST.in` & `gramex-1.90.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/PKG-INFO` & `gramex-1.90.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.89.2
+Version: 1.90.0
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.89.2/README.md` & `gramex-1.90.0/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/__init__.py` & `gramex-1.90.0/gramex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,26 +39,26 @@
 Helper applications. For usage, run "gramex <app> --help"
 
 gramex init                   Add Gramex project scaffolding to current dir
 gramex service                Windows service setup
 gramex mail                   Send email from command line
 gramex license                See Gramex license, accept or reject it
 gramex features               List features of Gramex used in the current project
+gramex complexity             Calculate cyclomatic complexity of the project
 
 Installation commands. For usage, run "gramex <command> --help"
 
 gramex install                Install an app
 gramex update                 Update an app
 gramex setup                  Run make, npm install, bower install etc on app
 gramex run                    Run an installed app
 gramex uninstall              Uninstall an app
-gramex complexity             Calculate cyclomatic complexity of the project
 '''
 
-__version__ = '1.89.2'
+__version__ = '1.90.0'
 
 paths = AttrDict()  # Paths where configurations are stored
 conf = AttrDict()  # Final merged configurations
 config_layers = ChainConfig()  # Loads all configurations. init() updates it
 appconfig = AttrDict()  # Final app configuration
 
 paths['source'] = Path(__file__).absolute().parent  # Where gramex source code is
@@ -112,15 +112,15 @@
 
     Values are parsed as YAML, e.g. `null` becomes `None`.
 
     If the keyword arguments include `--help`, it prints the usage of that function and exits.
     '''
     commands = sys.argv[1:] if args is None else args
 
-    # t first, setup log: service at INFO to log progress. App's log: may override this later.
+    # First, setup log: service at INFO to log progress. App's log: may override this later.
     log_config = (+PathConfig(paths['source'] / 'gramex.yaml')).get('log', AttrDict())
     log_config.loggers.gramex.level = logging.INFO
     from . import services
 
     services.log(log_config)
 
     # kwargs has all optional command line args as a dict of values / lists.
```

### Comparing `gramex-1.89.2/gramex/apps/admin2/gramex.yaml` & `gramex-1.90.0/gramex/apps/admin2/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/admin2/gramexadmin.py` & `gramex-1.90.0/gramex/apps/admin2/gramexadmin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/admin2/index.html` & `gramex-1.90.0/gramex/apps/admin2/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/admin2/schedule.js` & `gramex-1.90.0/gramex/apps/admin2/schedule.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,99 +1,169 @@
-(function(factory) {
-    typeof define === "function" && define.amd ? define(factory) : factory();
-})(function() {
-    "use strict";
-
-    var base_template =
-        '<div class="schedule-formhandler"></div><div class="schedule-logs"></div>';
-    var name_template = "<td><%- _.last((obj.value || '').split(/:/)) %></td>";
-    var actions_schedule_template =
-        '<td><button class="run btn btn-primary btn-xs" title="Run now" data-name="<%- row.name %>"><i class="fa fa-play"></i></button></td>';
-    var actions_alert_template =
-        '<td><button class="run btn btn-primary btn-xs" title="Send alert now" data-name="<%- row.name %>"><i class="fa fa-envelope"></i></button><button class="run btn btn-success btn-xs ml-1" title="Preview results" data-name="<%- row.name %>" data-mock="true"><i class="fa fa-eye"></i></button></td>';
-    var notification_template =
-        "<div class=\"alert alert-<%- obj.error ? 'danger' : 'success' %> alert-dismissible fade show\" role=\"alert\"><button type=\"button\" class=\"close\" data-dismiss=\"alert\" aria-label=\"Close\"><span aria-hidden=\"true\">×</span></button><div><strong><%- name %></strong> <% if (obj.error) { %> <%= obj.traceback || '' %> <% } else { %> <div><%- obj.mock ? 'Previewed successfully.' : 'Ran successfully.' %></div> <% } %> </div> <% _.each(obj.results, function (row) { %> <table class=\"table table-sm bg-white mt-3\"><tbody> <% _.each(['to', 'cc', 'bcc', 'from', 'reply_to', 'on_behalf_of', 'subject'], function (key) { %> <% if (key in row) { %> <tr><th><%- key %></th><td><%- row[key] %></td></tr> <% } %> <% }) %> <% if (row.body) { %><tr><th>body</th><td><%- row.body %></td></tr><% } %> <% if (row.html) { %><tr><th>html</th><td><%= row.html %></td></tr><% } %> <% if (row.attachments) { %> <tr><th>attachments</th><td><ul> <% _.each(row.attachments, function (path) { %> <li><%- path %></li> <% }) %> </ul></td></tr> <% } %> </tbody></table> <% }) %> </div>";
-    var function_template =
-        "<td><pre class=\"mb-0 pre-wrap\"><%- value %></pre> <% var args = JSON.parse(row.args), kwargs = JSON.parse(row.kwargs) %> <% if (_.size(args) + _.size(kwargs)) { %> <div><a data-toggle=\"collapse\" href=\"#kwargs<%- index %>\" class=\"sm1\">Expand arguments...</a></div><div class=\"collapse\" id=\"kwargs<%- index %>\"> <%= _.size(args) ? '<pre>' + JSON.stringify(args, null, 2) + '</pre>' : '' %> <%= _.size(kwargs) ? '<pre>' + JSON.stringify(kwargs, null, 2) + '</pre>' : '' %> </div> <% } %> </td>";
-    var schedule_template =
-        "<td><div><%- row.schedule %></div><div class=\"small\"><%- row.next ? moment.utc(row.next).fromNow() : '' %></div></td>";
-
-    /* eslint-env browser, jquery */
-
-    var notification_msg = _.template(notification_template);
-
-    function notify(el, obj) {
-        $(el).prepend(notification_msg(obj)).get(0).scrollIntoView();
-    }
-
-    $.fn.schedule = function(options) {
-        this.each(function() {
-            var self = $(this);
-            self.html(base_template);
-            var logs = self.find(".schedule-logs");
-            self.find(".schedule-formhandler").formhandler({
-                src: options.url,
-                columns: [{
-                    name: "actions",
-                    template: options.alert ?
-                        actions_alert_template :
-                        actions_schedule_template,
-                }, {
-                    name: "name",
-                    template: name_template
-                }, {
-                    name: "function",
-                    template: function_template
-                }, {
-                    name: "next",
-                    title: "schedule",
-                    type: "date",
-                    template: schedule_template,
-                }, {
-                    name: "startup"
-                }, {
-                    name: "thread"
-                }, ],
-                page: false,
-                pageSize: 1000,
-                export: false,
-            });
-            self.on("click", ".run", function() {
-                var $this = $(this);
-                var $icon = $(".fa", this).toggleClass("fa-play fa-spinner fa-spin");
-                $icon.parent(".btn").prop("disabled", true);
-                var name = $this.data("name");
-                var shortname = _.last((name || "").split(/:/));
-                $.ajax(options.url, {
-                        method: "POST",
-                        data: {
-                            name: name,
-                            _xsrf: options.xsrf,
-                            mock: $this.data("mock")
-                        },
-                    })
-                    .done(function(results) {
-                        notify(logs, {
-                            name: shortname,
-                            results: results,
-                            mock: $this.data("mock"),
-                        });
-                    })
-                    .fail(function(xhr, err, msg) {
-                        var error = $(xhr.responseText);
-                        notify(logs, {
-                            name: shortname,
-                            results: [],
-                            error: error.filter("section.content").find("pre").html() ||
-                                msg ||
-                                "Error",
-                            traceback: error.filter("#traceback").html() || "Unknown error",
-                        });
-                    })
-                    .always(function() {
-                        $icon.toggleClass("fa-play fa-spinner fa-spin");
-                        $icon.parent(".btn").prop("disabled", false);
+/* eslint-env jquery */
+/* globals _ */
+
+const base_template = /* html */ `
+  <div class="schedule-formhandler"></div>
+  <div class="schedule-logs"></div>
+`;
+
+const name_template = /* html */ `<td><%- _.last((obj.value || '').split(/:/)) %></td>`;
+
+const actions_schedule_template = /* html */ `
+  <td>
+    <button class="run btn btn-primary btn-xs" title="Run now" data-name="<%- row.name %>">
+      <i class="fa fa-play"></i>
+    </button>
+  </td>
+`;
+
+const actions_alert_template = /* html */ `
+  <td>
+    <button class="run btn btn-primary btn-xs" title="Send alert now" data-name="<%- row.name %>">
+      <i class="fa fa-envelope"></i>
+    </button>
+    <button class="run btn btn-success btn-xs ml-1" title="Preview results" data-name="<%- row.name %>" data-mock="true">
+      <i class="fa fa-eye"></i>
+    </button>
+  </td>
+`;
+
+const notification_template = /* html */ `
+  <div class="alert alert-<%- obj.error ? 'danger' : 'success' %> alert-dismissible fade show" role="alert">
+    <button type="button" class="close" data-dismiss="alert" aria-label="Close">
+      <span aria-hidden="true">&times;</span>
+    </button>
+    <div>
+      <strong><%- name %></strong>
+      <% if (obj.error) { %>
+        <%= obj.traceback || '' %>
+      <% } else { %>
+        <div><%- obj.mock ? 'Previewed successfully.' : 'Ran successfully.' %></div>
+      <% } %>
+    </div>
+    <% _.each(obj.results, function (row) { %>
+      <table class="table table-sm bg-white mt-3">
+        <tbody>
+          <% _.each(['to', 'cc', 'bcc', 'from', 'reply_to', 'on_behalf_of', 'subject'], function (key) { %>
+            <% if (key in row) { %>
+              <tr>
+                <th><%- key %></th>
+                <td><%- row[key] %></td>
+              </tr>
+            <% } %>
+          <% }) %>
+          <% if (row.body) { %><tr><th>body</th><td><%- row.body %></td></tr><% } %>
+          <% if (row.html) { %><tr><th>html</th><td><%= row.html %></td></tr><% } %>
+          <% if (row.attachments) { %>
+            <tr>
+              <th>attachments</th>
+              <td><ul>
+                <% _.each(row.attachments, function (path) { %>
+                  <li><%- path %></li>
+                <% }) %>
+              </ul></td>
+            </tr>
+          <% } %>
+        </tbody>
+      </table>
+    <% }) %>
+  </div>
+`;
+
+const function_template = /* html */ `
+  <td>
+    <pre class="mb-0 pre-wrap"><%- value %></pre>
+    <% const args = JSON.parse(row.args), kwargs = JSON.parse(row.kwargs) %>
+    <% if (_.size(args) + _.size(kwargs)) { %>
+    <div><a data-toggle="collapse" href="#kwargs<%- index %>" class="sm1">Expand arguments...</a></div>
+    <div class="collapse" id="kwargs<%- index %>">
+      <%= _.size(args) ? '<pre>' + JSON.stringify(args, null, 2) + '</pre>' : '' %>
+      <%= _.size(kwargs) ? '<pre>' + JSON.stringify(kwargs, null, 2) + '</pre>' : '' %>
+    </div>
+    <% } %>
+  </td>
+`;
+
+const schedule_template = /* html */ `
+  <td>
+    <div><%- row.schedule %></div>
+    <div class="small"><%- row.next ? moment.utc(row.next).fromNow() : '' %></div>
+  </td>
+`;
+
+const notification_msg = _.template(notification_template);
+
+function notify(el, obj) {
+    $(el).prepend(notification_msg(obj)).get(0).scrollIntoView();
+}
+
+$.fn.schedule = function(options) {
+    this.each(function() {
+        const self = $(this);
+        self.html(base_template);
+        const logs = self.find(".schedule-logs");
+        self.find(".schedule-formhandler").formhandler({
+            src: options.url,
+            columns: [{
+                name: "actions",
+                template: options.alert ?
+                    actions_alert_template :
+                    actions_schedule_template,
+            }, {
+                name: "name",
+                template: name_template
+            }, {
+                name: "function",
+                template: function_template
+            }, {
+                name: "next",
+                title: "schedule",
+                type: "date",
+                template: schedule_template,
+            }, {
+                name: "startup"
+            }, {
+                name: "thread"
+            }, ],
+            page: false,
+            pageSize: 1000,
+            export: false,
+        });
+        self.on("click", ".run", function() {
+            const $this = $(this);
+            const $icon = $(".fa", this).toggleClass("fa-play fa-spinner fa-spin");
+            $icon.parent(".btn").prop("disabled", true);
+            const name = $this.data("name");
+            const shortname = _.last((name || "").split(/:/));
+            $.ajax(options.url, {
+                    method: "POST",
+                    data: {
+                        name: name,
+                        _xsrf: options.xsrf,
+                        mock: $this.data("mock")
+                    },
+                })
+                .done(function(results) {
+                    notify(logs, {
+                        name: shortname,
+                        results: results,
+                        mock: $this.data("mock"),
+                    });
+                })
+                .fail(function(xhr, err, msg) {
+                    const error = $(xhr.responseText);
+                    notify(logs, {
+                        name: shortname,
+                        results: [],
+                        error: error.filter("section.content").find("pre").html() ||
+                            msg ||
+                            "Error",
+                        traceback: error.filter("#traceback").html() || "Unknown error",
                     });
-            });
+                })
+                .always(function() {
+                    $icon.toggleClass("fa-play fa-spinner fa-spin");
+                    $icon.parent(".btn").prop("disabled", false);
+                });
         });
-    };
-});
+    });
+};
```

### Comparing `gramex-1.89.2/gramex/apps/capture/README.md` & `gramex-1.90.0/gramex/apps/capture/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/capture/capture.js` & `gramex-1.90.0/gramex/apps/capture/capture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/capture/chromecapture.js` & `gramex-1.90.0/gramex/apps/capture/chromecapture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/capture/index.html` & `gramex-1.90.0/gramex/apps/capture/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/capture/package-lock.json` & `gramex-1.90.0/gramex/apps/capture/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992909918044349%*

 * *Differences: {"'dependencies'": "{'@puppeteer/browsers': {'version': '0.5.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@puppeteer/browsers/-/browsers-0.5.0.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-Uw6oB7VvmPRLE4iKsjuOh8zgDabhNX67dzo8U/BB0f9527qx+4eeUs+korU98OhG5C4ubg7ufBgVi63XYwS6TQ=='}, "*

 * *                   "'@types/node': {'version': '20.1.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz', 'integrity': "*

 * *                  […]*

```diff
@@ -35,33 +35,33 @@
                 },
                 "ms": {
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
-            "integrity": "sha512-3iB5pWn9Sr55PKKwqFWSWjLsTKCOEhKNI+uV3BZesgXuA3IhsX8I3hW0HI+3ksMIPkh2mVYzKSpvgq3oicjG2Q==",
+            "integrity": "sha512-Uw6oB7VvmPRLE4iKsjuOh8zgDabhNX67dzo8U/BB0f9527qx+4eeUs+korU98OhG5C4ubg7ufBgVi63XYwS6TQ==",
             "requires": {
                 "debug": "4.3.4",
                 "extract-zip": "2.0.1",
                 "https-proxy-agent": "5.0.1",
                 "progress": "2.0.3",
                 "proxy-from-env": "1.1.0",
                 "tar-fs": "2.1.1",
                 "unbzip2-stream": "1.4.3",
                 "yargs": "17.7.1"
             },
-            "resolved": "https://registry.npmjs.org/@puppeteer/browsers/-/browsers-0.4.0.tgz",
-            "version": "0.4.0"
+            "resolved": "https://registry.npmjs.org/@puppeteer/browsers/-/browsers-0.5.0.tgz",
+            "version": "0.5.0"
         },
         "@types/node": {
-            "integrity": "sha512-E5Kwq2n4SbMzQOn6wnmBjuK9ouqlURrcZDVfbo9ftDDTFt3nk7ZKK4GMOzoYgnpQJKcxwQw+lGaBvvlMo0qN/Q==",
+            "integrity": "sha512-O+z53uwx64xY7D6roOi4+jApDGFg0qn6WHcxe5QeqjMaTezBO/mxdfFXIVAVVyNWKx84OmPB3L8kbVYOTeN34A==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.15.11.tgz",
-            "version": "18.15.11"
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz",
+            "version": "20.1.0"
         },
         "@types/yauzl": {
             "integrity": "sha512-Cn6WYCm0tXv8p6k+A8PvbDG763EDpBoTzHdA+Q/MF6H3sapGjCm9NzoaJncJS9tUKSuCoDs9XHxYYsQDgxR6kw==",
             "optional": true,
             "requires": {
                 "@types/node": "*"
             },
@@ -281,20 +281,20 @@
         },
         "chownr": {
             "integrity": "sha512-jJ0bqzaylmJtVnNgzTeSOs8DPavpbYgEr/b0YL8/2GO3xJEhInFmhKMUnEJQjZumK7KXGFhUy89PrsJWlakBVg==",
             "resolved": "https://registry.npmjs.org/chownr/-/chownr-1.1.4.tgz",
             "version": "1.1.4"
         },
         "chromium-bidi": {
-            "integrity": "sha512-TQOkWRaLI/IWvoP8XC+7jO4uHTIiAUiklXU1T0qszlUFEai9LgKXIBXy3pOS3EnQZ3bQtMbKUPkug0fTAEHCSw==",
+            "integrity": "sha512-6+mJuFXwTMU6I3vYLs6IL8A1DyQTPjCfIL971X0aMPVGRbGnNfl6i6Cl0NMbxi2bRYLGESt9T2ZIMRM5PAEcIQ==",
             "requires": {
                 "mitt": "3.0.0"
             },
-            "resolved": "https://registry.npmjs.org/chromium-bidi/-/chromium-bidi-0.4.6.tgz",
-            "version": "0.4.6"
+            "resolved": "https://registry.npmjs.org/chromium-bidi/-/chromium-bidi-0.4.7.tgz",
+            "version": "0.4.7"
         },
         "cliui": {
             "integrity": "sha512-BSeNnyus75C4//NQ9gQt1/csTXyo/8Sb+afLAkzAptFuMsod9HFokGNudZpi/oQV73hnVK+sR+5PVRMd+Dr7YQ==",
             "requires": {
                 "string-width": "^4.2.0",
                 "strip-ansi": "^6.0.1",
                 "wrap-ansi": "^7.0.0"
@@ -1102,25 +1102,25 @@
                 "end-of-stream": "^1.1.0",
                 "once": "^1.3.1"
             },
             "resolved": "https://registry.npmjs.org/pump/-/pump-3.0.0.tgz",
             "version": "3.0.0"
         },
         "puppeteer": {
-            "integrity": "sha512-WSjouU7eux6cwBMEz4A7mDRVZWTQQTDXrb1R6AhKDdeEgpiBBkAzcAusPhILxiJOKj60rULZpWuCZ7HZIO6GTA==",
+            "integrity": "sha512-39olGaX2djYUdhaQQHDZ0T0GwEp+5f9UB9HmEP0qHfdQHIq0xGQZuAZ5TLnJIc/88SrPLpEflPC+xUqOTv3c5g==",
             "requires": {
-                "@puppeteer/browsers": "0.4.0",
+                "@puppeteer/browsers": "0.5.0",
                 "cosmiconfig": "8.1.3",
                 "https-proxy-agent": "5.0.1",
                 "progress": "2.0.3",
                 "proxy-from-env": "1.1.0",
-                "puppeteer-core": "19.8.5"
+                "puppeteer-core": "19.11.1"
             },
-            "resolved": "https://registry.npmjs.org/puppeteer/-/puppeteer-19.8.5.tgz",
-            "version": "19.8.5"
+            "resolved": "https://registry.npmjs.org/puppeteer/-/puppeteer-19.11.1.tgz",
+            "version": "19.11.1"
         },
         "puppeteer-core": {
             "dependencies": {
                 "debug": {
                     "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
                         "ms": "2.1.2"
@@ -1130,30 +1130,30 @@
                 },
                 "ms": {
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
-            "integrity": "sha512-zoGhim/oBQbkND6h4Xz4X7l5DkWVH9wH7z0mVty5qa/c0P1Yad47t/npVtt2xS10BiQwzztWKx7Pa2nJ5yykdw==",
+            "integrity": "sha512-qcuC2Uf0Fwdj9wNtaTZ2OvYRraXpAK+puwwVW8ofOhOgLPZyz1c68tsorfIZyCUOpyBisjr+xByu7BMbEYMepA==",
             "requires": {
-                "@puppeteer/browsers": "0.4.0",
-                "chromium-bidi": "0.4.6",
+                "@puppeteer/browsers": "0.5.0",
+                "chromium-bidi": "0.4.7",
                 "cross-fetch": "3.1.5",
                 "debug": "4.3.4",
                 "devtools-protocol": "0.0.1107588",
                 "extract-zip": "2.0.1",
                 "https-proxy-agent": "5.0.1",
                 "proxy-from-env": "1.1.0",
                 "tar-fs": "2.1.1",
                 "unbzip2-stream": "1.4.3",
                 "ws": "8.13.0"
             },
-            "resolved": "https://registry.npmjs.org/puppeteer-core/-/puppeteer-core-19.8.5.tgz",
-            "version": "19.8.5"
+            "resolved": "https://registry.npmjs.org/puppeteer-core/-/puppeteer-core-19.11.1.tgz",
+            "version": "19.11.1"
         },
         "qs": {
             "integrity": "sha512-MvjoMCJwEarSbUYk5O+nmoSzSutSsTwF85zcHPQ9OrlFoZOYIjaqBAJIqIXjptyD5vThxGq52Xu/MaJzRkIk4Q==",
             "requires": {
                 "side-channel": "^1.0.4"
             },
             "resolved": "https://registry.npmjs.org/qs/-/qs-6.11.0.tgz",
@@ -1592,25 +1592,25 @@
                 "tar-fs": "2.1.1",
                 "unbzip2-stream": "1.4.3",
                 "yargs": "17.7.1"
             },
             "engines": {
                 "node": ">=14.1.0"
             },
-            "integrity": "sha512-3iB5pWn9Sr55PKKwqFWSWjLsTKCOEhKNI+uV3BZesgXuA3IhsX8I3hW0HI+3ksMIPkh2mVYzKSpvgq3oicjG2Q==",
+            "integrity": "sha512-Uw6oB7VvmPRLE4iKsjuOh8zgDabhNX67dzo8U/BB0f9527qx+4eeUs+korU98OhG5C4ubg7ufBgVi63XYwS6TQ==",
             "peerDependencies": {
                 "typescript": ">= 4.7.4"
             },
             "peerDependenciesMeta": {
                 "typescript": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@puppeteer/browsers/-/browsers-0.4.0.tgz",
-            "version": "0.4.0"
+            "resolved": "https://registry.npmjs.org/@puppeteer/browsers/-/browsers-0.5.0.tgz",
+            "version": "0.5.0"
         },
         "node_modules/@puppeteer/browsers/node_modules/debug": {
             "dependencies": {
                 "ms": "2.1.2"
             },
             "engines": {
                 "node": ">=6.0"
@@ -1626,18 +1626,18 @@
         },
         "node_modules/@puppeteer/browsers/node_modules/ms": {
             "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
             "version": "2.1.2"
         },
         "node_modules/@types/node": {
-            "integrity": "sha512-E5Kwq2n4SbMzQOn6wnmBjuK9ouqlURrcZDVfbo9ftDDTFt3nk7ZKK4GMOzoYgnpQJKcxwQw+lGaBvvlMo0qN/Q==",
+            "integrity": "sha512-O+z53uwx64xY7D6roOi4+jApDGFg0qn6WHcxe5QeqjMaTezBO/mxdfFXIVAVVyNWKx84OmPB3L8kbVYOTeN34A==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.15.11.tgz",
-            "version": "18.15.11"
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz",
+            "version": "20.1.0"
         },
         "node_modules/@types/yauzl": {
             "dependencies": {
                 "@types/node": "*"
             },
             "integrity": "sha512-Cn6WYCm0tXv8p6k+A8PvbDG763EDpBoTzHdA+Q/MF6H3sapGjCm9NzoaJncJS9tUKSuCoDs9XHxYYsQDgxR6kw==",
             "optional": true,
@@ -1929,20 +1929,20 @@
             "resolved": "https://registry.npmjs.org/chownr/-/chownr-1.1.4.tgz",
             "version": "1.1.4"
         },
         "node_modules/chromium-bidi": {
             "dependencies": {
                 "mitt": "3.0.0"
             },
-            "integrity": "sha512-TQOkWRaLI/IWvoP8XC+7jO4uHTIiAUiklXU1T0qszlUFEai9LgKXIBXy3pOS3EnQZ3bQtMbKUPkug0fTAEHCSw==",
+            "integrity": "sha512-6+mJuFXwTMU6I3vYLs6IL8A1DyQTPjCfIL971X0aMPVGRbGnNfl6i6Cl0NMbxi2bRYLGESt9T2ZIMRM5PAEcIQ==",
             "peerDependencies": {
                 "devtools-protocol": "*"
             },
-            "resolved": "https://registry.npmjs.org/chromium-bidi/-/chromium-bidi-0.4.6.tgz",
-            "version": "0.4.6"
+            "resolved": "https://registry.npmjs.org/chromium-bidi/-/chromium-bidi-0.4.7.tgz",
+            "version": "0.4.7"
         },
         "node_modules/cliui": {
             "dependencies": {
                 "string-width": "^4.2.0",
                 "strip-ansi": "^6.0.1",
                 "wrap-ansi": "^7.0.0"
             },
@@ -2978,54 +2978,54 @@
             },
             "integrity": "sha512-LwZy+p3SFs1Pytd/jYct4wpv49HiYCqd9Rlc5ZVdk0V+8Yzv6jR5Blk3TRmPL1ft69TxP0IMZGJ+WPFU2BFhww==",
             "resolved": "https://registry.npmjs.org/pump/-/pump-3.0.0.tgz",
             "version": "3.0.0"
         },
         "node_modules/puppeteer": {
             "dependencies": {
-                "@puppeteer/browsers": "0.4.0",
+                "@puppeteer/browsers": "0.5.0",
                 "cosmiconfig": "8.1.3",
                 "https-proxy-agent": "5.0.1",
                 "progress": "2.0.3",
                 "proxy-from-env": "1.1.0",
-                "puppeteer-core": "19.8.5"
+                "puppeteer-core": "19.11.1"
             },
             "hasInstallScript": true,
-            "integrity": "sha512-WSjouU7eux6cwBMEz4A7mDRVZWTQQTDXrb1R6AhKDdeEgpiBBkAzcAusPhILxiJOKj60rULZpWuCZ7HZIO6GTA==",
-            "resolved": "https://registry.npmjs.org/puppeteer/-/puppeteer-19.8.5.tgz",
-            "version": "19.8.5"
+            "integrity": "sha512-39olGaX2djYUdhaQQHDZ0T0GwEp+5f9UB9HmEP0qHfdQHIq0xGQZuAZ5TLnJIc/88SrPLpEflPC+xUqOTv3c5g==",
+            "resolved": "https://registry.npmjs.org/puppeteer/-/puppeteer-19.11.1.tgz",
+            "version": "19.11.1"
         },
         "node_modules/puppeteer-core": {
             "dependencies": {
-                "@puppeteer/browsers": "0.4.0",
-                "chromium-bidi": "0.4.6",
+                "@puppeteer/browsers": "0.5.0",
+                "chromium-bidi": "0.4.7",
                 "cross-fetch": "3.1.5",
                 "debug": "4.3.4",
                 "devtools-protocol": "0.0.1107588",
                 "extract-zip": "2.0.1",
                 "https-proxy-agent": "5.0.1",
                 "proxy-from-env": "1.1.0",
                 "tar-fs": "2.1.1",
                 "unbzip2-stream": "1.4.3",
                 "ws": "8.13.0"
             },
             "engines": {
                 "node": ">=14.14.0"
             },
-            "integrity": "sha512-zoGhim/oBQbkND6h4Xz4X7l5DkWVH9wH7z0mVty5qa/c0P1Yad47t/npVtt2xS10BiQwzztWKx7Pa2nJ5yykdw==",
+            "integrity": "sha512-qcuC2Uf0Fwdj9wNtaTZ2OvYRraXpAK+puwwVW8ofOhOgLPZyz1c68tsorfIZyCUOpyBisjr+xByu7BMbEYMepA==",
             "peerDependencies": {
                 "typescript": ">= 4.7.4"
             },
             "peerDependenciesMeta": {
                 "typescript": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/puppeteer-core/-/puppeteer-core-19.8.5.tgz",
-            "version": "19.8.5"
+            "resolved": "https://registry.npmjs.org/puppeteer-core/-/puppeteer-core-19.11.1.tgz",
+            "version": "19.11.1"
         },
         "node_modules/puppeteer-core/node_modules/debug": {
             "dependencies": {
                 "ms": "2.1.2"
             },
             "engines": {
                 "node": ">=6.0"
```

### Comparing `gramex-1.89.2/gramex/apps/capture/package.json` & `gramex-1.90.0/gramex/apps/capture/package.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/README.html` & `gramex-1.90.0/gramex/apps/filemanager/README.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/drivehandler-snippet.html` & `gramex-1.90.0/gramex/apps/filemanager/drivehandler-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/filemanager-snippet.html` & `gramex-1.90.0/gramex/apps/filemanager/filemanager-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/filemanager.html` & `gramex-1.90.0/gramex/apps/filemanager/filemanager.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/filemanager.js` & `gramex-1.90.0/gramex/apps/filemanager/filemanager.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/filemanager.py` & `gramex-1.90.0/gramex/apps/filemanager/filemanager.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/gramex.yaml` & `gramex-1.90.0/gramex/apps/filemanager/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/index.html` & `gramex-1.90.0/gramex/apps/filemanager/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/filemanager/navbar.html` & `gramex-1.90.0/gramex/apps/filemanager/navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/.template.gitignore` & `gramex-1.90.0/gramex/apps/init/default/.template.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/assets/README.template.md` & `gramex-1.90.0/gramex/apps/init/default/assets/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/error/400.html` & `gramex-1.90.0/gramex/handlers/400.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/error/401.html` & `gramex-1.90.0/gramex/handlers/401.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/error/403.html` & `gramex-1.90.0/gramex/handlers/403.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/error/404.html` & `gramex-1.90.0/gramex/handlers/404.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/error/500.html` & `gramex-1.90.0/gramex/handlers/500.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/favicon.ico` & `gramex-1.90.0/gramex/favicon.ico`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/gramex.template.yaml` & `gramex-1.90.0/gramex/apps/init/default/gramex.template.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     pattern: /$YAMLURL/
     handler: FileHandler
     kwargs:
       path: $YAMLPATH/index.html
       # See https://gramener.com/gramex/guide/auth/#authorization for auth rules
       auth:
         login_url: /$YAMLURL/login/
-      template: ['index.html', 'template*.html']
+      template: ["index.html", "template*.html"]
       headers:
         # Templates may have user-specific content. Cache privately.
         # Keep max-age small (in case we log out & log in as another user.)
         Cache-Control: private, max-age=1
-    cache: {expiry: {duration: 1}}
+    cache: { expiry: { duration: 1 } }
 
   {{ appname }}-login:
     pattern: /$YAMLURL/login/
     # You MUST change the auth before deploying. DBAuth is commonly used.
     # See https://gramener.com/gramex/guide/auth/#database-auth
     handler: SimpleAuth
     kwargs:
@@ -30,51 +30,19 @@
         alpha: alpha
         beta: beta
 
   {{ appname }}-logout:
     pattern: /$YAMLURL/logout/
     handler: LogoutHandler
 
-# Notify testers what user ID and password to use
-test:
-  auth:
-    user: alpha
-    password: alpha
-
-
 # Gramex init configurations for app: {{ appname }}
 # ----------------------------------------------------------------------------
 import:
   # To secure application for production,
   # replace 'YOUR-PROD-SERVER-NAME' with your production server host name.
   deploy if socket.gethostname() in {'YOUR-PROD-SERVER-NAME'}: $GRAMEXPATH/deploy.yaml
   # For alternate methods, see https://gramener.com/gramex/guide/config/#conditions
 
   # /ui/ has Gramex UI components -- use this like the node_modules/ directory
   ui:
     path: $GRAMEXAPPS/ui/gramex.yaml
     YAMLURL: $YAMLURL/ui/
-
-  # /admin/ as an admin page to manage users, get system info, etc.
-  admin:
-    path: $GRAMEXAPPS/admin2/gramex.yaml    # Note the "admin2" instead of "admin"
-    YAMLURL: /$YAMLURL/admin/               # URL to show the admin page at
-    ADMIN_KWARGS:
-      logo: https://gramener.com/uistatic/gramener.png
-      home: /$YAMLURL/
-      title: Admin
-      theme: '?body-bg=white&navbar-dark-color=rgba(255%2C255%2C255%2C.8)&navbar-dark-hover-color=white'
-      # authhandler: name-of-DBAuth-handler    -- required for user management
-    ADMIN_AUTH:
-      membership:
-        hd: gramener.com                    # Only @gramener.com Google Auth are admins
-
-
-handlers:
-  BaseHandler:
-    # Custom error pages for this application
-    error:
-      400: {path: $YAMLPATH/error/400.html}     # Bad request: e.g. URL argument missing
-      401: {path: $YAMLPATH/error/401.html}     # Unauthorized: User not logged in
-      403: {path: $YAMLPATH/error/403.html}     # Forbidden: user does not have access
-      404: {path: $YAMLPATH/error/404.html}     # File not found
-      500: {path: $YAMLPATH/error/500.html}     # Internal server error
```

### Comparing `gramex-1.89.2/gramex/apps/init/default/js/README.template.md` & `gramex-1.90.0/gramex/apps/init/default/js/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/default/login.template.html` & `gramex-1.90.0/gramex/apps/init/default/login.template.html`

 * *Files 22% similar despite different names*

```diff
@@ -6,56 +6,52 @@
   <meta http-equiv="x-ua-compatible" content="ie=edge">
   <title>{{ appname }} Login</title>
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <link rel="stylesheet" href="../style.scss">
 </head>
 
 <body class="bg-primary gradient-tc bg-no-repeat text-white">
-  {%! set base = '..' %}
-  {%! include template-navbar.html %}
   {%! set kwargs = handler.kwargs %}
   {%! try %}{%! set user = kwargs.user.arg %}{%! except %}{%! set user = 'user' %}{%! end %}
   {%! try %}{%! set password = kwargs.password.arg %}{%! except %}{%! set password = 'password' %}{%! end %}
-  <div class="container d-flex flex-column align-items-center">
-    <div class="card shadow text-dark mx-auto my-4 px-5 py-3 col-md-6">
+  <div class="container d-flex flex-column justify-content-center align-items-center">
+    <div class="card shadow text-dark mx-auto my-5 px-4 py-3 col-md-6">
       {%! if error %}
         <div class="alert alert-danger mx-n3">
           <h1 class="h4">Error logging in</h1>
           <p>{{! error['error'] }}</p>
           <div><small><strong>code</strong>: {{! error['code'] }}</small></div>
         </div>
       {%! end %}
       <form method="POST">
-        <div class="form-group">
-          <label for="{{! user }}">Login</label>
-          <input type="text" class="form-control" name="{{! user }}" id="{{! user }}" value="{{! handler.get_argument(user, '') }}" placeholder="Login ID" autofocus required>
+        <div class="mb-3">
+          <label for="{{! user }}" class="form-label">Login</label>
+          <input type="text" class="form-control" name="{{! user }}" id="{{! user }}" value="{{! handler.get_argument(user, '') }}" autofocus required>
         </div>
-        <div class="form-group">
-          <label for="{{! password  }}">Password</label>
-          <input type="password" class="form-control" name="{{! password }}" id="{{! password }}" placeholder="Password" required>
+        <div class="mb-3">
+          <label for="{{! password }}" class="form-label">Password</label>
+          <input type="password" class="form-control" name="{{! password }}" id="{{! password }}" required aria-describedby="passwordHelp">
+          <div id="passwordHelp" class="form-text">Default login: alpha / alpha.</div>
         </div>
         <input type="hidden" name="_xsrf" value="{{! handler.xsrf_token }}">
-        <p><button type="submit" class="btn btn-primary w-100 small">Login</button></p>
+        <p><button type="submit" class="btn btn-primary w-100">Login</button></p>
         {%! if kwargs.get('forgot') %}
           <p class="small"><a href="?{{! kwargs.forgot.key }}">Forgot password</a></p>
         {%! end %}
-        <div>Default login: alpha (password: alpha)</div>
       </form>
     </div><!-- .card -->
   </div>
-  <script src="../ui/jquery/dist/jquery.min.js"></script>
-  <script src="../ui/bootstrap/dist/js/bootstrap.bundle.min.js"></script>
   {%! if 'hash' in kwargs.get('password', {}) %}
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/js-sha256/0.9.0/sha256.min.js"></script>
-    <script>
-      /* eslint-env browser, jquery */
-      /* globals sha256 */
+    <script type="module">
       // hash the password before submitting
-      $('form').on('submit', function() {
-        var $password = $('#{{! password }}').get(0)
-        $password.value = sha256($password.value)
-      })
+      document.querySelector('form').addEventListener('submit', async function(e) {
+        const $password = e.target.querySelector('[type="password"]');
+        const msg = new TextEncoder().encode($password.value);
+        const buffer = await crypto.subtle.digest("SHA-256", msg);
+        const array = Array.from(new Uint8Array(buffer));
+        $password.value = array.map((b) => b.toString(16).padStart(2, "0")).join("");
+      }, false)
     </script>
   {%! end %}
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
 
 
-{%! set base = '..' %} {%! include template-navbar.html %} {%! set kwargs =
-handler.kwargs %} {%! try %}{%! set user = kwargs.user.arg %}{%! except %}{%!
-set user = 'user' %}{%! end %} {%! try %}{%! set password = kwargs.password.arg
-%}{%! except %}{%! set password = 'password' %}{%! end %}
+{%! set kwargs = handler.kwargs %} {%! try %}{%! set user = kwargs.user.arg %}
+{%! except %}{%! set user = 'user' %}{%! end %} {%! try %}{%! set password =
+kwargs.password.arg %}{%! except %}{%! set password = 'password' %}{%! end %}
 {%! if error %}
 ****** Error logging in ******
 {{! error['error'] }}
 code: {{! error['code'] }}
 {%! end %}
 Login [{{! handler.get_argument(user, '') }}]
 Password [********************]
+Default login: alpha / alpha.
 Login
 {%! if kwargs.get('forgot') %}
 Forgot_password
 {%! end %}
-Default login: alpha (password: alpha)
- {%! if 'hash' in kwargs.get('password', {}) %}
+{%! if 'hash' in kwargs.get('password', {}) %}
  {%! end %}
```

### Comparing `gramex-1.89.2/gramex/apps/init/default/template-navbar.template.html` & `gramex-1.90.0/gramex/apps/init/default/template-navbar.template.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,62 @@
-<nav class="navbar navbar-expand-lg navbar-dark bg-dark py-0">
-  <a class="navbar-brand" href="{{! base }}">
-    <!-- Replace with your logo. Just specify height, not width. -->
-    <img height="36" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACQAAAAkAQAAAADJe6U1AAAABGdBTUEAALGPC/xhBQAAAAJ0Uk5TAAB2k804AAAANUlEQVR42mNgwAX4/x8AkvZgsh5M/geTP8CyH0ggP1BKMoLIH8wfwG54AHbPA7jb+P9jcz0AKpcxBQbNJ8sAAAAASUVORK5CYII=" alt="Logo">
-    <span class="text-uppercase">{{ appname }}</span>
-  </a>
-  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
-    <span class="navbar-toggler-icon"></span>
-  </button>
-  <div class="collapse navbar-collapse" id="navbarSupportedContent">
-    <!-- Navbar left -->
-    <ul class="navbar-nav mr-auto">
-      <li class="nav-item active">
-        <a class="nav-link" href="{{! base }}">Home <span class="sr-only">(current)</span></a>
-      </li>
-      <li class="nav-item dropdown">
-        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
-          Dropdown
-        </a>
-        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
-          <a class="dropdown-item" href="#">Action</a>
-          <a class="dropdown-item" href="#">Another action</a>
-          <div class="dropdown-divider"></div>
-          <a class="dropdown-item" href="#">Something else here</a>
-        </div>
-      </li>
-    </ul>
-    <!-- Navbar middle -->
-    <div class="navbar-nav mr-auto">
-      <span class="nav-item nav-link active text-uppercase h5 mb-0">Dashboard</span>
+<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
+  <div class="container-fluid">
+    <a class="navbar-brand" href="{{! base }}">
+      <!-- Replace with your logo. Just specify height, not width. -->
+      <img height="36" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACQAAAAkAQAAAADJe6U1AAAABGdBTUEAALGPC/xhBQAAAAJ0Uk5TAAB2k804AAAANUlEQVR42mNgwAX4/x8AkvZgsh5M/geTP8CyH0ggP1BKMoLIH8wfwG54AHbPA7jb+P9jcz0AKpcxBQbNJ8sAAAAASUVORK5CYII=" alt="Logo">
+      <span class="text-uppercase">{{ appname }}</span>
+    </a>
+    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
+      <span class="navbar-toggler-icon"></span>
+    </button>
+    <div class="collapse navbar-collapse" id="navbarSupportedContent">
+      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
+        <li class="nav-item">
+          <a class="nav-link active" aria-current="page" href="https://gramener.com/gramex/guide/">Guide</a>
+        </li>
+        <li class="nav-item">
+          <a class="nav-link" href="https://stackoverflow.com/search?tab=Relevance&pagesize=-1&q=gramex&searchOn=1">Q&A</a>
+        </li>
+        <li class="nav-item dropdown">
+          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
+            Links
+          </a>
+          <ul class="dropdown-menu">
+            <li><a class="dropdown-item" href="https://www.youtube.com/watch?v=lkBqm6XoccI&list=PLrn2FHBzHtaMDFAkpJ1JDXbtfvcVvpsAJ">Videos</a></li>
+            <li>
+              <hr class="dropdown-divider">
+            </li>
+            <li><a class="dropdown-item" href="https://uifactory.gramener.com/">UIFactory</a></li>
+            <li><a class="dropdown-item" href="https://gramener.com/charts/">Charts</a></li>
+          </ul>
+        </li>
+      </ul>
+      <form class="d-flex" role="search">
+        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
+        <button class="btn btn-primary" type="submit">Search</button>
+      </form>
+      <ul class="navbar-nav ms-2">
+        {%! if handler.current_user %}
+          <li class="nav-item">
+            <a class="nav-link" href="{{! base }}/login/" title="Log in again" data-placement="bottom">
+              {{! handler.current_user.id }}
+            </a>
+          </li>
+          <li class="nav-item">
+            <a class="btn btn-danger" href="{{! base }}/logout/" title="Log out" data-placement="bottom">
+              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-right" viewBox="0 0 16 16">
+                <path fill-rule="evenodd" d="M10 12.5a.5.5 0 0 1-.5.5h-8a.5.5 0 0 1-.5-.5v-9a.5.5 0 0 1 .5-.5h8a.5.5 0 0 1 .5.5v2a.5.5 0 0 0 1 0v-2A1.5 1.5 0 0 0 9.5 2h-8A1.5 1.5 0 0 0 0 3.5v9A1.5 1.5 0 0 0 1.5 14h8a1.5 1.5 0 0 0 1.5-1.5v-2a.5.5 0 0 0-1 0v2z" />
+                <path fill-rule="evenodd" d="M15.854 8.354a.5.5 0 0 0 0-.708l-3-3a.5.5 0 0 0-.708.708L14.293 7.5H5.5a.5.5 0 0 0 0 1h8.793l-2.147 2.146a.5.5 0 0 0 .708.708l3-3z" />
+              </svg>
+            </a>
+          </li>
+        {%! else %}
+          <li class="nav-item">
+            <a class="btn btn-primary" href="{{! base }}/login/" title="Log in again" data-placement="bottom">
+              Log in
+            </a>
+          </li>
+        {%! end %}
+        </ul>
     </div>
-    <!-- Navbar right -->
-    <div class="navbar-nav mr-2">
-      {%! if handler.current_user %}
-        <a class="nav-item nav-link" href="{{! base }}/login/" title="Log in again" data-placement="bottom">
-          {{! handler.current_user.id }}
-        </a>
-        <a class="nav-item nav-link" href="{{! base }}/logout/" title="Log out" data-placement="bottom"><span class="fas fa-arrow-right bg-light round text-dark p-1"></span></a>
-      {%! else %}
-        <a class="nav-item nav-link" href="{{! base }}/login/" title="Log in again" data-placement="bottom">
-          Log in
-        </a>
-      {%! end %}
-    </div>
-    <form class="form-inline my-2 my-lg-0">
-      <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
-      <button class="btn btn-light my-2 my-sm-0" type="submit">Search</button>
-    </form>
   </div>
 </nav>
```

### Comparing `gramex-1.89.2/gramex/apps/init/ide/index.template.html` & `gramex-1.90.0/gramex/apps/init/ide/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/init/minimal/index.template.html` & `gramex-1.90.0/gramex/apps/init/minimal/index.template.html`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <link rel="stylesheet" href="ui/theme/bootstrap5.scss">
 </head>
 
 <body>
   <div class="container my-5">
     <div class="jumbotron text-center">
-      <h1 class="display-4">Welcome to Gramex</h1>
+      <h1 class="display-4">Welcome to Gramex (minimal template)</h1>
       <a class="btn btn-primary btn-lg my-5" href="https://gramener.com/gramex/guide/" role="button">Learn more</a>
     </div>
   </div>
 
   <!-- Add commonly used libraries from https://gramener.com/gramex/guide/uicomponents/ -->
   <script src="ui/bootstrap5/dist/js/bootstrap.bundle.min.js"></script>
 </body>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 
 
-****** Welcome to Gramex ******
+****** Welcome to Gramex (minimal template) ******
 Learn_more
```

### Comparing `gramex-1.89.2/gramex/apps/languagetool/README.md` & `gramex-1.90.0/gramex/apps/languagetool/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/languagetool/gramex.yaml` & `gramex-1.90.0/gramex/apps/languagetool/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/logviewer/config.yaml` & `gramex-1.90.0/gramex/apps/logviewer/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/logviewer/gramex.yaml` & `gramex-1.90.0/gramex/apps/logviewer/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/logviewer/index.html` & `gramex-1.90.0/gramex/apps/logviewer/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/logviewer/logviewer.py` & `gramex-1.90.0/gramex/apps/logviewer/logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/logviewer/lv-datepicker.html` & `gramex-1.90.0/gramex/apps/logviewer/lv-datepicker.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/logviewer/package-lock.json` & `gramex-1.90.0/gramex/apps/logviewer/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/logviewer/render.js` & `gramex-1.90.0/gramex/apps/logviewer/render.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/logviewer/script.js` & `gramex-1.90.0/gramex/apps/logviewer/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/mail/index.html` & `gramex-1.90.0/gramex/apps/mail/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/mlhandler/template.html` & `gramex-1.90.0/gramex/apps/mlhandler/template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/pynode/index.js` & `gramex-1.90.0/gramex/apps/pynode/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/pynode/package-lock.json` & `gramex-1.90.0/gramex/apps/pynode/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/.snyk` & `gramex-1.90.0/gramex/apps/ui/.snyk`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/__init__.py` & `gramex-1.90.0/gramex/apps/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/bootstrap-theme.scss` & `gramex-1.90.0/gramex/apps/ui/bootstrap-theme.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/config.yaml` & `gramex-1.90.0/gramex/apps/ui/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/gramex.yaml` & `gramex-1.90.0/gramex/apps/ui/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/gramexui.scss` & `gramex-1.90.0/gramex/apps/ui/gramexui.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/package-lock.json` & `gramex-1.90.0/gramex/apps/ui/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963930690299432%*

 * *Differences: {"'dependencies'": "{'@babel/compat-data': {'version': '7.21.7', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.21.7.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-KYMqFYTaenzMK4yUtf4EW9wc4N9ef80FsbMtkwool5zpwl4YrT1SdWYSTRcT94KO4hannogdS+LxY7L+arP3gA=='}, "*

 * *                   "'@babel/core': {'version': '7.21.8', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@babel/core/-/core-7.21.8.tgz', 'integrity': "*

 * *               […]*

```diff
@@ -25,70 +25,70 @@
             "requires": {
                 "@babel/highlight": "^7.18.6"
             },
             "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.21.4.tgz",
             "version": "7.21.4"
         },
         "@babel/compat-data": {
-            "integrity": "sha512-/DYyDpeCfaVinT40FPGdkkb+lYSKvsVuMjDAG7jPOWWiM1ibOaB9CXJAlc4d1QpP/U2q2P9jbrSlClKSErd55g==",
-            "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.21.4.tgz",
-            "version": "7.21.4"
+            "integrity": "sha512-KYMqFYTaenzMK4yUtf4EW9wc4N9ef80FsbMtkwool5zpwl4YrT1SdWYSTRcT94KO4hannogdS+LxY7L+arP3gA==",
+            "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.21.7.tgz",
+            "version": "7.21.7"
         },
         "@babel/core": {
-            "integrity": "sha512-qt/YV149Jman/6AfmlxJ04LMIu8bMoyl3RB91yTFrxQmgbrSvQMy7cI8Q62FHx1t8wJ8B5fu0UDoLwHAhUo1QA==",
+            "integrity": "sha512-YeM22Sondbo523Sz0+CirSPnbj9bG3P0CdHcBZdqUuaeOaYEFbOLoGU7lebvGP6P5J/WE9wOn7u7C4J9HvS1xQ==",
             "peer": true,
             "requires": {
                 "@ampproject/remapping": "^2.2.0",
                 "@babel/code-frame": "^7.21.4",
-                "@babel/generator": "^7.21.4",
-                "@babel/helper-compilation-targets": "^7.21.4",
-                "@babel/helper-module-transforms": "^7.21.2",
-                "@babel/helpers": "^7.21.0",
-                "@babel/parser": "^7.21.4",
+                "@babel/generator": "^7.21.5",
+                "@babel/helper-compilation-targets": "^7.21.5",
+                "@babel/helper-module-transforms": "^7.21.5",
+                "@babel/helpers": "^7.21.5",
+                "@babel/parser": "^7.21.8",
                 "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.4",
-                "@babel/types": "^7.21.4",
+                "@babel/traverse": "^7.21.5",
+                "@babel/types": "^7.21.5",
                 "convert-source-map": "^1.7.0",
                 "debug": "^4.1.0",
                 "gensync": "^1.0.0-beta.2",
                 "json5": "^2.2.2",
                 "semver": "^6.3.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.21.8.tgz",
+            "version": "7.21.8"
         },
         "@babel/generator": {
-            "integrity": "sha512-NieM3pVIYW2SwGzKoqfPrQsf4xGs9M9AIG3ThppsSRmO+m7eQhmI6amajKMUeIO37wFfsvnvcxQFx6x6iqxDnA==",
+            "integrity": "sha512-SrKK/sRv8GesIW1bDagf9cCG38IOMYZusoe1dfg0D8aiUe3Amvoj1QtjTPAWcfrZFvIwlleLb0gxzQidL9w14w==",
             "peer": true,
             "requires": {
-                "@babel/types": "^7.21.4",
+                "@babel/types": "^7.21.5",
                 "@jridgewell/gen-mapping": "^0.3.2",
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jsesc": "^2.5.1"
             },
-            "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@babel/helper-compilation-targets": {
-            "integrity": "sha512-Fa0tTuOXZ1iL8IeDFUWCzjZcn+sJGd9RZdH9esYVjEejGmzf+FFYQpMi/kZUk2kPy/q1H3/GPw7np8qar/stfg==",
+            "integrity": "sha512-1RkbFGUKex4lvsB9yhIfWltJM5cZKUftB2eNajaDv3dCMEp49iBG0K14uH8NnX9IPux2+mK7JGEOB0jn48/J6w==",
             "requires": {
-                "@babel/compat-data": "^7.21.4",
+                "@babel/compat-data": "^7.21.5",
                 "@babel/helper-validator-option": "^7.21.0",
                 "browserslist": "^4.21.3",
                 "lru-cache": "^5.1.1",
                 "semver": "^6.3.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@babel/helper-environment-visitor": {
-            "integrity": "sha512-3r/aACDJ3fhQ/EVgFy0hpj8oHyHpQc+LPtJoY9SzTThAsStm4Ptegq92vqKoE3vD706ZVFWITnMnxucw+S9Ipg==",
+            "integrity": "sha512-IYl4gZ3ETsWocUWgsFZLM5i1BYx9SoemminVEXadgLBa9TdeorzgLKm8wWLA6J1N/kT3Kch8XIk1laNzYoHKvQ==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.18.9.tgz",
-            "version": "7.18.9"
+            "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@babel/helper-function-name": {
             "integrity": "sha512-HfK1aMRanKHpxemaY2gqBmL04iAPOPRj7DxtNbiDOrJK+gdwkiNRVpCpUJYbUT+aZyemKN8brqTOxzCaG6ExRg==",
             "peer": true,
             "requires": {
                 "@babel/template": "^7.20.7",
                 "@babel/types": "^7.21.0"
@@ -111,129 +111,129 @@
             "requires": {
                 "@babel/types": "^7.21.4"
             },
             "resolved": "https://registry.npmjs.org/@babel/helper-module-imports/-/helper-module-imports-7.21.4.tgz",
             "version": "7.21.4"
         },
         "@babel/helper-module-transforms": {
-            "integrity": "sha512-79yj2AR4U/Oqq/WOV7Lx6hUjau1Zfo4cI+JLAVYeMV5XIlbOhmjEk5ulbTc9fMpmlojzZHkUUxAiK+UKn+hNQQ==",
+            "integrity": "sha512-bI2Z9zBGY2q5yMHoBvJ2a9iX3ZOAzJPm7Q8Yz6YeoUjU/Cvhmi2G4QyTNyPBqqXSgTjUxRg3L0xV45HvkNWWBw==",
             "peer": true,
             "requires": {
-                "@babel/helper-environment-visitor": "^7.18.9",
-                "@babel/helper-module-imports": "^7.18.6",
-                "@babel/helper-simple-access": "^7.20.2",
+                "@babel/helper-environment-visitor": "^7.21.5",
+                "@babel/helper-module-imports": "^7.21.4",
+                "@babel/helper-simple-access": "^7.21.5",
                 "@babel/helper-split-export-declaration": "^7.18.6",
                 "@babel/helper-validator-identifier": "^7.19.1",
                 "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.2",
-                "@babel/types": "^7.21.2"
+                "@babel/traverse": "^7.21.5",
+                "@babel/types": "^7.21.5"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.21.2.tgz",
-            "version": "7.21.2"
+            "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@babel/helper-simple-access": {
-            "integrity": "sha512-+0woI/WPq59IrqDYbVGfshjT5Dmk/nnbdpcF8SnMhhXObpTq2KNBdLFRFrkVdbDOyUmHBCxzm5FHV1rACIkIbA==",
+            "integrity": "sha512-ENPDAMC1wAjR0uaCUwliBdiSl1KBJAVnMTzXqi64c2MG8MPR6ii4qf7bSXDqSFbr4W6W028/rf5ivoHop5/mkg==",
             "peer": true,
             "requires": {
-                "@babel/types": "^7.20.2"
+                "@babel/types": "^7.21.5"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helper-simple-access/-/helper-simple-access-7.20.2.tgz",
-            "version": "7.20.2"
+            "resolved": "https://registry.npmjs.org/@babel/helper-simple-access/-/helper-simple-access-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@babel/helper-split-export-declaration": {
             "integrity": "sha512-bde1etTx6ZyTmobl9LLMMQsaizFVZrquTEHOqKeQESMKo4PlObf+8+JA25ZsIpZhT/WEd39+vOdLXAFG/nELpA==",
             "peer": true,
             "requires": {
                 "@babel/types": "^7.18.6"
             },
             "resolved": "https://registry.npmjs.org/@babel/helper-split-export-declaration/-/helper-split-export-declaration-7.18.6.tgz",
             "version": "7.18.6"
         },
         "@babel/helper-string-parser": {
-            "integrity": "sha512-nHtDoQcuqFmwYNYPz3Rah5ph2p8PFeFCsZk9A/48dPc/rGocJ5J3hAAZ7pb76VWX3fZKu+uEr/FhH5jLx7umrw==",
+            "integrity": "sha512-5pTUx3hAJaZIdW99sJ6ZUUgWq/Y+Hja7TowEnLNMm1VivRgZQL3vpBY3qUACVsvw+yQU6+YgfBVmcbLaZtrA1w==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-string-parser/-/helper-string-parser-7.19.4.tgz",
-            "version": "7.19.4"
+            "resolved": "https://registry.npmjs.org/@babel/helper-string-parser/-/helper-string-parser-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@babel/helper-validator-identifier": {
             "integrity": "sha512-awrNfaMtnHUr653GgGEs++LlAvW6w+DcPrOliSMXWCKo597CwL5Acf/wWdNkf/tfEQE3mjkeD1YOVZOUV/od1w==",
             "resolved": "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.19.1.tgz",
             "version": "7.19.1"
         },
         "@babel/helper-validator-option": {
             "integrity": "sha512-rmL/B8/f0mKS2baE9ZpyTcTavvEuWhTTW8amjzXNvYG4AwBsqTLikfXsEofsJEfKHf+HQVQbFOHy6o+4cnC/fQ==",
             "resolved": "https://registry.npmjs.org/@babel/helper-validator-option/-/helper-validator-option-7.21.0.tgz",
             "version": "7.21.0"
         },
         "@babel/helpers": {
-            "integrity": "sha512-XXve0CBtOW0pd7MRzzmoyuSj0e3SEzj8pgyFxnTT1NJZL38BD1MK7yYrm8yefRPIDvNNe14xR4FdbHwpInD4rA==",
+            "integrity": "sha512-BSY+JSlHxOmGsPTydUkPf1MdMQ3M81x5xGCOVgWM3G8XH77sJ292Y2oqcp0CbbgxhqBuI46iUz1tT7hqP7EfgA==",
             "peer": true,
             "requires": {
                 "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.0",
-                "@babel/types": "^7.21.0"
+                "@babel/traverse": "^7.21.5",
+                "@babel/types": "^7.21.5"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.21.0.tgz",
-            "version": "7.21.0"
+            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@babel/highlight": {
             "integrity": "sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==",
             "requires": {
                 "@babel/helper-validator-identifier": "^7.18.6",
                 "chalk": "^2.0.0",
                 "js-tokens": "^4.0.0"
             },
             "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.18.6.tgz",
             "version": "7.18.6"
         },
         "@babel/parser": {
-            "integrity": "sha512-alVJj7k7zIxqBZ7BTRhz0IqJFxW1VJbm6N8JbcYhQ186df9ZBPbZBmWSqAMXwHGsCJdYks7z/voa3ibiS5bCIw==",
+            "integrity": "sha512-6zavDGdzG3gUqAdWvlLFfk+36RilI+Pwyuuh7HItyeScCWP3k6i8vKclAQ0bM/0y/Kz/xiwvxhMv9MgTJP5gmA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.21.8.tgz",
+            "version": "7.21.8"
         },
         "@babel/template": {
             "integrity": "sha512-8SegXApWe6VoNw0r9JHpSteLKTpTiLZ4rMlGIm9JQ18KiCtyQiAMEazujAHrUS5flrcqYZa75ukev3P6QmUwUw==",
             "peer": true,
             "requires": {
                 "@babel/code-frame": "^7.18.6",
                 "@babel/parser": "^7.20.7",
                 "@babel/types": "^7.20.7"
             },
             "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.20.7.tgz",
             "version": "7.20.7"
         },
         "@babel/traverse": {
-            "integrity": "sha512-eyKrRHKdyZxqDm+fV1iqL9UAHMoIg0nDaGqfIOd8rKH17m5snv7Gn4qgjBoFfLz9APvjFU/ICT00NVCv1Epp8Q==",
+            "integrity": "sha512-AhQoI3YjWi6u/y/ntv7k48mcrCXmus0t79J9qPNlk/lAsFlCiJ047RmbfMOawySTHtywXhbXgpx/8nXMYd+oFw==",
             "peer": true,
             "requires": {
                 "@babel/code-frame": "^7.21.4",
-                "@babel/generator": "^7.21.4",
-                "@babel/helper-environment-visitor": "^7.18.9",
+                "@babel/generator": "^7.21.5",
+                "@babel/helper-environment-visitor": "^7.21.5",
                 "@babel/helper-function-name": "^7.21.0",
                 "@babel/helper-hoist-variables": "^7.18.6",
                 "@babel/helper-split-export-declaration": "^7.18.6",
-                "@babel/parser": "^7.21.4",
-                "@babel/types": "^7.21.4",
+                "@babel/parser": "^7.21.5",
+                "@babel/types": "^7.21.5",
                 "debug": "^4.1.0",
                 "globals": "^11.1.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@babel/types": {
-            "integrity": "sha512-rU2oY501qDxE8Pyo7i/Orqma4ziCOrby0/9mvbDUGEfvZjb279Nk9k19e2fiCxHbRRpY2ZyrgW1eq22mvmOIzA==",
+            "integrity": "sha512-m4AfNvVF2mVC/F7fDEdH2El3HzUg9It/XsCxZiOTTA3m3qYfcSVSbTfM6Q9xG+hYDniZssYhlXKKUMD5m8tF4Q==",
             "peer": true,
             "requires": {
-                "@babel/helper-string-parser": "^7.19.4",
+                "@babel/helper-string-parser": "^7.21.5",
                 "@babel/helper-validator-identifier": "^7.19.1",
                 "to-fast-properties": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "@colors/colors": {
             "integrity": "sha512-ooWCrlZP11i8GImSjTHYHLkvFDP48nS4+204nGb1RiX/WXYHmJA2III9/e2DWVabCESdW7hBAEzHRqUn9OUVvQ==",
             "resolved": "https://registry.npmjs.org/@colors/colors/-/colors-1.5.0.tgz",
             "version": "1.5.0"
         },
         "@dabh/diagnostics": {
@@ -475,21 +475,21 @@
             "requires": {
                 "@types/node": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/connect/-/connect-3.4.35.tgz",
             "version": "3.4.35"
         },
         "@types/connect-history-api-fallback": {
-            "integrity": "sha512-h8QJa8xSb1WD4fpKBDcATDNGXghFj6/3GRWG6dhmRcu0RX1Ubasur2Uvx5aeEwlf0MwblEC2bMzzMQntxnw/Cw==",
+            "integrity": "sha512-4x5FkPpLipqwthjPsF7ZRbOv3uoLUFkTA9G9v583qi4pACvq0uTELrB8OLUzPWUI4IJIyvM85vzkV1nyiI2Lig==",
             "requires": {
                 "@types/express-serve-static-core": "*",
                 "@types/node": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/connect-history-api-fallback/-/connect-history-api-fallback-1.3.5.tgz",
-            "version": "1.3.5"
+            "resolved": "https://registry.npmjs.org/@types/connect-history-api-fallback/-/connect-history-api-fallback-1.5.0.tgz",
+            "version": "1.5.0"
         },
         "@types/eslint": {
             "integrity": "sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==",
             "requires": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
@@ -502,71 +502,72 @@
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
             "version": "3.7.4"
         },
         "@types/estree": {
-            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
-            "version": "0.0.51"
+            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
+            "version": "1.0.1"
         },
         "@types/express": {
             "integrity": "sha512-Q4FmmuLGBG58btUnfS1c1r/NQdlp3DMfGDGig8WhfpA2YRUtEkxAjkZb0yvplJGYdF1fsQ81iMDcH24sSCNC/Q==",
             "requires": {
                 "@types/body-parser": "*",
                 "@types/express-serve-static-core": "^4.17.33",
                 "@types/qs": "*",
                 "@types/serve-static": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/express/-/express-4.17.17.tgz",
             "version": "4.17.17"
         },
         "@types/express-serve-static-core": {
-            "integrity": "sha512-TPBqmR/HRYI3eC2E5hmiivIzv+bidAfXofM+sbonAGvyDhySGw9/PQZFt2BLOrjUUR++4eJVpx6KnLQK1Fk9tA==",
+            "integrity": "sha512-fvr49XlCGoUj2Pp730AItckfjat4WNb0lb3kfrLWffd+RLeoGAMsq7UOy04PAPtoL01uKwcp6u8nhzpgpDYr3w==",
             "requires": {
                 "@types/node": "*",
                 "@types/qs": "*",
-                "@types/range-parser": "*"
+                "@types/range-parser": "*",
+                "@types/send": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.33.tgz",
-            "version": "4.17.33"
+            "resolved": "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.34.tgz",
+            "version": "4.17.34"
         },
         "@types/html-minifier-terser": {
             "integrity": "sha512-oh/6byDPnL1zeNXFrDXFLyZjkr1MsBG667IM792caf1L2UPOOMf65NFzjUH/ltyfwjAGfs1rsX1eftK0jC/KIg==",
             "resolved": "https://registry.npmjs.org/@types/html-minifier-terser/-/html-minifier-terser-6.1.0.tgz",
             "version": "6.1.0"
         },
         "@types/http-proxy": {
-            "integrity": "sha512-Qs5aULi+zV1bwKAg5z1PWnDXWmsn+LxIvUGv6E2+OOMYhclZMO+OXd9pYVf2gLykf2I7IV2u7oTHwChPNsvJ7g==",
+            "integrity": "sha512-HC8G7c1WmaF2ekqpnFq626xd3Zz0uvaqFmBJNRZCGEZCXkvSdJoNFn/8Ygbd9fKNQj8UzLdCETaI0UWPAjK7IA==",
             "requires": {
                 "@types/node": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/http-proxy/-/http-proxy-1.17.10.tgz",
-            "version": "1.17.10"
+            "resolved": "https://registry.npmjs.org/@types/http-proxy/-/http-proxy-1.17.11.tgz",
+            "version": "1.17.11"
         },
         "@types/json-schema": {
             "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
             "version": "7.0.11"
         },
         "@types/mime": {
-            "integrity": "sha512-Y4XFY5VJAuw0FgAqPNd6NNoV44jbq9Bz2L7Rh/J6jLTiHBSBJa9fxqQIvkIld4GsoDOcCbvzOUAbLPsSKKg+uA==",
-            "resolved": "https://registry.npmjs.org/@types/mime/-/mime-3.0.1.tgz",
-            "version": "3.0.1"
+            "integrity": "sha512-YATxVxgRqNH6nHEIsvg6k2Boc1JHI9ZbH5iWFFv/MTkchz3b1ieGDa5T0a9RznNdI0KhVbdbWSN+KWWrQZRxTw==",
+            "resolved": "https://registry.npmjs.org/@types/mime/-/mime-1.3.2.tgz",
+            "version": "1.3.2"
         },
         "@types/minimist": {
             "integrity": "sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==",
             "resolved": "https://registry.npmjs.org/@types/minimist/-/minimist-1.2.2.tgz",
             "version": "1.2.2"
         },
         "@types/node": {
-            "integrity": "sha512-E5Kwq2n4SbMzQOn6wnmBjuK9ouqlURrcZDVfbo9ftDDTFt3nk7ZKK4GMOzoYgnpQJKcxwQw+lGaBvvlMo0qN/Q==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.15.11.tgz",
-            "version": "18.15.11"
+            "integrity": "sha512-O+z53uwx64xY7D6roOi4+jApDGFg0qn6WHcxe5QeqjMaTezBO/mxdfFXIVAVVyNWKx84OmPB3L8kbVYOTeN34A==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz",
+            "version": "20.1.0"
         },
         "@types/normalize-package-data": {
             "integrity": "sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==",
             "resolved": "https://registry.npmjs.org/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz",
             "version": "2.4.1"
         },
         "@types/parse-json": {
@@ -585,14 +586,23 @@
             "version": "1.2.4"
         },
         "@types/retry": {
             "integrity": "sha512-wWKOClTTiizcZhXnPY4wikVAwmdYHp8q6DmC+EJUzAMsycb7HB32Kh9RN4+0gExjmPmZSAQjgURXIGATPegAvA==",
             "resolved": "https://registry.npmjs.org/@types/retry/-/retry-0.12.0.tgz",
             "version": "0.12.0"
         },
+        "@types/send": {
+            "integrity": "sha512-Cwo8LE/0rnvX7kIIa3QHCkcuF21c05Ayb0ZfxPiv0W8VRiZiNW/WuRupHKpqqGVGf7SUA44QSOUKaEd9lIrd/Q==",
+            "requires": {
+                "@types/mime": "^1",
+                "@types/node": "*"
+            },
+            "resolved": "https://registry.npmjs.org/@types/send/-/send-0.17.1.tgz",
+            "version": "0.17.1"
+        },
         "@types/serve-index": {
             "integrity": "sha512-d/Hs3nWDxNL2xAczmOVZNj92YZCS6RGxfBPjKzuu/XirCgXdpKEb88dYNbrYGint6IVWLNP+yonwVAuRC0T2Dg==",
             "requires": {
                 "@types/express": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/serve-index/-/serve-index-1.9.1.tgz",
             "version": "1.9.1"
@@ -750,20 +760,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
+                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-                    "version": "7.4.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+                    "version": "7.5.0"
                 },
                 "supports-color": {
                     "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
                     "requires": {
                         "has-flag": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
@@ -865,143 +875,143 @@
         },
         "@vue/web-component-wrapper": {
             "integrity": "sha512-Iu8Tbg3f+emIIMmI2ycSI8QcEuAUgPTgHwesDU1eKMLE4YC/c/sFbGc70QgMq31ijRftV0R7vCm9co6rldCeOA==",
             "resolved": "https://registry.npmjs.org/@vue/web-component-wrapper/-/web-component-wrapper-1.3.0.tgz",
             "version": "1.3.0"
         },
         "@webassemblyjs/ast": {
-            "integrity": "sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==",
+            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
             "requires": {
-                "@webassemblyjs/helper-numbers": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1"
+                "@webassemblyjs/helper-numbers": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/floating-point-hex-parser": {
-            "integrity": "sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-api-error": {
-            "integrity": "sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-buffer": {
-            "integrity": "sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-numbers": {
-            "integrity": "sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==",
+            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
             "requires": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-wasm-bytecode": {
-            "integrity": "sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-wasm-section": {
-            "integrity": "sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==",
+            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/ieee754": {
-            "integrity": "sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==",
+            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
             "requires": {
                 "@xtuc/ieee754": "^1.2.0"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/leb128": {
-            "integrity": "sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==",
+            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
             "requires": {
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/utf8": {
-            "integrity": "sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-edit": {
-            "integrity": "sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==",
+            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/helper-wasm-section": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-opt": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
-                "@webassemblyjs/wast-printer": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/helper-wasm-section": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-opt": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5",
+                "@webassemblyjs/wast-printer": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-gen": {
-            "integrity": "sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==",
+            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-opt": {
-            "integrity": "sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==",
+            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-parser": {
-            "integrity": "sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==",
+            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wast-printer": {
-            "integrity": "sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==",
+            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/ast": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@xtuc/ieee754": {
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
         "@xtuc/long": {
@@ -1359,17 +1369,17 @@
                 "lodash.memoize": "^4.1.2",
                 "lodash.uniq": "^4.5.0"
             },
             "resolved": "https://registry.npmjs.org/caniuse-api/-/caniuse-api-3.0.0.tgz",
             "version": "3.0.0"
         },
         "caniuse-lite": {
-            "integrity": "sha512-lZim4iUHhGcy5p+Ri/G7m84hJwncj+Kz7S5aD4hoQfslKZJgt0tHc/hafVbqHC5bbhHb+mrW2JOUHkI5KH7toQ==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001477.tgz",
-            "version": "1.0.30001477"
+            "integrity": "sha512-uv7/gXuHi10Whlj0pp5q/tsK/32J2QSqVRKQhs2j8VsDCjgyruAh/eEXHF822VqO9yT6iZKw3nRwZRSPBE9OQg==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001486.tgz",
+            "version": "1.0.30001486"
         },
         "case-sensitive-paths-webpack-plugin": {
             "integrity": "sha512-roIFONhcxog0JSSWbvVAh3OocukmSgpqOH6YpMkCvav/ySIV3JKg4Dc8vYtQjYi/UxpNE36r/9v+VqTQqgkYmw==",
             "resolved": "https://registry.npmjs.org/case-sensitive-paths-webpack-plugin/-/case-sensitive-paths-webpack-plugin-2.4.0.tgz",
             "version": "2.4.0"
         },
         "chalk": {
@@ -1526,17 +1536,17 @@
                 "parse5-htmlparser2-tree-adapter": "^6.0.0",
                 "yargs": "^16.0.0"
             },
             "resolved": "https://registry.npmjs.org/cli-highlight/-/cli-highlight-2.1.11.tgz",
             "version": "2.1.11"
         },
         "cli-spinners": {
-            "integrity": "sha512-/eG5sJcvEIwxcdYM86k5tPwn0MUzkX5YY3eImTGpJOZgVe4SdTMY14vQpcxgBzJ0wXwAYrS8E+c3uHeK4JNyzQ==",
-            "resolved": "https://registry.npmjs.org/cli-spinners/-/cli-spinners-2.8.0.tgz",
-            "version": "2.8.0"
+            "integrity": "sha512-4/aL9X3Wh0yiMQlE+eeRhWP6vclO3QRtw1JHKIT0FFUs5FjpFmESqtMvYZ0+lbzBw900b95mS0hohy+qn2VK/g==",
+            "resolved": "https://registry.npmjs.org/cli-spinners/-/cli-spinners-2.9.0.tgz",
+            "version": "2.9.0"
         },
         "clipboardy": {
             "integrity": "sha512-mKhiIL2DrQIsuXMgBgnfEHOZOryC7kY7YO//TN6c63wlEm3NG5tz+YgY5rVi29KCmq/QQjKYvM7a19+MDOTHOQ==",
             "requires": {
                 "arch": "^2.1.1",
                 "execa": "^1.0.0",
                 "is-wsl": "^2.1.1"
@@ -1645,17 +1655,17 @@
         },
         "colord": {
             "integrity": "sha512-jeC1axXpnb0/2nn/Y1LPuLdgXBLH7aDcHu4KEKfqw3CUhX7ZpfBSlPKyqXE6btIgEzfWtrX3/tyBCaCvXvMkOw==",
             "resolved": "https://registry.npmjs.org/colord/-/colord-2.9.3.tgz",
             "version": "2.9.3"
         },
         "colorette": {
-            "integrity": "sha512-3tlv/dIP7FWvj3BsbHrGLJ6l/oKh1O3TcgBqMn+yyCagOxc23fyzDS6HypQbgxWbkpDnf52p1LuR4eWDQ/K9WQ==",
-            "resolved": "https://registry.npmjs.org/colorette/-/colorette-2.0.19.tgz",
-            "version": "2.0.19"
+            "integrity": "sha512-IfEDxwoWIjkeXL1eXcDiow4UbKjhLdq6/EuSVR9GMN7KVH3r9gQ83e73hsz1Nd1T3ijd5xv1wcWRYO+D6kCI2w==",
+            "resolved": "https://registry.npmjs.org/colorette/-/colorette-2.0.20.tgz",
+            "version": "2.0.20"
         },
         "colorspace": {
             "dependencies": {
                 "color": {
                     "integrity": "sha512-aBl7dZI9ENN6fUGC7mWpMTPNHmWUSNan9tuWN6ahh5ZLNk9baLJOnSMlrQkHcrfFgz2/RigjUVAjdx36VcemKA==",
                     "requires": {
                         "color-convert": "^1.9.3",
@@ -1855,20 +1865,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
+                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-                    "version": "7.4.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+                    "version": "7.5.0"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
@@ -1909,23 +1919,23 @@
                 },
                 "json-schema-traverse": {
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 },
                 "schema-utils": {
-                    "integrity": "sha512-1edyXKgh6XnJsJSQ8mKWXnN/BVaIbFMLpouRUrXgVq7WYne5kw3MW7UPhO44uRXQSIpTSXoJbmrR2X0w9kUTyg==",
+                    "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
                     "requires": {
                         "@types/json-schema": "^7.0.9",
-                        "ajv": "^8.8.0",
+                        "ajv": "^8.9.0",
                         "ajv-formats": "^2.1.1",
-                        "ajv-keywords": "^5.0.0"
+                        "ajv-keywords": "^5.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
-                    "version": "4.0.0"
+                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
+                    "version": "4.0.1"
                 }
             },
             "integrity": "sha512-1u6D71zeIfgngN2XNRJefc/hY7Ybsxd74Jm4qngIXyUEk7fss3VUzuHxLAq/R8NAba4QU9OUSaMZlbpRc7bM4Q==",
             "requires": {
                 "cssnano": "^5.0.6",
                 "jest-worker": "^27.0.2",
                 "postcss": "^8.3.5",
@@ -2198,20 +2208,20 @@
         },
         "dns-equal": {
             "integrity": "sha512-z+paD6YUQsk+AbGCEM4PrOXSss5gd66QfcVBFTKR/HpFL9jCqikS94HYwKww6fQyO7IxrIIyUu+g0Ka9tUS2Cg==",
             "resolved": "https://registry.npmjs.org/dns-equal/-/dns-equal-1.0.0.tgz",
             "version": "1.0.0"
         },
         "dns-packet": {
-            "integrity": "sha512-USawdAUzRkV6xrqTjiAEp6M9YagZEzWcSUaZTcIFAiyQWW1SoI6KyId8y2+/71wbgHKQAKd+iupLv4YvEwYWvA==",
+            "integrity": "sha512-rza3UH1LwdHh9qyPXp8lkwpjSNk/AMD3dPytUoRoqnypDUhY0xvbdmVhWOfxO68frEfV9BU8V12Ez7ZsHGZpCQ==",
             "requires": {
                 "@leichtgewicht/ip-codec": "^2.0.1"
             },
-            "resolved": "https://registry.npmjs.org/dns-packet/-/dns-packet-5.5.0.tgz",
-            "version": "5.5.0"
+            "resolved": "https://registry.npmjs.org/dns-packet/-/dns-packet-5.6.0.tgz",
+            "version": "5.6.0"
         },
         "dom-converter": {
             "integrity": "sha512-gd3ypIPfOMr9h5jIKq8E3sHOTCjeirnl0WK5ZdS1AW0Odt0b1PaWaHdJ4Qk4klv+YB9aJBS7mESXjFoDQPu6DA==",
             "requires": {
                 "utila": "~0.4"
             },
             "resolved": "https://registry.npmjs.org/dom-converter/-/dom-converter-0.2.0.tgz",
@@ -2281,17 +2291,17 @@
         },
         "ee-first": {
             "integrity": "sha512-WMwm9LhRUo+WUaRN+vRuETqG89IgZphVSNkdFgeb6sS/E4OrDIN7t48CAewSHXc6C8lefD8KKfr5vY61brQlow==",
             "resolved": "https://registry.npmjs.org/ee-first/-/ee-first-1.1.1.tgz",
             "version": "1.1.1"
         },
         "electron-to-chromium": {
-            "integrity": "sha512-UTkCbNTAcGXABmEnQrGcW4m3cG6fcyBfD4KDF0iyEAlbrGZiY9dmslyDAGOD1Kr5biN2F743Y30aRCOtau35Vw==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.357.tgz",
-            "version": "1.4.357"
+            "integrity": "sha512-L9zlje9bIw0h+CwPQumiuVlfMcV4boxRjFIWDcLfFqTZNbkwOExBzfmswytHawObQX4OUhtNv8gIiB21kOurIg==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.385.tgz",
+            "version": "1.4.385"
         },
         "emoji-regex": {
             "integrity": "sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz",
             "version": "8.0.0"
         },
         "emojis-list": {
@@ -2314,21 +2324,21 @@
             "requires": {
                 "once": "^1.4.0"
             },
             "resolved": "https://registry.npmjs.org/end-of-stream/-/end-of-stream-1.4.4.tgz",
             "version": "1.4.4"
         },
         "enhanced-resolve": {
-            "integrity": "sha512-QHTXI/sZQmko1cbDoNAa3mJ5qhWUUNAq3vR0/YiD379fWQrcfuoX1+HW2S0MTt7XmoPLapdaDKUtelUSPic7hQ==",
+            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
             "requires": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.12.0.tgz",
-            "version": "5.12.0"
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
+            "version": "5.13.0"
         },
         "entities": {
             "integrity": "sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==",
             "resolved": "https://registry.npmjs.org/entities/-/entities-2.2.0.tgz",
             "version": "2.2.0"
         },
         "error-ex": {
@@ -2344,17 +2354,17 @@
             "requires": {
                 "stackframe": "^1.3.4"
             },
             "resolved": "https://registry.npmjs.org/error-stack-parser/-/error-stack-parser-2.1.4.tgz",
             "version": "2.1.4"
         },
         "es-module-lexer": {
-            "integrity": "sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
-            "version": "0.9.3"
+            "integrity": "sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "escalade": {
             "integrity": "sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==",
             "resolved": "https://registry.npmjs.org/escalade/-/escalade-3.1.1.tgz",
             "version": "3.1.1"
         },
         "escape-html": {
@@ -2906,24 +2916,24 @@
                 "relateurl": "^0.2.7",
                 "terser": "^5.10.0"
             },
             "resolved": "https://registry.npmjs.org/html-minifier-terser/-/html-minifier-terser-6.1.0.tgz",
             "version": "6.1.0"
         },
         "html-webpack-plugin": {
-            "integrity": "sha512-sy88PC2cRTVxvETRgUHFrL4No3UxvcH8G1NepGhqaTT+GXN2kTamqasot0inS5hXeg1cMbFDt27zzo9p35lZVw==",
+            "integrity": "sha512-cTUzZ1+NqjGEKjmVgZKLMdiFg3m9MdRXkZW2OEe69WYVi5ONLMmlnSZdXzGGMOq0C8jGDrL6EWyEDDUioHO/pA==",
             "requires": {
                 "@types/html-minifier-terser": "^6.0.0",
                 "html-minifier-terser": "^6.0.2",
                 "lodash": "^4.17.21",
                 "pretty-error": "^4.0.0",
                 "tapable": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/html-webpack-plugin/-/html-webpack-plugin-5.5.0.tgz",
-            "version": "5.5.0"
+            "resolved": "https://registry.npmjs.org/html-webpack-plugin/-/html-webpack-plugin-5.5.1.tgz",
+            "version": "5.5.1"
         },
         "htmlparser2": {
             "integrity": "sha512-gyyPk6rgonLFEDGoeRgQNaEUvdJ4ktTmmUh/h2t7s+M8oPpIPxgNACWa+6ESR57kXstwqPiCut0V8NRpcwgU7A==",
             "requires": {
                 "domelementtype": "^2.0.1",
                 "domhandler": "^4.0.0",
                 "domutils": "^2.5.2",
@@ -3178,24 +3188,24 @@
                 "merge-stream": "^2.0.0",
                 "supports-color": "^8.0.0"
             },
             "resolved": "https://registry.npmjs.org/jest-worker/-/jest-worker-27.5.1.tgz",
             "version": "27.5.1"
         },
         "joi": {
-            "integrity": "sha512-FariIi9j6QODKATGBrEX7HZcja8Bsh3rfdGYy/Sb65sGlZWK/QWesU1ghk7aJWDj95knjXlQfSmzFSPPkLVsfw==",
+            "integrity": "sha512-Itk/r+V4Dx0V3c7RLFdRh12IOjySm2/WGPMubBT92cQvRfYZhPM2W0hZlctjj72iES8jsRCwp7S/cRmWBnJ4nw==",
             "requires": {
                 "@hapi/hoek": "^9.0.0",
                 "@hapi/topo": "^5.0.0",
                 "@sideway/address": "^4.1.3",
                 "@sideway/formula": "^3.0.1",
                 "@sideway/pinpoint": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/joi/-/joi-17.9.1.tgz",
-            "version": "17.9.1"
+            "resolved": "https://registry.npmjs.org/joi/-/joi-17.9.2.tgz",
+            "version": "17.9.2"
         },
         "jquery": {
             "integrity": "sha512-v28EW9DWDFpzcD9O5iyJXg3R3+q+mET5JhnjJzQUZMHOv67bpSIHq81GEYpPNZHG+XXHsfSme3nxp/hndKEcsQ==",
             "peer": true,
             "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.6.4.tgz",
             "version": "3.6.4"
         },
@@ -3517,20 +3527,20 @@
         },
         "media-typer": {
             "integrity": "sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==",
             "resolved": "https://registry.npmjs.org/media-typer/-/media-typer-0.3.0.tgz",
             "version": "0.3.0"
         },
         "memfs": {
-            "integrity": "sha512-yK6o8xVJlQerz57kvPROwTMgx5WtGwC2ZxDtOUsnGl49rHjYkfQoPNZPCKH73VdLE1BwBu/+Fx/NL8NYMUw2aA==",
+            "integrity": "sha512-UWbFJKvj5k+nETdteFndTpYxdeTMox/ULeqX5k/dpaQJCCFmj5EeKv3dBcyO2xmkRAx2vppRu5dVG7SOtsGOzA==",
             "requires": {
                 "fs-monkey": "^1.0.3"
             },
-            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.0.tgz",
-            "version": "3.5.0"
+            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.1.tgz",
+            "version": "3.5.1"
         },
         "merge-descriptors": {
             "integrity": "sha512-cCi6g3/Zr1iqQi6ySbseM1Xvooa98N0w31jzUYrXPX2xqObmFGHJ0tQ5u74H3mVh7wLouTseZyYIq39g8cNp1w==",
             "resolved": "https://registry.npmjs.org/merge-descriptors/-/merge-descriptors-1.0.1.tgz",
             "version": "1.0.1"
         },
         "merge-source-map": {
@@ -3616,23 +3626,23 @@
                 },
                 "json-schema-traverse": {
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 },
                 "schema-utils": {
-                    "integrity": "sha512-1edyXKgh6XnJsJSQ8mKWXnN/BVaIbFMLpouRUrXgVq7WYne5kw3MW7UPhO44uRXQSIpTSXoJbmrR2X0w9kUTyg==",
+                    "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
                     "requires": {
                         "@types/json-schema": "^7.0.9",
-                        "ajv": "^8.8.0",
+                        "ajv": "^8.9.0",
                         "ajv-formats": "^2.1.1",
-                        "ajv-keywords": "^5.0.0"
+                        "ajv-keywords": "^5.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
-                    "version": "4.0.0"
+                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
+                    "version": "4.0.1"
                 }
             },
             "integrity": "sha512-9HaR++0mlgom81s95vvNjxkg52n2b5s//3ZTI1EtzFb98awsLSivs2LMsVqnQ3ay0PVhqWcGNyDaTE961FOcjQ==",
             "requires": {
                 "schema-utils": "^4.0.0"
             },
             "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.5.tgz",
@@ -3777,33 +3787,33 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
+                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-                    "version": "7.4.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+                    "version": "7.5.0"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
-            "integrity": "sha512-jAlSOFR1Bls963NmFwxeQkNTzqjUF0NThm8Le7eRIRGzFUVJuMOFZDLv5Y30W/Oaw+KEebEJLAigwO9gQHoEmw==",
+            "integrity": "sha512-zNy02qivjjRosswoYmPi8hIKJRr8MpQyeKT6qlcq/OnOgA3Rhoae+IYOqsM9V5+JnHWmxKnWOT2GxvtqdtOCXA==",
             "requires": {
                 "semver": "^7.3.5"
             },
-            "resolved": "https://registry.npmjs.org/node-abi/-/node-abi-3.35.0.tgz",
-            "version": "3.35.0"
+            "resolved": "https://registry.npmjs.org/node-abi/-/node-abi-3.40.0.tgz",
+            "version": "3.40.0"
         },
         "node-addon-api": {
             "integrity": "sha512-eh0GgfEkpnoWDq+VY8OyvYhFEzBk6jIYbRKdIlyTiAXIVJ8PyBaKb0rp7oDtoddbdoHWhq8wwr+XZ81F1rpNdA==",
             "resolved": "https://registry.npmjs.org/node-addon-api/-/node-addon-api-5.1.0.tgz",
             "version": "5.1.0"
         },
         "node-fetch": {
@@ -4190,22 +4200,22 @@
                 "debug": "^3.2.7",
                 "mkdirp": "^0.5.6"
             },
             "resolved": "https://registry.npmjs.org/portfinder/-/portfinder-1.0.32.tgz",
             "version": "1.0.32"
         },
         "postcss": {
-            "integrity": "sha512-tP7u/Sn/dVxK2NnruI4H9BG+x+Wxz6oeZ1cJ8P6G/PZY0IKk4k/63TDsQf2kQq3+qoJeLm2kIBUNlZe3zgb4Zg==",
+            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
             "requires": {
-                "nanoid": "^3.3.4",
+                "nanoid": "^3.3.6",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.21.tgz",
-            "version": "8.4.21"
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
+            "version": "8.4.23"
         },
         "postcss-calc": {
             "integrity": "sha512-SmWMSJmB8MRnnULldx0lQIyhSNvuDl9HfrZkaqqE/WHAhToYsAvDq+yAsA/kIyINDszOp3Rh0GFoNuH5Ypsm3Q==",
             "requires": {
                 "postcss-selector-parser": "^6.0.9",
                 "postcss-value-parser": "^4.2.0"
             },
@@ -4263,20 +4273,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
+                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-                    "version": "7.4.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+                    "version": "7.5.0"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
@@ -4472,21 +4482,21 @@
             "requires": {
                 "postcss-value-parser": "^4.2.0"
             },
             "resolved": "https://registry.npmjs.org/postcss-reduce-transforms/-/postcss-reduce-transforms-5.1.0.tgz",
             "version": "5.1.0"
         },
         "postcss-selector-parser": {
-            "integrity": "sha512-zbARubNdogI9j7WY4nQJBiNqQf3sLS3wCP4WfOidu+p28LofJqDH1tcXypGrcmMHhDk2t9wGhCsYe/+szLTy1g==",
+            "integrity": "sha512-NdxGCAZdRrwVI1sy59+Wzrh+pMMHxapGnpfenDVlMEXoOcvt4pGE0JLK9YY2F5dLxcFYA/YbVQKhcGU+FtSYQg==",
             "requires": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.11.tgz",
-            "version": "6.0.11"
+            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.12.tgz",
+            "version": "6.0.12"
         },
         "postcss-svgo": {
             "integrity": "sha512-D75KsH1zm5ZrHyxPakAxJWtkyXew5qwS70v56exwvw542d9CRtTo78K0WeFxZB4G7JXKKMbEZtZayTGdIky/eA==",
             "requires": {
                 "postcss-value-parser": "^4.2.0",
                 "svgo": "^2.7.0"
             },
@@ -4522,18 +4532,18 @@
                 "tar-fs": "^2.0.0",
                 "tunnel-agent": "^0.6.0"
             },
             "resolved": "https://registry.npmjs.org/prebuild-install/-/prebuild-install-7.1.1.tgz",
             "version": "7.1.1"
         },
         "prettier": {
-            "integrity": "sha512-yPngTo3aXUUmyuTjeTUT75txrf+aMh9FiD7q9ZE/i6r0bPb22g4FsE6Y338PQX1bmfy08i9QQCB7/rcUAVntfw==",
+            "integrity": "sha512-tdN8qQGvNjw4CHbY+XXk0JgCXn9QiF21a55rBe5LJAU+kDyC4WQn4+awm2Xfk2lQMk5fKup9XgzTZtGkjBdP9Q==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/prettier/-/prettier-2.8.7.tgz",
-            "version": "2.8.7"
+            "resolved": "https://registry.npmjs.org/prettier/-/prettier-2.8.8.tgz",
+            "version": "2.8.8"
         },
         "pretty-error": {
             "integrity": "sha512-AoJ5YMAcXKYxKhuJGdcvse+Voc6v1RgnsR3nWcYU7q4t6z0Q6T86sv5Zq8VIRbOWWFpvdGE83LtdSMNd+6Y0xw==",
             "requires": {
                 "lodash": "^4.17.20",
                 "renderkid": "^3.0.0"
             },
@@ -4818,32 +4828,32 @@
         },
         "safer-buffer": {
             "integrity": "sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==",
             "resolved": "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz",
             "version": "2.1.2"
         },
         "sass": {
-            "integrity": "sha512-PDsN7BrVkNZK2+dj/dpKQAWZavbAQ87IXqVvw2+oEYI+GwlTWkvbQtL7F2cCNbMqJEYKPh1EcjSxsnqIb/kyaQ==",
+            "integrity": "sha512-NHpxIzN29MXvWiuswfc1W3I0N8SXBd8UR26WntmDlRYf0bSADnwnOjsyMZ3lMezSlArD33Vs3YFhp7dWvL770A==",
             "requires": {
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.61.0.tgz",
-            "version": "1.61.0"
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.62.1.tgz",
+            "version": "1.62.1"
         },
         "schema-utils": {
-            "integrity": "sha512-Y5PQxS4ITlC+EahLuXaY86TXfR7Dc5lw294alXOq86JAHCihAIZfqv8nNCWvaEJvaC51uN9hbLGeV0cFBdH+Fw==",
+            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
             "requires": {
                 "@types/json-schema": "^7.0.8",
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.1.tgz",
-            "version": "3.1.1"
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "select-hose": {
             "integrity": "sha512-mEugaLK+YfkijB4fx0e6kImuJdCIt2LxCRcbEYPqRGCs4F2ogyfZU5IAZRdjCP8JPq2AtdNoC/Dux63d9Kiryg==",
             "resolved": "https://registry.npmjs.org/select-hose/-/select-hose-2.0.0.tgz",
             "version": "2.0.0"
         },
         "selfsigned": {
@@ -5000,20 +5010,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
+                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-                    "version": "7.4.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+                    "version": "7.5.0"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
@@ -5335,35 +5345,35 @@
             "dependencies": {
                 "commander": {
                     "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
                     "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
                     "version": "2.20.3"
                 }
             },
-            "integrity": "sha512-HPa/FdTB9XGI2H1/keLFZHxl6WNvAI4YalHGtDQTlMnJcoqSab1UwL4l1hGEhs6/GmLHBZIg/YgB++jcbzoOEg==",
+            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
             "requires": {
                 "@jridgewell/source-map": "^0.3.2",
                 "acorn": "^8.5.0",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.16.9.tgz",
-            "version": "5.16.9"
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
+            "version": "5.17.1"
         },
         "terser-webpack-plugin": {
-            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
+            "integrity": "sha512-WiHL3ElchZMsK27P8uIUh4604IgJyAW47LVXGbEoB21DbQcZ+OuMpGjVYnEUaqcWM6dO8uS2qUbA7LSCWqvsbg==",
             "requires": {
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
                 "serialize-javascript": "^6.0.1",
-                "terser": "^5.16.5"
+                "terser": "^5.16.8"
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
-            "version": "5.3.7"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.8.tgz",
+            "version": "5.3.8"
         },
         "text-hex": {
             "integrity": "sha512-uuVGNWzgJ4yhRaNSiubPY7OjISw4sw4E5Uv0wbjp+OzcbmVU/rsT8ujgcXJhn9ypzsgr5vlzpPqP+MBBKcGvbg==",
             "resolved": "https://registry.npmjs.org/text-hex/-/text-hex-1.0.0.tgz",
             "version": "1.0.0"
         },
         "thenify": {
@@ -5507,21 +5517,21 @@
         },
         "unpipe": {
             "integrity": "sha512-pjy2bYhSsufwWlKwPc+l3cN7+wuJlK6uz0YdJEOlQDbl6jo/YlPi4mb8agUkVC8BF7V8NuzeyPNqRksA3hztKQ==",
             "resolved": "https://registry.npmjs.org/unpipe/-/unpipe-1.0.0.tgz",
             "version": "1.0.0"
         },
         "update-browserslist-db": {
-            "integrity": "sha512-OztqDenkfFkbSG+tRxBeAnCVPckDBcvibKd35yDONx6OU8N7sqgwc7rCbkJ/WcYtVRZ4ba68d6byhC21GFh7sQ==",
+            "integrity": "sha512-dCwEFf0/oT85M1fHBg4F0jtLwJrutGoHSQXCh7u4o2t1drG+c0a9Flnqww6XUKSfQMPpJBRjU8d4RXB09qtvaA==",
             "requires": {
                 "escalade": "^3.1.1",
                 "picocolors": "^1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.10.tgz",
-            "version": "1.0.10"
+            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.11.tgz",
+            "version": "1.0.11"
         },
         "uri-js": {
             "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
             "requires": {
                 "punycode": "^2.1.0"
             },
             "resolved": "https://registry.npmjs.org/uri-js/-/uri-js-4.4.1.tgz",
@@ -5599,41 +5609,31 @@
                     "version": "1.1.4"
                 },
                 "has-flag": {
                     "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
                     "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz",
                     "version": "4.0.0"
                 },
-                "loader-utils": {
-                    "integrity": "sha512-xXqpXoINfFhgua9xiqD8fPFHgkoq1mmmpE92WlDbm9rNRd/EbRb+Gqf908T2DMfuHjjJlksiK2RbHVOdD/MqSw==",
-                    "requires": {
-                        "big.js": "^5.2.2",
-                        "emojis-list": "^3.0.0",
-                        "json5": "^2.1.2"
-                    },
-                    "resolved": "https://registry.npmjs.org/loader-utils/-/loader-utils-2.0.4.tgz",
-                    "version": "2.0.4"
-                },
                 "supports-color": {
                     "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
                     "requires": {
                         "has-flag": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
                     "version": "7.2.0"
                 }
             },
-            "integrity": "sha512-/OOyugJnImKCkAKrAvdsWMuwoCqGxWT5USLsjohzWbMgOwpA5wQmzQiLMzZd7DjhIfunzAGIApTOgIylz/kwcg==",
+            "integrity": "sha512-zAjrT+TNWTpgRODxqDfzbDyvuTf5kCP9xmMk8aspQKuYNnTY2r0XK/bHu1DKLpSpk0I6fkQph5OLKB7HcRIPZw==",
             "requires": {
                 "chalk": "^4.1.0",
                 "hash-sum": "^2.0.0",
-                "loader-utils": "^2.0.0"
+                "watchpack": "^2.4.0"
             },
-            "resolved": "https://registry.npmjs.org/vue-loader/-/vue-loader-17.0.1.tgz",
-            "version": "17.0.1"
+            "resolved": "https://registry.npmjs.org/vue-loader/-/vue-loader-17.1.0.tgz",
+            "version": "17.1.0"
         },
         "vue-style-loader": {
             "dependencies": {
                 "hash-sum": {
                     "integrity": "sha512-fUs4B4L+mlt8/XAtSOGMUO1TXmAelItBPtJG7CyHJfYTdDjwisntGO2JQz7oUsatOY9o68+57eziUVNw/mRHmA==",
                     "resolved": "https://registry.npmjs.org/hash-sum/-/hash-sum-1.0.2.tgz",
                     "version": "1.0.2"
@@ -5688,43 +5688,43 @@
         },
         "webidl-conversions": {
             "integrity": "sha512-2JAn3z8AR6rjK8Sm8orRC0h/bcl/DqL7tRPdGZ4I1CjdF+EaMLmYxBHyXuKL849eucPFhvBoxMsflfOb8kxaeQ==",
             "resolved": "https://registry.npmjs.org/webidl-conversions/-/webidl-conversions-3.0.1.tgz",
             "version": "3.0.1"
         },
         "webpack": {
-            "integrity": "sha512-gT5DP72KInmE/3azEaQrISjTvLYlSM0j1Ezhht/KLVkrqtv10JoP/RXhwmX/frrutOPuSq3o5Vq0ehR/4Vmd1g==",
+            "integrity": "sha512-iGNA2fHhnDcV1bONdUu554eZx+XeldsaeQ8T67H6KKHl2nUSwX8Zm7cmzOA46ox/X1ARxf7Bjv8wQ/HsB5fxBg==",
             "requires": {
                 "@types/eslint-scope": "^3.7.3",
-                "@types/estree": "^0.0.51",
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/wasm-edit": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
+                "@types/estree": "^1.0.0",
+                "@webassemblyjs/ast": "^1.11.5",
+                "@webassemblyjs/wasm-edit": "^1.11.5",
+                "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.10.0",
-                "es-module-lexer": "^0.9.0",
+                "enhanced-resolve": "^5.13.0",
+                "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.1.0",
+                "schema-utils": "^3.1.2",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.1.3",
+                "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.78.0.tgz",
-            "version": "5.78.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.82.0.tgz",
+            "version": "5.82.0"
         },
         "webpack-bundle-analyzer": {
             "dependencies": {
                 "ansi-styles": {
                     "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
                     "requires": {
                         "color-convert": "^2.0.1"
@@ -5821,23 +5821,23 @@
                 },
                 "json-schema-traverse": {
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 },
                 "schema-utils": {
-                    "integrity": "sha512-1edyXKgh6XnJsJSQ8mKWXnN/BVaIbFMLpouRUrXgVq7WYne5kw3MW7UPhO44uRXQSIpTSXoJbmrR2X0w9kUTyg==",
+                    "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
                     "requires": {
                         "@types/json-schema": "^7.0.9",
-                        "ajv": "^8.8.0",
+                        "ajv": "^8.9.0",
                         "ajv-formats": "^2.1.1",
-                        "ajv-keywords": "^5.0.0"
+                        "ajv-keywords": "^5.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
-                    "version": "4.0.0"
+                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
+                    "version": "4.0.1"
                 }
             },
             "integrity": "sha512-hj5CYrY0bZLB+eTO+x/j67Pkrquiy7kWepMHmUMoPsmcUaeEnQJqFzHJOyxgWlq746/wUuA64p9ta34Kyb01pA==",
             "requires": {
                 "colorette": "^2.0.10",
                 "memfs": "^3.4.3",
                 "mime-types": "^2.1.31",
@@ -5875,32 +5875,32 @@
                 },
                 "json-schema-traverse": {
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 },
                 "schema-utils": {
-                    "integrity": "sha512-1edyXKgh6XnJsJSQ8mKWXnN/BVaIbFMLpouRUrXgVq7WYne5kw3MW7UPhO44uRXQSIpTSXoJbmrR2X0w9kUTyg==",
+                    "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
                     "requires": {
                         "@types/json-schema": "^7.0.9",
-                        "ajv": "^8.8.0",
+                        "ajv": "^8.9.0",
                         "ajv-formats": "^2.1.1",
-                        "ajv-keywords": "^5.0.0"
+                        "ajv-keywords": "^5.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
-                    "version": "4.0.0"
+                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
+                    "version": "4.0.1"
                 },
                 "ws": {
                     "integrity": "sha512-x9vcZYTrFPC7aSIbj7sRCYo7L/Xb8Iy+pW0ng0wt2vCJv7M9HOMy0UoN3rr+IFC7hb7vXoqS+P9ktyLLLhO+LA==",
                     "requires": {},
                     "resolved": "https://registry.npmjs.org/ws/-/ws-8.13.0.tgz",
                     "version": "8.13.0"
                 }
             },
-            "integrity": "sha512-5i6TrGBRxG4vnfDpB6qSQGfnB6skGBXNL5/542w2uRGLimX6qeE5BQMLrzIC3JYV/xlGOv+s+hTleI9AZKUQNw==",
+            "integrity": "sha512-HmNB5QeSl1KpulTBQ8UT4FPrByYyaLxpJoQ0+s7EvUrMc16m0ZS1sgb1XGqzmgCPk0c9y+aaXxn11tbLzuM7NQ==",
             "requires": {
                 "@types/bonjour": "^3.5.9",
                 "@types/connect-history-api-fallback": "^1.3.5",
                 "@types/express": "^4.17.13",
                 "@types/serve-index": "^1.9.1",
                 "@types/serve-static": "^1.13.10",
                 "@types/sockjs": "^0.3.33",
@@ -5925,16 +5925,16 @@
                 "selfsigned": "^2.1.1",
                 "serve-index": "^1.9.1",
                 "sockjs": "^0.3.24",
                 "spdy": "^4.0.2",
                 "webpack-dev-middleware": "^5.3.1",
                 "ws": "^8.13.0"
             },
-            "resolved": "https://registry.npmjs.org/webpack-dev-server/-/webpack-dev-server-4.13.2.tgz",
-            "version": "4.13.2"
+            "resolved": "https://registry.npmjs.org/webpack-dev-server/-/webpack-dev-server-4.15.0.tgz",
+            "version": "4.15.0"
         },
         "webpack-merge": {
             "integrity": "sha512-/SaI7xY0831XwP6kzuwhKWVKDP9t1QY1h65lAFLbZqMPIuYcD9QAW4u9STIbU9kaJbPBB/geU/gLr1wDjOhQ+Q==",
             "requires": {
                 "clone-deep": "^4.0.1",
                 "wildcard": "^2.0.0"
             },
@@ -5985,17 +5985,17 @@
             "requires": {
                 "isexe": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/which/-/which-1.3.1.tgz",
             "version": "1.3.1"
         },
         "wildcard": {
-            "integrity": "sha512-JcKqAHLPxcdb9KM49dufGXn2x3ssnfjbcaQdLlfZsL9rH9wgDQjUtDxbo8NE0F6SFvydeu1VhZe7hZuHsB2/pw==",
-            "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.0.tgz",
-            "version": "2.0.0"
+            "integrity": "sha512-CC1bOL87PIWSBhDcTrdeLo6eGT7mCFtrg0uIJtqJUFyK+eJnzl8A1niH56uu7KMa5XFrtiV+AQuHO3n7DsHnLQ==",
+            "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.1.tgz",
+            "version": "2.0.1"
         },
         "winston": {
             "dependencies": {
                 "async": {
                     "integrity": "sha512-iAB+JbDEGXhyIUavoDl9WP/Jj106Kz9DEn1DPgYw5ruDn0e3Wgi3sKFm55sASdGBNOQB8F59d9qQ7deqrHA8wQ==",
                     "resolved": "https://registry.npmjs.org/async/-/async-3.2.4.tgz",
                     "version": "3.2.4"
@@ -6176,89 +6176,89 @@
             "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.21.4.tgz",
             "version": "7.21.4"
         },
         "node_modules/@babel/compat-data": {
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-/DYyDpeCfaVinT40FPGdkkb+lYSKvsVuMjDAG7jPOWWiM1ibOaB9CXJAlc4d1QpP/U2q2P9jbrSlClKSErd55g==",
-            "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.21.4.tgz",
-            "version": "7.21.4"
+            "integrity": "sha512-KYMqFYTaenzMK4yUtf4EW9wc4N9ef80FsbMtkwool5zpwl4YrT1SdWYSTRcT94KO4hannogdS+LxY7L+arP3gA==",
+            "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.21.7.tgz",
+            "version": "7.21.7"
         },
         "node_modules/@babel/core": {
             "dependencies": {
                 "@ampproject/remapping": "^2.2.0",
                 "@babel/code-frame": "^7.21.4",
-                "@babel/generator": "^7.21.4",
-                "@babel/helper-compilation-targets": "^7.21.4",
-                "@babel/helper-module-transforms": "^7.21.2",
-                "@babel/helpers": "^7.21.0",
-                "@babel/parser": "^7.21.4",
+                "@babel/generator": "^7.21.5",
+                "@babel/helper-compilation-targets": "^7.21.5",
+                "@babel/helper-module-transforms": "^7.21.5",
+                "@babel/helpers": "^7.21.5",
+                "@babel/parser": "^7.21.8",
                 "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.4",
-                "@babel/types": "^7.21.4",
+                "@babel/traverse": "^7.21.5",
+                "@babel/types": "^7.21.5",
                 "convert-source-map": "^1.7.0",
                 "debug": "^4.1.0",
                 "gensync": "^1.0.0-beta.2",
                 "json5": "^2.2.2",
                 "semver": "^6.3.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/babel"
             },
-            "integrity": "sha512-qt/YV149Jman/6AfmlxJ04LMIu8bMoyl3RB91yTFrxQmgbrSvQMy7cI8Q62FHx1t8wJ8B5fu0UDoLwHAhUo1QA==",
+            "integrity": "sha512-YeM22Sondbo523Sz0+CirSPnbj9bG3P0CdHcBZdqUuaeOaYEFbOLoGU7lebvGP6P5J/WE9wOn7u7C4J9HvS1xQ==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.21.8.tgz",
+            "version": "7.21.8"
         },
         "node_modules/@babel/generator": {
             "dependencies": {
-                "@babel/types": "^7.21.4",
+                "@babel/types": "^7.21.5",
                 "@jridgewell/gen-mapping": "^0.3.2",
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jsesc": "^2.5.1"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-NieM3pVIYW2SwGzKoqfPrQsf4xGs9M9AIG3ThppsSRmO+m7eQhmI6amajKMUeIO37wFfsvnvcxQFx6x6iqxDnA==",
+            "integrity": "sha512-SrKK/sRv8GesIW1bDagf9cCG38IOMYZusoe1dfg0D8aiUe3Amvoj1QtjTPAWcfrZFvIwlleLb0gxzQidL9w14w==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@babel/helper-compilation-targets": {
             "dependencies": {
-                "@babel/compat-data": "^7.21.4",
+                "@babel/compat-data": "^7.21.5",
                 "@babel/helper-validator-option": "^7.21.0",
                 "browserslist": "^4.21.3",
                 "lru-cache": "^5.1.1",
                 "semver": "^6.3.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-Fa0tTuOXZ1iL8IeDFUWCzjZcn+sJGd9RZdH9esYVjEejGmzf+FFYQpMi/kZUk2kPy/q1H3/GPw7np8qar/stfg==",
+            "integrity": "sha512-1RkbFGUKex4lvsB9yhIfWltJM5cZKUftB2eNajaDv3dCMEp49iBG0K14uH8NnX9IPux2+mK7JGEOB0jn48/J6w==",
             "peerDependencies": {
                 "@babel/core": "^7.0.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@babel/helper-environment-visitor": {
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-3r/aACDJ3fhQ/EVgFy0hpj8oHyHpQc+LPtJoY9SzTThAsStm4Ptegq92vqKoE3vD706ZVFWITnMnxucw+S9Ipg==",
+            "integrity": "sha512-IYl4gZ3ETsWocUWgsFZLM5i1BYx9SoemminVEXadgLBa9TdeorzgLKm8wWLA6J1N/kT3Kch8XIk1laNzYoHKvQ==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.18.9.tgz",
-            "version": "7.18.9"
+            "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@babel/helper-function-name": {
             "dependencies": {
                 "@babel/template": "^7.20.7",
                 "@babel/types": "^7.21.0"
             },
             "engines": {
@@ -6291,42 +6291,42 @@
             "integrity": "sha512-orajc5T2PsRYUN3ZryCEFeMDYwyw09c/pZeaQEZPH0MpKzSvn3e0uXsDBu3k03VI+9DBiRo+l22BfKTpKwa/Wg==",
             "peer": true,
             "resolved": "https://registry.npmjs.org/@babel/helper-module-imports/-/helper-module-imports-7.21.4.tgz",
             "version": "7.21.4"
         },
         "node_modules/@babel/helper-module-transforms": {
             "dependencies": {
-                "@babel/helper-environment-visitor": "^7.18.9",
-                "@babel/helper-module-imports": "^7.18.6",
-                "@babel/helper-simple-access": "^7.20.2",
+                "@babel/helper-environment-visitor": "^7.21.5",
+                "@babel/helper-module-imports": "^7.21.4",
+                "@babel/helper-simple-access": "^7.21.5",
                 "@babel/helper-split-export-declaration": "^7.18.6",
                 "@babel/helper-validator-identifier": "^7.19.1",
                 "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.2",
-                "@babel/types": "^7.21.2"
+                "@babel/traverse": "^7.21.5",
+                "@babel/types": "^7.21.5"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-79yj2AR4U/Oqq/WOV7Lx6hUjau1Zfo4cI+JLAVYeMV5XIlbOhmjEk5ulbTc9fMpmlojzZHkUUxAiK+UKn+hNQQ==",
+            "integrity": "sha512-bI2Z9zBGY2q5yMHoBvJ2a9iX3ZOAzJPm7Q8Yz6YeoUjU/Cvhmi2G4QyTNyPBqqXSgTjUxRg3L0xV45HvkNWWBw==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.21.2.tgz",
-            "version": "7.21.2"
+            "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@babel/helper-simple-access": {
             "dependencies": {
-                "@babel/types": "^7.20.2"
+                "@babel/types": "^7.21.5"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-+0woI/WPq59IrqDYbVGfshjT5Dmk/nnbdpcF8SnMhhXObpTq2KNBdLFRFrkVdbDOyUmHBCxzm5FHV1rACIkIbA==",
+            "integrity": "sha512-ENPDAMC1wAjR0uaCUwliBdiSl1KBJAVnMTzXqi64c2MG8MPR6ii4qf7bSXDqSFbr4W6W028/rf5ivoHop5/mkg==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-simple-access/-/helper-simple-access-7.20.2.tgz",
-            "version": "7.20.2"
+            "resolved": "https://registry.npmjs.org/@babel/helper-simple-access/-/helper-simple-access-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@babel/helper-split-export-declaration": {
             "dependencies": {
                 "@babel/types": "^7.18.6"
             },
             "engines": {
                 "node": ">=6.9.0"
@@ -6336,18 +6336,18 @@
             "resolved": "https://registry.npmjs.org/@babel/helper-split-export-declaration/-/helper-split-export-declaration-7.18.6.tgz",
             "version": "7.18.6"
         },
         "node_modules/@babel/helper-string-parser": {
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-nHtDoQcuqFmwYNYPz3Rah5ph2p8PFeFCsZk9A/48dPc/rGocJ5J3hAAZ7pb76VWX3fZKu+uEr/FhH5jLx7umrw==",
+            "integrity": "sha512-5pTUx3hAJaZIdW99sJ6ZUUgWq/Y+Hja7TowEnLNMm1VivRgZQL3vpBY3qUACVsvw+yQU6+YgfBVmcbLaZtrA1w==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-string-parser/-/helper-string-parser-7.19.4.tgz",
-            "version": "7.19.4"
+            "resolved": "https://registry.npmjs.org/@babel/helper-string-parser/-/helper-string-parser-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@babel/helper-validator-identifier": {
             "engines": {
                 "node": ">=6.9.0"
             },
             "integrity": "sha512-awrNfaMtnHUr653GgGEs++LlAvW6w+DcPrOliSMXWCKo597CwL5Acf/wWdNkf/tfEQE3mjkeD1YOVZOUV/od1w==",
             "resolved": "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.19.1.tgz",
@@ -6360,24 +6360,24 @@
             "integrity": "sha512-rmL/B8/f0mKS2baE9ZpyTcTavvEuWhTTW8amjzXNvYG4AwBsqTLikfXsEofsJEfKHf+HQVQbFOHy6o+4cnC/fQ==",
             "resolved": "https://registry.npmjs.org/@babel/helper-validator-option/-/helper-validator-option-7.21.0.tgz",
             "version": "7.21.0"
         },
         "node_modules/@babel/helpers": {
             "dependencies": {
                 "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.0",
-                "@babel/types": "^7.21.0"
+                "@babel/traverse": "^7.21.5",
+                "@babel/types": "^7.21.5"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-XXve0CBtOW0pd7MRzzmoyuSj0e3SEzj8pgyFxnTT1NJZL38BD1MK7yYrm8yefRPIDvNNe14xR4FdbHwpInD4rA==",
+            "integrity": "sha512-BSY+JSlHxOmGsPTydUkPf1MdMQ3M81x5xGCOVgWM3G8XH77sJ292Y2oqcp0CbbgxhqBuI46iUz1tT7hqP7EfgA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.21.0.tgz",
-            "version": "7.21.0"
+            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@babel/highlight": {
             "dependencies": {
                 "@babel/helper-validator-identifier": "^7.18.6",
                 "chalk": "^2.0.0",
                 "js-tokens": "^4.0.0"
             },
@@ -6391,18 +6391,18 @@
         "node_modules/@babel/parser": {
             "bin": {
                 "parser": "bin/babel-parser.js"
             },
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-alVJj7k7zIxqBZ7BTRhz0IqJFxW1VJbm6N8JbcYhQ186df9ZBPbZBmWSqAMXwHGsCJdYks7z/voa3ibiS5bCIw==",
+            "integrity": "sha512-6zavDGdzG3gUqAdWvlLFfk+36RilI+Pwyuuh7HItyeScCWP3k6i8vKclAQ0bM/0y/Kz/xiwvxhMv9MgTJP5gmA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.21.8.tgz",
+            "version": "7.21.8"
         },
         "node_modules/@babel/template": {
             "dependencies": {
                 "@babel/code-frame": "^7.18.6",
                 "@babel/parser": "^7.20.7",
                 "@babel/types": "^7.20.7"
             },
@@ -6413,45 +6413,45 @@
             "peer": true,
             "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.20.7.tgz",
             "version": "7.20.7"
         },
         "node_modules/@babel/traverse": {
             "dependencies": {
                 "@babel/code-frame": "^7.21.4",
-                "@babel/generator": "^7.21.4",
-                "@babel/helper-environment-visitor": "^7.18.9",
+                "@babel/generator": "^7.21.5",
+                "@babel/helper-environment-visitor": "^7.21.5",
                 "@babel/helper-function-name": "^7.21.0",
                 "@babel/helper-hoist-variables": "^7.18.6",
                 "@babel/helper-split-export-declaration": "^7.18.6",
-                "@babel/parser": "^7.21.4",
-                "@babel/types": "^7.21.4",
+                "@babel/parser": "^7.21.5",
+                "@babel/types": "^7.21.5",
                 "debug": "^4.1.0",
                 "globals": "^11.1.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-eyKrRHKdyZxqDm+fV1iqL9UAHMoIg0nDaGqfIOd8rKH17m5snv7Gn4qgjBoFfLz9APvjFU/ICT00NVCv1Epp8Q==",
+            "integrity": "sha512-AhQoI3YjWi6u/y/ntv7k48mcrCXmus0t79J9qPNlk/lAsFlCiJ047RmbfMOawySTHtywXhbXgpx/8nXMYd+oFw==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@babel/types": {
             "dependencies": {
-                "@babel/helper-string-parser": "^7.19.4",
+                "@babel/helper-string-parser": "^7.21.5",
                 "@babel/helper-validator-identifier": "^7.19.1",
                 "to-fast-properties": "^2.0.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-rU2oY501qDxE8Pyo7i/Orqma4ziCOrby0/9mvbDUGEfvZjb279Nk9k19e2fiCxHbRRpY2ZyrgW1eq22mvmOIzA==",
+            "integrity": "sha512-m4AfNvVF2mVC/F7fDEdH2El3HzUg9It/XsCxZiOTTA3m3qYfcSVSbTfM6Q9xG+hYDniZssYhlXKKUMD5m8tF4Q==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.21.4.tgz",
-            "version": "7.21.4"
+            "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.21.5.tgz",
+            "version": "7.21.5"
         },
         "node_modules/@colors/colors": {
             "engines": {
                 "node": ">=0.1.90"
             },
             "integrity": "sha512-ooWCrlZP11i8GImSjTHYHLkvFDP48nS4+204nGb1RiX/WXYHmJA2III9/e2DWVabCESdW7hBAEzHRqUn9OUVvQ==",
             "resolved": "https://registry.npmjs.org/@colors/colors/-/colors-1.5.0.tgz",
@@ -6751,17 +6751,17 @@
             "version": "3.4.35"
         },
         "node_modules/@types/connect-history-api-fallback": {
             "dependencies": {
                 "@types/express-serve-static-core": "*",
                 "@types/node": "*"
             },
-            "integrity": "sha512-h8QJa8xSb1WD4fpKBDcATDNGXghFj6/3GRWG6dhmRcu0RX1Ubasur2Uvx5aeEwlf0MwblEC2bMzzMQntxnw/Cw==",
-            "resolved": "https://registry.npmjs.org/@types/connect-history-api-fallback/-/connect-history-api-fallback-1.3.5.tgz",
-            "version": "1.3.5"
+            "integrity": "sha512-4x5FkPpLipqwthjPsF7ZRbOv3uoLUFkTA9G9v583qi4pACvq0uTELrB8OLUzPWUI4IJIyvM85vzkV1nyiI2Lig==",
+            "resolved": "https://registry.npmjs.org/@types/connect-history-api-fallback/-/connect-history-api-fallback-1.5.0.tgz",
+            "version": "1.5.0"
         },
         "node_modules/@types/eslint": {
             "dependencies": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
             "integrity": "sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==",
@@ -6774,17 +6774,17 @@
                 "@types/estree": "*"
             },
             "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
             "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
             "version": "3.7.4"
         },
         "node_modules/@types/estree": {
-            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
-            "version": "0.0.51"
+            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
+            "version": "1.0.1"
         },
         "node_modules/@types/express": {
             "dependencies": {
                 "@types/body-parser": "*",
                 "@types/express-serve-static-core": "^4.17.33",
                 "@types/qs": "*",
                 "@types/serve-static": "*"
@@ -6793,52 +6793,53 @@
             "resolved": "https://registry.npmjs.org/@types/express/-/express-4.17.17.tgz",
             "version": "4.17.17"
         },
         "node_modules/@types/express-serve-static-core": {
             "dependencies": {
                 "@types/node": "*",
                 "@types/qs": "*",
-                "@types/range-parser": "*"
+                "@types/range-parser": "*",
+                "@types/send": "*"
             },
-            "integrity": "sha512-TPBqmR/HRYI3eC2E5hmiivIzv+bidAfXofM+sbonAGvyDhySGw9/PQZFt2BLOrjUUR++4eJVpx6KnLQK1Fk9tA==",
-            "resolved": "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.33.tgz",
-            "version": "4.17.33"
+            "integrity": "sha512-fvr49XlCGoUj2Pp730AItckfjat4WNb0lb3kfrLWffd+RLeoGAMsq7UOy04PAPtoL01uKwcp6u8nhzpgpDYr3w==",
+            "resolved": "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.34.tgz",
+            "version": "4.17.34"
         },
         "node_modules/@types/html-minifier-terser": {
             "integrity": "sha512-oh/6byDPnL1zeNXFrDXFLyZjkr1MsBG667IM792caf1L2UPOOMf65NFzjUH/ltyfwjAGfs1rsX1eftK0jC/KIg==",
             "resolved": "https://registry.npmjs.org/@types/html-minifier-terser/-/html-minifier-terser-6.1.0.tgz",
             "version": "6.1.0"
         },
         "node_modules/@types/http-proxy": {
             "dependencies": {
                 "@types/node": "*"
             },
-            "integrity": "sha512-Qs5aULi+zV1bwKAg5z1PWnDXWmsn+LxIvUGv6E2+OOMYhclZMO+OXd9pYVf2gLykf2I7IV2u7oTHwChPNsvJ7g==",
-            "resolved": "https://registry.npmjs.org/@types/http-proxy/-/http-proxy-1.17.10.tgz",
-            "version": "1.17.10"
+            "integrity": "sha512-HC8G7c1WmaF2ekqpnFq626xd3Zz0uvaqFmBJNRZCGEZCXkvSdJoNFn/8Ygbd9fKNQj8UzLdCETaI0UWPAjK7IA==",
+            "resolved": "https://registry.npmjs.org/@types/http-proxy/-/http-proxy-1.17.11.tgz",
+            "version": "1.17.11"
         },
         "node_modules/@types/json-schema": {
             "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
             "version": "7.0.11"
         },
         "node_modules/@types/mime": {
-            "integrity": "sha512-Y4XFY5VJAuw0FgAqPNd6NNoV44jbq9Bz2L7Rh/J6jLTiHBSBJa9fxqQIvkIld4GsoDOcCbvzOUAbLPsSKKg+uA==",
-            "resolved": "https://registry.npmjs.org/@types/mime/-/mime-3.0.1.tgz",
-            "version": "3.0.1"
+            "integrity": "sha512-YATxVxgRqNH6nHEIsvg6k2Boc1JHI9ZbH5iWFFv/MTkchz3b1ieGDa5T0a9RznNdI0KhVbdbWSN+KWWrQZRxTw==",
+            "resolved": "https://registry.npmjs.org/@types/mime/-/mime-1.3.2.tgz",
+            "version": "1.3.2"
         },
         "node_modules/@types/minimist": {
             "integrity": "sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==",
             "resolved": "https://registry.npmjs.org/@types/minimist/-/minimist-1.2.2.tgz",
             "version": "1.2.2"
         },
         "node_modules/@types/node": {
-            "integrity": "sha512-E5Kwq2n4SbMzQOn6wnmBjuK9ouqlURrcZDVfbo9ftDDTFt3nk7ZKK4GMOzoYgnpQJKcxwQw+lGaBvvlMo0qN/Q==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.15.11.tgz",
-            "version": "18.15.11"
+            "integrity": "sha512-O+z53uwx64xY7D6roOi4+jApDGFg0qn6WHcxe5QeqjMaTezBO/mxdfFXIVAVVyNWKx84OmPB3L8kbVYOTeN34A==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz",
+            "version": "20.1.0"
         },
         "node_modules/@types/normalize-package-data": {
             "integrity": "sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==",
             "resolved": "https://registry.npmjs.org/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz",
             "version": "2.4.1"
         },
         "node_modules/@types/parse-json": {
@@ -6857,14 +6858,23 @@
             "version": "1.2.4"
         },
         "node_modules/@types/retry": {
             "integrity": "sha512-wWKOClTTiizcZhXnPY4wikVAwmdYHp8q6DmC+EJUzAMsycb7HB32Kh9RN4+0gExjmPmZSAQjgURXIGATPegAvA==",
             "resolved": "https://registry.npmjs.org/@types/retry/-/retry-0.12.0.tgz",
             "version": "0.12.0"
         },
+        "node_modules/@types/send": {
+            "dependencies": {
+                "@types/mime": "^1",
+                "@types/node": "*"
+            },
+            "integrity": "sha512-Cwo8LE/0rnvX7kIIa3QHCkcuF21c05Ayb0ZfxPiv0W8VRiZiNW/WuRupHKpqqGVGf7SUA44QSOUKaEd9lIrd/Q==",
+            "resolved": "https://registry.npmjs.org/@types/send/-/send-0.17.1.tgz",
+            "version": "0.17.1"
+        },
         "node_modules/@types/serve-index": {
             "dependencies": {
                 "@types/express": "*"
             },
             "integrity": "sha512-d/Hs3nWDxNL2xAczmOVZNj92YZCS6RGxfBPjKzuu/XirCgXdpKEb88dYNbrYGint6IVWLNP+yonwVAuRC0T2Dg==",
             "resolved": "https://registry.npmjs.org/@types/serve-index/-/serve-index-1.9.1.tgz",
             "version": "1.9.1"
@@ -7110,17 +7120,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-            "version": "7.4.0"
+            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+            "version": "7.5.0"
         },
         "node_modules/@vue/cli-shared-utils/node_modules/supports-color": {
             "dependencies": {
                 "has-flag": "^4.0.0"
             },
             "engines": {
                 "node": ">=8"
@@ -7225,142 +7235,142 @@
         "node_modules/@vue/web-component-wrapper": {
             "integrity": "sha512-Iu8Tbg3f+emIIMmI2ycSI8QcEuAUgPTgHwesDU1eKMLE4YC/c/sFbGc70QgMq31ijRftV0R7vCm9co6rldCeOA==",
             "resolved": "https://registry.npmjs.org/@vue/web-component-wrapper/-/web-component-wrapper-1.3.0.tgz",
             "version": "1.3.0"
         },
         "node_modules/@webassemblyjs/ast": {
             "dependencies": {
-                "@webassemblyjs/helper-numbers": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1"
+                "@webassemblyjs/helper-numbers": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
             },
-            "integrity": "sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/floating-point-hex-parser": {
-            "integrity": "sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-api-error": {
-            "integrity": "sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-buffer": {
-            "integrity": "sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-numbers": {
             "dependencies": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
-            "integrity": "sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-wasm-bytecode": {
-            "integrity": "sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-wasm-section": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1"
-            },
-            "integrity": "sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz",
-            "version": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5"
+            },
+            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/ieee754": {
             "dependencies": {
                 "@xtuc/ieee754": "^1.2.0"
             },
-            "integrity": "sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/leb128": {
             "dependencies": {
                 "@xtuc/long": "4.2.2"
             },
-            "integrity": "sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/utf8": {
-            "integrity": "sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-edit": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/helper-wasm-section": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-opt": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
-                "@webassemblyjs/wast-printer": "1.11.1"
-            },
-            "integrity": "sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz",
-            "version": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/helper-wasm-section": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-opt": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5",
+                "@webassemblyjs/wast-printer": "1.11.5"
+            },
+            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-gen": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
-            },
-            "integrity": "sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz",
-            "version": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
+            },
+            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-opt": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1"
-            },
-            "integrity": "sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz",
-            "version": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5"
+            },
+            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-parser": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
-            },
-            "integrity": "sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz",
-            "version": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
+            },
+            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wast-printer": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/ast": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
-            "integrity": "sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@xtuc/ieee754": {
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/@xtuc/long": {
@@ -7910,17 +7920,17 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-lZim4iUHhGcy5p+Ri/G7m84hJwncj+Kz7S5aD4hoQfslKZJgt0tHc/hafVbqHC5bbhHb+mrW2JOUHkI5KH7toQ==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001477.tgz",
-            "version": "1.0.30001477"
+            "integrity": "sha512-uv7/gXuHi10Whlj0pp5q/tsK/32J2QSqVRKQhs2j8VsDCjgyruAh/eEXHF822VqO9yT6iZKw3nRwZRSPBE9OQg==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001486.tgz",
+            "version": "1.0.30001486"
         },
         "node_modules/case-sensitive-paths-webpack-plugin": {
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-roIFONhcxog0JSSWbvVAh3OocukmSgpqOH6YpMkCvav/ySIV3JKg4Dc8vYtQjYi/UxpNE36r/9v+VqTQqgkYmw==",
             "resolved": "https://registry.npmjs.org/case-sensitive-paths-webpack-plugin/-/case-sensitive-paths-webpack-plugin-2.4.0.tgz",
@@ -8143,17 +8153,17 @@
         "node_modules/cli-spinners": {
             "engines": {
                 "node": ">=6"
             },
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
-            "integrity": "sha512-/eG5sJcvEIwxcdYM86k5tPwn0MUzkX5YY3eImTGpJOZgVe4SdTMY14vQpcxgBzJ0wXwAYrS8E+c3uHeK4JNyzQ==",
-            "resolved": "https://registry.npmjs.org/cli-spinners/-/cli-spinners-2.8.0.tgz",
-            "version": "2.8.0"
+            "integrity": "sha512-4/aL9X3Wh0yiMQlE+eeRhWP6vclO3QRtw1JHKIT0FFUs5FjpFmESqtMvYZ0+lbzBw900b95mS0hohy+qn2VK/g==",
+            "resolved": "https://registry.npmjs.org/cli-spinners/-/cli-spinners-2.9.0.tgz",
+            "version": "2.9.0"
         },
         "node_modules/clipboardy": {
             "dependencies": {
                 "arch": "^2.1.1",
                 "execa": "^1.0.0",
                 "is-wsl": "^2.1.1"
             },
@@ -8275,17 +8285,17 @@
         },
         "node_modules/colord": {
             "integrity": "sha512-jeC1axXpnb0/2nn/Y1LPuLdgXBLH7aDcHu4KEKfqw3CUhX7ZpfBSlPKyqXE6btIgEzfWtrX3/tyBCaCvXvMkOw==",
             "resolved": "https://registry.npmjs.org/colord/-/colord-2.9.3.tgz",
             "version": "2.9.3"
         },
         "node_modules/colorette": {
-            "integrity": "sha512-3tlv/dIP7FWvj3BsbHrGLJ6l/oKh1O3TcgBqMn+yyCagOxc23fyzDS6HypQbgxWbkpDnf52p1LuR4eWDQ/K9WQ==",
-            "resolved": "https://registry.npmjs.org/colorette/-/colorette-2.0.19.tgz",
-            "version": "2.0.19"
+            "integrity": "sha512-IfEDxwoWIjkeXL1eXcDiow4UbKjhLdq6/EuSVR9GMN7KVH3r9gQ83e73hsz1Nd1T3ijd5xv1wcWRYO+D6kCI2w==",
+            "resolved": "https://registry.npmjs.org/colorette/-/colorette-2.0.20.tgz",
+            "version": "2.0.20"
         },
         "node_modules/colorspace": {
             "dependencies": {
                 "color": "^3.1.3",
                 "text-hex": "1.0.x"
             },
             "integrity": "sha512-BgvKJiuVu1igBUF2kEjRCZXol6wiiGbY5ipL/oVPwm0BL9sIpMIzM8IK7vwuxIIzOXMV3Ey5w+vxhm0rR/TN8w==",
@@ -8569,17 +8579,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-            "version": "7.4.0"
+            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+            "version": "7.5.0"
         },
         "node_modules/css-loader/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/css-minimizer-webpack-plugin": {
@@ -8649,28 +8659,28 @@
             "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/css-minimizer-webpack-plugin/node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.9",
-                "ajv": "^8.8.0",
+                "ajv": "^8.9.0",
                 "ajv-formats": "^2.1.1",
-                "ajv-keywords": "^5.0.0"
+                "ajv-keywords": "^5.1.0"
             },
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-1edyXKgh6XnJsJSQ8mKWXnN/BVaIbFMLpouRUrXgVq7WYne5kw3MW7UPhO44uRXQSIpTSXoJbmrR2X0w9kUTyg==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
-            "version": "4.0.0"
+            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
+            "version": "4.0.1"
         },
         "node_modules/css-select": {
             "dependencies": {
                 "boolbase": "^1.0.0",
                 "css-what": "^6.0.1",
                 "domhandler": "^4.3.1",
                 "domutils": "^2.8.0",
@@ -9058,17 +9068,17 @@
         "node_modules/dns-packet": {
             "dependencies": {
                 "@leichtgewicht/ip-codec": "^2.0.1"
             },
             "engines": {
                 "node": ">=6"
             },
-            "integrity": "sha512-USawdAUzRkV6xrqTjiAEp6M9YagZEzWcSUaZTcIFAiyQWW1SoI6KyId8y2+/71wbgHKQAKd+iupLv4YvEwYWvA==",
-            "resolved": "https://registry.npmjs.org/dns-packet/-/dns-packet-5.5.0.tgz",
-            "version": "5.5.0"
+            "integrity": "sha512-rza3UH1LwdHh9qyPXp8lkwpjSNk/AMD3dPytUoRoqnypDUhY0xvbdmVhWOfxO68frEfV9BU8V12Ez7ZsHGZpCQ==",
+            "resolved": "https://registry.npmjs.org/dns-packet/-/dns-packet-5.6.0.tgz",
+            "version": "5.6.0"
         },
         "node_modules/dom-converter": {
             "dependencies": {
                 "utila": "~0.4"
             },
             "integrity": "sha512-gd3ypIPfOMr9h5jIKq8E3sHOTCjeirnl0WK5ZdS1AW0Odt0b1PaWaHdJ4Qk4klv+YB9aJBS7mESXjFoDQPu6DA==",
             "resolved": "https://registry.npmjs.org/dom-converter/-/dom-converter-0.2.0.tgz",
@@ -9162,17 +9172,17 @@
         },
         "node_modules/ee-first": {
             "integrity": "sha512-WMwm9LhRUo+WUaRN+vRuETqG89IgZphVSNkdFgeb6sS/E4OrDIN7t48CAewSHXc6C8lefD8KKfr5vY61brQlow==",
             "resolved": "https://registry.npmjs.org/ee-first/-/ee-first-1.1.1.tgz",
             "version": "1.1.1"
         },
         "node_modules/electron-to-chromium": {
-            "integrity": "sha512-UTkCbNTAcGXABmEnQrGcW4m3cG6fcyBfD4KDF0iyEAlbrGZiY9dmslyDAGOD1Kr5biN2F743Y30aRCOtau35Vw==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.357.tgz",
-            "version": "1.4.357"
+            "integrity": "sha512-L9zlje9bIw0h+CwPQumiuVlfMcV4boxRjFIWDcLfFqTZNbkwOExBzfmswytHawObQX4OUhtNv8gIiB21kOurIg==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.385.tgz",
+            "version": "1.4.385"
         },
         "node_modules/emoji-regex": {
             "integrity": "sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz",
             "version": "8.0.0"
         },
         "node_modules/emojis-list": {
@@ -9208,17 +9218,17 @@
             "dependencies": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-QHTXI/sZQmko1cbDoNAa3mJ5qhWUUNAq3vR0/YiD379fWQrcfuoX1+HW2S0MTt7XmoPLapdaDKUtelUSPic7hQ==",
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.12.0.tgz",
-            "version": "5.12.0"
+            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
+            "version": "5.13.0"
         },
         "node_modules/entities": {
             "funding": {
                 "url": "https://github.com/fb55/entities?sponsor=1"
             },
             "integrity": "sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==",
             "resolved": "https://registry.npmjs.org/entities/-/entities-2.2.0.tgz",
@@ -9237,17 +9247,17 @@
                 "stackframe": "^1.3.4"
             },
             "integrity": "sha512-Sk5V6wVazPhq5MhpO+AUxJn5x7XSXGl1R93Vn7i+zS15KDVxQijejNCrz8340/2bgLBjR9GtEG8ZVKONDjcqGQ==",
             "resolved": "https://registry.npmjs.org/error-stack-parser/-/error-stack-parser-2.1.4.tgz",
             "version": "2.1.4"
         },
         "node_modules/es-module-lexer": {
-            "integrity": "sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
-            "version": "0.9.3"
+            "integrity": "sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "node_modules/escalade": {
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==",
             "resolved": "https://registry.npmjs.org/escalade/-/escalade-3.1.1.tgz",
@@ -9964,20 +9974,20 @@
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/html-webpack-plugin"
             },
-            "integrity": "sha512-sy88PC2cRTVxvETRgUHFrL4No3UxvcH8G1NepGhqaTT+GXN2kTamqasot0inS5hXeg1cMbFDt27zzo9p35lZVw==",
+            "integrity": "sha512-cTUzZ1+NqjGEKjmVgZKLMdiFg3m9MdRXkZW2OEe69WYVi5ONLMmlnSZdXzGGMOq0C8jGDrL6EWyEDDUioHO/pA==",
             "peerDependencies": {
                 "webpack": "^5.20.0"
             },
-            "resolved": "https://registry.npmjs.org/html-webpack-plugin/-/html-webpack-plugin-5.5.0.tgz",
-            "version": "5.5.0"
+            "resolved": "https://registry.npmjs.org/html-webpack-plugin/-/html-webpack-plugin-5.5.1.tgz",
+            "version": "5.5.1"
         },
         "node_modules/htmlparser2": {
             "dependencies": {
                 "domelementtype": "^2.0.1",
                 "domhandler": "^4.0.0",
                 "domutils": "^2.5.2",
                 "entities": "^2.0.0"
@@ -10364,17 +10374,17 @@
             "dependencies": {
                 "@hapi/hoek": "^9.0.0",
                 "@hapi/topo": "^5.0.0",
                 "@sideway/address": "^4.1.3",
                 "@sideway/formula": "^3.0.1",
                 "@sideway/pinpoint": "^2.0.0"
             },
-            "integrity": "sha512-FariIi9j6QODKATGBrEX7HZcja8Bsh3rfdGYy/Sb65sGlZWK/QWesU1ghk7aJWDj95knjXlQfSmzFSPPkLVsfw==",
-            "resolved": "https://registry.npmjs.org/joi/-/joi-17.9.1.tgz",
-            "version": "17.9.1"
+            "integrity": "sha512-Itk/r+V4Dx0V3c7RLFdRh12IOjySm2/WGPMubBT92cQvRfYZhPM2W0hZlctjj72iES8jsRCwp7S/cRmWBnJ4nw==",
+            "resolved": "https://registry.npmjs.org/joi/-/joi-17.9.2.tgz",
+            "version": "17.9.2"
         },
         "node_modules/jquery": {
             "integrity": "sha512-v28EW9DWDFpzcD9O5iyJXg3R3+q+mET5JhnjJzQUZMHOv67bpSIHq81GEYpPNZHG+XXHsfSme3nxp/hndKEcsQ==",
             "peer": true,
             "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.6.4.tgz",
             "version": "3.6.4"
         },
@@ -10794,17 +10804,17 @@
         "node_modules/memfs": {
             "dependencies": {
                 "fs-monkey": "^1.0.3"
             },
             "engines": {
                 "node": ">= 4.0.0"
             },
-            "integrity": "sha512-yK6o8xVJlQerz57kvPROwTMgx5WtGwC2ZxDtOUsnGl49rHjYkfQoPNZPCKH73VdLE1BwBu/+Fx/NL8NYMUw2aA==",
-            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.0.tgz",
-            "version": "3.5.0"
+            "integrity": "sha512-UWbFJKvj5k+nETdteFndTpYxdeTMox/ULeqX5k/dpaQJCCFmj5EeKv3dBcyO2xmkRAx2vppRu5dVG7SOtsGOzA==",
+            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.1.tgz",
+            "version": "3.5.1"
         },
         "node_modules/merge-descriptors": {
             "integrity": "sha512-cCi6g3/Zr1iqQi6ySbseM1Xvooa98N0w31jzUYrXPX2xqObmFGHJ0tQ5u74H3mVh7wLouTseZyYIq39g8cNp1w==",
             "resolved": "https://registry.npmjs.org/merge-descriptors/-/merge-descriptors-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/merge-source-map": {
@@ -10945,28 +10955,28 @@
             "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/mini-css-extract-plugin/node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.9",
-                "ajv": "^8.8.0",
+                "ajv": "^8.9.0",
                 "ajv-formats": "^2.1.1",
-                "ajv-keywords": "^5.0.0"
+                "ajv-keywords": "^5.1.0"
             },
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-1edyXKgh6XnJsJSQ8mKWXnN/BVaIbFMLpouRUrXgVq7WYne5kw3MW7UPhO44uRXQSIpTSXoJbmrR2X0w9kUTyg==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
-            "version": "4.0.0"
+            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
+            "version": "4.0.1"
         },
         "node_modules/minimalistic-assert": {
             "integrity": "sha512-UtJcAD4yEaGtjPezWuO9wC4nwUnVH/8/Im3yEHQP4b67cXlD/Qr9hdITCU1xDbSEXg2XKNaP8jsReV7vQd00/A==",
             "resolved": "https://registry.npmjs.org/minimalistic-assert/-/minimalistic-assert-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/minimatch": {
@@ -11137,17 +11147,17 @@
         "node_modules/node-abi": {
             "dependencies": {
                 "semver": "^7.3.5"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-jAlSOFR1Bls963NmFwxeQkNTzqjUF0NThm8Le7eRIRGzFUVJuMOFZDLv5Y30W/Oaw+KEebEJLAigwO9gQHoEmw==",
-            "resolved": "https://registry.npmjs.org/node-abi/-/node-abi-3.35.0.tgz",
-            "version": "3.35.0"
+            "integrity": "sha512-zNy02qivjjRosswoYmPi8hIKJRr8MpQyeKT6qlcq/OnOgA3Rhoae+IYOqsM9V5+JnHWmxKnWOT2GxvtqdtOCXA==",
+            "resolved": "https://registry.npmjs.org/node-abi/-/node-abi-3.40.0.tgz",
+            "version": "3.40.0"
         },
         "node_modules/node-abi/node_modules/lru-cache": {
             "dependencies": {
                 "yallist": "^4.0.0"
             },
             "engines": {
                 "node": ">=10"
@@ -11162,17 +11172,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-            "version": "7.4.0"
+            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+            "version": "7.5.0"
         },
         "node_modules/node-abi/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/node-addon-api": {
@@ -11705,34 +11715,38 @@
             },
             "integrity": "sha512-CFjzYYAi4ThfiQvizrFQevTTXHtnCqWfe7x1AhgEscTz6ZbLbfoLRLPugTQyBth6f8ZERVUSyWHFD/7Wu4t1XQ==",
             "resolved": "https://registry.npmjs.org/debug/-/debug-3.2.7.tgz",
             "version": "3.2.7"
         },
         "node_modules/postcss": {
             "dependencies": {
-                "nanoid": "^3.3.4",
+                "nanoid": "^3.3.6",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
             "engines": {
                 "node": "^10 || ^12 || >=14"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/postcss/"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/postcss"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-tP7u/Sn/dVxK2NnruI4H9BG+x+Wxz6oeZ1cJ8P6G/PZY0IKk4k/63TDsQf2kQq3+qoJeLm2kIBUNlZe3zgb4Zg==",
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.21.tgz",
-            "version": "8.4.21"
+            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
+            "version": "8.4.23"
         },
         "node_modules/postcss-calc": {
             "dependencies": {
                 "postcss-selector-parser": "^6.0.9",
                 "postcss-value-parser": "^4.2.0"
             },
             "integrity": "sha512-SmWMSJmB8MRnnULldx0lQIyhSNvuDl9HfrZkaqqE/WHAhToYsAvDq+yAsA/kIyINDszOp3Rh0GFoNuH5Ypsm3Q==",
@@ -11856,17 +11870,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-            "version": "7.4.0"
+            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+            "version": "7.5.0"
         },
         "node_modules/postcss-loader/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/postcss-merge-longhand": {
@@ -12189,17 +12203,17 @@
             "dependencies": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
             "engines": {
                 "node": ">=4"
             },
-            "integrity": "sha512-zbARubNdogI9j7WY4nQJBiNqQf3sLS3wCP4WfOidu+p28LofJqDH1tcXypGrcmMHhDk2t9wGhCsYe/+szLTy1g==",
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.11.tgz",
-            "version": "6.0.11"
+            "integrity": "sha512-NdxGCAZdRrwVI1sy59+Wzrh+pMMHxapGnpfenDVlMEXoOcvt4pGE0JLK9YY2F5dLxcFYA/YbVQKhcGU+FtSYQg==",
+            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.12.tgz",
+            "version": "6.0.12"
         },
         "node_modules/postcss-svgo": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0",
                 "svgo": "^2.7.0"
             },
             "engines": {
@@ -12262,18 +12276,18 @@
             },
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "url": "https://github.com/prettier/prettier?sponsor=1"
             },
-            "integrity": "sha512-yPngTo3aXUUmyuTjeTUT75txrf+aMh9FiD7q9ZE/i6r0bPb22g4FsE6Y338PQX1bmfy08i9QQCB7/rcUAVntfw==",
+            "integrity": "sha512-tdN8qQGvNjw4CHbY+XXk0JgCXn9QiF21a55rBe5LJAU+kDyC4WQn4+awm2Xfk2lQMk5fKup9XgzTZtGkjBdP9Q==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/prettier/-/prettier-2.8.7.tgz",
-            "version": "2.8.7"
+            "resolved": "https://registry.npmjs.org/prettier/-/prettier-2.8.8.tgz",
+            "version": "2.8.8"
         },
         "node_modules/pretty-error": {
             "dependencies": {
                 "lodash": "^4.17.20",
                 "renderkid": "^3.0.0"
             },
             "integrity": "sha512-AoJ5YMAcXKYxKhuJGdcvse+Voc6v1RgnsR3nWcYU7q4t6z0Q6T86sv5Zq8VIRbOWWFpvdGE83LtdSMNd+6Y0xw==",
@@ -12698,34 +12712,34 @@
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-PDsN7BrVkNZK2+dj/dpKQAWZavbAQ87IXqVvw2+oEYI+GwlTWkvbQtL7F2cCNbMqJEYKPh1EcjSxsnqIb/kyaQ==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.61.0.tgz",
-            "version": "1.61.0"
+            "integrity": "sha512-NHpxIzN29MXvWiuswfc1W3I0N8SXBd8UR26WntmDlRYf0bSADnwnOjsyMZ3lMezSlArD33Vs3YFhp7dWvL770A==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.62.1.tgz",
+            "version": "1.62.1"
         },
         "node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.8",
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-Y5PQxS4ITlC+EahLuXaY86TXfR7Dc5lw294alXOq86JAHCihAIZfqv8nNCWvaEJvaC51uN9hbLGeV0cFBdH+Fw==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.1.tgz",
-            "version": "3.1.1"
+            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "node_modules/select-hose": {
             "integrity": "sha512-mEugaLK+YfkijB4fx0e6kImuJdCIt2LxCRcbEYPqRGCs4F2ogyfZU5IAZRdjCP8JPq2AtdNoC/Dux63d9Kiryg==",
             "resolved": "https://registry.npmjs.org/select-hose/-/select-hose-2.0.0.tgz",
             "version": "2.0.0"
         },
         "node_modules/selfsigned": {
@@ -12935,17 +12949,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-RgOxM8Mw+7Zus0+zcLEUn8+JfoLpj/huFTItQy2hsM4khuC1HYRDp0cU482Ewn/Fcy6bCjufD8vAj7voC66KQw==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.4.0.tgz",
-            "version": "7.4.0"
+            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+            "version": "7.5.0"
         },
         "node_modules/sharp/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/shebang-command": {
@@ -13363,50 +13377,50 @@
                 "acorn": "^8.5.0",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-HPa/FdTB9XGI2H1/keLFZHxl6WNvAI4YalHGtDQTlMnJcoqSab1UwL4l1hGEhs6/GmLHBZIg/YgB++jcbzoOEg==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.16.9.tgz",
-            "version": "5.16.9"
+            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
+            "version": "5.17.1"
         },
         "node_modules/terser-webpack-plugin": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
                 "serialize-javascript": "^6.0.1",
-                "terser": "^5.16.5"
+                "terser": "^5.16.8"
             },
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
+            "integrity": "sha512-WiHL3ElchZMsK27P8uIUh4604IgJyAW47LVXGbEoB21DbQcZ+OuMpGjVYnEUaqcWM6dO8uS2qUbA7LSCWqvsbg==",
             "peerDependencies": {
                 "webpack": "^5.1.0"
             },
             "peerDependenciesMeta": {
                 "@swc/core": {
                     "optional": true
                 },
                 "esbuild": {
                     "optional": true
                 },
                 "uglify-js": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
-            "version": "5.3.7"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.8.tgz",
+            "version": "5.3.8"
         },
         "node_modules/terser/node_modules/commander": {
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
         "node_modules/text-hex": {
@@ -13604,36 +13618,40 @@
             },
             "integrity": "sha512-pjy2bYhSsufwWlKwPc+l3cN7+wuJlK6uz0YdJEOlQDbl6jo/YlPi4mb8agUkVC8BF7V8NuzeyPNqRksA3hztKQ==",
             "resolved": "https://registry.npmjs.org/unpipe/-/unpipe-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/update-browserslist-db": {
             "bin": {
-                "browserslist-lint": "cli.js"
+                "update-browserslist-db": "cli.js"
             },
             "dependencies": {
                 "escalade": "^3.1.1",
                 "picocolors": "^1.0.0"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-OztqDenkfFkbSG+tRxBeAnCVPckDBcvibKd35yDONx6OU8N7sqgwc7rCbkJ/WcYtVRZ4ba68d6byhC21GFh7sQ==",
+            "integrity": "sha512-dCwEFf0/oT85M1fHBg4F0jtLwJrutGoHSQXCh7u4o2t1drG+c0a9Flnqww6XUKSfQMPpJBRjU8d4RXB09qtvaA==",
             "peerDependencies": {
                 "browserslist": ">= 4.21.0"
             },
-            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.10.tgz",
-            "version": "1.0.10"
+            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.11.tgz",
+            "version": "1.0.11"
         },
         "node_modules/uri-js": {
             "dependencies": {
                 "punycode": "^2.1.0"
             },
             "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
             "resolved": "https://registry.npmjs.org/uri-js/-/uri-js-4.4.1.tgz",
@@ -13687,30 +13705,30 @@
             "resolved": "https://registry.npmjs.org/vue-hot-reload-api/-/vue-hot-reload-api-2.3.4.tgz",
             "version": "2.3.4"
         },
         "node_modules/vue-loader": {
             "dependencies": {
                 "chalk": "^4.1.0",
                 "hash-sum": "^2.0.0",
-                "loader-utils": "^2.0.0"
+                "watchpack": "^2.4.0"
             },
-            "integrity": "sha512-/OOyugJnImKCkAKrAvdsWMuwoCqGxWT5USLsjohzWbMgOwpA5wQmzQiLMzZd7DjhIfunzAGIApTOgIylz/kwcg==",
+            "integrity": "sha512-zAjrT+TNWTpgRODxqDfzbDyvuTf5kCP9xmMk8aspQKuYNnTY2r0XK/bHu1DKLpSpk0I6fkQph5OLKB7HcRIPZw==",
             "peerDependencies": {
                 "webpack": "^4.1.0 || ^5.0.0-0"
             },
             "peerDependenciesMeta": {
                 "@vue/compiler-sfc": {
                     "optional": true
                 },
                 "vue": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/vue-loader/-/vue-loader-17.0.1.tgz",
-            "version": "17.0.1"
+            "resolved": "https://registry.npmjs.org/vue-loader/-/vue-loader-17.1.0.tgz",
+            "version": "17.1.0"
         },
         "node_modules/vue-loader/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "engines": {
                 "node": ">=8"
@@ -13757,27 +13775,14 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
             "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz",
             "version": "4.0.0"
         },
-        "node_modules/vue-loader/node_modules/loader-utils": {
-            "dependencies": {
-                "big.js": "^5.2.2",
-                "emojis-list": "^3.0.0",
-                "json5": "^2.1.2"
-            },
-            "engines": {
-                "node": ">=8.9.0"
-            },
-            "integrity": "sha512-xXqpXoINfFhgua9xiqD8fPFHgkoq1mmmpE92WlDbm9rNRd/EbRb+Gqf908T2DMfuHjjJlksiK2RbHVOdD/MqSw==",
-            "resolved": "https://registry.npmjs.org/loader-utils/-/loader-utils-2.0.4.tgz",
-            "version": "2.0.4"
-        },
         "node_modules/vue-loader/node_modules/supports-color": {
             "dependencies": {
                 "has-flag": "^4.0.0"
             },
             "engines": {
                 "node": ">=8"
             },
@@ -13848,53 +13853,53 @@
         },
         "node_modules/webpack": {
             "bin": {
                 "webpack": "bin/webpack.js"
             },
             "dependencies": {
                 "@types/eslint-scope": "^3.7.3",
-                "@types/estree": "^0.0.51",
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/wasm-edit": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
+                "@types/estree": "^1.0.0",
+                "@webassemblyjs/ast": "^1.11.5",
+                "@webassemblyjs/wasm-edit": "^1.11.5",
+                "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.10.0",
-                "es-module-lexer": "^0.9.0",
+                "enhanced-resolve": "^5.13.0",
+                "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.1.0",
+                "schema-utils": "^3.1.2",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.1.3",
+                "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-gT5DP72KInmE/3azEaQrISjTvLYlSM0j1Ezhht/KLVkrqtv10JoP/RXhwmX/frrutOPuSq3o5Vq0ehR/4Vmd1g==",
+            "integrity": "sha512-iGNA2fHhnDcV1bONdUu554eZx+XeldsaeQ8T67H6KKHl2nUSwX8Zm7cmzOA46ox/X1ARxf7Bjv8wQ/HsB5fxBg==",
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.78.0.tgz",
-            "version": "5.78.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.82.0.tgz",
+            "version": "5.82.0"
         },
         "node_modules/webpack-bundle-analyzer": {
             "bin": {
                 "webpack-bundle-analyzer": "lib/bin/analyzer.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "0.5.7",
@@ -14051,28 +14056,28 @@
             "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/webpack-dev-middleware/node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.9",
-                "ajv": "^8.8.0",
+                "ajv": "^8.9.0",
                 "ajv-formats": "^2.1.1",
-                "ajv-keywords": "^5.0.0"
+                "ajv-keywords": "^5.1.0"
             },
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-1edyXKgh6XnJsJSQ8mKWXnN/BVaIbFMLpouRUrXgVq7WYne5kw3MW7UPhO44uRXQSIpTSXoJbmrR2X0w9kUTyg==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
-            "version": "4.0.0"
+            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
+            "version": "4.0.1"
         },
         "node_modules/webpack-dev-server": {
             "bin": {
                 "webpack-dev-server": "bin/webpack-dev-server.js"
             },
             "dependencies": {
                 "@types/bonjour": "^3.5.9",
@@ -14109,28 +14114,28 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-5i6TrGBRxG4vnfDpB6qSQGfnB6skGBXNL5/542w2uRGLimX6qeE5BQMLrzIC3JYV/xlGOv+s+hTleI9AZKUQNw==",
+            "integrity": "sha512-HmNB5QeSl1KpulTBQ8UT4FPrByYyaLxpJoQ0+s7EvUrMc16m0ZS1sgb1XGqzmgCPk0c9y+aaXxn11tbLzuM7NQ==",
             "peerDependencies": {
                 "webpack": "^4.37.0 || ^5.0.0"
             },
             "peerDependenciesMeta": {
                 "webpack": {
                     "optional": true
                 },
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack-dev-server/-/webpack-dev-server-4.13.2.tgz",
-            "version": "4.13.2"
+            "resolved": "https://registry.npmjs.org/webpack-dev-server/-/webpack-dev-server-4.15.0.tgz",
+            "version": "4.15.0"
         },
         "node_modules/webpack-dev-server/node_modules/ajv": {
             "dependencies": {
                 "fast-deep-equal": "^3.1.1",
                 "json-schema-traverse": "^1.0.0",
                 "require-from-string": "^2.0.2",
                 "uri-js": "^4.2.2"
@@ -14166,28 +14171,28 @@
             "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/webpack-dev-server/node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.9",
-                "ajv": "^8.8.0",
+                "ajv": "^8.9.0",
                 "ajv-formats": "^2.1.1",
-                "ajv-keywords": "^5.0.0"
+                "ajv-keywords": "^5.1.0"
             },
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-1edyXKgh6XnJsJSQ8mKWXnN/BVaIbFMLpouRUrXgVq7WYne5kw3MW7UPhO44uRXQSIpTSXoJbmrR2X0w9kUTyg==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
-            "version": "4.0.0"
+            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
+            "version": "4.0.1"
         },
         "node_modules/webpack-dev-server/node_modules/ws": {
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-x9vcZYTrFPC7aSIbj7sRCYo7L/Xb8Iy+pW0ng0wt2vCJv7M9HOMy0UoN3rr+IFC7hb7vXoqS+P9ktyLLLhO+LA==",
             "peerDependencies": {
@@ -14273,17 +14278,17 @@
                 "isexe": "^2.0.0"
             },
             "integrity": "sha512-HxJdYWq1MTIQbJ3nw0cqssHoTNU267KlrDuGZ1WYlxDStUtKUhOaJmh112/TZmHxxUfuJqPXSOm7tDyas0OSIQ==",
             "resolved": "https://registry.npmjs.org/which/-/which-1.3.1.tgz",
             "version": "1.3.1"
         },
         "node_modules/wildcard": {
-            "integrity": "sha512-JcKqAHLPxcdb9KM49dufGXn2x3ssnfjbcaQdLlfZsL9rH9wgDQjUtDxbo8NE0F6SFvydeu1VhZe7hZuHsB2/pw==",
-            "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.0.tgz",
-            "version": "2.0.0"
+            "integrity": "sha512-CC1bOL87PIWSBhDcTrdeLo6eGT7mCFtrg0uIJtqJUFyK+eJnzl8A1niH56uu7KMa5XFrtiV+AQuHO3n7DsHnLQ==",
+            "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.1.tgz",
+            "version": "2.0.1"
         },
         "node_modules/winston": {
             "dependencies": {
                 "@colors/colors": "1.5.0",
                 "@dabh/diagnostics": "^2.0.2",
                 "async": "^3.2.3",
                 "is-stream": "^2.0.0",
```

### Comparing `gramex-1.89.2/gramex/apps/ui/setup.js` & `gramex-1.90.0/gramex/apps/ui/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootstrap5.scss` & `gramex-1.90.0/gramex/apps/ui/theme/bootstrap5.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cerulean.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cerulean.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cosmo.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cosmo.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/cyborg.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cyborg.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/darkly.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/darkly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/flatly.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/flatly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/journal.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/journal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/litera.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/litera.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/lumen.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lumen.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/lux.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lux.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/materia.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/materia.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/minty.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/minty.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/pulse.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/pulse.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/sandstone.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sandstone.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/simplex.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/simplex.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/sketchy.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sketchy.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/slate.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/slate.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/solar.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/solar.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/spacelab.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/spacelab.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/superhero.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/superhero.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/united.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/united.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/bootswatch/yeti.png` & `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/yeti.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/default.png` & `gramex-1.90.0/gramex/apps/ui/theme/default.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/index.html` & `gramex-1.90.0/gramex/apps/ui/theme/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/sample.html` & `gramex-1.90.0/gramex/apps/ui/theme/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/blue_voltage.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/blue_voltage.scss` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/boldstrap.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/boldstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/darkster.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/darkster.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/darkster.scss` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/darkster.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/fresca.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/fresca.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/greyson.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/greyson.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/greyson.scss` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/greyson.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/hello_kiddie.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/herbie.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/herbie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/hootstrap.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hootstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/lovey.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/lovey.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/monotony.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/monotony.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/poypull.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/poypull.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/poypull.scss` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/poypull.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/signal.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/signal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/signal.scss` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/signal.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes-guide/tequila.png` & `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/tequila.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/ui/theme/themes.json` & `gramex-1.90.0/gramex/apps/ui/theme/themes.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/.eslintrc.js` & `gramex-1.90.0/gramex/apps/uifactory/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/assets/data/input.json` & `gramex-1.90.0/gramex/apps/uifactory/assets/data/input.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/assets/img/arrows-move.svg` & `gramex-1.90.0/gramex/apps/uifactory/assets/img/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png` & `gramex-1.90.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/assets/img/trash.svg` & `gramex-1.90.0/gramex/apps/uifactory/assets/img/trash.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/create.html` & `gramex-1.90.0/gramex/apps/uifactory/create.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/edit.html` & `gramex-1.90.0/gramex/apps/uifactory/edit.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/field-actions.html` & `gramex-1.90.0/gramex/apps/uifactory/field-actions.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/form_builder.py` & `gramex-1.90.0/gramex/apps/uifactory/form_builder.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/gramex.yaml` & `gramex-1.90.0/gramex/apps/uifactory/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/index.html` & `gramex-1.90.0/gramex/apps/uifactory/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/js/README.md` & `gramex-1.90.0/gramex/apps/uifactory/js/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/js/fields.js` & `gramex-1.90.0/gramex/apps/uifactory/js/fields.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/js/fork-form.js` & `gramex-1.90.0/gramex/apps/uifactory/js/fork-form.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/js/index.js` & `gramex-1.90.0/gramex/apps/uifactory/js/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/js/script.js` & `gramex-1.90.0/gramex/apps/uifactory/js/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/js/utils.js` & `gramex-1.90.0/gramex/apps/uifactory/js/utils.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/js/viewform.js` & `gramex-1.90.0/gramex/apps/uifactory/js/viewform.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/modals/add-field.html` & `gramex-1.90.0/gramex/apps/uifactory/modals/add-field.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/modals/embed.html` & `gramex-1.90.0/gramex/apps/uifactory/modals/embed.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/modals/remove.html` & `gramex-1.90.0/gramex/apps/uifactory/modals/remove.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/modals/rename.html` & `gramex-1.90.0/gramex/apps/uifactory/modals/rename.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/modals/themes.html` & `gramex-1.90.0/gramex/apps/uifactory/modals/themes.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/package-lock.json` & `gramex-1.90.0/gramex/apps/uifactory/package-lock.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940972222222222%*

 * *Differences: {"'dependencies'": "{'bootstrap-icons': {'version': '1.10.5', 'resolved': "*

 * *                   "'https://registry.npmjs.org/bootstrap-icons/-/bootstrap-icons-1.10.5.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-oSX26F37V7QV7NCE53PPEL45d7EGXmBgHG3pDpZvcRaKVzWMqIRL9wcqJUyEha1esFtM3NJzvmxFXDxjJYD0jQ=='}}",*

 * * "'packages'": "{'node_modules/bootstrap-icons': {'version': '1.10.5', 'resolved': "*

 * *               "'https://registry.npmjs.org/bootstrap-icons/-/bootstrap-icons-1.10.5.tgz', "*

 * *     […]*

```diff
@@ -1,13 +1,13 @@
 {
     "dependencies": {
         "bootstrap-icons": {
-            "integrity": "sha512-eI3HyIUmpGKRiRv15FCZccV+2sreGE2NnmH8mtxV/nPOzQVu0sPEj8HhF1MwjJ31IhjF0rgMvtYOX5VqIzcb/A==",
-            "resolved": "https://registry.npmjs.org/bootstrap-icons/-/bootstrap-icons-1.10.4.tgz",
-            "version": "1.10.4"
+            "integrity": "sha512-oSX26F37V7QV7NCE53PPEL45d7EGXmBgHG3pDpZvcRaKVzWMqIRL9wcqJUyEha1esFtM3NJzvmxFXDxjJYD0jQ==",
+            "resolved": "https://registry.npmjs.org/bootstrap-icons/-/bootstrap-icons-1.10.5.tgz",
+            "version": "1.10.5"
         },
         "clipboard": {
             "integrity": "sha512-C+0bbOqkezLIsmWSvlsXS0Q0bmkugu7jcfMIACB+RDEntIzQIkdr148we28AfSloQLRdZlYL/QYyrq05j/3Faw==",
             "requires": {
                 "good-listener": "^1.2.2",
                 "select": "^1.1.2",
                 "tiny-emitter": "^2.0.0"
@@ -67,17 +67,27 @@
                 "jqueryui": "^1.11.1",
                 "uifactory": "^0.0.4"
             },
             "hasInstallScript": true,
             "name": "uifactory"
         },
         "node_modules/bootstrap-icons": {
-            "integrity": "sha512-eI3HyIUmpGKRiRv15FCZccV+2sreGE2NnmH8mtxV/nPOzQVu0sPEj8HhF1MwjJ31IhjF0rgMvtYOX5VqIzcb/A==",
-            "resolved": "https://registry.npmjs.org/bootstrap-icons/-/bootstrap-icons-1.10.4.tgz",
-            "version": "1.10.4"
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/twbs"
+                },
+                {
+                    "type": "opencollective",
+                    "url": "https://opencollective.com/bootstrap"
+                }
+            ],
+            "integrity": "sha512-oSX26F37V7QV7NCE53PPEL45d7EGXmBgHG3pDpZvcRaKVzWMqIRL9wcqJUyEha1esFtM3NJzvmxFXDxjJYD0jQ==",
+            "resolved": "https://registry.npmjs.org/bootstrap-icons/-/bootstrap-icons-1.10.5.tgz",
+            "version": "1.10.5"
         },
         "node_modules/clipboard": {
             "dependencies": {
                 "good-listener": "^1.2.2",
                 "select": "^1.1.2",
                 "tiny-emitter": "^2.0.0"
             },
```

### Comparing `gramex-1.89.2/gramex/apps/uifactory/popover-form.html` & `gramex-1.90.0/gramex/apps/uifactory/popover-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/sample.html` & `gramex-1.90.0/gramex/apps/uifactory/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/button/bs4-button.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/button/bs4-button.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/email/bs4-email.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/email/bs4-email.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/number/bs4-number.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/number/bs4-number.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/radio/bs4-radio.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/range/bs4-range.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/range/bs4-range.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/select/bs4-select.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/select/bs4-select.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/setup.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/text/bs4-text.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/text/bs4-text.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js` & `gramex-1.90.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/style.scss` & `gramex-1.90.0/gramex/apps/uifactory/style.scss`

 * *Files 15% similar despite different names*

```diff
@@ -82,12 +82,13 @@
 #formTabContent form {
   pointer-events: none;
 }
 .edit-properties > * {
   padding: 0.5rem;
   display: inline-grid;
 }
+/* stylelint-disable selector-type-no-unknown */
 .form-fields > *:not(bs4-multiselect),
 .form-fields > *:not(.divider) {
   display: block;
   padding: 0.5rem;
 }
```

### Comparing `gramex-1.89.2/gramex/apps/uifactory/template-navbar-view-form.html` & `gramex-1.90.0/gramex/apps/uifactory/template-navbar-view-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/template-navbar.html` & `gramex-1.90.0/gramex/apps/uifactory/template-navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/uifactory/viewform.html` & `gramex-1.90.0/gramex/apps/uifactory/viewform.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/update/README.md` & `gramex-1.90.0/gramex/apps/update/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/update/gramex.yaml` & `gramex-1.90.0/gramex/apps/update/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/update/gramexupdate.py` & `gramex-1.90.0/gramex/apps/update/gramexupdate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/apps/update/index.html` & `gramex-1.90.0/gramex/apps/update/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/cache.py` & `gramex-1.90.0/gramex/cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/config.py` & `gramex-1.90.0/gramex/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-'''
-Manages YAML config files as layered configurations with imports.
-
-:class:PathConfig loads YAML files from a path::
-
-    pc = PathConfig('/path/to/file.yaml')
-
-This can be reloaded via the ``+`` operator. ``+pc`` reloads the YAML file
-(but only if it is newer than before.)
+'''Utilities to manage Gramex configurations.
 
-:class:ChainConfig chains multiple YAML files into a single config. For example
-this merges ``base.yaml`` and ``next.yaml`` in sequence::
+These utilities handle objects:
 
-    cc = ChainConfig()
-    cc['base'] = PathConfig('base.yaml')
-    cc['next'] = PathConfig('next.yaml')
-
-To get the merged file, use ``+cc``. This updates the PathConfig files and
-merges the YAMLs.
+- [gramex.config.walk][] walks through a data structure recursively
+- [gramex.config.merge][] merges two data structures recursively
+- [gramex.config.objectpath][] gets/sets a value in a nested data structure
+- [gramex.config.CustomJSONEncoder][] encodes objects with Pandas / Numpy objects as JSON
+- [gramex.config.CustomJSONDecoder][] decodes JSON converting ISO dates to datetime objects
+- [gramex.config.recursive_encode][] convert Unicode to UTF-8 encoded byte strings in-place
+- [gramex.config.prune_keys][] removes specified keys anywhere in a nested data structure
+- [gramex.config.used_kwargs][] splits kwargs into those used by method, and those that are not
+
+These classes manage YAML config files as layered configurations with imports.
+
+- [gramex.config.PathConfig][] loads YAML configs `PathConfig('/path/to/file.yaml')`
+- [gramex.config.ChainConfig][] chains multiple YAML files into a single config
+
+Some additional utilities are:
+
+- `gramex.config.app_log` is the default logger used by all of Gramex.
+  Use `gramex.config.app_log.error(...)` to log errors
+- `gramex.config.slug.filename(string)` converts a string to a valid filename,
+   replacing invalid characters with '-'
+- `gramex.config.slug.module(string)` converts a string to a valid Python module name,
+  replacing invalid characters with '_'
+- [gramex.config.locate][] loads a module from a string
+- [gramex.config.ioloop_running][] returns True if the Gramex is running, else False
 '''
 
 import os
 import re
 import csv
 import sys
 import yaml
@@ -73,25 +82,25 @@
     filename=lambda s: slugify(s, regex_pattern=r'[^!#$%&()+,-.0-9;<=>@A-Z\[\]^_`a-z{}~]'),
 )
 
 
 def walk(node):
     '''
     Bottom-up recursive walk through a data structure yielding a (key, value,
-    node) tuple for every entry. ``node[key] == value`` is true in every entry.
+    node) tuple for every entry. `node[key] == value` is true in every entry.
 
-    For example::
+    For example:
 
         >>> list(walk([{'x': 1}]))
         [
             ('x', 1, {'x': 1}),         # leaf:   key, value, node
             (0, {'x': 1}, [{'x': 1}])   # parent: index, value, node
         ]
 
-    Circular linkage can lead to a RuntimeError::
+    Circular linkage can lead to a RuntimeError.
 
         >>> x = {}
         >>> x['x'] = x
         >>> list(walk(x))
         ...
         RuntimeError: maximum recursion depth exceeded
     '''
@@ -109,22 +118,22 @@
 def merge(old, new, mode='overwrite', warn=None, _path=''):
     '''
     Update old dict with new dict recursively.
 
         >>> merge({'a': {'x': 1}}, {'a': {'y': 2}})
         {'a': {'x': 1, 'y': 2}}
 
-    If ``new`` is a list, convert into a dict with random keys.
+    If `new` is a list, convert into a dict with random keys.
 
-    If ``mode='overwrite'``, the old dict is overwritten (default).
-    If ``mode='setdefault'``, the old dict values are updated only if missing.
+    If `mode='overwrite'`, the old dict is overwritten (default).
+    If `mode='setdefault'`, the old dict values are updated only if missing.
 
-    ``warn=`` is an optional list of key paths. Any conflict on dictionaries
+    `warn=` is an optional list of key paths. Any conflict on dictionaries
     matching any of these paths is logged as a warning. For example,
-    ``warn=['url.*', 'watch.*']`` warns if any url: sub-key or watch: sub-key
+    `warn=['url.*', 'watch.*']` warns if any url: sub-key or watch: sub-key
     has a conflict.
     '''
     for key in new:
         if key in old and hasattr(old[key], 'items') and hasattr(new[key], 'items'):
             path_key = _path + ('.' if _path else '') + str(key)
             if warn is not None:
                 for pattern in warn:
@@ -133,25 +142,242 @@
                         break
             merge(old=old[key], new=new[key], mode=mode, warn=warn, _path=path_key)
         elif mode == 'overwrite' or key not in old:
             old[key] = deepcopy(new[key])
     return old
 
 
+def objectpath(node, keypath, default=None):
+    '''
+    Traverse down a dot-separated object path into dict items or object attrs.
+    For example, `objectpath(handler, 'request.headers.User-Agent')` returns
+    `handler.request.headers['User-Agent']`. Dictionary access is preferred.
+    Returns `None` if the path is not found.
+    '''
+    for key in keypath.split('.'):
+        if hasattr(node, '__getitem__'):
+            node = node.get(key)
+        else:
+            node = getattr(node, key, None)
+        if node is None:
+            return default
+    return node
+
+
+class CustomJSONEncoder(JSONEncoder):
+    '''
+    Encodes object to JSON, additionally converting datetime into ISO 8601 format
+    '''
+
+    def default(self, obj):
+        import numpy as np
+
+        # Detect Pandas objects without importing Pandas, which is slow
+        if hasattr(obj, 'to_json'):
+            fmt = 'index' if obj.__class__.__name__ == 'Series' else 'records'
+            # loads + to_json() is slow but reliable. Handles numpy objects, mixed types, etc.
+            return loads(obj.to_json(orient=fmt, date_format='iso'), object_pairs_hook=OrderedDict)
+        elif isinstance(obj, datetime.datetime):
+            # Use local timezone if no timezone is specified
+            if obj.tzinfo is None:
+                obj = obj.replace(tzinfo=dateutil.tz.tzlocal())
+            return obj.isoformat()
+        elif isinstance(obj, np.datetime64):
+            obj = obj.item()
+            if isinstance(obj, datetime.datetime) and obj.tzinfo is None:
+                obj = obj.replace(tzinfo=dateutil.tz.tzlocal())
+            return obj.isoformat()
+        elif isinstance(obj, np.integer):
+            return int(obj)
+        elif isinstance(obj, np.floating):
+            return float(obj)
+        elif isinstance(obj, np.ndarray):
+            return obj.tolist()
+        elif isinstance(obj, np.bool_):
+            return bool(obj)
+        elif isinstance(obj, np.bytes_):
+            return obj.decode('utf-8')
+        return super(CustomJSONEncoder, self).default(obj)
+
+
+class CustomJSONDecoder(JSONDecoder):
+    '''
+    Decodes JSON string, converting ISO 8601 datetime to datetime
+    '''
+
+    # Check if a string might be a datetime. Handles variants like:
+    # 2001-02-03T04:05:06Z
+    # 2001-02-03T04:05:06+000
+    # 2001-02-03T04:05:06.000+0000
+    re_datetimeval = re.compile(r'\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}')
+    re_datetimestr = re.compile(r'"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}')
+
+    def __init__(self, *args, **kwargs):
+        self.old_object_pairs_hook = kwargs.get('object_pairs_hook')
+        kwargs['object_pairs_hook'] = self.convert
+        super(CustomJSONDecoder, self).__init__(*args, **kwargs)
+
+    def decode(self, obj):
+        if self.re_datetimestr.match(obj):
+            return dateutil.parser.parse(obj[1:-1])
+        return super(CustomJSONDecoder, self).decode(obj)
+
+    def convert(self, obj):
+        for index, (key, val) in enumerate(obj):
+            if isinstance(val, str) and self.re_datetimeval.match(val):
+                obj[index] = (key, dateutil.parser.parse(val))
+        if callable(self.old_object_pairs_hook):
+            return self.old_object_pairs_hook(obj)
+        return dict(obj)
+
+
+def recursive_encode(data, encoding='utf-8'):
+    '''Convert Unicode to UTF-8 encoded byte strings in-place.'''
+    for key, value, node in walk(data):
+        if isinstance(key, str):
+            newkey = key.encode(encoding)
+            node[newkey] = node.pop(key)
+            key = newkey
+        if isinstance(value, str):
+            node[key] = value.encode(encoding)
+
+
+def prune_keys(conf, keys={}):
+    '''Returns a deep copy of a configuration removing specified keys.
+
+    `prune_keys(conf, {'comment'})` drops the "comment" key from any dict or sub-dict.
+    '''
+    if isinstance(conf, dict):
+        conf = AttrDict({k: prune_keys(v, keys) for k, v in conf.items() if k not in keys})
+    elif isinstance(conf, (list, tuple)):
+        conf = [prune_keys(v, keys) for v in conf]
+    return conf
+
+
+def used_kwargs(method, kwargs, ignore_keywords=False):
+    '''
+    Splits kwargs into those used by method, and those that are not.
+
+    Returns a tuple of (used, rest). *used* is a dict subset of kwargs with only
+    keys used by method. *rest* has the remaining kwargs keys.
+
+    If the method uses `**kwargs` (keywords), it uses all keys. To ignore this
+    and return only named arguments, use `ignore_keywords=True`.
+    '''
+    # In Pandas 1.5, DataFrame.to_csv and DataFrame.to_excel are wrapped with @deprecate_kwargs.
+    # We dive deeper to detect the actual keywords. __wrapped__ is provided by functools.wraps
+    # https://docs.python.org/3/library/functools.html
+    while hasattr(method, '__wrapped__'):
+        method = method.__wrapped__
+    argspec = inspect.getfullargspec(method)
+    # If method uses **kwargs, return all kwargs (unless you ignore **kwargs)
+    if argspec.varkw and not ignore_keywords:
+        used, rest = kwargs, {}
+    else:
+        # Split kwargs into 2 dicts -- used and rest
+        used, rest = {}, {}
+        for key, val in kwargs.items():
+            target = used if key in set(argspec.args) else rest
+            target[key] = val
+    return used, rest
+
+
+_valid_key_chars = string.ascii_letters + string.digits
+
+
+def random_string(size, chars=_valid_key_chars):
+    '''Return random string of length size using chars (which defaults to alphanumeric)'''
+    # B311:random random() is safe since it's for non-cryptographic use
+    return ''.join(choice(chars) for index in range(size))  # nosec B311
+
+
+class PathConfig(AttrDict):
+    '''
+    An `AttrDict` that is loaded from a path as a YAML file. For e.g.,
+    `conf = PathConfig(path)` loads the YAML file at `path` as an AttrDict.
+    `+conf` reloads the path if required.
+
+    `warn=` is an optional list of key paths. Any conflict on dictionaries
+    matching any of these paths is logged as a warning. For example,
+    `warn=['url.*', 'watch.*']` warns if any url: sub-key or watch: sub-key
+    has a conflict.
+
+    Like http://configure.readthedocs.org/ but supports imports not inheritance.
+    This lets us import YAML files in the middle of a YAML structure.
+
+        key:
+            import:
+                conf1: file1.yaml       # Import file1.yaml here
+                conf2: file2.yaml       # Import file2.yaml here
+
+    Each `PathConfig` object has an `__info__` attribute with the following
+    keys:
+
+    __info__.path
+        The path that this instance syncs with, stored as a `pathlib.Path`
+    __info__.warn
+        The keys to warn in case about in case of an import merge conflict
+    __info__.imports
+        A list of imported files, stored as an `AttrDict` with 2 attributes:
+
+        path
+            The path that was imported, stored as a `pathlib.Path`
+        stat
+            The `os.stat()` information about this file (or `None` if the
+            file is missing.)
+    '''
+
+    duplicate_warn = None
+
+    def __init__(self, path, warn=None):
+        super(PathConfig, self).__init__()
+        if warn is None:
+            warn = self.duplicate_warn
+        self.__info__ = AttrDict(path=Path(path), imports=[], warn=warn)
+        self.__pos__()
+
+    def __pos__(self):
+        '''+config reloads this config (if it has a path)'''
+        path = self.__info__.path
+
+        # We must reload the layer if nothing has been imported...
+        reload = not self.__info__.imports
+        # ... or if an imported file is deleted / updated
+        for imp in self.__info__.imports:
+            exists = imp.path.exists()
+            # If the path existed but has now been deleted, log it
+            if not exists and imp.stat is not None:
+                reload = True
+                app_log.debug(f'Config deleted: {imp.path}')
+                break
+            if exists and (
+                imp.path.stat().st_mtime > imp.stat.st_mtime
+                or imp.path.stat().st_size != imp.stat.st_size
+            ):
+                reload = True
+                app_log.info(f'Updated config: {imp.path}')
+                break
+        if reload:
+            self.clear()
+            self.update(_yaml_open(path))
+            self.__info__.imports = load_imports(self, source=path, warn=self.__info__.warn)
+        return self
+
+
 class ChainConfig(AttrDict):
     '''
     An AttrDict that manages multiple configurations as layers.
 
         >>> config = ChainConfig([
         ...     ('base', PathConfig('gramex.yaml')),
         ...     ('app1', PathConfig('app.yaml')),
         ...     ('app2', AttrDict())
         ... ])
 
-    Any dict-compatible values are allowed. ``+config`` returns the merged values.
+    Any dict-compatible values are allowed. `+config` returns the merged values.
     '''
 
     def __pos__(self):
         '''+config returns layers merged in order, removing null keys'''
         conf = AttrDict()
         for _name, config in self.items():
             if hasattr(config, '__pos__'):
@@ -203,14 +429,29 @@
 
     return variables
 
 
 variables = setup_variables()
 
 
+class ConfigYAMLLoader(SafeLoader):
+    '''
+    A YAML loader that loads a YAML file into an ordered AttrDict.
+
+        >>> attrdict = yaml.load(yaml_string, Loader=ConfigYAMLLoader)
+
+    If there are duplicate keys, this raises an error.
+    '''
+
+    def __init__(self, *args, **kwargs):
+        super(ConfigYAMLLoader, self).__init__(*args, **kwargs)
+        self.add_constructor('tag:yaml.org,2002:map', _from_yaml)
+        self.add_constructor('tag:yaml.org,2002:omap', _from_yaml)
+
+
 def _substitute_variable(val):
     '''
     If val contains a ${VAR} or $VAR and VAR is in the variables global,
     substitute it.
 
     Direct variables are substituted as-is. For example, $x will return
     variables['x'] without converting it to a string. Otherwise, treat it as a
@@ -253,23 +494,14 @@
             return {k: _calc_value(v, k) for k, v in val.items()}
     elif isinstance(val, (list, tuple)):
         return [_calc_value(v, key) for v in val]
     else:
         return _substitute_variable(val)
 
 
-_valid_key_chars = string.ascii_letters + string.digits
-
-
-def random_string(size, chars=_valid_key_chars):
-    '''Return random string of length size using chars (which defaults to alphanumeric)'''
-    # B311:random random() is safe since it's for non-cryptographic use
-    return ''.join(choice(chars) for index in range(size))  # nosec B311
-
-
 RANDOM_KEY = r'$*'
 
 
 def _from_yaml(loader, node):
     '''
     Load mapping as AttrDict, preserving order. Raise error on duplicate keys
     '''
@@ -302,35 +534,20 @@
                 node.start_mark,
                 f'found duplicate key ({key})',
                 key_node.start_mark,
             )
         attrdict[key] = loader.construct_object(value_node, deep=False)
 
 
-class ConfigYAMLLoader(SafeLoader):
-    '''
-    A YAML loader that loads a YAML file into an ordered AttrDict. Usage::
-
-        >>> attrdict = yaml.load(yaml_string, Loader=ConfigYAMLLoader)
-
-    If there are duplicate keys, this raises an error.
-    '''
-
-    def __init__(self, *args, **kwargs):
-        super(ConfigYAMLLoader, self).__init__(*args, **kwargs)
-        self.add_constructor('tag:yaml.org,2002:map', _from_yaml)
-        self.add_constructor('tag:yaml.org,2002:omap', _from_yaml)
-
-
 def _yaml_open(path, default=AttrDict(), **kwargs):
     '''
     Load a YAML path.Path as AttrDict. Replace ${VAR} or $VAR with variables.
     Defines special variables $YAMLPATH as the absolute path of the YAML file,
     and $YAMLURL as the path relative to current directory. These can be
-    overridden via keyward arguments (e.g. ``YAMLURL=...``)
+    overridden via keyward arguments (e.g. `YAMLURL=...`)
 
     If key has " if ", include it only if the condition (eval-ed in Python) is
     true.
 
     If the path is missing, or YAML has a parse error, or the YAML is not a
     dict, returns the default value.
     '''
@@ -414,29 +631,29 @@
             # Substitute with variables in context, defaulting to ''
             node[key] = _substitute_variable(value)
     return result
 
 
 def _pathstat(path):
     '''
-    Return a path stat object, which has 2 attributes/keys: ``.path`` is the
-    same as the ``path`` parameter. ``stat`` is the result of ``os.stat``. If
-    path is missing, ``stat`` has ``st_mtime`` and ``st_size`` set to ``0``.
+    Return a path stat object, which has 2 attributes/keys: `.path` is the
+    same as the `path` parameter. `stat` is the result of `os.stat`. If
+    path is missing, `stat` has `st_mtime` and `st_size` set to `0`.
     '''
     # If path doesn't exist, create a dummy stat structure with
     # safe defaults (old mtime, 0 filesize, etc)
     stat = path.stat() if path.exists() else AttrDict(st_mtime=0, st_size=0)
     return AttrDict(path=path, stat=stat)
 
 
 def _add_ns(config, namespace, prefix):
     '''
     Given a YAML config (basically a dict), add prefix to specified namespaces.
 
-    For example::
+    For example:
 
         >>> _add_ns({'x': 1}, '*', 'a')
         {'a.x': 1}
         >>> _add_ns({'x': {'y': 1}}, ['*', 'x'], 'a')
         {'a.x': {'a.y': 1}}
     '''
     if not isinstance(namespace, list):
@@ -456,73 +673,73 @@
     return config
 
 
 def load_imports(config, source, warn=None):
     '''
     Post-process a config for imports.
 
-    ``config`` is the data to process. ``source`` is the path where it was
+    `config` is the data to process. `source` is the path where it was
     loaded from.
 
-    If ``config`` has an ``import:`` key, treat all values below that as YAML
-    files (specified relative to ``source``) and import them in sequence.
+    If `config` has an `import:` key, treat all values below that as YAML
+    files (specified relative to `source`) and import them in sequence.
 
     Return a list of imported paths as :func:_pathstat objects. (This includes
-    ``source``.)
+    `source`.)
 
-    For example, if the ``source`` is  ``base.yaml`` (which has the below
-    configuration) and is loaded into ``config``::
+    For example, if the `source` is  `base.yaml` (which has the below
+    configuration) and is loaded into `config`.
 
         app:
             port: 20
             start: true
         path: /
         import: update*.yaml    # Can be any glob, e.g. */gramex.yaml
 
-    ... and ``update.yaml`` looks like this::
+    ... and `update.yaml` looks like this.
 
         app:
             port: 30
             new: yes
 
-    ... then after this function is called, ``config`` looks like this::
+    ... then after this function is called, `config` looks like this.
 
         app:
             port: 20        # From base.yaml. NOT updated by update.yaml
             start: true     # From base.yaml
             new: yes        # From update.yaml
         path: /             # From base.yaml
 
-    The ``import:`` keys are deleted. The return value contains :func:_pathstat
-    values for ``base.yaml`` and ``update.yaml`` in that order.
+    The `import:` keys are deleted. The return value contains :func:_pathstat
+    values for `base.yaml` and `update.yaml` in that order.
 
-    Multiple ``import:`` values can be specified as a dictionary::
+    Multiple `import:` values can be specified as a dictionary.
 
         import:
             first-app: app1/*.yaml
             next-app: app2/*.yaml
 
-    To import sub-keys as namespaces, use::
+    To import sub-keys as namespaces
 
         import:
             app: {path: */gramex.yaml, namespace: 'url'}
 
-    This prefixes all keys under ``url:``. Here are more examples::
+    This prefixes all keys under `url:`. Here are more examples.
 
         namespace: True             # Add namespace to all top-level keys
         namespace: url              # Add namespace to url.*
         namespace: log.loggers      # Add namespace to log.loggers.*
         namespace: [True, url]      # Add namespace to top level keys and url.*
 
     By default, the prefix is the relative path of the imported YAML file
     (relative to the importer).
 
-    ``warn=`` is an optional list of key paths. Any conflict on dictionaries
+    `warn=` is an optional list of key paths. Any conflict on dictionaries
     matching any of these paths is logged as a warning. For example,
-    ``warn=['url.*', 'watch.*']`` warns if any url: sub-key or watch: sub-key
+    `warn=['url.*', 'watch.*']` warns if any url: sub-key or watch: sub-key
     has a conflict.
     '''
     imported_paths = [_pathstat(source)]
     root = source.absolute().parent
     for key, value, node in list(walk(config)):
         if isinstance(key, str) and key.startswith('import.merge'):
             # Strip the top level key(s) from import.merge values
@@ -566,227 +783,45 @@
                     imported_paths += load_imports(new_conf, source=abspath)
                     merge(old=node, new=new_conf, mode='setdefault', warn=warn)
             # Delete the import key
             del node[key]
     return imported_paths
 
 
-class PathConfig(AttrDict):
-    '''
-    An ``AttrDict`` that is loaded from a path as a YAML file. For e.g.,
-    ``conf = PathConfig(path)`` loads the YAML file at ``path`` as an AttrDict.
-    ``+conf`` reloads the path if required.
-
-    ``warn=`` is an optional list of key paths. Any conflict on dictionaries
-    matching any of these paths is logged as a warning. For example,
-    ``warn=['url.*', 'watch.*']`` warns if any url: sub-key or watch: sub-key
-    has a conflict.
-
-    Like http://configure.readthedocs.org/ but supports imports not inheritance.
-    This lets us import YAML files in the middle of a YAML structure::
-
-        key:
-            import:
-                conf1: file1.yaml       # Import file1.yaml here
-                conf2: file2.yaml       # Import file2.yaml here
-
-    Each ``PathConfig`` object has an ``__info__`` attribute with the following
-    keys:
-
-    __info__.path
-        The path that this instance syncs with, stored as a ``pathlib.Path``
-    __info__.warn
-        The keys to warn in case about in case of an import merge conflict
-    __info__.imports
-        A list of imported files, stored as an ``AttrDict`` with 2 attributes:
-
-        path
-            The path that was imported, stored as a ``pathlib.Path``
-        stat
-            The ``os.stat()`` information about this file (or ``None`` if the
-            file is missing.)
-    '''
-
-    duplicate_warn = None
-
-    def __init__(self, path, warn=None):
-        super(PathConfig, self).__init__()
-        if warn is None:
-            warn = self.duplicate_warn
-        self.__info__ = AttrDict(path=Path(path), imports=[], warn=warn)
-        self.__pos__()
-
-    def __pos__(self):
-        '''+config reloads this config (if it has a path)'''
-        path = self.__info__.path
-
-        # We must reload the layer if nothing has been imported...
-        reload = not self.__info__.imports
-        # ... or if an imported file is deleted / updated
-        for imp in self.__info__.imports:
-            exists = imp.path.exists()
-            # If the path existed but has now been deleted, log it
-            if not exists and imp.stat is not None:
-                reload = True
-                app_log.debug(f'Config deleted: {imp.path}')
-                break
-            if exists and (
-                imp.path.stat().st_mtime > imp.stat.st_mtime
-                or imp.path.stat().st_size != imp.stat.st_size
-            ):
-                reload = True
-                app_log.info(f'Updated config: {imp.path}')
-                break
-        if reload:
-            self.clear()
-            self.update(_yaml_open(path))
-            self.__info__.imports = load_imports(self, source=path, warn=self.__info__.warn)
-        return self
-
-
 def locate(path, modules=[], forceload=0):
     '''
     Locate an object by name or dotted path.
 
-    For example, ``locate('str')`` returns the ``str`` built-in.
-    ``locate('gramex.handlers.FileHandler')`` returns the class
-    ``gramex.handlers.FileHandler``.
-
-    ``modules`` is a list of modules to search for the path in first. So
-    ``locate('FileHandler', modules=[gramex.handlers])`` will return
-    ``gramex.handlers.FileHandler``.
+    For example, `locate('str')` returns the `str` built-in.
+    `locate('gramex.handlers.FileHandler')` returns the class
+    `gramex.handlers.FileHandler`.
+
+    `modules` is a list of modules to search for the path in first. So
+    `locate('FileHandler', modules=[gramex.handlers])` will return
+    `gramex.handlers.FileHandler`.
 
     If importing raises an Exception, log it and return None.
     '''
     try:
         for module_name in modules:
             module = _locate(module_name, forceload)
             if hasattr(module, path):
                 return getattr(module, path)
         return _locate(path, forceload)
     except ErrorDuringImport:
         app_log.exception(f'Exception when importing {path}')
         return None
 
 
-class CustomJSONEncoder(JSONEncoder):
-    '''
-    Encodes object to JSON, additionally converting datetime into ISO 8601 format
-    '''
-
-    def default(self, obj):
-        import numpy as np
-
-        if hasattr(obj, 'to_dict'):
-            # Slow but reliable. Handles conversion of numpy objects, mixed types, etc.
-            return loads(
-                obj.to_json(orient='records', date_format='iso'), object_pairs_hook=OrderedDict
-            )
-        elif isinstance(obj, datetime.datetime):
-            # Use local timezone if no timezone is specified
-            if obj.tzinfo is None:
-                obj = obj.replace(tzinfo=dateutil.tz.tzlocal())
-            return obj.isoformat()
-        elif isinstance(obj, np.datetime64):
-            obj = obj.item()
-            if isinstance(obj, datetime.datetime) and obj.tzinfo is None:
-                obj = obj.replace(tzinfo=dateutil.tz.tzlocal())
-            return obj.isoformat()
-        elif isinstance(obj, np.integer):
-            return int(obj)
-        elif isinstance(obj, np.floating):
-            return float(obj)
-        elif isinstance(obj, np.ndarray):
-            return obj.tolist()
-        elif isinstance(obj, np.bool_):
-            return bool(obj)
-        elif isinstance(obj, np.bytes_):
-            return obj.decode('utf-8')
-        return super(CustomJSONEncoder, self).default(obj)
-
-
-class CustomJSONDecoder(JSONDecoder):
-    '''
-    Decodes JSON string, converting ISO 8601 datetime to datetime
-    '''
-
-    # Check if a string might be a datetime. Handles variants like:
-    # 2001-02-03T04:05:06Z
-    # 2001-02-03T04:05:06+000
-    # 2001-02-03T04:05:06.000+0000
-    re_datetimeval = re.compile(r'\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}')
-    re_datetimestr = re.compile(r'"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}')
-
-    def __init__(self, *args, **kwargs):
-        self.old_object_pairs_hook = kwargs.get('object_pairs_hook')
-        kwargs['object_pairs_hook'] = self.convert
-        super(CustomJSONDecoder, self).__init__(*args, **kwargs)
-
-    def decode(self, obj):
-        if self.re_datetimestr.match(obj):
-            return dateutil.parser.parse(obj[1:-1])
-        return super(CustomJSONDecoder, self).decode(obj)
-
-    def convert(self, obj):
-        for index, (key, val) in enumerate(obj):
-            if isinstance(val, str) and self.re_datetimeval.match(val):
-                obj[index] = (key, dateutil.parser.parse(val))
-        if callable(self.old_object_pairs_hook):
-            return self.old_object_pairs_hook(obj)
-        return dict(obj)
-
-
-def objectpath(node, keypath, default=None):
-    '''
-    Traverse down a dot-separated object path into dict items or object attrs.
-    For example, ``objectpath(handler, 'request.headers.User-Agent')`` returns
-    ``handler.request.headers['User-Agent']``. Dictionary access is preferred.
-    Returns ``None`` if the path is not found.
-    '''
-    for key in keypath.split('.'):
-        if hasattr(node, '__getitem__'):
-            node = node.get(key)
-        else:
-            node = getattr(node, key, None)
-        if node is None:
-            return default
-    return node
-
-
-def recursive_encode(data, encoding='utf-8'):
-    '''
-    Convert all Unicode values into UTF-8 encoded byte strings in-place
-    '''
-    for key, value, node in walk(data):
-        if isinstance(key, str):
-            newkey = key.encode(encoding)
-            node[newkey] = node.pop(key)
-            key = newkey
-        if isinstance(value, str):
-            node[key] = value.encode(encoding)
-
-
-def prune_keys(conf, keys={}):
-    '''
-    Returns a deep copy of a configuration removing specified keys.
-    ``prune_keys(conf, {'comment'})`` drops the "comment" key from any dict or sub-dict.
-    '''
-    if isinstance(conf, dict):
-        conf = AttrDict({k: prune_keys(v, keys) for k, v in conf.items() if k not in keys})
-    elif isinstance(conf, (list, tuple)):
-        conf = [prune_keys(v, keys) for v in conf]
-    return conf
-
-
 class TimedRotatingCSVHandler(logging.handlers.TimedRotatingFileHandler):
     '''
     Same as logging.handlers.TimedRotatingFileHandler, but writes to a CSV.
-    The constructor accepts an additional ``keys`` list as input that has
-    column keys. When ``.emit()`` is called, it expects an object with the
-    same keys as ``keys``.
+    The constructor accepts an additional `keys` list as input that has
+    column keys. When `.emit()` is called, it expects an object with the
+    same keys as `keys`.
     '''
 
     def __init__(self, *args, **kwargs):
         self.keys = kwargs.pop('keys')
         super(TimedRotatingCSVHandler, self).__init__(*args, **kwargs)
 
     def _open(self):
@@ -823,50 +858,22 @@
 
 def ioloop_running(loop):
     '''Returns whether the Tornado ioloop is running on not'''
     # TODO: Pressing Ctrl+C may cause this to raise an exception. Explore how to handle that
     return loop.asyncio_loop.is_running()
 
 
-def used_kwargs(method, kwargs, ignore_keywords=False):
-    '''
-    Splits kwargs into those used by method, and those that are not.
-
-    Returns a tuple of (used, rest). *used* is a dict subset of kwargs with only
-    keys used by method. *rest* has the remaining kwargs keys.
-
-    If the method uses ``**kwargs`` (keywords), it uses all keys. To ignore this
-    and return only named arguments, use ``ignore_keywords=True``.
-    '''
-    # In Pandas 1.5, DataFrame.to_csv and DataFrame.to_excel are wrapped with @deprecate_kwargs.
-    # We dive deeper to detect the actual keywords. __wrapped__ is provided by functools.wraps
-    # https://docs.python.org/3/library/functools.html
-    while hasattr(method, '__wrapped__'):
-        method = method.__wrapped__
-    argspec = inspect.getfullargspec(method)
-    # If method uses **kwargs, return all kwargs (unless you ignore **kwargs)
-    if argspec.varkw and not ignore_keywords:
-        used, rest = kwargs, {}
-    else:
-        # Split kwargs into 2 dicts -- used and rest
-        used, rest = {}, {}
-        for key, val in kwargs.items():
-            target = used if key in set(argspec.args) else rest
-            target[key] = val
-    return used, rest
-
-
 def setup_secrets(path, max_age_days=1000000, clear=True):
     '''
-    Load ``<path>`` (which must be Path) as a YAML file. Update it into gramex.config.variables.
+    Load `<path>` (which must be Path) as a YAML file. Update it into gramex.config.variables.
 
-    If there's a ``SECRETS_URL:`` and ``SECRETS_KEY:`` key, the text from ``SECRETS_URL:`` is
-    decrypted using ``secrets_key``.
+    If there's a `SECRETS_URL:` and `SECRETS_KEY:` key, the text from `SECRETS_URL:` is
+    decrypted using `secrets_key`.
 
-    If there's a ``SECRETS_IMPORT:`` string, list or dict, the values are treated as file patterns
+    If there's a `SECRETS_IMPORT:` string, list or dict, the values are treated as file patterns
     pointing to other secrets file to be imported.
     '''
     if not path.is_file():
         return
 
     with path.open(encoding='utf-8') as handle:
         result = yaml.safe_load(handle)
```

### Comparing `gramex-1.89.2/gramex/data.py` & `gramex-1.90.0/gramex/data.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/debug.py` & `gramex-1.90.0/gramex/debug.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/deploy.yaml` & `gramex-1.90.0/gramex/deploy.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/download.vega.js` & `gramex-1.90.0/gramex/download.vega.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/gramex.yaml` & `gramex-1.90.0/gramex/gramex.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,21 @@
 
   FilterHandler:
     formats: *FORMATS
 
     default:
       _limit: 10000 # Limit entries by default
 
+  MessageHandler:
+    message_default:
+      POST:
+        id: base64.urlsafe_b64encode(uuid.uuid4().bytes).strip(b"=").decode('utf-8')
+        user: handler.current_user.get('id', None) if handler.current_user else None
+        timestamp: datetime.datetime.utcnow().isoformat()
+
 # The `log:` section defines the log handlers. It uses the same structure as the
 # Python logging schema.
 # https://docs.python.org/3/library/logging.config.html#logging-config-dictschema
 log:
   version: 1
   root:
     level: DEBUG
@@ -133,28 +140,30 @@
     # Elasticsearch DEBUG logs are verbose. Restrict to INFO
     elasticsearch:
       level: INFO
     # Watchdog DEBUG logs are verbose. Restrict to INFO
     watchdog:
       level: INFO
     # DEPRECATED. authhandler.py used to log login/logout as CSV. Now we use storelocations
+    # Remove after 1 Jan 2024
     gramex.user:
       level: INFO
       propagate: false
       handlers: [user]
   handlers:
     none:
       class: logging.NullHandler
     console:
       class: logging.StreamHandler
       formatter: console
     gramex-console:
       class: logging.StreamHandler
       formatter: gramex-console
     # DEPRECATED. authhandler.py used to log login/logout as CSV. Now we use storelocations
+    # Remove after 1 Jan 2024
     user:
       class: gramex.config.TimedRotatingCSVHandler
       filename: $GRAMEXDATA/logs/user.csv
       # NOTE: Use any key supported by gramex.transforms.build_log_info()
       keys: [datetime, event, session, user, ip, headers.User-Agent]
       level: INFO
       <<: *ROTATE_WEEKLY
```

### Comparing `gramex-1.89.2/gramex/gramexfeatures.csv` & `gramex-1.90.0/gramex/gramexfeatures.csv`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/gramexsize.csv` & `gramex-1.90.0/gramex/gramexsize.csv`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 gramex.cache.HDF5Store.*,app.session.type=hdf5,18
 gramex.cache.HDF5Store.*,url.*.kwargs.store.type=hdf5,18
 gramex.cache.JSONStore.*,app.session.type=json,15
 gramex.cache.JSONStore.*,url.*.kwargs.store.type=json,15
 gramex.config.*,*,158
 gramex.data.*,url.*.handler=FormHandler|FilterHandler|MLHandler|DriverHandler,348
 gramex.debug.*,TODO - if any PY code uses gramex.debug,32
-gramex.install.*,TODO - Gramex app installation & management,162
+gramex.install.*,TODO - Gramex app installation & management,164
 gramex.license.*,TODO - Gramex enterprise license management,9
 gramex.migrate.*,url.*.handler=GoogleAuth|SimpleAuth|OAuth2|FacebookAuth|TwitterAuth|SAMLAuth|SAMLAuth2|LDAPAuth|DBAuth|IntegratedAuth|SMSAuth|EmailAuth,3
 gramex.ml.Classifier.*,url.*.handler=ModelHandler,15
 gramex.ml._conda_r_home,TODO - if any PY code uses gramex.ml.r,4
 gramex.ml.r,TODO - if any PY code uses gramex.ml.r,11
 gramex.ml.groupmeans,TODO - if any PY code use gramex.ml.groupmeans,11
 gramex.ml.weighted_avg,TODO - if any PY code use gramex.ml.groupmeans,1
@@ -102,25 +102,25 @@
 gramex.handlers.basehandler.BaseMixin.apikey,url.*.kwargs.auth,1
 gramex.handlers.basehandler.BaseMixin.revoke_apikey,url.*.kwargs.auth,1
 gramex.handlers.basehandler.BaseMixin.override_user,url.*.kwargs.auth,7
 gramex.handlers.basehandler.BaseMixin.set_last_visited,url.*.kwargs.auth,3
 gramex.handlers.basehandler.BaseMixin.check_ratelimit,url.*.kwargs.ratelimit,2
 gramex.handlers.basehandler.BaseMixin.update_ratelimit,url.*.kwargs.ratelimit,2
 gramex.handlers.basehandler.BaseMixin.set_ratelimit_headers,url.*.kwargs.ratelimit,2
-gramex.handlers.basehandler.BaseHandler.initialize,url,8
+gramex.handlers.basehandler.BaseHandler.initialize,url,3
 gramex.handlers.basehandler.BaseHandler.get_arg,url,3
 gramex.handlers.basehandler.BaseHandler.prepare,url,2
 gramex.handlers.basehandler.BaseHandler.set_default_headers,url,1
 gramex.handlers.basehandler.BaseHandler.on_finish,url,2
 gramex.handlers.basehandler.BaseHandler.get_current_user,url,1
 gramex.handlers.basehandler.BaseHandler.log_exception,url,1
 gramex.handlers.basehandler.BaseHandler.authorize,url.*.kwargs.auth,10
 gramex.handlers.basehandler.BaseHandler.argparse,url.*.handler=CaptureHandler|MLHandler|ModelHandler|OpenAPIHandler,26
 gramex.handlers.basehandler.BaseHandler.create_template_loader,url.*.kwargs.template,1
-gramex.handlers.basehandler.BaseWebSocketHandler.*,url.*.handler=WebSocketHandler|Websocket,13
+gramex.handlers.basehandler.BaseWebSocketHandler.*,url.*.handler=WebSocketHandler|Websocket,11
 gramex.handlers.basehandler.SetupFailedHandler.get,url,1
 gramex.handlers.basehandler.check_membership,url.*.kwargs.auth.membership,4
 gramex.handlers.basehandler._check_condition,url.*.kwargs.auth.membership,6
 gramex.handlers.capturehandler.*,url.*.handler=CaptureHandler|Screenshot,46
 gramex.handlers.comichandler.*,url.*.handler=ComicHandler|Comic,6
 gramex.handlers.drivehandler.*,url.*.handler=DriveHandler|Storage,36
 gramex.handlers.filehandler.*,url.*.handler=FileHandler|DirectoryHandler|File,59
@@ -140,15 +140,15 @@
 gramex.handlers.socialhandler.TwitterRESTHandler.*,url.*.handler=TwitterRESTHandler|Twitter,8
 gramex.handlers.socialhandler.FacebookGraphHandler.*,url.*.handler=FacebookGraphHandler|Facebook,6
 gramex.handlers.uploadhandler.*,url.*.handler=UploadHandler|Upload,44
 gramex.handlers.websockethandler.*,url.*.handler=WebSocketHandler|Websocket,7
 gramex.handlers.__init__.*,url.*.handler=OAuth2|FacebookAuth|TwitterAuth|SAMLAuth|SAMLAuth2|LDAPAuth|DBAuth|IntegratedAuth|SMSAuth|EmailAuth,4
 gramex.pptgen.*,url.*.handler=PPTXHandler,363
 gramex.pptgen2.*,url.*.handler=PPTXHandler,244
-gramex.services.emailer.*,email,31
+gramex.services.emailer.*,email,34
 gramex.services.rediscache.*,cache.*.type=redis,23
 gramex.services.scheduler.*,schedule,26
 gramex.services.sms.*,sms,10
 gramex.services.ttlcache.*,cache.*.type=memory,46
 gramex.services.urlcache.get_cachefile,cache,4
 gramex.services.urlcache.CacheFile.*,cache,3
 gramex.services.urlcache.MemoryCacheFile.*,cache.*.type=memory,4
@@ -172,15 +172,15 @@
 gramex.services.__init__.encrypt,encrypt,1
 gramex.services.__init__.test,test,1
 gramex.services.__init__.gramexlog,gramexlog,11
 gramex.services.__init__.storelocations,storelocations,2
 gramex.services.__init__._storelocations_purge,storelocations,1
 gramex.services.__init__.GramexApp.log_request,log,4
 gramex.services.__init__.GramexApp.clear_handlers,app,1
-gramex.services.__init__.create_alert,alert,52
+gramex.services.__init__.create_alert,alert,36
 gramex.services.__init__._markdown_convert,alert,2
 gramex.services.__init__._tmpl,alert,2
 gramex.services.__init__._stop_all_tasks,schedule,2
 gramex.services.__init__._stop_all_tasks,alert,2
 gramex.services.__init__._sort_url_patterns,url.*.pattern,1
 gramex.services.__init__._url_normalize,url.*.pattern,2
 gramex.services.__init__._get_cache_key,url.*.cache,10
```

### Comparing `gramex-1.89.2/gramex/handlers/__init__.py` & `gramex-1.90.0/gramex/handlers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 from .proxyhandler import ProxyHandler
 from .modelhandler import ModelHandler
 from .mlhandler import MLHandler, MLPredictor
 from .filterhandler import FilterHandler
 from .drivehandler import DriveHandler
 from .comichandler import ComicHandler
 from .openapihandler import OpenAPIHandler
+from .messagehandler import MessageHandler
 
 # Aliases
 Comic = ComicHandler
 Command = ProcessHandler
+Message = CommentHandler = MessageHandler
 Data = FormHandler
 Facebook = FacebookGraphHandler
 File = DirectoryHandler = FileHandler
 Filter = FilterHandler
 Function = FunctionHandler
 JSON = JSONHandler
 ML = MLHandler
@@ -43,14 +45,15 @@
 __all__ = [
     'BaseHandler',
     'BaseWebSocketHandler',
     'BaseMixin',
     'Capture',
     'CaptureHandler',
     'Command',
+    'CommentHandler',
     'Comic',
     'ComicHandler',
     'Data',
     'DirectoryHandler',
     'DriveHandler',
     'FacebookGraphHandler',
     'File',
@@ -60,14 +63,16 @@
     'FormHandler',
     'Function',
     'FunctionHandler',
     'GoogleAuth',
     'JSON',
     'JSONHandler',
     'LogoutHandler',
+    'Message',
+    'MessageHandler',
     'ModelHandler',
     'ML',
     'MLHandler',
     'MLPredictor',
     'OpenAPI',
     'OpenAPIHandler',
     'PPTXHandler',
```

### Comparing `gramex-1.89.2/gramex/handlers/auth.recaptcha.template.html` & `gramex-1.90.0/gramex/handlers/auth.recaptcha.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/authhandler.py` & `gramex-1.90.0/gramex/handlers/authhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/basehandler.py` & `gramex-1.90.0/gramex/handlers/basehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1072,43 +1072,46 @@
         remaining = max(ratelimit.limit - ratelimit.usage - 1, 0)
         self.set_header('X-Ratelimit-Limit', str(ratelimit.limit))
         self.set_header('X-Ratelimit-Remaining', str(remaining))
         self.set_header('X-RateLimit-Reset', str(ratelimit.expiry))
         if ratelimit.usage >= ratelimit.limit:
             self.set_header('Retry-After', str(ratelimit.expiry))
 
-
-class BaseHandler(RequestHandler, BaseMixin):
-    '''
-    BaseHandler provides auth, caching and other services common to all request
-    handlers. All RequestHandlers must inherit from BaseHandler.
-    '''
-
-    def initialize(self, **kwargs):
-        # self.request.arguments does not handle unicode keys well.
-        # In Py2, it returns a str (not unicode). In Py3, it returns latin-1 unicode.
+    def initialize_handler(self):
+        '''Initialize self.args and other handler attributes'''
+        # self.request.arguments does not handle unicode keys well. It returns latin-1 unicode.
+        # https://github.com/tornadoweb/tornado/issues/2733
         # Convert this to proper unicode using UTF-8 and store in self.args
         self.args = {}
         for k in self.request.arguments:
-            key = (k if isinstance(k, bytes) else k.encode('latin-1')).decode('utf-8')
+            key = k.encode('latin-1').decode('utf-8')
             # Invalid unicode (e.g. ?x=%f4) throws HTTPError. This disrupts even
             # error handlers. So if there's invalid unicode, log & continue.
             try:
                 self.args[key] = self.get_arguments(k)
             except HTTPError:
-                app_log.exception(f'Invalid URL argument {k}')
-
+                app_log.exception(f'{self.name}: Invalid unicode ?{k}')
         self._session, self._session_json = None, 'null'
         if self.cache:
             self.cachefile = self.cache()
             self.original_get = self.get
             self.get = self._cached_get
         if self._set_xsrf:
             self.xsrf_token
 
+
+class BaseHandler(RequestHandler, BaseMixin):
+    '''
+    BaseHandler provides auth, caching and other services common to all request
+    handlers. All RequestHandlers must inherit from BaseHandler.
+    '''
+
+    def initialize(self, **kwargs):
+        self.initialize_handler()
+
         # Set the method to the ?x-http-method-overrride argument or the
         # X-HTTP-Method-Override header if they exist
         if 'x-http-method-override' in self.args:
             self.request.method = self.args.pop('x-http-method-override')[0].upper()
         elif 'X-HTTP-Method-Override' in self.request.headers:
             self.request.method = self.request.headers['X-HTTP-Method-Override'].upper()
 
@@ -1359,21 +1362,15 @@
             autoescape=settings['autoescape'],
             whitespace=settings.get('template_whitespace', None),
         )
 
 
 class BaseWebSocketHandler(WebSocketHandler, BaseMixin):
     def initialize(self, **kwargs):
-        self._session, self._session_json = None, 'null'
-        if self.cache:
-            self.cachefile = self.cache()
-            self.original_get = self.get
-            self.get = self._cached_get
-        if self._set_xsrf:
-            self.xsrf_token
+        self.initialize_handler()
 
     @tornado.gen.coroutine
     def get(self, *args, **kwargs):
         for method in self._on_init_methods:
             method(self)
         yield super(BaseWebSocketHandler, self).get(*args, **kwargs)
```

### Comparing `gramex-1.89.2/gramex/handlers/capturehandler.py` & `gramex-1.90.0/gramex/handlers/capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/comichandler.py` & `gramex-1.90.0/gramex/handlers/comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/drivehandler.py` & `gramex-1.90.0/gramex/handlers/drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/filehandler.py` & `gramex-1.90.0/gramex/handlers/filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/filehandler.template.html` & `gramex-1.90.0/gramex/handlers/filehandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/formhandler.py` & `gramex-1.90.0/gramex/handlers/formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/functionhandler.py` & `gramex-1.90.0/gramex/handlers/functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/jsonhandler.py` & `gramex-1.90.0/gramex/handlers/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/mlhandler.py` & `gramex-1.90.0/gramex/handlers/mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/modelhandler.py` & `gramex-1.90.0/gramex/handlers/modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/openapiconfig.yaml` & `gramex-1.90.0/gramex/handlers/openapiconfig.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/openapihandler.py` & `gramex-1.90.0/gramex/handlers/openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/pptxhandler.py` & `gramex-1.90.0/gramex/handlers/pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/processhandler.py` & `gramex-1.90.0/gramex/handlers/processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/proxyhandler.py` & `gramex-1.90.0/gramex/handlers/proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/queryhandler.template.html` & `gramex-1.90.0/gramex/handlers/queryhandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/socialhandler.py` & `gramex-1.90.0/gramex/handlers/socialhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/uploadhandler.py` & `gramex-1.90.0/gramex/handlers/uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/handlers/websockethandler.py` & `gramex-1.90.0/gramex/handlers/websockethandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/http.py` & `gramex-1.90.0/gramex/http.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/install.py` & `gramex-1.90.0/gramex/install.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-'''
-Defines command line services to install, setup and run apps.
-'''
+'''Defines command line services to install, setup and run apps.'''
 import contextlib
 import io
 import os
 import sys
 import time
 import yaml
 import stat
@@ -13,67 +11,146 @@
 import shutil
 import datetime
 import requests
 from shutil import which
 from pathlib import Path
 from collections import Counter
 
+from orderedattrdict import AttrDict
+
 # B404:import_subprocess only developers can access this, not users
 from subprocess import Popen, check_output, CalledProcessError  # nosec B404
-from orderedattrdict import AttrDict
-from orderedattrdict.yamlutils import AttrDictYAMLLoader
-from zipfile import ZipFile
+from textwrap import dedent
 from tornado.template import Template
+from zipfile import ZipFile
 import gramex
 import gramex.license
 from gramex.config import ChainConfig, PathConfig, variables, app_log, slug
 
-usage = '''
-install: |
-    usage:
-        gramex install <app> <url> [--target=DIR]
-        gramex install <app> --cmd="COMMAND" [--target=DIR]
+
+def install(args, kwargs):
+    '''
+    usage: gramex install <app> <url> [--target=DIR]
 
     "app" is any name you want to locally call the application.
 
     "url" can be a:
-        - local ZIP file (/path/to/app.zip)
-        - local directory (/path/to/directory)
-        - URL of a ZIP file (https://github.com/user/repo/archive/master.zip)
 
-    target is the directory to install at (defaults to user data directory.)
+    - local ZIP file (/path/to/app.zip)
+    - local directory (/path/to/directory)
+    - URL of a ZIP file (https://github.com/user/repo/archive/master.zip)
 
-    cmd is a shell command to run. If it has the word "TARGET" in caps, it is
-    replaced by the target directory.
+    target is the directory to install at (defaults to user data directory.)
 
     After installation, runs "gramex setup" which runs the Makefile, setup.ps1,
     setup.sh, requirements.txt, setup.py, bower install, npm install, yarn install.
 
+    Options:
+
+    - `--cmd="COMMAND"` is a shell command to run. Any word "TARGET" in caps
+      is substituted by the target directory.
+
     Installed apps:
     {apps}
+    '''
+    if len(args) < 1:
+        app_log.error(show_usage('install'))
+        return
 
-setup: |
+    appname = args[0]
+    app_log.info(f'Installing: {appname}')
+    app_config = get_app_config(appname, kwargs)
+    if len(args) == 2:
+        app_config.url = args[1]
+        run_install(app_config)
+    elif 'url' in app_config:
+        run_install(app_config)
+    elif 'cmd' in app_config:
+        returncode = run_command(app_config)
+        if returncode != 0:
+            app_log.error(f'Command failed with return code {returncode}. Aborting installation')
+            return
+    else:
+        app_log.error(f'Use --url=... or --cmd=... to specific source of {appname}')
+        return
+
+    # Post-installation
+    app_config.target = run_setup(app_config.target)
+    app_config['installed'] = {'time': datetime.datetime.utcnow()}
+    save_user_config(appname, app_config)
+    app_log.info(f'Installed. Run `gramex run {appname}`')
+
+
+def setup(args, kwargs):
+    '''
     usage: gramex setup <target> [<target> ...] [--all]
 
     target is the directory to set up (required). This can be an absolute path,
     relative path, or a directory name under $GRAMEXPATH/apps/.
 
     gramex setup --all sets up all apps under $GRAMEXPATH/apps/
 
     Run the following commands at that directory in sequence, if possible:
-        - make
-        - powershell -File setup.ps1
-        - bash setup.sh
-        - pip install --upgrade -r requirements.txt
-        - python setup.py
-        - bower --allow-root install
-        - npm install
-        - yarn install --prefer-offline
 
-run: |
+    - make
+    - powershell -File setup.ps1
+    - bash setup.sh
+    - pip install --upgrade -r requirements.txt
+    - python setup.py
+    - bower --allow-root install
+    - npm install
+    - yarn install --prefer-offline
+    '''
+    for target in args:
+        run_setup(target)
+        return
+    if 'all' in kwargs:
+        root = os.path.join(variables['GRAMEXPATH'], 'apps')
+        for filename in os.listdir(root):
+            target = os.path.join(root, filename)
+            # Only run setup on directories. Ignore __pycache__, etc
+            if os.path.isdir(target) and not filename.startswith('_'):
+                run_setup(target)
+        return
+    app_log.error(show_usage('setup'))
+
+
+def uninstall(args, kwargs):
+    '''
+    usage: gramex uninstall <app> [<app> ...]
+
+    "app" is the name of the locally installed application. You can uninstall
+    multiple applications in one command.
+
+    All information about the application is lost. You cannot undo this.
+
+    Installed apps:
+    {apps}
+    '''
+    if len(args) < 1:
+        app_log.error(show_usage('uninstall'))
+        return
+    if len(args) > 1 and kwargs:
+        app_log.errorf(f'Arguments allowed only with single app. Ignoring {", ".join(args[1:])}')
+        args = args[:1]
+
+    for appname in args:
+        app_log.info(f'Uninstalling: {appname}')
+
+        # Delete the target directory if it exists
+        app_config = get_app_config(appname, kwargs)
+        if os.path.exists(app_config.target):
+            safe_rmtree(app_config.target)
+        else:
+            app_log.error(f'No directory {app_config.target} to remove')
+        save_user_config(appname, None)
+
+
+def run(args, kwargs):
+    '''
     usage: gramex run <app> [--target=DIR] [--dir=DIR] [--<options>=<value>]
 
     "app" is the name of the locally installed application.
 
     If "app" is not installed, specify --target=DIR to run from DIR. The next
     "gramex run app" will automatically run from DIR.
 
@@ -86,86 +163,448 @@
 
     ... will preserve the "target", "listen.port" and "browser" values. Running
     "gramex run app" will re-use these values. To clear the option, leave the
     value blank. For example "--browser=" will clear the browser option.
 
     Installed apps:
     {apps}
+    '''
+    if len(args) < 1:
+        app_log.error(show_usage('run'))
+        return
+    if len(args) > 1:
+        app_log.error(f'Can only run one app. Ignoring {", ".join(args[1:])}')
 
-uninstall: |
-    usage: gramex uninstall <app> [<app> ...]
-
-    "app" is the name of the locally installed application. You can uninstall
-    multiple applications in one command.
+    appname = args.pop(0)
+    app_config = get_app_config(appname, kwargs)
 
-    All information about the application is lost. You cannot undo this.
+    target = app_config.target
+    if 'dir' in app_config:
+        target = os.path.join(target, app_config.dir)
+    if os.path.isdir(target):
+        os.chdir(target)
+        gramex.paths['base'] = Path('.')
+        # If we run with updated parameters, save for next run under the .run config
+        run_config = app_config.setdefault('run', {})
+        for key in kwargs:
+            if key not in app_keys:
+                run_config[key] = app_config.pop(key)
+        save_user_config(appname, app_config)
+        # Tell the user what configs are used
+        cline = ' '.join('--%s=%s' % arg for arg in flatten_config(app_config.get('run', {})))
+        app_log.info(
+            'Gramex %s | %s %s | %s | Python %s',
+            gramex.__version__,
+            appname,
+            cline,
+            os.getcwd(),
+            sys.version.replace('\n', ' '),
+        )
+        gramex.init(args=AttrDict(app=app_config['run']))
+    elif appname in apps_config['user']:
+        # The user configuration has a wrong path. Inform user
+        app_log.error(
+            f'{appname}: no target path {app_config.target}. '
+            f'Run "gramex uninstall {appname}" and try again.',
+        )
+    else:
+        app_log.error(f'{appname}: no target path {app_config.target}')
 
-    Installed apps:
-    {apps}
 
-service: |
+def service(args, kwargs):
+    '''
     usage: gramex service <cmd> [--options]
 
-    Install a Gramex application as a Windows service:
+    Install a Gramex application as a Windows service
 
         gramex service install
             --cwd  "C:/path/to/application/"
             --user "DOMAIN\\USER"                # Optional user to run as
             --password "user-password"          # Required if user is specified
             --startup manual|auto|disabled
 
-    Update:
+    Update the Windows service
 
         gramex service update <same parameters as install>
 
-    Remove:
+    Remove the Windows service
 
         gramex service remove       # or gramex service uninstall
 
     Start / stop commands
 
         gramex service start
         gramex service stop
+    '''
+    try:
+        import gramex.winservice
+    except ImportError:
+        app_log.error('Unable to load winservice. Is this Windows?')
+        raise
+    if len(args) < 1:
+        app_log.error(show_usage('service'))
+        return
+    gramex.winservice.GramexService.setup(args, **kwargs)
 
-init: |
-    gramex init [--target=DIR]
-    gramex init minimal [--target=DIR]
 
-    Initializes a Gramex project at the current or target dir. Specifically, it:
+def init(args, kwargs):
+    '''
+    usage: gramex init [minimal] [--target=<path>]
+
+    Initializes a Gramex project at the current directory or target path.
+    Specifically, it:
+
     - Sets up a git repo
     - Install supporting files for a Gramex project from a template
-      - "gramex init" sets up dependencies for a local system
+      - "gramex init" sets up all dependencies
       - "gramex init minimal" sets up minimal dependencies
     - Runs gramex setup (which runs npm install and other dependencies)
 
     Options:
-      --target <path>               # Location to install at. Defaults to
 
-mail: |
-    gramex mail <key>               # Send mail named <key>
-    gramex mail --list              # Lists all keys in config file
-    gramex mail --init              # Initializes config file
+    - `--target <path>` is the location to install at. Defaults to $GRAMEXAPPS
+    '''
+    if len(args) > 2:
+        app_log.error(show_usage('init'))
+        return
+    if len(args) == 0:
+        args.append('default')
+    source_dir = os.path.join(variables['GRAMEXPATH'], 'apps', 'init', args[0])
+    if not os.path.exists(source_dir):
+        app_log.error(f'Unknown init template: {args[0]} under {source_dir}')
+
+    kwargs.setdefault('target', os.getcwd())
+    app_log.info(f'Initializing Gramex project at {kwargs.target}')
+    data = {
+        'appname': os.path.basename(kwargs.target),
+        'author': _check_output('git config user.name', default='Author'),
+        'email': _check_output('git config user.email', default='user@example.org'),
+        'date': datetime.datetime.today().strftime('%Y-%m-%d'),
+        'version': gramex.__version__,
+    }
+    # Ensure that appname is a valid Python module name
+    appname = slug.module(data['appname'])
+    if appname[0] not in string.ascii_lowercase:
+        appname = 'app' + appname
+    data['appname'] = appname
+
+    # Create a git repo. But if git fails, do not stop. Continue with the rest.
+    with contextlib.suppress(OSError):
+        _run_console('git init')
+    # Install Git LFS if available. Set git_lfs=None if it fails, so .gitignore ignores assets/**
+    data['git_lfs'] = which('git-lfs')
+    if data['git_lfs']:
+        try:
+            _run_console('git lfs install')
+            _run_console('git lfs track "assets/**"')
+        except OSError:
+            data['git_lfs'] = None
+
+    # Copy all directories & files. Files with '.template.' are treated as templates.
+    for root, dirs, files in os.walk(source_dir):
+        relpath = os.path.relpath(root, start=source_dir)
+        for name in dirs + files:
+            source, targetname, template_data = os.path.join(root, name), name, None
+            if '.template.' in name:
+                targetname, template_data = name.replace('.template.', '.'), data
+            target = os.path.join(kwargs.target, relpath, targetname)
+            if os.path.exists(target):
+                app_log.warning(f'Skip existing {target}')
+            elif os.path.isdir(source):
+                _mkdir(target)
+            elif os.path.isfile(source):
+                app_log.info(f'Copy file {source}')
+                with io.open(source, 'rb') as handle:
+                    result = handle.read()
+                    if template_data is not None:
+                        result = Template(result).generate(**template_data)
+                with io.open(target, 'wb') as handle:
+                    handle.write(result)
+            else:
+                app_log.warning(f'Skip unknown file {source}')
+
+    run_setup(kwargs.target)
+
+
+default_mail_config = r'''# Gramex mail configuration at
+# List keys with "gramex mail --list --conf={confpath}"
+
+# See https://gramener.com/gramex/guide/email/ for help
+email:
+  default-email:
+    type: gmail
+    email: $GRAMEXMAILUSER
+    password: $GRAMEXMAILPASSWORD
+    # Add stub: log to test the application without sending mails
+
+# See https://gramener.com/gramex/guide/alert/
+alert:
+  hello-world:
+    to: admin@example.org
+    subject: Alert from Gramex
+    body: |
+      This is a test email
+'''
+
+
+def mail(args, kwargs):
+    '''
+    usage
+
+        gramex mail <key>           # Send mail named <key>
+        gramex mail --list          # Lists all keys in config file
+        gramex mail --init          # Initializes config file
 
     The config is a gramex.yaml file. It must have email: and alert: sections.
     If the current folder has a gramex.yaml, that's used. Else the default is
     $GRAMEXDATA/mail/gramexmail.yaml.
 
     Options:
-      --conf <path>                 # Specify a different conf file location
 
-license: |
-    gramex license                  # Show Gramex license
-    gramex license accept           # Accept Gramex license
-    gramex license reject           # Reject Gramex license
+    - `--conf <path>` specifies a different conf file location
+    '''
+    # Get config file location
+    default_dir = os.path.join(variables['GRAMEXDATA'], 'mail')
+    _mkdir(default_dir)
+    if 'conf' in kwargs:
+        confpath = kwargs.conf
+    elif os.path.exists('gramex.yaml'):
+        confpath = os.path.abspath('gramex.yaml')
+    else:
+        confpath = os.path.join(default_dir, 'gramexmail.yaml')
 
-features: |
-    gramex features                 # Show Gramex features used in current project
-'''
-# B506:yaml_load yaml.load is safe since it only reads the string above, not user-created content
-usage = yaml.load(usage, Loader=AttrDictYAMLLoader)  # nosec B506
+    if not os.path.exists(confpath):
+        if 'init' in kwargs:
+            with io.open(confpath, 'w', encoding='utf-8') as handle:
+                handle.write(default_mail_config.format(confpath=confpath))
+            app_log.info(f'Initialized {confpath}')
+        elif not args and not kwargs:
+            app_log.error(show_usage('mail'))
+        else:
+            app_log.error(f'Missing config {confpath}. Use --init to generate skeleton')
+        return
+
+    conf = PathConfig(confpath)
+    if 'list' in kwargs:
+        for key, alert in conf.get('alert', {}).items():
+            to = alert.get('to', '')
+            if isinstance(to, list):
+                to = ', '.join(to)
+            gramex.console('{:15}\t"{}" to {}'.format(key, alert.get('subject'), to))
+        return
+
+    if 'init' in kwargs:
+        app_log.error(f'Config already exists at {confpath}')
+        return
+
+    if len(args) < 1:
+        app_log.error(show_usage('mail'))
+        return
+
+    from gramex.services import email as setup_email, create_alert
+
+    alert_conf = conf.get('alert', {})
+    email_conf = conf.get('email', {})
+    setup_email(email_conf)
+    sys.path += os.path.dirname(confpath)
+    for key in args:
+        if key not in alert_conf:
+            app_log.error(f'Missing key {key} in {confpath}')
+            continue
+        alert = create_alert(key, alert_conf[key])
+        alert()
+
+
+def license(args, kwargs):
+    '''
+    usage: gramex license [accept|reject]
+
+    Commands
+
+        gramex license          # Show Gramex license
+        gramex license accept   # Accept Gramex license
+        gramex license reject   # Reject Gramex license
+    '''
+    if len(args) == 0:
+        gramex.console(gramex.license.EULA)
+        if gramex.license.is_accepted():
+            gramex.console('License already ACCEPTED. Run "gramex license reject" to reject')
+        else:
+            gramex.console('License NOT YET accepted. Run "gramex license accept" to accept')
+    elif args[0] == 'accept':
+        gramex.license.accept(force=True)
+    elif args[0] == 'reject':
+        gramex.license.reject()
+    else:
+        app_log.error(f'Invalid command license {args[0]}')
+
+
+def features(args, kwargs) -> dict:
+    '''
+    usage: gramex features [<path> [...]]
+
+    Counts gramex features used in a project path (or current directory) from gramex.yaml.
+    Prints 3 columns:
+
+    - type: SVC=Service, MS=Microservice, KWARG=Config (keyword argument)
+    - feature: Feature name (e.g. FormHandler)
+    - count: Number of times the feature is used
+
+    Options:
+
+    - `--format [table|json|csv]` picks an output format. Defaults to table
+    '''
+    import pandas as pd
+
+    # Load the feature mapping from cache
+    features = gramex.cache.open("gramexfeatures.csv", rel=True).set_index(["type", "name"])[
+        "feature"
+    ]
+
+    base = gramex.config.PathConfig(os.path.join(os.path.dirname(gramex.__file__), 'gramex.yaml'))
+    # Load the gramex.yaml configuration
+    usage = Counter({(type, feature): 0 for ((type, _name), feature) in features.items()})
+    parsed_count = 0
+    for folder in args or [os.getcwd()]:
+        project_yaml = os.path.join(folder, 'gramex.yaml')
+        app = gramex.config.PathConfig(project_yaml)
+        # Skip if gramex.yaml is not found or empty or we're unable to parse
+        if not app:
+            continue
+        parsed_count += 1
+        conf = +gramex.config.ChainConfig([('base', base), ('app', app)])
+
+        # Convert invalid gramex.yaml (e.g. empty gramex.yaml) as an empty dict
+        conf = conf if isinstance(conf, dict) else {}
+        # List the features used. TODO: Improve this using configuration
+        for url in conf.get('url', {}).values():
+            if isinstance(url, dict):
+                name = url.get('handler', '').replace('gramex.handlers.', '')
+                # Count micro-services usage
+                if name in features['MS']:
+                    usage[('MS', features['MS'][name])] += 1
+                else:
+                    usage[('ERR-MS', name)] += 1
+                # Count kwargs: usage
+                url_kwargs = url.get('kwargs', {})
+                for key in url_kwargs:
+                    if key in features['KWARG']:
+                        usage[('KWARG', features['KWARG'][key])] += 1
+                # cache: is a special kwarg that sits outside kwargs. Count it too
+                if 'cache' in url:
+                    usage[('KWARG', 'cache')] += 1
+        # List the services used
+        for service in conf.keys():
+            # If the service is conditional, e.g. `log if condition`, take just the first part
+            name = service.split()[0]
+            if name in features['SVC']:
+                usage[('SVC', features['SVC'][name])] += 1
+
+    # Return features usage table
+    output = ''
+    if parsed_count:
+        usage = pd.DataFrame(usage.values(), index=usage.keys()).reset_index()
+        usage.columns = ['type', 'feature', 'count']
+        format = kwargs.get('format', 'table')
+        if format == 'table':
+            output = usage.to_string()
+        elif format == 'csv':
+            output = usage.to_csv(index=False, lineterminator='\n')
+        elif format == 'json':
+            output = usage.to_json(orient='records')
+        else:
+            app_log.error(f'--format must be [table|csv|json] not {format}')
+            return
+    return output
+
+
+def complexity(args, kwargs) -> dict:
+    '''
+    usage: gramex complexity [folder [...]]
+    '''
+    # Calulate cyclomatic complexity of the project
+    import ast
+    import fnmatch
+    import mccabe
+    import pandas as pd
+    import re
+
+    # B404:import_subprocess only used for internal Gramex scripts
+    from subprocess import check_output  # nosec B404
+
+    project_path = os.getcwd() if len(args) == 0 else args[0]
+    project_yaml = _gramex_yaml_path(project_path, kwargs)
+    if project_yaml is None:
+        return
+
+    def walk(node: dict, parents: tuple = ()):
+        for key, value in node.items():
+            new_key = parents + (str(key),)
+            if hasattr(value, 'items'):
+                yield new_key, None
+                yield from walk(value, new_key)
+            else:
+                yield new_key, value
+
+    py_complexity = 0
+    relevent_file_matcher = re.compile(r'^((?!(site-packages|node_modules)).)*\.py$')
+
+    for root, _dirs, files in os.walk(project_path):
+        for filename in files:
+            path: str = os.path.join(root, filename)
+            if not relevent_file_matcher.match(path):
+                continue
+            rel_path: str = os.path.relpath(path, project_path)
+            with open(path, 'rb') as handle:
+                code = handle.read()
+            try:
+                tree = compile(code, rel_path, 'exec', ast.PyCF_ONLY_AST)
+            except SyntaxError as e:
+                app_log.exception('SYNTAXERROR: %s %s', path, e)
+                continue
+            visitor = mccabe.PathGraphingAstVisitor()
+            visitor.preorder(tree, visitor)
+            for node in visitor.graphs.values():
+                py_complexity += node.complexity()
+
+    base = gramex.config.PathConfig(os.path.join(os.path.dirname(gramex.__file__), 'gramex.yaml'))
+    try:
+        app = gramex.config.PathConfig(project_yaml)
+        conf = +gramex.config.ChainConfig([('base', base), ('app', app)])
+    except Exception as e:  # noqa: B902 capture load errors as a "feature"
+        app_log.exception(str(e))
+        return
+    yamlpaths = {'.'.join(key): val for key, val in walk(conf)}
+    used = set()
+    gramexsize = gramex.cache.open('gramexsize.csv', rel=True)
+    for _index, gramex_code in gramexsize.iterrows():
+        # TODO: fnmatch.filter() is the slowest part. Optimize it
+        if '=' not in gramex_code['yamlpath']:
+            if fnmatch.filter(yamlpaths.keys(), gramex_code['yamlpath']):
+                used.add(gramex_code['codepath'])
+        else:
+            yaml_key, yaml_value = gramex_code['yamlpath'].split('=', 1)
+            matches = fnmatch.filter(yamlpaths.keys(), yaml_key)
+            for key in matches:
+                if yamlpaths[key] in yaml_value.split('|'):
+                    used.add(gramex_code['codepath'])
+    gramex_complexity = gramexsize.set_index('codepath')['complexity'][list(used)].sum()
+
+    # Calculate JS complexity
+    # B602:subprocess_popen_with_shell_equals_true and
+    # B607:start_process_with_partial_path are safe to skip since this is a Gramex internal cmd
+    output = check_output(['npx', '@gramex/escomplexity'], cwd=project_path, shell=True)  # nosec
+    es_complexity = int(output.decode('utf-8').split('\n')[-2].strip())
+    return pd.DataFrame(
+        {
+            'py': [py_complexity],
+            'js': [es_complexity],
+            'gramex': [gramex_complexity],
+        }
+    )
 
 
 class TryAgainError(Exception):
     '''If shutil.rmtree fails, and we've fixed the problem, raise this to try again'''
 
     pass
 
@@ -255,18 +694,15 @@
             app_log.warning(f'Not removing directory {target} (outside $GRAMEXDATA)')
             return False
     else:
         _try_remove(target, retries, delay, func, **kwargs)
 
 
 def zip_prefix_filter(members, prefix):
-    '''
-    Return only ZIP file members starting with the directory prefix, with the
-    prefix stripped out.
-    '''
+    '''Return only ZIP file members starting with directory prefix, with prefix stripped out.'''
     if not prefix:
         return members
     offset = len(prefix)
     result = []
     for zipinfo in members:
         if zipinfo.filename.startswith(prefix):
             zipinfo.filename = zipinfo.filename[offset:]
@@ -464,138 +900,15 @@
             yield from flatten_config(value, keystr)
         else:
             yield keystr, value
 
 
 def show_usage(command):
     apps = (+apps_config).keys()
-    return 'gramex {command}\n\n{desc}'.format(
-        command=command,
-        desc=usage[command].strip().format(apps='\n'.join('- ' + app for app in sorted(apps))),
-    )
-
-
-def install(args, kwargs):
-    if len(args) < 1:
-        app_log.error(show_usage('install'))
-        return
-
-    appname = args[0]
-    app_log.info(f'Installing: {appname}')
-    app_config = get_app_config(appname, kwargs)
-    if len(args) == 2:
-        app_config.url = args[1]
-        run_install(app_config)
-    elif 'url' in app_config:
-        run_install(app_config)
-    elif 'cmd' in app_config:
-        returncode = run_command(app_config)
-        if returncode != 0:
-            app_log.error(f'Command failed with return code {returncode}. Aborting installation')
-            return
-    else:
-        app_log.error(f'Use --url=... or --cmd=... to specific source of {appname}')
-        return
-
-    # Post-installation
-    app_config.target = run_setup(app_config.target)
-    app_config['installed'] = {'time': datetime.datetime.utcnow()}
-    save_user_config(appname, app_config)
-    app_log.info(f'Installed. Run `gramex run {appname}`')
-
-
-def setup(args, kwargs):
-    for target in args:
-        run_setup(target)
-        return
-    if 'all' in kwargs:
-        root = os.path.join(variables['GRAMEXPATH'], 'apps')
-        for filename in os.listdir(root):
-            target = os.path.join(root, filename)
-            # Only run setup on directories. Ignore __pycache__, etc
-            if os.path.isdir(target) and not filename.startswith('_'):
-                run_setup(target)
-        return
-    app_log.error(show_usage('setup'))
-
-
-def uninstall(args, kwargs):
-    if len(args) < 1:
-        app_log.error(show_usage('uninstall'))
-        return
-    if len(args) > 1 and kwargs:
-        app_log.errorf(f'Arguments allowed only with single app. Ignoring {", ".join(args[1:])}')
-        args = args[:1]
-
-    for appname in args:
-        app_log.info(f'Uninstalling: {appname}')
-
-        # Delete the target directory if it exists
-        app_config = get_app_config(appname, kwargs)
-        if os.path.exists(app_config.target):
-            safe_rmtree(app_config.target)
-        else:
-            app_log.error(f'No directory {app_config.target} to remove')
-        save_user_config(appname, None)
-
-
-def run(args, kwargs):
-    if len(args) < 1:
-        app_log.error(show_usage('run'))
-        return
-    if len(args) > 1:
-        app_log.error(f'Can only run one app. Ignoring {", ".join(args[1:])}')
-
-    appname = args.pop(0)
-    app_config = get_app_config(appname, kwargs)
-
-    target = app_config.target
-    if 'dir' in app_config:
-        target = os.path.join(target, app_config.dir)
-    if os.path.isdir(target):
-        os.chdir(target)
-        gramex.paths['base'] = Path('.')
-        # If we run with updated parameters, save for next run under the .run config
-        run_config = app_config.setdefault('run', {})
-        for key in kwargs:
-            if key not in app_keys:
-                run_config[key] = app_config.pop(key)
-        save_user_config(appname, app_config)
-        # Tell the user what configs are used
-        cline = ' '.join('--%s=%s' % arg for arg in flatten_config(app_config.get('run', {})))
-        app_log.info(
-            'Gramex %s | %s %s | %s | Python %s',
-            gramex.__version__,
-            appname,
-            cline,
-            os.getcwd(),
-            sys.version.replace('\n', ' '),
-        )
-        gramex.init(args=AttrDict(app=app_config['run']))
-    elif appname in apps_config['user']:
-        # The user configuration has a wrong path. Inform user
-        app_log.error(
-            f'{appname}: no target path {app_config.target}. '
-            f'Run "gramex uninstall {appname}" and try again.',
-        )
-    else:
-        app_log.error(f'{appname}: no target path {app_config.target}')
-
-
-def service(args, kwargs):
-    '''Install, remove, start or stop Gramex as a Windows service.'''
-    try:
-        import gramex.winservice
-    except ImportError:
-        app_log.error('Unable to load winservice. Is this Windows?')
-        raise
-    if len(args) < 1:
-        app_log.error(show_usage('service'))
-        return
-    gramex.winservice.GramexService.setup(args, **kwargs)
+    return usage[command].format(apps='\n'.join('- ' + app for app in sorted(apps)))
 
 
 def _check_output(cmd, default=b'', **kwargs):
     '''Run cmd and return output. Return default in case the command fails'''
     try:
         # B603:subprocess_without_shell_equals_true is safe since this is developer-initiated
         return check_output(shlex.split(cmd), **kwargs).strip()  # nosec B603
@@ -619,331 +932,31 @@
 
 def _mkdir(path):
     '''Create directory tree up to path if path does not exist'''
     if not os.path.exists(path):
         os.makedirs(path)
 
 
-def init(args, kwargs):
-    '''Create Gramex scaffolding files.'''
-    if len(args) > 2:
-        app_log.error(show_usage('init'))
-        return
-    if len(args) == 0:
-        args.append('default')
-    source_dir = os.path.join(variables['GRAMEXPATH'], 'apps', 'init', args[0])
-    if not os.path.exists(source_dir):
-        app_log.error(f'Unknown init template: {args[0]} under {source_dir}')
-
-    kwargs.setdefault('target', os.getcwd())
-    app_log.info(f'Initializing Gramex project at {kwargs.target}')
-    data = {
-        'appname': os.path.basename(kwargs.target),
-        'author': _check_output('git config user.name', default='Author'),
-        'email': _check_output('git config user.email', default='user@example.org'),
-        'date': datetime.datetime.today().strftime('%Y-%m-%d'),
-        'version': gramex.__version__,
-    }
-    # Ensure that appname is a valid Python module name
-    appname = slug.module(data['appname'])
-    if appname[0] not in string.ascii_lowercase:
-        appname = 'app' + appname
-    data['appname'] = appname
-
-    # Create a git repo. But if git fails, do not stop. Continue with the rest.
-    with contextlib.suppress(OSError):
-        _run_console('git init')
-    # Install Git LFS if available. Set git_lfs=None if it fails, so .gitignore ignores assets/**
-    data['git_lfs'] = which('git-lfs')
-    if data['git_lfs']:
-        try:
-            _run_console('git lfs install')
-            _run_console('git lfs track "assets/**"')
-        except OSError:
-            data['git_lfs'] = None
-
-    # Copy all directories & files. Files with '.template.' are treated as templates.
-    for root, dirs, files in os.walk(source_dir):
-        relpath = os.path.relpath(root, start=source_dir)
-        for name in dirs + files:
-            source = os.path.join(root, name)
-            targetname = name.replace('$appname', appname)
-            template_data = None
-            if '.template.' in name:
-                targetname, template_data = name.replace('.template.', '.'), data
-            target = os.path.join(kwargs.target, relpath, targetname)
-            if os.path.exists(target):
-                app_log.warning(f'Skip existing {target}')
-            elif os.path.isdir(source):
-                _mkdir(target)
-            elif os.path.isfile(source):
-                app_log.info(f'Copy file {source}')
-                with io.open(source, 'rb') as handle:
-                    result = handle.read()
-                    if template_data is not None:
-                        result = Template(result).generate(**template_data)
-                with io.open(target, 'wb') as handle:
-                    handle.write(result)
-            else:
-                app_log.warning(f'Skip unknown file {source}')
-
-    run_setup(kwargs.target)
-
-
-default_mail_config = r'''# Gramex mail configuration at
-# List keys with "gramex mail --list --conf={confpath}"
-
-# See https://gramener.com/gramex/guide/email/ for help
-email:
-  default-email:
-    type: gmail
-    email: $GRAMEXMAILUSER
-    password: $GRAMEXMAILPASSWORD
-    # Add stub: log to test the application without sending mails
-
-# See https://gramener.com/gramex/guide/alert/
-alert:
-  hello-world:
-    to: admin@example.org
-    subject: Alert from Gramex
-    body: |
-      This is a test email
-'''
-
-
-def mail(args, kwargs):
-    # Get config file location
-    default_dir = os.path.join(variables['GRAMEXDATA'], 'mail')
-    _mkdir(default_dir)
-    if 'conf' in kwargs:
-        confpath = kwargs.conf
-    elif os.path.exists('gramex.yaml'):
-        confpath = os.path.abspath('gramex.yaml')
-    else:
-        confpath = os.path.join(default_dir, 'gramexmail.yaml')
-
-    if not os.path.exists(confpath):
-        if 'init' in kwargs:
-            with io.open(confpath, 'w', encoding='utf-8') as handle:
-                handle.write(default_mail_config.format(confpath=confpath))
-            app_log.info(f'Initialized {confpath}')
-        elif not args and not kwargs:
-            app_log.error(show_usage('mail'))
-        else:
-            app_log.error(f'Missing config {confpath}. Use --init to generate skeleton')
-        return
-
-    conf = PathConfig(confpath)
-    if 'list' in kwargs:
-        for key, alert in conf.get('alert', {}).items():
-            to = alert.get('to', '')
-            if isinstance(to, list):
-                to = ', '.join(to)
-            gramex.console('{:15}\t"{}" to {}'.format(key, alert.get('subject'), to))
-        return
-
-    if 'init' in kwargs:
-        app_log.error(f'Config already exists at {confpath}')
-        return
-
-    if len(args) < 1:
-        app_log.error(show_usage('mail'))
-        return
-
-    from gramex.services import email as setup_email, create_alert
-
-    alert_conf = conf.get('alert', {})
-    email_conf = conf.get('email', {})
-    setup_email(email_conf)
-    sys.path += os.path.dirname(confpath)
-    for key in args:
-        if key not in alert_conf:
-            app_log.error(f'Missing key {key} in {confpath}')
-            continue
-        alert = create_alert(key, alert_conf[key])
-        alert()
-
-
-def license(args, kwargs):
-    if len(args) == 0:
-        gramex.console(gramex.license.EULA)
-        if gramex.license.is_accepted():
-            gramex.console('License already ACCEPTED. Run "gramex license reject" to reject')
-        else:
-            gramex.console('License NOT YET accepted. Run "gramex license accept" to accept')
-    elif args[0] == 'accept':
-        gramex.license.accept(force=True)
-    elif args[0] == 'reject':
-        gramex.license.reject()
-    else:
-        app_log.error(f'Invalid command license {args[0]}')
-
-
-def features(args, kwargs) -> dict:
-    """
-    This function extracts feature information from a gramex.yaml file and returns
-    a dictionary with a Pandas DataFrame containing information about the features
-    used in the gramex application.
-
-    Args:
-        args: This function doesn't use any arguments.
-        kwargs: A dictionary that can contain a 'conf' key that specifies the path
-            to the gramex.yaml file. If 'conf' is not specified, the function will
-            use the current working directory.
-
-    Returns:
-        A dictionary containing a Pandas DataFrame with the following columns:
-            - type: The type of feature (e.g., 'MS' for a URL handler)
-            - feature: The name of the feature (e.g., the name of the URL handler)
-            - count: The number of times the feature is used in the gramex app.
-    """
-    import pandas as pd
-
-    project_yaml = _gramex_yaml_path(os.getcwd() if len(args) == 0 else args[0], kwargs)
-    if project_yaml is None:
-        return
-
-    # Load the feature mapping from cache
-    features = gramex.cache.open("gramexfeatures.csv", rel=True).set_index(["type", "name"])[
-        "feature"
-    ]
-    # Load the gramex.yaml configuration
-    base = gramex.config.PathConfig(os.path.join(os.path.dirname(gramex.__file__), 'gramex.yaml'))
-    proj_features = Counter({(type, feature): 0 for ((type, _name), feature) in features.items()})
-    try:
-        app = gramex.config.PathConfig(project_yaml)
-        conf = +gramex.config.ChainConfig([('base', base), ('app', app)])
-    except Exception as e:  # noqa: B902 capture load errors as a "feature"
-        app_log.exception(str(e))
-        return
-
-    # If the configuration is not a dictionary, return an empty result
-    if not isinstance(conf, dict):
-        return
-
-    # List the features used. TODO: Improve this using configuration
-    for url in conf.get('url', {}).values():
-        if not isinstance(url, dict):
-            continue
-        name = url.get('handler', '').replace('gramex.handlers.', '')
-        if name in features['MS']:
-            proj_features[('MS', features['MS'][name])] += 1
-        else:
-            proj_features[('ERR-MS', name)] += 1
-
-        if 'cache' in url:
-            proj_features[('KWARG', 'cache')] += 1
-
-        url_kwargs = url.get('kwargs', {})
-        for key in url_kwargs:
-            if key not in features['KWARG']:
-                continue
-            proj_features[('KWARG', features['KWARG'][key])] += 1
-
-    # List the services used
-    for service in conf.keys():
-        # If the service is conditional, e.g. `log if condition`, take just the first part
-        name = service.split()[0]
-        if name in features['SVC']:
-            proj_features[('SVC', features['SVC'][name])] += 1
-
-    # Create features table
-
-    proj_features = pd.DataFrame(proj_features.values(), index=proj_features.keys()).reset_index()
-    proj_features.columns = ['type', 'feature', 'count']
-
-    return proj_features
-
-
-def complexity(args, kwargs) -> dict:
-    # Calulate cyclomatic complexity of the project
-    import ast
-    import fnmatch
-    import mccabe
-    import pandas as pd
-    import re
-
-    # B404:import_subprocess only used for internal Gramex scripts
-    from subprocess import check_output  # nosec B404
-
-    project_path = os.getcwd() if len(args) == 0 else args[0]
-    project_yaml = _gramex_yaml_path(project_path, kwargs)
-    if project_yaml is None:
-        return
-
-    def walk(node: dict, parents: tuple = ()):
-        for key, value in node.items():
-            new_key = parents + (str(key),)
-            if hasattr(value, 'items'):
-                yield new_key, None
-                yield from walk(value, new_key)
-            else:
-                yield new_key, value
-
-    py_complexity = 0
-    relevent_file_matcher = re.compile(r'^((?!(site-packages|node_modules)).)*\.py$')
-
-    for root, _dirs, files in os.walk(project_path):
-        for filename in files:
-            path: str = os.path.join(root, filename)
-            if not relevent_file_matcher.match(path):
-                continue
-            rel_path: str = os.path.relpath(path, project_path)
-            with open(path, 'rb') as handle:
-                code = handle.read()
-            try:
-                tree = compile(code, rel_path, 'exec', ast.PyCF_ONLY_AST)
-            except SyntaxError as e:
-                app_log.exception('SYNTAXERROR: %s %s', path, e)
-                continue
-            visitor = mccabe.PathGraphingAstVisitor()
-            visitor.preorder(tree, visitor)
-            for node in visitor.graphs.values():
-                py_complexity += node.complexity()
-
-    base = gramex.config.PathConfig(os.path.join(os.path.dirname(gramex.__file__), 'gramex.yaml'))
-    try:
-        app = gramex.config.PathConfig(project_yaml)
-        conf = +gramex.config.ChainConfig([('base', base), ('app', app)])
-    except Exception as e:  # noqa: B902 capture load errors as a "feature"
-        app_log.exception(str(e))
-        return
-    yamlpaths = {'.'.join(key): val for key, val in walk(conf)}
-    used = set()
-    gramexsize = gramex.cache.open('gramexsize.csv', rel=True)
-    for _index, gramex_code in gramexsize.iterrows():
-        # TODO: fnmatch.filter() is the slowest part. Optimize it
-        if '=' not in gramex_code['yamlpath']:
-            if fnmatch.filter(yamlpaths.keys(), gramex_code['yamlpath']):
-                used.add(gramex_code['codepath'])
-        else:
-            yaml_key, yaml_value = gramex_code['yamlpath'].split('=', 1)
-            matches = fnmatch.filter(yamlpaths.keys(), yaml_key)
-            for key in matches:
-                if yamlpaths[key] in yaml_value.split('|'):
-                    used.add(gramex_code['codepath'])
-    gramex_complexity = gramexsize.set_index('codepath')['complexity'][list(used)].sum()
-
-    # Calculate JS complexity
-    # B602:subprocess_popen_with_shell_equals_true and
-    # B607:start_process_with_partial_path are safe to skip since this is a Gramex internal cmd
-    output = check_output(['npx', '@gramex/escomplexity'], cwd=project_path, shell=True)  # nosec
-    es_complexity = int(output.decode('utf-8').split('\n')[-2].strip())
-    return pd.DataFrame(
-        {
-            'py': [py_complexity],
-            'js': [es_complexity],
-            'gramex': [gramex_complexity],
-        }
-    )
-
-
 def _gramex_yaml_path(folder, kwargs):
     project_yaml = os.path.join(folder, 'gramex.yaml')
     # Get config file location
     if 'conf' in kwargs:
         return kwargs.conf
     elif os.path.exists(project_yaml):
         return project_yaml
     else:
         app_log.error(f'Missing {project_yaml}')
         return
+
+
+usage = {
+    'complexity': dedent(complexity.__doc__),
+    'features': dedent(features.__doc__),
+    'init': dedent(init.__doc__),
+    'install': dedent(install.__doc__),
+    'license': dedent(license.__doc__),
+    'mail': dedent(mail.__doc__),
+    'run': dedent(run.__doc__),
+    'service': dedent(service.__doc__),
+    'setup': dedent(setup.__doc__),
+    'uninstall': dedent(uninstall.__doc__),
+}
```

### Comparing `gramex-1.89.2/gramex/license.py` & `gramex-1.90.0/gramex/license.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/migrate.py` & `gramex-1.90.0/gramex/migrate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/ml.py` & `gramex-1.90.0/gramex/ml.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/ml_api.py` & `gramex-1.90.0/gramex/ml_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen/__init__.py` & `gramex-1.90.0/gramex/pptgen/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen/color.py` & `gramex-1.90.0/gramex/pptgen/color.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen/colors.json` & `gramex-1.90.0/gramex/pptgen/colors.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen/commands.py` & `gramex-1.90.0/gramex/pptgen/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen/fonts.json` & `gramex-1.90.0/gramex/pptgen/fonts.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen/fontwidth.py` & `gramex-1.90.0/gramex/pptgen/fontwidth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen/utils.py` & `gramex-1.90.0/gramex/pptgen/utils.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen2/__init__.py` & `gramex-1.90.0/gramex/pptgen2/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen2/commands.py` & `gramex-1.90.0/gramex/pptgen2/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pptgen2/config.yaml` & `gramex-1.90.0/gramex/pptgen2/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/pynode.py` & `gramex-1.90.0/gramex/pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/scale.py` & `gramex-1.90.0/gramex/scale.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/secrets.py` & `gramex-1.90.0/gramex/secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/servicenow.yaml` & `gramex-1.90.0/gramex/servicenow.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/services/__init__.py` & `gramex-1.90.0/gramex/services/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -589,43 +589,103 @@
 
     def clear_handlers(self):
         # Clear all handlers in the application
         del self.default_router.rules[:]
         del self.wildcard_router.rules[:]
 
 
-def create_alert(name, alert):
-    '''Generate the function to be run by alert() using the alert configuration'''
-
-    # Configure email service
-    if alert.get('service', None) is None:
+def get_mailer(config, name=''):
+    '''Return the email service config and corresponding mailer for a given config.'''
+    if config.get('service', None) is None:
         if len(info.email) > 0:
-            service = alert['service'] = list(info.email.keys())[0]
-            app_log.warning(f'alert: {name}: using first email service: {service}')
+            service = config['service'] = list(info.email.keys())[0]
+            app_log.warning(f'{name}: using first email service: {service}')
         else:
-            app_log.error(f'alert: {name}: define an email: service to use')
-            return
-    service = alert['service']
+            app_log.error(f'{name}: define an email: service to use')
+            return None, None
+    service = config['service']
     mailer = info.email.get(service, None)
     if mailer is None:
-        app_log.error(f'alert: {name}: undefined email service: {service}')
-        return
+        app_log.error(f'{name}: undefined email service: {service}')
+        return None, None
+    return service, mailer
+
+
+_addr_fields = ['to', 'cc', 'bcc', 'reply_to', 'on_behalf_of', 'from']
+
+
+def create_mail(data, config, name):
+    '''Return kwargs that can be passed to a mailer.mail'''
+    mail = {}
+    for key in ['bodyfile', 'htmlfile', 'markdownfile']:
+        target = key.replace('file', '')
+        if key in config and target not in config:
+            path = _tmpl(config[key]).generate(**data).decode('utf-8')
+            tmpl = gramex.cache.open(path, 'template')
+            mail[target] = tmpl.generate(**data).decode('utf-8')
+    for key in _addr_fields + ['subject', 'body', 'html', 'markdown']:
+        if key not in config:
+            continue
+        if isinstance(config[key], list):
+            mail[key] = [_tmpl(v).generate(**data).decode('utf-8') for v in config[key]]
+        else:
+            mail[key] = _tmpl(config[key]).generate(**data).decode('utf-8')
+    headers = {}
+    # user: {id: ...} creates an X-Gramex-User header to mimic the user
+    if 'user' in config:
+        user = deepcopy(config['user'])
+        for key, val, node in walk(user):
+            node[key] = _tmpl(val).generate(**data).decode('utf-8')
+        user = json.dumps(user, ensure_ascii=True, separators=(',', ':'))
+        headers['X-Gramex-User'] = tornado.web.create_signed_value(
+            info.app.settings['cookie_secret'], 'user', user
+        )
+    if 'markdown' in mail:
+        mail['html'] = _markdown_convert(mail.pop('markdown'))
+    if 'images' in config:
+        mail['images'] = {}
+        for cid, val in config['images'].items():
+            urlpath = _tmpl(val).generate(**data).decode('utf-8')
+            urldata = urlfetch(urlpath, info=True, headers=headers)
+            if urldata['content_type'].startswith('image/'):
+                mail['images'][cid] = urldata['name']
+            else:
+                with io.open(urldata['name'], 'rb') as temp_file:
+                    bytestoread = 80
+                    first_line = temp_file.read(bytestoread)
+                # TODO: let admin know that the image was not processed
+                app_log.error(
+                    f'{name}: {cid}: {urldata["r"].status_code} '
+                    f'({urldata["content_type"]}) not an image: {urlpath}\n'
+                    f'{first_line!r}'
+                )
+    if 'attachments' in config:
+        mail['attachments'] = [
+            urlfetch(_tmpl(v).generate(**data).decode('utf-8'), headers=headers)
+            for v in config['attachments']
+        ]
+    return mail
+
+
+def create_alert(name, alert):
+    '''Generate the function to be run by alert() using the alert configuration'''
+    # Configure email service
+    service, mailer = get_mailer(alert, name=f'alert: {name}')
 
     # - Warn if to, cc, bcc exists and is not a string or list of strings. Ignore incorrect
     #    - if to: [1, 'user@example.org'], then
     #    - log a warning about the 1. Drop the 1. to: becomes ['user@example.org']
 
     # Error if to, cc, bcc are all missing, return None
     if not any(key in alert for key in ['to', 'cc', 'bcc']):
         app_log.error(f'alert: {name}: missing to/cc/bcc')
         return
     # Ensure that config has the right type (str, dict, list)
     contentfields = ['body', 'html', 'bodyfile', 'htmlfile', 'markdown', 'markdownfile']
-    addr_fields = ['to', 'cc', 'bcc', 'reply_to', 'on_behalf_of', 'from']
-    for key in ['subject'] + addr_fields + contentfields:
+    for key in ['subject'] + _addr_fields + contentfields:
         if not isinstance(alert.get(key, ''), (str, list)):
             app_log.error(f'alert: {name}.{key}: {alert[key]!r} must be a list or str')
             return
     if not isinstance(alert.get('images', {}), dict):
         app_log.error(f'alert: {name}.images: {alert["images"]!r} is not a dict')
         return
     if not isinstance(alert.get('attachments', []), list):
@@ -708,68 +768,14 @@
                 raise ValueError(
                     f'alert: {name}: each: data.{alert["each"]} must be '
                     + 'dict/list/DF, not {type(each_data)}'
                 )
         else:
             each.append((0, None))
 
-    def create_mail(data):
-        '''
-        Return kwargs that can be passed to a mailer.mail
-        '''
-        mail = {}
-        for key in ['bodyfile', 'htmlfile', 'markdownfile']:
-            target = key.replace('file', '')
-            if key in alert and target not in alert:
-                path = _tmpl(alert[key]).generate(**data).decode('utf-8')
-                tmpl = gramex.cache.open(path, 'template')
-                mail[target] = tmpl.generate(**data).decode('utf-8')
-        for key in addr_fields + ['subject', 'body', 'html', 'markdown']:
-            if key not in alert:
-                continue
-            if isinstance(alert[key], list):
-                mail[key] = [_tmpl(v).generate(**data).decode('utf-8') for v in alert[key]]
-            else:
-                mail[key] = _tmpl(alert[key]).generate(**data).decode('utf-8')
-        headers = {}
-        # user: {id: ...} creates an X-Gramex-User header to mimic the user
-        if 'user' in alert:
-            user = deepcopy(alert['user'])
-            for key, val, node in walk(user):
-                node[key] = _tmpl(val).generate(**data).decode('utf-8')
-            user = json.dumps(user, ensure_ascii=True, separators=(',', ':'))
-            headers['X-Gramex-User'] = tornado.web.create_signed_value(
-                info.app.settings['cookie_secret'], 'user', user
-            )
-        if 'markdown' in mail:
-            mail['html'] = _markdown_convert(mail.pop('markdown'))
-        if 'images' in alert:
-            mail['images'] = {}
-            for cid, val in alert['images'].items():
-                urlpath = _tmpl(val).generate(**data).decode('utf-8')
-                urldata = urlfetch(urlpath, info=True, headers=headers)
-                if urldata['content_type'].startswith('image/'):
-                    mail['images'][cid] = urldata['name']
-                else:
-                    with io.open(urldata['name'], 'rb') as temp_file:
-                        bytestoread = 80
-                        first_line = temp_file.read(bytestoread)
-                    # TODO: let admin know that the image was not processed
-                    app_log.error(
-                        f'alert: {name}: {cid}: {urldata["r"].status_code} '
-                        f'({urldata["content_type"]}) not an image: {urlpath}\n'
-                        f'{first_line!r}'
-                    )
-        if 'attachments' in alert:
-            mail['attachments'] = [
-                urlfetch(_tmpl(v).generate(**data).decode('utf-8'), headers=headers)
-                for v in alert['attachments']
-            ]
-        return mail
-
     def run_alert(callback=None, args=None):
         '''
         Runs the configured alert. If a callback is specified, calls the
         callback with all email arguments. Else sends the email.
         If args= is specified, add it as data['args'].
         '''
         app_log.info(f'alert: {name} running')
@@ -780,15 +786,17 @@
             app_log.exception(f'alert: {name} data processing failed')
             fail.append({'error': e})
 
         retval = []
         for index, row in each:
             data['index'], data['row'], data['config'] = index, row, alert
             try:
-                retval.append(AttrDict(index=index, row=row, mail=create_mail(data)))
+                retval.append(
+                    AttrDict(index=index, row=row, mail=create_mail(data, alert, f'alert: {name}'))
+                )
             except Exception as e:
                 app_log.exception(f'alert: {name}[{index}] templating (row={row!r})')
                 fail.append({'index': index, 'row': row, 'error': e})
 
         callback = mailer.mail if not callable(callback) else callback
         done = []
         for v in retval:
```

### Comparing `gramex-1.89.2/gramex/services/emailer.py` & `gramex-1.90.0/gramex/services/emailer.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,14 +157,22 @@
             server.starttls()
         if self.email is not None and self.password is not None:
             server.login(self.email, self.password)
         server.sendmail(sender, to, msg.as_string())
         server.quit()
         app_log.info(f'Email sent via {self.client["host"]} ({self.email}) to {", ".join(to)}')
 
+    def mail_log(self, **kwargs):
+        '''Same as mail() but logs the exception. Useful with running in a thread'''
+        try:
+            self.mail(**kwargs)
+        except Exception:
+            app_log.exception(f'SMTP failed: {kwargs}')
+            raise
+
 
 def recipients(**kwargs):
     # Return all recipients from to/cc/bcc fields.
     # They may be comma-separated strings or lists of comma-separated strings.
     recipients = []
     for key in kwargs:
         if key.lower() in {'to', 'cc', 'bcc'}:
```

### Comparing `gramex-1.89.2/gramex/services/rediscache.py` & `gramex-1.90.0/gramex/services/rediscache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/services/scheduler.py` & `gramex-1.90.0/gramex/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/services/sms.py` & `gramex-1.90.0/gramex/services/sms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/services/ttlcache.py` & `gramex-1.90.0/gramex/services/ttlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/services/urlcache.py` & `gramex-1.90.0/gramex/services/urlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/services/watcher.py` & `gramex-1.90.0/gramex/services/watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/sm_api.py` & `gramex-1.90.0/gramex/sm_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/topcause.py` & `gramex-1.90.0/gramex/topcause.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/transformers.py` & `gramex-1.90.0/gramex/transformers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/transforms/__init__.py` & `gramex-1.90.0/gramex/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/transforms/auth.py` & `gramex-1.90.0/gramex/transforms/auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/transforms/template.py` & `gramex-1.90.0/gramex/transforms/template.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/transforms/transforms.py` & `gramex-1.90.0/gramex/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/transforms/twitterstream.py` & `gramex-1.90.0/gramex/transforms/twitterstream.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex/winservice.py` & `gramex-1.90.0/gramex/winservice.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/gramex.egg-info/PKG-INFO` & `gramex-1.90.0/gramex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.89.2
+Version: 1.90.0
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.89.2/gramex.egg-info/SOURCES.txt` & `gramex-1.90.0/gramex.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,20 @@
 gramex.egg-info/dependency_links.txt
 gramex.egg-info/entry_points.txt
 gramex.egg-info/requires.txt
 gramex.egg-info/top_level.txt
 gramex/apps/__init__.py
 gramex/apps/admin/.gitignore
 gramex/apps/admin/gramex.yaml
-gramex/apps/admin2/.eslintrc.js
 gramex/apps/admin2/.snyk
 gramex/apps/admin2/admin.css
 gramex/apps/admin2/gramex.yaml
 gramex/apps/admin2/gramexadmin.py
 gramex/apps/admin2/index.html
-gramex/apps/admin2/package-lock.json
-gramex/apps/admin2/package.json
-gramex/apps/admin2/rollup.config.js
 gramex/apps/admin2/schedule.js
-gramex/apps/admin2/schedule.src.js
-gramex/apps/admin2/schedule.template.html
 gramex/apps/capture/README.md
 gramex/apps/capture/capture.js
 gramex/apps/capture/chromecapture.js
 gramex/apps/capture/index.html
 gramex/apps/capture/package-lock.json
 gramex/apps/capture/package.json
 gramex/apps/filemanager/.snyk
@@ -64,34 +58,27 @@
 gramex/apps/filemanager/filemanager-snippet.html
 gramex/apps/filemanager/filemanager.html
 gramex/apps/filemanager/filemanager.js
 gramex/apps/filemanager/filemanager.py
 gramex/apps/filemanager/gramex.yaml
 gramex/apps/filemanager/index.html
 gramex/apps/filemanager/navbar.html
-gramex/apps/init/default/$appname.py
+gramex/apps/init/default/.eslintrc.yml
 gramex/apps/init/default/.flake8
 gramex/apps/init/default/.gitlab-ci.yml
 gramex/apps/init/default/.secrets.yaml
-gramex/apps/init/default/.stylelintrc.js
 gramex/apps/init/default/.template.gitignore
 gramex/apps/init/default/README.template.md
-gramex/apps/init/default/favicon.ico
 gramex/apps/init/default/gramex.template.yaml
 gramex/apps/init/default/index.template.html
 gramex/apps/init/default/login.template.html
 gramex/apps/init/default/package.template.json
 gramex/apps/init/default/style.scss
 gramex/apps/init/default/template-navbar.template.html
 gramex/apps/init/default/assets/README.template.md
-gramex/apps/init/default/error/400.html
-gramex/apps/init/default/error/401.html
-gramex/apps/init/default/error/403.html
-gramex/apps/init/default/error/404.html
-gramex/apps/init/default/error/500.html
 gramex/apps/init/default/js/README.template.md
 gramex/apps/init/ide/.gitlab-ci.template.yml
 gramex/apps/init/ide/gramex.template.yaml
 gramex/apps/init/ide/index.template.html
 gramex/apps/init/minimal/gramex.template.yaml
 gramex/apps/init/minimal/index.template.html
 gramex/apps/languagetool/README.md
@@ -280,14 +267,15 @@
 gramex/handlers/drivehandler.py
 gramex/handlers/filehandler.py
 gramex/handlers/filehandler.template.html
 gramex/handlers/filterhandler.py
 gramex/handlers/formhandler.py
 gramex/handlers/functionhandler.py
 gramex/handlers/jsonhandler.py
+gramex/handlers/messagehandler.py
 gramex/handlers/mlhandler.py
 gramex/handlers/modelhandler.py
 gramex/handlers/openapiconfig.yaml
 gramex/handlers/openapihandler.py
 gramex/handlers/pptxhandler.py
 gramex/handlers/processhandler.py
 gramex/handlers/proxyhandler.py
```

### Comparing `gramex-1.89.2/gramex.egg-info/requires.txt` & `gramex-1.90.0/gramex.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/pyproject.toml` & `gramex-1.90.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gramex"
-version = "1.89.2"
+version = "1.90.0"
 description = "Gramex: Low Code Data Solutions Platform"
 # People with 2+ contributions on https://github.com/gramener/gramex/graphs/contributors
 authors = [
     {name = "Anand S", email = "s.anand@gramener.com"},
     {name = "Pratap Vardhan", email = "pratapapvr@gmail.com"},
     {name = "Jaidev Deshpande", email = "jaidev.deshpande@gramener.com"},
     {name = "Bhanu Kamapantula", email = "talk2kish@gmail.com"},
@@ -85,14 +85,18 @@
 gramex = "gramex:commandline"
 secrets = "gramex.secrets:commandline"
 slidesense = "gramex.pptgen2:commandline"
 
 [tool.setuptools.packages.find]
 include = ["gramex*"]
 
+[tool.black]
+# pytest/complexity_error/invalid.py has non-parseable Python code
+force-exclude = "complexity_error"
+
 [project.optional-dependencies]
 # pip install "gramex[full]" for better debugging and ML support
 full = [
     "boto3",  # for gramex.services.sns.AmazonSNS
     "datasets",  # for gramex.transformers
     "line_profiler",  # for gramex.debug.lineprofile
     "pymysql",  # for MySQL connections
```

### Comparing `gramex-1.89.2/setup.cfg` & `gramex-1.90.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_admin.py` & `gramex-1.90.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_alerts.py` & `gramex-1.90.0/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_args.py` & `gramex-1.90.0/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_auth.py` & `gramex-1.90.0/tests/test_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,20 @@
     def login_ok(self, *args, **kwargs):
         check_next = kwargs.pop('check_next')
         r = self.login(*args, **kwargs)
         eq_(r.status_code, OK)
         self.assertNotRegexpMatches(r.text, 'error code')
         eq_(r.url, urljoin(server.base_url, check_next))
         if self.check_userlog:
-            expected = {'event': 'login', 'uri': self.url[len(server.base_url) :], 'user': args[0]}
+            expected = {
+                'event': 'login',
+                'uri': self.url[len(server.base_url) :],
+                'user': args[0],
+                'request.method': 'POST',
+            }
             ok_(expected.items() <= self.last_userlog().items())
 
     def logout_ok(self, *args, **kwargs):
         check_next = kwargs.pop('check_next')
         # logout() does not accept user, password. So Just pass the kwargs
         r = self.logout(**kwargs)
         eq_(r.status_code, OK)
```

### Comparing `gramex-1.89.2/tests/test_cache.py` & `gramex-1.90.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_capturehandler.py` & `gramex-1.90.0/tests/test_capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_comichandler.py` & `gramex-1.90.0/tests/test_comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_drivehandler.py` & `gramex-1.90.0/tests/test_drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_filehandler.py` & `gramex-1.90.0/tests/test_filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_filterhandler.py` & `gramex-1.90.0/tests/test_filterhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_formhandler.py` & `gramex-1.90.0/tests/test_formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_functionhandler.py` & `gramex-1.90.0/tests/test_functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_gramexlog.py` & `gramex-1.90.0/tests/test_gramexlog.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_handlers.py` & `gramex-1.90.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_init.py` & `gramex-1.90.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_install.py` & `gramex-1.90.0/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_jsonhandler.py` & `gramex-1.90.0/tests/test_jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_ldapauth.py` & `gramex-1.90.0/tests/test_ldapauth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_logviewer.py` & `gramex-1.90.0/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_mlhandler.py` & `gramex-1.90.0/tests/test_mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_modelhandler.py` & `gramex-1.90.0/tests/test_modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_openapihandler.py` & `gramex-1.90.0/tests/test_openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_pptxhandler.py` & `gramex-1.90.0/tests/test_pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_processhandler.py` & `gramex-1.90.0/tests/test_processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_proxyhandler.py` & `gramex-1.90.0/tests/test_proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_pynode.py` & `gramex-1.90.0/tests/test_pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_schedule.py` & `gramex-1.90.0/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_secrets.py` & `gramex-1.90.0/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_subprocess.py` & `gramex-1.90.0/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_translater.py` & `gramex-1.90.0/tests/test_translater.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_twitterresthandler.py` & `gramex-1.90.0/tests/test_twitterresthandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_ui.py` & `gramex-1.90.0/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_update.py` & `gramex-1.90.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_uploadhandler.py` & `gramex-1.90.0/tests/test_uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_watcher.py` & `gramex-1.90.0/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.2/tests/test_websockethandler.py` & `gramex-1.90.0/tests/test_websockethandler.py`

 * *Files identical despite different names*

