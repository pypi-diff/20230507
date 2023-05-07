# Comparing `tmp/client_order_fix-0.3.tar.gz` & `tmp/client_order_fix-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_order_fix-0.3.tar", last modified: Thu Apr 27 11:16:02 2023, max compression
+gzip compressed data, was "client_order_fix-0.4.tar", last modified: Sun May  7 12:46:45 2023, max compression
```

## Comparing `client_order_fix-0.3.tar` & `client_order_fix-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 11:16:02.088871 client_order_fix-0.3/
--rw-rw-rw-   0        0        0      149 2023-04-27 11:16:02.084804 client_order_fix-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 11:16:02.053049 client_order_fix-0.3/client_order_fix/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:23:09.000000 client_order_fix-0.3/client_order_fix/__init__.py
--rw-rw-rw-   0        0        0     8594 2023-04-27 11:14:20.000000 client_order_fix-0.3/client_order_fix/client_order.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:16:02.079780 client_order_fix-0.3/client_order_fix.egg-info/
--rw-rw-rw-   0        0        0      149 2023-04-27 11:16:01.000000 client_order_fix-0.3/client_order_fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-04-27 11:16:01.000000 client_order_fix-0.3/client_order_fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 11:16:01.000000 client_order_fix-0.3/client_order_fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-27 11:16:01.000000 client_order_fix-0.3/client_order_fix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 11:16:02.088871 client_order_fix-0.3/setup.cfg
--rw-rw-rw-   0        0        0      153 2023-04-27 11:15:58.000000 client_order_fix-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:46:45.217575 client_order_fix-0.4/
+-rw-rw-rw-   0        0        0      149 2023-05-07 12:46:45.213134 client_order_fix-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-07 12:46:45.184187 client_order_fix-0.4/client_order_fix/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:23:09.000000 client_order_fix-0.4/client_order_fix/__init__.py
+-rw-rw-rw-   0        0        0     9142 2023-05-07 12:46:42.000000 client_order_fix-0.4/client_order_fix/client_order.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:46:45.209146 client_order_fix-0.4/client_order_fix.egg-info/
+-rw-rw-rw-   0        0        0      149 2023-05-07 12:46:44.000000 client_order_fix-0.4/client_order_fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-07 12:46:44.000000 client_order_fix-0.4/client_order_fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:46:44.000000 client_order_fix-0.4/client_order_fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-07 12:46:44.000000 client_order_fix-0.4/client_order_fix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 12:46:45.218538 client_order_fix-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      153 2023-05-07 12:45:56.000000 client_order_fix-0.4/setup.py
```

### Comparing `client_order_fix-0.3/client_order_fix/client_order.py` & `client_order_fix-0.4/client_order_fix/client_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,18 @@
                     message.setField(quickfix.Account(ACCOUNT_DEV))
                 elif env == 'UAT':
                     message.setField(quickfix.Account(ACCOUNT_UAT))
 
         if self.__data_row.get('orderQty'):
             message.setField(quickfix.OrderQty(float(self.__data_row['orderQty'])))
 
+        if self.__data_row.get('price'):
+            if not self.__data_row.get('pq_order'):
+                message.setField(quickfix.Price(float(self.__data_row['price'])))
+
         if self.__data_row.get('side'):
             if self.__data_row['side'] == 'empty':
                 message.setField(quickfix.Side(''))
             else:
                 message.setField(quickfix.Side(self.__data_row['side']))
 
         if self.__data_row.get('symbol'):
@@ -146,30 +150,35 @@
                 else:
                     groupOne.setField(quickfix.PartyRole(int(self.__data_row['partyRole'])))
                     groupTwo.setField(quickfix.PartyRole(int(self.__data_row['partyRole'])))
                     message.addGroup(groupOne)
                     message.addGroup(groupTwo)
 
         if self.__data_row.get('quoteReqId'):
-            message.setField(quickfix.QuoteReqID(self.__quote_request_id))
+            if self.__data_row.get('quoteReqId') != "no tag":
+                message.setField(quickfix.QuoteReqID(self.__quote_request_id))
 
         if self.__data_row.get('ordType'):
             if self.__data_row['ordType'] == 'empty':
                 message.setField(quickfix.OrdType(''))
             else:
                 message.setField(quickfix.OrdType(self.__data_row['ordType']))
 
         if self.__data_row.get('tif'):
             if self.__data_row['tif'] == 'empty':
                 message.setField(quickfix.TimeInForce(''))
             else:
                 message.setField(quickfix.TimeInForce(self.__data_row['tif']))
 
         if self.__data_row.get('clOrdId'):
-            message.setField(quickfix.ClOrdID(self.__client_order_id))
+            if self.__data_row.get('clOrdId') != "no tag":
+                message.setField(quickfix.ClOrdID(self.__client_order_id))
+            if self.__data_row.get('pq_order'):
+                self.__client_order_id = str(randint(0, 100000)) + str(datetime.now().strftime('%M:%S.%f')[:-4])
+                message.setField(quickfix.ClOrdID(self.__client_order_id))
 
         if self.__data_row.get('tradSesReqId'):
             if self.__data_row['tradSesReqId'] == 'empty':
                 message.setField(quickfix.TradSesReqID(''))
             elif self.__data_row['tradSesReqId'] == 'no tag':
                 pass
             elif self.__data_row['tradSesReqId'] == 'yes':
@@ -201,8 +210,8 @@
             return ''
         elif row[requestString] == 'duplicate':
             return '12345'
 
     @staticmethod
     def from_table_row(row: dict, requestString) -> 'ClientOrder':
         unique_id = ClientOrder.generateUniqueId(row, requestString)
-        return ClientOrder(unique_id, row)
+        return ClientOrder(unique_id, row)
```

