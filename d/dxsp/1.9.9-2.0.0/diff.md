# Comparing `tmp/dxsp-1.9.9.tar.gz` & `tmp/dxsp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.9.9.tar", max compression
+gzip compressed data, was "dxsp-2.0.0.tar", max compression
```

## Comparing `dxsp-1.9.9.tar` & `dxsp-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-06 15:58:19.476954 dxsp-1.9.9/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-06 15:58:19.476954 dxsp-1.9.9/README.md
--rw-r--r--   0        0        0       38 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-06 15:58:20.268993 dxsp-1.9.9/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/config.py
--rw-r--r--   0        0        0      581 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28290 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/main.py
--rw-r--r--   0        0        0     1787 2023-05-06 15:58:20.268993 dxsp-1.9.9/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-07 16:22:16.549232 dxsp-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-07 16:22:16.549232 dxsp-2.0.0/README.md
+-rw-r--r--   0        0        0       38 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/.gitignore
+-rw-r--r--   0        0        0       86 2023-05-07 16:22:17.225232 dxsp-2.0.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/config.py
+-rw-r--r--   0        0        0     2967 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26204 2023-05-07 16:22:16.549232 dxsp-2.0.0/dxsp/main.py
+-rw-r--r--   0        0        0     1769 2023-05-07 16:22:17.225232 dxsp-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.0/PKG-INFO
```

### Comparing `dxsp-1.9.9/LICENSE` & `dxsp-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.9/README.md` & `dxsp-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.9/dxsp/assets/blockchains.py` & `dxsp-2.0.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.9/dxsp/main.py` & `dxsp-2.0.0/dxsp/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,113 +2,53 @@
  DEX SWAP Main
 """
 
 import logging
 
 import requests
 from dxsp import __version__
-from dxsp.assets.blockchains import blockchains
+# from dxsp.assets.blockchains import blockchains
 from dxsp.config import settings
-from ping3 import ping
+
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 
 
 class DexSwap:
     """Do a swap."""
 
-    def __init__(self,
-                 chain_id: int = 1,
-                 wallet_address: str | None = None,
-                 private_key: str | None = None,
-                 block_explorer_api: str | None = None,
-                 block_explorer_url: str | None = None,
-                 rpc: str | None = None,
-                 w3: Web3 | None = None,
-                 protocol_type: str | None = None,
-                 router_contract_addr: str | None = None,
-                 ):
-        """build a web3 object for swap"""
-        self.logger = logging.getLogger(__name__)
+    def __init__(self, w3: Web3 | None = None,):
+        """build a dex object """
+        self.logger = logging.getLogger(name="DexSwap")
         self.logger.info("DexSwap version: %s", __version__)
-        self.logger.info("Initializing DexSwap for %s on %s",
-                         wallet_address, chain_id)
-
-        self.chain_id = int(chain_id)
-        self.logger.debug("self.chain_id %s", self.chain_id)
-        if self.chain_id is None:
-            self.logger.warning("self.chain_id not setup")
-            return
-        blockchain = blockchains[self.chain_id]
-        self.logger.debug("blockchain %s", blockchain)
-
-        self.wallet_address = wallet_address
-        self.logger.debug("self.wallet_address %s", self.wallet_address)
-        self.private_key = private_key
-
-        self.block_explorer_api = block_explorer_api
-        if self.block_explorer_api is None:
-            self.logger.warning("self.block_explorer_api not setup")
-        self.block_explorer_url = block_explorer_url
-        self.block_explorer_url = (
-            block_explorer_url
-            or blockchain.get("block_explorer_url")
-            or self.logger.warning("self.block_explorer_url not set up")
-        )
-        self.logger.debug("explorer_url %s", self.block_explorer_url)
-
-        self.rpc = rpc or blockchain.get("rpc")
-        self.logger.debug("self.rpc %s", self.rpc)
-        try:
-            self.latency = round(ping(self.rpc, unit='ms'), 3)
-            self.logger.debug("self.latency %s", self.latency)
-        except Exception as e:
-            self.logger.error("Failed to ping %s:%s", self.rpc, e)
 
-        self.w3 = w3 or Web3(Web3.HTTPProvider(self.rpc))
+        self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         try:
-            self.w3.net.listening
-            self.logger.info("connected to %s with w3 %s", self.rpc, self.w3)
+            if self.w3.net.listening:
+                self.logger.info("connected to %s", self.w3)
         except Exception as e:
             self.logger.error("connectivity failed %s", e)
             return
-        self.logger.debug("self.w3 %s", self.w3)
-        self.logger.info("connected")
-
-        self.protocol_type = protocol_type or "1inch"
-        if self.protocol_type == "0x":
-            base_url = blockchain["0x"]
-        elif self.protocol_type == "1inch_limit":
-            base_url = blockchain["1inch_limit"]
-        else:
-            base_url = blockchain["1inch"]
-
-        self.dex_url = f"{base_url}"
-        self.logger.debug("self.dex_url %s", self.dex_url)
-        self.logger.debug("self.protocol_type %s", self.protocol_type)
-
-        self.router_contract_addr = router_contract_addr
-        if self.router_contract_addr is None:
-            self.router_contract_addr = blockchain["uniswap_v2"]
 
-        self.name = "TBD"
-        self.logger.debug("self.name %s", self.name)
+        self.protocol_type = settings.dex_protocol_type
 
-        self.trading_quote_ccy = settings.trading_quote_ccy
-        self.logger.debug("self.trading_quote_ccy %s", self.trading_quote_ccy)
+        # USER SECRET
+        self.wallet_address = settings.dex_wallet_address
+        self.private_key = settings.dex_private_key
 
+        # COINGECKO
         try:
-            self.gecko_api = CoinGeckoAPI()
-            assetplatform = self.gecko_api.get_asset_platforms()
+            self.cg = CoinGeckoAPI()
+            assetplatform = self.cg.get_asset_platforms()
             output_dict = [x for x in assetplatform if x['chain_identifier']
-                           == int(self.chain_id)]
-            self.gecko_platform = output_dict[0]['id']
-            self.logger.debug("self.gecko_platform %s", self.gecko_platform)
+                           == int(settings.dex_chain_id)]
+            self.cg_platform = output_dict[0]['id']
+            self.logger.debug("cg_platform %s", self.cg_platform)
         except Exception as e:
-            self.logger.error("CoinGeckoAPI setup: %s", e)
+            self.logger.error("CoinGecko: %s", e)
             return
 
     async def _get(
                 self,
                 url,
                 params=None,
                 headers=None
@@ -119,68 +59,112 @@
                             url,
                             params=params,
                             headers=headers,
                             timeout=10
                         )
         return response.json()
 
+    async def router(self):
+        try:
+            router_abi = await self.get_abi(settings.dex_router_contract_addr)
+            router = self.w3.eth.contract(
+                self.w3.to_checksum_address(
+                    settings.dex_router_contract_addr),
+                router_abi)
+            return router
+        except Exception as e:
+            self.logger.error("router setup: %s", e)
+            return
+
     async def get_quote(
                 self,
                 symbol
             ):
         self.logger.debug("get_quote %s", symbol)
         asset_in_address = await self.search_contract(symbol)
-        self.logger.debug("asset_in_address %s", asset_in_address)
-        asset_out_symbol = self.trading_quote_ccy
+        asset_out_symbol = settings.trading_quote_ccy
         asset_out_address = await self.search_contract(asset_out_symbol)
-        self.logger.debug("asset_out_address %s", asset_out_address)
         if asset_out_address is None:
             self.logger.warning("No Valid Contract %s", symbol)
             return
-        # asset_out_contract = await self.get_token_contract(asset_out_symbol)
-        # asset_out_decimals = asset_out_contract.functions.decimals().call()
-        # self.logger.debug(f"asset_out_decimals {asset_out_decimals}")
-        try:
-            if self.protocol_type == "1inch":
-                asset_out_amount = self.w3.to_wei(1, 'ether')
-                self.logger.debug("asset_out_amount %s", asset_out_amount)
-                quote_url = (self.dex_url
-                             + "/quote?fromTokenAddress="
-                             + asset_in_address
-                             + "&toTokenAddress="
-                             + asset_out_address
-                             + "&amount="
-                             + asset_out_amount)
-                quote = await self._get(quote_url)
-                self.logger.debug("quote %s", quote)
-                raw_quote = quote['toTokenAmount']
-                self.logger.debug("raw_quote %s", raw_quote)
-                asset_quote_decimals = quote['fromToken']['decimals']
-                self.logger.debug("asset_quote_decimals %s",
-                                  asset_quote_decimals)
-                quote_readable = (self.w3.from_wei(int(raw_quote), 'wei') /
-                                  (10 ** asset_quote_decimals))
-                self.logger.debug("quote_readable %s", quote_readable)
-                return round(quote_readable, 2)
-            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-                return
+        try:
+            if self.protocol_type in ["1inch", "1inch_limit"]:
+                self.oneinch_quote(
+                    asset_in_address,
+                    asset_out_address)
+            if self.protocol_type == "uniswap_v2":
+                self.uniswap_v2_quote(
+                    asset_in_address,
+                    asset_out_address)
+            if self.protocol_type == "uniswap_v3":
+                self.uniswap_v3_quote(
+                    asset_in_address,
+                    asset_out_address)
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
 
+    async def oneinch_quote(
+        self,
+        asset_in_address,
+        asset_out_address,
+        amount=1
+    ):
+        asset_out_amount = self.w3.to_wei(amount, 'ether')
+        quote_url = (
+            settings.dex_base_api
+            + "/quote?fromTokenAddress="
+            + str(asset_in_address)
+            + "&toTokenAddress="
+            + str(asset_out_address)
+            + "&amount="
+            + str(asset_out_amount))
+        quote_response = await self._get(quote_url)
+        self.logger.debug("quote %s", quote_response)
+        quote_amount = quote_response['toTokenAmount']
+        quote_decimals = quote_response['fromToken']['decimals']
+        quote = (
+            self.w3.from_wei(int(quote_amount), 'wei') /
+            (10 ** quote_decimals))
+        self.logger.debug("quote %s", quote)
+        return round(quote, 2)
+
+    async def uniswap_v2_quote(
+        self,
+        asset_in_address,
+        asset_out_address,
+        amount=1
+    ):
+        order_path_dex = [asset_out_address, asset_in_address]
+        order_min_amount = int(
+            self.router().functions.getAmountsOut(
+                amount,
+                order_path_dex)
+            .call()[1])
+        return order_min_amount
+
+    async def uniswap_v3_quote(
+        self,
+        asset_in_address,
+        asset_out_address,
+        amount=1
+    ):
+        return
+
     async def execute_order(self, order_params):
         """execute swap function"""
         action = order_params.get('action')
         instrument = order_params.get('instrument')
         quantity = order_params.get('quantity', 1)
+
         try:
-            asset_out_symbol = (self.trading_quote_ccy if
+            asset_out_symbol = (settings.trading_quote_ccy if
                                 action == "BUY" else instrument)
             asset_in_symbol = (instrument if action == "BUY"
-                               else self.trading_quote_ccy)
+                               else settings.trading_quote_ccy)
             asset_out_contract = await self.get_token_contract(
                 asset_out_symbol)
             try:
                 asset_out_decimals = (
                     asset_out_contract.functions.decimals().call())
             except Exception as e:
                 self.logger.error("execute_order decimals: %s", e)
@@ -205,99 +189,70 @@
             return "error processing order in DXSP"
 
     async def get_swap(
                 self,
                 asset_out_symbol: str,
                 asset_in_symbol: str,
                 amount: int,
-                slippage_tolerance_percentage=2
                 ):
         """main swap function"""
 
         self.logger.debug("get_swap")
         try:
             # ASSET OUT
             asset_out_address = await self.search_contract(
                 asset_out_symbol)
             asset_out_contract = await self.get_token_contract(
                 asset_out_symbol)
             if asset_out_contract is None:
                 raise ValueError("No contract identified")
-            asset_out_decimals = asset_out_contract.functions.decimals().call()
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
-            self.logger.debug("asset_out_balance %s", asset_out_balance)
             if asset_out_balance == 0:
                 self.logger.warning("No Money")
-                raise ValueError("Non contract identified")
+                raise ValueError("No Money")
                 return
             # ASSETS IN
             asset_in_address = await self.search_contract(asset_in_symbol)
             self.logger.debug("asset_in_address %s", asset_in_address)
             if asset_in_address is None:
                 return
 
             # AMOUNT
             asset_out_decimals = asset_out_contract.functions.decimals().call()
             self.logger.debug("asset_out_decimals %s", asset_out_decimals)
             asset_out_amount = amount * 10 ** asset_out_decimals
-            # defaulted to 2% slippage if not given
-            slippage = slippage_tolerance_percentage
-            self.logger.debug("slippage %s", slippage)
             asset_out_amount_converted = self.w3.to_wei(
                 asset_out_amount, 'ether')
 
-            order_amount = int((asset_out_amount_converted * (slippage/100)))
+            order_amount = int(
+                (asset_out_amount_converted *
+                 (settings.slippage/100)))
             self.logger.debug("order_amount %s", order_amount)
 
             # VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
             await self.get_approve(asset_out_address)
 
             # 1INCH
             if self.protocol_type in ["1inch"]:
-                swap_url = (self.dex_url
-                            + "/swap?fromTokenAddress="
-                            + asset_out_address
-                            + "&toTokenAddress="
-                            + asset_in_address
-                            + "&amount="
-                            + order_amount
-                            + "&fromAddress="
-                            + self.wallet_address
-                            + "&slippage="
-                            + slippage
-                            )
-                swap_order = await self._get(swap_url)
-                swap_order_status = swap_order['statusCode']
-                if swap_order_status != 200:
-                    return
+                swap_order = self.oneinch_swap(
+                    asset_out_address,
+                    asset_in_address,
+                    order_amount)
             # UNISWAP V2
             if self.protocol_type in ["uniswap_v2"]:
-                order_path_dex = [asset_out_address, asset_in_address]
-                router_abi = await self.get_abi(self.router_contract_addr)
-                router = self.w3.eth.contract(
-                                  self.w3.to_checksum_address(
-                                    self.router_contract_addr),
-                                  router_abi)
-                deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
-                order_min_amount = int(router.functions.getAmountsOut(
-                                        order_amount,
-                                        order_path_dex).call()[1])
-                swap_order = router.functions.swapExactTokensForTokens(
-                                order_amount,
-                                order_min_amount,
-                                order_path_dex,
-                                self.wallet_address,
-                                deadline)
+                swap_order = self.uniswap_v2_swap(
+                    asset_out_address,
+                    asset_in_address,
+                    order_amount)
             # 1INCH LIMIT
             if self.protocol_type in ["1inch_limit"]:
                 return
-
             # UNISWAP V3
             if self.protocol_type in ['uniswap_v3']:
-                return
+                swap_order = self.uniswap_v3_swap()
             if swap_order:
                 self.logger.debug("swap_order %s", swap_order)
                 signed_order = await self.get_sign(swap_order)
                 order_hash = str(self.w3.to_hex(signed_order))
                 order_hash_details = self.w3.wait_for_transaction_receipt(
                                         order_hash,
                                         timeout=120,
@@ -309,14 +264,62 @@
                         asset_out_symbol,
                         asset_out_address,
                         order_amount,)
         except Exception as e:
             self.logger.error("get_swap %s", e)
             return
 
+    async def oneinch_swap(
+        self,
+        asset_out_address,
+        asset_in_address,
+        amount
+    ):
+        swap_url = (settings.dex_base_api
+                    + "/swap?fromTokenAddress="
+                    + asset_out_address
+                    + "&toTokenAddress="
+                    + asset_in_address
+                    + "&amount="
+                    + amount
+                    + "&fromAddress="
+                    + self.wallet_address
+                    + "&slippage="
+                    + settings.slippage
+                    )
+        swap_order = await self._get(swap_url)
+        swap_order_status = swap_order['statusCode']
+        if swap_order_status != 200:
+            return
+        return swap_order
+
+    async def uniswap_v2_swap(
+        self,
+        asset_out_address,
+        asset_in_address,
+        amount
+    ):
+        order_path_dex = [asset_out_address, asset_in_address]
+
+        deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
+        order_min_amount = self.uniswap_v2_quote(
+            asset_in_address,
+            asset_out_address)
+        swap_order = self.router().functions.swapExactTokensForTokens(
+                        amount,
+                        order_min_amount,
+                        order_path_dex,
+                        self.wallet_address,
+                        deadline)
+        return swap_order
+
+    async def uniswap_v3_swap(self):
+        self.logger.debug("Not available")
+        return
+
     async def get_confirmation(self,
                                order_hash,
                                order_hash_details,
                                asset_out_symbol,
                                asset_out_address,
                                order_amount,
                                ):
@@ -341,86 +344,86 @@
             self.logger.info("trade %s", trade)
             return trade
         except Exception as e:
             self.logger.error("get_confirmation %s", e)
             return
 
     async def get_block_explorer_status(self, txHash):
-        self.logger.debug("get_block_explorer_status %s", txHash)
-        checkTransactionSuccessURL = (
-            self.block_explorer_url
-            + "?module=transaction&action=gettxreceiptstatus&txhash="
-            + txHash
-            + "&apikey="
-            + self.block_explorer_api)
-        checkTransactionRequest = self._get(checkTransactionSuccessURL)
-        return checkTransactionRequest['status']
+        if settings.block_explorer_api:
+            self.logger.debug("get_block_explorer_status %s", txHash)
+            checkTransactionSuccessURL = (
+                settings.block_explorer_url
+                + "?module=transaction&action=gettxreceiptstatus&txhash="
+                + str(txHash)
+                + "&apikey="
+                + str(settings.block_explorer_api))
+            checkTransactionRequest = self._get(checkTransactionSuccessURL)
+            return checkTransactionRequest['status']
 
 # ###CONTRACT SEARCH
     async def search_contract(
                             self,
                             token
                             ):
         """search a contract function"""
         self.logger.debug("search_contract")
 
         try:
             token_contract = await self.get_contract_address(
-                settings.TOKEN_PERSONAL_LIST,
+                settings.token_personal_list,
                 token)
             if token_contract is None:
                 token_contract = await self.get_contract_address(
-                    settings.TOKEN_TESTNET_LIST,
+                    settings.token_testnet_list,
                     token)
                 if token_contract is None:
                     token_contract = await self.get_contract_address(
-                        settings.TOKEN_MAINNET_LIST,
+                        settings.token_mainnet_list,
                         token)
                     if token_contract is None:
-                        token_contract = await self.search_gecko_contract(
+                        token_contract = await self.search_cg_contract(
                             token)
             if token_contract is not None:
                 self.logger.info("token_contract found %s", token_contract)
                 return self.w3.to_checksum_address(token_contract)
             self.logger.info("no contract found for %s", token)
         except Exception as e:
             self.logger.error("search_contract %s", e)
             return
 
     async def search_gecko(self, token):
         """search coingecko"""
         self.logger.debug("search_gecko")
         try:
-            search_results = self.gecko_api.search(query=token)
+            search_results = self.cg.search(query=token)
             search_dict = search_results['coins']
             filtered_dict = [x for x in search_dict if
                              x['symbol'] == token.upper()]
             api_dict = [sub['api_symbol'] for sub in filtered_dict]
             self.logger.debug("api_dict %s", api_dict)
             for i in api_dict:
-                coin_dict = self.gecko_api.get_coin_by_id(i)
+                coin_dict = self.cg.get_coin_by_id(i)
                 try:
-                    if coin_dict['platforms'][f'{self.gecko_platform}']:
+                    if coin_dict['platforms'][f'{self.cg_platform}']:
                         return coin_dict
                 except KeyError:
                     pass
         except Exception as e:
             self.logger.error("search_gecko %s", e)
             return
 
-    async def search_gecko_contract(self, token):
+    async def search_cg_contract(self, token):
         """search coingecko contract"""
-        self.logger.debug("🦎search_gecko_contract %s", token)
-        self.logger.debug("🦎self.gecko_platform %s", self.gecko_platform)
+        self.logger.debug("🦎search_cg_contract %s", token)
         try:
             coin_info = await self.search_gecko(token)
             if coin_info is not None:
-                return coin_info['platforms'][f'{self.gecko_platform}']
+                return coin_info['platforms'][f'{self.cg_platform}']
         except Exception as e:
-            self.logger.error(f"error search_gecko_contract {e}")
+            self.logger.error(f"error search_cg_contract {e}")
             return
 
     async def get_contract_address(
                             self,
                             token_list_url,
                             symbol
                         ):
@@ -428,89 +431,93 @@
         get token address"""
         self.logger.debug("get_contract_address %s %s", token_list_url, symbol)
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and
-                   keyval['chainId'] == self.chain_id):
+                   keyval['chainId'] == settings.dex_chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug("get_contract_address %s", e)
             return
 
     async def get_token_contract(
                                 self,
                                 token
                             ):
         """Given a token symbol, returns a contract object. """
         self.logger.debug("get_token_contract %s", token)
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
-            return self.w3.eth.contract(address=token_address, abi=token_abi)
+            return self.w3.eth.contract(
+                address=token_address,
+                abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s", e)
             return
 
 # ###UTILS
     async def get_approve(
                         self,
                         asset_out_address: str,
                         amount=None
                     ):
+
         self.logger.debug("get_approve %s", asset_out_address)
         if self.protocol_type in ["1inch", "1inch_limit"]:
             approval_check_URL = (
-                self.dex_url
+                settings.dex_base_api
                 + "/approve/allowance?tokenAddress="
-                + asset_out_address
+                + str(asset_out_address)
                 + "&walletAddress="
-                + self.wallet_address)
+                + str(self.wallet_address))
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check == 0):
                 approval_URL = (
-                    self.dex_url
+                    settings.dex_base_api
                     + "/approve/transaction?tokenAddress="
-                    + asset_out_address)
+                    + str(asset_out_address))
                 approval_response = await self._get(approval_URL)
         elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
             asset_out_abi = await self.get_abi(asset_out_address)
             asset_out_contract = self.w3.eth.contract(
-                                 asset_out_address,
-                                 asset_out_abi)
+                                 address=asset_out_address,
+                                 abi=asset_out_abi)
             approval_check = asset_out_contract.functions.allowance(
                              self.w3.to_checksum_address(self.wallet_address),
                              self.w3.to_checksum_address(
-                                self.router_contract_addr)
+                                settings.dex_router_contract_addr)
                              ).call()
             if (approval_check == 0):
                 approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
                 asset_out_abi = await self.get_abi(asset_out_address)
                 asset_out_contract = self.w3.eth.contract(
-                                     asset_out_address,
-                                     asset_out_abi)
+                                     address=asset_out_address,
+                                     abi=asset_out_abi)
                 approval_TX = asset_out_contract.functions.approve(
                                 self.w3.to_checksum_address(
-                                    self.router_contract_addr),
+                                    settings.router_contract_addr),
                                 approved_amount)
                 approval_txHash = await self.get_sign(approval_TX)
                 approval_txHash_complete = (
                     self.w3.eth.wait_for_transaction_receipt(
                         approval_txHash,
                         timeout=120,
                         poll_latency=0.1))
                 return approval_txHash_complete
 
     async def get_sign(
                     self,
                     order
                 ):
         self.logger.debug("get_sign %s", order)
