# Comparing `tmp/grrif_tools-0.5.0.tar.gz` & `tmp/grrif_tools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrif_tools-0.5.0.tar", last modified: Sun May  7 15:44:55 2023, max compression
+gzip compressed data, was "grrif_tools-0.5.1.tar", last modified: Sun May  7 16:00:24 2023, max compression
```

## Comparing `grrif_tools-0.5.0.tar` & `grrif_tools-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:44:55.800473 grrif_tools-0.5.0/
--rw-r--r--   0 fetzu      (501) staff       (20)     3099 2023-05-07 11:10:03.000000 grrif_tools-0.5.0/.gitignore
--rw-r--r--   0 fetzu      (501) staff       (20)     1076 2023-05-07 09:42:56.000000 grrif_tools-0.5.0/LICENSE
--rw-r--r--   0 fetzu      (501) staff       (20)       18 2023-05-07 15:22:37.000000 grrif_tools-0.5.0/MANIFEST.in
--rw-r--r--   0 fetzu      (501) staff       (20)     1359 2023-05-07 15:44:55.800268 grrif_tools-0.5.0/PKG-INFO
--rw-r--r--   0 fetzu      (501) staff       (20)      732 2023-05-07 15:20:19.000000 grrif_tools-0.5.0/README.md
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:44:55.799115 grrif_tools-0.5.0/grrif_tools/
--rw-r--r--   0 fetzu      (501) staff       (20)        0 2023-05-07 13:23:06.000000 grrif_tools-0.5.0/grrif_tools/__init__.py
--rw-r--r--   0 fetzu      (501) staff       (20)     3402 2023-05-07 15:27:48.000000 grrif_tools-0.5.0/grrif_tools/cli.py
--rw-r--r--   0 fetzu      (501) staff       (20)     7312 2023-05-07 15:14:39.000000 grrif_tools-0.5.0/grrif_tools/grrif_archiver.py
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:44:55.800083 grrif_tools-0.5.0/grrif_tools.egg-info/
--rw-r--r--   0 fetzu      (501) staff       (20)     1359 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/PKG-INFO
--rw-r--r--   0 fetzu      (501) staff       (20)      349 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fetzu      (501) staff       (20)        1 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       53 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/entry_points.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       55 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/requires.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       12 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/top_level.txt
--rw-r--r--   0 fetzu      (501) staff       (20)      678 2023-05-07 15:43:33.000000 grrif_tools-0.5.0/pyproject.toml
--rw-r--r--   0 fetzu      (501) staff       (20)       38 2023-05-07 15:44:55.800513 grrif_tools-0.5.0/setup.cfg
--rw-r--r--   0 fetzu      (501) staff       (20)      600 2023-05-07 15:27:37.000000 grrif_tools-0.5.0/setup.py
+drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 16:00:24.173706 grrif_tools-0.5.1/
+-rw-r--r--   0 fetzu      (501) staff       (20)     3099 2023-05-07 11:10:03.000000 grrif_tools-0.5.1/.gitignore
+-rw-r--r--   0 fetzu      (501) staff       (20)     1076 2023-05-07 09:42:56.000000 grrif_tools-0.5.1/LICENSE
+-rw-r--r--   0 fetzu      (501) staff       (20)       18 2023-05-07 15:22:37.000000 grrif_tools-0.5.1/MANIFEST.in
+-rw-r--r--   0 fetzu      (501) staff       (20)     1359 2023-05-07 16:00:24.173560 grrif_tools-0.5.1/PKG-INFO
+-rw-r--r--   0 fetzu      (501) staff       (20)      732 2023-05-07 15:20:19.000000 grrif_tools-0.5.1/README.md
+drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 16:00:24.172302 grrif_tools-0.5.1/grrif_tools/
+-rw-r--r--   0 fetzu      (501) staff       (20)        0 2023-05-07 13:23:06.000000 grrif_tools-0.5.1/grrif_tools/__init__.py
+-rw-r--r--   0 fetzu      (501) staff       (20)     3401 2023-05-07 15:58:08.000000 grrif_tools-0.5.1/grrif_tools/cli.py
+-rw-r--r--   0 fetzu      (501) staff       (20)     7758 2023-05-07 15:56:52.000000 grrif_tools-0.5.1/grrif_tools/grrif_archiver.py
+drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 16:00:24.173352 grrif_tools-0.5.1/grrif_tools.egg-info/
+-rw-r--r--   0 fetzu      (501) staff       (20)     1359 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 fetzu      (501) staff       (20)      349 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)        1 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)       53 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)       55 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/requires.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)       12 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/top_level.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)      678 2023-05-07 15:58:03.000000 grrif_tools-0.5.1/pyproject.toml
+-rw-r--r--   0 fetzu      (501) staff       (20)       38 2023-05-07 16:00:24.173757 grrif_tools-0.5.1/setup.cfg
+-rw-r--r--   0 fetzu      (501) staff       (20)      600 2023-05-07 15:57:58.000000 grrif_tools-0.5.1/setup.py
```

### Comparing `grrif_tools-0.5.0/.gitignore` & `grrif_tools-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.0/LICENSE` & `grrif_tools-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.0/PKG-INFO` & `grrif_tools-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grrif_tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: An unofficial set of tools for Cool Cats™.
 Home-page: https://fetzu.ch/
 Download-URL: https://github.com/fetzu/grrif_tools
 Author: Julien 'fetzu' Bono
 License: License :: OSI Approved :: MIT License
 Project-URL: Homepage, https://github.com/fetzu/grrif_tools
 Project-URL: Bug Tracker, https://github.com/fetzu/grrif_tools/issues
