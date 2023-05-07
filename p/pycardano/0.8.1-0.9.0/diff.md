# Comparing `tmp/pycardano-0.8.1.tar.gz` & `tmp/pycardano-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycardano-0.8.1.tar", max compression
+gzip compressed data, was "pycardano-0.9.0.tar", max compression
```

## Comparing `pycardano-0.8.1.tar` & `pycardano-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1062 2023-04-06 17:01:21.098474 pycardano-0.8.1/LICENSE
--rw-r--r--   0        0        0     8826 2023-04-06 17:01:21.098474 pycardano-0.8.1/README.md
--rw-r--r--   0        0        0      445 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/__init__.py
--rw-r--r--   0        0        0    13503 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/address.py
--rw-r--r--   0        0        0       84 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/backend/__init__.py
--rw-r--r--   0        0        0     3757 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/backend/base.py
--rw-r--r--   0        0        0    10050 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/backend/blockfrost.py
--rw-r--r--   0        0        0    18163 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/backend/ogmios.py
--rw-r--r--   0        0        0     1268 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/certificate.py
--rw-r--r--   0        0        0       36 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/cip/__init__.py
--rw-r--r--   0        0        0     6679 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/cip/cip8.py
--rw-r--r--   0        0        0    13478 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/coinselection.py
--rw-r--r--   0        0        0       37 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/crypto/__init__.py
--rw-r--r--   0        0        0     4622 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/crypto/bech32.py
--rw-r--r--   0        0        0    18871 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/crypto/bip32.py
--rw-r--r--   0        0        0     1008 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/exception.py
--rw-r--r--   0        0        0     3133 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/hash.py
--rw-r--r--   0        0        0     9615 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/key.py
--rw-r--r--   0        0        0      432 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/logging.py
--rw-r--r--   0        0        0     4820 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/metadata.py
--rw-r--r--   0        0        0     6259 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/nativescript.py
--rw-r--r--   0        0        0      520 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/network.py
--rw-r--r--   0        0        0    32620 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/plutus.py
--rw-r--r--   0        0        0    27826 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/serialization.py
--rw-r--r--   0        0        0    17682 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/transaction.py
--rw-r--r--   0        0        0    50748 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/txbuilder.py
--rw-r--r--   0        0        0      125 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/types.py
--rw-r--r--   0        0        0     7111 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/utils.py
--rw-r--r--   0        0        0     2189 2023-04-06 17:01:21.126474 pycardano-0.8.1/pycardano/witness.py
--rw-r--r--   0        0        0     1789 2023-04-06 17:01:21.126474 pycardano-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    10373 1970-01-01 00:00:00.000000 pycardano-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-07 20:18:53.588145 pycardano-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9062 2023-05-07 20:18:53.588145 pycardano-0.9.0/README.md
+-rw-r--r--   0        0        0      445 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/__init__.py
+-rw-r--r--   0        0        0    13503 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/address.py
+-rw-r--r--   0        0        0       84 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/backend/__init__.py
+-rw-r--r--   0        0        0     5373 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/backend/base.py
+-rw-r--r--   0        0        0    10850 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/backend/blockfrost.py
+-rw-r--r--   0        0        0    18597 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/backend/ogmios.py
+-rw-r--r--   0        0        0     1268 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/certificate.py
+-rw-r--r--   0        0        0       36 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/cip/__init__.py
+-rw-r--r--   0        0        0     6679 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/cip/cip8.py
+-rw-r--r--   0        0        0    13478 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/coinselection.py
+-rw-r--r--   0        0        0       37 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/crypto/__init__.py
+-rw-r--r--   0        0        0     4622 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/crypto/bech32.py
+-rw-r--r--   0        0        0    18871 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/crypto/bip32.py
+-rw-r--r--   0        0        0     1008 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/exception.py
+-rw-r--r--   0        0        0     3133 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/hash.py
+-rw-r--r--   0        0        0     9619 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/key.py
+-rw-r--r--   0        0        0      432 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/logging.py
+-rw-r--r--   0        0        0     4813 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/metadata.py
+-rw-r--r--   0        0        0     6252 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/nativescript.py
+-rw-r--r--   0        0        0      520 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/network.py
+-rw-r--r--   0        0        0    32814 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/plutus.py
+-rw-r--r--   0        0        0    30189 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/serialization.py
+-rw-r--r--   0        0        0    17668 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/transaction.py
+-rw-r--r--   0        0        0    51428 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/txbuilder.py
+-rw-r--r--   0        0        0      650 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/types.py
+-rw-r--r--   0        0        0     7097 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/utils.py
+-rw-r--r--   0        0        0     2189 2023-05-07 20:18:53.616145 pycardano-0.9.0/pycardano/witness.py
+-rw-r--r--   0        0        0     1833 2023-05-07 20:18:53.616145 pycardano-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10695 1970-01-01 00:00:00.000000 pycardano-0.9.0/PKG-INFO
```

### Comparing `pycardano-0.8.1/LICENSE` & `pycardano-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/README.md` & `pycardano-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 builder = TransactionBuilder(context)
 
 # Tell the builder that transaction input will come from a specific address, assuming that there are some ADA and native
 # assets sitting at this address. "add_input_address" could be called multiple times with different address.
 builder.add_input_address(address)
 
 # Get all UTxOs currently sitting at this address
-utxos = context.utxos(str(address))
+utxos = context.utxos(address)
 
 # We can also tell the builder to include a specific UTxO in the transaction.
 # Similarly, "add_input" could be called multiple times.
 builder.add_input(utxos[0])
 
 # Send 1.5 ADA and a native asset (CHOC) in quantity of 2000 to an address.
 builder.add_output(
@@ -152,15 +152,15 @@
     )
 )
 
 # Create final signed transaction
 signed_tx = builder.build_and_sign([psk], change_address=address)
 
 # Submit signed transaction to the network
-context.submit_tx(signed_tx.to_cbor())
+context.submit_tx(signed_tx)
 
 ```
 </details>
 
 See more usages under [examples](https://github.com/Python-Cardano/pycardano/tree/main/examples).
 
 
@@ -254,8 +254,10 @@
 ## Sponsors :heart:
 
 <p align="left">
   <a href="https://github.com/KtorZ"><img src="https://avatars.githubusercontent.com/u/5680256?s=50&v=4"/></a>
   <a href="https://github.com/CardanoDur"><img width="50" src="https://avatars.githubusercontent.com/u/1000466?s=50&v=4"/></a>
   <a href="https://github.com/huths0lo"><img width="50" src="https://avatars.githubusercontent.com/u/78839856?s=50&v=4"/></a>
   <a href="https://github.com/markrufino"><img width="50" src="https://avatars.githubusercontent.com/u/30117352?v=4"/></a>
+  <a href="https://github.com/OpShin"><img width="50" src="https://avatars.githubusercontent.com/u/102762047?s=200&v=4"/></a>
+  <a href="https://github.com/aada-finance"><img width="50" src="https://avatars.githubusercontent.com/u/89693711?v=4"/></a>
 </p>
```

### Comparing `pycardano-0.8.1/pycardano/address.py` & `pycardano-0.9.0/pycardano/address.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/backend/blockfrost.py` & `pycardano-0.9.0/pycardano/backend/blockfrost.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
 import tempfile
 import time
 import warnings
 from typing import Dict, List, Optional, Union
 