+
         try:
             if not isinstance(order, dict):
                 raise ValueError("Transaction must be a dictionary")
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 order_params = {
                             'from': self.wallet_address,
                             'gas': await self.get_gas(order),
@@ -524,15 +531,15 @@
                 order['gas'] = await self.get_gas(order)
                 order['nonce'] = self.w3.eth.get_transaction_count(
                     self.wallet_address)
                 order['value'] = int(order['value'])
                 order['gasPrice'] = await self.get_gasPrice(order)
             signed = self.w3.eth.account.sign_transaction(
                 order,
-                self.private_key)
+                settings.dex_private_key)
             raw_order = signed.rawTransaction
             return self.w3.eth.send_raw_transaction(raw_order)
         except (ValueError, TypeError, KeyError) as e:
             self.logger.error("get_sign: %s", e)
             raise
         except Exception as e:
             self.logger.error("get_sign: %s", e)
@@ -556,28 +563,28 @@
         self.logger.debug("get_gasPrice %s", tx)
         gasprice = self.w3.eth.generate_gas_price()
         return self.w3.to_wei(gasprice, 'gwei')
 
     async def get_abi(self, addr):
         # Log a debug message to the logger
         self.logger.debug("get_abi %s", addr)
-        if self.block_explorer_api:
+        if settings.dex_block_explorer_api:
             try:
                 # Create a dictionary of parameters
                 params = {
                     "module": "contract",
                     "action": "getabi",
                     "address": addr,
-                    "apikey": self.block_explorer_api
+                    "apikey": settings.dex_block_explorer_api
                     }
                 # Create a dictionary of headers
                 headers = {"User-Agent": "Mozilla/5.0"}
                 # Make a GET request to the block explorer URL
                 resp = await self._get(
-                                       url=self.block_explorer_url,
+                                       url=settings.dex_block_explorer_url,
                                        params=params,
                                        headers=headers
                                        )
                 # If the response status is 1, log the ABI
                 if resp['status'] == "1":
                     self.logger.debug("ABI found %s", resp)
                     abi = resp["result"]
