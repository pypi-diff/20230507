# Comparing `tmp/tplink-ess-lib-0.4.4.tar.gz` & `tmp/tplink-ess-lib-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tplink-ess-lib-0.4.4.tar", last modified: Tue Feb  7 13:37:25 2023, max compression
+gzip compressed data, was "tplink-ess-lib-0.4.5.tar", last modified: Sun May  7 01:36:58 2023, max compression
```

## Comparing `tplink-ess-lib-0.4.4.tar` & `tplink-ess-lib-0.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 13:37:25.500077 tplink-ess-lib-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-07 13:37:25.500077 tplink-ess-lib-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-07 13:37:19.000000 tplink-ess-lib-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 13:37:25.500077 tplink-ess-lib-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-07 13:37:19.000000 tplink-ess-lib-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 13:37:25.500077 tplink-ess-lib-0.4.4/tplink_ess_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-02-07 13:37:19.000000 tplink-ess-lib-0.4.4/tplink_ess_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-07 13:37:19.000000 tplink-ess-lib-0.4.4/tplink_ess_lib/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-02-07 13:37:19.000000 tplink-ess-lib-0.4.4/tplink_ess_lib/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-02-07 13:37:19.000000 tplink-ess-lib-0.4.4/tplink_ess_lib/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 13:37:25.500077 tplink-ess-lib-0.4.4/tplink_ess_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-07 13:37:25.000000 tplink-ess-lib-0.4.4/tplink_ess_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-07 13:37:25.000000 tplink-ess-lib-0.4.4/tplink_ess_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 13:37:25.000000 tplink-ess-lib-0.4.4/tplink_ess_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 13:37:25.000000 tplink-ess-lib-0.4.4/tplink_ess_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-07 13:37:25.000000 tplink-ess-lib-0.4.4/tplink_ess_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:36:58.978880 tplink-ess-lib-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-07 01:36:58.974880 tplink-ess-lib-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-07 01:36:54.000000 tplink-ess-lib-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 01:36:58.978880 tplink-ess-lib-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-07 01:36:54.000000 tplink-ess-lib-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:36:58.974880 tplink-ess-lib-0.4.5/tplink_ess_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-07 01:36:54.000000 tplink-ess-lib-0.4.5/tplink_ess_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-07 01:36:54.000000 tplink-ess-lib-0.4.5/tplink_ess_lib/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-07 01:36:54.000000 tplink-ess-lib-0.4.5/tplink_ess_lib/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-07 01:36:54.000000 tplink-ess-lib-0.4.5/tplink_ess_lib/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:36:58.974880 tplink-ess-lib-0.4.5/tplink_ess_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-07 01:36:58.000000 tplink-ess-lib-0.4.5/tplink_ess_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-07 01:36:58.000000 tplink-ess-lib-0.4.5/tplink_ess_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:36:58.000000 tplink-ess-lib-0.4.5/tplink_ess_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:36:58.000000 tplink-ess-lib-0.4.5/tplink_ess_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 01:36:58.000000 tplink-ess-lib-0.4.5/tplink_ess_lib.egg-info/top_level.txt
```

### Comparing `tplink-ess-lib-0.4.4/PKG-INFO` & `tplink-ess-lib-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplink-ess-lib
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python package and software for the TP-Link TL-SG105E and TL-SG108E smart switches
 Home-page: https://github.com/firstof9/tplink-ess-lib
 Author: firstof9
 Author-email: firstof9@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/firstof9/tplink-ess-lib
 Platform: UNKNOWN
```

### Comparing `tplink-ess-lib-0.4.4/README.md` & `tplink-ess-lib-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `tplink-ess-lib-0.4.4/setup.py` & `tplink-ess-lib-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for tplink-ess-lib."""
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.4.4"
+VERSION = "0.4.5"
 
 setup(
     name="tplink-ess-lib",
     version=VERSION,
     url="https://github.com/firstof9/tplink-ess-lib",
     download_url="https://github.com/firstof9/tplink-ess-lib",
     author="firstof9",
```

### Comparing `tplink-ess-lib-0.4.4/tplink_ess_lib/__init__.py` & `tplink-ess-lib-0.4.5/tplink_ess_lib/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,72 +55,79 @@
         16640: ("hex", "mirror", 0),
         16384: ("stat", "stats", 0),
         17152: ("bool", "loop_prev", 0),
     }
 
     tp_ids = {v[1]: k for k, v in working_ids_tp.items()}
 
