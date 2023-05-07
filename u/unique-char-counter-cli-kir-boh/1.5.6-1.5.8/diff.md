# Comparing `tmp/unique_char_counter_cli_kir_boh-1.5.6.tar.gz` & `tmp/unique_char_counter_cli_kir_boh-1.5.8.tar.gz`

## Comparing `unique_char_counter_cli_kir_boh-1.5.6.tar` & `unique_char_counter_cli_kir_boh-1.5.8.tar`

### file list

```diff
@@ -1,15 +1,22 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/tests/__init__.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/LICENSE
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.coverage
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/__init__.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/__init__.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/test_unique_char_counter_cli.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/LICENSE
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/pyproject.toml
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/PKG-INFO
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/v/cache/nodeids` & `unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/test_unique_char_counter_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.assertEqual(unique_char_counter_cli.return_amount_once_occured_items(' '), 0)
 
     def test_return_amount_once_occured_items_with_unhashable_obj(self):
         with self.assertRaises(TypeError) as e:
             unique_char_counter_cli.return_amount_once_occured_items(['ff'])
         self.assertEqual("unhashable type: 'list'", e.exception.args[0])
 
-    @patch('unique_char_counter_cli.unique_char_counter_cli.get_obj_from_cli')
+    @patch('unique_char_counter_cli_kir_boh.unique_char_counter_cli.get_obj_from_cli')
     @patch('builtins.open', new_callable=mock_open, read_data='dataff')
     def test_main_with_mock_file(self, mock_open, mock_get_obj_from_cli):
         mock_get_obj_from_cli.return_value = Namespace(string=False, file=True, hashable_obj='some file')
         self.assertEqual(unique_char_counter_cli.main(), 2)
 
     @patch('unique_char_counter_cli_kir_boh.unique_char_counter_cli.get_obj_from_cli')
     def test_main_with_mock_file(self, mock_get_obj_from_cli):
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.6/LICENSE` & `unique_char_counter_cli_kir_boh-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.6/README.md` & `unique_char_counter_cli_kir_boh-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.6/pyproject.toml` & `unique_char_counter_cli_kir_boh-1.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "unique_char_counter_cli_kir_boh"
-version = "1.5.6"
+version = "1.5.8"
 authors = [
   { name="Kiril Bogatiuk", email="kirillbogatu2005@gmail.com" },
 ]
 maintainers = [
     {name ="Stanislav Hrytsyshyn", email="kirillbogatu2005@gmail.com"},
 ]
 description = "Project gets hashable obj from cli an returns uniqe items amount, other funcs desribed in README.md"
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.6/PKG-INFO` & `unique_char_counter_cli_kir_boh-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique_char_counter_cli_kir_boh
-Version: 1.5.6
+Version: 1.5.8
 Summary: Project gets hashable obj from cli an returns uniqe items amount, other funcs desribed in README.md
 Author-email: Kiril Bogatiuk <kirillbogatu2005@gmail.com>
 Maintainer-email: Stanislav Hrytsyshyn <kirillbogatu2005@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

