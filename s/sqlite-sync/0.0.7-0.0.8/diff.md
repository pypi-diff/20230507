# Comparing `tmp/sqlite_sync-0.0.7-py3-none-any.whl.zip` & `tmp/sqlite_sync-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 6092 bytes, number of entries: 14
+Zip file size: 6453 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       64 b- defN 23-Apr-28 13:42 engine/__init__.py
 -rw-r--r--  2.0 unx     1007 b- defN 23-Apr-28 13:42 engine/client.py
 -rw-r--r--  2.0 unx      973 b- defN 23-Apr-28 13:42 engine/control_db.py
 -rw-r--r--  2.0 unx     1423 b- defN 23-Apr-28 13:42 engine/handler.py
 -rw-r--r--  2.0 unx      414 b- defN 23-Apr-28 13:42 engine/listen.py
 -rw-r--r--  2.0 unx       64 b- defN 23-Apr-28 05:40 sqlite_sync/__init__.py
 -rw-r--r--  2.0 unx     1007 b- defN 23-Apr-28 05:40 sqlite_sync/client.py
 -rw-r--r--  2.0 unx      973 b- defN 23-Apr-28 05:40 sqlite_sync/control_db.py
--rw-r--r--  2.0 unx     1635 b- defN 23-Apr-28 13:53 sqlite_sync/handler.py
--rw-r--r--  2.0 unx      414 b- defN 23-Apr-28 05:40 sqlite_sync/listen.py
--rw-r--r--  2.0 unx     1048 b- defN 23-Apr-28 13:55 sqlite_sync-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 13:55 sqlite_sync-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-28 13:55 sqlite_sync-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1075 b- defN 23-Apr-28 13:55 sqlite_sync-0.0.7.dist-info/RECORD
-14 files, 10201 bytes uncompressed, 4320 bytes compressed:  57.7%
+-rw-r--r--  2.0 unx     2426 b- defN 23-May-07 14:47 sqlite_sync/handler.py
+-rw-r--r--  2.0 unx      981 b- defN 23-May-07 14:20 sqlite_sync/listen.py
+-rw-r--r--  2.0 unx     1048 b- defN 23-May-07 14:47 sqlite_sync-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 14:47 sqlite_sync-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-07 14:47 sqlite_sync-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1075 b- defN 23-May-07 14:47 sqlite_sync-0.0.8.dist-info/RECORD
+14 files, 11559 bytes uncompressed, 4681 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: sqlite_sync/handler.py
 Comment: 
 
 Filename: sqlite_sync/listen.py
 Comment: 
 
-Filename: sqlite_sync-0.0.7.dist-info/METADATA
+Filename: sqlite_sync-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_sync-0.0.7.dist-info/WHEEL
+Filename: sqlite_sync-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_sync-0.0.7.dist-info/top_level.txt
+Filename: sqlite_sync-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_sync-0.0.7.dist-info/RECORD
+Filename: sqlite_sync-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_sync/handler.py

```diff
@@ -1,47 +1,62 @@
 import json
 import time
 import traceback
 
 from .control_db import Driver
 from .listen import Listen
 
-from multiprocessing import Process
+from multiprocessing import Process, Event
 from threading import Thread
 from sys import platform
 
 
 class HandlerDB(Driver, Listen):
     __slots__ = ["HD", "config"]
 
     def __init__(self, warp_file=':memory:', config=("127.0.0.1", 1001)):
         super().__init__(warp_file)
         self.config = config
-
+        self.event = Event()
         if platform not in ['darwin', 'win32']:
             self.HD = Process(target=self.handler, name='HANDLER_DB')
             self.HD.start()
         else:
             self.HD = Thread(target=self.handler, name='HANDLER_DB')
             self.HD.start()
         time.sleep(0.1)
 
     def handler(self):
-        while True:
+        while not self.event.is_set():  # sooner or later...
             try:
                 for data in self.listen(self.config):
                     response = data[0]
                     if 'query' in response and 'type' in response:
-                        match response['type']:
+                        """match response['type']:
                             case 'save':
                                 result = self.save(response['query'])
                             case 'receive':
                                 result = self.receive(response['query'])
                             case 'receives':
                                 result = self.receives(response['query'])
                             case _:
-                                result = 'Unknown request!', None
+                                result = 'Unknown request!', None"""  # this is a new feature in python 3.10
+                        if response['type'] == 'save':
+                            result = self.save(response['query'])
+                        elif response['type'] == 'receive':
+                            result = self.receive(response['query'])
+                        elif response['type'] == 'receives':
+                            result = self.receives(response['query'])
+                        else:
+                            result = 'Unknown request!', None
                         data[1].send(bytes(json.dumps({'result': result[0], 'status': result[1]}), encoding='UTF-8'))
             except KeyboardInterrupt:
                 break
             except:
                 traceback.print_exc()
+
+    def kill(self):
+        if platform not in ['darwin', 'win32']:
+            self.HD.terminate()
+        else:
+            self.event.set()
+        # self.event.set()  # TODO: Maybe use this?
```

