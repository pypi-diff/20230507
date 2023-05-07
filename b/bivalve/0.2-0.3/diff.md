# Comparing `tmp/bivalve-0.2.tar.gz` & `tmp/bivalve-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bivalve-0.2.tar", last modified: Wed May  3 07:11:32 2023, max compression
+gzip compressed data, was "bivalve-0.3.tar", last modified: Sun May  7 09:56:58 2023, max compression
```

## Comparing `bivalve-0.2.tar` & `bivalve-0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 07:11:32.305411 bivalve-0.2/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-03 07:11:32.302078 bivalve-0.2/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      434 2023-04-04 02:24:44.000000 bivalve-0.2/README.md
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 07:11:32.302078 bivalve-0.2/bivalve/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5262 2023-05-03 07:07:36.000000 bivalve-0.2/bivalve/agent.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2847 2023-05-03 07:07:36.000000 bivalve-0.2/bivalve/aio.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 07:11:32.302078 bivalve-0.2/bivalve/example/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/example/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2249 2023-05-03 07:05:37.000000 bivalve-0.2/bivalve/example/client.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1592 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/example/server.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2908 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/logging.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1634 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/nio.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1895 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/util.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 07:11:32.302078 bivalve-0.2/bivalve.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-03 07:11:32.000000 bivalve-0.2/bivalve.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      324 2023-05-03 07:11:32.000000 bivalve-0.2/bivalve.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-03 07:11:32.000000 bivalve-0.2/bivalve.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-03 07:11:32.000000 bivalve-0.2/bivalve.egg-info/top_level.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-03 07:11:32.305411 bivalve-0.2/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1194 2023-05-03 07:11:27.000000 bivalve-0.2/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-07 09:56:58.565713 bivalve-0.3/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-07 09:56:58.565713 bivalve-0.3/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      434 2023-04-04 02:24:44.000000 bivalve-0.3/README.md
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-07 09:56:58.565713 bivalve-0.3/bivalve/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.3/bivalve/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8092 2023-05-07 09:30:11.000000 bivalve-0.3/bivalve/agent.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5699 2023-05-07 08:43:55.000000 bivalve-0.3/bivalve/aio.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-07 09:56:58.565713 bivalve-0.3/bivalve/example/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.3/bivalve/example/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      802 2023-05-07 07:36:46.000000 bivalve-0.3/bivalve/example/bridge.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2281 2023-05-07 09:30:37.000000 bivalve-0.3/bivalve/example/client.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1731 2023-05-07 09:30:35.000000 bivalve-0.3/bivalve/example/server.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2990 2023-05-07 05:59:39.000000 bivalve-0.3/bivalve/logging.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1799 2023-05-07 06:10:19.000000 bivalve-0.3/bivalve/nio.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1502 2023-05-07 06:02:08.000000 bivalve-0.3/bivalve/util.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-07 09:56:58.565713 bivalve-0.3/bivalve.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-07 09:56:58.000000 bivalve-0.3/bivalve.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      350 2023-05-07 09:56:58.000000 bivalve-0.3/bivalve.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-07 09:56:58.000000 bivalve-0.3/bivalve.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-07 09:56:58.000000 bivalve-0.3/bivalve.egg-info/top_level.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-07 09:56:58.565713 bivalve-0.3/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1194 2023-05-07 09:55:39.000000 bivalve-0.3/setup.py
```

### Comparing `bivalve-0.2/PKG-INFO` & `bivalve-0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bivalve
-Version: 0.2
+Version: 0.3
 Summary: A bi-directional shell-like socket protocol framework using asyncio.
 Home-page: https://github.com/lainproliant/bivalve
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: network sockets protocol shell
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bivalve-0.2/bivalve/aio.py` & `bivalve-0.3/bivalve/example/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,74 @@
 # --------------------------------------------------------------------
-# async.py
+# client.py
 #
 # Author: Lain Musgrove (lain.proliant@gmail.com)
-# Date: Thursday February 16, 2023
+# Date: Friday February 17, 2023
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 import asyncio
-import inspect
 import shlex
-from dataclasses import dataclass, field
-from datetime import datetime
-from typing import Optional
-from uuid import UUID, uuid4
+import signal
+import threading
 
+from bivalve.agent import BivalveAgent
 from bivalve.logging import LogManager