+import cbor2
 from blockfrost import ApiError, ApiUrls, BlockFrostApi
 from blockfrost.utils import Namespace
 
 from pycardano.address import Address
 from pycardano.backend.base import (
     ALONZO_COINS_PER_UTXO_WORD,
     ChainContext,
     GenesisParameters,
     ProtocolParameters,
 )
 from pycardano.exception import TransactionFailedException
 from pycardano.hash import SCRIPT_HASH_SIZE, DatumHash, ScriptHash
 from pycardano.nativescript import NativeScript
 from pycardano.network import Network
-from pycardano.plutus import ExecutionUnits, PlutusV1Script, PlutusV2Script
+from pycardano.plutus import ExecutionUnits, PlutusV1Script, PlutusV2Script, script_hash
 from pycardano.serialization import RawCBOR
 from pycardano.transaction import (
     Asset,
     AssetName,
     MultiAsset,
     TransactionInput,
     TransactionOutput,
@@ -30,14 +31,27 @@
     Value,
 )
 from pycardano.types import JsonDict
 
 __all__ = ["BlockFrostChainContext"]
 
 
+def _try_fix_script(
+    scripth: str, script: Union[PlutusV1Script, PlutusV2Script]
+) -> Union[PlutusV1Script, PlutusV2Script]:
+    if str(script_hash(script)) == scripth:
+        return script
+    else:
+        new_script = script.__class__(cbor2.loads(script))
+        if str(script_hash(new_script)) == scripth:
+            return new_script
+        else:
+            raise ValueError("Cannot recover script from hash.")
+
+
 class BlockFrostChainContext(ChainContext):
     """A `BlockFrost <https://blockfrost.io/>`_ API wrapper for the client code to interact with.
 
     Args:
         project_id (str): A BlockFrost project ID obtained from https://blockfrost.io.
         network (Network): Network to use.
         base_url (str): Base URL for the BlockFrost API. Defaults to the preprod url.
@@ -147,25 +161,37 @@
         return self._protocol_param
 
     def _get_script(
         self, script_hash: str
     ) -> Union[PlutusV1Script, PlutusV2Script, NativeScript]:
         script_type = self.api.script(script_hash).type
         if script_type == "plutusV1":
-            return PlutusV1Script(bytes.fromhex(self.api.script_cbor(script_hash).cbor))
+            v1script = PlutusV1Script(
+                bytes.fromhex(self.api.script_cbor(script_hash).cbor)
+            )
+            return _try_fix_script(script_hash, v1script)
         elif script_type == "plutusV2":
-            return PlutusV2Script(bytes.fromhex(self.api.script_cbor(script_hash).cbor))
+            v2script = PlutusV2Script(
+                bytes.fromhex(self.api.script_cbor(script_hash).cbor)
+            )
+            return _try_fix_script(script_hash, v2script)
         else:
             script_json: JsonDict = self.api.script_json(
                 script_hash, return_type="json"
             )["json"]
             return NativeScript.from_dict(script_json)
 
-    def utxos(self, address: str) -> List[UTxO]:
-        results = self.api.address_utxos(address, gather_pages=True)
+    def _utxos(self, address: str) -> List[UTxO]:
+        try:
+            results = self.api.address_utxos(address, gather_pages=True)
+        except ApiError as e:
+            if e.status_code == 404:
+                return []
+            else:
+                raise e
 
         utxos = []
 
         for result in results:
             tx_in = TransactionInput.from_primitive(
                 [result.tx_hash, result.output_index]
             )
@@ -213,15 +239,15 @@
                 datum=datum,
                 script=script,
             )
             utxos.append(UTxO(tx_in, tx_out))
 
         return utxos
 
-    def submit_tx(self, cbor: Union[bytes, str]) -> str:
+    def submit_tx_cbor(self, cbor: Union[bytes, str]) -> str:
         """Submit a transaction.
 
         Args:
             cbor (Union[bytes, str]): The serialized transaction to be submitted.
 
         Returns:
             str: The transaction hash.
@@ -239,15 +265,15 @@
             os.remove(f.name)
             raise TransactionFailedException(
                 f"Failed to submit transaction. Error code: {e.status_code}. Error message: {e.message}"
             ) from e
         os.remove(f.name)
         return response
 
-    def evaluate_tx(self, cbor: Union[bytes, str]) -> Dict[str, ExecutionUnits]:
+    def evaluate_tx_cbor(self, cbor: Union[bytes, str]) -> Dict[str, ExecutionUnits]:
         """Evaluate execution units of a transaction.
 
         Args:
             cbor (Union[bytes, str]): The serialized transaction to be evaluated.
 
         Returns:
             Dict[str, ExecutionUnits]: A list of execution units calculated for each of the transaction's redeemers
```

### Comparing `pycardano-0.8.1/pycardano/backend/ogmios.py` & `pycardano-0.9.0/pycardano/backend/ogmios.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import time
 from datetime import datetime, timezone
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import cbor2
 import requests
 import websocket
@@ -41,31 +42,44 @@
 
 class OgmiosChainContext(ChainContext):
     _ws_url: str
     _network: Network
     _service_name: str
     _kupo_url: Optional[str]
     _last_known_block_slot: int
+    _last_chain_tip_fetch: float
     _genesis_param: Optional[GenesisParameters]
     _protocol_param: Optional[ProtocolParameters]
 
     def __init__(
         self,
         ws_url: str,
         network: Network,
         compact_result=True,
         kupo_url=None,
+        refetch_chain_tip_interval: Optional[float] = None,
     ):
         self._ws_url = ws_url
         self._network = network
         self._service_name = "ogmios.v1:compact" if compact_result else "ogmios"
         self._kupo_url = kupo_url
         self._last_known_block_slot = 0
+        self._refetch_chain_tip_interval = (
+            refetch_chain_tip_interval
+            if refetch_chain_tip_interval is not None
+            else 1000
+        )
+        self._last_chain_tip_fetch = 0
         self._genesis_param = None
         self._protocol_param = None
+        if refetch_chain_tip_interval is None:
+            self._refetch_chain_tip_interval = (
+                self.genesis_param.slot_length
+                / self.genesis_param.active_slots_coefficient
+            )
 
     def _request(self, method: OgmiosQueryType, args: JsonDict) -> Any:
         ws = websocket.WebSocket()
         ws.connect(self._ws_url)
         request = json.dumps(
             {
                 "type": "jsonwsp/request",
@@ -106,16 +120,20 @@
         return self._request(OgmiosQueryType.Query, args)
 
     def _query_utxos_by_tx_id(self, tx_id: str, index: int) -> List[List[JsonDict]]:
         args = {"query": {"utxo": [{"txId": tx_id, "index": index}]}}
         return self._request(OgmiosQueryType.Query, args)
 
     def _is_chain_tip_updated(self):
+        # fetch at most every twenty seconds!
+        if time.time() - self._last_chain_tip_fetch < self._refetch_chain_tip_interval:
+            return False
+        self._last_chain_tip_fetch = time.time()
         slot = self.last_block_slot
-        if self._last_known_block_slot != slot:
+        if self._last_known_block_slot < slot:
             self._last_known_block_slot = slot
             return True
         else:
             return False
 
     @staticmethod
     def _fraction_parser(fraction: str) -> float:
@@ -222,15 +240,15 @@
 
     @property
     def last_block_slot(self) -> int:
         """Slot number of last block"""
         result = self._query_chain_tip()
         return result["slot"]
 
-    def utxos(self, address: str) -> List[UTxO]:
+    def _utxos(self, address: str) -> List[UTxO]:
         """Get all UTxOs associated with an address.
 
         Args:
             address (str): An address encoded with bech32.
 
         Returns:
             List[UTxO]: A list of UTxOs.
