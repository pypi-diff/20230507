# Comparing `tmp/eth-accounts-index-0.5.1.tar.gz` & `tmp/eth-accounts-index-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-accounts-index-0.5.1.tar", last modified: Sun Mar 26 07:13:25 2023, max compression
+gzip compressed data, was "eth-accounts-index-0.5.2.tar", last modified: Sat May  6 22:02:07 2023, max compression
```

## Comparing `eth-accounts-index-0.5.1.tar` & `eth-accounts-index-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:13:25.579993 eth-accounts-index-0.5.1/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-03-22 12:10:40.000000 eth-accounts-index-0.5.1/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       55 2021-08-24 19:20:29.000000 eth-accounts-index-0.5.1/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      778 2023-03-26 07:13:25.579993 eth-accounts-index-0.5.1/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:13:25.576660 eth-accounts-index-0.5.1/eth_accounts_index/
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-30 11:12:04.000000 eth-accounts-index-0.5.1/eth_accounts_index/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:13:25.576660 eth-accounts-index-0.5.1/eth_accounts_index/data/
--rw-r--r--   0 lash      (1000) lash      (1000)    14348 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.1/eth_accounts_index/data/AccountsIndex.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     3975 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.1/eth_accounts_index/data/AccountsIndex.json
--rw-r--r--   0 lash      (1000) lash      (1000)     4670 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.1/eth_accounts_index/data/AccountsIndex.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)     5377 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.1/eth_accounts_index/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2083 2023-02-05 04:53:47.000000 eth-accounts-index-0.5.1/eth_accounts_index/registry.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:13:25.579993 eth-accounts-index-0.5.1/eth_accounts_index/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-02-12 07:50:27.000000 eth-accounts-index-0.5.1/eth_accounts_index/runnable/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2560 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.1/eth_accounts_index/runnable/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3037 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.1/eth_accounts_index/runnable/list.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2289 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.1/eth_accounts_index/runnable/publish.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:13:25.576660 eth-accounts-index-0.5.1/eth_accounts_index.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      778 2023-03-26 07:13:25.000000 eth-accounts-index-0.5.1/eth_accounts_index.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      730 2023-03-26 07:13:25.000000 eth-accounts-index-0.5.1/eth_accounts_index.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-26 07:13:25.000000 eth-accounts-index-0.5.1/eth_accounts_index.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      215 2023-03-26 07:13:25.000000 eth-accounts-index-0.5.1/eth_accounts_index.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       97 2023-03-26 07:13:25.000000 eth-accounts-index-0.5.1/eth_accounts_index.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       19 2023-03-26 07:13:25.000000 eth-accounts-index-0.5.1/eth_accounts_index.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       35 2023-02-04 10:13:04.000000 eth-accounts-index-0.5.1/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1188 2023-03-26 07:13:25.579993 eth-accounts-index-0.5.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      467 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.1/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-14 06:33:34.000000 eth-accounts-index-0.5.1/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:13:25.579993 eth-accounts-index-0.5.1/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     8652 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.1/tests/test_app.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-03-22 12:10:40.000000 eth-accounts-index-0.5.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       55 2021-08-24 19:20:29.000000 eth-accounts-index-0.5.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      778 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/eth_accounts_index/
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-30 11:12:04.000000 eth-accounts-index-0.5.2/eth_accounts_index/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/eth_accounts_index/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)    14348 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     3975 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     4670 2023-03-26 07:13:10.000000 eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     5377 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/eth_accounts_index/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2083 2023-02-05 04:53:47.000000 eth-accounts-index-0.5.2/eth_accounts_index/registry.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/eth_accounts_index/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-02-12 07:50:27.000000 eth-accounts-index-0.5.2/eth_accounts_index/runnable/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2560 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/eth_accounts_index/runnable/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3037 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/eth_accounts_index/runnable/list.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2289 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/eth_accounts_index/runnable/publish.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      778 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      730 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      215 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       97 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       19 2023-05-06 22:02:07.000000 eth-accounts-index-0.5.2/eth_accounts_index.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       35 2023-02-04 10:13:04.000000 eth-accounts-index-0.5.2/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1188 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      467 2023-02-12 14:04:06.000000 eth-accounts-index-0.5.2/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-14 06:33:34.000000 eth-accounts-index-0.5.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-06 22:02:07.146456 eth-accounts-index-0.5.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     7828 2023-05-06 21:56:46.000000 eth-accounts-index-0.5.2/tests/test_app.py
```

### Comparing `eth-accounts-index-0.5.1/LICENSE` & `eth-accounts-index-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/PKG-INFO` & `eth-accounts-index-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-accounts-index
-Version: 0.5.1
+Version: 0.5.2
 Summary: Accounts index evm contract tooling with permissioned writes
 Home-page: https://holbrook.no/src/eth-accounts-index/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: ethereum
 Platform: UNKNOWN
