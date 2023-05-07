# Comparing `tmp/gsheetquery-0.0.2.tar.gz` & `tmp/gsheetquery-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsheetquery-0.0.2.tar", last modified: Fri Mar 24 17:46:11 2023, max compression
+gzip compressed data, was "gsheetquery-0.0.3.tar", last modified: Sun May  7 20:02:36 2023, max compression
```

## Comparing `gsheetquery-0.0.2.tar` & `gsheetquery-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-03-24 17:46:11.121183 gsheetquery-0.0.2/
--rw-r--r--   0 noah      (1000) noah      (1000)     1070 2023-02-19 15:37:33.000000 gsheetquery-0.0.2/LICENSE
--rw-r--r--   0 noah      (1000) noah      (1000)      356 2023-03-02 18:11:17.000000 gsheetquery-0.0.2/MANIFEST.in
--rw-r--r--   0 noah      (1000) noah      (1000)     2272 2023-03-23 17:50:59.000000 gsheetquery-0.0.2/Makefile
--rw-r--r--   0 noah      (1000) noah      (1000)     3162 2023-03-24 17:46:11.119187 gsheetquery-0.0.2/PKG-INFO
--rw-r--r--   0 noah      (1000) noah      (1000)     1091 2023-03-24 17:22:16.000000 gsheetquery-0.0.2/README.md
-drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-03-24 17:46:11.092408 gsheetquery-0.0.2/gsheetquery/
--rw-r--r--   0 noah      (1000) noah      (1000)     1832 2023-03-04 01:51:44.000000 gsheetquery-0.0.2/gsheetquery/Client.py
--rw-r--r--   0 noah      (1000) noah      (1000)     1605 2023-03-04 01:51:44.000000 gsheetquery-0.0.2/gsheetquery/Database.py
--rw-r--r--   0 noah      (1000) noah      (1000)       58 2023-03-04 01:51:44.000000 gsheetquery-0.0.2/gsheetquery/Model.py
--rw-r--r--   0 noah      (1000) noah      (1000)       45 2023-03-04 01:51:44.000000 gsheetquery-0.0.2/gsheetquery/__init__.py
--rw-r--r--   0 noah      (1000) noah      (1000)       22 2023-03-24 17:22:16.000000 gsheetquery-0.0.2/gsheetquery/_version.py
-drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-03-24 17:46:11.115201 gsheetquery-0.0.2/gsheetquery/tests/
--rw-r--r--   0 noah      (1000) noah      (1000)     2794 2023-03-04 01:51:44.000000 gsheetquery-0.0.2/gsheetquery/tests/ClientTest.py
--rw-r--r--   0 noah      (1000) noah      (1000)     3173 2023-03-23 17:50:59.000000 gsheetquery-0.0.2/gsheetquery/tests/DatabaseTest.py
--rw-r--r--   0 noah      (1000) noah      (1000)      583 2023-03-23 17:50:59.000000 gsheetquery-0.0.2/gsheetquery/tests/IntegrationTest.py
-drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-03-24 17:46:11.107671 gsheetquery-0.0.2/gsheetquery.egg-info/
--rw-r--r--   0 noah      (1000) noah      (1000)     3162 2023-03-24 17:46:10.000000 gsheetquery-0.0.2/gsheetquery.egg-info/PKG-INFO
--rw-r--r--   0 noah      (1000) noah      (1000)      454 2023-03-24 17:46:11.000000 gsheetquery-0.0.2/gsheetquery.egg-info/SOURCES.txt
--rw-r--r--   0 noah      (1000) noah      (1000)        1 2023-03-24 17:46:10.000000 gsheetquery-0.0.2/gsheetquery.egg-info/dependency_links.txt
--rw-r--r--   0 noah      (1000) noah      (1000)      181 2023-03-24 17:46:10.000000 gsheetquery-0.0.2/gsheetquery.egg-info/requires.txt
--rw-r--r--   0 noah      (1000) noah      (1000)       12 2023-03-24 17:46:10.000000 gsheetquery-0.0.2/gsheetquery.egg-info/top_level.txt
--rw-r--r--   0 noah      (1000) noah      (1000)     2172 2023-03-24 17:22:16.000000 gsheetquery-0.0.2/pyproject.toml
--rw-r--r--   0 noah      (1000) noah      (1000)       38 2023-03-24 17:46:11.121183 gsheetquery-0.0.2/setup.cfg
--rw-r--r--   0 noah      (1000) noah      (1000)       39 2023-03-04 01:51:44.000000 gsheetquery-0.0.2/setup.py
+drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-05-07 20:02:36.071877 gsheetquery-0.0.3/
+-rw-r--r--   0 noah      (1000) noah      (1000)      557 2023-05-07 18:22:06.000000 gsheetquery-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 noah      (1000) noah      (1000)     1070 2023-04-07 00:03:41.000000 gsheetquery-0.0.3/LICENSE
+-rw-r--r--   0 noah      (1000) noah      (1000)      380 2023-04-07 00:03:41.000000 gsheetquery-0.0.3/MANIFEST.in
+-rw-r--r--   0 noah      (1000) noah      (1000)     2272 2023-04-07 00:03:41.000000 gsheetquery-0.0.3/Makefile
+-rw-r--r--   0 noah      (1000) noah      (1000)     4060 2023-05-07 20:02:36.070875 gsheetquery-0.0.3/PKG-INFO
+-rw-r--r--   0 noah      (1000) noah      (1000)     1988 2023-05-07 19:59:25.000000 gsheetquery-0.0.3/README.md
+drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-05-07 20:02:36.055120 gsheetquery-0.0.3/gsheetquery/
+-rw-r--r--   0 noah      (1000) noah      (1000)       45 2023-04-07 00:03:41.000000 gsheetquery-0.0.3/gsheetquery/__init__.py
+-rw-r--r--   0 noah      (1000) noah      (1000)       22 2023-05-07 19:59:25.000000 gsheetquery-0.0.3/gsheetquery/_version.py
+-rw-r--r--   0 noah      (1000) noah      (1000)     2258 2023-04-15 22:04:19.000000 gsheetquery-0.0.3/gsheetquery/client.py
+-rw-r--r--   0 noah      (1000) noah      (1000)     2236 2023-05-07 18:22:06.000000 gsheetquery-0.0.3/gsheetquery/collection.py
+-rw-r--r--   0 noah      (1000) noah      (1000)     2397 2023-04-15 22:04:19.000000 gsheetquery-0.0.3/gsheetquery/database.py
+drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-05-07 20:02:36.070875 gsheetquery-0.0.3/gsheetquery/tests/
+-rw-r--r--   0 noah      (1000) noah      (1000)     2794 2023-04-15 22:04:19.000000 gsheetquery-0.0.3/gsheetquery/tests/client_test.py
+-rw-r--r--   0 noah      (1000) noah      (1000)     2673 2023-05-07 18:22:06.000000 gsheetquery-0.0.3/gsheetquery/tests/collection_test.py
+-rw-r--r--   0 noah      (1000) noah      (1000)     3608 2023-04-15 22:04:19.000000 gsheetquery-0.0.3/gsheetquery/tests/database_test.py
+-rw-r--r--   0 noah      (1000) noah      (1000)      583 2023-04-15 22:04:19.000000 gsheetquery-0.0.3/gsheetquery/tests/integration_test.py
+-rw-r--r--   0 noah      (1000) noah      (1000)     1289 2023-04-15 22:04:19.000000 gsheetquery-0.0.3/gsheetquery/tests/utils_test.py
+-rw-r--r--   0 noah      (1000) noah      (1000)      792 2023-04-15 22:04:19.000000 gsheetquery-0.0.3/gsheetquery/utils.py
+drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-05-07 20:02:36.063350 gsheetquery-0.0.3/gsheetquery.egg-info/
+-rw-r--r--   0 noah      (1000) noah      (1000)     4060 2023-05-07 20:02:35.000000 gsheetquery-0.0.3/gsheetquery.egg-info/PKG-INFO
+-rw-r--r--   0 noah      (1000) noah      (1000)      568 2023-05-07 20:02:36.000000 gsheetquery-0.0.3/gsheetquery.egg-info/SOURCES.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)        1 2023-05-07 20:02:35.000000 gsheetquery-0.0.3/gsheetquery.egg-info/dependency_links.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)      218 2023-05-07 20:02:35.000000 gsheetquery-0.0.3/gsheetquery.egg-info/requires.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)       12 2023-05-07 20:02:35.000000 gsheetquery-0.0.3/gsheetquery.egg-info/top_level.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)     2230 2023-05-07 19:59:25.000000 gsheetquery-0.0.3/pyproject.toml
+-rw-r--r--   0 noah      (1000) noah      (1000)       38 2023-05-07 20:02:36.071877 gsheetquery-0.0.3/setup.cfg
+-rw-r--r--   0 noah      (1000) noah      (1000)       39 2023-04-07 00:03:41.000000 gsheetquery-0.0.3/setup.py
```

### Comparing `gsheetquery-0.0.2/LICENSE` & `gsheetquery-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gsheetquery-0.0.2/Makefile` & `gsheetquery-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `gsheetquery-0.0.2/PKG-INFO` & `gsheetquery-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsheetquery
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Google Sheets ORM and Query Builder
 Author-email: Noah Czelusta <swimninja247@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Noah Czelusta
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,24 +37,54 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # GSheetQuery
-GSheetQuery is a python library for using Google Sheets as a database.  It provides an ORM and query builder.
+GSheetQuery is a python library for using Google Sheets as a document database.  It modeled after pymongo's interface.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Open Issues](https://img.shields.io/github/issues/swimninja247/gsheetquery)
 [![Build Status](https://github.com/swimninja247/gsheetquery/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/swimninja247/gsheetquery/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/swimninja247/gsheetquery/branch/main/graph/badge.svg)](https://codecov.io/gh/swimninja247/gsheetquery)
+[![PyPI](https://img.shields.io/pypi/v/gsheetquery)](https://pypi.org/project/gsheetquery/)
+[![ReadTheDocs](https://readthedocs.org/projects/gsheetquery/badge/?version=latest)](https://gsheetquery.readthedocs.io/en/latest/)
 
 ## Overview
 
-For small projects, full Python frameworks can be overkill (Django), especially if you want code up and running quickly.  Google Sheets can be leveraged as a database and made accessible by GSheetQuery.
+For small projects, full Python frameworks can be overkill (Django).  Especially if you want code up and running quickly.  Google Sheets can be leveraged as a database and made accessible by GSheetQuery.
 
 This library will allow users to interact with google sheets as a document database similar to MongoDB.
 
 ## Install
 
 Install using `pip install gsheetquery` in your preferred command line.  Import to your python files like any other module.
 
+## Quickstart
+
+```python
+from gsheetquery import Client, Collection
+
+# Initialize the client object
+client = Client()
+
+# Create a new database
+database = client.create_database("my_new_database")
+
+# Add a new collection to the database
+new_collection = database['new-collection']
+
+# List the collections in the database
+collection_names = database.list_collection_names()
+print("Collections in the database:", collection_names)
+
+# Add a doc to the collection
+new_doc = {"name": "Bob", "age", "30"}
+new_collection.insert_one(new_doc)
+
+# Query the collection
+new_collection.find_one({"age": "30"})
+
+# Delete the database
+client.drop_collection('new-collection')
+```
```