```

### Comparing `grrif_tools-0.5.0/README.md` & `grrif_tools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.0/grrif_tools/cli.py` & `grrif_tools-0.5.1/grrif_tools/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,104 +1,104 @@
 ### [ GRRIF Tools by Julien 'fetzu' Bono ]
 ## [ IMPORTS ]
 import sys
 import argparse
 from datetime import date, datetime
 
 ## [ CONFIGURATION ]
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 ## [ Is CLI even cooler with argparse? ]
 parser = argparse.ArgumentParser(
-    description='A set of tools for Cool Cats™. Allows you to archive GRRIF\'s play history and scrobble it to last.fm (upcoming).'
+    description="A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming)."
 )
 
-subparsers = parser.add_subparsers(dest='subcommand')
+subparsers = parser.add_subparsers(dest="subcommand")
 
-archive_parser = subparsers.add_parser(
-    'archive',
-    help='Archive GRRIF\'s play history.'
-)
+archive_parser = subparsers.add_parser("archive", help="Archive GRRIF's play history.")
 archive_parser.add_argument(
-    'destination',
-    choices=['print', 'db', 'txt'],
-    help='Specify where to archive the play history (print to stdout, save to SQLite database or to text in YYYY/MM/DD.txt file(s)).',
+    "destination",
+    choices=["print", "db", "txt"],
+    help="Specify where to archive the play history (print to stdout, save to SQLite database or to text in YYYY/MM/DD.txt file(s)).",
 )
 archive_parser.add_argument(
-    'from_date',
-    nargs='?',
-    default='2021-01-01',
-    help='Specify the start date for the archive in YYYY-MM-DD format. Defaults to 2021-01-01.',
+    "from_date",
+    nargs="?",
+    default="2021-01-01",
+    help="Specify the start date for the archive in YYYY-MM-DD format. Defaults to 2021-01-01.",
 )
 archive_parser.add_argument(
-    'to_date',
-    nargs='?',
-    default=date.today().strftime('%Y-%m-%d'),
+    "to_date",
+    nargs="?",
+    default=date.today().strftime("%Y-%m-%d"),
     help=f"Specify the start date for the archive in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')})",
 )
 
 scrobble_parser = subparsers.add_parser(
-    'scrobble',
-    help='Scrobble to Last.fm.',
+    "scrobble",
+    help="Scrobble to Last.fm.",
 )
 scrobble_parser.add_argument(
-    'from_date',
-    nargs='?',
-    default='2021-01-01',
-    help='Specify the start date for the archive in YYYY-MM-DD format. Defaults to 2021-01-01.',
+    "from_date",
+    nargs="?",
+    default="2021-01-01",
+    help="Specify the start date for the archive in YYYY-MM-DD format. Defaults to 2021-01-01.",
 )
 scrobble_parser.add_argument(
-    'to_date',
-    nargs='?',
-    default=date.today().strftime('%Y-%m-%d'),
+    "to_date",
+    nargs="?",
+    default=date.today().strftime("%Y-%m-%d"),
     help=f"Specify the start date for the archive in YYYY-MM-DD format. Defaults to today ({date.today().strftime('%Y-%m-%d')})",
 )
 
 args = parser.parse_args()
 
+
 ## [ MAIN ]
 def main():
