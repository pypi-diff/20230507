# Comparing `tmp/jsonrpcx-4.0.0-py3-none-any.whl.zip` & `tmp/jsonrpcx-4.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15161 bytes, number of entries: 6
--rw-r--r--  2.0 unx    32630 b- defN 23-May-02 18:21 jsonrpcx/__init__.py
--rw-r--r--  2.0 unx     1023 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/LICENCE
--rw-r--r--  2.0 unx    15210 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      469 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/RECORD
-6 files, 49433 bytes uncompressed, 14315 bytes compressed:  71.0%
+Zip file size: 16014 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    35720 b- defN 23-May-07 08:01 jsonrpcx/__init__.py
+-rw-r--r--  2.0 unx     1023 b- defN 23-May-07 08:05 jsonrpcx-4.1.0.dist-info/LICENCE
+-rw-r--r--  2.0 unx    16061 b- defN 23-May-07 08:05 jsonrpcx-4.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 08:05 jsonrpcx-4.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-07 08:05 jsonrpcx-4.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      469 b- defN 23-May-07 08:05 jsonrpcx-4.1.0.dist-info/RECORD
+6 files, 53374 bytes uncompressed, 15168 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jsonrpcx/__init__.py
 Comment: 
 
-Filename: jsonrpcx-4.0.0.dist-info/LICENCE
+Filename: jsonrpcx-4.1.0.dist-info/LICENCE
 Comment: 
 
-Filename: jsonrpcx-4.0.0.dist-info/METADATA
+Filename: jsonrpcx-4.1.0.dist-info/METADATA
 Comment: 
 
-Filename: jsonrpcx-4.0.0.dist-info/WHEEL
+Filename: jsonrpcx-4.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: jsonrpcx-4.0.0.dist-info/top_level.txt
+Filename: jsonrpcx-4.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jsonrpcx-4.0.0.dist-info/RECORD
+Filename: jsonrpcx-4.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonrpcx/__init__.py

```diff
@@ -7,14 +7,26 @@
 import io
 import logging
 import inspect
 from pytz import utc as tz_utc
 from tzlocal import get_localzone as tz_getlocal
 from functools import reduce
 import asyncio
+import uuid
+try:
+    from asyncio_mqtt import Client
+except ImportError:
+    pass
+
+
+logging.basicConfig(level=logging.DEBUG)
+
+
+logging.basicConfig(level=logging.DEBUG)
+
 
 PARSE_ERROR = -32700
 INVALID_REQUEST = -32600
 METHOD_NOT_FOUND = -32601
 INVALID_PARAMS = -32602
 INTERNAL_ERROR = -32603
 REQUEST_CANCELLED = -32800 # as defined by Microsoft Language Server Protocol
@@ -882,7 +894,68 @@
         # RPC Result is None if the response is a stream the response will already have been sent in that caase
         if rpcResult is not None:
             await send({
                 'type': 'http.response.body',
                 'body': rpcResult.stringify().encode("utf-8")
             })
 
+
+class MqttJSONRPCServerDelegate(CommonDelegate):
+    pass
+
+class MqttJSONRPCServer(CommonAsyncServer):
+    def __init__(self, host: str, user: str, password: str, topic: str, port: int = 1883, delegate=None):
+        self.log = logging.getLogger("MqttJSONServer")
+        if not delegate:
+            self.delegate = MqttJSONRPCServerDelegate()
+
+        self._mqttHost = host
+        self._mqttPort = port
+        self._mqttUser = user
+        self._mqttPassword = password
+        self._mqttTopic = topic
+
+    async def processRequests(self):
+        async with Client(self._mqttHost, self._mqttPort, username=self._mqttUser, password=self._mqttPassword) as client:
+            async with client.filtered_messages(self._mqttTopic) as messages:
+                await client.subscribe(self._mqttTopic)
+                async for message in messages:
+                    try:
+                        rawRequest = message.payload.decode()
+                        request = json.loads(rawRequest)
+                        if not "method" in request.keys():
+                            # Don't process our own response
+                            continue
+                        response = await self._async_processRequest(rawRequest)
+                        payload = response.stringify()
+                        print(payload)
+                        await client.publish(self._mqttTopic, payload=payload, qos=0, retain=False)
+                    except Exception as ex:
+                        logging.exception(ex)
+
+
+async def mqttRPCCall(method: str, params: Union[Dict, List], *, id: Optional[str]=None, mqttHost: str, mqttUser: str, mqttPassword: str, mqttTopic: str, mqttPort: int = 1883):
+    if not id:
+        id = str(uuid.uuid4())
+    request = Request(method, params)
+    requestMessage = Message()    
+    requestMessage.request = request
+    requestMessage.id = id
+
+    async with Client(mqttHost, mqttPort, username=mqttUser, password=mqttPassword) as client:
+        payload = requestMessage.stringify()
+        logging.debug(f"Sending {payload=}")
+        await client.publish(mqttTopic, payload=payload, qos=0, retain=False)
+        async with client.filtered_messages(mqttTopic) as messages:
+            await client.subscribe(mqttTopic)
+            async for message in messages:
+                try:
+                    data = message.payload.decode()
+                    potentialResponseMessage = Message()
+                    potentialResponseMessage.parse(data)
+                    if potentialResponseMessage.isResponse() and potentialResponseMessage.id == requestMessage.id:
+                        res = potentialResponseMessage.response
+                        if res.indicatesSuccess:
+                            return res.result
+                        raise Exception(f"MQTT JSON-RPC 2.0 Error {res.error=}")
+                except Exception as ex:
+                    logging.exception(ex)
```

