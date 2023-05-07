# Comparing `tmp/dxsp-2.0.4.tar.gz` & `tmp/dxsp-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.4.tar", max compression
+gzip compressed data, was "dxsp-2.0.5.tar", max compression
```

## Comparing `dxsp-2.0.4.tar` & `dxsp-2.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-07 20:04:55.556050 dxsp-2.0.4/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-07 20:04:55.556050 dxsp-2.0.4/README.md
--rw-r--r--   0        0        0       86 2023-05-07 20:04:56.360065 dxsp-2.0.4/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/config.py
--rw-r--r--   0        0        0     2967 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26224 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-07 20:04:56.360065 dxsp-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-07 20:42:37.754900 dxsp-2.0.5/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-07 20:42:37.754900 dxsp-2.0.5/README.md
+-rw-r--r--   0        0        0       86 2023-05-07 20:42:38.446911 dxsp-2.0.5/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/config.py
+-rw-r--r--   0        0        0     2967 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26307 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-07 20:42:38.442911 dxsp-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.5/PKG-INFO
```

### Comparing `dxsp-2.0.4/LICENSE` & `dxsp-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.4/README.md` & `dxsp-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.4/dxsp/assets/blockchains.py` & `dxsp-2.0.5/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.4/dxsp/default_settings.toml` & `dxsp-2.0.5/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.4/dxsp/main.py` & `dxsp-2.0.5/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,16 +130,17 @@
     async def uniswap_v2_quote(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
         order_path_dex = [asset_out_address, asset_in_address]
+        router_instance = await self.router()
         order_min_amount = int(
-            self.router().functions.getAmountsOut(
+            router_instance.functions.getAmountsOut(
                 amount,
                 order_path_dex)
             .call()[1])
         return order_min_amount
 
     async def uniswap_v3_quote(
         self,
@@ -299,24 +300,25 @@
     ):
         order_path_dex = [asset_out_address, asset_in_address]
 
         deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
         order_min_amount = self.uniswap_v2_quote(
             asset_in_address,
             asset_out_address)
-        swap_order = self.router().functions.swapExactTokensForTokens(
+        router_instance = await self.router()
+        swap_order = router_instance.functions.swapExactTokensForTokens(
                         amount,
                         order_min_amount,
                         order_path_dex,
                         self.wallet_address,
                         deadline)
         return swap_order
 
     async def uniswap_v3_swap(self):
-        self.logger.debug("Not available")
+        self.logger.warning("Not available")
         return
 
     async def get_confirmation(self,
                                order_hash,
                                order_hash_details,
                                asset_out_symbol,
                                asset_out_address,
@@ -385,17 +387,17 @@
                 self.logger.info("token_contract found %s", token_contract)
                 return self.w3.to_checksum_address(token_contract)
             self.logger.info("no contract found for %s", token)
         except Exception as e:
             self.logger.error("search_contract %s", e)
             return
 
-    async def search_gecko(self, token):
+    async def search_cg(self, token):
         """search coingecko"""
-        self.logger.debug("search_gecko")
+        self.logger.debug("search_cg")
         try:
             search_results = self.cg.search(query=token)
             search_dict = search_results['coins']
             filtered_dict = [x for x in search_dict if
                              x['symbol'] == token.upper()]
             api_dict = [sub['api_symbol'] for sub in filtered_dict]
             self.logger.debug("api_dict %s", api_dict)
@@ -403,26 +405,26 @@
                 coin_dict = self.cg.get_coin_by_id(i)
                 try:
                     if coin_dict['platforms'][f'{self.cg_platform}']:
                         return coin_dict
                 except KeyError:
                     pass
         except Exception as e:
-            self.logger.error("search_gecko %s", e)
+            self.logger.error("search_cg %s", e)
             return
 
     async def search_cg_contract(self, token):
         """search coingecko contract"""
         self.logger.debug("🦎search_cg_contract %s", token)
         try:
-            coin_info = await self.search_gecko(token)
+            coin_info = await self.search_cg(token)
             if coin_info is not None:
                 return coin_info['platforms'][f'{self.cg_platform}']
         except Exception as e:
-            self.logger.error(f"error search_cg_contract {e}")
+            self.logger.error(" search_cg_contract: %s", e)
             return
 
     async def get_contract_address(
                             self,
                             token_list_url,
                             symbol
                         ):
```

### Comparing `dxsp-2.0.4/pyproject.toml` & `dxsp-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.4"
+version = "2.0.5"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.0.4/PKG-INFO` & `dxsp-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.4
+Version: 2.0.5
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

