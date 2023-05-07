# Comparing `tmp/dxsp-1.9.8.tar.gz` & `tmp/dxsp-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.9.8.tar", max compression
+gzip compressed data, was "dxsp-1.9.9.tar", max compression
```

## Comparing `dxsp-1.9.8.tar` & `dxsp-1.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-06 11:58:14.037258 dxsp-1.9.8/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-06 11:58:14.037258 dxsp-1.9.8/README.md
--rw-r--r--   0        0        0       38 2023-05-06 11:58:14.037258 dxsp-1.9.8/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-06 11:58:14.793290 dxsp-1.9.8/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-06 11:58:14.037258 dxsp-1.9.8/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-06 11:58:14.037258 dxsp-1.9.8/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-06 11:58:14.037258 dxsp-1.9.8/dxsp/config.py
--rw-r--r--   0        0        0      581 2023-05-06 11:58:14.037258 dxsp-1.9.8/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28246 2023-05-06 11:58:14.037258 dxsp-1.9.8/dxsp/main.py
--rw-r--r--   0        0        0     1787 2023-05-06 11:58:14.793290 dxsp-1.9.8/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-06 15:58:19.476954 dxsp-1.9.9/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-06 15:58:19.476954 dxsp-1.9.9/README.md
+-rw-r--r--   0        0        0       38 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-06 15:58:20.268993 dxsp-1.9.9/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/config.py
+-rw-r--r--   0        0        0      581 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28290 2023-05-06 15:58:19.476954 dxsp-1.9.9/dxsp/main.py
+-rw-r--r--   0        0        0     1787 2023-05-06 15:58:20.268993 dxsp-1.9.9/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.9/PKG-INFO
```

### Comparing `dxsp-1.9.8/LICENSE` & `dxsp-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.8/README.md` & `dxsp-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.8/dxsp/assets/blockchains.py` & `dxsp-1.9.9/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.8/dxsp/default_settings.toml` & `dxsp-1.9.9/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.8/dxsp/main.py` & `dxsp-1.9.9/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,19 +649,20 @@
             self.logger.error("get_stablecoin_balance error: %s", e)
             return 0
 
     async def get_account_balance(
                             self
                         ):
         try:
-            return self.w3.eth.get_balance(self.w3.to_checksum_address(self.wallet_address))
+            balance = self.w3.eth.get_balance(self.w3.to_checksum_address(self.wallet_address)
+            balance = (self.w3.from_wei(balance, 'ether'))
+            return round(balance, 5)
         except Exception as e:
             self.logger.error("get_account_balance error: %s", e)
             return "balance error"
-            # bal = round(ex.from_wei(bal,'ether'),5)
 
     async def get_account_position(
                                     self
                                     ):
         try:
             self.logger.debug("get_account_position")
             return
```

### Comparing `dxsp-1.9.8/pyproject.toml` & `dxsp-1.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.9.8"
+version = "1.9.9"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.9.8/PKG-INFO` & `dxsp-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.9.8
+Version: 1.9.9
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

