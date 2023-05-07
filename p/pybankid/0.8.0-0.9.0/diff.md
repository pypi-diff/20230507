# Comparing `tmp/pybankid-0.8.0.tar.gz` & `tmp/pybankid-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybankid-0.8.0.tar", last modified: Sun Mar  3 19:54:21 2019, max compression
+gzip compressed data, was "dist/pybankid-0.9.0.tar", last modified: Tue Jun 11 04:59:29 2019, max compression
```

## Comparing `pybankid-0.8.0.tar` & `pybankid-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2019-03-03 19:54:21.000000 pybankid-0.8.0/
--rw-r--r--   0 vsts      (1001) docker     (999)       61 2019-03-03 19:54:21.000000 pybankid-0.8.0/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2019-03-03 19:54:21.000000 pybankid-0.8.0/pybankid.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (999)        1 2019-03-03 19:54:20.000000 pybankid-0.8.0/pybankid.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (999)      501 2019-03-03 19:54:21.000000 pybankid-0.8.0/pybankid.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (999)    10767 2019-03-03 19:54:20.000000 pybankid-0.8.0/pybankid.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (999)        7 2019-03-03 19:54:20.000000 pybankid-0.8.0/pybankid.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (999)       69 2019-03-03 19:54:20.000000 pybankid-0.8.0/pybankid.egg-info/requires.txt
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2019-03-03 19:54:21.000000 pybankid-0.8.0/tests/
--rw-r--r--   0 vsts      (1001) docker     (999)      413 2019-03-03 19:54:07.000000 pybankid-0.8.0/tests/test_certutils.py
--rw-r--r--   0 vsts      (1001) docker     (999)        0 2019-03-03 19:54:07.000000 pybankid-0.8.0/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (999)     5228 2019-03-03 19:54:07.000000 pybankid-0.8.0/tests/test_client.py
--rw-r--r--   0 vsts      (1001) docker     (999)     1958 2019-03-03 19:54:07.000000 pybankid-0.8.0/tests/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (999)     5447 2019-03-03 19:54:07.000000 pybankid-0.8.0/tests/test_jsonclient.py
--rw-r--r--   0 vsts      (1001) docker     (999)      449 2019-03-03 19:54:07.000000 pybankid-0.8.0/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2019-03-03 19:54:21.000000 pybankid-0.8.0/bankid/
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2019-03-03 19:54:21.000000 pybankid-0.8.0/bankid/certs/
--rw-r--r--   0 vsts      (1001) docker     (999)      118 2019-03-03 19:54:07.000000 pybankid-0.8.0/bankid/certs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (999)    10331 2019-03-03 19:54:07.000000 pybankid-0.8.0/bankid/jsonclient.py
--rw-r--r--   0 vsts      (1001) docker     (999)     1212 2019-03-03 19:54:07.000000 pybankid-0.8.0/bankid/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (999)     6443 2019-03-03 19:54:07.000000 pybankid-0.8.0/bankid/client.py
--rw-r--r--   0 vsts      (1001) docker     (999)      254 2019-03-03 19:54:07.000000 pybankid-0.8.0/bankid/__version__.py
--rw-r--r--   0 vsts      (1001) docker     (999)     8813 2019-03-03 19:54:07.000000 pybankid-0.8.0/bankid/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (999)     5144 2019-03-03 19:54:07.000000 pybankid-0.8.0/bankid/certutils.py
--rw-r--r--   0 vsts      (1001) docker     (999)     8042 2019-03-03 19:54:07.000000 pybankid-0.8.0/README.rst
--rw-r--r--   0 vsts      (1001) docker     (999)     1079 2019-03-03 19:54:07.000000 pybankid-0.8.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (999)       84 2019-03-03 19:54:07.000000 pybankid-0.8.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (999)       41 2019-03-03 19:54:07.000000 pybankid-0.8.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (999)    10767 2019-03-03 19:54:21.000000 pybankid-0.8.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (999)     3562 2019-03-03 19:54:07.000000 pybankid-0.8.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-06-11 04:59:29.000000 pybankid-0.9.0/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-06-11 04:59:29.000000 pybankid-0.9.0/pybankid.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (117)        7 2019-06-11 04:59:28.000000 pybankid-0.9.0/pybankid.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)       69 2019-06-11 04:59:28.000000 pybankid-0.9.0/pybankid.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)    10767 2019-06-11 04:59:28.000000 pybankid-0.9.0/pybankid.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-06-11 04:59:28.000000 pybankid-0.9.0/pybankid.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)      501 2019-06-11 04:59:29.000000 pybankid-0.9.0/pybankid.egg-info/SOURCES.txt
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-06-11 04:59:29.000000 pybankid-0.9.0/bankid/
+-rw-r--r--   0 vsts      (1001) docker     (117)     6658 2019-06-11 04:59:20.000000 pybankid-0.9.0/bankid/client.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1212 2019-06-11 04:59:20.000000 pybankid-0.9.0/bankid/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8813 2019-06-11 04:59:20.000000 pybankid-0.9.0/bankid/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      254 2019-06-11 04:59:20.000000 pybankid-0.9.0/bankid/__version__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-06-11 04:59:29.000000 pybankid-0.9.0/bankid/certs/
+-rw-r--r--   0 vsts      (1001) docker     (117)      118 2019-06-11 04:59:20.000000 pybankid-0.9.0/bankid/certs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10673 2019-06-11 04:59:20.000000 pybankid-0.9.0/bankid/jsonclient.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5144 2019-06-11 04:59:20.000000 pybankid-0.9.0/bankid/certutils.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3562 2019-06-11 04:59:20.000000 pybankid-0.9.0/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       61 2019-06-11 04:59:29.000000 pybankid-0.9.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (117)    10767 2019-06-11 04:59:29.000000 pybankid-0.9.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (117)       84 2019-06-11 04:59:20.000000 pybankid-0.9.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (117)     1079 2019-06-11 04:59:20.000000 pybankid-0.9.0/LICENSE
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-06-11 04:59:29.000000 pybankid-0.9.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (117)     5228 2019-06-11 04:59:20.000000 pybankid-0.9.0/tests/test_client.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-06-11 04:59:20.000000 pybankid-0.9.0/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      413 2019-06-11 04:59:20.000000 pybankid-0.9.0/tests/test_certutils.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      449 2019-06-11 04:59:20.000000 pybankid-0.9.0/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1958 2019-06-11 04:59:20.000000 pybankid-0.9.0/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5447 2019-06-11 04:59:20.000000 pybankid-0.9.0/tests/test_jsonclient.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       41 2019-06-11 04:59:20.000000 pybankid-0.9.0/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)     8042 2019-06-11 04:59:20.000000 pybankid-0.9.0/README.rst
```

### Comparing `pybankid-0.8.0/pybankid.egg-info/PKG-INFO` & `pybankid-0.9.0/pybankid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybankid
-Version: 0.8.0
+Version: 0.9.0
 Summary: BankID Relying Party client for Python
 Home-page: https://github.com/hbldh/pybankid
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Description: 
         PyBankID