+from bivalve.nio import NonBlockingTextInput
 
 # --------------------------------------------------------------------
 log = LogManager().get(__name__)
 
-
 # --------------------------------------------------------------------
-@dataclass
-class Stream:
-    ID = UUID
-    reader: asyncio.StreamReader
-    writer: asyncio.StreamWriter
-    id: UUID = field(default_factory=uuid4)
-
-    async def close(self):
-        self.writer.close()
-        await self.writer.wait_closed()
-
-    @staticmethod
-    async def connect(host: str, port: int, ssl=None):
-        reader, writer = await asyncio.open_connection(host, port, ssl=ssl)
-        return Stream(reader, writer)
-
-    @staticmethod
-    async def start_server(callback, host: str, port: int, ssl=None):
-        async def connected_callback(reader, writer):
-            if inspect.iscoroutinefunction(callback):
-                await callback(Stream(reader, writer))
-            else:
-                callback(Stream(reader, writer))
-
-        return await asyncio.start_server(connected_callback, host, port, ssl=ssl)
-
-
-# --------------------------------------------------------------------
-@dataclass
-class Connection:
-    ID = Stream.ID
-    stream: Stream
-    task: asyncio.Task
-    syn_at: datetime = datetime.min
-    ack_ttl: Optional[datetime] = None
-    alive: bool = True
-
-    @property
-    def id(self):
-        return self.stream.id
-
-    async def close(self):
-        if self.alive:
-            await self.stream.close()
-            self.alive = False
-
-    async def send(self, *argv: str):
-        assert argv
-        self.stream.writer.write((shlex.join(argv) + "\n").encode())
-        await self.stream.writer.drain()
-        log.debug(f"Sent `{shlex.join(argv)}` to {self.id}")
-
-    async def recv(self) -> list[str]:
-        out = await self.stream.reader.readline()
-        if not out or not self.alive:
-            raise ConnectionAbortedError()
-        argv = shlex.split(out.decode())
-        assert argv
-        log.debug(f"Received `{shlex.join(argv)}` from {self.id}")
-        return argv
-
-    async def try_send(self, *argv: str):
-        assert argv
+class ExampleClient(BivalveAgent):
+    def __init__(self, host="", port=0):
+        super().__init__()
+        self.host = host
+        self.port = port
+
+    def ctrlc_handler(self, *_):
+        log.critical("Ctrl+C received.")
+        self.shutdown()
+
+    async def run(self):
+        signal.signal(signal.SIGINT, self.ctrlc_handler)
+        if self.host and self.port:
+            try:
+                await self.connect(self.host, self.port)
+            except Exception as e:
+                log.fatal("Failed to connect to server.", e)
+                self.shutdown()
+
+        loop = asyncio.get_event_loop()
+        thread = threading.Thread(target=self.input_thread, args=(loop,))
+        thread.start()
+        await super().run()
+        thread.join()
+
+    async def on_client_disconnect(self, _):
+        self.shutdown()
+
+    async def cmd_echo(self, _, msg: str):
+        print(f"<< ECHO >> {msg}")
+
+    def input_thread(self, loop):
+        with NonBlockingTextInput() as ninput:
+            while not self._shutdown_event.is_set():
+                s = ninput.read("> ", timeout=1)
+                if s is not None:
+                    argv = shlex.split(s)
+                    asyncio.run_coroutine_threadsafe(self.send("echo", *argv), loop)
+
 
-        try:
-            await self.send(*argv)
+# --------------------------------------------------------------------
+def main():
+    LogManager().setup()
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
 
-        except ConnectionError:
-            log.warning(f"Could not send `{argv[0]}`, connection was lost.")
+    client = ExampleClient("localhost", 9595)
+    loop.run_until_complete(client.run())
 
-        except Exception as e:
-            log.warning(f"Could not send `{argv[0]}`, unexpected error occurred.", e)
+# --------------------------------------------------------------------
+if __name__ == '__main__':
+    main()
```

### Comparing `bivalve-0.2/bivalve/example/server.py` & `bivalve-0.3/bivalve/example/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 from bivalve.logging import LogManager
 
 # --------------------------------------------------------------------
 log = LogManager().get(__name__)
 
 # --------------------------------------------------------------------
 class ExampleServer(BivalveAgent):