@@ -254,28 +272,24 @@
             List[UTxO]: A list of UTxOs.
         """
         if self._kupo_url is None:
             raise AssertionError(
                 "kupo_url object attribute has not been assigned properly."
             )
 
-        kupo_utxo_url = self._kupo_url + "/matches/" + address
+        kupo_utxo_url = self._kupo_url + "/matches/" + address + "?unspent"
         results = requests.get(kupo_utxo_url).json()
 
         utxos = []
 
         for result in results:
             tx_id = result["transaction_id"]
             index = result["output_index"]
 
-            # Right now, all UTxOs of the address will be returned with Kupo, which requires Ogmios to
-            # validate if the UTxOs are spent with output reference. This feature is being considered to
-            # be added to Kupo to avoid extra API calls.
-            # See discussion here: https://github.com/CardanoSolutions/kupo/discussions/19.
-            if self._check_utxo_unspent(tx_id, index):
+            if result["spent_at"] is None:
                 tx_in = TransactionInput.from_primitive([tx_id, index])
 
                 lovelace_amount = result["value"]["coins"]
 
                 script = None
                 script_hash = result.get("script_hash", None)
                 if script_hash:
@@ -294,15 +308,15 @@
 
                 datum = None
                 datum_hash = (
                     DatumHash.from_primitive(result["datum_hash"])
                     if result["datum_hash"]
                     else None
                 )
-                if datum_hash:
+                if datum_hash and result.get("datum_type", "inline"):
                     kupo_datum_url = self._kupo_url + "/datums/" + result["datum_hash"]
                     datum_result = requests.get(kupo_datum_url).json()
                     if datum_result and datum_result["datum"] != datum_hash:
                         datum = RawCBOR(bytes.fromhex(datum_result["datum"]))
                         datum_hash = None
 
                 if not result["value"]["assets"]:
@@ -434,15 +448,15 @@
                 datum_hash=datum_hash,
                 datum=datum,
                 script=script,
             )
         utxo = UTxO(tx_in, tx_out)
         return utxo
 
-    def submit_tx(self, cbor: Union[bytes, str]):
+    def submit_tx_cbor(self, cbor: Union[bytes, str]):
         """Submit a transaction to the blockchain.
 
         Args:
             cbor (Union[bytes, str]): The transaction to be submitted.
 
         Raises:
             :class:`InvalidArgumentException`: When the transaction is invalid.
@@ -452,15 +466,15 @@
             cbor = cbor.hex()
 
         args = {"submit": cbor}
         result = self._request(OgmiosQueryType.SubmitTx, args)
         if "SubmitFail" in result:
             raise TransactionFailedException(result["SubmitFail"])
 
-    def evaluate_tx(self, cbor: Union[bytes, str]) -> Dict[str, ExecutionUnits]:
+    def evaluate_tx_cbor(self, cbor: Union[bytes, str]) -> Dict[str, ExecutionUnits]:
         """Evaluate execution units of a transaction.
 
         Args:
             cbor (Union[bytes, str]): The serialized transaction to be evaluated.
 
         Returns:
             Dict[str, ExecutionUnits]: A list of execution units calculated for each of the transaction's redeemers
```

### Comparing `pycardano-0.8.1/pycardano/certificate.py` & `pycardano-0.9.0/pycardano/certificate.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/cip/cip8.py` & `pycardano-0.9.0/pycardano/cip/cip8.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/coinselection.py` & `pycardano-0.9.0/pycardano/coinselection.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/crypto/bech32.py` & `pycardano-0.9.0/pycardano/crypto/bech32.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/crypto/bip32.py` & `pycardano-0.9.0/pycardano/crypto/bip32.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/exception.py` & `pycardano-0.9.0/pycardano/exception.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/hash.py` & `pycardano-0.9.0/pycardano/hash.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/key.py` & `pycardano-0.9.0/pycardano/key.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         Returns:
             str: JSON representation of the key.
         """
         return json.dumps(
             {
                 "type": self.key_type,
                 "description": self.description,
-                "cborHex": self.to_cbor(),
+                "cborHex": self.to_cbor_hex(),
             }
         )
 
     @classmethod
     def from_json(cls: Type[Key], data: str, validate_type=False) -> Key:
         """Restore a key from a JSON string.
```

### Comparing `pycardano-0.8.1/pycardano/metadata.py` & `pycardano-0.9.0/pycardano/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,9 +123,9 @@
                 return AuxiliaryData(t.from_primitive(value))  # type: ignore
             except DeserializeException:
                 pass
         raise DeserializeException(f"Couldn't parse auxiliary data: {value}")
 
     def hash(self) -> AuxiliaryDataHash:
         return AuxiliaryDataHash(
-            blake2b(self.to_cbor("bytes"), AUXILIARY_DATA_HASH_SIZE, encoder=RawEncoder)  # type: ignore
+            blake2b(self.to_cbor(), AUXILIARY_DATA_HASH_SIZE, encoder=RawEncoder)  # type: ignore
         )
```

### Comparing `pycardano-0.8.1/pycardano/nativescript.py` & `pycardano-0.9.0/pycardano/nativescript.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             return super(NativeScript, InvalidBefore).from_primitive(value[1:])
         elif script_type == InvalidHereAfter._TYPE:
             return super(NativeScript, InvalidHereAfter).from_primitive(value[1:])
         else:
             raise DeserializeException(f"Unknown script type indicator: {script_type}")
 
     def hash(self) -> ScriptHash:
-        cbor_bytes = cast(bytes, self.to_cbor("bytes"))
+        cbor_bytes = cast(bytes, self.to_cbor())
         return ScriptHash(
             blake2b(bytes(1) + cbor_bytes, SCRIPT_HASH_SIZE, encoder=RawEncoder)
         )
 
     @classmethod
     def from_dict(
         cls: Type[NativeScript], script_json: JsonDict
```

### Comparing `pycardano-0.8.1/pycardano/network.py` & `pycardano-0.9.0/pycardano/network.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pycardano/plutus.py` & `pycardano-0.9.0/pycardano/plutus.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,15 +451,15 @@
 
         >>> @dataclass
         ... class Test(PlutusData):
         ...     CONSTR_ID = 1
         ...     a: int
         ...     b: bytes
         >>> test = Test(123, b"321")
-        >>> test.to_cbor()
+        >>> test.to_cbor_hex()
         'd87a9f187b43333231ff'
         >>> assert test == Test.from_cbor("d87a9f187b43333231ff")
     """
 
     CONSTR_ID: ClassVar[int] = 0
     """Constructor ID of this plutus data.
        It is primarily used by Plutus core to reconstruct a data structure from serialized CBOR bytes."""
