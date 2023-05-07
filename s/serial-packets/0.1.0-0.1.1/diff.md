# Comparing `tmp/serial_packets-0.1.0.tar.gz` & `tmp/serial_packets-0.1.1.tar.gz`

## Comparing `serial_packets-0.1.0.tar` & `serial_packets-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/_packet_decoder.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/_packet_encoder.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17547 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/client.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.0/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.0/LICENSE
--rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 serial_packets-0.1.0/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    14014 2020-02-02 00:00:00.000000 serial_packets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/_interval_tracker.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/_packet_decoder.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/_packet_encoder.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/client.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.1/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.1/LICENSE
+-rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 serial_packets-0.1.1/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    16624 2020-02-02 00:00:00.000000 serial_packets-0.1.1/PKG-INFO
```

### Comparing `serial_packets-0.1.0/src/serial_packets/_packet_decoder.py` & `serial_packets-0.1.1/src/serial_packets/_packet_decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,101 +2,77 @@
 
 import logging
 import asyncio
 from PyCRC.CRCCCITT import CRCCCITT
 from typing import Optional, Callable
 
 from ._packets import PacketType, PACKET_FLAG, PACKET_ESC, MIN_PACKET_LEN, MAX_PACKET_LEN
-from .packets import MAX_DATA_LEN
+from .packets import PacketData, MAX_DATA_LEN
 # from .packets import  PACKET_MAX_LEN
 
 logger = logging.getLogger(__name__)
 
 
-# class DecodedPacket:
-
-#     def __init__(self, cmd_id: int, type: PacketType, endpoint: Optional(int),
-#                  status: Optional(int), data: bytearray):
-#         self.cmd_id = cmd_id
-#         self.type = type
-#         self.endpoint = endpoint
-#         self.status = status
-#         self.data = data
-
-#     def __str__(self):
-#         return f"{self.cmd_id}, {self.endpoint}, {len(self.data)}"
-
-#     def dump(self, title="Decoded packet"):
-#         print(f"{title}", flush=True)
-#         print(f"  Cmd id   {self.cmd_id: 10d}", flush=True)
-#         print(f"  Type   {self.type.name}", flush=True)
-#         print(f"  Endpoint   {self.endpoint}", flush=True)
-#         print(f"  Status   {self.status}", flush=True)
-#         print(f"  Data: {self.data.hex(sep=' ')}", flush=True)
-
-
 class DecodedCommandPacket:
 
-    def __init__(self, cmd_id: int, endpoint: int, data: bytearray):
-        self.cmd_id = cmd_id
-        self.endpoint = endpoint
-        self.data = data
+    def __init__(self, cmd_id: int, endpoint: int, data: PacketData):
+        self.cmd_id: int = cmd_id
+        self.endpoint: int = endpoint
+        self.data: PacketData = data
 
     def __str__(self):
-        return f"Command packet: {self.cmd_id}, {self.endpoint}, {len(self.data)}"
+        return f"Command packet: {self.cmd_id}, {self.endpoint}, {self.data.size()}"
 
 
 class DecodedResponsePacket:
 
-    def __init__(self, cmd_id: int, status: int, data: bytearray):
-        self.cmd_id = cmd_id
-        self.status = status
-        self.data = data
+    def __init__(self, cmd_id: int, status: int, data: PacketData):
+        self.cmd_id: int = cmd_id
+        self.status: int = status
+        self.data: PacketData = data
 
     def __str__(self):
-        return f"Response packet: {self.cmd_id}, {self.endpoint}, {len(self.data)}"
+        return f"Response packet: {self.cmd_id}, {self.status}, {self.data.size()}"
 
 
 class DecodedMessagePacket:
 
-    def __init__(self, endpoint: int, data: bytearray):
-        self.endpoint = endpoint
-        self.data = data
+    def __init__(self, endpoint: int, data: PacketData):
+        self.endpoint: int = endpoint
+        self.data: PacketData = data
 
     def __str__(self):
-        return f"Message packet: {self.endpoint}, {len(self.data)}"
-
+        return f"Message packet: {self.endpoint}, {self.data.size()}"
 
 
 class PacketDecoder:
 
-    def __init__(self, decoded_packet_callback: Callable[[DecodedPacket], None]):
+    def __init__(self, decoded_packet_callback: Callable[
+        [DecodedCommandPacket | DecodedResponsePacket | DecodedMessagePacket], None]):
         assert (decoded_packet_callback is not None)
         self.__crc_calc = CRCCCITT("FFFF")
         self.__packet_bfr = bytearray()
         self.__in_packet = False
         self.__pending_escape = False
-        self.__packet_bfr.clear()
         self.__decoded_packet_callback = decoded_packet_callback
-        # self.__packets_queue = asyncio.Queue()
 
     def __str__(self):
         return f"In_packet ={self.__in_packet}, pending_escape={self.__pending_escape}, len={len(self.__packet_bytes)}"
 
     def __reset_packet(self):
         # self.__state = state
         self.__in_packet = False
         self.__pending_escape = False
         self.__packet_bfr.clear()
 
     # async def get_next_packet(self):
     #     """Blocking asyncio fetch of next pending packet."""
     #     return await self.__packets_queue.get()
 
-    def _receive(self, data: bytes):
+    def receive(self, data: bytes):
         for b in data:
             self.__receive_byte(b)
 
     def __receive_byte(self, b: int):
         # If not already in a packet, wait for next flag.
         if not self.__in_packet:
             if b == PACKET_FLAG:
@@ -169,31 +145,30 @@
             return
 
         # Construct decoded packet
         type_value = rx_bfr[0]
         if type_value == PacketType.COMMAND.value:
             cmd_id = int.from_bytes(rx_bfr[1:5], byteorder='big', signed=False)
             endpoint = rx_bfr[5]
-            data = rx_bfr[6:-2]
-            decoded_packet = DecodedCommandPacket(cmd_id,  endpoint,  data)
+            data = PacketData().add_bytes(rx_bfr[6:-2])
+            decoded_packet = DecodedCommandPacket(cmd_id, endpoint, data)
         elif type_value == PacketType.RESPONSE.value:
             cmd_id = int.from_bytes(rx_bfr[1:5], byteorder='big', signed=False)
             status = rx_bfr[5]
-            data = rx_bfr[6:-2]
-            decoded_packet = DecodedResponsePacket(cmd_id,  status, data)
+            data = PacketData().add_bytes(rx_bfr[6:-2])
+            decoded_packet = DecodedResponsePacket(cmd_id, status, data)
         elif type_value == PacketType.MESSAGE.value:
             endpoint = rx_bfr[1]
-            data = rx_bfr[2:-2]
-            decoded_packet = DecodedMessagePacket(endpoint,  data)
+            data = PacketData().add_bytes(rx_bfr[2:-2])
+            decoded_packet = DecodedMessagePacket(endpoint, data)
         else:
             logger.error("Invalid packet type %02x, dropping packet", type.value)
             return
 
