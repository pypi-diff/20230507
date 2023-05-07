# Comparing `tmp/bring-python-api-1.0.1.tar.gz` & `tmp/bring-python-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring-python-api-1.0.1.tar", last modified: Sun May  7 10:29:09 2023, max compression
+gzip compressed data, was "bring-python-api-1.0.2.tar", last modified: Sun May  7 10:44:16 2023, max compression
```

## Comparing `bring-python-api-1.0.1.tar` & `bring-python-api-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:29:09.330693 bring-python-api-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:29:09.330693 bring-python-api-1.0.1/BringPythonApi/
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/BringPythonApi/Bring.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/BringPythonApi/BringList.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/BringPythonApi/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/BringPythonApi/Item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/BringPythonApi/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/BringPythonApi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-07 10:29:09.330693 bring-python-api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:29:09.330693 bring-python-api-1.0.1/bring_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-07 10:29:08.000000 bring-python-api-1.0.1/bring_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-07 10:29:09.000000 bring-python-api-1.0.1/bring_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:29:08.000000 bring-python-api-1.0.1/bring_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 10:29:08.000000 bring-python-api-1.0.1/bring_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 10:29:08.000000 bring-python-api-1.0.1/bring_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:29:09.334693 bring-python-api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 10:28:53.000000 bring-python-api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:44:16.152743 bring-python-api-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:44:16.152743 bring-python-api-1.0.2/BringPythonApi/
+-rw-r--r--   0 runner    (1001) docker     (123)    13971 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/BringPythonApi/Bring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/BringPythonApi/BringList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/BringPythonApi/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/BringPythonApi/Item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/BringPythonApi/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/BringPythonApi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-07 10:44:16.152743 bring-python-api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:44:16.152743 bring-python-api-1.0.2/bring_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-07 10:44:15.000000 bring-python-api-1.0.2/bring_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-07 10:44:16.000000 bring-python-api-1.0.2/bring_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:44:15.000000 bring-python-api-1.0.2/bring_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 10:44:15.000000 bring-python-api-1.0.2/bring_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 10:44:15.000000 bring-python-api-1.0.2/bring_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:44:16.152743 bring-python-api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 10:44:04.000000 bring-python-api-1.0.2/setup.py
```

### Comparing `bring-python-api-1.0.1/BringPythonApi/Bring.py` & `bring-python-api-1.0.2/BringPythonApi/Bring.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,14 +423,37 @@
 			url=f'{self.API_URL}/bringlistitemdetails/{itemUuid}/usersection',
 			headers=self._headers,
 			data={
 				'userSectionId': newCategory
 			}
 		)
 
