# Comparing `tmp/prelude-sdk-1.0.1.tar.gz` & `tmp/prelude-sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.0.1.tar", last modified: Fri Apr 21 19:55:43 2023, max compression
+gzip compressed data, was "prelude-sdk-1.1.0.tar", last modified: Sun May  7 12:44:09 2023, max compression
```

## Comparing `prelude-sdk-1.0.1.tar` & `prelude-sdk-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:55:43.421934 prelude-sdk-1.0.1/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.0.1/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-04-21 19:55:43.422005 prelude-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.0.1/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:55:43.417044 prelude-sdk-1.0.1/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.0.1/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:55:43.419498 prelude-sdk-1.0.1/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.0.1/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3363 2023-04-07 19:23:14.000000 prelude-sdk-1.0.1/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     6594 2023-04-18 17:04:09.000000 prelude-sdk-1.0.1/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4658 2023-04-21 19:52:17.000000 prelude-sdk-1.0.1/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     1348 2023-04-19 20:10:59.000000 prelude-sdk-1.0.1/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      540 2023-04-07 19:23:14.000000 prelude-sdk-1.0.1/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:55:43.420120 prelude-sdk-1.0.1/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.0.1/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.0.1/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2609 2023-04-08 00:28:18.000000 prelude-sdk-1.0.1/prelude_sdk/models/codes.py
--rw-r--r--   0 pack       (501) staff       (20)      867 2023-03-09 20:15:21.000000 prelude-sdk-1.0.1/prelude_sdk/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:55:43.418088 prelude-sdk-1.0.1/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-04-21 19:55:43.000000 prelude-sdk-1.0.1/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      796 2023-04-21 19:55:43.000000 prelude-sdk-1.0.1/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-21 19:55:43.000000 prelude-sdk-1.0.1/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-04-21 19:55:43.000000 prelude-sdk-1.0.1/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-04-21 19:55:43.000000 prelude-sdk-1.0.1/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-04-21 19:55:43.422262 prelude-sdk-1.0.1/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:55:43.421597 prelude-sdk-1.0.1/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.0.1/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1101 2023-04-11 22:16:02.000000 prelude-sdk-1.0.1/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:55:43.421829 prelude-sdk-1.0.1/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.0.1/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2658 2023-04-11 22:16:02.000000 prelude-sdk-1.0.1/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4402 2023-04-18 17:04:09.000000 prelude-sdk-1.0.1/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3885 2023-04-13 13:44:46.000000 prelude-sdk-1.0.1/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.0.1/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:44:09.742916 prelude-sdk-1.1.0/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.1.0/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-07 12:44:09.742997 prelude-sdk-1.1.0/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.1.0/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:44:09.738330 prelude-sdk-1.1.0/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.0/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:44:09.740270 prelude-sdk-1.1.0/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.0/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2230 2023-05-07 12:16:47.000000 prelude-sdk-1.1.0/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4077 2023-05-03 13:30:52.000000 prelude-sdk-1.1.0/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3201 2023-05-03 13:30:52.000000 prelude-sdk-1.1.0/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2046 2023-05-03 13:30:52.000000 prelude-sdk-1.1.0/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.1.0/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:44:09.740854 prelude-sdk-1.1.0/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.0/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.1.0/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2609 2023-04-08 00:28:18.000000 prelude-sdk-1.1.0/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:44:09.738908 prelude-sdk-1.1.0/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-07 12:44:09.000000 prelude-sdk-1.1.0/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      806 2023-05-07 12:44:09.000000 prelude-sdk-1.1.0/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-07 12:44:09.000000 prelude-sdk-1.1.0/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-05-07 12:44:09.000000 prelude-sdk-1.1.0/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-05-07 12:44:09.000000 prelude-sdk-1.1.0/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.1.0/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-05-07 12:44:09.743225 prelude-sdk-1.1.0/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:44:09.742595 prelude-sdk-1.1.0/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.1.0/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1101 2023-04-11 22:16:02.000000 prelude-sdk-1.1.0/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:44:09.742820 prelude-sdk-1.1.0/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.1.0/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2188 2023-05-07 12:16:47.000000 prelude-sdk-1.1.0/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3734 2023-05-03 13:30:52.000000 prelude-sdk-1.1.0/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3327 2023-05-04 16:11:50.000000 prelude-sdk-1.1.0/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      785 2023-05-02 14:19:17.000000 prelude-sdk-1.1.0/tests/test_partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.1.0/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.0.1/LICENSE` & `prelude-sdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.0.1/PKG-INFO` & `prelude-sdk-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.0.1
+Version: 1.1.0
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.0.1/README.md` & `prelude-sdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.0.1/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.1.0/prelude_sdk/controllers/detect_controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,191 +1,126 @@
 import requests
 