-        if len(data) > MAX_DATA_LEN:
-            logger.error("Packet data too long (type=%d, len=%d), dropping", type_value,
-                         len(data))
+        if data.size() > MAX_DATA_LEN:
+            logger.error("Packet data too long (type=%d, len=%d), dropping", type_value, data.size())
             return
 
         # Inform the user about the new packet.
         self.__decoded_packet_callback(decoded_packet)
 
         # self.__packets_queue.put_nowait(decoded_packet)
```

### Comparing `serial_packets-0.1.0/src/serial_packets/_packet_encoder.py` & `serial_packets-0.1.1/src/serial_packets/_packet_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class PacketEncoder:
 
     def __init__(self):
-        self.__last_packet_time = 0
+        # self.__last_packet_time = 0
         self.__crc_calc = CRCCCITT("FFFF")
 
     def __construct_command_packet(self, cmd_id: int, endpoint: int, data: bytearray):
         """Constructs a command packet, before byte stuffing"""
         packet = bytearray()
         packet.append(PacketType.COMMAND.value)
         packet.extend(cmd_id.to_bytes(4, 'big'))
@@ -46,53 +46,50 @@
         packet.append(endpoint)
         packet.extend(data)
         crc = self.__crc_calc.calculate(bytes(packet))
         packet.extend(crc.to_bytes(2, 'big'))
         assert (len(packet) <= MAX_PACKET_LEN)
         return packet
 
-    def __stuff_packet_bytes(self, packet: bytearray, insert_pre_flag: bool):
+    def __byte_stuffing(self, packet: bytearray, insert_pre_flag: bool):
         """Byte stuff the packet using HDLC format. Also adds packet flag(s)"""
         result = bytearray()
         if insert_pre_flag:
             result.append(PACKET_FLAG)
         for byte in packet:
             if byte == PACKET_FLAG or byte == PACKET_ESC:
                 result.append(PACKET_ESC)
                 result.append(byte ^ 0x20)
             else:
                 result.append(byte)
         result.append(PACKET_FLAG)
         return result
 
-    def __track_packet_interval(self):
-        last_packet_time = self.__last_packet_time
-        self.__last_packet_time = time.time()
-        elapsed = self.__last_packet_time - last_packet_time
-        # We insert a pre packet flag only if the packets are sparse.
-        insert_pre_flag = elapsed > PRE_FLAG_TIMEOUT
-        return insert_pre_flag
+    # def __track_packet_interval(self):
+    #     last_packet_time = self.__last_packet_time
+    #     self.__last_packet_time = time.time()
+    #     elapsed = self.__last_packet_time - last_packet_time
+    #     # We insert a pre packet flag only if the packets are sparse.
+    #     insert_pre_flag = elapsed > PRE_FLAG_TIMEOUT
+    #     return insert_pre_flag
 
-    def encode_command_packet(self, cmd_id: int, endpoint: int, data: bytearray):
+    def encode_command_packet(self, cmd_id: int, endpoint: int, data: bytearray, insert_pre_flag: bool):
         """Returns the command packet in wire format"""
         assert (len(data) <= MAX_DATA_LEN)
-        insert_pre_flag = self.__track_packet_interval()
         packet = self.__construct_command_packet(cmd_id, endpoint, data)
-        stuffed_packet = self.__stuff_packet_bytes(packet, insert_pre_flag)
+        stuffed_packet = self.__byte_stuffing(packet, insert_pre_flag)
         return stuffed_packet
 
-    def encode_response_packet(self, cmd_id: int, status: int, data: bytearray):
+    def encode_response_packet(self, cmd_id: int, status: int, data: bytearray, insert_pre_flag: bool):
         """Returns the packet in wire format."""
         assert (len(data) <= MAX_DATA_LEN)
-        insert_pre_flag = self.__track_packet_interval()
         packet = self.__construct_response_packet(cmd_id, status, data)
-        stuffed_packet = self.__stuff_packet_bytes(packet, insert_pre_flag)
+        stuffed_packet = self.__byte_stuffing(packet, insert_pre_flag)
         return stuffed_packet
       
-    def encode_message_packet(self,  endpoint: int, data: bytearray):
+    def encode_message_packet(self,  endpoint: int, data: bytearray, insert_pre_flag: bool):
         """Returns the message packet in wire format"""
         assert (len(data) <= MAX_DATA_LEN)
-        insert_pre_flag = self.__track_packet_interval()
         packet = self.__construct_message_packet(endpoint, data)
-        stuffed_packet = self.__stuff_packet_bytes(packet, insert_pre_flag)
+        stuffed_packet = self.__byte_stuffing(packet, insert_pre_flag)
         return stuffed_packet
```

### Comparing `serial_packets-0.1.0/src/serial_packets/_packets.py` & `serial_packets-0.1.1/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.0/src/serial_packets/client.py` & `serial_packets-0.1.1/src/serial_packets/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import traceback
 
 from enum import Enum
 from typing import Optional, Tuple, Dict, Callable
 from asyncio.transports import BaseTransport
 from ._packet_encoder import PacketEncoder
 from ._packet_decoder import PacketDecoder, DecodedCommandPacket, DecodedResponsePacket, DecodedMessagePacket
-from ._packets import PacketType, MAX_DATA_LEN, MIN_CMD_TIMEOUT, MAX_CMD_TIMEOUT, DEFAULT_CMD_TIMEOUT, MIN_WORKERS_COUNT, MAX_WORKERS_COUNT, DEFAULT_WORKERS_COUNT
-from .packets import PacketStatus, PacketsEvent, PacketsEventType, PacketsEvent, MAX_USER_ENDPOINT
+from ._packets import PacketType, MAX_DATA_LEN, MIN_CMD_TIMEOUT, MAX_CMD_TIMEOUT, DEFAULT_CMD_TIMEOUT, MIN_WORKERS_COUNT, MAX_WORKERS_COUNT, DEFAULT_WORKERS_COUNT, PRE_FLAG_TIMEOUT
+from ._interval_tracker import IntervalTracker
+from .packets import PacketStatus, PacketsEvent, PacketsEventType, PacketsEvent, PacketData, MAX_USER_ENDPOINT
 
 logger = logging.getLogger(__name__)
 
 # pyserial_asyncio is documented at
 # https://github.com/pyserial/pyserial-asyncio
 
 
@@ -27,15 +28,15 @@
         self.__cmd_id = cmd_id
         self.__future = future
         self.__expiration_time = expiration_time
 
     def __str__(self):
         return f"cmd_context {self.__cmd_id}, {self.__expiration_time - time.time()} sec left"
 
-    def set_result(self, status: int, data: bytearray):
+    def set_command_result(self, status: int, data: PacketData):
         """Transfer the command result to its future."""
         self.__future.set_result((status, data))
 
     def is_expired(self):
         """Tests if the command timeout."""
         return time.time() > self.__expiration_time
 