### Comparing `gsheetquery-0.0.2/gsheetquery/Client.py` & `gsheetquery-0.0.3/gsheetquery/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,72 @@
 import gspread
 from gspread.exceptions import SpreadsheetNotFound
 
 from gsheetquery import SPREADSHEET_FILENAME_PREFIX
-from gsheetquery.Database import Database
-
-"""
-The client represents the main object that users will interact with
-"""
+from gsheetquery.database import Database
 
 
 class Client:
-    def __init__(self) -> None:
-        self._gs = gspread.oauth()
-
     """
-    Gets spreadsheet file associated with database.
+    A class representing a client for accessing Google Sheets API.
     """
 
+    def __init__(self) -> None:
+        """
+        Initialize the Client object.
+        """
+        self._gs = gspread.oauth()
+
     def get_database(self, name):
+        """
+        Get the spreadsheet file associated with a database.
+
+        :param name: The name of the database to retrieve.
+        :return: A Database object representing the spreadsheet file, or None if the file was not found.
+        """
         full_name = SPREADSHEET_FILENAME_PREFIX + name
         try:
-            # Try to open the spreadsheet by its name
             spreadsheet = self._gs.open(full_name)
             return Database(spreadsheet)
 
         except SpreadsheetNotFound:
-            # Handle the case where the spreadsheet does not exist
             print(f"Spreadsheet '{full_name}' not found in your Google Drive account.")
             return None
 