-from prelude_sdk.spinner import Spinner
 from prelude_sdk.models.account import verify_credentials
 
 
 class DetectController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
     def register_endpoint(self, host, serial_num, edr_id, tags, endpoint_id=None):
         """ Register (or re-register) an endpoint to your account """
-        with Spinner():
-            params = dict(id=f'{host}:{serial_num}:{edr_id}', tags=tags) if not endpoint_id else \
-                dict(endpoint_id=endpoint_id, tags=tags, edr_id=edr_id, host=host)
-            res = requests.post(
-                f'{self.account.hq}/detect/endpoint',
-                headers=self.account.headers,
-                json=params,
-                timeout=10
-            )
-            if res.status_code == 200:
-                return res.text
-            raise Exception(res.text)
+        params = dict(id=f'{host}:{serial_num}:{edr_id}', tags=tags) if not endpoint_id else \
+            dict(endpoint_id=endpoint_id, tags=tags, edr_id=edr_id, host=host)
+        res = requests.post(
+            f'{self.account.hq}/detect/endpoint',
+            headers=self.account.headers,
+            json=params,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.text
+        raise Exception(res.text)
 
     @verify_credentials
     def delete_endpoint(self, ident: str):
         """ Delete an endpoint from your account """
-        with Spinner():
-            params = dict(id=ident)
-            res = requests.delete(
-                f'{self.account.hq}/detect/endpoint',
-                headers=self.account.headers,
-                json=params,
-                timeout=10
-            )
-            if res.status_code != 200:
-                raise Exception(res.text)
+        params = dict(id=ident)
+        res = requests.delete(
+            f'{self.account.hq}/detect/endpoint',
+            headers=self.account.headers,
+            json=params,
+            timeout=10
+        )
+        if res.status_code != 200:
+            raise Exception(res.text)
 
     @verify_credentials
     def list_endpoints(self, days: int = 90):
         """ List all endpoints on your account """
-        with Spinner():
-            params = dict(days=days)
-            res = requests.get(
-                f'{self.account.hq}/detect/endpoint',
-                headers=self.account.headers,
-                params=params,
-                timeout=10
-            )
-            if res.status_code == 200:
-                return res.json()
-            raise Exception(res.text)
+        params = dict(days=days)
+        res = requests.get(
+            f'{self.account.hq}/detect/endpoint',
+            headers=self.account.headers,
+            params=params,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
 
     @verify_credentials
     def describe_activity(self, filters: dict, view: str = 'logs'):
         """ Get report for an Account """
-        with Spinner():
-            params = dict(view=view, **filters)
-            res = requests.get(
-                f'{self.account.hq}/detect/activity',
-                headers=self.account.headers,
-                params=params,
-                timeout=10
-            )
-            if res.status_code == 200:
-                return res.json()
-            raise Exception(res.text)
+        params = dict(view=view, **filters)
+        res = requests.get(
+            f'{self.account.hq}/detect/activity',
+            headers=self.account.headers,
+            params=params,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
 
     @verify_credentials
     def list_queue(self):
         """ List all tests in the queue """
-        with Spinner():
-            res = requests.get(
-                f'{self.account.hq}/detect/queue',
-                headers=self.account.headers,
-                timeout=10
-            )
-            if res.status_code == 200:
-                return res.json()
-            raise Exception(res.text)
+        res = requests.get(
+            f'{self.account.hq}/detect/queue',
+            headers=self.account.headers,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
 
     @verify_credentials
     def list_tests(self):
         """ List all tests available to an account """
-        with Spinner():
-            res = requests.get(
-                f'{self.account.hq}/detect/tests',
-                headers=self.account.headers,
-                timeout=10
-            )
-            if res.status_code == 200:
-                return res.json()
-            raise Exception(res.text)
+        res = requests.get(
+            f'{self.account.hq}/detect/tests',
+            headers=self.account.headers,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
 
     @verify_credentials
     def enable_test(self, ident: str, run_code: int, tags: str):
         """ Enable a test so endpoints will start running it """
-        with Spinner():
-            res = requests.post(
-                url=f'{self.account.hq}/detect/queue/{ident}',
-                headers=self.account.headers,
-                json=dict(code=run_code, tags=tags),
-                timeout=10
-            )
-            if res.status_code != 200:
-                raise Exception(res.text)
+        res = requests.post(
+            url=f'{self.account.hq}/detect/queue/{ident}',
+            headers=self.account.headers,
+            json=dict(code=run_code, tags=tags),
+            timeout=10
+        )
+        if res.status_code != 200:
+            raise Exception(res.text)
 
     @verify_credentials
     def disable_test(self, ident: str, tags: str):
         """ Disable a test so endpoints will stop running it """
-        with Spinner():
-            res = requests.delete(
-                f'{self.account.hq}/detect/queue/{ident}',
-                headers=self.account.headers,
-                params=dict(tags=tags),
-                timeout=10
-            )
-            if res.status_code != 200:
-                raise Exception(res.text)
+        res = requests.delete(
+            f'{self.account.hq}/detect/queue/{ident}',
+            headers=self.account.headers,
+            params=dict(tags=tags),
+            timeout=10
+        )
+        if res.status_code != 200:
+            raise Exception(res.text)
 
     @verify_credentials
     def social_stats(self, ident: str, days: int = 30):
         """ Pull social statistics for a specific test """
-        with Spinner():
-            res = requests.get(
-                f'{self.account.hq}/detect/{ident}/social',
-                headers=self.account.headers,
-                params=dict(days=days),
-                timeout=10
-            )
-            if res.status_code == 200:
-                return res.json()
-            raise Exception(res.text)
-
-    @verify_credentials
-    def search(self, identifier: str):
-        """ Search the NVD for a keyword """
-        with Spinner():
-            res = requests.get(
-                f'{self.account.hq}/detect/search',
-                headers=self.account.headers,
-                params=dict(identifier=identifier),
-                timeout=10
-            )
-            if res.status_code == 200:
-                return res.json()
-            raise Exception(res.text)
-
-    @verify_credentials
-    def recommendations(self):
-        """ List all security recommendations for your account """
-        with Spinner():
-            res = requests.get(
-                f'{self.account.hq}/detect/recommendations',
-                headers=self.account.headers,
-                timeout=10
-            )
-            if res.status_code == 200:
-                return res.json()
-            raise Exception(res.text)
-
-    @verify_credentials
-    def create_recommendation(self, title: str, description: str):
-        """ Create a new security recommendation """
-        with Spinner():
-            params = dict(title=title, description=description)
-            res = requests.post(
-                f'{self.account.hq}/detect/recommendations',
-                headers=self.account.headers,
-                json=params,
-                timeout=10
-            )
-            if res.status_code != 200:
-                raise Exception(res.text)
-
-    @verify_credentials
-    def make_decision(self, id: str, decision: int):
-        """ Add a new decision for a security recommendation """
-        with Spinner():
-            params = dict(decision=decision)
-            res = requests.post(
-                f'{self.account.hq}/detect/recommendations/{id}',
-                headers=self.account.headers,
-                json=params,
-                timeout=10
-            )
-            if res.status_code != 200:
-                raise Exception(res.text)
+        res = requests.get(
+            f'{self.account.hq}/detect/{ident}/social',
+            headers=self.account.headers,
+            params=dict(days=days),
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
```

### Comparing `prelude-sdk-1.0.1/prelude_sdk/models/account.py` & `prelude-sdk-1.1.0/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.0.1/prelude_sdk/models/codes.py` & `prelude-sdk-1.1.0/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.0.1/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.1.0/prelude_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.0.1
+Version: 1.1.0
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.0.1/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.1.0/prelude_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 prelude_sdk/__init__.py
-prelude_sdk/spinner.py
 prelude_sdk.egg-info/PKG-INFO
 prelude_sdk.egg-info/SOURCES.txt
 prelude_sdk.egg-info/dependency_links.txt
 prelude_sdk.egg-info/requires.txt
 prelude_sdk.egg-info/top_level.txt
 prelude_sdk/controllers/__init__.py
 prelude_sdk/controllers/build_controller.py
@@ -19,9 +18,10 @@
 prelude_sdk/models/account.py
 prelude_sdk/models/codes.py
 tests/__init__.py
 tests/conftest.py
 tests/test_build_controller.py
 tests/test_detect_controller.py
 tests/test_iam_controller.py
+tests/test_partner_controller.py
 tests/test_probe_controller.py
 tests/templates/__init__.py
```

### Comparing `prelude-sdk-1.0.1/setup.cfg` & `prelude-sdk-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.0.1
+version = 1.1.0
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.0.1/tests/conftest.py` & `prelude-sdk-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.0.1/tests/test_build_controller.py` & `prelude-sdk-1.1.0/tests/test_build_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 from datetime import datetime
 from importlib.resources import files
 
 from tests import templates as templates
 from prelude_sdk.controllers.build_controller import BuildController
 
 
-@pytest.mark.order(after='test_iam_controller.py::TestIAMController::test_detach_partner')
+@pytest.mark.order(after='test_partner_controller.py::TestPartnerController::test_detach_partner')
 class TestBuildController:
 
     def setup_class(self):
         """Setup the test class"""
         self.test_id = str(uuid.uuid4())
         self.test_name = 'test'
+        self.test_unit = 'AV'
         self.build = BuildController(pytest.account)
 
     def test_create_test(self, unwrap):
         """Test create_test method"""
-        unwrap(self.build.create_test)(self.build, test_id=self.test_id, name=self.test_name)
+        unwrap(self.build.create_test)(self.build, test_id=self.test_id, name=self.test_name, unit=self.test_unit)
         assert True
 
     def test_get_test(self, unwrap):
         """Test get_test method"""
         res = unwrap(self.build.get_test)(self.build, test_id=self.test_id)
         assert res['id'] == self.test_id
         assert res['name'] == self.test_name
+        assert res['unit'] == self.test_unit
 
     def test_upload(self, unwrap):
         """Test upload method"""
         template = files(templates).joinpath('template.go').read_text()
         template = template.replace('$ID', self.test_id)
         template = template.replace('$NAME', self.test_name)
         template = template.replace('$CREATED', str(datetime.utcnow()))
@@ -44,25 +46,11 @@
         res = unwrap(self.build.download)(self.build, test_id=self.test_id, filename=f'{self.test_id}.go')
         assert res is not None
         with open(f'{self.test_id}.go', 'wb') as f:
             f.write(res)
         assert os.path.isfile(f'{self.test_id}.go')
         os.remove(f'{self.test_id}.go')
 
-    def test_map(self, unwrap):
-        """Test map method"""
-        mapping = 'TEST'
-        unwrap(self.build.map)(self.build, test_id=self.test_id, x=mapping)
-        res = unwrap(self.build.get_test)(self.build, test_id=self.test_id)
-        assert mapping in res['mappings']
-
-    def test_unmap(self, unwrap):
-        """Test unmap method"""
-        mapping = 'TEST'
-        unwrap(self.build.unmap)(self.build, test_id=self.test_id, x=mapping)
-        res = unwrap(self.build.get_test)(self.build, test_id=self.test_id)
-        assert mapping not in res['mappings']
-
     def test_delete_test(self, unwrap):
         """Test delete_test method"""
         unwrap(self.build.delete_test)(self.build, test_id=self.test_id)
         assert True
```

### Comparing `prelude-sdk-1.0.1/tests/test_detect_controller.py` & `prelude-sdk-1.1.0/tests/test_detect_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+from datetime import datetime, timedelta, time
+
 import pytest
 import subprocess
 
 from prelude_sdk.models.codes import Decision, RunCode
 from prelude_sdk.controllers.detect_controller import DetectController
 
 
@@ -56,15 +58,19 @@
         assert len([test for test in res if test['test'] == pytest.test_id]) == 1
 
     def test_describe_activity(self, unwrap):
         """Test describe_activity method"""
         try:
             subprocess.run([pytest.probe], capture_output=True, env={'PRELUDE_TOKEN': pytest.endpoint_token}, timeout=20)
         except subprocess.TimeoutExpired:
-            describe_activity = unwrap(self.detect.describe_activity)(self.detect, filters={'endpoint_id': pytest.endpoint_id})
+            filters = dict(
+                start=datetime.utcnow() - timedelta(days=7),
+                finish=datetime.utcnow() + timedelta(days=1)
+            )
+            describe_activity = unwrap(self.detect.describe_activity)(self.detect, filters=filters | {'endpoint_id': pytest.endpoint_id})
             assert len(describe_activity) == 2
         finally:
             os.remove(pytest.probe)
 
     def test_disable_test(self, unwrap):
         """Test disable_test method"""
         unwrap(self.detect.disable_test)(self.detect, ident=pytest.test_id, tags=self.tags)
@@ -77,25 +83,7 @@
         assert len(res.values()) >= 1
 
     def test_delete_endpoint(self, unwrap):
         """Test delete_endpoint method"""
         unwrap(self.detect.delete_endpoint)(self.detect, ident=pytest.endpoint_id)
         res = unwrap(self.detect.list_endpoints)(self.detect)
         assert len(res) == 0
-
-    def test_create_recommendation(self, unwrap):
-        """Test create_recommendation method"""
-        unwrap(self.detect.create_recommendation)(self.detect, title=self.recommendation, description=self.recommendation)
-        assert True
-
-    def test_recommendations(self, unwrap):
-        """Test recommendations method"""
-        res = unwrap(self.detect.recommendations)(self.detect)
-        assert self.recommendation == res[0]['title']
-        assert self.recommendation == res[0]['description']
-        pytest.recommendation_id = res[0]['id']
-
-    def test_make_decision(self, unwrap):
-        """Test make_decision method"""
-        unwrap(self.detect.make_decision)(self.detect, id=pytest.recommendation_id, decision=Decision.APPROVE.value)
-        res = unwrap(self.detect.recommendations)(self.detect)
-        assert Decision.APPROVE.value == res[0]['events'][0]['decision']
```

### Comparing `prelude-sdk-1.0.1/tests/test_iam_controller.py` & `prelude-sdk-1.1.0/tests/test_iam_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 import uuid
 import pytest
 
 from datetime import datetime, timedelta
 from prelude_sdk.models.codes import Permission, Mode
 from prelude_sdk.controllers.iam_controller import IAMController
 
@@ -36,16 +37,19 @@
 
     @pytest.mark.order(1)
     def test_new_account(self, unwrap, pause_for_manual_action, email, api):
         """Test new_account method"""
         pytest.account = Account(hq=api)
         iam = IAMController(pytest.account)
         res = unwrap(iam.new_account)(iam, handle=email)
-        with pause_for_manual_action:
-            input("Press ENTER to continue testing after verifying the account...\n")
+        if email.endswith('@auto-accept.developer.preludesecurity.com'):
+            time.sleep(5)
+        else:
+            with pause_for_manual_action:
+                input("Press ENTER to continue testing after verifying the account...\n")
         pytest.account.headers['account'] = res['account_id']
         pytest.account.headers['token'] = res['token']
         assert len(pytest.account.headers['account']) == 32
         assert check_if_string_is_uuid(pytest.account.headers['token'])
 
     @pytest.mark.order(2)
     def test_get_account(self, unwrap, email):
@@ -68,39 +72,21 @@
     def test_delete_user(self, unwrap):
         """Test delete_user method"""
         iam = IAMController(pytest.account)
         res = unwrap(iam.delete_user)(iam, handle='registration')
         res = unwrap(iam.get_account)(iam)
         assert len([user for user in res['users'] if user['handle'] == 'registration']) == 0
 
-    @pytest.mark.order(5)
-    def test_attach_partner(self, unwrap):
-        """Test attach_partner method"""
-        try:
-            iam = IAMController(pytest.account)
-            unwrap(iam.attach_partner)(iam, 'crowdstrike', 'https://api.us-2.crowdstrike.com', 'test')
-        except Exception as e:
-            assert 'Authentication failed with crowdstrike' in str(e)
-
-    @pytest.mark.order(6)
-    def test_detach_partner(self, unwrap):
-        """Test detach_partner method"""
-        try:
-            iam = IAMController(pytest.account)
-            unwrap(iam.detach_partner)(iam, 'crowdstrike')
-        except Exception as e:
-            assert 'No partner by that name' in str(e)
-
     @pytest.mark.order(after='test_detect_controller.py::TestDetectController::test_describe_activity')
     def test_update_account(self, unwrap):
         """Test update_account method"""
         iam = IAMController(pytest.account)
         unwrap(iam.update_account)(iam, mode=Mode.FROZEN.value)
         res = unwrap(iam.get_account)(iam)
         assert res['mode'] == Mode.FROZEN.value
 
-    @pytest.mark.order(after='test_detect_controller.py::TestDetectController::test_make_decision')
+    @pytest.mark.order(after='test_detect_controller.py::TestDetectController::test_delete_endpoint')
     def test_purge_account(self, unwrap):
         """Test purge_account method"""
         iam = IAMController(pytest.account)
         res = unwrap(iam.purge_account)(iam)
         assert res is not None
```

### Comparing `prelude-sdk-1.0.1/tests/test_probe_controller.py` & `prelude-sdk-1.1.0/tests/test_probe_controller.py`

 * *Files identical despite different names*