-    def __init__(self, host_mac: str = "", user: str = "", pwd: str = "") -> None:
+    def __init__(
+        self, host_mac: str = "", user: str = "", pwd: str = "", testing: bool = False
+    ) -> None:
         """Connect or discover a TP-Link ESS switch on the network."""
         if not host_mac:
             _LOGGER.error("MAC address missing.")
             raise MissingMac
 
         self._user = user
         self._pwd = pwd
         self._host_mac = host_mac
         self._data: Dict[Any, Any] = {}
+        self._testing = testing
 
-    async def discovery(self, testing: bool = False) -> list[dict]:
+    async def discovery(self) -> list[dict]:
         """Return a list of unique switches found by discovery."""
         switches = {}
-        with Network(self._host_mac) as net:
+        with Network(self._host_mac, testing=self._testing) as net:
             net.send(Network.BROADCAST_MAC, Protocol.DISCOVERY, {})
             while True:
                 try:
-                    header, payload = net.receive(testing)
+                    header, payload = net.receive()
                     switches[header["switch_mac"]] = TpLinkESS.parse_response(payload)
                 except ConnectionProblem:
                     break
         return list(switches.values())
 
-    async def query(self, switch_mac: str, action: str, testing: bool = False) -> dict:
+    async def query(self, switch_mac: str, action: str) -> dict:
         """
         Send a query.
 
         Sends a query to a specific switch and return the results
         as a dict.
         """
-        with Network(host_mac=self._host_mac) as net:
+        with Network(host_mac=self._host_mac, testing=self._testing) as net:
             header, payload = net.query(  # pylint: disable=unused-variable
                 switch_mac=switch_mac,
                 op_code=Protocol.GET,
                 payload=[(Protocol.tp_ids[action], b"")],
-                testing=testing,
             )
             return TpLinkESS.parse_response(payload)
 
-    async def update_data(self, switch_mac, testing: bool = False) -> dict:
-        """Refresh switch data."""
+    async def update_data(self, switch_mac, action_names=None) -> dict:
+        """Refresh switch data. Optional list of items to query (default all)."""
         try:
-            net = Network(host_mac=self._host_mac)
+            net = Network(host_mac=self._host_mac, testing=self._testing)
         except OSError as err:
             _LOGGER.error("Problems with network interface: %s", err)
             raise err
         # Login to switch
-        net.login(switch_mac, self._user, self._pwd, testing)
-        actions = TpLinkESS.working_ids_tp
+        net.login(switch_mac, self._user, self._pwd)
+        if action_names is None:
+            actions = TpLinkESS.working_ids_tp
+        else:
+            actions = {
+                TpLinkESS.tp_ids[name]: TpLinkESS.working_ids_tp[TpLinkESS.tp_ids[name]]
+                for name in action_names
+            }
 
         for action in actions:
             try:
                 header, payload = net.query(  # pylint: disable=unused-variable
                     switch_mac=switch_mac,
                     op_code=Protocol.GET,
                     payload=[(action, b"")],
-                    testing=testing,
                 )
                 index = TpLinkESS.working_ids_tp[action][1]
                 self._data[index] = TpLinkESS.parse_response(payload)
             except ConnectionProblem:
                 break
 
         return self._data
```

### Comparing `tplink-ess-lib-0.4.4/tplink_ess_lib/network.py` & `tplink-ess-lib-0.4.5/tplink_ess_lib/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,19 +30,20 @@
     BROADCAST_MAC = "00:00:00:00:00:00"
     UDP_SEND_TO_PORT = 29808
     UDP_RECEIVE_FROM_PORT = 29809
 
     SOCKET_TIMEOUT = 2  # timeout for socket operations
     RECEIVE_TIMEOUT = 10  # total amount of time to wait for tx/rx sequence
 
-    def __init__(self, host_mac):
+    def __init__(self, host_mac, testing: bool = False):
         """Initialize."""
         self.host_mac = host_mac
         self.sequence_id = random.randint(0, 1000)
         self.token_id = None
+        self.testing = testing
 
         # Sending socket
         self.s_socket = socket.socket(
             socket.AF_INET,
             socket.SOCK_DGRAM,
             socket.IPPROTO_UDP,
         )