-    """
-    Creates a spreadsheet file with the given @name.
-    """
-
     def create_database(self, name):
+        """
+        Create a new spreadsheet file with the given name.
+
+        :param name: The name of the spreadsheet to create.
+        :return: A Database object representing the newly created spreadsheet file.
+        """
         full_name = SPREADSHEET_FILENAME_PREFIX + name
-        # First see if a spreadsheet with this name already exists
         try:
             spreadsheet = self._gs.open(full_name)
             return Database(spreadsheet)
 
         except SpreadsheetNotFound:
             return Database(self._gs.create(title=full_name))
 
     def del_database(self, name):
+        """
+        Delete a spreadsheet file associated with a database.
+
+        :param name: The name of the database to delete.
+        """
         full_name = SPREADSHEET_FILENAME_PREFIX + name
         try:
             id = self._gs.open(full_name).id
         except SpreadsheetNotFound:
             return
 
         self._gs.del_spreadsheet(id)
 
-    """
-    Returns a list of databases in the user's Drive
-    """
-
     def list_databases(self):
+        """
+        Return a list of databases in the user's Google Drive.
+
+        :return: A list of database names.
+        """
         files = self._gs.list_spreadsheet_files()
         database_filenames = [file['name'] for file in files if file['name'].startswith(SPREADSHEET_FILENAME_PREFIX)]
         return database_filenames
