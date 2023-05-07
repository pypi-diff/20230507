# Comparing `tmp/client_order_fix-0.4.tar.gz` & `tmp/client_order_fix-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_order_fix-0.4.tar", last modified: Sun May  7 12:46:45 2023, max compression
+gzip compressed data, was "client_order_fix-1.0.tar", last modified: Sun May  7 14:51:53 2023, max compression
```

## Comparing `client_order_fix-0.4.tar` & `client_order_fix-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 12:46:45.217575 client_order_fix-0.4/
--rw-rw-rw-   0        0        0      149 2023-05-07 12:46:45.213134 client_order_fix-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-07 12:46:45.184187 client_order_fix-0.4/client_order_fix/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:23:09.000000 client_order_fix-0.4/client_order_fix/__init__.py
--rw-rw-rw-   0        0        0     9142 2023-05-07 12:46:42.000000 client_order_fix-0.4/client_order_fix/client_order.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:46:45.209146 client_order_fix-0.4/client_order_fix.egg-info/
--rw-rw-rw-   0        0        0      149 2023-05-07 12:46:44.000000 client_order_fix-0.4/client_order_fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-07 12:46:44.000000 client_order_fix-0.4/client_order_fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:46:44.000000 client_order_fix-0.4/client_order_fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-07 12:46:44.000000 client_order_fix-0.4/client_order_fix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 12:46:45.218538 client_order_fix-0.4/setup.cfg
--rw-rw-rw-   0        0        0      153 2023-05-07 12:45:56.000000 client_order_fix-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:51:53.355665 client_order_fix-1.0/
+-rw-rw-rw-   0        0        0      149 2023-05-07 14:51:53.350228 client_order_fix-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-07 14:51:53.313309 client_order_fix-1.0/client_order_fix/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:23:09.000000 client_order_fix-1.0/client_order_fix/__init__.py
+-rw-rw-rw-   0        0        0     9347 2023-05-07 14:39:53.000000 client_order_fix-1.0/client_order_fix/client_order.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:51:53.345139 client_order_fix-1.0/client_order_fix.egg-info/
+-rw-rw-rw-   0        0        0      149 2023-05-07 14:51:53.000000 client_order_fix-1.0/client_order_fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-07 14:51:53.000000 client_order_fix-1.0/client_order_fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 14:51:53.000000 client_order_fix-1.0/client_order_fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-07 14:51:53.000000 client_order_fix-1.0/client_order_fix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 14:51:53.356657 client_order_fix-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      153 2023-05-07 14:51:21.000000 client_order_fix-1.0/setup.py
```

### Comparing `client_order_fix-0.4/client_order_fix/client_order.py` & `client_order_fix-1.0/client_order_fix/client_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,23 @@
         self.__client_order_id = unique_id
         self.__quote_request_id = unique_id
         self.__data_row = data_row
 
     def get_client_order_id(self) -> str:
         return self.__client_order_id
 
+    def set_client_order_id(self, clientOrderId):
+        self.__client_order_id = clientOrderId
+
     def get_quote_request_id(self) -> str:
         return self.__quote_request_id
 
+    def set_quote_request_id(self, quoteReqId) -> str:
+        self.__quote_request_id = quoteReqId
+
     def get_test_fields(self) -> List[str]:
         return self.__data_row['testField'].split(',')
 
     def get_message_type(self) -> str:
         return self.__data_row['msgType']
 
     def get_expected_message_type(self) -> str:
```

