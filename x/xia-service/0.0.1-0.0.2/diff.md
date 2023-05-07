# Comparing `tmp/xia_service-0.0.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_service-0.0.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 100724 bytes, number of entries: 7
--rw-r--r--  2.0 unx       94 b- defN 23-May-07 12:24 xia_service/__init__.py
--rw-r--r--  2.0 unx   239104 b- defN 23-May-07 12:50 xia_service/service.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-07 12:50 xia_service-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      668 b- defN 23-May-07 12:50 xia_service-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-07 12:50 xia_service-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-07 12:50 xia_service-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      583 b- defN 23-May-07 12:50 xia_service-0.0.1.dist-info/RECORD
-7 files, 240710 bytes uncompressed, 99682 bytes compressed:  58.6%
+Zip file size: 100745 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       94 b- defN 23-May-07 20:32 xia_service/__init__.py
+-rw-r--r--  2.0 unx   239104 b- defN 23-May-07 20:34 xia_service/service.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-07 20:34 xia_service-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      668 b- defN 23-May-07 20:34 xia_service-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-07 20:34 xia_service-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-07 20:34 xia_service-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      583 b- defN 23-May-07 20:34 xia_service-0.0.2.dist-info/RECORD
+7 files, 240710 bytes uncompressed, 99703 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_service/__init__.py
 Comment: 
 
 Filename: xia_service/service.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_service-0.0.1.dist-info/LICENSE.txt
+Filename: xia_service-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_service-0.0.1.dist-info/METADATA
+Filename: xia_service-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_service-0.0.1.dist-info/WHEEL
+Filename: xia_service-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_service-0.0.1.dist-info/top_level.txt
+Filename: xia_service-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_service-0.0.1.dist-info/RECORD
+Filename: xia_service-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_service/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 
 __all__ = [
     "Service"
 ]
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## Comparing `xia_service-0.0.1.dist-info/METADATA` & `xia_service-0.0.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-service
-Version: 0.0.1
+Version: 0.0.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-service/0.0.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-service/0.0.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