```

### Comparing `gsheetquery-0.0.2/gsheetquery/tests/ClientTest.py` & `gsheetquery-0.0.3/gsheetquery/tests/client_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest.mock import patch, MagicMock
 import unittest
 import gspread
-from gsheetquery.Client import Client
-from gsheetquery.Database import Database
+from gsheetquery.client import Client
+from gsheetquery.database import Database
 from gsheetquery import SPREADSHEET_FILENAME_PREFIX
 
 
 class TestClient(unittest.TestCase):
     @patch.object(gspread, 'oauth')
     def setUp(self, mock_oauth):
         self.client = Client()
```

### Comparing `gsheetquery-0.0.2/gsheetquery/tests/IntegrationTest.py` & `gsheetquery-0.0.3/gsheetquery/tests/integration_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from gsheetquery.Client import Client
+from gsheetquery.client import Client
 import pytest
 
 
 @pytest.mark.skip(reason="need to automate google api auth")
 def test_client():
     client = Client()
```

### Comparing `gsheetquery-0.0.2/gsheetquery.egg-info/PKG-INFO` & `gsheetquery-0.0.3/gsheetquery.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsheetquery
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Google Sheets ORM and Query Builder
 Author-email: Noah Czelusta <swimninja247@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Noah Czelusta
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,24 +37,54 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # GSheetQuery
-GSheetQuery is a python library for using Google Sheets as a database.  It provides an ORM and query builder.
+GSheetQuery is a python library for using Google Sheets as a document database.  It modeled after pymongo's interface.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Open Issues](https://img.shields.io/github/issues/swimninja247/gsheetquery)
 [![Build Status](https://github.com/swimninja247/gsheetquery/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/swimninja247/gsheetquery/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/swimninja247/gsheetquery/branch/main/graph/badge.svg)](https://codecov.io/gh/swimninja247/gsheetquery)
+[![PyPI](https://img.shields.io/pypi/v/gsheetquery)](https://pypi.org/project/gsheetquery/)
+[![ReadTheDocs](https://readthedocs.org/projects/gsheetquery/badge/?version=latest)](https://gsheetquery.readthedocs.io/en/latest/)
 
 ## Overview
 
-For small projects, full Python frameworks can be overkill (Django), especially if you want code up and running quickly.  Google Sheets can be leveraged as a database and made accessible by GSheetQuery.
+For small projects, full Python frameworks can be overkill (Django).  Especially if you want code up and running quickly.  Google Sheets can be leveraged as a database and made accessible by GSheetQuery.
 
 This library will allow users to interact with google sheets as a document database similar to MongoDB.
 
 ## Install
 
 Install using `pip install gsheetquery` in your preferred command line.  Import to your python files like any other module.
 
+## Quickstart
+
+```python
+from gsheetquery import Client, Collection
+
+# Initialize the client object
+client = Client()
+
+# Create a new database
+database = client.create_database("my_new_database")
+
+# Add a new collection to the database
+new_collection = database['new-collection']
+
+# List the collections in the database
+collection_names = database.list_collection_names()
+print("Collections in the database:", collection_names)
+
+# Add a doc to the collection
+new_doc = {"name": "Bob", "age", "30"}
+new_collection.insert_one(new_doc)
+
+# Query the collection
+new_collection.find_one({"age": "30"})
+
+# Delete the database
+client.drop_collection('new-collection')
+```
```

### Comparing `gsheetquery-0.0.2/pyproject.toml` & `gsheetquery-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "gsheetquery"
 authors = [{name = "Noah Czelusta", email = "swimninja247@gmail.com"}]
 description="A Google Sheets ORM and Query Builder"
 readme = "README.md"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.8"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -46,14 +46,17 @@
     "mypy",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "twine",
     "wheel",
     "gspread",
     "pyproject-flake8",
+    "sphinx",
+    "sphinx_rtd_theme",
+    "recommonmark"
 ]
 
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
@@ -94,8 +97,8 @@
 # warn_unused_configs = true
 # disallow_subclassing_any = true
 # disallow_incomplete_defs = true
 # disallow_untyped_decorators = true
 # disallow_untyped_calls = true
 
 [tool.pytest.ini_options]
-testpaths = 'tests'
+testpaths = 'tests'
```

