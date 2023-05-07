# Comparing `tmp/dxsp-2.0.0.tar.gz` & `tmp/dxsp-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.0.tar", max compression
+gzip compressed data, was "dxsp-2.0.1.tar", max compression
```

## Comparing `dxsp-2.0.0.tar` & `dxsp-2.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-07 16:22:16.549232 dxsp-2.0.0/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-07 16:22:16.549232 dxsp-2.0.0/README.md
--rw-r--r--   0        0        0       38 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/.gitignore
--rw-r--r--   0        0        0       86 2023-05-07 16:22:17.225232 dxsp-2.0.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/config.py
--rw-r--r--   0        0        0     2967 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26204 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/main.py
--rw-r--r--   0        0        0     1769 2023-05-07 16:22:17.225232 dxsp-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-07 17:55:16.842321 dxsp-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-07 17:55:16.842321 dxsp-2.0.1/README.md
+-rw-r--r--   0        0        0       38 2023-05-07 17:55:16.842321 dxsp-2.0.1/dxsp/.gitignore
+-rw-r--r--   0        0        0       86 2023-05-07 17:55:17.502320 dxsp-2.0.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-07 17:55:16.842321 dxsp-2.0.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-07 17:55:16.842321 dxsp-2.0.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-07 17:55:16.842321 dxsp-2.0.1/dxsp/config.py
+-rw-r--r--   0        0        0     2967 2023-05-07 17:55:16.842321 dxsp-2.0.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26184 2023-05-07 17:55:16.846321 dxsp-2.0.1/dxsp/main.py
+-rw-r--r--   0        0        0     1769 2023-05-07 17:55:17.502320 dxsp-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.1/PKG-INFO
```

### Comparing `dxsp-2.0.0/LICENSE` & `dxsp-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.0/README.md` & `dxsp-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.0/dxsp/assets/blockchains.py` & `dxsp-2.0.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.0/dxsp/default_settings.toml` & `dxsp-2.0.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.0/dxsp/main.py` & `dxsp-2.0.1/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,39 +2,38 @@
  DEX SWAP Main
 """
 
 import logging
 
 import requests
 from dxsp import __version__
-# from dxsp.assets.blockchains import blockchains
 from dxsp.config import settings
 
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 
 
 class DexSwap:
     """Do a swap."""
 
     def __init__(self, w3: Web3 | None = None,):
         """build a dex object """
         self.logger = logging.getLogger(name="DexSwap")
-        self.logger.info("DexSwap version: %s", __version__)
+        self.logger.info("DexSwap: %s", __version__)
 
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         try:
             if self.w3.net.listening:
-                self.logger.info("connected to %s", self.w3)
+                self.logger.info("connected %s", self.w3)
         except Exception as e:
             self.logger.error("connectivity failed %s", e)
             return
 
         self.protocol_type = settings.dex_protocol_type
-
+        self.chain_id = settings.chain_id
         # USER SECRET
         self.wallet_address = settings.dex_wallet_address
         self.private_key = settings.dex_private_key
 
         # COINGECKO
         try:
             self.cg = CoinGeckoAPI()
```

### Comparing `dxsp-2.0.0/pyproject.toml` & `dxsp-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.0"
+version = "2.0.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.0.0/PKG-INFO` & `dxsp-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.0
+Version: 2.0.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

