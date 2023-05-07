# Comparing `tmp/grrif_tools-0.5.3.tar.gz` & `tmp/grrif_tools-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrif_tools-0.5.3.tar", last modified: Sun May  7 19:11:01 2023, max compression
+gzip compressed data, was "grrif_tools-0.5.4.tar", last modified: Sun May  7 19:29:41 2023, max compression
```

## Comparing `grrif_tools-0.5.3.tar` & `grrif_tools-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:11:01.283422 grrif_tools-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 19:10:50.000000 grrif_tools-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 19:10:50.000000 grrif_tools-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-07 19:11:01.283422 grrif_tools-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-07 19:10:50.000000 grrif_tools-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:11:01.283422 grrif_tools-0.5.3/grrif_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:10:50.000000 grrif_tools-0.5.3/grrif_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-07 19:10:50.000000 grrif_tools-0.5.3/grrif_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-07 19:10:50.000000 grrif_tools-0.5.3/grrif_tools/grrif_archiver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:11:01.283422 grrif_tools-0.5.3/grrif_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-07 19:11:01.000000 grrif_tools-0.5.3/grrif_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-07 19:11:01.000000 grrif_tools-0.5.3/grrif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:11:01.000000 grrif_tools-0.5.3/grrif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 19:11:01.000000 grrif_tools-0.5.3/grrif_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 19:11:01.000000 grrif_tools-0.5.3/grrif_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 19:11:01.000000 grrif_tools-0.5.3/grrif_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 19:11:01.283422 grrif_tools-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-07 19:10:50.000000 grrif_tools-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:29:41.206409 grrif_tools-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-07 19:29:41.202409 grrif_tools-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:29:41.202409 grrif_tools-0.5.4/grrif_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/grrif_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/grrif_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/grrif_tools/grrif_archiver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:29:41.202409 grrif_tools-0.5.4/grrif_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 19:29:41.000000 grrif_tools-0.5.4/grrif_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 19:29:41.206409 grrif_tools-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 19:29:34.000000 grrif_tools-0.5.4/setup.py
```

### Comparing `grrif_tools-0.5.3/LICENSE` & `grrif_tools-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.3/PKG-INFO` & `grrif_tools-0.5.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grrif_tools
-Version: 0.5.3
+Version: 0.5.4
 Summary: An unofficial set of tools for Cool Cats™.
-Home-page: https://fetzu.ch/
-Download-URL: https://github.com/fetzu/grrif_tools
+Home-page: https://github.com/fetzu/grrif_tools
+Download-URL: https://github.com/fetzu/grrif_tools/releases/latest
 Author: Julien 'fetzu' Bono
 License: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GRRIF Tools
```

### Comparing `grrif_tools-0.5.3/README.md` & `grrif_tools-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.3/grrif_tools/grrif_archiver.py` & `grrif_tools-0.5.4/grrif_tools/grrif_archiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         )
 
         conn.commit()
         conn.close()
     else:
         pass
 
+    print(f"Database loaded at {database_path}.")
     return database_path
 
 
 def write_to_db(base_url, start_date, end_date, database_path):
     """
     Function to scrape the website between start_date and end_date
     and write all the plays to a database
@@ -107,14 +108,17 @@
                     ),
                 )
                 conn.commit()
             except sqlite3.IntegrityError:
                 # print("Error: row already exists")
                 continue
 
+        # Update the user on current progress
+        print(f"Plays for {current_date.strftime('%Y-%m-%d')} saved to database.")
+
         # Wait 2 seconds before moving on
         time.sleep(2)
 
         # Move to the next day
         current_date += timedelta(days=1)
 
     # When all is over, close the connection to the DB
@@ -171,14 +175,17 @@
             # Format and write the data to a DD.txt file
             formatteddata = f"{pretty_artist} - {pretty_title} (@{playtime})"
             currentfile = os.path.join(dirtree, f'{current_date.strftime("%d")}.txt')
             with open(currentfile, "a") as f:
                 f.write(formatteddata)
                 f.write("\n")
 
+        # Update the user on current progress
+        print(f"Plays for {current_date.strftime('%Y-%m-%d')} saved to {currentfile}.")
+
         # Wait 2 seconds before moving on
         time.sleep(2)
 
         # Move to the next day
         current_date += timedelta(days=1)
 
     # Print a success message
```

### Comparing `grrif_tools-0.5.3/grrif_tools.egg-info/PKG-INFO` & `grrif_tools-0.5.4/grrif_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grrif-tools
-Version: 0.5.3
+Version: 0.5.4
 Summary: An unofficial set of tools for Cool Cats™.
-Home-page: https://fetzu.ch/
-Download-URL: https://github.com/fetzu/grrif_tools
+Home-page: https://github.com/fetzu/grrif_tools
+Download-URL: https://github.com/fetzu/grrif_tools/releases/latest
 Author: Julien 'fetzu' Bono
 License: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GRRIF Tools
```

### Comparing `grrif_tools-0.5.3/setup.py` & `grrif_tools-0.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 setup(
     name="grrif_tools",
     description="An unofficial set of tools for Cool Cats™.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Julien 'fetzu' Bono", 
-    url="https://fetzu.ch/",
-    version="0.5.3",
-    download_url="https://github.com/fetzu/grrif_tools",
+    url="https://github.com/fetzu/grrif_tools",
+    version="0.5.4",
+    download_url="https://github.com/fetzu/grrif_tools/releases/latest",
     packages=find_packages(include=['grrif_tools','grrif_tools.*']),
     license="License :: OSI Approved :: MIT License",
     install_requires=[
         "Requests==2.30.0",
         "beautifulsoup4==4.11.1",
         "titlecase==2.4",
     ],
```