@@ -90,37 +91,37 @@
         packet = Protocol.encode(packet)
         _LOGGER.debug("Sending Header: %s", str(header))
         _LOGGER.debug("Sending Payload: %s", str(payload))
 
         # Send packet
         self.s_socket.sendto(packet, (Network.BROADCAST_ADDR, Network.UDP_SEND_TO_PORT))
 
-    def receive(self, testing: bool = False):
+    def receive(self):
         """Wait for an incoming packet, then return header+payload as a tuple."""
         end_time = datetime.now() + timedelta(seconds=Network.RECEIVE_TIMEOUT)
         while (data := self.receive_socket()) and datetime.now() < end_time:
             data = Protocol.decode(data)
             _LOGGER.debug("Receive Packet: %s", data.hex())
             header, payload = Protocol.split(data)
             header, payload = Protocol.interpret_header(
                 header
             ), Protocol.interpret_payload(payload)
             _LOGGER.debug("Received Header: %s", str(header))
             _LOGGER.debug("Received Payload: %s", str(payload))
             # check sequence_id alignment
-            if self.sequence_id != header["sequence_id"] and not testing:
+            if self.sequence_id != header["sequence_id"] and not self.testing:
                 _LOGGER.debug(
                     "Ignoring sequence_id %d expected %d",
                     header["sequence_id"],
                     self.sequence_id,
                 )
                 continue
             # check host_mac alignment
             data_mac = mac_to_str(header["host_mac"])
-            if self.host_mac != data_mac and not testing:
+            if self.host_mac != data_mac and not self.testing:
                 _LOGGER.debug(
                     "Ignoring host-mac %s expected %s", data_mac, self.host_mac
                 )
                 continue
             self.token_id = header["token_id"]
             return header, payload
         raise ConnectionProblem()
@@ -130,42 +131,36 @@
         try:
             data, addr = self.r_socket.recvfrom(1500)  # pylint: disable=unused-variable
         except OSError as err:
             _LOGGER.debug("Error: %s", err)
             return False
         return data
 
-    def query(self, switch_mac, op_code, payload, testing: bool = False):
+    def query(self, switch_mac, op_code, payload):
         """
         Send packet to switch.
 
         Send a packet to the given switch, then wait for a response and
         return header+payload as a tuple.
         """
         self.send(switch_mac, op_code, payload)
-        return self.receive(testing)
+        return self.receive()
 
     @staticmethod
     def login_dict(username, password):
         """Return login dict."""
         return [
             (Protocol.get_id("username"), username.encode("ascii") + b"\x00"),
             (Protocol.get_id("password"), password.encode("ascii") + b"\x00"),
         ]
 
-    def login(
-        self, switch_mac: str, username: str, password: str, testing: bool = False
-    ):
+    def login(self, switch_mac: str, username: str, password: str):
         """Send login credentials to switch."""
-        self.query(
-            switch_mac, Protocol.GET, [(Protocol.get_id("get_token_id"), b"")], testing
-        )
-        self.query(
-            switch_mac, Protocol.LOGIN, self.login_dict(username, password), testing
-        )
+        self.query(switch_mac, Protocol.GET, [(Protocol.get_id("get_token_id"), b"")])
+        self.query(switch_mac, Protocol.LOGIN, self.login_dict(username, password))
 
     def set(self, switch_mac, username, password, payload):
         """Authenticate to the switch."""
         self.query(switch_mac, Protocol.GET, [(Protocol.get_id("get_token_id"), b"")])
         real_payload = self.login_dict(username, password)
         real_payload += payload
         header, payload = self.query(switch_mac, Protocol.LOGIN, real_payload)
```

### Comparing `tplink-ess-lib-0.4.4/tplink_ess_lib/protocol.py` & `tplink-ess-lib-0.4.5/tplink_ess_lib/protocol.py`

 * *Files identical despite different names*

### Comparing `tplink-ess-lib-0.4.4/tplink_ess_lib.egg-info/PKG-INFO` & `tplink-ess-lib-0.4.5/tplink_ess_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplink-ess-lib
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python package and software for the TP-Link TL-SG105E and TL-SG108E smart switches
 Home-page: https://github.com/firstof9/tplink-ess-lib
 Author: firstof9
 Author-email: firstof9@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/firstof9/tplink-ess-lib
 Platform: UNKNOWN
```

