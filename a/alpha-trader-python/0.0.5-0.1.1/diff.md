# Comparing `tmp/alpha_trader_python-0.0.5.tar.gz` & `tmp/alpha_trader_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha_trader_python-0.0.5.tar", max compression
+gzip compressed data, was "alpha_trader_python-0.1.1.tar", max compression
```

## Comparing `alpha_trader_python-0.0.5.tar` & `alpha_trader_python-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      255 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/README.md
--rw-r--r--   0        0        0       22 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/achievement/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/authentication/__init__.py
--rw-r--r--   0        0        0      529 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/bank_account/__init__.py
--rw-r--r--   0        0        0     5117 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/bonds/__init__.py
--rw-r--r--   0        0        0     8445 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/client/__init__.py
--rw-r--r--   0        0        0     3002 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/company/__init__.py
--rw-r--r--   0        0        0      776 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/filter/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/listing/__init__.py
--rw-r--r--   0        0        0      387 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/logging/__init__.py
--rw-r--r--   0        0        0     4276 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/miner/__init__.py
--rw-r--r--   0        0        0     6087 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/order/__init__.py
--rw-r--r--   0        0        0      470 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/owner/__init__.py
--rw-r--r--   0        0        0       71 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/partner/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/portfolio/position.py
--rw-r--r--   0        0        0        0 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/price/__init__.py
--rw-r--r--   0        0        0      405 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/price/price.py
--rw-r--r--   0        0        0     2790 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/price/price_spread.py
--rw-r--r--   0        0        0     2771 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/securities_account/__init__.py
--rw-r--r--   0        0        0     7727 2023-05-05 07:31:55.541037 alpha_trader_python-0.0.5/alpha_trader/user/__init__.py
--rw-r--r--   0        0        0      922 2023-05-05 07:31:55.545038 alpha_trader_python-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-07 10:49:45.503481 alpha_trader_python-0.1.1/alpha_trader/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/achievement/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/authentication/__init__.py
+-rw-r--r--   0        0        0      961 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/bank_account/__init__.py
+-rw-r--r--   0        0        0     5117 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/bonds/__init__.py
+-rw-r--r--   0        0        0     8445 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/client/__init__.py
+-rw-r--r--   0        0        0     3017 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/company/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/filter/__init__.py
+-rw-r--r--   0        0        0     1155 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/listing/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/logging/__init__.py
+-rw-r--r--   0        0        0     4276 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/miner/__init__.py
+-rw-r--r--   0        0        0     6091 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/order/__init__.py
+-rw-r--r--   0        0        0      470 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/owner/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-07 10:49:44.443478 alpha_trader_python-0.1.1/alpha_trader/partner/__init__.py
+-rw-r--r--   0        0        0     1629 2023-05-07 10:49:44.447478 alpha_trader_python-0.1.1/alpha_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-07 10:49:44.447478 alpha_trader_python-0.1.1/alpha_trader/portfolio/position.py
+-rw-r--r--   0        0        0        0 2023-05-07 10:49:44.447478 alpha_trader_python-0.1.1/alpha_trader/price/__init__.py
+-rw-r--r--   0        0        0      405 2023-05-07 10:49:44.447478 alpha_trader_python-0.1.1/alpha_trader/price/price.py
+-rw-r--r--   0        0        0     2790 2023-05-07 10:49:44.447478 alpha_trader_python-0.1.1/alpha_trader/price/price_spread.py
+-rw-r--r--   0        0        0     2771 2023-05-07 10:49:44.447478 alpha_trader_python-0.1.1/alpha_trader/securities_account/__init__.py
+-rw-r--r--   0        0        0     8216 2023-05-07 10:49:44.447478 alpha_trader_python-0.1.1/alpha_trader/user/__init__.py
+-rw-r--r--   0        0        0      929 2023-05-07 10:49:45.499481 alpha_trader_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.1.1/PKG-INFO
```

### Comparing `alpha_trader_python-0.0.5/alpha_trader/achievement/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/achievement/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/bonds/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/bonds/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/client/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/client/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/company/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/company/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     @staticmethod
     def initialize_from_api_response(api_response: Dict, client: Client):
         from alpha_trader.user import User
 
         return Company(
             achievement_count=api_response["achievementCount"],
             bank_account=BankAccount.initialize_from_api_response(
-                api_response["bankAccount"]
+                api_response["bankAccount"], client=client
             ),
             ceo=User.initialize_from_api_response(api_response["ceo"], client),
             id=api_response["id"],
             listing=Listing.initialize_from_api_response(
                 api_response["listing"], client
             ),
             logo_url=api_response["logoUrl"],
```

### Comparing `alpha_trader_python-0.0.5/alpha_trader/filter/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/listing/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/listing/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/miner/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/order/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/order/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,19 @@
             concerningParams=api_response["concerningParams"],
         )
 
 
 class Order(BaseModel):
     action: str
     check_result: Union[OrderCheckResult, None]