@@ -59,15 +60,15 @@
 
     def connection_made(self, transport: BaseTransport):
         self.__is_connected = True
         self.__client._post_event(
             PacketsEvent(PacketsEventType.CONNECTED, f"Connected to {self.__port}"))
 
     def data_received(self, data: bytes):
-        self.__packet_decoder._receive(data)
+        self.__packet_decoder.receive(data)
 
     def connection_lost(self, exc):
         self.__is_connected = False
         self.__client._post_event(
             PacketsEvent(PacketsEventType.DISCONNECTED, f"Disconnected from {self.__port}"))
 
     def pause_writing(self):
@@ -78,36 +79,36 @@
         logger.warn("Serial [%s] resumed.", self.__port)
 
 
 class SerialPacketsClient:
 
     def __init__(self,
                  port: str,
-                 command_async_callback: Optional(Callable[[int, bytearray],
-                                                           Tuple(int, bytearray)]) = None,
-                 message_async_callback: Optional(Callable[[int, bytearray], None]) = None,
+                 command_async_callback: Optional(Callable[[int, PacketData],
+                                                           Tuple(int, PacketData)]) = None,
+                 message_async_callback: Optional(Callable[[int, PacketData], None]) = None,
                  event_async_callback: Optional(Callable[[PacketsEvent], None]) = None,
                  baudrate: int = 115200,
                  workers: int = DEFAULT_WORKERS_COUNT):
         """
         Constructs a serial messaging client. 
         
         The constructor doesn't actually open the port. To do that, call connect().
 
         Args:
         * port: A string with dependent serial port to use. E.g. 'COM1'.
             
         * command_async_callback: An optional async callback function to be called on incoming
           command requests. Ignored if None. This is an async function that accepts 
-          an endpoint (int [0-255]) and command data (bytearray, [0 to DATA_MAX_LEN]) and return
-          status (int [0-255]) and response data (bytearray, [0 to DATA_MAX_LEN]).
+          an endpoint (int [0-255]) and command data (PacketData, [0 to DATA_MAX_LEN]) and return
+          status (int [0-255]) and response data (PacketData, [0 to DATA_MAX_LEN]).
           
         * message_async_callback: An optional async callback function to be called on incoming
           messages. Ignored if None. This is an async function that accepts 
-          an endpoint (int [0-255]) and command data (bytearray, [0 to DATA_MAX_LEN]) 
+          an endpoint (int [0-255]) and command data (PacketData, [0 to DATA_MAX_LEN]) 
           and does not return a value.
           
         * event_async_callback: An optional async callback function to be called on
           on certain client events such as port connection and disconnection. 
           Ignored if None. This is an async function that accepts 
           a PacketEvent argument and returns no value.
                 
@@ -128,14 +129,15 @@
         self.__message_async_callback = message_async_callback
         self.__event_async_callback = event_async_callback
         self.__transport = None
         self.__protocol = None
         self.__packet_encoder = PacketEncoder()
         self.__packet_decoder = PacketDecoder(self.__on_decoded_packet)
         self.__command_id_counter = 0
+        self.__interval_tracker = IntervalTracker(PRE_FLAG_TIMEOUT)
         self.__tx_cmd_contexts: Dict[int, _TxCommandContext] = {}
         # Work items types:
         # * PacketsEvent: call user's event handler.
         # * DecodedCommandPacket: handle incoming command packet.
         # * DecodedResponsePacket: handle incoming response packet.
         # * DecodedMessagePacket: handle incoming message packet.
         self.__work_queue = asyncio.Queue()
@@ -202,15 +204,15 @@
         # NOTE: Deleting dict elements inside a dict iteration is not allowed.
         # Using a workaround instead.
         keys = list(self.__tx_cmd_contexts.keys())
         for cmd_id in keys:
             tx_context = self.__tx_cmd_contexts.get(cmd_id)
             if tx_context.is_expired():
                 logger.error("Command [%d] timeout", cmd_id)
-                tx_context.set_result(0xff, bytearray())
+                tx_context.set_command_result(0xff, PacketData())
                 self.__tx_cmd_contexts.pop(cmd_id)
 
     async def __worker_task_loop(self, task_name):
         """Body of the worker tasks to serve incoming packets."""
         # task_name = asyncio.current_task().get_name()
         # print(f"RX task '{task_name}' started", flush=True)
         # logger.debug("RX worker task [%s] started", task_name)
@@ -230,33 +232,33 @@
             logger.error(f"Unknown work item type [%s], dropping", type(work_item))
 
     async def __handle_incoming_command_packet(self, decoded_cmd_packet: DecodedCommandPacket):
         assert (isinstance(decoded_cmd_packet, DecodedCommandPacket))
         if self.__command_async_callback:
             status, data = await self.__command_async_callback(decoded_cmd_packet.endpoint,
                                                                decoded_cmd_packet.data)
-            if len(data) > MAX_DATA_LEN:
-                logger.error("Command response data too long (%d), failing command", len(data))
-                status, data = (PacketStatus.LENGTH_ERROR.value, bytearray())
+            if data.size() > MAX_DATA_LEN:
+                logger.error("Command response data too long (%d), failing command", data.size9)
+                status, data = (PacketStatus.LENGTH_ERROR.value, PacketData())
         else:
-            status, data = (PacketStatus.UNHANDLED.value, bytearray())
+            status, data = (PacketStatus.UNHANDLED.value, PacketData())
         response_packet = self.__packet_encoder.encode_response_packet(
-            decoded_cmd_packet.cmd_id, status, data)
+            decoded_cmd_packet.cmd_id, status, data._internal_bytes_buffer(), self.__interval_tracker.track_packet())
         self.__transport.write(response_packet)
 
     async def __handle_incoming_response_packet(self, decoded_rsp_packet: DecodedResponsePacket):
         # print(f"Handling resp packet ({len(self.__tx_cmd_contexts)} tx contexts)", flush=True)
         assert (isinstance(decoded_rsp_packet, DecodedResponsePacket))
         tx_context: _TxCommandContext = self.__tx_cmd_contexts.pop(decoded_rsp_packet.cmd_id, None)
         if not tx_context:
             logger.error("Response has no matching command [%d], may timeout. Dropping",
                          decoded_rsp_packet.cmd_id)
             # print(f"Response has no matching context {packet.cmd_id}, dropping", flush=True)
             return
-        tx_context.set_result(decoded_rsp_packet.status, decoded_rsp_packet.data)
+        tx_context.set_command_result(decoded_rsp_packet.status, decoded_rsp_packet.data)
 
     async def __handle_incoming_message_packet(self, decoded_msg_packet: DecodedMessagePacket):
         assert (isinstance(decoded_msg_packet, DecodedMessagePacket))
         if self.__message_async_callback:
             await self.__message_async_callback(decoded_msg_packet.endpoint,
                                                 decoded_msg_packet.data)
         else:
@@ -268,100 +270,100 @@
             logger.debug("No event callback, dropping event: %s", packets_event)
         else:
             logger.debug("Callback with event %s", packets_event)
             await self.__event_async_callback(packets_event)
 
     async def send_command_blocking(self,
                                     endpoint: int,
-                                    data: bytearray,
-                                    timeout=DEFAULT_CMD_TIMEOUT) -> Tuple([int, bytearray]):
+                                    data: PacketData,
+                                    timeout=DEFAULT_CMD_TIMEOUT) -> Tuple([int, PacketData]):
         """ Sends a command and wait for result or timeout. This is a convenience
         method that calls send_command_future() and then waits on the future
         for command result.
 
         Args:
         * endpoint: The target endpoint (int [0-MAX_USER_ENDPOINT]) on the receiver side.  
