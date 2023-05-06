# Comparing `tmp/eth-accounts-index-0.5.2.tar.gz` & `tmp/eth-accounts-index-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-accounts-index-0.5.2.tar", last modified: Sat May  6 22:02:07 2023, max compression
+gzip compressed data, was "eth-accounts-index-0.5.3.tar", last modified: Sat May  6 23:02:34 2023, max compression
```

## Comparing `eth-accounts-index-0.5.2.tar` & `eth-accounts-index-0.5.3.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-03-22 12:10:40.000000 eth-accounts-index-0.5.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       55 2021-08-24 19:20:29.000000 eth-accounts-index-0.5.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      778 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/eth_accounts_index/
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-30 11:12:04.000000 eth-accounts-index-0.5.2/eth_accounts_index/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/eth_accounts_index/data/
--rw-r--r--   0 lash      (1000) lash      (1000)    14348 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     3975 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.json
--rw-r--r--   0 lash      (1000) lash      (1000)     4670 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)     5377 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/eth_accounts_index/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2083 2023-02-05 04:53:47.000000 eth-accounts-index-0.5.2/eth_accounts_index/registry.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/eth_accounts_index/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-02-12 07:50:27.000000 eth-accounts-index-0.5.2/eth_accounts_index/runnable/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2560 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/eth_accounts_index/runnable/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3037 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/eth_accounts_index/runnable/list.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2289 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/eth_accounts_index/runnable/publish.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      778 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      730 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      215 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       97 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       19 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       35 2023-02-04 10:13:04.000000 eth-accounts-index-0.5.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1188 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      467 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-14 06:33:34.000000 eth-accounts-index-0.5.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     7828 2023-05-06 21:56:46.000000 eth-accounts-index-0.5.2/tests/test_app.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-03-22 12:10:40.000000 eth-accounts-index-0.5.3/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       55 2021-08-24 19:20:29.000000 eth-accounts-index-0.5.3/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      750 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/eth_accounts_index/
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-30 11:12:04.000000 eth-accounts-index-0.5.3/eth_accounts_index/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/eth_accounts_index/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)    14348 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.3/eth_accounts_index/data/AccountsIndex.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     3975 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.3/eth_accounts_index/data/AccountsIndex.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     4670 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.3/eth_accounts_index/data/AccountsIndex.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     5377 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.3/eth_accounts_index/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2083 2023-02-05 04:53:47.000000 eth-accounts-index-0.5.3/eth_accounts_index/registry.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/eth_accounts_index/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-02-12 07:50:27.000000 eth-accounts-index-0.5.3/eth_accounts_index/runnable/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2560 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.3/eth_accounts_index/runnable/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3037 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.3/eth_accounts_index/runnable/list.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2289 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.3/eth_accounts_index/runnable/publish.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/eth_accounts_index/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       36 2023-05-06 21:53:18.000000 eth-accounts-index-0.5.3/eth_accounts_index/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1204 2023-05-06 22:01:06.000000 eth-accounts-index-0.5.3/eth_accounts_index/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/eth_accounts_index.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      750 2023-05-06 23:02:34.000000 eth-accounts-index-0.5.3/eth_accounts_index.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      806 2023-05-06 23:02:34.000000 eth-accounts-index-0.5.3/eth_accounts_index.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-06 23:02:34.000000 eth-accounts-index-0.5.3/eth_accounts_index.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      214 2023-05-06 23:02:34.000000 eth-accounts-index-0.5.3/eth_accounts_index.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       97 2023-05-06 23:02:34.000000 eth-accounts-index-0.5.3/eth_accounts_index.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       19 2023-05-06 23:02:34.000000 eth-accounts-index-0.5.3/eth_accounts_index.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       35 2023-02-04 10:13:04.000000 eth-accounts-index-0.5.3/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1217 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      467 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.3/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-14 06:33:34.000000 eth-accounts-index-0.5.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 23:02:34.515455 eth-accounts-index-0.5.3/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     7828 2023-05-06 21:56:46.000000 eth-accounts-index-0.5.3/tests/test_app.py
```

### Comparing `eth-accounts-index-0.5.2/LICENSE` & `eth-accounts-index-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/PKG-INFO` & `eth-accounts-index-0.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: eth-accounts-index
-Version: 0.5.2
+Version: 0.5.3
 Summary: Accounts index evm contract tooling with permissioned writes
 Home-page: https://holbrook.no/src/eth-accounts-index/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Provides-Extra: testing
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.bin` & `eth-accounts-index-0.5.3/eth_accounts_index/data/AccountsIndex.bin`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.json` & `eth-accounts-index-0.5.3/eth_accounts_index/data/AccountsIndex.json`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.metadata.json` & `eth-accounts-index-0.5.3/eth_accounts_index/data/AccountsIndex.metadata.json`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index/interface.py` & `eth-accounts-index-0.5.3/eth_accounts_index/interface.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index/registry.py` & `eth-accounts-index-0.5.3/eth_accounts_index/registry.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index/runnable/add.py` & `eth-accounts-index-0.5.3/eth_accounts_index/runnable/add.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index/runnable/list.py` & `eth-accounts-index-0.5.3/eth_accounts_index/runnable/list.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index/runnable/publish.py` & `eth-accounts-index-0.5.3/eth_accounts_index/runnable/publish.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index.egg-info/PKG-INFO` & `eth-accounts-index-0.5.3/eth_accounts_index.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: eth-accounts-index
-Version: 0.5.2
+Version: 0.5.3
 Summary: Accounts index evm contract tooling with permissioned writes
 Home-page: https://holbrook.no/src/eth-accounts-index/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Provides-Extra: testing
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `eth-accounts-index-0.5.2/eth_accounts_index.egg-info/SOURCES.txt` & `eth-accounts-index-0.5.3/eth_accounts_index.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 eth_accounts_index/data/AccountsIndex.bin
 eth_accounts_index/data/AccountsIndex.json
 eth_accounts_index/data/AccountsIndex.metadata.json
 eth_accounts_index/runnable/__init__.py
 eth_accounts_index/runnable/add.py
 eth_accounts_index/runnable/list.py
 eth_accounts_index/runnable/publish.py
+eth_accounts_index/unittest/__init__.py
+eth_accounts_index/unittest/base.py
 tests/test_app.py
```

### Comparing `eth-accounts-index-0.5.2/setup.cfg` & `eth-accounts-index-0.5.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-accounts-index
-version = 0.5.2
+version = 0.5.3
 description = Accounts index evm contract tooling with permissioned writes
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/eth-accounts-index/log.html
 keywords = 
 	ethereum
 classifiers = 
@@ -22,14 +22,15 @@
 
 [options]
 include_package_data = True
 python_requires = >= 3.8
 packages = 
 	eth_accounts_index
 	eth_accounts_index.runnable
+	eth_accounts_index.unittest
 
 [options.extras_require]
 testing = 
 	pytest==6.0.1
 	eth-tester==0.5.0b2
 	py-evm==0.3.0a20
```

### Comparing `eth-accounts-index-0.5.2/tests/test_app.py` & `eth-accounts-index-0.5.3/tests/test_app.py`

 * *Files identical despite different names*

