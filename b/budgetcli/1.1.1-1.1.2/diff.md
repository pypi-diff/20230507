# Comparing `tmp/budgetcli-1.1.1.tar.gz` & `tmp/budgetcli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetcli-1.1.1.tar", last modified: Sat May  6 19:35:07 2023, max compression
+gzip compressed data, was "budgetcli-1.1.2.tar", last modified: Sun May  7 20:29:18 2023, max compression
```

## Comparing `budgetcli-1.1.1.tar` & `budgetcli-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.095886 budgetcli-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-06 19:34:41.000000 budgetcli-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-06 19:35:07.095886 budgetcli-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-06 19:34:41.000000 budgetcli-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-06 19:34:41.000000 budgetcli-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-06 19:35:07.095886 budgetcli-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.091886 budgetcli-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.091886 budgetcli-1.1.1/src/budgetcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.095886 budgetcli-1.1.1/src/budgetcli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/cli/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.095886 budgetcli-1.1.1/src/budgetcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.095886 budgetcli-1.1.1/src/budgetcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-07 20:28:54.000000 budgetcli-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-07 20:29:18.454256 budgetcli-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-07 20:28:54.000000 budgetcli-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-07 20:28:54.000000 budgetcli-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-07 20:29:18.454256 budgetcli-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.450256 budgetcli-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/src/budgetcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/src/budgetcli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/cli/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/src/budgetcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-07 20:28:54.000000 budgetcli-1.1.2/src/budgetcli/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:29:18.454256 budgetcli-1.1.2/src/budgetcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 20:29:18.000000 budgetcli-1.1.2/src/budgetcli.egg-info/top_level.txt
```

### Comparing `budgetcli-1.1.1/LICENSE` & `budgetcli-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/PKG-INFO` & `budgetcli-1.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetcli
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
 Author: Code Rustle
 Author-email: coderustle@gmail.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,18 @@
 
 [![Build](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml/badge.svg)](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml) [![Test](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml/badge.svg)](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml) [![License](https://img.shields.io/pypi/l/budgetcli)](https://img.shields.io/pypi/l/budgetcli)
 
 A simple terminal app written in Python to manage budgets and expenses in Google Sheet.
 
 ## Features
 
-- Ability to track incomes and expenses as transactions
-- Ability to list transactions by month
+- Add income transactions 
+- Add outcome transactions 
+- List transactions by month
+- Add spending categories
 
 ## Installation
 
 ```
 pip install budgetcli
 ```
 
@@ -35,15 +37,15 @@
 
 Please follow the following link for more details: [Authorize credentials for a desktop application](https://developers.google.com/sheets/api/quickstart/python)
 
 ## Configuration
 
 Before start adding transactions and data, you need to do the following steps:
 
-**Provide the google spreadsheet id**
+**Provide Google spreadsheet id**
 ```
 budgetcli config spreadsheet-id ID
 ```
 
 **Copy the client_secret_XXX.json to app config**
 ```
 budgetcli config credentials-file-path /path/to/client_secret.json
@@ -54,57 +56,57 @@
 budgetcli auth
 ```
 
 **Init sheet tables headers**
 ```
 budgetcli init
 ```
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/init.gif)
 
 ## Usage
 
 The commands follow the below structure.
 ```
 budgetcli <VERB> <OBJECT> <OPTIONS>
 ```
 ### Incomes
 To add an income you need to provide only an amount and a category. By default, all the income transactions are added
 with default today date and without no description.
 
 **Add an income**
-```bash
-budgetcli add income 5000 Salary
-```
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income.gif)
+
 **Add an income with description**
-```bash
-budgetcli add income 500 projects --description "Project A"
-```
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income-description.gif)
+
 **Add an income with date and description**
-```bash
-budgetcli add income 500 projects --description "Project A" --date 2023-04-01
-```
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income-date.gif)
 
 ### Outcomes
 Same for outcome transactions, you need to provide only an amount and a category. By default, all the outcome transactions are added
 with default today date and without no description.
 
 **Add an outcome**
-```bash
-budgetcli add outcome 400 Rent
-```
-```bash
-budgetcli add outcome 400 Rent --date 2023-05-01 --description "Rent for April"
-```
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/outcome.gif)
+
+**Add an outcome with description**
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/outcome-date.gif)
+
 ### List transactions
-**List transactions. Default first 100 rows**
-```
-budgetcli list transactions 
-```
+
+**List first 100 transactions**
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/transactions.gif)
+
 **List only first 10 transactions**
 
-```bash
-budgetcli list transactions --rows 10 
-```
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/transactions-rows.gif)
 
 **List transactions for a specific month**
 ```bash
 budgetcli list transactions --month April 
 ```