@@ -586,86 +593,84 @@
                 self.logger.warning("No ABI identified")
             except Exception as e:
                 # Log an error
                 self.logger.error("error get_abi %s", e)
                 return
         else:
             # If no block_explorer_api is set, log a warning
-            self.logger.warning("No block_explorer_api. Option B needed TBD")
+            self.logger.warning("No block_explorer_api.")
             return
 
-# ####USERS RELATED
+# USER BALANCE AND POSITION RELATED
 
     async def get_token_balance(
                                 self,
                                 token
                             ):
         self.logger.debug("get_token_balance %s", token)
+
         try:
             token_address = await self.search_contract(token)
             if token_address is None:
                 raise ValueError(f"Token address not found for {token}")
             token_abi = await self.get_abi(token_address)
             if token_abi is None:
                 raise ValueError(f"ABI not found for {token_address}")
             token_contract = self.w3.eth.contract(
-                token_address,
-                token_abi)
+                address=token_address,
+                abi=token_abi)
             token_balance = 0
             try:
                 token_balance = token_contract.functions.balanceOf(
                     self.wallet_address).call()
             except ValueError as e:
                 self.logger.warning("Invalid address: %s", e)
             return 0 if token_balance <= 0 else token_balance
         except Exception as e:
             self.logger.error("get_token_balance %s: %s", token, e)
             return 0
 