@@ -662,14 +662,17 @@
 
         Returns:
             PlutusData: The restored PlutusData.
         """
         obj = json.loads(data)
         return cls.from_dict(obj)
 
+    def __deepcopy__(self, memo):
+        return self.__class__.from_cbor(self.to_cbor_hex())
+
 
 @dataclass
 class RawPlutusData(CBORSerializable):
     data: CBORTag
 
     def to_primitive(self) -> CBORTag:
         def _dfs(obj):
@@ -688,16 +691,19 @@
         return _dfs(self.data)
 
     @classmethod
     @limit_primitive_type(CBORTag)
     def from_primitive(cls: Type[RawPlutusData], value: CBORTag) -> RawPlutusData:
         return cls(value)
 
+    def __deepcopy__(self, memo):
+        return self.__class__.from_cbor(self.to_cbor_hex())
+
 
-Datum = Union[PlutusData, dict, IndefiniteList, int, bytes, RawCBOR, RawPlutusData]
+Datum = Union[PlutusData, dict, int, bytes, IndefiniteList, RawCBOR, RawPlutusData]
 """Plutus Datum type. A Union type that contains all valid datum types."""
 
 
 def datum_hash(datum: Datum) -> DatumHash:
     return DatumHash(
         blake2b(
             cbor2.dumps(datum, default=default_encoder),
```

### Comparing `pycardano-0.8.1/pycardano/serialization.py` & `pycardano-0.9.0/pycardano/serialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,34 @@
 from collections import OrderedDict, UserList, defaultdict
 from copy import deepcopy
 from dataclasses import Field, dataclass, fields
 from datetime import datetime
 from decimal import Decimal
 from functools import wraps
 from inspect import isclass
-from typing import Any, Callable, List, Optional, Type, TypeVar, Union, get_type_hints
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    Dict,
+    List,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    get_type_hints,
+)
 
 from cbor2 import CBOREncoder, CBORSimpleValue, CBORTag, dumps, loads, undefined
+from frozendict import frozendict
+from frozenlist import FrozenList
 from pprintpp import pformat
-from typeguard import check_type, typechecked
 
-from pycardano.exception import (
-    DeserializeException,
-    InvalidArgumentException,
-    SerializeException,
-)
+from pycardano.exception import DeserializeException, SerializeException
+from pycardano.types import check_type, typechecked
 
 __all__ = [
     "default_encoder",
     "IndefiniteList",
     "Primitive",
     "CBORBase",
     "CBORSerializable",
@@ -43,14 +52,18 @@
 
 
 class IndefiniteList(UserList):
     def __init__(self, li: Primitive):  # type: ignore
         super().__init__(li)  # type: ignore
 
 
+class IndefiniteFrozenList(FrozenList, IndefiniteList):  # type: ignore
+    pass
+
+
 @dataclass
 class RawCBOR:
     """A wrapper class for bytes that represents a CBOR value."""
 
     cbor: bytes
 
 
@@ -72,14 +85,17 @@
     undefined.__class__,
     datetime,
     re.Pattern,
     CBORSimpleValue,
     CBORTag,
     set,
     frozenset,
+    frozendict,
+    FrozenList,
+    IndefiniteFrozenList,
 ]
 
 PRIMITIVE_TYPES = (
     bytes,
     bytearray,
     str,
     int,
@@ -96,14 +112,17 @@
     type(undefined),
     datetime,
     re.Pattern,
     CBORSimpleValue,
     CBORTag,
     set,
     frozenset,
+    frozendict,
+    FrozenList,
+    IndefiniteFrozenList,
 )
 """
 A list of types that could be encoded by
 `Cbor2 encoder <https://cbor2.readthedocs.io/en/latest/modules/encoder.html>`_ directly.
 """
 
 
@@ -134,27 +153,41 @@
 CBORBase = TypeVar("CBORBase", bound="CBORSerializable")
 
 
 def default_encoder(
     encoder: CBOREncoder, value: Union[CBORSerializable, IndefiniteList]
 ):
     """A fallback function that encodes CBORSerializable to CBOR"""
-    assert isinstance(value, (CBORSerializable, IndefiniteList, RawCBOR)), (
+    assert isinstance(
+        value,
+        (
+            CBORSerializable,
+            IndefiniteList,
+            RawCBOR,
+            FrozenList,
+            IndefiniteFrozenList,
+            frozendict,
+        ),
+    ), (
         f"Type of input value is not CBORSerializable, " f"got {type(value)} instead."
     )
-    if isinstance(value, IndefiniteList):
+    if isinstance(value, (IndefiniteList, IndefiniteFrozenList)):
         # Currently, cbor2 doesn't support indefinite list, therefore we need special
         # handling here to explicitly write header (b'\x9f'), each body item, and footer (b'\xff') to
         # the output bytestring.
         encoder.write(b"\x9f")
         for item in value:
             encoder.encode(item)
         encoder.write(b"\xff")
     elif isinstance(value, RawCBOR):
         encoder.write(value.cbor)
+    elif isinstance(value, FrozenList):
+        encoder.encode(list(value))
+    elif isinstance(value, frozendict):
+        encoder.encode(dict(value))
     else:
         encoder.encode(value.to_validated_primitive())
 
 
 @typechecked
 class CBORSerializable:
     """
@@ -199,66 +232,100 @@
             :const:`Primitive`: A CBOR primitive.
 
         Raises:
             SerializeException: When the object or its elements could not be converted to
                 CBOR primitive types.
         """
         result = self.to_shallow_primitive()
-        container_types = (
-            dict,
-            OrderedDict,
-            defaultdict,
-            set,
-            frozenset,
-            tuple,
-            list,
-            CBORTag,
-            IndefiniteList,
-        )
 
-        def _helper(value):
+        def _dfs(value, freeze=False):
             if isinstance(value, CBORSerializable):
-                return value.to_primitive()
-            elif isinstance(value, container_types):
-                return _dfs(value)
-            else:
-                return value
-
-        def _dfs(value):
-            if isinstance(value, (dict, OrderedDict, defaultdict)):
-                new_result = type(value)()
+                return _dfs(value.to_primitive(), freeze)
+            elif isinstance(value, (dict, OrderedDict, defaultdict)):
+                _dict = type(value)()
                 if hasattr(value, "default_factory"):
-                    new_result.setdefault(value.default_factory)
+                    _dict.setdefault(value.default_factory)
                 for k, v in value.items():
-                    new_result[_helper(k)] = _helper(v)
-                return new_result
+                    _dict[_dfs(k, freeze=True)] = _dfs(v, freeze)
+                if freeze:
+                    return frozendict(_dict)
+                return _dict
             elif isinstance(value, set):
-                return {_helper(v) for v in value}
-            elif isinstance(value, frozenset):
-                return frozenset({_helper(v) for v in value})
+                _set = set(_dfs(v, freeze=True) for v in value)
+                if freeze:
+                    return frozenset(_set)
+                return _set
             elif isinstance(value, tuple):
-                return tuple([_helper(k) for k in value])
+                return tuple(_dfs(v, freeze) for v in value)
             elif isinstance(value, list):
-                return [_helper(k) for k in value]
+                _list = [_dfs(v, freeze) for v in value]
+                if freeze:
+                    fl = FrozenList(_list)
+                    fl.freeze()
+                    return fl
+                return _list
             elif isinstance(value, IndefiniteList):
-                return IndefiniteList([_helper(k) for k in value])
+                _list = [_dfs(v, freeze) for v in value]
+                if freeze:
+                    fl = IndefiniteFrozenList(_list)
+                    fl.freeze()
+                    return fl
+                return IndefiniteList(_list)
             elif isinstance(value, CBORTag):
-                return CBORTag(value.tag, _helper(value.value))
+                return CBORTag(value.tag, _dfs(value.value, freeze))
             else:
                 return value
 
         return _dfs(result)
 
     def validate(self):
         """Validate the data stored in the current instance. Defaults to always pass.
 
         Raises:
             InvalidDataException: When the data is invalid.
         """
-        pass
+        type_hints = get_type_hints(self.__class__)
+
+        def _check_recursive(value, type_hint):
+            if type_hint is Any:
+                return True
+            origin = getattr(type_hint, "__origin__", None)
+            if origin is None:
+                if isinstance(value, CBORSerializable):
+                    value.validate()
+                return isinstance(value, type_hint)
+            elif origin is ClassVar:
+                return _check_recursive(value, type_hint.__args__[0])
+            elif origin is Union:
+                return any(_check_recursive(value, arg) for arg in type_hint.__args__)
+            elif origin is Dict or isinstance(value, (dict, frozendict)):
+                key_type, value_type = type_hint.__args__
+                return all(
+                    _check_recursive(k, key_type) and _check_recursive(v, value_type)
+                    for k, v in value.items()
+                )
+            elif origin in (list, set, tuple):
+                if value is None:
+                    return True
+                args = type_hint.__args__
+                if len(args) == 1:
+                    return all(_check_recursive(item, args[0]) for item in value)
+                elif len(args) > 1:
+                    return all(
+                        _check_recursive(item, arg) for item, arg in zip(value, args)
+                    )
+            return True  # We don't know how to check this type
+
+        for field_name, field_type in type_hints.items():
+            field_value = getattr(self, field_name)
+            if not _check_recursive(field_value, field_type):
+                raise TypeError(
+                    f"Field '{field_name}' should be of type {field_type}, "
+                    f"got {repr(field_value)} instead."
+                )
 
     def to_validated_primitive(self) -> Primitive:
         """Convert the instance and its elements to CBOR primitives recursively with data validated by :meth:`validate`
         method.
 
         Returns:
             :const:`Primitive`: A CBOR primitive.