## Comparing `jsonrpcx-4.0.0.dist-info/LICENCE` & `jsonrpcx-4.1.0.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `jsonrpcx-4.0.0.dist-info/METADATA` & `jsonrpcx-4.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpcx
-Version: 4.0.0
+Version: 4.1.0
 Summary: A battle tested Python JSON-RPC2.0 library supporting client and server code in sync and async fashion.
 Home-page: https://codeberg.org/_laphilipa/jsonrpcx
 License: ISC
 Keywords: JSON,jsonrpc,rpc
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
@@ -29,15 +29,16 @@
 
 # Overview
 
 A JSON-RPC 2.0 implementation.
 
 Features:
 - **Experimental support for request canceling with `rpc.cancel(id)` in async servers**
-- **Experimental support for response streaming in async servers**
+- **Experimental support for response streaming in the ASGI server**
+- **Experimental support for MQTT Transport**
 - Supports calling JSON-RCP 2.0 servers
 - Build a JSON-RPC server using ASGI, WSGI and CGI
 - Optionally supports async client and server code
 - Use the JSON-RPC 2.0 with any transport layer by using building blocks
 - Battle tested code because it was alreay used ~10 years in varioius closed source projects
 - Unittests are written for new code and whenever a bug is fixed for older parts
 - Abstracts handling of datetime.datetime() over the RPC
@@ -409,14 +410,51 @@
             print(chunk)
             
             
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
+# MQTT Transport
+
+WARNING: MQTT Transport is currently EXPERIMENTAL and its interface is subject to change.
+NOTE: To use MQTT Transport you need to install the package `asyncio_mqtt`.
+
+Server:
+```
+from jsonrpcx import *
+
+class API(MqttJSONRPCServer):
+    async def ping(self):
+        return "pong"
+    
+    async def add(self, a, b):
+        return a + b
+
+
+async def main():
+    server = API("localhost", "user", "password", "mqttChannel")
+    await server.processRequests()
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+Client:
+```
+from jsonrpcx import *
+
+async def main():
+    res = await mqttRPCCall("add", [5, 5], mqttHost="host", mqttUser="user", mqttPassword="password", mqttPort=1883, mqttChannel="mqttChannel")
+    print(res)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
 
 
 # Setup development
 
 Run `pipenv install`
 
 # Testing
```