-    print('##########################################\n'
-          f'##### [ GRRIF Tools version {__version__} ] ######\n'
-          '##########################################\n')
+    print(
+        "##########################################\n"
+        f"##### [ GRRIF Tools version {__version__} ] ######\n"
+        "##########################################\n"
+    )
 
     # Displays argparse's help message if no arguments are given
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
 
     # Set the base URL to scrape data from
-    BASE_URL = 'https://www.grrif.ch/recherche-de-titres/?date={}'
+    BASE_URL = "https://www.grrif.ch/recherche-de-titres/?date={}"
 
     # Set the date range to scrape data for
-    START_DATE = datetime.strptime(args.from_date, '%Y-%m-%d')
-    END_DATE = datetime.strptime(args.to_date, '%Y-%m-%d')
+    START_DATE = datetime.strptime(args.from_date, "%Y-%m-%d")
+    END_DATE = datetime.strptime(args.to_date, "%Y-%m-%d")
 
     # Archive was passed !
-    if args.subcommand == 'archive':
+    if args.subcommand == "archive":
         # The "save to SQLite database" option was chosen
-        if args.destination == 'db':
+        if args.destination == "db":
             # Import the necessary functions
             from .grrif_archiver import plays_to_db
 
             # Create/open the database
             plays_to_db(BASE_URL, START_DATE, END_DATE)
 
         # The "save to text files" option was chosen
-        if args.destination == 'txt':
+        if args.destination == "txt":
             # Import the necessary functions
             from .grrif_archiver import plays_to_txt
 
             # Create/open the database
             plays_to_txt(BASE_URL, START_DATE, END_DATE)
 
         # The "output data to stdout" option was chosen
-        if args.destination == 'print':
+        if args.destination == "print":
             # Import the necessary functions
             from .grrif_archiver import plays_to_stdout
 
             # Create/open the database
             plays_to_stdout(BASE_URL, START_DATE, END_DATE)
 
     # Scrobble was passed !
-    if args.subcommand == 'scrobble':
+    if args.subcommand == "scrobble":
         print("Uh-oh, this doesn't exist yet!")
```

### Comparing `grrif_tools-0.5.0/grrif_tools/grrif_archiver.py` & `grrif_tools-0.5.1/grrif_tools/grrif_archiver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,229 @@
-'''
+"""
 GRRIF Archiver helper functions
-'''
+"""
 
 ## [ IMPORTS ]
 from datetime import timedelta
 import os
+import time
 import sqlite3
 import requests
 import titlecase
 from bs4 import BeautifulSoup
 
+
 def plays_to_db(BASE_URL, START_DATE, END_DATE):
-    '''
+    """
     Scrapes the BASE_URL and adds the plays between START_DATE
     and END_DATE to a SQLite database
-    '''
+    """
     database_path = database_handler()
     write_to_db(BASE_URL, START_DATE, END_DATE, database_path)
 
+
 def database_handler():
-    '''
+    """
     Function to check if the  SQLite database
     with a "plays" table containing the plays exists,
     create it if it doesn't...
-    '''
+    """
     database_path = os.path.join(os.path.expanduser("~"), "grrif_data", "grrif_data.db")
 
     # Creates the ../data/ directory if it does not exist yet
     if not os.path.isdir(os.path.dirname(database_path)):
         os.makedirs(os.path.dirname(database_path))
 
     # Create an emtpy db if it does not exist yet
     if not os.path.isfile(database_path):
         # Create the 'plays' table
         conn = sqlite3.connect(database_path)
-        conn.execute('''CREATE TABLE plays (
+        conn.execute(
+            """CREATE TABLE plays (
             id INTEGER PRIMARY KEY AUTOINCREMENT,
             date DATE NOT NULL,
             time TIME NOT NULL,
             artist TEXT NOT NULL,
             title TEXT NOT NULL,
             CONSTRAINT unique_play UNIQUE (date, time)
             );
-        ''')
+        """
+        )
 
         conn.commit()
         conn.close()
     else:
         pass
 
     return database_path
 
+
 def write_to_db(base_url, start_date, end_date, database_path):
-    '''
+    """
     Function to scrape the website between start_date and end_date
     and write all the plays to a database