## sqlite_sync/listen.py

```diff
@@ -1,16 +1,34 @@
 import json
 import socket
 
 
-class Listen:
-    @staticmethod
-    def listen(config):
-        sock = socket.socket(socket.SOCK_DGRAM)
-        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        sock.bind(config)
-        sock.listen()
+class ListeningSocket:
+    __slots__ = ('_addr', '_buffer_size', '_socket')
+
+    def __init__(self, address: str, buffer_size: int = 16384):
+        self._addr = address
+        self._buffer_size = buffer_size
+        self._socket = socket.socket(socket.SOCK_DGRAM)
+        self._socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self._socket.bind(self._addr)
+        self._socket.listen()
+
+    def listen(self):
         while True:
-            conn, addr = sock.accept()
+            conn, addr = self._socket.accept()
             with conn:
-                data = conn.recv(16384)
+                try:
+                    data = conn.recv(self._buffer_size)
+                except KeyboardInterrupt:
+                    conn.close()
+                    self._socket.close()
+                    break
                 yield json.loads(data), conn
+
+
+class Listen:
+    @staticmethod
+    def listen(config):
+        sock = ListeningSocket(config)
+        for data, conn in sock.listen():
+            yield data, conn
```

## Comparing `sqlite_sync-0.0.7.dist-info/METADATA` & `sqlite_sync-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-sync
-Version: 0.0.7
+Version: 0.0.8
 Summary: SQLite3 wrapper for query synchronization
 Home-page: https://github.com/RobertMeow/sqlite_sync
 Author: Robert Popov
 Author-email: robert@berht.dev
 
 SQLite3 is a lightweight embeddable database that is widely used in various projects. However, using SQLite3 multithreaded can lead to unexpected results such as data loss, blocking, recursive errors.
```

## Comparing `sqlite_sync-0.0.7.dist-info/RECORD` & `sqlite_sync-0.0.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 engine/client.py,sha256=UE3aMauWLws9zeNzikHstZmtS7Jrea_mRZeiWLnXuQ0,1007
 engine/control_db.py,sha256=JCv6UxeDr2_P3edAqHfgsHKQr5uP2bjuRq5jS6Pa1xw,973
 engine/handler.py,sha256=g-cO8YZWtIZadkzuyExcB5fCNuElLsYFKhrCPPsvpH8,1423
 engine/listen.py,sha256=F_xNU_IugFKno0T1UHRX0-rnwdkAqpiicegHZrteqYg,414
 sqlite_sync/__init__.py,sha256=zCnoGgU83SmtJ1pKXN175Vy0PxGqL8qsgZMnUrMBfu4,64
 sqlite_sync/client.py,sha256=UE3aMauWLws9zeNzikHstZmtS7Jrea_mRZeiWLnXuQ0,1007
 sqlite_sync/control_db.py,sha256=JCv6UxeDr2_P3edAqHfgsHKQr5uP2bjuRq5jS6Pa1xw,973
-sqlite_sync/handler.py,sha256=zzeY7jNeVNjTbm9361vU3BppQr5gaixiBnpwL_UnHq8,1635
-sqlite_sync/listen.py,sha256=F_xNU_IugFKno0T1UHRX0-rnwdkAqpiicegHZrteqYg,414
-sqlite_sync-0.0.7.dist-info/METADATA,sha256=MTcC5p1710JrkpwIrtU-bMchF6SqeZ6R3KqMslZsIUQ,1048
-sqlite_sync-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sqlite_sync-0.0.7.dist-info/top_level.txt,sha256=KmiUKkAR61MPTL_8aAXAJ-DKcqi_CJ63JGGHheK1M1Q,12
-sqlite_sync-0.0.7.dist-info/RECORD,,
+sqlite_sync/handler.py,sha256=7SOXwC7p1Pd5hMZqI-twY7ffQhizX2Eyk91VWib-VCU,2426
+sqlite_sync/listen.py,sha256=n2ZKEEj6_zqA9sD_DzNy1mjpR2jFspXPsgZ6Cdin088,981
+sqlite_sync-0.0.8.dist-info/METADATA,sha256=Eu2Mt1CJybG57-Tan2oXiq4StcPcYTVOL-3Zp8l8uZ8,1048
+sqlite_sync-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sqlite_sync-0.0.8.dist-info/top_level.txt,sha256=KmiUKkAR61MPTL_8aAXAJ-DKcqi_CJ63JGGHheK1M1Q,12
+sqlite_sync-0.0.8.dist-info/RECORD,,
```

