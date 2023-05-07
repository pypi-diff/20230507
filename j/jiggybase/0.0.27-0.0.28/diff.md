# Comparing `tmp/jiggybase-0.0.27.tar.gz` & `tmp/jiggybase-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.27.tar", last modified: Sun May  7 04:38:19 2023, max compression
+gzip compressed data, was "jiggybase-0.0.28.tar", last modified: Sun May  7 16:34:32 2023, max compression
```

## Comparing `jiggybase-0.0.27.tar` & `jiggybase-0.0.28.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.866749 jiggybase-0.0.27/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.27/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 04:38:19.866240 jiggybase-0.0.27/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6181 2023-05-05 04:06:19.000000 jiggybase-0.0.27/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.856720 jiggybase-0.0.27/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.27/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.27/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     9498 2023-05-07 04:35:02.000000 jiggybase-0.0.27/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.859101 jiggybase-0.0.27/jiggybase/examples/
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.27/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.27/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.27/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.27/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.865017 jiggybase-0.0.27/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.27/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.27/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.27/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.27/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.27/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.27/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.27/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.27/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.27/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3166 2023-05-07 04:31:10.000000 jiggybase-0.0.27/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.27/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.27/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.27/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.27/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.27/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.858364 jiggybase-0.0.27/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-07 04:37:31.000000 jiggybase-0.0.27/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-07 04:38:19.866877 jiggybase-0.0.27/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.865643 jiggybase-0.0.27/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.27/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 16:34:32.632058 jiggybase-0.0.28/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.28/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 16:34:32.631754 jiggybase-0.0.28/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6181 2023-05-05 04:06:19.000000 jiggybase-0.0.28/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 16:34:32.623569 jiggybase-0.0.28/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.28/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.28/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     9498 2023-05-07 04:35:02.000000 jiggybase-0.0.28/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 16:34:32.626080 jiggybase-0.0.28/jiggybase/examples/
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.28/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.28/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5535 2023-05-07 14:55:55.000000 jiggybase-0.0.28/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.28/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 16:34:32.631027 jiggybase-0.0.28/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.28/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.28/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.28/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.28/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.28/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.28/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.28/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.28/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.28/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3166 2023-05-07 04:31:10.000000 jiggybase-0.0.28/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.28/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.28/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.28/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.28/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.28/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 16:34:32.625480 jiggybase-0.0.28/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 16:34:32.000000 jiggybase-0.0.28/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-07 16:34:32.000000 jiggybase-0.0.28/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-07 16:34:32.000000 jiggybase-0.0.28/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-07 16:34:32.000000 jiggybase-0.0.28/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-07 16:34:32.000000 jiggybase-0.0.28/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-07 16:34:32.000000 jiggybase-0.0.28/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-07 16:33:59.000000 jiggybase-0.0.28/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-07 16:34:32.632169 jiggybase-0.0.28/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 16:34:32.631354 jiggybase-0.0.28/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.28/test/test.py
```

### Comparing `jiggybase-0.0.27/LICENSE` & `jiggybase-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/PKG-INFO` & `jiggybase-0.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.27
+Version: 0.0.28
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.27/README.md` & `jiggybase-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/client.py` & `jiggybase-0.0.28/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/collection.py` & `jiggybase-0.0.28/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.28/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.28/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/jiggybase_session.py` & `jiggybase-0.0.28/jiggybase/jiggybase_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 # Jiggy Client
-
 import os
 from requests.auth import HTTPBasicAuth
 from requests.packages.urllib3 import Retry
 from requests.adapters import HTTPAdapter
 import requests
+from time import sleep
 from .login import window_open
 
 JIGGYBASE_HOST     = 'https://api.gpt-gateway.com'   # transition to jiggy.ai in progress
 
 JB_KEY_FILE = os.path.expanduser('~') + '/.jiggybase'   # local file to store user entered apikey 
 
+"""
+Retry the following status codes:
+500 Internal Server Error: The server encountered an error while processing the request.
+502 Bad Gateway: The server, while acting as a gateway, received an invalid response from the upstream server.
+503 Service Unavailable: The server is currently unable to handle the request due to maintenance or overload.
+504 Gateway Timeout: The server, while acting as a gateway, did not receive a timely response from the upstream server.
+"""
+RETRY_STATUS_CODES = [500, 502, 503, 504]
 
 class ClientError(Exception):
     """
     API returned 4xx client error
     """
 
 class ServerError(Exception):