```

### Comparing `budgetcli-1.1.1/README.md` & `budgetcli-1.1.2/src/budgetcli.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,34 @@
+Metadata-Version: 2.1
+Name: budgetcli
+Version: 1.1.2
+Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
+Author: Code Rustle
+Author-email: coderustle@gmail.com
+License: MIT
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Budget CLI
 
 [![Build](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml/badge.svg)](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml) [![Test](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml/badge.svg)](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml) [![License](https://img.shields.io/pypi/l/budgetcli)](https://img.shields.io/pypi/l/budgetcli)
 
 A simple terminal app written in Python to manage budgets and expenses in Google Sheet.
 
 ## Features
 
-- Ability to track incomes and expenses as transactions
-- Ability to list transactions by month
+- Add income transactions 
+- Add outcome transactions 
+- List transactions by month
+- Add spending categories
 
 ## Installation
 
 ```
 pip install budgetcli
 ```
 
@@ -20,15 +37,15 @@
 
 Please follow the following link for more details: [Authorize credentials for a desktop application](https://developers.google.com/sheets/api/quickstart/python)
 
 ## Configuration
 
 Before start adding transactions and data, you need to do the following steps:
 
-**Provide the google spreadsheet id**
+**Provide Google spreadsheet id**
 ```
 budgetcli config spreadsheet-id ID
 ```
 
 **Copy the client_secret_XXX.json to app config**
 ```
 budgetcli config credentials-file-path /path/to/client_secret.json
@@ -39,57 +56,57 @@
 budgetcli auth
 ```
 
 **Init sheet tables headers**
 ```
 budgetcli init
 ```
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/init.gif)
 
 ## Usage
 
 The commands follow the below structure.
 ```
 budgetcli <VERB> <OBJECT> <OPTIONS>
 ```
 ### Incomes
 To add an income you need to provide only an amount and a category. By default, all the income transactions are added
 with default today date and without no description.
 
 **Add an income**
-```bash
-budgetcli add income 5000 Salary
-```
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income.gif)
+
 **Add an income with description**
-```bash
-budgetcli add income 500 projects --description "Project A"
-```
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income-description.gif)
+
 **Add an income with date and description**
-```bash
-budgetcli add income 500 projects --description "Project A" --date 2023-04-01
-```
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income-date.gif)
 
 ### Outcomes
 Same for outcome transactions, you need to provide only an amount and a category. By default, all the outcome transactions are added
 with default today date and without no description.
 
 **Add an outcome**
-```bash
-budgetcli add outcome 400 Rent
-```
-```bash
-budgetcli add outcome 400 Rent --date 2023-05-01 --description "Rent for April"
-```
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/outcome.gif)
+
+**Add an outcome with description**
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/outcome-date.gif)
+
 ### List transactions
-**List transactions. Default first 100 rows**
-```
-budgetcli list transactions 
-```
+
+**List first 100 transactions**
+
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/transactions.gif)
+
 **List only first 10 transactions**
 