-    committed_cash: int
+    committed_cash: float
     counter_party: Union[str, None]
     counter_party_name: Union[str, None]
     creation_date: int
-    execution_price: Union[int, None]
+    execution_price: Union[float, None]
     execution_volume: Union[int, None]
     good_after_date: Union[int, None]
     good_till_date: Union[int, None]
     hourly_change: Union[int, None]
     id: str
     listing: Listing
     next_hourly_change_date: Union[int, None]
```

### Comparing `alpha_trader_python-0.0.5/alpha_trader/portfolio/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/portfolio/position.py` & `alpha_trader_python-0.1.1/alpha_trader/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/price/price_spread.py` & `alpha_trader_python-0.1.1/alpha_trader/price/price_spread.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/securities_account/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/securities_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.5/alpha_trader/user/__init__.py` & `alpha_trader_python-0.1.1/alpha_trader/user/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pydantic import BaseModel
 from typing import Dict, Union, List
 
 from alpha_trader.client import Client
 from alpha_trader.achievement import Achievement
 from alpha_trader.logging import logger
 from alpha_trader.securities_account import SecuritiesAccount
+from alpha_trader.bank_account import BankAccount
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from alpha_trader.company import Company
 
 
@@ -211,14 +212,28 @@
         Returns:
             Daily salary
         """
         response = self.client.request("GET", f"api/v2/possibledailysalary/{self.id}")
 
         return response.json()["value"]
 
+    @property
+    def bank_account(self) -> BankAccount:
+        """
+            Get the bank account for the user
+        Returns:
+            Bank account
+        """
+        if not self.my_user:
+            raise Exception("Cannot retrieve bank account for other users")
+
+        response = self.client.request("GET", "api/v2/my/bankaccounts/")
+
+        return BankAccount.initialize_from_api_response(response.json()[0], self.client)
+
     def retrieve_salary(self) -> None:
         """
             Retrieve all the salaries for the user
         Returns:
             None
 
         """
```

### Comparing `alpha_trader_python-0.0.5/pyproject.toml` & `alpha_trader_python-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpha-trader-python"
-version = "0.0.5"
+version = "0.1.1"
 description = "Python SDK for https://alpha-trader.com"
 authors = ["maltemelzer"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alpha_trader"}]
 
 [tool.poetry.dependencies]
@@ -27,12 +27,12 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = [
     "pyproject.toml:version",
     "alpha_trader/__init__.py:__version__"
 ]
-version_source = "tag"
-upload_to_release = false
-upload_to_pypi = false
+version_source = "commit"
+upload_to_release = true
+upload_to_repository = true
 branch = "main"
 build_command = "pip install poetry && poetry build"
```

### Comparing `alpha_trader_python-0.0.5/PKG-INFO` & `alpha_trader_python-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpha-trader-python
-Version: 0.0.5
+Version: 0.1.1
 Summary: Python SDK for https://alpha-trader.com
 License: MIT
 Author: maltemelzer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