```

### Comparing `pybankid-0.8.0/tests/test_client.py` & `pybankid-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pybankid-0.8.0/tests/test_exceptions.py` & `pybankid-0.9.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pybankid-0.8.0/tests/test_jsonclient.py` & `pybankid-0.9.0/tests/test_jsonclient.py`

 * *Files identical despite different names*

### Comparing `pybankid-0.8.0/bankid/jsonclient.py` & `pybankid-0.9.0/bankid/jsonclient.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,19 +45,22 @@
     """The client to use for communicating with BankID servers via the v.5 API.
 
     :param certificates: Tuple of string paths to the certificate to use and
         the key to sign with.
     :type certificates: tuple
     :param test_server: Use the test server for authenticating and signing.
     :type test_server: bool
+    :param request_timeout: Timeout for BankID requests.
+    :type request_timeout: int
 
     """
 
-    def __init__(self, certificates, test_server=False):
+    def __init__(self, certificates, test_server=False, request_timeout=None):
         self.certs = certificates
+        self._request_timeout = request_timeout
 
         if test_server:
             self.api_url = "https://appapi2.test.bankid.com/rp/v5/"
             self.verify_cert = resource_filename(
                 "bankid.certs", "appapi2.test.bankid.com.pem"
             )
         else:
@@ -72,14 +75,18 @@
         self.client.headers = {"Content-Type": "application/json"}
 
         self._auth_endpoint = urlparse.urljoin(self.api_url, "auth")
         self._sign_endpoint = urlparse.urljoin(self.api_url, "sign")
         self._collect_endpoint = urlparse.urljoin(self.api_url, "collect")
         self._cancel_endpoint = urlparse.urljoin(self.api_url, "cancel")
 