-    def __init__(self, host: str, port: int):
+    def __init__(self, host="", port=0):
         super().__init__()
         self.host = host
         self.port = port
 
     def ctrlc_handler(self, *_):
         log.critical("Ctrl+C received.")
-        self.shutdown_event.set()
+        self._shutdown_event.set()
 
     async def run(self):
         signal.signal(signal.SIGINT, self.ctrlc_handler)
-        await self.serve(self.host, self.port)
+        if self.host and self.port:
+            await self.serve(self.host, self.port)
         await super().run()
 
+    def on_connect(self, conn: Connection):
+        self.schedule(conn.send("echo", "Hello, there!"))
+
     async def cmd_echo(self, conn: Connection, msg: str):
         await conn.send("echo", msg)
 
     async def cmd_quit(self, conn: Connection):
         await self.disconnect(conn)
```

### Comparing `bivalve-0.2/bivalve/logging.py` & `bivalve-0.3/bivalve/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from typing import Optional
 
 from bivalve.util import Borg
 
 
 # --------------------------------------------------------------------
 class LogManager(Borg):
+    """
+    A borg singleton allowing for globally managed log handlers.
+    """
+
     def __init__(self):
         super().__init__()
         if hasattr(self, "_initialized"):
             return
 
         self._filename: Optional[str] = None
         self._format = "%(asctime)s [%(levelname)s]: %(message)s"
```

### Comparing `bivalve-0.2/bivalve/nio.py` & `bivalve-0.3/bivalve/nio.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,37 @@
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 import fcntl
 import os
 import selectors
 import sys
-from dataclasses import dataclass
 from typing import Optional, TextIO
 
 
 # --------------------------------------------------------------------
-@dataclass
 class NonBlockingTextInput:
+    """
+    Controller for non-blocking console text input.
+    """
+
     def __init__(self, infile: TextIO = sys.stdin, promptfile: TextIO = sys.stdout):
         self.infile = infile
         self.promptfile = promptfile
         self.orig_fl: Optional[int] = None
         self.selector = selectors.DefaultSelector()
         self.timed_out = False
 
+    def __enter__(self):
+        self.start()
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        self.stop()
+
     def start(self):
         assert self.orig_fl is None
         self.orig_fl = fcntl.fcntl(self.infile, fcntl.F_GETFL)
         fcntl.fcntl(self.infile, fcntl.F_SETFL, self.orig_fl | os.O_NONBLOCK)
         self.selector.register(self.infile, selectors.EVENT_READ)
 
     def read(self, prompt: Optional[str] = None, timeout: Optional[int] = None):
```

### Comparing `bivalve-0.2/bivalve/util.py` & `bivalve-0.3/bivalve/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,27 @@
 #
 # Author: Lain Musgrove (lain.proliant@gmail.com)
 # Date: Saturday February 11, 2023
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
-import asyncio
-import fcntl
 import inspect
-import os
-import selectors
-import sys
-from dataclasses import dataclass, field
-from typing import Any, Optional, TextIO
-from uuid import UUID, uuid4
+from typing import Any
 
 
 # --------------------------------------------------------------------
 class Borg:
-    _shared_state = {}
+    _shared_state: dict[str, Any] = {}
 
     def __init__(self):
         self.__dict__ = self._shared_state
 
 
 # --------------------------------------------------------------------
-def get_prefixed_methods(prefix, obj):
-    return [
-        getattr(obj, name)
-        for name in dir(obj)
-        if name.startswith(prefix) and callable(getattr(obj, name))
-    ]
-
-
-# --------------------------------------------------------------------
 class Commands:
     @staticmethod
     def get_prefixed_methods(prefix, obj):
         return [
             getattr(obj, name)
             for name in dir(obj)
             if name.startswith(prefix) and callable(getattr(obj, name))
```

### Comparing `bivalve-0.2/bivalve.egg-info/PKG-INFO` & `bivalve-0.3/bivalve.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bivalve
-Version: 0.2
+Version: 0.3
 Summary: A bi-directional shell-like socket protocol framework using asyncio.
 Home-page: https://github.com/lainproliant/bivalve
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: network sockets protocol shell
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bivalve-0.2/setup.py` & `bivalve-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="bivalve",
-    version="0.2",
+    version="0.3",
     description="A bi-directional shell-like socket protocol framework using asyncio.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/bivalve",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

