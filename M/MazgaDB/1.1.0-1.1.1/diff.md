# Comparing `tmp/MazgaDB-1.1.0.tar.gz` & `tmp/MazgaDB-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MazgaDB-1.1.0.tar", last modified: Tue May  2 13:03:54 2023, max compression
+gzip compressed data, was "MazgaDB-1.1.1.tar", last modified: Sun May  7 10:50:45 2023, max compression
```

## Comparing `MazgaDB-1.1.0.tar` & `MazgaDB-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.758739 MazgaDB-1.1.0/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.754739 MazgaDB-1.1.0/MazgaDB.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     8396 2023-05-02 13:03:54.000000 MazgaDB-1.1.0/MazgaDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      483 2023-05-02 13:03:54.000000 MazgaDB-1.1.0/MazgaDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-02 13:03:54.000000 MazgaDB-1.1.0/MazgaDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2023-05-02 13:03:54.000000 MazgaDB-1.1.0/MazgaDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     8396 2023-05-02 13:03:54.758739 MazgaDB-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     5551 2023-05-02 12:24:10.000000 MazgaDB-1.1.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.754739 MazgaDB-1.1.0/bot_func/
--rw-r--r--   0 runner    (1000) runner    (1000)       54 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/bot_func/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      327 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/bot_func/class_people.py
--rw-r--r--   0 runner    (1000) runner    (1000)      177 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/bot_func/new_people.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.754739 MazgaDB-1.1.0/package/
--rw-r--r--   0 runner    (1000) runner    (1000)     3880 2023-05-02 12:18:43.000000 MazgaDB-1.1.0/package/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-04-26 09:07:23.000000 MazgaDB-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-02 13:03:54.758739 MazgaDB-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      753 2023-05-02 13:03:36.000000 MazgaDB-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.758739 MazgaDB-1.1.0/sql_func/
--rw-r--r--   0 runner    (1000) runner    (1000)      236 2023-05-01 12:09:34.000000 MazgaDB-1.1.0/sql_func/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/append.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3802 2023-05-02 10:42:39.000000 MazgaDB-1.1.0/sql_func/class_db.py
--rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/column.py
--rw-r--r--   0 runner    (1000) runner    (1000)      154 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/delete.py
--rw-r--r--   0 runner    (1000) runner    (1000)      467 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/delete_column.py
--rw-r--r--   0 runner    (1000) runner    (1000)      187 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/is_there.py
--rw-r--r--   0 runner    (1000) runner    (1000)      400 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/new_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      459 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/read_all.py
--rw-r--r--   0 runner    (1000) runner    (1000)      251 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/select.py
--rw-r--r--   0 runner    (1000) runner    (1000)      235 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/update.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-07 10:50:45.197079 MazgaDB-1.1.1/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-07 10:50:45.193079 MazgaDB-1.1.1/MazgaDB.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     8556 2023-05-07 10:50:45.000000 MazgaDB-1.1.1/MazgaDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-05-07 10:50:45.000000 MazgaDB-1.1.1/MazgaDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-07 10:50:45.000000 MazgaDB-1.1.1/MazgaDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2023-05-07 10:50:45.000000 MazgaDB-1.1.1/MazgaDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       26 2023-05-07 10:50:45.000000 MazgaDB-1.1.1/MazgaDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     8556 2023-05-07 10:50:45.197079 MazgaDB-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     5631 2023-05-07 10:37:54.000000 MazgaDB-1.1.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-07 10:50:45.193079 MazgaDB-1.1.1/bot_func/
+-rw-r--r--   0 runner    (1000) runner    (1000)       54 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/bot_func/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      327 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/bot_func/class_people.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      177 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/bot_func/new_people.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-07 10:50:45.193079 MazgaDB-1.1.1/package/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4435 2023-05-07 09:00:10.000000 MazgaDB-1.1.1/package/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-04-26 09:07:23.000000 MazgaDB-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-07 10:50:45.197079 MazgaDB-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      817 2023-05-07 10:50:41.000000 MazgaDB-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-07 10:50:45.197079 MazgaDB-1.1.1/sql_func/
+-rw-r--r--   0 runner    (1000) runner    (1000)      236 2023-05-01 12:09:34.000000 MazgaDB-1.1.1/sql_func/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/append.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3802 2023-05-02 10:42:39.000000 MazgaDB-1.1.1/sql_func/class_db.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/column.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      154 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/delete.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      467 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/delete_column.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      187 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/is_there.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      400 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/new_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      459 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/read_all.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      251 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/select.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      235 2023-05-01 07:50:45.000000 MazgaDB-1.1.1/sql_func/update.py
```

### Comparing `MazgaDB-1.1.0/MazgaDB.egg-info/PKG-INFO` & `MazgaDB-1.1.1/MazgaDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MazgaDB
-Version: 1.1.0
+Version: 1.1.1
 Summary: ОРМ для базы данных SQlite3
 Home-page: https://github.com/Mazgagzam/MazgaDB
 Author: Mazga
 Author-email: agzamikail@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/Mazgagzam/MazgaDB
 Description: # Documentation MazgaDB
