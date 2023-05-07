# Comparing `tmp/pkglog-1.8.tar.gz` & `tmp/pkglog-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkglog-1.8.tar", last modified: Wed Aug 10 04:56:14 2022, max compression
+gzip compressed data, was "pkglog-1.9.tar", last modified: Tue Oct 11 06:03:13 2022, max compression
```

## Comparing `pkglog-1.8.tar` & `pkglog-1.9.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-08-10 04:56:14.438894 pkglog-1.8/
--rw-r--r--   0 mark      (1000) mark      (1000)       89 2022-02-24 22:37:47.000000 pkglog-1.8/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       56 2019-12-12 13:46:56.000000 pkglog-1.8/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      617 2022-07-02 02:32:37.000000 pkglog-1.8/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)     9524 2022-08-10 04:56:14.435561 pkglog-1.8/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     9151 2022-07-10 05:54:23.000000 pkglog-1.8/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-08-10 04:56:14.435561 pkglog-1.8/pkglog/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:49:59.000000 pkglog-1.8/pkglog/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       66 2022-07-01 07:52:12.000000 pkglog-1.8/pkglog/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-08-10 04:56:14.435561 pkglog-1.8/pkglog/parsers/
--rw-r--r--   0 mark      (1000) mark      (1000)     1077 2021-01-17 23:13:26.000000 pkglog-1.8/pkglog/parsers/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1096 2021-01-18 01:26:09.000000 pkglog-1.8/pkglog/parsers/dnf.py
--rw-r--r--   0 mark      (1000) mark      (1000)      563 2021-01-18 02:40:45.000000 pkglog-1.8/pkglog/parsers/pacman.py
--rw-r--r--   0 mark      (1000) mark      (1000)     9118 2022-08-10 01:37:05.000000 pkglog-1.8/pkglog/pkglog.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-08-10 04:56:14.435561 pkglog-1.8/pkglog.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     9524 2022-08-10 04:56:14.000000 pkglog-1.8/pkglog.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      352 2022-08-10 04:56:14.000000 pkglog-1.8/pkglog.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-08-10 04:56:14.000000 pkglog-1.8/pkglog.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       46 2022-08-10 04:56:14.000000 pkglog-1.8/pkglog.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        5 2022-08-10 04:56:14.000000 pkglog-1.8/pkglog.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       22 2022-08-10 04:56:14.000000 pkglog-1.8/pkglog.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2022-08-10 04:56:14.438894 pkglog-1.8/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1047 2022-08-10 04:54:40.000000 pkglog-1.8/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-11 06:03:13.233339 pkglog-1.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)     9753 2022-10-11 06:03:13.233339 pkglog-1.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     9396 2022-10-11 05:37:14.000000 pkglog-1.9/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-11 06:03:13.233339 pkglog-1.9/pkglog/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:49:59.000000 pkglog-1.9/pkglog/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       66 2022-07-01 07:52:12.000000 pkglog-1.9/pkglog/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-11 06:03:13.233339 pkglog-1.9/pkglog/parsers/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1077 2021-01-17 23:13:26.000000 pkglog-1.9/pkglog/parsers/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1096 2021-01-18 01:26:09.000000 pkglog-1.9/pkglog/parsers/dnf.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      563 2021-01-18 02:40:45.000000 pkglog-1.9/pkglog/parsers/pacman.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     9357 2022-10-11 05:52:35.000000 pkglog-1.9/pkglog/pkglog.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-11 06:03:13.233339 pkglog-1.9/pkglog.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     9753 2022-10-11 06:03:13.000000 pkglog-1.9/pkglog.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      324 2022-10-11 06:03:13.000000 pkglog-1.9/pkglog.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-10-11 06:03:13.000000 pkglog-1.9/pkglog.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2022-10-11 06:03:13.000000 pkglog-1.9/pkglog.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        5 2022-10-11 06:03:13.000000 pkglog-1.9/pkglog.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       22 2022-10-11 06:03:13.000000 pkglog-1.9/pkglog.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2022-10-11 06:03:13.233339 pkglog-1.9/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1051 2022-10-11 05:59:03.000000 pkglog-1.9/setup.py
```

### Comparing `pkglog-1.8/PKG-INFO` & `pkglog-1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,62 @@
-Metadata-Version: 2.1
-Name: pkglog
-Version: 1.8
-Summary: Reports log of package updates
-Home-page: https://github.com/bulletmark/pkglog
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
-License: GPLv3
-Keywords: pacman apt
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 ## PKGLOG - Linux utility to output list of changed packages
 [![PyPi](https://img.shields.io/pypi/v/pkglog)](https://pypi.org/project/pkglog/)
 [![AUR](https://img.shields.io/aur/version/pkglog)](https://aur.archlinux.org/packages/pkglog/)
 
 This is a Linux command line utility to output a list of packages
 installed, removed, upgraded, or downgraded. It should be able to parse
 the package log formats used by the common Linux distributions. Example
-output is:
+output is shown below (although it is displayed with colored lines
+in most terminals, just not here in the text README).
 
-    $ pkglog
-    ---------------------------------------------------------------------------------
-    2021-01-15 10:52:18 alsa-card-profiles   14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 libpulse             14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 pulseaudio           14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 mutter               3.38.2+7+gfbb9a34f2-1 -> 3.38.3-1
-    2021-01-15 10:52:18 pulseaudio-bluetooth 14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 gnome-shell          1:3.38.2+22+g3a343a8aa-1 -> 1:3.38.3-1
-    --------------------------------------------------------------------------------
-    2021-01-15 16:16:26 gridsome-cli 0.3.3-1 removed
-    --------------------------------------------------------------------------------
-    2021-01-16 07:11:33 httpie                2.3.0-3 -> 2.3.0-4
-    2021-01-16 07:11:33 nodejs                15.5.1-1 -> 15.6.0-1
-    2021-01-16 07:11:33 glib2                 2.66.4-1 -> 2.66.4-2
-    2021-01-16 07:11:33 glib2-docs            2.66.4-1 -> 2.66.4-2
-    2021-01-16 07:11:33 gtk-update-icon-cache 1:4.0.1-1 -> 1:4.0.1-2
-    2021-01-16 07:11:33 qt5-base              5.15.2-2 -> 5.15.2-3
-    2021-01-16 07:11:33 kdiagram              2.7.0-1 -> 2.8.0-1
-    ---------------------------------------------------------------------------------
-    2021-01-17 07:13:15 nano         5.4-1 -> 5.5-1
-    2021-01-17 07:13:15 mesa         20.3.2-2 -> 20.3.3-1
-    2021-01-17 07:13:15 rav1e        0.3.5-1 -> 0.4.0-1
-    2021-01-17 07:13:15 tk           8.6.11-1 -> 8.6.11.1-1
-    2021-01-17 07:13:15 vulkan-intel 20.3.2-2 -> 20.3.3-1
-    ---------------------------------------------------------------------------------
-    2021-01-18 06:51:45 perl-datetime-timezone      2.35-2 -> 2.44-1
-    2021-01-18 06:51:46 python-h11                  0.11.0-1 -> 0.12.0-1
-    2021-01-18 06:51:46 python-pkginfo              1.6.1-3 -> 1.7.0-1
-    2021-01-18 06:51:46 alsa-card-profiles          14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 imagemagick                 7.0.10.57-1 -> 7.0.10.58-1
-    2021-01-18 06:51:46 libbytesize                 2.4-3 -> 2.4-4
-    2021-01-18 06:51:46 libblockdev                 2.24-3 -> 2.25-1
-    2021-01-18 06:51:46 libibus                     1.5.23+3+gaa558de8-2 -> 1.5.23+3+gaa558de8-3
-    2021-01-18 06:51:46 libmm-glib                  1.14.8-1 -> 1.14.10-1
-    2021-01-18 06:51:46 libpulse                    14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 modemmanager                1.14.8-1 -> 1.14.10-1
-    2021-01-18 06:51:46 pulseaudio                  14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 pulseaudio-bluetooth        14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 python-urllib3              1.26.1-1 -> 1.26.2-1
-    ---------------------------------------------------------------------------------
-    2021-01-18 07:21:10 ### LAST SYSTEM BOOT ###
-    ---------------------------------------------------------------------------------
-    2021-01-18 07:57:48 tree 1.8.0-2 installed
+```
+$ pkglog
+---------------------------------------------------------------------------------
+2021-01-15 10:52:18 alsa-card-profiles   14.1-1 -> 14.1-2
+2021-01-15 10:52:18 libpulse             14.1-1 -> 14.1-2
+2021-01-15 10:52:18 pulseaudio           14.1-1 -> 14.1-2
+2021-01-15 10:52:18 mutter               3.38.2+7+gfbb9a34f2-1 -> 3.38.3-1
+2021-01-15 10:52:18 pulseaudio-bluetooth 14.1-1 -> 14.1-2
+2021-01-15 10:52:18 gnome-shell          1:3.38.2+22+g3a343a8aa-1 -> 1:3.38.3-1
+--------------------------------------------------------------------------------
+2021-01-15 16:16:26 gridsome-cli 0.3.3-1 removed
+--------------------------------------------------------------------------------
+2021-01-16 07:11:33 httpie                2.3.0-3 -> 2.3.0-4
+2021-01-16 07:11:33 nodejs                15.5.1-1 -> 15.6.0-1
+2021-01-16 07:11:33 glib2                 2.66.4-1 -> 2.66.4-2
+2021-01-16 07:11:33 glib2-docs            2.66.4-1 -> 2.66.4-2
+2021-01-16 07:11:33 gtk-update-icon-cache 1:4.0.1-1 -> 1:4.0.1-2
+2021-01-16 07:11:33 qt5-base              5.15.2-2 -> 5.15.2-3
+2021-01-16 07:11:33 kdiagram              2.7.0-1 -> 2.8.0-1
+---------------------------------------------------------------------------------
+2021-01-17 07:13:15 nano         5.4-1 -> 5.5-1
+2021-01-17 07:13:15 mesa         20.3.2-2 -> 20.3.3-1
+2021-01-17 07:13:15 rav1e        0.3.5-1 -> 0.4.0-1
+2021-01-17 07:13:15 tk           8.6.11-1 -> 8.6.11.1-1
+2021-01-17 07:13:15 vulkan-intel 20.3.2-2 -> 20.3.3-1
+---------------------------------------------------------------------------------
+2021-01-18 06:51:45 perl-datetime-timezone      2.35-2 -> 2.44-1
+2021-01-18 06:51:46 python-h11                  0.11.0-1 -> 0.12.0-1
+2021-01-18 06:51:46 python-pkginfo              1.6.1-3 -> 1.7.0-1
+2021-01-18 06:51:46 alsa-card-profiles          14.1-2 -> 14.2-1
+2021-01-18 06:51:46 imagemagick                 7.0.10.57-1 -> 7.0.10.58-1
+2021-01-18 06:51:46 libbytesize                 2.4-3 -> 2.4-4
+2021-01-18 06:51:46 libblockdev                 2.24-3 -> 2.25-1
+2021-01-18 06:51:46 libibus                     1.5.23+3+gaa558de8-2 -> 1.5.23+3+gaa558de8-3
+2021-01-18 06:51:46 libmm-glib                  1.14.8-1 -> 1.14.10-1
+2021-01-18 06:51:46 libpulse                    14.1-2 -> 14.2-1
+2021-01-18 06:51:46 modemmanager                1.14.8-1 -> 1.14.10-1
+2021-01-18 06:51:46 pulseaudio                  14.1-2 -> 14.2-1
+2021-01-18 06:51:46 pulseaudio-bluetooth        14.1-2 -> 14.2-1
+2021-01-18 06:51:46 python-urllib3              1.26.1-1 -> 1.26.2-1
+---------------------------------------------------------------------------------
+2021-01-18 07:21:10 ### LAST SYSTEM BOOT ###
+---------------------------------------------------------------------------------
+2021-01-18 07:57:48 tree 1.8.0-2 installed
+```
 
 1. By default, only package updates over the last 30 days are shown. You
    can choose to specify a specific date, or number of days back, or for
    all time.
 
 2. Updates are grouped together by time (all updates with less than a 2
    minute gap between any of them) so you can distinguish the group of
@@ -78,26 +67,39 @@
    since updated you may decide to reboot asap. In the above example,
    only the `tree` package has been installed since the last boot.
 
 4. You can specify a package name and only updates to that package are
    shown. See the USAGE section below.
 
 5. Most terminals show this output in color. Five different colors are
-   used to identify _installed_, _removed_, _upgraded_, _downgraded_, or
-   _reinstalled_ lines. You can choose to disable colored output.
+   used to identify the package actions as shown below.
+   You can choose to disable colored output.
 
 6. You can use the `-n/--installed-net` option to see a list of all
    packages currently installed and their date of installation. E.g. use
    this option after you have installed and removed a heap of trial
    packages and you want to easily see if you have actually removed all
    of them.
 
 See the latest documentation and code at https://github.com/bulletmark/pkglog.
 
-### LOG FILE FORMATS
+## COLORED OUTPUT LINES
+
+|Package Action|Line Text Color
+|--------------|-----
+|Installed     |green
+|Removed       |red
+|Upgraded      |yellow
+|Downgraded    |magenta
+|Reinstalled   |cyan
+
+You can use a command line option to disable colored output, or set it
+as a [default option](#default-options).
+
+## LOG FILE FORMATS
 
 Parsers for the following log formats currently exist. The appropriate
 parser for you system is normally automatically determined.
 Alternatively, you can choose the log directory[s], file[s], and/or
 parser explicitly using the `-p/--parser` option. A very simple parser
 plugin architecture is used, so creating a new parser is easy. Simply
 drop the parser file in the `parsers/` directory and the program will
@@ -106,20 +108,22 @@
 
 |Log Parser|Default Path           |Systems            |
 |----------|-----------------------|-------------------|
 |apt       |`/var/log/apt/history*`|Debian, Ubuntu, etc|
 |dnf       |`/var/log/dnf.rpm.log` |RedHat, Fedora, etc|
 |pacman    |`/var/log/pacman.log`  |Arch, Manjaro, etc |
 
-### USAGE
+## USAGE
+
+Type `pkglog -h` to view the usage summary:
 
 ```
 usage: pkglog [-h] [-u] [-i] [-I] [-n] [-d DAYS] [-a] [-j] [-v] [-c]
-              [-p {pacman,apt,dnf}] [-t TIMEGAP] [-P PATH] [-g | -r]
-              [package]
+                   [-p {pacman,apt,dnf}] [-t TIMEGAP] [-P PATH] [-g | -r]
+                   [package]
 
 Reports log of package updates.
 
 positional arguments:
   package               specific package name to report
 
 options:
@@ -139,32 +143,32 @@
   -t TIMEGAP, --timegap TIMEGAP
                         max minutes gap between grouped updates, default=2
   -P PATH, --path PATH  alternate log path[s] (separate multiple using ":",
                         must be time sequenced)
   -g, --glob            given package name is glob pattern to match
   -r, --regex           given package name is regular expression to match
 
-Note you can set default starting arguments in ~/.config/pkglog-flags.conf.
+Note you can set default starting options in ~/.config/pkglog-flags.conf.
 ```
 
-### DEFAULT ARGUMENTS
+## DEFAULT OPTIONS
 
-You can add default arguments to a personal configuration file
+You can add default options to a personal configuration file
 `~/.config/pkglog-flags.conf`. If that file exists then each line of
-arguments in the file will be concatenated and automatically prepended
-to your `pkglog` command line arguments.
+options in the file will be concatenated and automatically prepended
+to your `pkglog` command line options.
 
-This allow you to set default preferred starting arguments to `pkglog`.
-Type `pkglog -h` to see the arguments supported.
+This allow you to set default preferred starting options to `pkglog`.
+Type `pkglog -h` to see the options supported.
 E.g. `echo "--days 7" >~/.config/pkglog-flags.conf` to make `pkglog`
 only display the last 7 days of updates by default. This is also useful
 to set your parser explicitly using `-p/--parser` (e.g. if the default
 parser is not automatically determined correctly on your system).
 
-### INSTALLATION
+## INSTALLATION
 
 Arch Linux users can install [pkglog from the
 AUR](https://aur.archlinux.org/packages/pkglog). Python 3.7 or later is
 required. The [`python-rich`](https://pypi.org/project/rich/) package is
 required if you want colored output (which is the default unless you
 specify the `-c/--no-color` option).
 
@@ -180,35 +184,33 @@
 
 ```sh
 $ git clone http://github.com/bulletmark/pkglog
 $ cd pkglog
 $ sudo pip3 install -U .
 ```
 
-### UPGRADE
+## UPGRADE
 
 ```sh
 $ cd pkglog  # Source dir, as above
 $ git pull
 $ sudo pip3 install -U .
 ```
 
-### REMOVAL
+## REMOVAL
 
 ```sh
 $ sudo pip3 uninstall pkglog
 ```
 
-### LICENSE
+## LICENSE
 
 Copyright (C) 2020 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
 under the terms of the GNU General Public License as published by the
 Free Software Foundation, either version 3 of the License, or any later
 version.
 This program is distributed in the hope that it will be useful, but
 WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
 Public License at <http://www.gnu.org/licenses/> for more details.
-
-
```

### Comparing `pkglog-1.8/README.md` & `pkglog-1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,75 @@
+Metadata-Version: 2.1
+Name: pkglog
+Version: 1.9
+Summary: Reports log of package updates
+Home-page: https://github.com/bulletmark/pkglog
+Author: Mark Blakeney
+Author-email: mark.blakeney@bullet-systems.net
+License: GPLv3
+Keywords: pacman apt dnf
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 ## PKGLOG - Linux utility to output list of changed packages
 [![PyPi](https://img.shields.io/pypi/v/pkglog)](https://pypi.org/project/pkglog/)
 [![AUR](https://img.shields.io/aur/version/pkglog)](https://aur.archlinux.org/packages/pkglog/)
 
 This is a Linux command line utility to output a list of packages
 installed, removed, upgraded, or downgraded. It should be able to parse
 the package log formats used by the common Linux distributions. Example
-output is:
+output is shown below (although it is displayed with colored lines
+in most terminals, just not here in the text README).
 
-    $ pkglog
-    ---------------------------------------------------------------------------------
-    2021-01-15 10:52:18 alsa-card-profiles   14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 libpulse             14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 pulseaudio           14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 mutter               3.38.2+7+gfbb9a34f2-1 -> 3.38.3-1
-    2021-01-15 10:52:18 pulseaudio-bluetooth 14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 gnome-shell          1:3.38.2+22+g3a343a8aa-1 -> 1:3.38.3-1
-    --------------------------------------------------------------------------------
-    2021-01-15 16:16:26 gridsome-cli 0.3.3-1 removed
-    --------------------------------------------------------------------------------
-    2021-01-16 07:11:33 httpie                2.3.0-3 -> 2.3.0-4
-    2021-01-16 07:11:33 nodejs                15.5.1-1 -> 15.6.0-1
-    2021-01-16 07:11:33 glib2                 2.66.4-1 -> 2.66.4-2
-    2021-01-16 07:11:33 glib2-docs            2.66.4-1 -> 2.66.4-2
-    2021-01-16 07:11:33 gtk-update-icon-cache 1:4.0.1-1 -> 1:4.0.1-2
-    2021-01-16 07:11:33 qt5-base              5.15.2-2 -> 5.15.2-3
-    2021-01-16 07:11:33 kdiagram              2.7.0-1 -> 2.8.0-1
-    ---------------------------------------------------------------------------------
-    2021-01-17 07:13:15 nano         5.4-1 -> 5.5-1
-    2021-01-17 07:13:15 mesa         20.3.2-2 -> 20.3.3-1
-    2021-01-17 07:13:15 rav1e        0.3.5-1 -> 0.4.0-1
-    2021-01-17 07:13:15 tk           8.6.11-1 -> 8.6.11.1-1
-    2021-01-17 07:13:15 vulkan-intel 20.3.2-2 -> 20.3.3-1
-    ---------------------------------------------------------------------------------
-    2021-01-18 06:51:45 perl-datetime-timezone      2.35-2 -> 2.44-1
-    2021-01-18 06:51:46 python-h11                  0.11.0-1 -> 0.12.0-1
-    2021-01-18 06:51:46 python-pkginfo              1.6.1-3 -> 1.7.0-1
-    2021-01-18 06:51:46 alsa-card-profiles          14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 imagemagick                 7.0.10.57-1 -> 7.0.10.58-1
-    2021-01-18 06:51:46 libbytesize                 2.4-3 -> 2.4-4
-    2021-01-18 06:51:46 libblockdev                 2.24-3 -> 2.25-1
-    2021-01-18 06:51:46 libibus                     1.5.23+3+gaa558de8-2 -> 1.5.23+3+gaa558de8-3
-    2021-01-18 06:51:46 libmm-glib                  1.14.8-1 -> 1.14.10-1
-    2021-01-18 06:51:46 libpulse                    14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 modemmanager                1.14.8-1 -> 1.14.10-1
-    2021-01-18 06:51:46 pulseaudio                  14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 pulseaudio-bluetooth        14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 python-urllib3              1.26.1-1 -> 1.26.2-1
-    ---------------------------------------------------------------------------------
-    2021-01-18 07:21:10 ### LAST SYSTEM BOOT ###
-    ---------------------------------------------------------------------------------
-    2021-01-18 07:57:48 tree 1.8.0-2 installed
+```
+$ pkglog
+---------------------------------------------------------------------------------
+2021-01-15 10:52:18 alsa-card-profiles   14.1-1 -> 14.1-2
+2021-01-15 10:52:18 libpulse             14.1-1 -> 14.1-2
+2021-01-15 10:52:18 pulseaudio           14.1-1 -> 14.1-2
+2021-01-15 10:52:18 mutter               3.38.2+7+gfbb9a34f2-1 -> 3.38.3-1
+2021-01-15 10:52:18 pulseaudio-bluetooth 14.1-1 -> 14.1-2
+2021-01-15 10:52:18 gnome-shell          1:3.38.2+22+g3a343a8aa-1 -> 1:3.38.3-1
+--------------------------------------------------------------------------------
+2021-01-15 16:16:26 gridsome-cli 0.3.3-1 removed
+--------------------------------------------------------------------------------
+2021-01-16 07:11:33 httpie                2.3.0-3 -> 2.3.0-4
+2021-01-16 07:11:33 nodejs                15.5.1-1 -> 15.6.0-1
+2021-01-16 07:11:33 glib2                 2.66.4-1 -> 2.66.4-2
+2021-01-16 07:11:33 glib2-docs            2.66.4-1 -> 2.66.4-2
+2021-01-16 07:11:33 gtk-update-icon-cache 1:4.0.1-1 -> 1:4.0.1-2
+2021-01-16 07:11:33 qt5-base              5.15.2-2 -> 5.15.2-3
+2021-01-16 07:11:33 kdiagram              2.7.0-1 -> 2.8.0-1
+---------------------------------------------------------------------------------
+2021-01-17 07:13:15 nano         5.4-1 -> 5.5-1
+2021-01-17 07:13:15 mesa         20.3.2-2 -> 20.3.3-1
+2021-01-17 07:13:15 rav1e        0.3.5-1 -> 0.4.0-1
+2021-01-17 07:13:15 tk           8.6.11-1 -> 8.6.11.1-1
+2021-01-17 07:13:15 vulkan-intel 20.3.2-2 -> 20.3.3-1
+---------------------------------------------------------------------------------
+2021-01-18 06:51:45 perl-datetime-timezone      2.35-2 -> 2.44-1
+2021-01-18 06:51:46 python-h11                  0.11.0-1 -> 0.12.0-1
+2021-01-18 06:51:46 python-pkginfo              1.6.1-3 -> 1.7.0-1
+2021-01-18 06:51:46 alsa-card-profiles          14.1-2 -> 14.2-1
+2021-01-18 06:51:46 imagemagick                 7.0.10.57-1 -> 7.0.10.58-1
+2021-01-18 06:51:46 libbytesize                 2.4-3 -> 2.4-4
+2021-01-18 06:51:46 libblockdev                 2.24-3 -> 2.25-1
+2021-01-18 06:51:46 libibus                     1.5.23+3+gaa558de8-2 -> 1.5.23+3+gaa558de8-3
+2021-01-18 06:51:46 libmm-glib                  1.14.8-1 -> 1.14.10-1
+2021-01-18 06:51:46 libpulse                    14.1-2 -> 14.2-1
+2021-01-18 06:51:46 modemmanager                1.14.8-1 -> 1.14.10-1
+2021-01-18 06:51:46 pulseaudio                  14.1-2 -> 14.2-1
+2021-01-18 06:51:46 pulseaudio-bluetooth        14.1-2 -> 14.2-1
+2021-01-18 06:51:46 python-urllib3              1.26.1-1 -> 1.26.2-1
+---------------------------------------------------------------------------------
+2021-01-18 07:21:10 ### LAST SYSTEM BOOT ###
+---------------------------------------------------------------------------------
+2021-01-18 07:57:48 tree 1.8.0-2 installed
+```
 
 1. By default, only package updates over the last 30 days are shown. You
    can choose to specify a specific date, or number of days back, or for
    all time.
 
 2. Updates are grouped together by time (all updates with less than a 2
    minute gap between any of them) so you can distinguish the group of
@@ -64,26 +80,39 @@
    since updated you may decide to reboot asap. In the above example,
    only the `tree` package has been installed since the last boot.
 
 4. You can specify a package name and only updates to that package are
    shown. See the USAGE section below.
 
 5. Most terminals show this output in color. Five different colors are
-   used to identify _installed_, _removed_, _upgraded_, _downgraded_, or
-   _reinstalled_ lines. You can choose to disable colored output.
+   used to identify the package actions as shown below.
+   You can choose to disable colored output.
 
 6. You can use the `-n/--installed-net` option to see a list of all
    packages currently installed and their date of installation. E.g. use
    this option after you have installed and removed a heap of trial
    packages and you want to easily see if you have actually removed all
    of them.
 
 See the latest documentation and code at https://github.com/bulletmark/pkglog.
 
-### LOG FILE FORMATS
+## COLORED OUTPUT LINES
+
+|Package Action|Line Text Color
+|--------------|-----
+|Installed     |green
+|Removed       |red
+|Upgraded      |yellow
+|Downgraded    |magenta
+|Reinstalled   |cyan
+
+You can use a command line option to disable colored output, or set it
+as a [default option](#default-options).
+
+## LOG FILE FORMATS
 
 Parsers for the following log formats currently exist. The appropriate
 parser for you system is normally automatically determined.
 Alternatively, you can choose the log directory[s], file[s], and/or
 parser explicitly using the `-p/--parser` option. A very simple parser
 plugin architecture is used, so creating a new parser is easy. Simply
 drop the parser file in the `parsers/` directory and the program will
@@ -92,20 +121,22 @@
 
 |Log Parser|Default Path           |Systems            |
 |----------|-----------------------|-------------------|
 |apt       |`/var/log/apt/history*`|Debian, Ubuntu, etc|
 |dnf       |`/var/log/dnf.rpm.log` |RedHat, Fedora, etc|
 |pacman    |`/var/log/pacman.log`  |Arch, Manjaro, etc |
 
-### USAGE
+## USAGE
+
+Type `pkglog -h` to view the usage summary:
 
 ```
 usage: pkglog [-h] [-u] [-i] [-I] [-n] [-d DAYS] [-a] [-j] [-v] [-c]
-              [-p {pacman,apt,dnf}] [-t TIMEGAP] [-P PATH] [-g | -r]
-              [package]
+                   [-p {pacman,apt,dnf}] [-t TIMEGAP] [-P PATH] [-g | -r]
+                   [package]
 
 Reports log of package updates.
 
 positional arguments:
   package               specific package name to report
 
 options:
@@ -125,32 +156,32 @@
   -t TIMEGAP, --timegap TIMEGAP
                         max minutes gap between grouped updates, default=2
   -P PATH, --path PATH  alternate log path[s] (separate multiple using ":",
                         must be time sequenced)
   -g, --glob            given package name is glob pattern to match
   -r, --regex           given package name is regular expression to match
 
-Note you can set default starting arguments in ~/.config/pkglog-flags.conf.
+Note you can set default starting options in ~/.config/pkglog-flags.conf.
 ```
 
-### DEFAULT ARGUMENTS
+## DEFAULT OPTIONS
 
-You can add default arguments to a personal configuration file
+You can add default options to a personal configuration file
 `~/.config/pkglog-flags.conf`. If that file exists then each line of
-arguments in the file will be concatenated and automatically prepended
-to your `pkglog` command line arguments.
+options in the file will be concatenated and automatically prepended
+to your `pkglog` command line options.
 
-This allow you to set default preferred starting arguments to `pkglog`.
-Type `pkglog -h` to see the arguments supported.
+This allow you to set default preferred starting options to `pkglog`.
+Type `pkglog -h` to see the options supported.
 E.g. `echo "--days 7" >~/.config/pkglog-flags.conf` to make `pkglog`
 only display the last 7 days of updates by default. This is also useful
 to set your parser explicitly using `-p/--parser` (e.g. if the default
 parser is not automatically determined correctly on your system).
 
-### INSTALLATION
+## INSTALLATION
 
 Arch Linux users can install [pkglog from the
 AUR](https://aur.archlinux.org/packages/pkglog). Python 3.7 or later is
 required. The [`python-rich`](https://pypi.org/project/rich/) package is
 required if you want colored output (which is the default unless you
 specify the `-c/--no-color` option).
 
@@ -166,29 +197,29 @@
 
 ```sh
 $ git clone http://github.com/bulletmark/pkglog
 $ cd pkglog
 $ sudo pip3 install -U .
 ```
 
-### UPGRADE
+## UPGRADE
 
 ```sh
 $ cd pkglog  # Source dir, as above
 $ git pull
 $ sudo pip3 install -U .
 ```
 
-### REMOVAL
+## REMOVAL
 
 ```sh
 $ sudo pip3 uninstall pkglog
 ```
 
-### LICENSE
+## LICENSE
 
 Copyright (C) 2020 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
 under the terms of the GNU General Public License as published by the
 Free Software Foundation, either version 3 of the License, or any later
 version.
```

### Comparing `pkglog-1.8/pkglog/parsers/apt.py` & `pkglog-1.9/pkglog/parsers/apt.py`

 * *Files identical despite different names*

### Comparing `pkglog-1.8/pkglog/parsers/dnf.py` & `pkglog-1.9/pkglog/parsers/dnf.py`

 * *Files identical despite different names*

### Comparing `pkglog-1.8/pkglog/parsers/pacman.py` & `pkglog-1.9/pkglog/parsers/pacman.py`

 * *Files identical despite different names*

### Comparing `pkglog-1.8/pkglog/pkglog.py` & `pkglog-1.9/pkglog/pkglog.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 'Reports log of package updates.'
 # Author: Mark Blakeney, 2016->2021.
 
 import os
 import sys
 import re
 import argparse
-from importlib import util, machinery
 import fileinput
 import shlex
 import fnmatch
+from importlib import util, machinery
 from datetime import datetime, date, timedelta
 from pathlib import Path
 
 TIMEGAP = 2  # mins
 PATHSEP = ':'
 
 DAYS = 30
@@ -30,17 +30,31 @@
 CNFFILE = Path(os.getenv('XDG_CONFIG_HOME', '~/.config'),
         f'{MODDIR.name}-flags.conf')
 
 class Queue:
     queue = []
     installed = {}
     console = None
+    boottime = None
+    bootstr = None
+    delim = None
 
     @classmethod
-    def output(cls, args, delim):
+    def print(cls, color, *msg):
+        'Output given message'
+        for m in msg:
+            if m:
+                if cls.console:
+                    cls.console.print(m, style=(color or 'white'),
+                                      highlight=False)
+                else:
+                    print(m)
+
+    @classmethod
+    def output(cls, args):
         'Output queued set of package transactions to screen'
         if not cls.queue:
             return
 
         out = []
         maxlen = 1
 
@@ -68,36 +82,34 @@
                     continue
             if actcode != 3 or args.verbose:
                 vers += ' ' + action
             out.append((dt, pkg, vers, color))
             if not args.nojustify:
                 maxlen = max(maxlen, len(pkg))
 
-        if out:
-            if delim is not None:
-                print(delim)
-
-            # Now output justified lines to screen
-            for dt, pkg, vers, color in out:
-                msg = f'{dt} {pkg:{maxlen}} {vers}'
-                if cls.console:
-                    cls.console.print(msg, style=color, highlight=False)
-                else:
-                    print(msg)
+        # Now output justified lines to screen
+        for num, (dt, pkg, vers, color) in enumerate(out):
+            if cls.bootstr and dt > cls.boottime:
+                cls.print(None, cls.delim, cls.bootstr, cls.delim)
+                cls.bootstr = None
+            elif num == 0:
+                cls.print(None, cls.delim)
+
+            cls.print(color, f'{dt} {pkg:{maxlen}} {vers}')
 
         cls.queue.clear()
 
     @classmethod
     def append(cls, dt, action, pkg, vers):
         'Append this package + action to the internal queue'
         actcode, _ = ACTIONS[action]
         if actcode == 1:
             cls.installed[pkg] = dt
-        elif actcode == 2 and pkg in cls.installed:
-            del cls.installed[pkg]
+        elif actcode == 2:
+            cls.installed.pop(pkg, None)
 
         cls.queue.append((dt, action, pkg, vers))
 
 def import_path(path):
     'Import given module path'
     modname = path.stem.replace('-', '_')
     spec = util.spec_from_loader(modname,
@@ -125,15 +137,15 @@
         if Path(parsers[parser].logfile).exists():
             break
     else:
         parser = '?'
 
     # Process command line options
     opt = argparse.ArgumentParser(description=__doc__.strip(),
-            epilog=f'Note you can set default starting arguments in {CNFFILE}.')
+            epilog=f'Note you can set default starting options in {CNFFILE}.')
     opt.add_argument('-u', '--updated-only', action='store_true',
             help='show updated only')
     opt.add_argument('-i', '--installed', action='store_true',
             help='show installed/removed only')
     opt.add_argument('-I', '--installed-only', action='store_true',
             help='show installed only')
     opt.add_argument('-n', '--installed-net', action='store_true',
@@ -150,38 +162,42 @@
     opt.add_argument('-c', '--no-color', action='store_true',
             help='do not color output lines')
     opt.add_argument('-p', '--parser', choices=parsers,
             help=f'log parser type, default={parser}')
     opt.add_argument('-t', '--timegap', type=float, default=TIMEGAP,
             help=f'max minutes gap between grouped updates, default={TIMEGAP}')
     opt.add_argument('-P', '--path',
-            help='alternate log path[s] (separate multiple using "{}", '
-            'must be time sequenced)'.format(PATHSEP))
+            help='alternate log path[s] '
+            f'(separate multiple using "{PATHSEP}", must be time sequenced)')
     grp = opt.add_mutually_exclusive_group()
     grp.add_argument('-g', '--glob', action='store_true',
             help='given package name is glob pattern to match')
     grp.add_argument('-r', '--regex', action='store_true',
             help='given package name is regular expression to match')
     opt.add_argument('package', nargs='?',
             help='specific package name to report')
 
-    # Merge in default args from user config file. Then parse the
+    # Merge in default options from user config file. Then parse the
     # command line.
     cnflines = ''
     cnffile = CNFFILE.expanduser()
     if cnffile.exists():
         with cnffile.open() as fp:
             cnflines = [re.sub(r'#.*$', '', line).strip() for line in fp]
         cnflines = ' '.join(cnflines).strip()
 
     args = opt.parse_args(shlex.split(cnflines) + sys.argv[1:])
 
     if not args.no_color:
-        from rich.console import Console
-        Queue.console = Console()
+        try:
+            from rich.console import Console
+        except Exception:
+            args.no_color = True
+        else:
+            Queue.console = Console()
 
     if args.parser:
         parser = args.parser
 
     if args.package:
         if args.glob:
             args.package = fnmatch.translate(args.package)
@@ -197,37 +213,33 @@
 
     logmod = parsers.get(parser)
     if not logmod:
         sys.exit('ERROR: Can not determine log parser for this system.')
 
     defpath = Path(logmod.logfile)
 
-    delim = 80 * '-' if not args.package \
-            and not (args.installed or args.installed_only) else None
+    if not args.package and not (args.installed or args.installed_only):
+        Queue.delim = 80 * '-'
 
     timegap = timedelta(minutes=args.timegap)
 
     if args.days:
         if args.days.isdigit():
             days = int(args.days)
         else:
             days = (date.today() - date.fromisoformat(args.days)).days
     else:
         days = -1 if args.package else DAYS
 
-    if args.package:
-        bootstr = None
-    else:
+    if not args.package:
         # Get last boot time
         upsecs = float(Path('/proc/uptime').read_text().split()[0])
-        timeboot = datetime.now() - timedelta(seconds=upsecs)
-        timestr = timeboot.isoformat(' ', 'seconds')
-        dline = '' if delim is None else (delim + '\n')
-
-        bootstr = f'{dline}{timestr} ### LAST SYSTEM BOOT ###'
+        Queue.boottime = datetime.now() - timedelta(seconds=upsecs)
+        timestr = Queue.boottime.isoformat(' ', 'seconds')
+        Queue.bootstr = f'{timestr} ### LAST SYSTEM BOOT ###'
 
     start_date = date.today() - timedelta(days=days) if days >= 0 and \
             not args.alldays else None
 
     dt_out = datetime.max
 
     if args.path:
@@ -252,31 +264,26 @@
                 openhook=fileinput.hook_compressed):
             line = lineb if isinstance(lineb, str) else lineb.decode()
 
             dt = logmod.get_date(line.strip())
             if not dt:
                 continue
 
-            if bootstr and dt > timeboot:
-                Queue.output(args, delim)
-                print(bootstr)
-                bootstr = None
-
             if start_date and dt.date() < start_date:
                 continue
 
             if dt - dt_out > timegap and not args.installed_net:
-                Queue.output(args, delim)
+                Queue.output(args)
 
             dt_out = dt
 
             for fields in logmod.get_packages():
                 if fields and len(fields) == 3 and fields[0] in ACTIONS:
                     Queue.append(dt, *fields)
 
     # Flush any remaining queued output
-    Queue.output(args, delim)
-    if bootstr:
-        print(bootstr)
+    Queue.output(args)
+    if Queue.bootstr:
+        Queue.print(None, Queue.delim, Queue.bootstr)
 
 if __name__ == '__main__':
     main()
```

### Comparing `pkglog-1.8/pkglog.egg-info/PKG-INFO` & `pkglog-1.9/pkglog.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 Metadata-Version: 2.1
 Name: pkglog
-Version: 1.8
+Version: 1.9
 Summary: Reports log of package updates
 Home-page: https://github.com/bulletmark/pkglog
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
-Keywords: pacman apt
-Platform: UNKNOWN
+Keywords: pacman apt dnf
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## PKGLOG - Linux utility to output list of changed packages
 [![PyPi](https://img.shields.io/pypi/v/pkglog)](https://pypi.org/project/pkglog/)
 [![AUR](https://img.shields.io/aur/version/pkglog)](https://aur.archlinux.org/packages/pkglog/)
 
 This is a Linux command line utility to output a list of packages
 installed, removed, upgraded, or downgraded. It should be able to parse
 the package log formats used by the common Linux distributions. Example
-output is:
+output is shown below (although it is displayed with colored lines
+in most terminals, just not here in the text README).
 
-    $ pkglog
-    ---------------------------------------------------------------------------------
-    2021-01-15 10:52:18 alsa-card-profiles   14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 libpulse             14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 pulseaudio           14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 mutter               3.38.2+7+gfbb9a34f2-1 -> 3.38.3-1
-    2021-01-15 10:52:18 pulseaudio-bluetooth 14.1-1 -> 14.1-2
-    2021-01-15 10:52:18 gnome-shell          1:3.38.2+22+g3a343a8aa-1 -> 1:3.38.3-1
-    --------------------------------------------------------------------------------
-    2021-01-15 16:16:26 gridsome-cli 0.3.3-1 removed
-    --------------------------------------------------------------------------------
-    2021-01-16 07:11:33 httpie                2.3.0-3 -> 2.3.0-4
-    2021-01-16 07:11:33 nodejs                15.5.1-1 -> 15.6.0-1
-    2021-01-16 07:11:33 glib2                 2.66.4-1 -> 2.66.4-2
-    2021-01-16 07:11:33 glib2-docs            2.66.4-1 -> 2.66.4-2
-    2021-01-16 07:11:33 gtk-update-icon-cache 1:4.0.1-1 -> 1:4.0.1-2
-    2021-01-16 07:11:33 qt5-base              5.15.2-2 -> 5.15.2-3
-    2021-01-16 07:11:33 kdiagram              2.7.0-1 -> 2.8.0-1
-    ---------------------------------------------------------------------------------
-    2021-01-17 07:13:15 nano         5.4-1 -> 5.5-1
-    2021-01-17 07:13:15 mesa         20.3.2-2 -> 20.3.3-1
-    2021-01-17 07:13:15 rav1e        0.3.5-1 -> 0.4.0-1
-    2021-01-17 07:13:15 tk           8.6.11-1 -> 8.6.11.1-1
-    2021-01-17 07:13:15 vulkan-intel 20.3.2-2 -> 20.3.3-1
-    ---------------------------------------------------------------------------------
-    2021-01-18 06:51:45 perl-datetime-timezone      2.35-2 -> 2.44-1
-    2021-01-18 06:51:46 python-h11                  0.11.0-1 -> 0.12.0-1
-    2021-01-18 06:51:46 python-pkginfo              1.6.1-3 -> 1.7.0-1
-    2021-01-18 06:51:46 alsa-card-profiles          14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 imagemagick                 7.0.10.57-1 -> 7.0.10.58-1
-    2021-01-18 06:51:46 libbytesize                 2.4-3 -> 2.4-4
-    2021-01-18 06:51:46 libblockdev                 2.24-3 -> 2.25-1
-    2021-01-18 06:51:46 libibus                     1.5.23+3+gaa558de8-2 -> 1.5.23+3+gaa558de8-3
-    2021-01-18 06:51:46 libmm-glib                  1.14.8-1 -> 1.14.10-1
-    2021-01-18 06:51:46 libpulse                    14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 modemmanager                1.14.8-1 -> 1.14.10-1
-    2021-01-18 06:51:46 pulseaudio                  14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 pulseaudio-bluetooth        14.1-2 -> 14.2-1
-    2021-01-18 06:51:46 python-urllib3              1.26.1-1 -> 1.26.2-1
-    ---------------------------------------------------------------------------------
-    2021-01-18 07:21:10 ### LAST SYSTEM BOOT ###
-    ---------------------------------------------------------------------------------
-    2021-01-18 07:57:48 tree 1.8.0-2 installed
+```
+$ pkglog
+---------------------------------------------------------------------------------
+2021-01-15 10:52:18 alsa-card-profiles   14.1-1 -> 14.1-2
+2021-01-15 10:52:18 libpulse             14.1-1 -> 14.1-2
+2021-01-15 10:52:18 pulseaudio           14.1-1 -> 14.1-2
+2021-01-15 10:52:18 mutter               3.38.2+7+gfbb9a34f2-1 -> 3.38.3-1
+2021-01-15 10:52:18 pulseaudio-bluetooth 14.1-1 -> 14.1-2
+2021-01-15 10:52:18 gnome-shell          1:3.38.2+22+g3a343a8aa-1 -> 1:3.38.3-1
+--------------------------------------------------------------------------------
+2021-01-15 16:16:26 gridsome-cli 0.3.3-1 removed
+--------------------------------------------------------------------------------
+2021-01-16 07:11:33 httpie                2.3.0-3 -> 2.3.0-4
+2021-01-16 07:11:33 nodejs                15.5.1-1 -> 15.6.0-1
+2021-01-16 07:11:33 glib2                 2.66.4-1 -> 2.66.4-2
+2021-01-16 07:11:33 glib2-docs            2.66.4-1 -> 2.66.4-2
+2021-01-16 07:11:33 gtk-update-icon-cache 1:4.0.1-1 -> 1:4.0.1-2
+2021-01-16 07:11:33 qt5-base              5.15.2-2 -> 5.15.2-3
+2021-01-16 07:11:33 kdiagram              2.7.0-1 -> 2.8.0-1
+---------------------------------------------------------------------------------
+2021-01-17 07:13:15 nano         5.4-1 -> 5.5-1
+2021-01-17 07:13:15 mesa         20.3.2-2 -> 20.3.3-1
+2021-01-17 07:13:15 rav1e        0.3.5-1 -> 0.4.0-1
+2021-01-17 07:13:15 tk           8.6.11-1 -> 8.6.11.1-1
+2021-01-17 07:13:15 vulkan-intel 20.3.2-2 -> 20.3.3-1
+---------------------------------------------------------------------------------
+2021-01-18 06:51:45 perl-datetime-timezone      2.35-2 -> 2.44-1
+2021-01-18 06:51:46 python-h11                  0.11.0-1 -> 0.12.0-1
+2021-01-18 06:51:46 python-pkginfo              1.6.1-3 -> 1.7.0-1
+2021-01-18 06:51:46 alsa-card-profiles          14.1-2 -> 14.2-1
+2021-01-18 06:51:46 imagemagick                 7.0.10.57-1 -> 7.0.10.58-1
+2021-01-18 06:51:46 libbytesize                 2.4-3 -> 2.4-4
+2021-01-18 06:51:46 libblockdev                 2.24-3 -> 2.25-1
+2021-01-18 06:51:46 libibus                     1.5.23+3+gaa558de8-2 -> 1.5.23+3+gaa558de8-3
+2021-01-18 06:51:46 libmm-glib                  1.14.8-1 -> 1.14.10-1
+2021-01-18 06:51:46 libpulse                    14.1-2 -> 14.2-1
+2021-01-18 06:51:46 modemmanager                1.14.8-1 -> 1.14.10-1
+2021-01-18 06:51:46 pulseaudio                  14.1-2 -> 14.2-1
+2021-01-18 06:51:46 pulseaudio-bluetooth        14.1-2 -> 14.2-1
+2021-01-18 06:51:46 python-urllib3              1.26.1-1 -> 1.26.2-1
+---------------------------------------------------------------------------------
+2021-01-18 07:21:10 ### LAST SYSTEM BOOT ###
+---------------------------------------------------------------------------------
+2021-01-18 07:57:48 tree 1.8.0-2 installed
+```
 
 1. By default, only package updates over the last 30 days are shown. You
    can choose to specify a specific date, or number of days back, or for
    all time.
 
 2. Updates are grouped together by time (all updates with less than a 2
    minute gap between any of them) so you can distinguish the group of
@@ -78,26 +80,39 @@
    since updated you may decide to reboot asap. In the above example,
    only the `tree` package has been installed since the last boot.
 
 4. You can specify a package name and only updates to that package are
    shown. See the USAGE section below.
 
 5. Most terminals show this output in color. Five different colors are
-   used to identify _installed_, _removed_, _upgraded_, _downgraded_, or
-   _reinstalled_ lines. You can choose to disable colored output.
+   used to identify the package actions as shown below.
+   You can choose to disable colored output.
 
 6. You can use the `-n/--installed-net` option to see a list of all
    packages currently installed and their date of installation. E.g. use
    this option after you have installed and removed a heap of trial
    packages and you want to easily see if you have actually removed all
    of them.
 
 See the latest documentation and code at https://github.com/bulletmark/pkglog.
 
-### LOG FILE FORMATS
+## COLORED OUTPUT LINES
+
+|Package Action|Line Text Color
+|--------------|-----
+|Installed     |green
+|Removed       |red
+|Upgraded      |yellow
+|Downgraded    |magenta
+|Reinstalled   |cyan
+
+You can use a command line option to disable colored output, or set it
+as a [default option](#default-options).
+
+## LOG FILE FORMATS
 
 Parsers for the following log formats currently exist. The appropriate
 parser for you system is normally automatically determined.
 Alternatively, you can choose the log directory[s], file[s], and/or
 parser explicitly using the `-p/--parser` option. A very simple parser
 plugin architecture is used, so creating a new parser is easy. Simply
 drop the parser file in the `parsers/` directory and the program will
@@ -106,20 +121,22 @@
 
 |Log Parser|Default Path           |Systems            |
 |----------|-----------------------|-------------------|
 |apt       |`/var/log/apt/history*`|Debian, Ubuntu, etc|
 |dnf       |`/var/log/dnf.rpm.log` |RedHat, Fedora, etc|
 |pacman    |`/var/log/pacman.log`  |Arch, Manjaro, etc |
 
-### USAGE
+## USAGE
+
+Type `pkglog -h` to view the usage summary:
 
 ```
 usage: pkglog [-h] [-u] [-i] [-I] [-n] [-d DAYS] [-a] [-j] [-v] [-c]
-              [-p {pacman,apt,dnf}] [-t TIMEGAP] [-P PATH] [-g | -r]
-              [package]
+                   [-p {pacman,apt,dnf}] [-t TIMEGAP] [-P PATH] [-g | -r]
+                   [package]
 
 Reports log of package updates.
 
 positional arguments:
   package               specific package name to report
 
 options:
@@ -139,32 +156,32 @@
   -t TIMEGAP, --timegap TIMEGAP
                         max minutes gap between grouped updates, default=2
   -P PATH, --path PATH  alternate log path[s] (separate multiple using ":",
                         must be time sequenced)
   -g, --glob            given package name is glob pattern to match
   -r, --regex           given package name is regular expression to match
 
-Note you can set default starting arguments in ~/.config/pkglog-flags.conf.
+Note you can set default starting options in ~/.config/pkglog-flags.conf.
 ```
 
-### DEFAULT ARGUMENTS
+## DEFAULT OPTIONS
 
-You can add default arguments to a personal configuration file
+You can add default options to a personal configuration file
 `~/.config/pkglog-flags.conf`. If that file exists then each line of
-arguments in the file will be concatenated and automatically prepended
-to your `pkglog` command line arguments.
+options in the file will be concatenated and automatically prepended
+to your `pkglog` command line options.
 
-This allow you to set default preferred starting arguments to `pkglog`.
-Type `pkglog -h` to see the arguments supported.
+This allow you to set default preferred starting options to `pkglog`.
+Type `pkglog -h` to see the options supported.
 E.g. `echo "--days 7" >~/.config/pkglog-flags.conf` to make `pkglog`
 only display the last 7 days of updates by default. This is also useful
 to set your parser explicitly using `-p/--parser` (e.g. if the default
 parser is not automatically determined correctly on your system).
 
-### INSTALLATION
+## INSTALLATION
 
 Arch Linux users can install [pkglog from the
 AUR](https://aur.archlinux.org/packages/pkglog). Python 3.7 or later is
 required. The [`python-rich`](https://pypi.org/project/rich/) package is
 required if you want colored output (which is the default unless you
 specify the `-c/--no-color` option).
 
@@ -180,35 +197,33 @@
 
 ```sh
 $ git clone http://github.com/bulletmark/pkglog
 $ cd pkglog
 $ sudo pip3 install -U .
 ```
 
-### UPGRADE
+## UPGRADE
 
 ```sh
 $ cd pkglog  # Source dir, as above
 $ git pull
 $ sudo pip3 install -U .
 ```
 
-### REMOVAL
+## REMOVAL
 
 ```sh
 $ sudo pip3 uninstall pkglog
 ```
 
-### LICENSE
+## LICENSE
 
 Copyright (C) 2020 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
 under the terms of the GNU General Public License as published by the
 Free Software Foundation, either version 3 of the License, or any later
 version.
 This program is distributed in the hope that it will be useful, but
 WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
 Public License at <http://www.gnu.org/licenses/> for more details.
-
-
```

### Comparing `pkglog-1.8/setup.py` & `pkglog-1.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 name = 'pkglog'
 module = name.replace('-', '_')
 here = Path(__file__).resolve().parent
 
 setup(
     name=name,
-    version='1.8',
+    version='1.9',
     description='Reports log of package updates',
     long_description=here.joinpath('README.md').read_text(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/bulletmark/{name}',
     author='Mark Blakeney',
     author_email='mark.blakeney@bullet-systems.net',
-    keywords='pacman apt',
+    keywords='pacman apt dnf',
     license='GPLv3',
     packages=[module] + [str(d) for d in Path(module).iterdir() if d.is_dir()
         and not d.name.startswith('_') and not d.name.startswith('.')],
     python_requires='>=3.7',
     install_requires=['rich'],
     classifiers=[
         'Programming Language :: Python :: 3',
```

