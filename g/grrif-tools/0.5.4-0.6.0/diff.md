# Comparing `tmp/grrif_tools-0.5.4.tar.gz` & `tmp/grrif_tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrif_tools-0.5.4.tar", last modified: Sun May  7 19:29:41 2023, max compression
+gzip compressed data, was "grrif_tools-0.6.0.tar", last modified: Sun May  7 20:49:57 2023, max compression
```

## Comparing `grrif_tools-0.5.4.tar` & `grrif_tools-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:29:41.206409 grrif_tools-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-07 19:29:41.202409 grrif_tools-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:29:41.202409 grrif_tools-0.5.4/grrif_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/grrif_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/grrif_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/grrif_tools/grrif_archiver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:29:41.202409 grrif_tools-0.5.4/grrif_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 19:29:41.206409 grrif_tools-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/grrif_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/grrif_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/grrif_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/grrif_tools/grrif_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/grrif_tools/grrif_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/grrif_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/setup.py
```

### Comparing `grrif_tools-0.5.4/LICENSE` & `grrif_tools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.4/README.md` & `grrif_tools-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # GRRIF Tools
 
-A set of tools for Cool Cats™. Allows you to archive GRRIF's play history to a SQLite database or text files, ~~and scrobble it to last.fm~~ (upcoming).
+A set of tools for Cool Cats™. Allows you to archive GRRIF's play history to a SQLite database (or text files), compute/display some stats (top 10/25/100 artists and tracks), ~~and scrobble it to last.fm~~ (upcoming).
 
 ```
-usage: grrif_tools [-h] {archive,scrobble} ...
+usage: grrif_tools [-h] {archive,stats,scrobble} ...
 
 A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming).
 
 positional arguments:
-  {archive,scrobble}
-    archive           Archive GRRIF's play history.
-    scrobble          Scrobble to Last.fm.
+  {archive,stats,scrobble}
+    archive             Archive GRRIF's play history.
+    stats               Get some stats out of the database.
+    scrobble            Scrobble to Last.fm.
 
 options:
-  -h, --help          show this help message and exit
+  -h, --help            show this help message and exit
   ```
   
   **NOTE:** This package is unofficial and meant mostly as a playground to experiment with some new things (argparse, python packaging, etc...). Please do not DDoS GRRIF's website !
```

### Comparing `grrif_tools-0.5.4/grrif_tools/cli.py` & `grrif_tools-0.6.0/grrif_tools/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ### [ GRRIF Tools by Julien 'fetzu' Bono ]
 ## [ IMPORTS ]
 import sys
 import argparse
 from datetime import date, datetime
 
 ## [ CONFIGURATION ]
-__version__ = "0.5.4"
+__version__ = "0.6.0"
 
 ## [ Is CLI even cooler with argparse? ]
 parser = argparse.ArgumentParser(
     description="A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming)."
 )
 
-subparsers = parser.add_subparsers(dest="subcommand")
+subparsers = parser.add_subparsers(dest="command")
 
 archive_parser = subparsers.add_parser("archive", help="Archive GRRIF's play history.")
 archive_parser.add_argument(
     "destination",
     choices=["print", "db", "txt"],
     help="Specify where to archive the play history (print to stdout, save to SQLite database or to text in YYYY/MM/DD.txt file(s)).",
 )