@@ -290,14 +290,24 @@
         db.execute('SELECT * FROM users')
         ```
         
         #### Output:
         ```
         [(1, 'Mazga')]
         ```
+        
+        
+        
+        
+        
+        --------------
+        | id | fname |
+        |----|-------|
+        | 1  | Mazga |
+        --------------
 Keywords: example python orm sql
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `MazgaDB-1.1.0/PKG-INFO` & `MazgaDB-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MazgaDB
-Version: 1.1.0
+Version: 1.1.1
 Summary: ОРМ для базы данных SQlite3
 Home-page: https://github.com/Mazgagzam/MazgaDB
 Author: Mazga
 Author-email: agzamikail@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/Mazgagzam/MazgaDB
 Description: # Documentation MazgaDB
@@ -290,14 +290,24 @@
         db.execute('SELECT * FROM users')
         ```
         
         #### Output:
         ```
         [(1, 'Mazga')]
         ```
+        
+        
+        
+        
+        
+        --------------
+        | id | fname |
+        |----|-------|
+        | 1  | Mazga |
+        --------------
 Keywords: example python orm sql
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `MazgaDB-1.1.0/README.md` & `MazgaDB-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -280,8 +280,18 @@
 db = MazgaDB('users.db')
 db.execute('SELECT * FROM users')
 ```
 
 #### Output:
 ```
 [(1, 'Mazga')]
-```
+```
+
+
+
+
+
+--------------
+| id | fname |
+|----|-------|
+| 1  | Mazga |
+--------------
```

### Comparing `MazgaDB-1.1.0/package/__init__.py` & `MazgaDB-1.1.1/sql_func/class_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,23 @@
 import sqlite3
 from prettytable import from_db_cursor
 
 
-class MazgaDB:
-    def __init__(self, db: str, data_classes: dict = dict()):
+class DataBase:
+    def __init__(self, db: str, data_class: dict = dict()):
         self.conn = sqlite3.connect(db)
         self.cur = self.conn.cursor()
         self.db = db
-        self.data_class = data_classes
-      
-    def create_table(self, name_table: str, param: dict):
-        """Пример создания таблицы CREATE TABLE IF NOT EXISTS users(
-        userid INT PRIMARY KEY,
-        fname TEXT,
-        lname TEXT,
-        gender TEXT);
-        """
-        self.execute(
-            f"""CREATE TABLE IF NOT EXISTS {name_table}({','.join([t + ' ' + param[t] for t in param])});"""
-        )
-      
-    def append_line(self, name_table: str, values: list):
+        self.data_class = data_class
+
+    def append(self, name_table: str, values: list):
         self.execute(
             f"""INSERT INTO {name_table} VALUES({','.join(['"' + str(t) + '"' for t in values])});"""
         )