@@ -284,22 +351,19 @@
         Raises:
             DeserializeException: When the object could not be restored from primitives.
         """
         raise NotImplementedError(
             f"'from_primitive()' is not implemented by {cls.__name__}."
         )
 
-    def to_cbor(self, encoding: str = "hex") -> Union[str, bytes]:
-        """Encode a Python object into CBOR format.
-
-        Args:
-            encoding (str): Encoding to use. Choose from "hex" or "bytes".
+    def to_cbor(self) -> bytes:
+        """Encode a Python object into CBOR bytes.
 
         Returns:
-            Union[str, bytes]: CBOR encoded in a hex string if encoding is hex (default) or bytes if encoding is bytes.
+            bytes: Python object encoded in cbor bytes.
 
         Examples:
             >>> class Test(CBORSerializable):
             ...     def __init__(self, number1, number2):
             ...         self.number1 = number1
             ...         self.number2 = number2
             ...
@@ -309,30 +373,26 @@
             ...     @classmethod
             ...     def from_primitive(cls, value):
             ...         return cls(value[0], value[1])
             ...
             ...     def __repr__(self):
             ...         return f"Test({self.number1}, {self.number2})"
             >>> a = Test(1, 2)
-            >>> a.to_cbor()
+            >>> a.to_cbor().hex()
             '820102'
         """
-        valid_encodings = ("hex", "bytes")
+        return dumps(self, default=default_encoder)
 
-        # Make sure encoding is selected correctly before proceeding further.
-        if encoding not in ("hex", "bytes"):
-            raise InvalidArgumentException(
-                f"Invalid encoding: {encoding}. Please choose from {valid_encodings}"
-            )
+    def to_cbor_hex(self) -> str:
+        """Encode a Python object into CBOR hex.
 
-        cbor = dumps(self, default=default_encoder)
-        if encoding == "hex":
-            return cbor.hex()
-        else:
-            return cbor
+        Returns:
+            str: Python object encoded in cbor hex string.
+        """
+        return self.to_cbor().hex()
 
     @classmethod
     def from_cbor(cls, payload: Union[str, bytes]) -> CBORSerializable:
         """Restore a CBORSerializable object from a CBOR.
 
         Args:
             payload (Union[str, bytes]): CBOR bytes or hex string to restore from.
@@ -355,15 +415,15 @@
             ...     @classmethod
             ...     def from_primitive(cls, value):
             ...         return cls(value[0], value[1])
             ...
             ...     def __repr__(self):
             ...         return f"Test({self.number1}, {self.number2})"
             >>> a = Test(1, 2)
-            >>> cbor_hex = a.to_cbor()
+            >>> cbor_hex = a.to_cbor_hex()
             >>> print(Test.from_cbor(cbor_hex))
             Test(1, 2)
 
             For a CBORSerializable that has CBORSerializables as attributes, we will need to pass
             each child value to the :meth:`from_primitive` method of its corresponding CBORSerializable. Example:
 
             >>> class TestParent(CBORSerializable):
@@ -382,15 +442,15 @@
             ...
             ...     def __repr__(self):
             ...         return f"TestParent({self.number1}, {self.test})"
             >>> a = Test(1, 2)
             >>> b = TestParent(3, a)
             >>> b
             TestParent(3, Test(1, 2))
-            >>> cbor_hex = b.to_cbor()
+            >>> cbor_hex = b.to_cbor_hex()
             >>> cbor_hex
             '8203820102'
             >>> print(TestParent.from_cbor(cbor_hex))
             TestParent(3, Test(1, 2))
 
         """
         if type(payload) == str:
@@ -443,15 +503,18 @@
                 f"List types need exactly one type argument, but got {t_args}"
             )
         t = t_args[0]
         if not isinstance(v, list):
             raise DeserializeException(f"Expected type list but got {type(v)}")
         return IndefiniteList([_restore_typed_primitive(t, w) for w in v])
     elif isclass(t) and issubclass(t, IndefiniteList):
-        return IndefiniteList(v)
+        try:
+            return IndefiniteList(v)
+        except TypeError:
+            raise DeserializeException(f"Can not initialize IndefiniteList from {v}")
     elif hasattr(t, "__origin__") and (t.__origin__ is dict):
         t_args = t.__args__
         if len(t_args) != 2:
             raise DeserializeException(
                 f"Dict types need exactly two type arguments, but got {t_args}"
             )
         key_t = t_args[0]
@@ -501,16 +564,16 @@
         >>> @dataclass
         ... class Test2(ArrayCBORSerializable):
         ...     c: str
         ...     test1: Test1
         >>> t = Test2(c="c", test1=Test1(a="a"))
         >>> t
         Test2(c='c', test1=Test1(a='a', b=None))
