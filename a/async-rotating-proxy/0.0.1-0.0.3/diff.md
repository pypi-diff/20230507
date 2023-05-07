# Comparing `tmp/async_rotating_proxy-0.0.1.tar.gz` & `tmp/async_rotating_proxy-0.0.3.tar.gz`

## Comparing `async_rotating_proxy-0.0.1.tar` & `async_rotating_proxy-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.1/requirements.txt
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.1/src/async_rotating_proxy/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.1/src/async_rotating_proxy/browser.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.1/README.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/src/async_rotating_proxy/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/src/async_rotating_proxy/browser.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/PKG-INFO
```

### Comparing `async_rotating_proxy-0.0.1/src/async_rotating_proxy/__init__.py` & `async_rotating_proxy-0.0.3/src/async_rotating_proxy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from fastapi import FastAPI
 from fastapi.responses import HTMLResponse
 import uvicorn
 
 import aiohttp
+from multiprocessing import Process
 
 import urllib.parse
 import random
-import threading
+import os
 
 
 def app(proxies: list[str],
         proxy_username: str | None = None, 
         proxy_password: str | None = None,
         proxy_scheme: str = "http",
         headers: dict = {"User-Agent": "Chrome"}):
@@ -25,14 +26,16 @@
 
     Returns:
         FastAPI: The proxy-redirect server
     """
 
     app = FastAPI()
 
+    app.pid = os.getpid()
+
     @app.get("/")
     async def forward_proxy(url: str):
         """Forward a request through a proxy and return the response
 
         Args:
             url (str): URL to get encoded with urllib.parse.quote_plus()
 
@@ -60,70 +63,61 @@
     return app
 
 
 class ProxyAPI():
     """Start an API on localhost to redirect traffic through proxies
 
     Usage:
-        # Create the ProxyAPI
-        # Instantiating this class launches the server
-        proxy_api = ProxyAPI([proxy1:port, proxy2:port, proxy3:port],
-                              proxy_username='my_auth_cred',
-                              proxy_password='my_auth_cred',
-                              port=9001)
-
-        # Encode and format the URL to get
-        url = 'http://checkip.dyndns.org/' 
-        formatted_url = proxy_api.format_url(url)
-
-        # Visit the formatted URL using preferred method
-        # I use pyppeteer in this example
-        browser = await pyppeteer.launch()
-        page = await browser.newPage()
-        await page.goto(formatted_url)
+        with ProxyAPI([proxy_list]) as proxy_api:
+            url = proxy_api.format_url("your_url")
+            do scraping stuff with your url now
         
 
     Constructor Args:
         proxies (list[str]): List of proxies to rotate through in ip:port form
         proxy_username (str | None): Username for proxy authentication if applicable
         proxy_password (str | None): Password for proxy authentication if applicable
         port (int): The port on localhost where the proxy API is running
         proxy_scheme (http): The scheme of the proxy server
     """
+    api_pid: int
+
     def __init__(
             self,
             proxies: list[str], 
             proxy_username: str | None = None,
             proxy_password: str | None = None,
             port: int = 8000,
             proxy_scheme: str = "http"
         ):
         self.proxies = proxies
         self.proxy_username = proxy_username
         self.proxy_password = proxy_password
         self.port = port
         self.proxy_scheme = proxy_scheme
 
-        self.start_server()
+
+    def __enter__(self):
+        self._process = Process(target=self._start_server)
+        self._process.start()
+        return self
+        
+    
+    def __exit__(self, exc_type, value, traceback):
+        self._process.terminate()
 
 
-    def start_server(self):
+    def _start_server(self):
         """Start a FastAPI daemon for routing requests through proxies."""
         api = app(self.proxies, 
                   proxy_username=self.proxy_username,
                   proxy_password=self.proxy_password,
                   proxy_scheme=self.proxy_scheme)
 
-        thread = threading.Thread(target=uvicorn.run,
-                                  args=[api],
-                                  kwargs={"port": self.port},
-                                  name="uvicorn_proxy_server",
-                                  daemon=True)
-
-        thread.start()
+        uvicorn.run(api, port=self.port)
 
 
     def format_url(self, url: str):
         """Format the URL to route through the ProxyAPI server.
     
         1. Encodes the URL parameter
         2. Prepends http://127.0.0.1:{port}/ to the URL
```

### Comparing `async_rotating_proxy-0.0.1/src/async_rotating_proxy/browser.py` & `async_rotating_proxy-0.0.3/src/async_rotating_proxy/browser.py`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.1/LICENSE.txt` & `async_rotating_proxy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.1/pyproject.toml` & `async_rotating_proxy-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "async_rotating_proxy"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
     { name="Greg Bizup", email="g.bizup@gmail.com" }
 ]
 description = "Run an API on your local machine that reroutes traffic through rotating proxies. Useful for pyppeteer proxy rotation."
 readme = "README.md"
 requires-python = ">3.10"
 classifiers = [
@@ -20,15 +20,15 @@
     "fastapi",
     "proxy",
     "rotating proxy",
     "pyppeteer",
     "scraping",
 ]
 dependencies = [
-    "aiohttp>=3.8.4",
-    "fastapi>=0.95.1",
-    "pyppeteer>=1.0.2",
-    "uvicorn>=0.21.1",
+    "aiohttp >= 3.8.4",
+    "fastapi >= 0.95.1",
+    "pyppeteer >= 1.0.2",
+    "uvicorn >= 0.21.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/gbiz123/async-rotating-proxy"
```