-        * data: The command data (bytearray, [0, DATA_MAX_LEN]).
+        * data: The command data (PacketData, [0, DATA_MAX_LEN]).
         * timeout: Command timeout in secs (float MIN_CMD_TIMEOUT to MAX_CMD_TIMEOUT, default DEFAULT_CMD_TIMEOUT). 
         If a command response is not received within this period, the command
         is aborted with status PacketStatus.TIMEOUT.value and an empty 
-        data bytearray.
+        data PacketData.
         
         Returns:
         * status: The command returned status (int, [0-255]) or PacketStatus.TIMEOUT.value
         in case of a timeout.
-        * data: The command's response data (bytearray [0, DATA_MAX_LEN] or an empty bytearray
+        * data: The command's response data (PacketData [0, DATA_MAX_LEN] or an empty PacketData
         in case of a timeout.
         """
         future = self.send_command_future(endpoint, data, timeout=timeout)
         status, data = await future
         return (status, data)
 
     def send_command_future(self,
                             endpoint: int,
-                            data: bytearray,
-                            timeout=DEFAULT_CMD_TIMEOUT) -> Tuple([int, bytearray]):
+                            data: PacketData,
+                            timeout=DEFAULT_CMD_TIMEOUT) -> Tuple([int, PacketData]):
         """ Sends a command and return immediately without blocking. 
         
         Caller should wait on the returned future to receive the command
         response once available. The command response is a Tuple with 
         two values, the status code (int, [0-255]) and  response data
-        byte returned from the caller (bytearray [0, MAX_DATA_LEN]). Some status
+        byte returned from the caller (PacketData [0, MAX_DATA_LEN]). Some status
         code values are defined by PacketStatus enum.
 
         Args:
         * endpoint: The target endpoint (int [0-255]) on the receiver side.  
-        * data: The command's data (bytearray [0, DATA_MAX_LEN]).
+        * data: The command's data (PacketData [0, DATA_MAX_LEN]).
         * timeout: Command timeout in secs (float MIN_CMD_TIMEOUT to MAX_CMD_TIMEOUT, default DEFAULT_CMD_TIMEOUT). 
         If a command response is not received within this period, the command
         is aborted with status PacketStatus.TIMEOUT.value and an empty 
-        data bytearray.
+        data PacketData.
         
         Returns:
         * A future to wait on for command result. 
         """
         assert (endpoint >= 0 and endpoint <= MAX_USER_ENDPOINT)
-        assert (len(data) <= MAX_DATA_LEN)
+        assert (data.size() <= MAX_DATA_LEN)
         assert (timeout >= MIN_CMD_TIMEOUT and timeout <= MAX_CMD_TIMEOUT)
         if not self.is_connected():
             logger.error("Client not connected when trying to send a message")
             future = asyncio.Future()
-            future.set_result((PacketStatus.NOT_CONNECTED.value, bytearray()))
+            future.set_result((PacketStatus.NOT_CONNECTED.value, PacketData()))
             return future
         # Allocate a 32 bit fresh command id. Wrap around are ok since
         # commands are short living.
         self.__command_id_counter = (self.__command_id_counter + 1) & 0xffffffff
         cmd_id = self.__command_id_counter
         assert (not cmd_id in self.__tx_cmd_contexts)
         # Encode packet bytes
-        packet = self.__packet_encoder.encode_command_packet(cmd_id, endpoint, data)
+        packet = self.__packet_encoder.encode_command_packet(cmd_id, endpoint, data._internal_bytes_buffer(), self.__interval_tracker.track_packet())
         logger.debug("TX command packet [%d]: %s", endpoint, packet.hex(sep=' '))
         # Create command tx context
         expiration_time = time.time() + timeout
         future = asyncio.Future()
         tx_cmd_context = _TxCommandContext(cmd_id, expiration_time, future)
         self.__tx_cmd_contexts[cmd_id] = tx_cmd_context
         # Start sending
         self.__transport.write(packet)
         # Future will be signaled on response or timeout.
         return future
 
-    def send_message(self, endpoint: int, data: bytearray) -> None:
+    def send_message(self, endpoint: int, data: PacketData) -> None:
         """ Sends a message. Returns immediately, before sending completed. 
 
             Args:
             * endpoint: The target endpoint (int [0-255]) on the receiver side.  