-        >>> cbor_hex = t.to_cbor()
-        >>> cbor_hex
+        >>> cbor_hex = t.to_cbor_hex() # doctest: +SKIP
+        >>> cbor_hex # doctest: +SKIP
         '826163826161f6'
         >>> Test2.from_cbor(cbor_hex) # doctest: +SKIP
         Test2(c='c', test1=Test1(a='a', b=None))
 
         A value of `None` will be encoded as nil (#7.22) in cbor. This will become a problem if the field is meant to be
         optional. To exclude an optional attribute from cbor, we can use `field` constructor with a metadata field
         "optional" set to True and default value set to `None`.
@@ -530,16 +593,16 @@
         ...     c: str
         ...     test1: Test1
         >>> t = Test2(c="c", test1=Test1(a="a"))
         >>> t
         Test2(c='c', test1=Test1(a='a', b=None))
         >>> t.to_primitive() # Notice below that attribute "b" is not included in converted primitive.
         ['c', ['a']]
-        >>> cbor_hex = t.to_cbor()
-        >>> cbor_hex
+        >>> cbor_hex = t.to_cbor_hex() # doctest: +SKIP
+        >>> cbor_hex # doctest: +SKIP
         '826163816161'
         >>> Test2.from_cbor(cbor_hex) # doctest: +SKIP
         Test2(c='c', test1=Test1(a='a', b=None))
     """
 
     def to_shallow_primitive(self) -> List[Primitive]:
         """
@@ -617,16 +680,16 @@
         ...     c: str=None
         ...     test1: Test1=field(default_factory=Test1)
         >>> t = Test2(test1=Test1(a="a"))
         >>> t
         Test2(c=None, test1=Test1(a='a', b=''))
         >>> t.to_primitive()
         {'c': None, 'test1': {'a': 'a', 'b': ''}}
-        >>> cbor_hex = t.to_cbor()
-        >>> cbor_hex
+        >>> cbor_hex = t.to_cbor_hex() # doctest: +SKIP
+        >>> cbor_hex # doctest: +SKIP
         'a26163f6657465737431a261616161616260'
         >>> Test2.from_cbor(cbor_hex) # doctest: +SKIP
         Test2(c=None, test1=Test1(a='a', b=''))
 
         In the example above, all keys in the map share the same name as their corresponding attributes. However,
         sometimes we want to use different keys when serializing some attributes, this could be achieved by adding a
         "key" value to the metadata of a field. Example:
@@ -641,16 +704,16 @@
         ...     c: str=field(default=None, metadata={"key": "0", "optional": True})
         ...     test1: Test1=field(default_factory=Test1, metadata={"key": "1"})
         >>> t = Test2(test1=Test1(a="a"))
         >>> t
         Test2(c=None, test1=Test1(a='a', b=''))
         >>> t.to_primitive()
         {'1': {'0': 'a', '1': ''}}
-        >>> cbor_hex = t.to_cbor()
-        >>> cbor_hex
+        >>> cbor_hex = t.to_cbor_hex() # doctest: +SKIP
+        >>> cbor_hex # doctest: +SKIP
         'a16131a261306161613160'
         >>> Test2.from_cbor(cbor_hex) # doctest: +SKIP
         Test2(c=None, test1=Test1(a='a', b=''))
     """
 
     def to_shallow_primitive(self) -> Primitive:
         primitives = {}
@@ -772,15 +835,15 @@
     def __deepcopy__(self, memodict={}):
         return self.__class__(deepcopy(self.data))
 
     def to_shallow_primitive(self) -> dict:
         # Sort keys in a map according to https://datatracker.ietf.org/doc/html/rfc7049#section-3.9
         def _get_sortable_val(key):
             if isinstance(key, CBORSerializable):
-                cbor_bytes = key.to_cbor("bytes")
+                cbor_bytes = key.to_cbor()
             else:
                 cbor_bytes = dumps(key)
             return len(cbor_bytes), cbor_bytes
 
         return dict(sorted(self.data.items(), key=lambda x: _get_sortable_val(x[0])))
 
     @classmethod
```

### Comparing `pycardano-0.8.1/pycardano/transaction.py` & `pycardano-0.9.0/pycardano/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pprint import pformat
 from typing import Any, Callable, List, Optional, Type, Union
 
 import cbor2
 from cbor2 import CBORTag
 from nacl.encoding import RawEncoder
 from nacl.hash import blake2b
-from typeguard import typechecked
 
 from pycardano.address import Address
 from pycardano.certificate import Certificate
 from pycardano.exception import InvalidDataException, InvalidOperationException
 from pycardano.hash import (
     TRANSACTION_HASH_SIZE,
     AuxiliaryDataHash,
@@ -35,14 +34,15 @@
     CBORSerializable,
     DictCBORSerializable,
     MapCBORSerializable,
     Primitive,
     default_encoder,
     list_hook,
 )
+from pycardano.types import typechecked
 from pycardano.witness import TransactionWitnessSet
 
 __all__ = [
     "TransactionInput",
     "AssetName",
     "Asset",
     "MultiAsset",
@@ -386,14 +386,15 @@
     def __post_init__(self):
         if isinstance(self.address, str):
             self.address = Address.from_primitive(self.address)
         if isinstance(self.amount, int):
             self.amount = Value(self.amount)
 
     def validate(self):
+        super().validate()
         if isinstance(self.amount, int) and self.amount < 0:
             raise InvalidDataException(
                 f"Transaction output cannot have negative amount of ADA or "
                 f"native asset: \n {self.amount}"
             )
         if isinstance(self.amount, Value) and (
             self.amount.coin < 0
@@ -431,15 +432,15 @@
 
     @classmethod
     def from_primitive(
         cls: Type[TransactionOutput], value: Primitive
     ) -> TransactionOutput:
         if isinstance(value, list):
             output = _TransactionOutputLegacy.from_primitive(value)
-            return cls(output.address, output.amount, datum=output.datum_hash)
+            return cls(output.address, output.amount, datum_hash=output.datum_hash)
         else:
             output = _TransactionOutputPostAlonzo.from_primitive(value)
             datum = output.datum.datum if output.datum else None
             if isinstance(datum, DatumHash):
                 return cls(
                     output.address,
                     output.amount,
@@ -461,17 +462,15 @@
 
     output: TransactionOutput
 
     def __repr__(self):
         return pformat(vars(self))
 
     def __hash__(self):
-        return hash(
-            blake2b(self.input.to_cbor("bytes") + self.output.to_cbor("bytes"), 32)
-        )
+        return hash(blake2b(self.input.to_cbor() + self.output.to_cbor(), 32))
 
 
 class Withdrawals(DictCBORSerializable):
     """A disctionary of reward addresses to reward withdrawal amount.
 
     Key is address bytes, value is an integer.
 
@@ -567,15 +566,15 @@
             "key": 18,
             "object_hook": list_hook(TransactionInput),
             "optional": True,
         },
     )
 
     def hash(self) -> bytes:
-        return blake2b(self.to_cbor(encoding="bytes"), TRANSACTION_HASH_SIZE, encoder=RawEncoder)  # type: ignore
+        return blake2b(self.to_cbor(), TRANSACTION_HASH_SIZE, encoder=RawEncoder)  # type: ignore
 
     @property
     def id(self) -> TransactionId:
         return TransactionId(self.hash())
 
 
 @dataclass(repr=False)
```

### Comparing `pycardano-0.8.1/pycardano/txbuilder.py` & `pycardano-0.9.0/pycardano/txbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
 
     reference_inputs: Set[Union[UTxO, TransactionInput]] = field(
         init=False, default_factory=lambda: set()
     )
 
     _inputs: List[UTxO] = field(init=False, default_factory=lambda: [])
 