@@ -26,15 +26,58 @@
     default="2021-01-01",
     help="Specify the start date for the archive in YYYY-MM-DD format. Defaults to 2021-01-01.",
 )
 archive_parser.add_argument(
     "to_date",
     nargs="?",
     default=date.today().strftime("%Y-%m-%d"),
-    help=f"Specify the start date for the archive in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')})",
+    help=f"Specify the start date for the archive in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')}).",
+)
+
+stats_parser = subparsers.add_parser(
+    "stats", help="Get some stats out of the database."
+)
+stats_subparsers = stats_parser.add_subparsers(dest="stats_command")
+artists_parser = stats_subparsers.add_parser(
+    "artists", help="Display stats for artists"
+)
+artists_parser.add_argument(
+    "topofthepop",
+    choices=["top10", "top25", "top100"],
+    help="Display the top 10, 25 or 100 artists.",
+)
+artists_parser.add_argument(
+    "from_date",
+    nargs="?",
+    default="2021-01-01",
+    help="Specify the start date for the stats in YYYY-MM-DD format. Defaults to 2021-01-01.",
+)
+artists_parser.add_argument(
+    "to_date",
+    nargs="?",
+    default=date.today().strftime("%Y-%m-%d"),
+    help=f"Specify the start date for the stats in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')}).",
+)
+tracks_parser = stats_subparsers.add_parser("tracks", help="Display stats for tracks")
+tracks_parser.add_argument(
+    "topofthepop",
+    choices=["top10", "top25", "top100"],
+    help="Display the top 10, 25 or 100 tracks.",
+)
+tracks_parser.add_argument(
+    "from_date",
+    nargs="?",
+    default="2021-01-01",
+    help="Specify the start date for the stats in YYYY-MM-DD format. Defaults to 2021-01-01.",
+)
+tracks_parser.add_argument(
+    "to_date",
+    nargs="?",
+    default=date.today().strftime("%Y-%m-%d"),
+    help=f"Specify the start date for the stats in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')}).",
 )
 
 scrobble_parser = subparsers.add_parser(
     "scrobble",
     help="Scrobble to Last.fm.",
 )
 scrobble_parser.add_argument(
@@ -43,15 +86,15 @@
     default="2021-01-01",
     help="Specify the start date for the archive in YYYY-MM-DD format. Defaults to 2021-01-01.",
 )
 scrobble_parser.add_argument(
     "to_date",
     nargs="?",
     default=date.today().strftime("%Y-%m-%d"),
-    help=f"Specify the start date for the archive in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')})",
+    help=f"Specify the start date for the archive in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')}).",
 )
 
 args = parser.parse_args()
 
 
 ## [ MAIN ]
 def main():
@@ -70,15 +113,15 @@
     BASE_URL = "https://www.grrif.ch/recherche-de-titres/?date={}"
 
     # Set the date range to scrape data for
     START_DATE = datetime.strptime(args.from_date, "%Y-%m-%d")
     END_DATE = datetime.strptime(args.to_date, "%Y-%m-%d")
 
     # Archive was passed !
-    if args.subcommand == "archive":
+    if args.command == "archive":
         # The "save to SQLite database" option was chosen
         if args.destination == "db":
             # Let the user know what we are attempting
             print(
                 f"Attempting to archive plays from {START_DATE.strftime('%Y-%m-%d')} to {END_DATE.strftime('%Y-%m-%d')} to a SQLite database."
             )
 
@@ -110,10 +153,30 @@
 
             # Import the necessary functions
             from .grrif_archiver import plays_to_stdout
 
             # Create/open the database
             plays_to_stdout(BASE_URL, START_DATE, END_DATE)
 
+    # Stats was passed !
+    # Import the necessary functions
+    from .grrif_stats import topofthepop
+
+    if args.stats_command == "artists":
+        if args.topofthepop == "top10":
+            topofthepop("artist", "10", START_DATE, END_DATE)
+        if args.topofthepop == "top25":
+            topofthepop("artist", "25", START_DATE, END_DATE)
+        if args.topofthepop == "top100":
+            topofthepop("artist", "100", START_DATE, END_DATE)
+
+    if args.stats_command == "tracks":
+        if args.topofthepop == "top10":
+            topofthepop("artist, title", "10", START_DATE, END_DATE)
+        if args.topofthepop == "top25":
+            topofthepop("artist, title", "25", START_DATE, END_DATE)
+        if args.topofthepop == "top100":
+            topofthepop("title", "100", START_DATE, END_DATE)
+
     # Scrobble was passed !
-    if args.subcommand == "scrobble":
+    if args.command == "scrobble":
         print("Uh-oh, this doesn't exist yet!")
```

### Comparing `grrif_tools-0.5.4/grrif_tools/grrif_archiver.py` & `grrif_tools-0.6.0/grrif_tools/grrif_archiver.py`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.4/setup.py` & `grrif_tools-0.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import os
 from setuptools import setup, find_packages
 
-with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
+with open(
+    os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md"),
+    encoding="utf-8",
+) as f:
     long_description = f.read()
 
 setup(
     name="grrif_tools",
     description="An unofficial set of tools for Cool Cats™.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    author="Julien 'fetzu' Bono", 
+    long_description_content_type="text/markdown",
+    author="Julien 'fetzu' Bono",
     url="https://github.com/fetzu/grrif_tools",
-    version="0.5.4",
+    version="0.6.0",
     download_url="https://github.com/fetzu/grrif_tools/releases/latest",
-    packages=find_packages(include=['grrif_tools','grrif_tools.*']),
+    packages=find_packages(include=["grrif_tools", "grrif_tools.*"]),
     license="License :: OSI Approved :: MIT License",
     install_requires=[
         "Requests==2.30.0",
         "beautifulsoup4==4.11.1",
         "titlecase==2.4",
     ],
     entry_points={"console_scripts": ["grrif_tools=grrif_tools.cli:main"]},
-)
+)
```