-    '''
+    """
     # Connect to the DB
     conn = sqlite3.connect(database_path)
     c = conn.cursor()
 
     # Main loop
     current_date = start_date
     while current_date <= end_date:
         # Construct the URL for the current date
-        URL = base_url.format(current_date.strftime('%Y-%m-%d'))
+        URL = base_url.format(current_date.strftime("%Y-%m-%d"))
 
         # Send a request to the server and get the response
         response = requests.get(URL)
 
         # Parse the HTML content of the response using BeautifulSoup
-        soup = BeautifulSoup(response.content, 'html.parser')
+        soup = BeautifulSoup(response.content, "html.parser")
 
         # Find the section of the page containing the data
-        data_section = soup.find('div', {'class': 'listing-search-titres'})
+        data_section = soup.find("div", {"class": "listing-search-titres"})
 
         # Find all the data items
-        data_items = data_section.find_all('article')
+        data_items = data_section.find_all("article")
 
         # Extract the data from each item
         for item in data_items:
-            time = item.find('div', {'class': 'hours'}).text.strip()
-            artist = item.find('div', {'class': 'artist'}).text.strip()
-            title = item.find('div', {'class': 'title'}).text.strip()
+            playtime = item.find("div", {"class": "hours"}).text.strip()
+            artist = item.find("div", {"class": "artist"}).text.strip()
+            title = item.find("div", {"class": "title"}).text.strip()
 
             # Prettify the data
             pretty_artist = titlecase.titlecase(artist)
             pretty_title = titlecase.titlecase(title)
 
             # Save into the database
             # Make sure that the entries are not already present
             try:
-                c.execute('INSERT INTO plays (date, time, artist, title) VALUES (?, ?, ?, ?)', (current_date.strftime('%Y-%m-%d'), time, pretty_artist, pretty_title))
+                c.execute(
+                    "INSERT INTO plays (date, time, artist, title) VALUES (?, ?, ?, ?)",
+                    (
+                        current_date.strftime("%Y-%m-%d"),
+                        playtime,
+                        pretty_artist,
+                        pretty_title,
+                    ),
+                )
                 conn.commit()
             except sqlite3.IntegrityError:
-                #print("Error: row already exists")
+                # print("Error: row already exists")
                 continue
 
+        # Wait 2 seconds before moving on
+        time.sleep(2)
+
         # Move to the next day
         current_date += timedelta(days=1)
 
     # When all is over, close the connection to the DB
     conn.close()
 
     # Print a success message
     print(f"Data archived to {database_path} successfully !")
 
+
 def plays_to_txt(base_url, start_date, end_date):
-    '''
+    """
     Function to scrape the website between start_date and end_date
     and write all the plays to text files in a YYYY/MM/DD.txt structure
-    '''
+    """
     # Set the path for the files and creates the ../data/plays directory if it does not exist yet
     plays_path = os.path.join(os.path.expanduser("~"), "grrif_data", "plays")
-    os.makedirs(os.path.join(os.path.expanduser("~"), "grrif_data", "plays"), exist_ok=True)
+    os.makedirs(
+        os.path.join(os.path.expanduser("~"), "grrif_data", "plays"), exist_ok=True
+    )
 
     current_date = start_date
     while current_date <= end_date:
         # Construct the URL for the current date
-        URL = base_url.format(current_date.strftime('%Y-%m-%d'))
+        URL = base_url.format(current_date.strftime("%Y-%m-%d"))
 
         # Send a request to the server and get the response
         response = requests.get(URL)
 
         # Parse the HTML content of the response using BeautifulSoup
-        soup = BeautifulSoup(response.content, 'html.parser')
+        soup = BeautifulSoup(response.content, "html.parser")
 
         # Find the section of the page containing the data
-        data_section = soup.find('div', {'class': 'listing-search-titres'})
+        data_section = soup.find("div", {"class": "listing-search-titres"})
 
         # Find all the data items
-        data_items = data_section.find_all('article')
+        data_items = data_section.find_all("article")
 
         # Extract the data from each item
         for item in reversed(data_items):
-            time = item.find('div', {'class': 'hours'}).text.strip()
-            artist = item.find('div', {'class': 'artist'}).text.strip()
-            title = item.find('div', {'class': 'title'}).text.strip()
+            playtime = item.find("div", {"class": "hours"}).text.strip()
+            artist = item.find("div", {"class": "artist"}).text.strip()
+            title = item.find("div", {"class": "title"}).text.strip()
 
             # Prettify the data
             pretty_artist = titlecase.titlecase(artist)
             pretty_title = titlecase.titlecase(title)
 
             # Creates the a /YYYY/MM/ structure as needed within the ../data/plays directory