+    _potential_inputs: List[UTxO] = field(init=False, default_factory=lambda: [])
+
     _excluded_inputs: List[UTxO] = field(init=False, default_factory=lambda: [])
 
     _input_addresses: List[Union[Address, str]] = field(
         init=False, default_factory=lambda: []
     )
 
     _outputs: List[TransactionOutput] = field(init=False, default_factory=lambda: [])
@@ -236,15 +238,15 @@
             self._inputs_to_redeemers[utxo] = redeemer
 
         if utxo.output.script:
             self._inputs_to_scripts[utxo] = utxo.output.script
             self.reference_inputs.add(utxo)
             self._reference_scripts.append(utxo.output.script)
         elif not script:
-            for i in self.context.utxos(str(utxo.output.address)):
+            for i in self.context.utxos(utxo.output.address):
                 if i.output.script:
                     self._inputs_to_scripts[utxo] = i.output.script
                     self.reference_inputs.add(i)
                     self._reference_scripts.append(i.output.script)
                     break
         elif isinstance(script, UTxO):
             assert script.output.script is not None
@@ -328,14 +330,18 @@
         return self
 
     @property
     def inputs(self) -> List[UTxO]:
         return self._inputs
 
     @property
+    def potential_inputs(self) -> List[UTxO]:
+        return self._potential_inputs
+
+    @property
     def excluded_inputs(self) -> List[UTxO]:
         return self._excluded_inputs
 
     @excluded_inputs.setter
     def excluded_inputs(self, excluded_inputs: List[UTxO]):
         self._excluded_inputs = excluded_inputs
 
@@ -586,15 +592,15 @@
 
         # Calculate minimum ada requirements for more precise value size
         required_lovelace = min_lovelace_post_alonzo(
             TransactionOutput(output.address, attempt_amount), self.context
         )
         attempt_amount.coin = required_lovelace
 
-        return len(attempt_amount.to_cbor("bytes")) > max_val_size
+        return len(attempt_amount.to_cbor()) > max_val_size
 
     def _pack_tokens_for_change(
         self,
         change_address: Optional[Address],
         change_estimator: Value,
         max_val_size: int,
     ) -> List[MultiAsset]:
@@ -646,15 +652,15 @@
             # Calculate min lovelace required for more precise size
             updated_amount = deepcopy(output.amount)
             required_lovelace = min_lovelace_post_alonzo(
                 TransactionOutput(change_address, updated_amount), self.context
             )
             updated_amount.coin = required_lovelace
 
-            if len(updated_amount.to_cbor("bytes")) > max_val_size:
+            if len(updated_amount.to_cbor()) > max_val_size:
                 output.amount = old_amount
                 break
 
         multi_asset_arr.append(output.amount.multi_asset)
         # Remove records where MultiAsset is null due to overflow of adding
         # items at the beginning of next policy to previous policy MultiAssets
         return multi_asset_arr
@@ -722,17 +728,15 @@
         return results
 
     def _set_redeemer_index(self):
         # Set redeemers' index according to section 4.1 in
         # https://hydra.iohk.io/build/13099856/download/1/alonzo-changes.pdf
 
         if self.mint:
