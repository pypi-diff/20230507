# Comparing `tmp/dxsp-2.0.2.tar.gz` & `tmp/dxsp-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.2.tar", max compression
+gzip compressed data, was "dxsp-2.0.3.tar", max compression
```

## Comparing `dxsp-2.0.2.tar` & `dxsp-2.0.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-07 19:12:16.476887 dxsp-2.0.2/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-07 19:12:16.476887 dxsp-2.0.2/README.md
--rw-r--r--   0        0        0       38 2023-05-07 19:12:16.476887 dxsp-2.0.2/dxsp/.gitignore
--rw-r--r--   0        0        0       86 2023-05-07 19:12:17.144891 dxsp-2.0.2/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-07 19:12:16.476887 dxsp-2.0.2/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-07 19:12:16.476887 dxsp-2.0.2/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-07 19:12:16.476887 dxsp-2.0.2/dxsp/config.py
--rw-r--r--   0        0        0     2967 2023-05-07 19:12:16.476887 dxsp-2.0.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26188 2023-05-07 19:12:16.476887 dxsp-2.0.2/dxsp/main.py
--rw-r--r--   0        0        0     1769 2023-05-07 19:12:17.144891 dxsp-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-07 19:57:35.733774 dxsp-2.0.3/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-07 19:57:35.733774 dxsp-2.0.3/README.md
+-rw-r--r--   0        0        0       86 2023-05-07 19:57:36.397783 dxsp-2.0.3/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/config.py
+-rw-r--r--   0        0        0     2967 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26224 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/main.py
+-rw-r--r--   0        0        0     1769 2023-05-07 19:57:36.397783 dxsp-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.3/PKG-INFO
```

### Comparing `dxsp-2.0.2/LICENSE` & `dxsp-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.2/README.md` & `dxsp-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.2/dxsp/assets/blockchains.py` & `dxsp-2.0.3/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.2/dxsp/default_settings.toml` & `dxsp-2.0.3/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.2/dxsp/main.py` & `dxsp-2.0.3/dxsp/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,23 +83,23 @@
         asset_out_symbol = settings.trading_quote_ccy
         asset_out_address = await self.search_contract(asset_out_symbol)
         if asset_out_address is None:
             self.logger.warning("No Valid Contract %s", symbol)
             return
         try:
             if self.protocol_type in ["1inch", "1inch_limit"]:
-                self.oneinch_quote(
+                await self.oneinch_quote(
                     asset_in_address,
                     asset_out_address)
             if self.protocol_type == "uniswap_v2":
-                self.uniswap_v2_quote(
+                await self.uniswap_v2_quote(
                     asset_in_address,
                     asset_out_address)
             if self.protocol_type == "uniswap_v3":
-                self.uniswap_v3_quote(
+                await self.uniswap_v3_quote(
                     asset_in_address,
                     asset_out_address)
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
 
     async def oneinch_quote(
@@ -228,30 +228,30 @@
             self.logger.debug("order_amount %s", order_amount)
 
             # VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
             await self.get_approve(asset_out_address)
 
             # 1INCH
             if self.protocol_type in ["1inch"]:
-                swap_order = self.oneinch_swap(
+                swap_order = await self.oneinch_swap(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
             # UNISWAP V2
             if self.protocol_type in ["uniswap_v2"]:
-                swap_order = self.uniswap_v2_swap(
+                swap_order = await self.uniswap_v2_swap(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
             # 1INCH LIMIT
             if self.protocol_type in ["1inch_limit"]:
                 return
             # UNISWAP V3
             if self.protocol_type in ['uniswap_v3']:
-                swap_order = self.uniswap_v3_swap()
+                swap_order = await self.uniswap_v3_swap()
             if swap_order:
                 self.logger.debug("swap_order %s", swap_order)
                 signed_order = await self.get_sign(swap_order)
                 order_hash = str(self.w3.to_hex(signed_order))
                 order_hash_details = self.w3.wait_for_transaction_receipt(
                                         order_hash,
                                         timeout=120,
```

### Comparing `dxsp-2.0.2/pyproject.toml` & `dxsp-2.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.2"
+version = "2.0.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.0.2/PKG-INFO` & `dxsp-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.2
+Version: 2.0.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