```

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index/data/AccountsIndex.bin` & `eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.bin`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index/data/AccountsIndex.json` & `eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.json`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index/data/AccountsIndex.metadata.json` & `eth-accounts-index-0.5.2/eth_accounts_index/data/AccountsIndex.metadata.json`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index/interface.py` & `eth-accounts-index-0.5.2/eth_accounts_index/interface.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index/registry.py` & `eth-accounts-index-0.5.2/eth_accounts_index/registry.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index/runnable/add.py` & `eth-accounts-index-0.5.2/eth_accounts_index/runnable/add.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index/runnable/list.py` & `eth-accounts-index-0.5.2/eth_accounts_index/runnable/list.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index/runnable/publish.py` & `eth-accounts-index-0.5.2/eth_accounts_index/runnable/publish.py`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index.egg-info/PKG-INFO` & `eth-accounts-index-0.5.2/eth_accounts_index.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-accounts-index
-Version: 0.5.1
+Version: 0.5.2
 Summary: Accounts index evm contract tooling with permissioned writes
 Home-page: https://holbrook.no/src/eth-accounts-index/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: ethereum
 Platform: UNKNOWN
```

### Comparing `eth-accounts-index-0.5.1/eth_accounts_index.egg-info/SOURCES.txt` & `eth-accounts-index-0.5.2/eth_accounts_index.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-accounts-index-0.5.1/setup.cfg` & `eth-accounts-index-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-accounts-index
-version = 0.5.1
+version = 0.5.2
 description = Accounts index evm contract tooling with permissioned writes
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/eth-accounts-index/log.html
 keywords = 
 	ethereum
 classifiers =
```

### Comparing `eth-accounts-index-0.5.1/tests/test_app.py` & `eth-accounts-index-0.5.2/tests/test_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,54 +22,26 @@
         block_latest,
         block_by_number,
         )
 
 # local imports
 from eth_accounts_index.registry import AccountRegistry
 from eth_accounts_index import AccountsIndex
+from eth_accounts_index.unittest import TestAccountsIndex
 
 logging.basicConfig(level=logging.DEBUG)
 logg = logging.getLogger()
 
 testdir = os.path.dirname(__file__)
 
 
-class TestNonceOracle:
-
-    def __init__(self, address, default_value=0):
-        self.nonce = default_value
-
-
-    def next_nonce(self):
-        nonce = self.nonce
-        self.nonce += 1
-        return nonce
-
-
-class Test(EthTesterCase):
+class Test(TestAccountsIndex):
 
     def setUp(self):
         super(Test, self).setUp()
-        nonce_oracle = TestNonceOracle(self.accounts[0])
-        c = AccountRegistry(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
-        (tx_hash, o) = c.constructor(self.accounts[0])
-        self.conn = RPCConnection.connect(self.chain_spec, 'default')
-        r = self.conn.do(o)
-        logg.debug(f'published with hash {r}')
-
-        o = receipt(r)
-        r = self.conn.do(o)
-        self.address = to_checksum_address(r['contract_address'])
-
-        (tx_hash, o) = c.add_writer(self.address, self.accounts[0], self.accounts[0])
-        r = self.conn.do(o)
-
-        o = receipt(r)
-        r = self.conn.do(o)
-        self.assertEqual(r['status'], 1)
 
 
     def test_1_count(self):
         #o = self.o.count(self.address, sender_address=self.accounts[0])
         c = AccountsIndex(self.chain_spec)
         o = c.entry_count(self.address, sender_address=self.accounts[0])
         r = self.conn.do(o)
```