-      
-    def update_line(self, name_table: str, key1: str, value1: str, key2: str, value2: str):
-        self.execute(
-            f"UPDATE {name_table} SET {key2} = '{value2}' WHERE {key1} = '{value1}' "
-        )
-      
-    def delete_line(self, name_table: str, key: str, value: str):
-        self.execute(f"""DELETE from {name_table} where {key} = {value}""")
-      
+
     def append_column(self, name_table: str, name_column: str, type_column: str):
         self.execute(
             f"alter table {name_table} add column {name_column} '{type_column}'"
         )
 
     def delete_column(self, name_table: str, column: str):
         """
@@ -52,28 +33,42 @@
         columns = [
             col.split()[0]
             for col in table[-1].split("(")[1].replace(")", "").split(",")
         ]
 
         columns.remove(column)
 
-        self.execute(f"CREATE TABLE config AS SELECT {','.join(columns)} FROM {name_table};")
+        self.execute(f"CREATE TABLE config AS SELECT {','.join(columns)} FROM test;")
         self.execute(f"DROP TABLE {name_table}")
         self.execute(f"ALTER TABLE config RENAME TO {name_table};")
 
-    
+    def delete(self, id: int, name_table: str, key: str, value: str):
+        self.execute(f"""DELETE from {name_table} where {key} = {value}""")
 
     def is_there(self, name_table: str, key: str, value: str) -> bool:
         self.cur.execute(f"SELECT * FROM {name_table} WHERE {key} = {value}")
         return True if len(self.cur.fetchall()) > 0 else False
 
-    
+    def update(self, name_table: str, key1: str, value1: str, key2: str, value2: str):
+        self.execute(
+            f"UPDATE {name_table} SET {key2} = '{value2}' WHERE {key1} = '{value1}' "
+        )
 
+    def create_table(self, name_table: str, param: dict):
+        """Пример создания таблицы CREATE TABLE IF NOT EXISTS users(
+        userid INT PRIMARY KEY,
+        fname TEXT,
+        lname TEXT,
+        gender TEXT);
+        """
+        self.execute(
+            f"""CREATE TABLE IF NOT EXISTS {name_table}({','.join([t + ' ' + param[t] for t in param])});"""
+        )
 
-    def read_table(self, name_table: str, param: list = None) -> str:
+    def read_table(self, name_table: str, param=None) -> str:
         try:
             self.cur.execute(
                 f"SELECT {','.join(param) if param else '*'} FROM {name_table}"
             )
             mytable = from_db_cursor(self.cur)
             return str(mytable)
         except sqlite3.Error as error:
@@ -82,15 +77,15 @@
     def saw_tables(self):
         """
         Возращает все таблицы из базы данных
         """
         return self.execute("SELECT name FROM sqlite_master WHERE type='table';")
 
     def select_class(
-        self, name_table: str, key, value, param: str = "*", class_data=None
+        self, key, value, name_table: str, param: str = "*", class_data=None
     ):
         """
         Возращает значения в виде классом
         """
 
         self.cur.execute(f"SELECT {param} FROM {name_table} WHERE {key} = {value}")
         if class_data:
@@ -103,12 +98,11 @@
     def select(self, name_table: str, key, value, param: str = "*"):
         """
         Обычный SELECT из SQL
         """
         self.cur.execute(f"SELECT {param} FROM {name_table} WHERE {key} = {value}")
         return self.cur.fetchall()
 
-    def execute(self, sql_request: str, params: list = None):
-        
+    def execute(self, sql_request: str, params: str = None):
         self.cur.execute(sql_request)
         self.conn.commit()
         return self.cur.fetchall()
```

### Comparing `MazgaDB-1.1.0/setup.py` & `MazgaDB-1.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import setup, find_packages
 
 def readme():
-  with open('README.md', 'r') as f:
-    return f.read()
+    with open("README.md", "r") as f:
+        return f.read()
 
 setup(
-  name='MazgaDB',
-  version='1.1.0',
-  author='Mazga',
-  author_email='agzamikail@gmail.com',
-  description='ОРМ для базы данных SQlite3',
-  long_description=readme(),
-  long_description_content_type='text/markdown',
-  url='https://github.com/Mazgagzam/MazgaDB',
-  packages=find_packages(),
-  install_requires=[],
-  classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-  ],
-  keywords='example python orm sql',
-  project_urls={
-    'Documentation': 'https://github.com/Mazgagzam/MazgaDB'
-  },
-  python_requires='>=3.8'
-)
+    name="MazgaDB",
+    version="1.1.1",
+    author="Mazga",
+    author_email="agzamikail@gmail.com",
+    description="ОРМ для базы данных SQlite3",
+    long_description=readme(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/Mazgagzam/MazgaDB",
+    packages= find_packages(),
+    install_requires=['sqlite3','prettytable'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    keywords="example python orm sql",
+    project_urls={"Documentation": "https://github.com/Mazgagzam/MazgaDB"},
+    python_requires=">=3.8",
+)
```

### Comparing `MazgaDB-1.1.0/sql_func/class_db.py` & `MazgaDB-1.1.1/package/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,116 @@
 import sqlite3
 from prettytable import from_db_cursor
 
 
-class DataBase:
-    def __init__(self, db: str, data_class: dict = dict()):
+class MazgaDB:
+    def __init__(self, db: str, data_classes: dict = dict()):
         self.conn = sqlite3.connect(db)
         self.cur = self.conn.cursor()
         self.db = db
-        self.data_class = data_class
+        self.data_class = data_classes
 
-    def append(self, name_table: str, values: list):
+    def accept_columns(self, name_table: str):
+      self.cur.execute("SELECT * FROM sqlite_master")
+      
+      for tables in self.cur.fetchall():
+        if name_table in tables:
+          break
+      else:
+        raise ValueError('no such table exists')
+        
+      columns = [
+            column.split()[0]
+            for column in tables[-1].split("(")[1].replace(")", "").split(",")
+      ]
+              
+      return columns
+
+
+    
+
+    def create_table(self, name_table: str, param: dict):
+        """Пример создания таблицы CREATE TABLE IF NOT EXISTS users(
+        userid INT PRIMARY KEY,
+        fname TEXT,
+        lname TEXT,
+        gender TEXT);
+        """
+        self.execute(
+            f"""CREATE TABLE IF NOT EXISTS {name_table}({','.join([t + ' ' + param[t] for t in param])});"""
+        )
+
+    def append_line(self, name_table: str, values: list):
         self.execute(
             f"""INSERT INTO {name_table} VALUES({','.join(['"' + str(t) + '"' for t in values])});"""
         )
 
+    def update_line(
+        self, name_table: str, key1: str, value1: str, key2: str, value2: str
+    ):
+        self.execute(
+            f"UPDATE {name_table} SET {key2} = '{value2}' WHERE {key1} = '{value1}' "
+        )
+
+    def delete_line(self, name_table: str, key: str, value: str):
+        self.execute(f"""DELETE from {name_table} where {key} = {value}""")
+
     def append_column(self, name_table: str, name_column: str, type_column: str):
         self.execute(
             f"alter table {name_table} add column {name_column} '{type_column}'"
         )
 
     def delete_column(self, name_table: str, column: str):
         """
         Передайте те столбцы которые хотите оставить
         """
 
-        self.cur.execute("SELECT * FROM sqlite_master")
-
-        for table in self.cur.fetchall():
-            if name_table in table:
-                break
-
-        columns = [
-            col.split()[0]
-            for col in table[-1].split("(")[1].replace(")", "").split(",")
-        ]
+        columns = self.accept_columns(name_table)
 
         columns.remove(column)
 
-        self.execute(f"CREATE TABLE config AS SELECT {','.join(columns)} FROM test;")
+        self.execute(
+            f"CREATE TABLE config AS SELECT {','.join(columns)} FROM {name_table};"
+        )
         self.execute(f"DROP TABLE {name_table}")
         self.execute(f"ALTER TABLE config RENAME TO {name_table};")
 
-    def delete(self, id: int, name_table: str, key: str, value: str):
-        self.execute(f"""DELETE from {name_table} where {key} = {value}""")
-
     def is_there(self, name_table: str, key: str, value: str) -> bool:
         self.cur.execute(f"SELECT * FROM {name_table} WHERE {key} = {value}")
         return True if len(self.cur.fetchall()) > 0 else False
 
-    def update(self, name_table: str, key1: str, value1: str, key2: str, value2: str):
-        self.execute(
-            f"UPDATE {name_table} SET {key2} = '{value2}' WHERE {key1} = '{value1}' "
-        )
-
-    def create_table(self, name_table: str, param: dict):
-        """Пример создания таблицы CREATE TABLE IF NOT EXISTS users(
-        userid INT PRIMARY KEY,
-        fname TEXT,
-        lname TEXT,
-        gender TEXT);
-        """
-        self.execute(
-            f"""CREATE TABLE IF NOT EXISTS {name_table}({','.join([t + ' ' + param[t] for t in param])});"""
-        )
-
-    def read_table(self, name_table: str, param=None) -> str:
+    def read_table(self, name_table: str, type: str = 's', param: list = None) -> str:
         try:
             self.cur.execute(
                 f"SELECT {','.join(param) if param else '*'} FROM {name_table}"
             )
             mytable = from_db_cursor(self.cur)
-            return str(mytable)
+
+            if type == 's':
+              return str(mytable)
+            elif type == 'm':
+              counts = len(self.accept_columns(name_table)) + 1
+              
+              table = str(mytable).replace('+','-', counts).replace('+','|', counts).replace('+','-')
+              return table
+
+            else:
+              raise ValueError('unknown type')
+            
         except sqlite3.Error as error:
             return error
 
     def saw_tables(self):
         """
         Возращает все таблицы из базы данных
         """
         return self.execute("SELECT name FROM sqlite_master WHERE type='table';")
 
     def select_class(
-        self, key, value, name_table: str, param: str = "*", class_data=None
+        self, name_table: str, key, value, param: str = "*", class_data=None
     ):
         """
         Возращает значения в виде классом
         """
 
         self.cur.execute(f"SELECT {param} FROM {name_table} WHERE {key} = {value}")
         if class_data:
@@ -98,11 +123,11 @@
     def select(self, name_table: str, key, value, param: str = "*"):
         """
         Обычный SELECT из SQL
         """
         self.cur.execute(f"SELECT {param} FROM {name_table} WHERE {key} = {value}")
         return self.cur.fetchall()
 
-    def execute(self, sql_request: str, params: str = None):
+    def execute(self, sql_request: str, params: list = None):
         self.cur.execute(sql_request)
         self.conn.commit()
-        return self.cur.fetchall()
+        return self.cur.fetchall()
```