+    def _post(self, endpoint, *args, **kwargs):
+        """Internal helper method for adding timeout to requests."""
+        return self.client.post(endpoint, *args, timeout=self._request_timeout, **kwargs)
+
     def authenticate(
         self, end_user_ip, personal_number=None, requirement=None, **kwargs
     ):
         """Request an authentication order. The :py:meth:`collect` method
         is used to query the status of the order.
 
         Note that personal number is not needed when authentication is to
@@ -114,15 +121,15 @@
         data = {"endUserIp": end_user_ip}
         if personal_number:
             data["personalNumber"] = personal_number
         if requirement and isinstance(requirement, dict):
             data["requirement"] = requirement
         # Handling potentially changed optional in-parameters.
         data.update(kwargs)
-        response = self.client.post(self._auth_endpoint, json=data)
+        response = self._post(self._auth_endpoint, json=data)
 
         if response.status_code == 200:
             return response.json()
         else:
             raise get_json_error_class(response)
 
     def sign(
@@ -178,15 +185,15 @@
         data["userVisibleData"] = self._encode_user_data(user_visible_data)
         if user_non_visible_data:
             data["userNonVisibleData"] = self._encode_user_data(user_non_visible_data)
         if requirement and isinstance(requirement, dict):
             data["requirement"] = requirement
         # Handling potentially changed optional in-parameters.
         data.update(kwargs)
-        response = self.client.post(self._sign_endpoint, json=data)
+        response = self._post(self._sign_endpoint, json=data)
 
         if response.status_code == 200:
             return response.json()
         else:
             raise get_json_error_class(response)
 
     def collect(self, order_ref):
@@ -253,15 +260,15 @@
         :type order_ref: str
         :return: The CollectResponse parsed to a dictionary.
         :rtype: dict
         :raises BankIDError: raises a subclass of this error
                              when error has been returned from server.
 
         """
-        response = self.client.post(
+        response = self._post(
             self._collect_endpoint, json={"orderRef": order_ref}
         )
 
         if response.status_code == 200:
             return response.json()
         else:
             raise get_json_error_class(response)
@@ -276,15 +283,15 @@
         :type order_ref: str
         :return: Boolean regarding success of cancellation.
         :rtype: bool
         :raises BankIDError: raises a subclass of this error
                              when error has been returned from server.
 
         """
-        response = self.client.post(self._cancel_endpoint, json={"orderRef": order_ref})
+        response = self._post(self._cancel_endpoint, json={"orderRef": order_ref})
 
         if response.status_code == 200:
             return response.json() == {}
         else:
             raise get_json_error_class(response)
 
     def _encode_user_data(self, user_data):
```

### Comparing `pybankid-0.8.0/bankid/__init__.py` & `pybankid-0.9.0/bankid/__init__.py`

 * *Files identical despite different names*

### Comparing `pybankid-0.8.0/bankid/client.py` & `pybankid-0.9.0/bankid/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,18 +41,20 @@
     """The client to use for communicating with BankID servers.
 
     :param certificates: Tuple of string paths to the certificate to use and
         the key to sign with.
     :type certificates: tuple
     :param test_server: Use the test server for authenticating and signing.
     :type test_server: bool
+    :param request_timeout: Timeout for BankID requests.
+    :type request_timeout: int
 
     """
 
-    def __init__(self, certificates, test_server=False, **kwargs):
+    def __init__(self, certificates, test_server=False, request_timeout=None, **kwargs):
         self.certs = certificates
 
         warnings.warn(
             "BankIDClient using the SOAP API will "
             "be deprecated in February 2020. Use "
             "bankid.BankIDJSONClient instead.",
             PendingDeprecationWarning,
@@ -74,15 +76,16 @@
 
         headers = {"Content-Type": "text/xml;charset=UTF-8"}
 
         session = requests.Session()
         session.verify = self.verify_cert
         session.cert = self.certs
         session.headers = headers
-        transport = Transport(session=session)
+        timeout_kwarg = {} if request_timeout is None else {"timeout": request_timeout}
+        transport = Transport(session=session, **timeout_kwarg)
         self.client = Client(self.wsdl_url, transport=transport)
 
     def authenticate(self, personal_number, **kwargs):
         """Request an authentication order. The :py:meth:`collect` method
         is used to query the status of the order.
 
         :param personal_number: The Swedish personal number
```

### Comparing `pybankid-0.8.0/bankid/exceptions.py` & `pybankid-0.9.0/bankid/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybankid-0.8.0/bankid/certutils.py` & `pybankid-0.9.0/bankid/certutils.py`

 * *Files identical despite different names*

### Comparing `pybankid-0.8.0/README.rst` & `pybankid-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pybankid-0.8.0/LICENSE` & `pybankid-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybankid-0.8.0/PKG-INFO` & `pybankid-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybankid
-Version: 0.8.0
+Version: 0.9.0
 Summary: BankID Relying Party client for Python
 Home-page: https://github.com/hbldh/pybankid
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Description: 
         PyBankID
```

### Comparing `pybankid-0.8.0/setup.py` & `pybankid-0.9.0/setup.py`

 * *Files identical despite different names*