-            sorted_mint_policies = sorted(
-                self.mint.keys(), key=lambda x: x.to_cbor("bytes")
-            )
+            sorted_mint_policies = sorted(self.mint.keys(), key=lambda x: x.to_cbor())
         else:
             sorted_mint_policies = []
 
         for i, utxo in enumerate(self.inputs):
             if (
                 utxo in self._inputs_to_redeemers
                 and self._inputs_to_redeemers[utxo].tag == RedeemerTag.SPEND
@@ -801,15 +805,15 @@
         if tx_body.fee == 0:
             # When fee is not specified, we will use max possible fee to fill in the fee field.
             # This will make sure the size of fee field itself is taken into account during fee estimation.
             tx_body.fee = max_tx_fee(self.context)
 
         witness = self._build_fake_witness_set()
         tx = Transaction(tx_body, witness, True, self.auxiliary_data)
-        size = len(tx.to_cbor("bytes"))
+        size = len(tx.to_cbor())
         if size > self.context.protocol_param.max_tx_size:
             raise InvalidTransactionException(
                 f"Transaction size ({size}) exceeds the max limit "
                 f"({self.context.protocol_param.max_tx_size}). Please try reducing the "
                 f"number of inputs or outputs."
             )
         return tx
@@ -859,15 +863,15 @@
     def _estimate_fee(self):
         plutus_execution_units = ExecutionUnits(0, 0)
         for redeemer in self.redeemers:
             plutus_execution_units += redeemer.ex_units
 
         estimated_fee = fee(
             self.context,
-            len(self._build_full_fake_tx().to_cbor("bytes")),
+            len(self._build_full_fake_tx().to_cbor()),
             plutus_execution_units.steps,
             plutus_execution_units.mem,
         )
 
         return estimated_fee
 
     def build(
@@ -980,29 +984,36 @@
             unfulfilled_amount.coin = max(0, unfulfilled_amount.coin)
 
         # Clean up all non-positive assets
         unfulfilled_amount.multi_asset = unfulfilled_amount.multi_asset.filter(
             lambda p, n, v: v > 0
         )
 
+        # Create a set of all seen utxos in addition to other utxo lists.
+        # We need this set to avoid adding the same utxo twice.
+        # The reason of not turning all utxo lists into sets is that we want to keep the order of utxos and make
+        # utxo selection deterministic.
+        seen_utxos = set(selected_utxos)
+
         # When there are positive coin or native asset quantity in unfulfilled Value
         if Value() < unfulfilled_amount:
             additional_utxo_pool = []
             additional_amount = Value()
+
+            for utxo in self.potential_inputs:
+                additional_amount += utxo.output.amount
+                seen_utxos.add(utxo)
+                additional_utxo_pool.append(utxo)
+
             for address in self.input_addresses:
-                for utxo in self.context.utxos(str(address)):
-                    if (
-                        utxo not in selected_utxos
-                        and utxo not in self.excluded_inputs
-                        and not utxo.output.datum_hash  # UTxO with datum should be added by using `add_script_input`
-                        and not utxo.output.datum
-                        and not utxo.output.script
-                    ):
+                for utxo in self.context.utxos(address):
+                    if utxo not in seen_utxos and utxo not in self.excluded_inputs:
                         additional_utxo_pool.append(utxo)
                         additional_amount += utxo.output.amount
+                        seen_utxos.add(utxo)
 
             for index, selector in enumerate(self.utxo_selectors):
                 try:
                     selected, _ = selector.select(
                         additional_utxo_pool,
                         [
                             TransactionOutput(
@@ -1113,22 +1124,22 @@
                         and candidate.output.amount.coin > 2000000
                     ):
                         self.collaterals.append(candidate)
                         cur_total += candidate.output.amount
 
             sorted_inputs = sorted(
                 self.inputs.copy(),
-                key=lambda i: (len(i.output.to_cbor()), -i.output.amount.coin),
+                key=lambda i: (len(i.output.to_cbor_hex()), -i.output.amount.coin),
             )
             _add_collateral_input(tmp_val, sorted_inputs)
 
             if tmp_val.coin < collateral_amount:
                 sorted_inputs = sorted(
-                    self.context.utxos(str(collateral_return_address)),
-                    key=lambda i: (len(i.output.to_cbor()), -i.output.amount.coin),
+                    self.context.utxos(collateral_return_address),
+                    key=lambda i: (len(i.output.to_cbor_hex()), -i.output.amount.coin),
                 )
                 _add_collateral_input(tmp_val, sorted_inputs)
 
         total_input = Value()
 
         for utxo in self.collaterals:
             total_input += utxo.output.amount
@@ -1203,15 +1214,15 @@
             change_address, merge_change, collateral_change_address
         )
         witness_set = tmp_builder._build_fake_witness_set()
         tx = Transaction(
             tx_body, witness_set, auxiliary_data=tmp_builder.auxiliary_data
         )
 
-        return self.context.evaluate_tx(tx.to_cbor())
+        return self.context.evaluate_tx(tx)
 
     def build_and_sign(
         self,
         signing_keys: List[Union[SigningKey, ExtendedSigningKey]],
         change_address: Optional[Address] = None,
         merge_change: Optional[bool] = False,
         collateral_change_address: Optional[Address] = None,
@@ -1233,20 +1244,25 @@
             auto_validity_start_offset (Optional[int]): Automatically set the validity start interval of the transaction
                 to the current slot number + the given offset (default -1000).
                 A manually set validity start will always take precedence.
             auto_ttl_offset (Optional[int]): Automatically set the validity end interval (ttl) of the transaction
                 to the current slot number + the given offset (default 10_000).
                 A manually set ttl will always take precedence.
             auto_required_signers (Optional[bool]): Automatically add all pubkeyhashes of transaction inputs
-                to required signatories (default only for Smart Contract transactions).
+                and the given signers to required signatories (default only for Smart Contract transactions).
                 Manually set required signers will always take precedence.
 
         Returns:
             Transaction: A signed transaction.
         """
+        # The given signers should be required signers if they weren't added yet
+        if auto_required_signers and self.scripts and not self.required_signers:
+            self.required_signers = [
+                s.to_verification_key().hash() for s in signing_keys
+            ]
 
         tx_body = self.build(
             change_address=change_address,
             merge_change=merge_change,
             collateral_change_address=collateral_change_address,
             auto_validity_start_offset=auto_validity_start_offset,
             auto_ttl_offset=auto_ttl_offset,
```

### Comparing `pycardano-0.8.1/pycardano/utils.py` & `pycardano-0.9.0/pycardano/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     max_mem_unit: int = 0,
 ) -> int:
     """Calculate fee based on the length of a transaction's CBOR bytes and script execution.
 
     Args:
         context (ChainConext): A chain context.
         length (int): The length of CBOR bytes, which could usually be derived
-            by `len(tx.to_cbor("bytes"))`.
+            by `len(tx.to_cbor())`.
         exec_steps (Optional[int]): Number of execution steps run by plutus scripts in the transaction.
         max_mem_unit (Optional[int]): Max numer of memory units run by plutus scripts in the transaction.
 
     Return:
         int: Minimum acceptable transaction fee.
     """
     return (
@@ -176,15 +176,15 @@
         output.datum_hash,
         output.datum,
         output.script,
         True,
     )
 
     return (
-        constant_overhead + len(tmp_out.to_cbor("bytes"))
+        constant_overhead + len(tmp_out.to_cbor())
     ) * context.protocol_param.coins_per_utxo_byte
 
 
 def script_data_hash(
     redeemers: List[Redeemer],
     datums: List[Datum],
     cost_models: Optional[Union[CostModels, Dict]] = None,
```

### Comparing `pycardano-0.8.1/pycardano/witness.py` & `pycardano-0.9.0/pycardano/witness.py`

 * *Files identical despite different names*

### Comparing `pycardano-0.8.1/pyproject.toml` & `pycardano-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycardano"
-version = "0.8.1"
+version = "0.9.0"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
@@ -28,14 +28,16 @@
 typeguard = "^2.13.3"
 blockfrost-python = "0.5.3"
 websocket-client = "^1.4.1"
 cose = "0.9.dev8"
 pprintpp = "^0.4.0"
 mnemonic = "^0.20"
 ECPy = "^1.2.5"
+frozendict = "^2.3.8"
+frozenlist = "^1.3.3"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.1.1"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
```

### Comparing `pycardano-0.8.1/PKG-INFO` & `pycardano-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycardano
-Version: 0.8.1
+Version: 0.9.0
 Summary: A Cardano library in Python
 Home-page: https://github.com/Python-Cardano/pycardano
 License: MIT
 Keywords: python,cardano,blockchain,crypto
 Author: Jerry
 Author-email: jerrycgh@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -24,14 +24,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: ECPy (>=1.2.5,<2.0.0)
 Requires-Dist: PyNaCl (>=1.5.0,<2.0.0)
 Requires-Dist: blockfrost-python (==0.5.3)
 Requires-Dist: cbor2 (>=5.4.3,<6.0.0)
 Requires-Dist: cose (==0.9.dev8)
+Requires-Dist: frozendict (>=2.3.8,<3.0.0)
+Requires-Dist: frozenlist (>=1.3.3,<2.0.0)
 Requires-Dist: mnemonic (>=0.20,<0.21)
 Requires-Dist: pprintpp (>=0.4.0,<0.5.0)
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
 Requires-Dist: websocket-client (>=1.4.1,<2.0.0)
 Project-URL: Documentation, https://pycardano.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/cffls/pycardano
 Description-Content-Type: text/markdown
@@ -139,15 +141,15 @@
 builder = TransactionBuilder(context)
 
 # Tell the builder that transaction input will come from a specific address, assuming that there are some ADA and native
 # assets sitting at this address. "add_input_address" could be called multiple times with different address.
 builder.add_input_address(address)
 
 # Get all UTxOs currently sitting at this address
-utxos = context.utxos(str(address))
+utxos = context.utxos(address)
 
 # We can also tell the builder to include a specific UTxO in the transaction.
 # Similarly, "add_input" could be called multiple times.
 builder.add_input(utxos[0])
 
 # Send 1.5 ADA and a native asset (CHOC) in quantity of 2000 to an address.
 builder.add_output(
@@ -190,15 +192,15 @@
     )
 )
 
 # Create final signed transaction
 signed_tx = builder.build_and_sign([psk], change_address=address)
 
 # Submit signed transaction to the network
-context.submit_tx(signed_tx.to_cbor())
+context.submit_tx(signed_tx)
 
 ```
 </details>
 
 See more usages under [examples](https://github.com/Python-Cardano/pycardano/tree/main/examples).
 
 
@@ -292,9 +294,11 @@
 ## Sponsors :heart:
 
 <p align="left">
   <a href="https://github.com/KtorZ"><img src="https://avatars.githubusercontent.com/u/5680256?s=50&v=4"/></a>
   <a href="https://github.com/CardanoDur"><img width="50" src="https://avatars.githubusercontent.com/u/1000466?s=50&v=4"/></a>
   <a href="https://github.com/huths0lo"><img width="50" src="https://avatars.githubusercontent.com/u/78839856?s=50&v=4"/></a>
   <a href="https://github.com/markrufino"><img width="50" src="https://avatars.githubusercontent.com/u/30117352?v=4"/></a>
+  <a href="https://github.com/OpShin"><img width="50" src="https://avatars.githubusercontent.com/u/102762047?s=200&v=4"/></a>
+  <a href="https://github.com/aada-finance"><img width="50" src="https://avatars.githubusercontent.com/u/89693711?v=4"/></a>
 </p>
```