-            * data: The message's data (bytearray [0, DATA_MAX_LEN]).
+            * data: The message's data (PacketData [0, DATA_MAX_LEN]).
             
             Returns:
             * None.
             """
         assert (endpoint >= 0 and endpoint <= MAX_USER_ENDPOINT)
-        assert (len(data) <= MAX_DATA_LEN)
+        assert (data.size() <= MAX_DATA_LEN)
         if not self.is_connected():
             logger.warn("Client not connected, ignoring message send")
             return
         # Encode packet bytes
-        packet = self.__packet_encoder.encode_message_packet(endpoint, data)
+        packet = self.__packet_encoder.encode_message_packet(endpoint, data._internal_bytes_buffer(), self.__interval_tracker.track_packet())
         logger.debug("TX message packet [%d]: %s", endpoint, packet.hex(sep=' '))
         # Start sending
         self.__transport.write(packet)
```

### Comparing `serial_packets-0.1.0/LICENSE` & `serial_packets-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.0/README.md` & `serial_packets-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # Python Serial Packets
 
 Python implementations of the Serial Packets protocol.
 
-AS OF MAY 2023, THIS IS WORK IN PROGRESS, NOT READY YET FOR PUBLIC RELEASE.
-
 * PYPI: <https://pypi.org/project/serial-packets/>
 * Github: <https://github.com/zapta/serial_packets_py>
 
+Related works:
+
+* Simple HDLC: <https://github.com/wuttem/simple-hdlc>
+* ArduHDLC: <https://github.com/jarkko-hautakorpi/Arduhdlc>
+* Firmata: <https://github.com/firmata/arduino>
+
 ## Protocol Description
 
-The Serial Packets protocol provides packet based point-to-point serial transport for communication between devices. For example, it can be used for communication between an Arduino device and a PC, where the PC controls the device and the device sends data in real time back to the PC. The protocol is symmetrical and both sides to the communication   have the same capabilities with no designation of master/slave at the transport level.
+The Serial Packets protocol provides packet based point-to-point serial transport for communication between devices. For example, it can be used to connect an Arduino device to a PC, where the PC controls the device, and the device sends data in real time back to the PC. The protocol is fully symmetrical such that both sides to the communication have the same capabilities, with no designation of master/slave at the transport level.
 
 ### Highlights
 
-* Protocol is packet oriented, saving the need to implement framing in the application.
-* The protocol is Efficient with low per-packet overhead, and requires minimal computation and memory.
+* Protocol is packet oriented, saving the need to implement framing by the application.
+* The protocol is efficient with low per-packet overhead, and minimal memory and computation requirements.
 * The protocol is symmetrical, and both sides can initiate or response to interactions.
 * The protocol is full duplex, and works independently on each direction.
 * The protocol support endpoint addressing to simplify routing of messages within the application.
 * The protocol supports both one way and two way request/response interactions.
 * Each packet is verified with a 16 bits CRC.
-* The protocol uses the HDLC byte stuffing algorithm which allow to resync on next frame despite communication errors.
+* The protocol uses the HDLC byte stuffing algorithm which allow to resync on next frame despite line errors.
 * The wire representation is intuitive which simplifies debugging.
-* The protocol is connectionless and stateless, though application can implement the notion of connection and state at their layer..
+* The protocol is connectionless and stateless, though application can implement the notion of connection and state at their layer.
+
 
 ### Commands
 
-Commands are round-trip interactions where one node send a 'command' packet and the other node sends back 'response' packet that references the original command packet. Commands are useful to control a device and to retrieve information by polling the device using a RPC like
-API.
+Commands are round-trip interactions where one node send a 'command' packet receives as 'response' packet from the other node. Commands can be used for example the device and to retrieve information selected
+information.
 
-The following tables lists the fields of command request and response  packets, before converting to wire representation as explained later:
+The following tables lists the fields of command request and response  packets respectively. Note that this is not the exact wire representation since the packets are subject to flagging and byte stuffing as explained later.
 
 #### Command packet
 
 | Field     | Size [bytes] | Source   | Description                                            |
 | :-------- | :----------- | :------- | :----------------------------------------------------- |
 | PACKET_TYPE      | 1            | Auto     | The value 0x01                                         |
 | CMD_ID    | 4            | Auto     | A unique command id for response matching. Big Endian. |
@@ -59,52 +64,59 @@
 Future base command sending:
 
 ```python
 client = SerialPacketsClient("COM1", my_command_async_callback, my_message_async_callback,  my_event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 
-cmd_endpoint = 20
-cmd_data = bytearray([0x01, 0x02, 0x03])
-future =  client.send_command_future(cmd_endpoint, cmd_data, timeout=0.2)
+endpoint = 20
+cmd_data = PacketData()
+cmd_data.add_uint8(0x01)
+cmd_data.add_uint16(0x0203)
+future =  client.send_command_future(endpoint, cmd_data, timeout=0.2)
 
 # Sometime later
-status, data = await future
+status, rsp_data = await future
 ```
 
 Blocking style command sending:
 
 ```python
 client = SerialPacketsClient("COM1", my_command_async_callback, my_message_async_callback, my_event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 
-cmd_endpoint = 20
-cmd_data = bytearray([0x01, 0x02, 0x03])
-rx_status, rx_data = await client.send_command_blocking(cmd_endpoint, cmd_data, timeout=0.2)
+endpoint = 20
+cmd_data = PacketData()
+cmd_data.add_uint8(0x01)
+cmd_data.add_uint16(0x0203)
+rx_status, rx_data = await client.send_command_blocking(endpoint, cmd_data, timeout=0.2)
 ```
 
 #### Receiving a command
 
-Incoming commands are received via a callback function that is passed to the SerialPacketsClient when it's created. The callback is an async function that receives the target endpoint and the data of the command and returns the status and data of the response. The client maintains a pool of asyncio workers tasks that serves incoming packets such it's processing one command doesn't block reception of new commands,and command execution can be performed in parallel. If the command is not handled, the callback function should return an empty response with the status UNHANDLED.value.
+Incoming commands are received via an optional callback function that is passed to the SerialPacketsClient when it's created. The callback is an async function that receives the command's endpoint and data,  and returns the response's status and data. The client uses a pool of asyncio worker tasks that serves incoming packets, and therefore it's ok
+for the command handler to perform asyncio await operations as part of serving the command. If the command is not handled, the callback function should return the status UNHANDLED.value and empty data.
 
 ```python
-async def my_command_async_callback(endpoint: int, data: bytearray) -> Tuple[int, bytearray]:
-    logger.info(f"Received command: [%d] %s", endpoint, data.hex(sep=' '))
+async def command_async_callback(endpoint: int, data: PacketData) -> Tuple[int, PacketData]:
+    logger.info(f"Received command: [%d] %s", endpoint, data.hex_bytes())
     if (endpoint == 20):
-        return handle_command_endpoint_20(data)
-    # Add here handling of other end points.
+        v1 = data.read_uint8()
+        v2 = data.read_uint16()
+        if not data.all_read_ok():
+          logger.info(f"Errors parsing command", status, response_data.hex(sep=' '))
+          return (PacketStatus.INVALID_ARGUMENT.value, PacketData())
+        response_data = PacketData()
+        response_dat.add_uint32(0x12345678)
+        logger.info(f"Command response: [%d] %s", PacketStatus.OK.value, response_data.hex(sep=' '))
+    # Add here handling of additional command end points.
     return (PacketStatus.UNHANDLED.value, bytearray())
 
-def handle_command_endpoint_20(data: bytearray) -> Tuple[int, bytearray]:
-    status, response_data = (PacketStatus.OK.value, bytearray([1, 2, 3, 4]))
-    logger.info(f"Command response: [%d] %s", status, response_data.hex(sep=' '))
-    return (status, response_data)
-
-client = SerialPacketsClient(args.port, my_command_async_callback, my)message_async_callback, my_event_async_callback)
+client = SerialPacketsClient(args.port, command_async_callback, message_async_callback, event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 ```
 
 ### Messages
 
 Messages are a simpler case of a commands with no response. They are useful for periodic notifications, for example for data reporting, and have lower overhead than commands.
@@ -120,46 +132,54 @@
 
 #### Sending a message
 
 The *SerialPacketsClient* class provides a method for sending a command. The method is non blocking and merely queues the message for sending.
 two methods for sending commands.
 
 ```python
-client = SerialPacketsClient("COM1", my_command_async_callback my_event_async_callback)
+client = SerialPacketsClient("COM1", command_async_callback, message_async_callback, event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 ...
-msg_endpoint = 20
-msg_data = bytearray([0x01, 0x02, 0x03])
-client.send_message(msg_endpoint, msg_data)
+endpoint = 20
+data = PacketData()
+data.add_uint16(12345)
+client.send_message(endpoint, data)
 ```
 
 #### Receiving a message
 
 Incoming messages are received via a callback function that is passed to the SerialPacketsClient when it's created. The callback is an async function that receives the target endpoint and the data of the message and returns no value.
 
 ```python
-async def my_message_async_callback(endpoint: int, data: bytearray) -> Tuple[int, bytearray]:
+async def message_async_callback(endpoint: int, data: bytearray) -> Tuple[int, PacketData]:
     logger.info(f"Received message: [%d] %s", endpoint, data.hex(sep=' '))
+    if endpoint == 20:
+        v1 = data.read_uint16()
+        v2 = data.read_uint16()
+        if v1.read_all_ok():
+          logger.info(f"Message data: {v1} {v2}")
+    else:
+      logger.error(f"Unhandled message at endpoint {endpoint}")
 
 client = SerialPacketsClient(args.port, my_command_async_callback, my_message_async_callback, my_event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 ```
 
 ## Events
 
 The SerialPacketsClient signals the application about certain events via an events callback that the use pass to it upon initialization.
 
 ```python
-async def my_event_async_callback(event: PacketsEvent) -> None:
+async def event_async_callback(event: PacketsEvent) -> None:
     logger.info("Event %s: %s", event.event_type(), event.description())
     logger.info("%s event", event)
 
-client = SerialPacketsClient(args.port, my_command_async_callback, my_message_async_callback, my_event_async_callback)
+client = SerialPacketsClient(args.port, command_async_callback, message_async_callback, event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 ```
 
 ```python
 ```
 
@@ -167,14 +187,62 @@
 
 ```python
 class PacketsEventType(Enum):
     CONNECTED = 1
     DISCONNECTED = 2
 ```
 
+## PacketData class
+
+Packet data is represented by instances of the class PacketData which also provides a simple serialization/deserialization API.
+
+Serialization methods:
+
+```python
+add_uint8(v)   # Adds a single byte unsigned integer value
+add_uint16(v)  # Adds a two byte unsigned integer value
+add_uint32(v)  # Adds a four byte unsigned integer value
+add_bytes(v)   # Adds an arbitrary number of bytes
+
+```
+
+> ***NOTE:***  Variable length string and data can be encoded as a byte count followed by the byte themselves. .
+
+Deserialization methods:
+
+```python
+v = read_uint8()    # Read a single byte unsigned integer value
+v = read_uint16(v)  # Read a two byte unsigned integer value
+v = read_uint32(v)  # Read a four byte unsigned integer value
+v = read_bytes(v)   # Read an arbitrary number of bytes
+```
+
+> ***NOTE:***  If any of the read methods encounter an error, it returns None and sets the internal read error flag of the PacketData, which
+will force all future read methods to fail as well..
+
+Deserialization control methods:
+
+```python
+bytes_read() -> int            # Returns number of bytes returned so far.
+bytes_left_to_read() -> int    # Returns the count of data bytes that have not been read yet.
+read_error() -> int            # Tests if read errors where encountered so far.
+all_read() -> bool             # Tests if all data were read.     
+all_read_ok() -> bool          # Tests if all data read with no errors.
+reset_read_location() -> None  # Resets read pointer and error flag.
+```
+
+Utility methods:
+
+```python
+hex_str() -> str    # Returns an hex representation fo the data, for debugging.
+data_bytes() -> bytearray  # Returns a copy of the data bytes.
+size() -> int  # Returns the number of data bytes.
+clear() -> None # Clear the data and reset the read location and error flag..
+```
+
 ## Wire representation
 
 ### Packet flag byte
 
 The Serial Packets protocol uses packet flags similar to the HDLC protocol, with the special flag byte 0x7E inserted in the serial stream to mark packet ends. A flag byte is always inserted immediately after the
 last byte of each packet, and also optionally just before the first byte of packets, if the interval from the previous packet was longer than a certain time period.
 
@@ -184,14 +252,37 @@
 
 | Packet byte | Wire bytes | Comments            |
 | :---------- | :--------- | :------------------ |
 | 0x7E        | 0x7D, 0x5E | Escaped flag byte   |
 | 0x7D        | 0x7D, 0x5D | Escaped escape byte |
 | Other bytes | No change  | The common case     |
 
+Example of a command packet:
+
+```python
+
+Stuffed command packet:
+0x7e, 0x01, 0xff, 0x12, 0x34, 0x56, 0x20, 0xff, 
+0x00, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99, 0x09,
+0x8c, 0x7e
+
+Breakdown into parts:
+flag:         0x7e
+packet_type:  0x01
+cmd_id:       0xff, 0x12, 0x34, 0x56
+endpoint:     0x20
+data:         0xff, 0x00, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99
+crc:          0x09, 0x8c
+flag:         0x7e
+
+# In this examples, only the data part contains escaped bytes and its
+# unescaped version is:
+data:   0xff, 0x00, 0x7e, 0x22, 0x7d, 0x99
+```
+
 ## Status codes
 
 The Serial Packets protocol uses 1 byte status codes where 0x00 indicates success and all other values indicate errors. These status codes are used in the command responses, and optionally also by the implementation API for other reasons.
 
 As of May 2023, these are the predefined status codes. For the updated list, look at the *serial_packets.packets.PacketStatus* enum.
 
 | Status Value | Status name      | Comments                             |
@@ -260,16 +351,10 @@
 
 **Q**: Why asyncio based implementation, doesn't it complicate things?
 
 A: Asyncio may make simple programs more complicated but it allows for more responsive programs with efficient parallel I/O.
 
 ---
 
-**Q**: Do you plan to provide also cross platform APIs for data serialization/deserialization?
-
-A: This is a good idea, but we are not working on it as of May 2023. We would any recommendations or implementations of such a portable API.
-
----
-
 **Q**: Is there a serial sniffer for the Serial Packets protocol?
 
 A: Note at the moment, but if you will implement one, we would love to a reference it here. It can be implemented for example with a Python program or with an Arduino sketch.
```

### Comparing `serial_packets-0.1.0/pyproject.toml` & `serial_packets-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.1.0/PKG-INFO` & `serial_packets-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
@@ -14,42 +14,47 @@
 Requires-Dist: pythoncrc>=1.21.0
 Description-Content-Type: text/markdown
 
 # Python Serial Packets
 
 Python implementations of the Serial Packets protocol.
 
-AS OF MAY 2023, THIS IS WORK IN PROGRESS, NOT READY YET FOR PUBLIC RELEASE.
-
 * PYPI: <https://pypi.org/project/serial-packets/>
 * Github: <https://github.com/zapta/serial_packets_py>
 
+Related works:
+
+* Simple HDLC: <https://github.com/wuttem/simple-hdlc>
+* ArduHDLC: <https://github.com/jarkko-hautakorpi/Arduhdlc>
+* Firmata: <https://github.com/firmata/arduino>
+
 ## Protocol Description
 
-The Serial Packets protocol provides packet based point-to-point serial transport for communication between devices. For example, it can be used for communication between an Arduino device and a PC, where the PC controls the device and the device sends data in real time back to the PC. The protocol is symmetrical and both sides to the communication   have the same capabilities with no designation of master/slave at the transport level.
+The Serial Packets protocol provides packet based point-to-point serial transport for communication between devices. For example, it can be used to connect an Arduino device to a PC, where the PC controls the device, and the device sends data in real time back to the PC. The protocol is fully symmetrical such that both sides to the communication have the same capabilities, with no designation of master/slave at the transport level.
 
 ### Highlights
 
-* Protocol is packet oriented, saving the need to implement framing in the application.
-* The protocol is Efficient with low per-packet overhead, and requires minimal computation and memory.
+* Protocol is packet oriented, saving the need to implement framing by the application.
+* The protocol is efficient with low per-packet overhead, and minimal memory and computation requirements.
 * The protocol is symmetrical, and both sides can initiate or response to interactions.
 * The protocol is full duplex, and works independently on each direction.
 * The protocol support endpoint addressing to simplify routing of messages within the application.
 * The protocol supports both one way and two way request/response interactions.
 * Each packet is verified with a 16 bits CRC.
-* The protocol uses the HDLC byte stuffing algorithm which allow to resync on next frame despite communication errors.
+* The protocol uses the HDLC byte stuffing algorithm which allow to resync on next frame despite line errors.
 * The wire representation is intuitive which simplifies debugging.
-* The protocol is connectionless and stateless, though application can implement the notion of connection and state at their layer..
+* The protocol is connectionless and stateless, though application can implement the notion of connection and state at their layer.
+
 
 ### Commands
 
-Commands are round-trip interactions where one node send a 'command' packet and the other node sends back 'response' packet that references the original command packet. Commands are useful to control a device and to retrieve information by polling the device using a RPC like
-API.
+Commands are round-trip interactions where one node send a 'command' packet receives as 'response' packet from the other node. Commands can be used for example the device and to retrieve information selected
+information.
 
-The following tables lists the fields of command request and response  packets, before converting to wire representation as explained later:
+The following tables lists the fields of command request and response  packets respectively. Note that this is not the exact wire representation since the packets are subject to flagging and byte stuffing as explained later.
 
 #### Command packet
 
 | Field     | Size [bytes] | Source   | Description                                            |
 | :-------- | :----------- | :------- | :----------------------------------------------------- |
 | PACKET_TYPE      | 1            | Auto     | The value 0x01                                         |
 | CMD_ID    | 4            | Auto     | A unique command id for response matching. Big Endian. |
@@ -75,52 +80,59 @@
 Future base command sending:
 
 ```python
 client = SerialPacketsClient("COM1", my_command_async_callback, my_message_async_callback,  my_event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 
-cmd_endpoint = 20
-cmd_data = bytearray([0x01, 0x02, 0x03])
-future =  client.send_command_future(cmd_endpoint, cmd_data, timeout=0.2)
+endpoint = 20
+cmd_data = PacketData()
+cmd_data.add_uint8(0x01)
+cmd_data.add_uint16(0x0203)
+future =  client.send_command_future(endpoint, cmd_data, timeout=0.2)
 
 # Sometime later
-status, data = await future
+status, rsp_data = await future
 ```
 
 Blocking style command sending:
 
 ```python
 client = SerialPacketsClient("COM1", my_command_async_callback, my_message_async_callback, my_event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 
-cmd_endpoint = 20
-cmd_data = bytearray([0x01, 0x02, 0x03])
-rx_status, rx_data = await client.send_command_blocking(cmd_endpoint, cmd_data, timeout=0.2)
+endpoint = 20
+cmd_data = PacketData()
+cmd_data.add_uint8(0x01)
+cmd_data.add_uint16(0x0203)
+rx_status, rx_data = await client.send_command_blocking(endpoint, cmd_data, timeout=0.2)
 ```
 
 #### Receiving a command
 
-Incoming commands are received via a callback function that is passed to the SerialPacketsClient when it's created. The callback is an async function that receives the target endpoint and the data of the command and returns the status and data of the response. The client maintains a pool of asyncio workers tasks that serves incoming packets such it's processing one command doesn't block reception of new commands,and command execution can be performed in parallel. If the command is not handled, the callback function should return an empty response with the status UNHANDLED.value.
+Incoming commands are received via an optional callback function that is passed to the SerialPacketsClient when it's created. The callback is an async function that receives the command's endpoint and data,  and returns the response's status and data. The client uses a pool of asyncio worker tasks that serves incoming packets, and therefore it's ok
+for the command handler to perform asyncio await operations as part of serving the command. If the command is not handled, the callback function should return the status UNHANDLED.value and empty data.
 
 ```python
-async def my_command_async_callback(endpoint: int, data: bytearray) -> Tuple[int, bytearray]:
-    logger.info(f"Received command: [%d] %s", endpoint, data.hex(sep=' '))
+async def command_async_callback(endpoint: int, data: PacketData) -> Tuple[int, PacketData]:
+    logger.info(f"Received command: [%d] %s", endpoint, data.hex_bytes())
     if (endpoint == 20):
-        return handle_command_endpoint_20(data)
-    # Add here handling of other end points.
+        v1 = data.read_uint8()
+        v2 = data.read_uint16()
+        if not data.all_read_ok():
+          logger.info(f"Errors parsing command", status, response_data.hex(sep=' '))
+          return (PacketStatus.INVALID_ARGUMENT.value, PacketData())
+        response_data = PacketData()
+        response_dat.add_uint32(0x12345678)
+        logger.info(f"Command response: [%d] %s", PacketStatus.OK.value, response_data.hex(sep=' '))
+    # Add here handling of additional command end points.
     return (PacketStatus.UNHANDLED.value, bytearray())
 
-def handle_command_endpoint_20(data: bytearray) -> Tuple[int, bytearray]:
-    status, response_data = (PacketStatus.OK.value, bytearray([1, 2, 3, 4]))
-    logger.info(f"Command response: [%d] %s", status, response_data.hex(sep=' '))
-    return (status, response_data)
-
-client = SerialPacketsClient(args.port, my_command_async_callback, my)message_async_callback, my_event_async_callback)
+client = SerialPacketsClient(args.port, command_async_callback, message_async_callback, event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 ```
 
 ### Messages
 
 Messages are a simpler case of a commands with no response. They are useful for periodic notifications, for example for data reporting, and have lower overhead than commands.
@@ -136,46 +148,54 @@
 
 #### Sending a message
 
 The *SerialPacketsClient* class provides a method for sending a command. The method is non blocking and merely queues the message for sending.
 two methods for sending commands.
 
 ```python
-client = SerialPacketsClient("COM1", my_command_async_callback my_event_async_callback)
+client = SerialPacketsClient("COM1", command_async_callback, message_async_callback, event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 ...
-msg_endpoint = 20
-msg_data = bytearray([0x01, 0x02, 0x03])
-client.send_message(msg_endpoint, msg_data)
+endpoint = 20
+data = PacketData()
+data.add_uint16(12345)
+client.send_message(endpoint, data)
 ```
 
 #### Receiving a message
 
 Incoming messages are received via a callback function that is passed to the SerialPacketsClient when it's created. The callback is an async function that receives the target endpoint and the data of the message and returns no value.
 
 ```python
-async def my_message_async_callback(endpoint: int, data: bytearray) -> Tuple[int, bytearray]:
+async def message_async_callback(endpoint: int, data: bytearray) -> Tuple[int, PacketData]:
     logger.info(f"Received message: [%d] %s", endpoint, data.hex(sep=' '))
+    if endpoint == 20:
+        v1 = data.read_uint16()
+        v2 = data.read_uint16()
+        if v1.read_all_ok():
+          logger.info(f"Message data: {v1} {v2}")
+    else:
+      logger.error(f"Unhandled message at endpoint {endpoint}")
 
 client = SerialPacketsClient(args.port, my_command_async_callback, my_message_async_callback, my_event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 ```
 
 ## Events
 
 The SerialPacketsClient signals the application about certain events via an events callback that the use pass to it upon initialization.
 
 ```python
-async def my_event_async_callback(event: PacketsEvent) -> None:
+async def event_async_callback(event: PacketsEvent) -> None:
     logger.info("Event %s: %s", event.event_type(), event.description())
     logger.info("%s event", event)
 
-client = SerialPacketsClient(args.port, my_command_async_callback, my_message_async_callback, my_event_async_callback)
+client = SerialPacketsClient(args.port, command_async_callback, message_async_callback, event_async_callback)
 is_connected = await client.connect()
 assert(is_connected)
 ```
 
 ```python
 ```
 
@@ -183,14 +203,62 @@
 
 ```python
 class PacketsEventType(Enum):
     CONNECTED = 1
     DISCONNECTED = 2
 ```
 
+## PacketData class
+
+Packet data is represented by instances of the class PacketData which also provides a simple serialization/deserialization API.
+
+Serialization methods:
+
+```python
+add_uint8(v)   # Adds a single byte unsigned integer value
+add_uint16(v)  # Adds a two byte unsigned integer value
+add_uint32(v)  # Adds a four byte unsigned integer value
+add_bytes(v)   # Adds an arbitrary number of bytes
+
+```
+
+> ***NOTE:***  Variable length string and data can be encoded as a byte count followed by the byte themselves. .
+
+Deserialization methods:
+
+```python
+v = read_uint8()    # Read a single byte unsigned integer value
+v = read_uint16(v)  # Read a two byte unsigned integer value
+v = read_uint32(v)  # Read a four byte unsigned integer value
+v = read_bytes(v)   # Read an arbitrary number of bytes
+```
+
+> ***NOTE:***  If any of the read methods encounter an error, it returns None and sets the internal read error flag of the PacketData, which
+will force all future read methods to fail as well..
+
+Deserialization control methods:
+
+```python
+bytes_read() -> int            # Returns number of bytes returned so far.
+bytes_left_to_read() -> int    # Returns the count of data bytes that have not been read yet.
+read_error() -> int            # Tests if read errors where encountered so far.
+all_read() -> bool             # Tests if all data were read.     
+all_read_ok() -> bool          # Tests if all data read with no errors.
+reset_read_location() -> None  # Resets read pointer and error flag.
+```
+
+Utility methods:
+
+```python
+hex_str() -> str    # Returns an hex representation fo the data, for debugging.
+data_bytes() -> bytearray  # Returns a copy of the data bytes.
+size() -> int  # Returns the number of data bytes.
+clear() -> None # Clear the data and reset the read location and error flag..
+```
+
 ## Wire representation
 
 ### Packet flag byte
 
 The Serial Packets protocol uses packet flags similar to the HDLC protocol, with the special flag byte 0x7E inserted in the serial stream to mark packet ends. A flag byte is always inserted immediately after the
 last byte of each packet, and also optionally just before the first byte of packets, if the interval from the previous packet was longer than a certain time period.
 
@@ -200,14 +268,37 @@
 
 | Packet byte | Wire bytes | Comments            |
 | :---------- | :--------- | :------------------ |
 | 0x7E        | 0x7D, 0x5E | Escaped flag byte   |
 | 0x7D        | 0x7D, 0x5D | Escaped escape byte |
 | Other bytes | No change  | The common case     |
 
+Example of a command packet:
+
+```python
+
+Stuffed command packet:
+0x7e, 0x01, 0xff, 0x12, 0x34, 0x56, 0x20, 0xff, 
+0x00, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99, 0x09,
+0x8c, 0x7e
+
+Breakdown into parts:
+flag:         0x7e
+packet_type:  0x01
+cmd_id:       0xff, 0x12, 0x34, 0x56
+endpoint:     0x20
+data:         0xff, 0x00, 0x7d, 0x5e, 0x22, 0x7d, 0x5d, 0x99
+crc:          0x09, 0x8c
+flag:         0x7e
+
+# In this examples, only the data part contains escaped bytes and its
+# unescaped version is:
+data:   0xff, 0x00, 0x7e, 0x22, 0x7d, 0x99
+```
+
 ## Status codes
 
 The Serial Packets protocol uses 1 byte status codes where 0x00 indicates success and all other values indicate errors. These status codes are used in the command responses, and optionally also by the implementation API for other reasons.
 
 As of May 2023, these are the predefined status codes. For the updated list, look at the *serial_packets.packets.PacketStatus* enum.
 
 | Status Value | Status name      | Comments                             |
@@ -276,16 +367,10 @@
 
 **Q**: Why asyncio based implementation, doesn't it complicate things?
 
 A: Asyncio may make simple programs more complicated but it allows for more responsive programs with efficient parallel I/O.
 
 ---
 
-**Q**: Do you plan to provide also cross platform APIs for data serialization/deserialization?
-
-A: This is a good idea, but we are not working on it as of May 2023. We would any recommendations or implementations of such a portable API.
-
----
-
 **Q**: Is there a serial sniffer for the Serial Packets protocol?
 
 A: Note at the moment, but if you will implement one, we would love to a reference it here. It can be implemented for example with a Python program or with an Arduino sketch.
```