+	def createNewList(self, listName: str, theme: Optional[str] = 'ch.publisheria.bring.theme.home') -> Response:
+		"""
+		Creates a new list on your account
+
+		:param listName: The name of the new list
+		:param theme: Used by the web app as a background
+		:returns Requests.Response
+		"""
+
+		response = requests.post(
+			url=f'{self.API_URL}/bringusers/{self.user.uuid}/lists',
+			headers=self._headers,
+			data={
+				'name': listName,
+				'theme': theme
+			}
+		)
+
+		if response.status_code == 200:
+			self.user.setLists(data=[{'listUuid': response.json()['bringListUUID'], 'name': listName, 'theme': theme}])
+
+		return response
+
 	def getItemDetails(self, itemId: str, listUuid: Optional[str] = '') -> Response:
 		if not listUuid:
 			listUuid = self._user.defaultListUUID
 
 		headers = self._headers.copy()
 
 		payload = {
```

### Comparing `bring-python-api-1.0.1/BringPythonApi/Exceptions.py` & `bring-python-api-1.0.2/BringPythonApi/Exceptions.py`

 * *Files identical despite different names*

### Comparing `bring-python-api-1.0.1/BringPythonApi/User.py` & `bring-python-api-1.0.2/BringPythonApi/User.py`

 * *Files identical despite different names*

### Comparing `bring-python-api-1.0.1/BringPythonApi/__init__.py` & `bring-python-api-1.0.2/BringPythonApi/__init__.py`

 * *Files identical despite different names*

### Comparing `bring-python-api-1.0.1/LICENSE` & `bring-python-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bring-python-api-1.0.1/PKG-INFO` & `bring-python-api-1.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,76 @@
-Metadata-Version: 2.1
-Name: bring-python-api
-Version: 1.0.1
-Summary: Bring! web api for Python
-Home-page: https://github.com/Psychokiller1888/bring-api
-Author: Psychokiller1888
-Author-email: laurentchervet@bluewin.ch
-Maintainer: Psychokiller1888
-License: GPL-3.0
-Description: ## Bring Python API
-        
-        This is an unofficial python API for Bring! the shopping list service, based on their webapi. Some endpoints might be missing, this is solely based on traffic capture while using the web app.
-        
-        
-        ### API doc
-        You'll find the API documentation on this page: https://psychokiller1888.github.io/bring-api/
-        
-        Please note that sme endpoints might be missing
-        
-        ### Insomnia repository
-        Import the repository in your Insomnia app: https://github.com/Psychokiller1888/bring-api/tree/master
-        
-        ### Usage
-        
-        - Import the package in your project
-        - Create a Bring instance by passing your login and password to use the API:
-        
-        ```python
-        from BringPythonApi.Bring import Bring
-        
-        try:
-            bring = Bring(email='foo@bar.com', password='foobar')
-        except Exception as e:
-            print(f'Error logging in: {e}')
-        else:
-            # Add an item to your default list
-            bring.purchase(item='Milk', detail='3 liters')
-            
-            # Remove 1 cat food from your default list
-            bring.remove(item='Cat food', detail=1)
-            
-            # Empty your list called "My work list". If no name provided, defaults to you default list
-            bring.emptyPurchaseList(listUuid=bring.user.getList(name='My work list'))
-        
-            # Change the default list language
-            bring.changeUserListLanguage(languageCode='en-US')
-        
-            # Change the account password
-            bring.changeUserPassword(newPassword='myNewPassword')
-        
-            # Get stats for Cat food
-            bring.getItemStatistic(itemName='Cat food')
-        
-            # Get profile picture
-            bring.getUserProfilePicture()
-        
-            # Add item to recent list
-            bring.addToRecentItems(item='Milk', detail='2 liters')
-            
-            # Get my work shopping list
-            bring.getShoppingList(listUuid=bring.user.getList(name='Work list'))
-            
-            # Move cucumber to another category
-            bring.changeItemCategory(newCategory='Eigene Artikel')
-        ```
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+## Bring Python API
+
+This is an unofficial python API for Bring! the shopping list service, based on their webapi. Some endpoints might be missing, this is solely based on traffic capture while using the web app.
+
+
+### API doc
+You'll find the API documentation on this page: https://psychokiller1888.github.io/bring-api/
+
+Please note that sme endpoints might be missing
+
+### Insomnia repository
+Import the repository in your Insomnia app: https://github.com/Psychokiller1888/bring-api/tree/master
+
+### Usage
+
+- Import the package in your project
+- Create a Bring instance by passing your login and password to use the API:
+
+```python
+from BringPythonApi.Bring import Bring
+
+try:
+    bring = Bring(email='foo@bar.com', password='foobar')
+except Exception as e:
+    print(f'Error logging in: {e}')
+else:
+    # Add an item to your default list
+    bring.purchase(item='Milk', detail='3 liters')
+    
+    # Remove 1 cat food from your default list
+    bring.remove(item='Cat food', detail=1)
+    
+    # Empty your list called "My work list". If no name provided, defaults to you default list
+    bring.emptyPurchaseList(listUuid=bring.user.getList(name='My work list'))
+
+    # Change the default list language
+    bring.changeUserListLanguage(languageCode='en-US')
+
+    # Change the account password
+    bring.changeUserPassword(newPassword='myNewPassword')
+
+    # Get stats for Cat food
+    bring.getItemStatistic(itemName='Cat food')
+
+    # Get profile picture
+    bring.getUserProfilePicture()
+
+    # Add item to recent list
+    bring.addToRecentItems(item='Milk', detail='2 liters')
+    
+    # Get my work shopping list
+    bring.getShoppingList(listUuid=bring.user.getList(name='Work list'))
+    
+    # Move cucumber to another category
+    bring.changeItemCategory(newCategory='Eigene Artikel')
+
+    # Create a new "Bauhaus" list
+    bring.createNewList(listName='Bauhaus')
+
+    # Add power drill to Bauhaus shopping list
+    bring.purchase(
+        item='Power drill',
+        detail='With bits',
+        listUuid=bring.user.getList(name='Bauhaus')
+    )
+
+    # Create a new "Aldi" list
+    bring.createNewList(listName='Aldi')
+    
+    # Add rice to Aldi's list
+    bring.purchase(
+        item='Rice (1kg)',
+        detail=2,
+        listUuid=bring.user.getList(name='Aldi')
+    )
+```
```

### Comparing `bring-python-api-1.0.1/README.md` & `bring-python-api-1.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,95 @@
-## Bring Python API
-
-This is an unofficial python API for Bring! the shopping list service, based on their webapi. Some endpoints might be missing, this is solely based on traffic capture while using the web app.
-
-
-### API doc
-You'll find the API documentation on this page: https://psychokiller1888.github.io/bring-api/
-
-Please note that sme endpoints might be missing
-
-### Insomnia repository
-Import the repository in your Insomnia app: https://github.com/Psychokiller1888/bring-api/tree/master
-
-### Usage
-
-- Import the package in your project
-- Create a Bring instance by passing your login and password to use the API:
-
-```python
-from BringPythonApi.Bring import Bring
-
-try:
-    bring = Bring(email='foo@bar.com', password='foobar')
-except Exception as e:
-    print(f'Error logging in: {e}')
-else:
-    # Add an item to your default list
-    bring.purchase(item='Milk', detail='3 liters')
-    
-    # Remove 1 cat food from your default list
-    bring.remove(item='Cat food', detail=1)
-    
-    # Empty your list called "My work list". If no name provided, defaults to you default list
-    bring.emptyPurchaseList(listUuid=bring.user.getList(name='My work list'))
-
-    # Change the default list language
-    bring.changeUserListLanguage(languageCode='en-US')
-
-    # Change the account password
-    bring.changeUserPassword(newPassword='myNewPassword')
-
-    # Get stats for Cat food
-    bring.getItemStatistic(itemName='Cat food')
-
-    # Get profile picture
-    bring.getUserProfilePicture()
-
-    # Add item to recent list
-    bring.addToRecentItems(item='Milk', detail='2 liters')
-    
-    # Get my work shopping list
-    bring.getShoppingList(listUuid=bring.user.getList(name='Work list'))
-    
-    # Move cucumber to another category
-    bring.changeItemCategory(newCategory='Eigene Artikel')
-```
+Metadata-Version: 2.1
+Name: bring-python-api
+Version: 1.0.2
+Summary: Bring! web api for Python
+Home-page: https://github.com/Psychokiller1888/bring-api
+Author: Psychokiller1888
+Author-email: laurentchervet@bluewin.ch
+Maintainer: Psychokiller1888
+License: GPL-3.0
+Description: ## Bring Python API
+        
+        This is an unofficial python API for Bring! the shopping list service, based on their webapi. Some endpoints might be missing, this is solely based on traffic capture while using the web app.
+        
+        
+        ### API doc
+        You'll find the API documentation on this page: https://psychokiller1888.github.io/bring-api/
+        
+        Please note that sme endpoints might be missing
+        
+        ### Insomnia repository
+        Import the repository in your Insomnia app: https://github.com/Psychokiller1888/bring-api/tree/master
+        
+        ### Usage
+        
+        - Import the package in your project
+        - Create a Bring instance by passing your login and password to use the API:
+        
+        ```python
+        from BringPythonApi.Bring import Bring
+        
+        try:
+            bring = Bring(email='foo@bar.com', password='foobar')
+        except Exception as e:
+            print(f'Error logging in: {e}')
+        else:
+            # Add an item to your default list
+            bring.purchase(item='Milk', detail='3 liters')
+            
+            # Remove 1 cat food from your default list
+            bring.remove(item='Cat food', detail=1)
+            
+            # Empty your list called "My work list". If no name provided, defaults to you default list
+            bring.emptyPurchaseList(listUuid=bring.user.getList(name='My work list'))
+        
+            # Change the default list language
+            bring.changeUserListLanguage(languageCode='en-US')
+        
+            # Change the account password
+            bring.changeUserPassword(newPassword='myNewPassword')
+        
+            # Get stats for Cat food
+            bring.getItemStatistic(itemName='Cat food')
+        
+            # Get profile picture
+            bring.getUserProfilePicture()
+        
+            # Add item to recent list
+            bring.addToRecentItems(item='Milk', detail='2 liters')
+            
+            # Get my work shopping list
+            bring.getShoppingList(listUuid=bring.user.getList(name='Work list'))
+            
+            # Move cucumber to another category
+            bring.changeItemCategory(newCategory='Eigene Artikel')
+        
+            # Create a new "Bauhaus" list
+            bring.createNewList(listName='Bauhaus')
+        
+            # Add power drill to Bauhaus shopping list
+            bring.purchase(
+                item='Power drill',
+                detail='With bits',
+                listUuid=bring.user.getList(name='Bauhaus')
+            )
+        
+            # Create a new "Aldi" list
+            bring.createNewList(listName='Aldi')
+            
+            # Add rice to Aldi's list
+            bring.purchase(
+                item='Rice (1kg)',
+                detail=2,
+                listUuid=bring.user.getList(name='Aldi')
+            )
+        ```
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `bring-python-api-1.0.1/bring_python_api.egg-info/PKG-INFO` & `bring-python-api-1.0.2/bring_python_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-python-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bring! web api for Python
 Home-page: https://github.com/Psychokiller1888/bring-api
 Author: Psychokiller1888
 Author-email: laurentchervet@bluewin.ch
 Maintainer: Psychokiller1888
 License: GPL-3.0
 Description: ## Bring Python API
@@ -58,14 +58,34 @@
             bring.addToRecentItems(item='Milk', detail='2 liters')
             
             # Get my work shopping list
             bring.getShoppingList(listUuid=bring.user.getList(name='Work list'))
             
             # Move cucumber to another category
             bring.changeItemCategory(newCategory='Eigene Artikel')
+        
+            # Create a new "Bauhaus" list
+            bring.createNewList(listName='Bauhaus')
+        
+            # Add power drill to Bauhaus shopping list
+            bring.purchase(
+                item='Power drill',
+                detail='With bits',
+                listUuid=bring.user.getList(name='Bauhaus')
+            )
+        
+            # Create a new "Aldi" list
+            bring.createNewList(listName='Aldi')
+            
+            # Add rice to Aldi's list
+            bring.purchase(
+                item='Rice (1kg)',
+                detail=2,
+                listUuid=bring.user.getList(name='Aldi')
+            )
         ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `bring-python-api-1.0.1/setup.py` & `bring-python-api-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
 	name='bring-python-api',
-	version='1.0.1',
+	version='1.0.2',
 	long_description=Path('README.md').read_text(encoding='utf8'),
 	long_description_content_type='text/markdown',
 	python_requires='>=3.8',
 	packages=find_packages(),
 	include_package_data=True,
 	url='https://github.com/Psychokiller1888/bring-api',
 	license='GPL-3.0',
```