@@ -44,20 +52,20 @@
             self.prefix_url = host            
         test_url = f"{self.prefix_url}/docs"
         if requests.head(test_url).status_code != 200:
             raise Exception(f"Invalid or unreachable api: {self.prefix_url}")
             
         self.bearer_token = None
         super(JiggyBaseSession, self).mount('https://',
-                                        HTTPAdapter(max_retries=Retry(connect=5,
-                                                                      read=5,
-                                                                      status=5,
-                                                                      redirect=2,
-                                                                      backoff_factor=.001,
-                                                                      status_forcelist=(500, 502, 503, 504))))
+                                            HTTPAdapter(max_retries=Retry(connect=5,
+                                                                          read=5,
+                                                                          status=5,
+                                                                          redirect=2,
+                                                                          backoff_factor=.001,
+                                                                          status_forcelist=None)))
 
     def _set_bearer(self, jwt):
         self.bearer_token = jwt
         self.headers['Authorization'] = f"Bearer {jwt}"
 
     def _getjwt(self, key):        
         resp = requests.post(f"{JIGGYBASE_HOST}/gpt-gateway-v1/auth", json={'key': key})
@@ -90,25 +98,42 @@
                 print("Invalid API Key")
 
         
     def request(self, method, url, *args, **kwargs):
         if not self.bearer_token:
             self._auth()
         url = self.prefix_url + url
-        #print("~~~~~~~~~~~~~~~~~~~~~~~~\n", method, url)
         # support 'model' (pydantic BaseModel) arg which we convert to json parameter
         if 'model' in kwargs:
             kwargs['data'] = kwargs.pop('model').json()
-        resp =  super(JiggyBaseSession, self).request(method, url, *args, **kwargs)
-        if resp.status_code == 401:
-            self.bearer_token = None
-            del self.headers['Authorization']
-            self._auth()
-            resp =  super(JiggyBaseSession, self).request(method, url, *args, **kwargs)
-        if resp.status_code in [500, 502, 503, 504]:
-            pass # TODO: retry these cases        
+
+        max_attempts = 7
+        backoff_factor = 0.5
+
+        for attempt in range(max_attempts):        
+            try:        
+                resp =  super(JiggyBaseSession, self).request(method, url, *args, **kwargs)
+            except Exception as e:
+                print(f"Exception: {e}")
+                if attempt == max_attempts - 1:
+                    raise
+                continue
+
+            if resp.status_code == 401:
+                self.bearer_token = None
+                del self.headers['Authorization']
+                self._auth()
+                if attempt == max_attempts - 1:
+                    print("Unable to authenticate")
+                    raise ValueError("Unable to authenticate")
+                continue
+            if resp.status_code not in RETRY_STATUS_CODES:
+                break
+            sleep_duration = backoff_factor * (2 ** attempt)
+            sleep(sleep_duration)
+            
         if resp.status_code >= 500:
             raise ServerError(resp.content)
         if resp.status_code >= 400:
             raise ClientError(resp.content)
         return resp
```

### Comparing `jiggybase-0.0.27/jiggybase/login.py` & `jiggybase-0.0.28/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/auth.py` & `jiggybase-0.0.28/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/chat.py` & `jiggybase-0.0.28/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/chunk.py` & `jiggybase-0.0.28/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/collection.py` & `jiggybase-0.0.28/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/metadata.py` & `jiggybase-0.0.28/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/org.py` & `jiggybase-0.0.28/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/plugin.py` & `jiggybase-0.0.28/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/plugin_config.py` & `jiggybase-0.0.28/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/prompt.py` & `jiggybase-0.0.28/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/providers.py` & `jiggybase-0.0.28/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/models/user.py` & `jiggybase-0.0.28/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase/org.py` & `jiggybase-0.0.28/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.28/jiggybase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.27
+Version: 0.0.28
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.27/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.28/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.27/pyproject.toml` & `jiggybase-0.0.28/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.27"
+version = "0.0.28"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.27/test/test.py` & `jiggybase-0.0.28/test/test.py`

 * *Files identical despite different names*