-    async def get_quote_ccy_balance(
-                                self
-                            ):
+    async def get_account_balance(
+                            self
+                        ):
+
         try:
-            trading_quote_ccy_balance = await self.get_token_balance(
-                self.trading_quote_ccy
-                )
-            return trading_quote_ccy_balance
+            balance = self.w3.eth.get_balance(
+                self.w3.to_checksum_address(
+                    self.wallet_address))
+            balance = (self.w3.from_wei(balance, 'ether'))
+            try:
+                trading_quote_ccy_balance = (
+                    await self.get_trading_quote_ccy_balance())
+                if trading_quote_ccy_balance:
+                    balance += "💵" + trading_quote_ccy_balance
+            except Exception as e:
+                self.logger.error("trading_quote_ccy_balance error: %s", e)
+
+            return round(balance, 5)
 
         except Exception as e:
-            self.logger.error("get_basecoin_balance %s: %s", e)
-            return 0
+            self.logger.error("get_account_balance error: %s", e)
+            return "balance error"
 
-    async def get_stablecoin_balance(
+    async def get_trading_quote_ccy_balance(
                                 self
                             ):
-        stablecoins = settings.stablecoins
+
         try:
-            msg = ""
-            for i in stablecoins:
-                bal_stablecoins = await self.get_token_balance(i)
-                if bal_stablecoins:
-                    msg += f"\n💵{bal_stablecoins} {i}"
-            return msg
+            trading_quote_ccy_balance = await self.get_token_balance(
+                settings.trading_quote_ccy)
+            if trading_quote_ccy_balance:
+                return trading_quote_ccy_balance
+            return 0
         except Exception as e:
-            self.logger.error("get_stablecoin_balance error: %s", e)
+            self.logger.error("get_trading_quote_ccy_balance error: %s", e)
             return 0
 
-    async def get_account_balance(
-                            self
-                        ):
-        try:
-            balance = self.w3.eth.get_balance(self.w3.to_checksum_address(self.wallet_address)
-            balance = (self.w3.from_wei(balance, 'ether'))
-            return round(balance, 5)
-        except Exception as e:
-            self.logger.error("get_account_balance error: %s", e)
-            return "balance error"
+    async def get_account_position(self):
 
-    async def get_account_position(
-                                    self
-                                    ):
         try:
             self.logger.debug("get_account_position")
             return
         except Exception as e:
             self.logger.error("get_account_position error: %s", e)
             return 0
```

### Comparing `dxsp-1.9.9/pyproject.toml` & `dxsp-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.9.9"
+version = "2.0.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 asyncio = "*"
 dynaconf = "*"
 web3 = ">=6.0.0"
 pycoingecko = "*"
-ping3 = "*"
+
 #web3-ethereum-defi = "*"
 # web3client = ">=1.1.8"
 # # many-abis = ">=0.1.7"
 # apollox-connector-python = "*"
 
 
 [tool.poetry.dev-dependencies]
@@ -52,16 +52,12 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
 
-#patch_emoji
-# 🐛🚑🤖🏁🔒👽🔍💬🥅⚡♿🍏🐧
+#patch_emoji # 🐛🚑⚡🔒👽🔍💬🥅♿🍏🐧🏁🤖
 #:ambulance:, :lock:, :bug:, :zap:, :goal_net:, :alien:, :wheelchair:, :speech_balloon:, :mag:, :apple:, :penguin:, :checkered_flag:, :robot:, :green_apple
-#minor_emoji
-#✨🥚🚸📱💄📈
-#:sparkles: ✨, :children_crossing:, :lipstick:, :iphone:, :egg:, :chart_with_upwards_trend
-#major_emoji¶
-#💥
-# :boom:
+#minor_emoji #✨🥚🚸📱💄📈
+#:sparkles:, :children_crossing:, :lipstick:, :iphone:, :egg:, :chart_with_upwards_trend
+#major_emoji¶ #💥:boom:
```

### Comparing `dxsp-1.9.9/PKG-INFO` & `dxsp-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.9.9
+Version: 2.0.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
-Requires-Dist: ping3
 Requires-Dist: pycoingecko
 Requires-Dist: web3 (>=6.0.0)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
```

