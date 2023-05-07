# Comparing `tmp/cardano-nft-vending-machine-0.7.0.tar.gz` & `tmp/cardano-nft-vending-machine-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-ghk_ag8n/cardano-nft-vending-machine-0.7.0.tar", last modified: Sat May  6 17:50:48 2023, max compression
+gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-gbttx_9q/cardano-nft-vending-machine-0.7.1.tar", last modified: Sun May  7 16:30:51 2023, max compression
```

## Comparing `cardano-nft-vending-machine-0.7.0.tar` & `cardano-nft-vending-machine-0.7.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.674536 cardano-nft-vending-machine-0.7.0/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.7.0/LICENSE
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13134 2023-05-06 17:50:48.674041 cardano-nft-vending-machine-0.7.0/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12474 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.0/README.md
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-05-05 03:11:27.000000 cardano-nft-vending-machine-0.7.0/pyproject.toml
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-05-06 17:50:48.674697 cardano-nft-vending-machine-0.7.0/setup.cfg
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.660414 cardano-nft-vending-machine-0.7.0/src/
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.662286 cardano-nft-vending-machine-0.7.0/src/cardano/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.7.0/src/cardano/__init__.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.665296 cardano-nft-vending-machine-0.7.0/src/cardano/wt/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5054 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/blockfrost.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.666368 cardano-nft-vending-machine-0.7.0/src/cardano/wt/bonuses/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/bonuses/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/bonuses/bogo.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     3931 2023-05-06 03:37:44.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/cardano_cli.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5604 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/mint.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       40 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/network.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11029 2023-05-06 03:12:13.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/nft_vending_machine.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/utxo.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.670117 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/asset_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2503 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/filesystem.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/no_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/wallet_whitelist.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.673272 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13134 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      798 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/requires.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/top_level.txt
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-07 16:30:51.996293 cardano-nft-vending-machine-0.7.1/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.7.1/LICENSE
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13134 2023-05-07 16:30:51.995658 cardano-nft-vending-machine-0.7.1/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12474 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.1/README.md
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-05-07 16:30:36.000000 cardano-nft-vending-machine-0.7.1/pyproject.toml
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-05-07 16:30:51.996496 cardano-nft-vending-machine-0.7.1/setup.cfg
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-07 16:30:51.979900 cardano-nft-vending-machine-0.7.1/src/
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-07 16:30:51.982457 cardano-nft-vending-machine-0.7.1/src/cardano/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.7.1/src/cardano/__init__.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-07 16:30:51.986271 cardano-nft-vending-machine-0.7.1/src/cardano/wt/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5054 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/blockfrost.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-07 16:30:51.987600 cardano-nft-vending-machine-0.7.1/src/cardano/wt/bonuses/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/bonuses/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/bonuses/bogo.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     3931 2023-05-06 03:37:44.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/cardano_cli.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5604 2023-05-07 16:27:55.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/mint.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       40 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/network.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11029 2023-05-06 03:12:13.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/nft_vending_machine.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/utxo.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-07 16:30:51.991253 cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/asset_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2503 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/filesystem.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/no_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/wallet_whitelist.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-07 16:30:51.994655 cardano-nft-vending-machine-0.7.1/src/cardano_nft_vending_machine.egg-info/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13134 2023-05-07 16:30:51.000000 cardano-nft-vending-machine-0.7.1/src/cardano_nft_vending_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      798 2023-05-07 16:30:51.000000 cardano-nft-vending-machine-0.7.1/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-05-07 16:30:51.000000 cardano-nft-vending-machine-0.7.1/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-05-07 16:30:51.000000 cardano-nft-vending-machine-0.7.1/src/cardano_nft_vending_machine.egg-info/requires.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-05-07 16:30:51.000000 cardano-nft-vending-machine-0.7.1/src/cardano_nft_vending_machine.egg-info/top_level.txt
```

### Comparing `cardano-nft-vending-machine-0.7.0/LICENSE` & `cardano-nft-vending-machine-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/PKG-INFO` & `cardano-nft-vending-machine-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.7.0
+Version: 0.7.1
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.7.0 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.7.1 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
```

### Comparing `cardano-nft-vending-machine-0.7.0/README.md` & `cardano-nft-vending-machine-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/pyproject.toml` & `cardano-nft-vending-machine-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.3.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cardano-nft-vending-machine"
-version = "0.7.0"
+version = "0.7.1"
 
 description = "Library to perform NFT mints automatically on the Cardano blockchain"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/blockfrost.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/blockfrost.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/cardano_cli.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/cardano_cli.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/mint.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/mint.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         self.nfts_dir = nfts_dir
         self.scripts = scripts
         self.sign_keys = sign_keys
         self.whitelist = whitelist
         self.bogo = bogo
 
         after_slots = list(filter(None, [Mint.__read_validator('after', 'slot', script) for script in self.scripts]))
-        self.initial_slot = min(after_slots) if after_slots else None
+        self.initial_slot = max(after_slots) if after_slots else None
         before_slots = list(filter(None, [Mint.__read_validator('before', 'slot', script) for script in self.scripts]))
-        self.expiration_slot = max(before_slots) if before_slots else None
+        self.expiration_slot = min(before_slots) if before_slots else None
 
     def validate(self):
         if self.dev_fee and self.dev_fee < Utxo.MIN_UTXO_VALUE:
             raise ValueError(f"Thank you for offering to pay your dev {self.dev_fee} but the minUTxO on Cardano is {Utxo.MIN_UTXO_VALUE} lovelace")
         if self.dev_fee and not self.dev_addr:
             raise ValueError(f"Thank you for offering to pay your dev {self.dev_fee} but you did not provide a dev address")
         if self.price and self.price < Mint._MIN_PRICE:
```

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/nft_vending_machine.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/nft_vending_machine.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/utxo.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/utxo.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/asset_whitelist.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/asset_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/filesystem.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/filesystem.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/no_whitelist.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/no_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/wallet_whitelist.py` & `cardano-nft-vending-machine-0.7.1/src/cardano/wt/whitelist/wallet_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/PKG-INFO` & `cardano-nft-vending-machine-0.7.1/src/cardano_nft_vending_machine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.7.0
+Version: 0.7.1
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.7.0 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.7.1 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
```

### Comparing `cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/SOURCES.txt` & `cardano-nft-vending-machine-0.7.1/src/cardano_nft_vending_machine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

