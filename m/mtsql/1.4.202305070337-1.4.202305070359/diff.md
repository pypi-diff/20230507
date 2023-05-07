# Comparing `tmp/mtsql-1.4.202305070337-py3-none-any.whl.zip` & `tmp/mtsql-1.4.202305070359-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19238 bytes, number of entries: 11
+Zip file size: 19241 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       44 b- defN 22-Dec-30 06:14 mt/sql/__init__.py
--rw-r--r--  2.0 unx     9989 b- defN 23-Apr-23 11:37 mt/sql/base.py
+-rw-r--r--  2.0 unx     9994 b- defN 23-May-07 03:59 mt/sql/base.py
 -rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 12:37 mt/sql/mysql.py
 -rw-r--r--  2.0 unx    65252 b- defN 23-May-07 03:37 mt/sql/psql.py
 -rw-r--r--  2.0 unx     8678 b- defN 23-Feb-27 00:37 mt/sql/sqlite.py
--rw-r--r--  2.0 unx      396 b- defN 23-May-07 03:37 mt/sql/version.py
--rw-r--r--  2.0 unx     1070 b- defN 23-May-07 03:37 mtsql-1.4.202305070337.dist-info/LICENSE
--rw-r--r--  2.0 unx      597 b- defN 23-May-07 03:37 mtsql-1.4.202305070337.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 03:37 mtsql-1.4.202305070337.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-May-07 03:37 mtsql-1.4.202305070337.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 23-May-07 03:37 mtsql-1.4.202305070337.dist-info/RECORD
-11 files, 91878 bytes uncompressed, 17784 bytes compressed:  80.6%
+-rw-r--r--  2.0 unx      396 b- defN 23-May-07 03:59 mt/sql/version.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/LICENSE
+-rw-r--r--  2.0 unx      597 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/RECORD
+11 files, 91883 bytes uncompressed, 17787 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mt/sql/sqlite.py
 Comment: 
 
 Filename: mt/sql/version.py
 Comment: 
 
-Filename: mtsql-1.4.202305070337.dist-info/LICENSE
+Filename: mtsql-1.4.202305070359.dist-info/LICENSE
 Comment: 
 
-Filename: mtsql-1.4.202305070337.dist-info/METADATA
+Filename: mtsql-1.4.202305070359.dist-info/METADATA
 Comment: 
 
-Filename: mtsql-1.4.202305070337.dist-info/WHEEL
+Filename: mtsql-1.4.202305070359.dist-info/WHEEL
 Comment: 
 
-Filename: mtsql-1.4.202305070337.dist-info/top_level.txt
+Filename: mtsql-1.4.202305070359.dist-info/top_level.txt
 Comment: 
 
-Filename: mtsql-1.4.202305070337.dist-info/RECORD
+Filename: mtsql-1.4.202305070359.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/sql/base.py

```diff
@@ -335,15 +335,15 @@
         connection engine to the server
 
     Returns
     -------
     list
         list of all schema names
     """
-    return sa.inspect(engine).get_schemas()
+    return sa.inspect(engine).get_schema_names()
 
 
 def list_tables(engine, schema: tp.Optional[str] = None):
     """Lists all tables of a given schema.
 
     Parameters
     ----------
```

## mt/sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
 VERSION_DAY = int('07')
 VERSION_HOUR = int('03')
-VERSION_MINUTE = int('37')
+VERSION_MINUTE = int('59')
 MAJOR_VERSION = 1
 MINOR_VERSION = 4
-PATCH_VERSION = 202305070337
-version_date = '2023/05/07 03:37'
+PATCH_VERSION = 202305070359
+version_date = '2023/05/07 03:59'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtsql-1.4.202305070337.dist-info/LICENSE` & `mtsql-1.4.202305070359.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtsql-1.4.202305070337.dist-info/METADATA` & `mtsql-1.4.202305070359.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsql
-Version: 1.4.202305070337
+Version: 1.4.202305070359
 Summary: Extra Python modules to deal with the interaction between pandas dataframes and remote SQL servers, for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtsql
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.sql/mt.sql.html
 Project-URL: Source Code, https://github.com/inteplus/mtsql
 License-File: LICENSE
 Requires-Dist: sqlalchemy (>=2.0)
```