-            dirtree = os.path.join(plays_path, current_date.strftime('%Y'), current_date.strftime('%m'))
+            dirtree = os.path.join(
+                plays_path, current_date.strftime("%Y"), current_date.strftime("%m")
+            )
             os.makedirs(dirtree, exist_ok=True)
 
             # Format and write the data to a DD.txt file
-            formatteddata = f'{pretty_artist} - {pretty_title} (@{time})'
+            formatteddata = f"{pretty_artist} - {pretty_title} (@{playtime})"
             currentfile = os.path.join(dirtree, f'{current_date.strftime("%d")}.txt')
-            with open(currentfile, 'a') as f:
+            with open(currentfile, "a") as f:
                 f.write(formatteddata)
-                f.write('\n')
+                f.write("\n")
+
+        # Wait 2 seconds before moving on
+        time.sleep(2)
 
         # Move to the next day
         current_date += timedelta(days=1)
 
     # Print a success message
     print(f"Data archived to {plays_path} successfully !")
 
+
 def plays_to_stdout(base_url, start_date, end_date):
-    '''
+    """
     Function to scrape the website between start_date and end_date
     and output the data to stdout
-    '''
+    """
     current_date = start_date
     while current_date <= end_date:
         # Construct the URL for the current date
-        URL = base_url.format(current_date.strftime('%Y-%m-%d'))
+        URL = base_url.format(current_date.strftime("%Y-%m-%d"))
 
         # Send a request to the server and get the response
         response = requests.get(URL)
 
         # Parse the HTML content of the response using BeautifulSoup
-        soup = BeautifulSoup(response.content, 'html.parser')
+        soup = BeautifulSoup(response.content, "html.parser")
 
         # Find the section of the page containing the data
-        data_section = soup.find('div', {'class': 'listing-search-titres'})
+        data_section = soup.find("div", {"class": "listing-search-titres"})
 
         # Find all the data items
-        data_items = data_section.find_all('article')
+        data_items = data_section.find_all("article")
 
         # Extract the data from each item
         for item in reversed(data_items):
-            time = item.find('div', {'class': 'hours'}).text.strip()
-            artist = item.find('div', {'class': 'artist'}).text.strip()
-            title = item.find('div', {'class': 'title'}).text.strip()
+            playtime = item.find("div", {"class": "hours"}).text.strip()
+            artist = item.find("div", {"class": "artist"}).text.strip()
+            title = item.find("div", {"class": "title"}).text.strip()
 
             # Prettify the data
             pretty_artist = titlecase.titlecase(artist)
             pretty_title = titlecase.titlecase(title)
 
             # Print the data to stdout
-            print(f"{pretty_artist} - {pretty_title} (@{time} on {current_date.strftime('%Y-%m-%d')})")
+            print(
+                f"{pretty_artist} - {pretty_title} (@{playtime} on {current_date.strftime('%Y-%m-%d')})"
+            )
 
         # Wait 2 seconds before moving on
         time.sleep(2)
 
         # Move to the next day
         current_date += timedelta(days=1)
```

### Comparing `grrif_tools-0.5.0/grrif_tools.egg-info/PKG-INFO` & `grrif_tools-0.5.1/grrif_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grrif-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: An unofficial set of tools for Cool Cats™.
 Home-page: https://fetzu.ch/
 Download-URL: https://github.com/fetzu/grrif_tools
 Author: Julien 'fetzu' Bono
 License: License :: OSI Approved :: MIT License
 Project-URL: Homepage, https://github.com/fetzu/grrif_tools
 Project-URL: Bug Tracker, https://github.com/fetzu/grrif_tools/issues
```

### Comparing `grrif_tools-0.5.0/pyproject.toml` & `grrif_tools-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grrif_tools"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Julien 'fetzu' Bono", url="https://www.fetzu.ch/" },
 ]
 description = "An unofficial set of tools for Cool Cats™."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `grrif_tools-0.5.0/setup.py` & `grrif_tools-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="grrif_tools",
     description="An unofficial set of tools for Cool Cats™.",
     author="Julien 'fetzu' Bono", 
     url="https://fetzu.ch/",
-    version="0.5.0",
+    version="0.5.1",
     download_url="https://github.com/fetzu/grrif_tools",
     packages=find_packages(include=['grrif_tools','grrif_tools.*']),
     license="License :: OSI Approved :: MIT License",
     install_requires=[
         "Requests==2.30.0",
         "beautifulsoup4==4.11.1",
         "titlecase==2.4",
```

