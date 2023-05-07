# Comparing `tmp/masedb-1.1.8.tar.gz` & `tmp/masedb-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\masedb-1.1.8.tar", last modified: Sat May  6 18:10:40 2023, max compression
+gzip compressed data, was "dist\masedb-1.2.1.tar", last modified: Sun May  7 11:12:53 2023, max compression
```

## Comparing `masedb-1.1.8.tar` & `masedb-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:10:40.000000 masedb-1.1.8/
--rw-rw-rw-   0        0        0     2290 2023-05-06 01:50:34.000000 masedb-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     3078 2023-05-06 18:10:40.000000 masedb-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2953 2023-05-06 09:36:32.000000 masedb-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 18:10:40.000000 masedb-1.1.8/masedb/
--rw-rw-rw-   0        0        0       47 2023-05-06 18:05:49.000000 masedb-1.1.8/masedb/exceptions.py
--rw-rw-rw-   0        0        0     4548 2023-05-06 18:06:40.000000 masedb-1.1.8/masedb/queries.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:10:40.000000 masedb-1.1.8/masedb.egg-info/
--rw-rw-rw-   0        0        0     3078 2023-05-06 18:10:38.000000 masedb-1.1.8/masedb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-06 18:10:38.000000 masedb-1.1.8/masedb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:10:38.000000 masedb-1.1.8/masedb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-06 18:10:38.000000 masedb-1.1.8/masedb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 18:10:38.000000 masedb-1.1.8/masedb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 02:35:52.000000 masedb-1.1.8/masedb.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-06 18:10:40.000000 masedb-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     3337 2023-05-06 18:09:05.000000 masedb-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 11:12:53.000000 masedb-1.2.1/
+-rw-rw-rw-   0        0        0     2290 2023-05-06 01:50:34.000000 masedb-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2661 2023-05-07 11:12:53.000000 masedb-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-05-07 11:11:27.000000 masedb-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 11:12:53.000000 masedb-1.2.1/masedb/
+-rw-rw-rw-   0        0        0       47 2023-05-06 18:05:49.000000 masedb-1.2.1/masedb/exceptions.py
+-rw-rw-rw-   0        0        0     4548 2023-05-07 10:12:32.000000 masedb-1.2.1/masedb/queries.py
+-rw-rw-rw-   0        0        0     3477 2023-05-07 10:57:17.000000 masedb-1.2.1/masedb/query.py
+drwxrwxrwx   0        0        0        0 2023-05-07 11:12:53.000000 masedb-1.2.1/masedb.egg-info/
+-rw-rw-rw-   0        0        0     2661 2023-05-07 11:12:50.000000 masedb-1.2.1/masedb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-07 11:12:51.000000 masedb-1.2.1/masedb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 11:12:50.000000 masedb-1.2.1/masedb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-07 11:12:50.000000 masedb-1.2.1/masedb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 11:12:50.000000 masedb-1.2.1/masedb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 02:35:52.000000 masedb-1.2.1/masedb.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-07 11:12:53.000000 masedb-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2920 2023-05-07 11:11:12.000000 masedb-1.2.1/setup.py
```

### Comparing `masedb-1.1.8/LICENSE` & `masedb-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `masedb-1.1.8/PKG-INFO` & `masedb-1.2.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,27 @@
-Metadata-Version: 2.1
-Name: masedb
-Version: 1.1.8
-Summary: Easy mase-db use mongodb, motor asyncio
-Home-page: https://github.com/MaseZev/Mase-DB
-Author: MaseZev
-Author-email: csgomanagement1@gmail.com
-License: mit
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+from setuptools import setup
+import re
 
-<h1 align=center>Mase-DB v1.1.8</h1>
+readme = '''<h1 align=center>Mase-DB v1.2.1</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
-##Документация
+## Документация
 
 Документация:
- - Скоро будет!
+ - [docs](https://mase-db.gitbook.io/docs/)
 
 ## Установка
 ```py
 # ЕСЛИ УСТНОВЛЕН
 pip install --upgrade masedb
 
 # ЕСЛИ НЕ УСТАНОВЛЕН
 python3 -m pip install --upgrade masedb
 ```
-##or
+## or
 ```py
 pip install masedb
 ```
 
 ## Применение
 ### Предпосылки
 Прежде чем приступить к работе, вам понадобится несколько вещей:
@@ -38,57 +29,77 @@
  - Так же установить masedb 
  - И понять как это все работает
  
  И так поехали!(жабы топ)
 
 ### Примеры
 ```py
-from masedb.queries import *
 from config import url
+from masedb.query import Query
 import asyncio
 
 #--------------------------------------------------------------------------------------------------------------------------------------------------------
 
-#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
-#await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
-#await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name': 'mark'}, param2={'$set':{'let': 10}})
-#await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
+#client = Query(DatabaseName, CollectionName, url.uri)
+
+#await client.find(param={'name': 'mark'})
+#await client.insert(param={'name': 'mark'})
+#await client.update(param1={'name': 'mark'}, param2={'$set':{'let': 10}})
+#await client.delete(param={'cash': 10})
 
 #--------------------------------------------------------------------------------------------------------------------------------------------------------
 
 #     Название базы данных и колекции
 
 DatabaseName = 'pondb2'
 CollectionName = 'poncoll2'
 
 
 #--------------------------------------------------------------------------------------------------------------------------------------------------------
 
+client = Query(DatabaseName, CollectionName, url.uri)
+
 async def test():
 
-	db = await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
+	db = await client.find(param={'name': 'mark'})
 	print(db)
 
 	if not db:
 		print('занесение')
 
-		return await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name':'mark'})
+		return await client.insert(param={'name':'mark'})
 
 	try: cash = db['cash']
 	except: cash = None
 
-	await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
+	await client.delete(param={'cash': 10})
 
 	if not cash:
 		print('update data')
-		return await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name':'mark'}, param2={'$set':{'cash': 10}})
+		return await client.update(param1={'name':'mark'}, param2={'$set':{'cash': 10}})
 
 	print(cash)
 
 asyncio.run(test())
 
 
-
 ```
 
 
 <br>
+'''
+
+requirements = ["pymongo","dnspython","motor"]
+
+setup(name='masedb',
+      version='1.2.1',
+      description='Easy mase-db use mongodb, motor asyncio',
+      url='https://github.com/MaseZev/Mase-DB',
+      packages=['masedb'],
+      license='mit',
+      author="MaseZev",
+      author_email='csgomanagement1@gmail.com',
+      long_description=readme,
+      long_description_content_type="text/markdown",
+      install_requires=requirements,
+      python_requires='>=3.7',
+      zip_safe=True)
```

### Comparing `masedb-1.1.8/masedb/queries.py` & `masedb-1.2.1/masedb/queries.py`

 * *Files identical despite different names*