-```bash
-budgetcli list transactions --rows 10 
-```
+![](https://github.com/coderustle/budgetcli/blob/main/images/commands/transactions-rows.gif)
 
 **List transactions for a specific month**
 ```bash
 budgetcli list transactions --month April 
 ```
```

### Comparing `budgetcli-1.1.1/pyproject.toml` & `budgetcli-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/setup.cfg` & `budgetcli-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = budgetcli
-version = 1.1.1
+version = 1.1.2
 author = Code Rustle
 author_email = coderustle@gmail.com
 description = A simple async budgeting app to manage expenses and budgets in google spreadsheets
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
```

### Comparing `budgetcli-1.1.1/src/budgetcli/auth.py` & `budgetcli-1.1.2/src/budgetcli/auth.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/cli/add.py` & `budgetcli-1.1.2/src/budgetcli/cli/add.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/cli/config.py` & `budgetcli-1.1.2/src/budgetcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/cli/display.py` & `budgetcli-1.1.2/src/budgetcli/cli/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/commands.py` & `budgetcli-1.1.2/src/budgetcli/commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,21 +38,36 @@
     def execute(self) -> None:
         asyncio.run(self.init())
 
 
 class AddTransactionCommand(Command):
     def __init__(self, transaction: Transaction):
         self.transaction = transaction
-        self.manager = ManagerFactory.create_manager_for("transactions")
+        self.tra_manager = ManagerFactory.create_manager_for("transactions")
+        self.cat_manager = ManagerFactory.create_manager_for("categories")
+
+    async def add_transaction(self):
+        tra_row = self.transaction.to_sheet_row()
+        category_name = self.transaction.category
+
+        categories = await self.cat_manager.get_records_by_name(category_name)
+        if categories and category_name in categories[0]:
+            await self.tra_manager.append(tra_row)
+        else:
+            category = Category(name=category_name)
+            row = category.to_sheet_row()
+            cat_task = asyncio.create_task(self.cat_manager.append(row))
+            tra_task = asyncio.create_task(self.tra_manager.append(tra_row))
+            await cat_task
+            await tra_task
 
     def execute(self):
         try:
             with task_progress(description="Processing.."):
-                row = self.transaction.to_sheet_row()
-                asyncio.run(self.manager.append(row))
+                asyncio.run(self.add_transaction())
                 print(":heavy_check_mark: Transaction was added successfully")
             pass
         except AttributeError:
             print("Init factory manager error")
 
 
 class ListTransactionCommand(Command):
```

### Comparing `budgetcli-1.1.1/src/budgetcli/data_manager.py` & `budgetcli-1.1.2/src/budgetcli/data_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,18 +93,18 @@
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
         return None
 
     async def _query(
-        self, query: str, sheet_index: int
+        self, query: str, sheet: str
     ) -> list[dict[str, list]] | None:
         """A method to use Google Visualization API"""
-        params = f"gid={sheet_index}&tq={query}&tqx=out:json"
+        params = f"sheet={sheet}&tq={query}&tqx=out:json"
         url = f"{self.gvi_url}?{params}"
         response = await self.session.get(url)
         try:
             response.raise_for_status()
             to_replace = "/*O_o*/\ngoogle.visualization.Query.setResponse("
             clean_data = response.text.replace(to_replace, "")[:-2]
             json_data = json.loads(clean_data)
@@ -208,17 +208,15 @@
         a1 = f"{self.SHEET_NAME}!A1"
         headers = "DATE CATEGORY DESCRIPTION INCOME OUTCOME"
         sheet_coroutine: Coroutine = self._get_sheet_or_create(self.SHEET_NAME)
         update_coroutine: Coroutine = self._update(headers.split(), a1)
         try:
             sheet = await asyncio.wait_for(sheet_coroutine, timeout=5)
             if sheet:
-                index = sheet["index"]
-                update_config("transactions_sheet_index", str(index))
-            await asyncio.wait_for(update_coroutine, timeout=5)
+                await asyncio.wait_for(update_coroutine, timeout=5)
         except asyncio.TimeoutError:
             print("Timeout error")
 
     async def update(self, values: list[str], a1: str) -> dict[str, str]:
         notation = f"{self.SHEET_NAME}!{a1}"
         result = await self._update(values=values, a1=notation)
         return result
@@ -234,22 +232,17 @@
         result: list[list[str]] = await self._list(a1=transaction_range)
         return result if result else []
 
     async def get_records_for_month(self, month: int) -> list[list[str]]:
         """Query the transactions for current month"""
         month -= 1  # month query starts from 0 to 11
         query = f"select A,B,C,D,E where month(A)={month}"
-        index = get_config("transactions_sheet_index")
-        if index:
-            rows = await self._query(query, int(index))
-            transactions = [self._process_row(i) for i in rows] if rows else []
-            return transactions
-        else:
-            pprint(":warning: Transactions sheet index is missing")
-        return []
+        rows = await self._query(query, self.SHEET_NAME)
+        transactions = [self._process_row(i) for i in rows] if rows else []
+        return transactions
 
 
 class CategoryDataManager(AbstractDataManager):
     SHEET_NAME = "CATEGORIES"
     FIRST_COLUMN = "A"
     LAST_COLUMN = "A"
     ROW_START = 2
@@ -260,17 +253,15 @@
         a1 = f"{self.SHEET_NAME}!A1"
         headers = "CATEGORY"
         sheet_coroutine: Coroutine = self._get_sheet_or_create(self.SHEET_NAME)
         update_coroutine: Coroutine = self._update([headers], a1)
         try:
             sheet = await asyncio.wait_for(sheet_coroutine, timeout=5)
             if sheet:
-                index = sheet["index"]
-                update_config("categories_sheet_index", str(index))
-            await asyncio.wait_for(update_coroutine, timeout=5)
+                await asyncio.wait_for(update_coroutine, timeout=5)
         except asyncio.TimeoutError:
             print("Timeout error")
 
     async def update(self, values: list[str], a1: str) -> dict[str, str]:
         notation = f"{self.SHEET_NAME}!{a1}"
         result = await self._update(values=values, a1=notation)
         return result
@@ -286,22 +277,17 @@
         result: list[list[str]] = await self._list(a1=category_range)
         return result if result else []
 
     async def get_records_by_name(self, name: str) -> list[list[str]]:
         """Return a category by a given name"""
         name = name.lower()
         query = f"select A where A='{name}'"
-        index = get_config("categories_sheet_index")
-        if index:
-            rows = await self._query(query, int(index))
-            categories = [self._process_row(i) for i in rows] if rows else []
-            return categories
-        else:
-            pprint(":warning: Categories sheet index is missing")
-        return []
+        rows = await self._query(query, self.SHEET_NAME)
+        categories = [self._process_row(i) for i in rows] if rows else []
+        return categories
 
 
 class ManagerFactory:
     @staticmethod
     def create_manager_for(manager_name: str) -> T | None:
         match manager_name:
             case "transactions":
```

### Comparing `budgetcli-1.1.1/src/budgetcli/main.py` & `budgetcli-1.1.2/src/budgetcli/main.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/models.py` & `budgetcli-1.1.2/src/budgetcli/models.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/settings.py` & `budgetcli-1.1.2/src/budgetcli/settings.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/utils/config.py` & `budgetcli-1.1.2/src/budgetcli/utils/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/utils/dates.py` & `budgetcli-1.1.2/src/budgetcli/utils/dates.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli/utils/display.py` & `budgetcli-1.1.2/src/budgetcli/utils/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.1/src/budgetcli.egg-info/SOURCES.txt` & `budgetcli-1.1.2/src/budgetcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

