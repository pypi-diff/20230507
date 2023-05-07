# Comparing `tmp/xia_scw_mongodb-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_mongodb-0.0.3-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 238510 bytes, number of entries: 8
--rw-r--r--  2.0 unx      295 b- defN 23-May-06 16:34 xia_scw_mongodb/__init__.py
--rw-r--r--  2.0 unx   323072 b- defN 23-May-06 19:01 xia_scw_mongodb/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   252928 b- defN 23-May-06 19:02 xia_scw_mongodb/mongo.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-06 19:02 xia_scw_mongodb-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      711 b- defN 23-May-06 19:02 xia_scw_mongodb-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-06 19:02 xia_scw_mongodb-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-06 19:02 xia_scw_mongodb-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      710 b- defN 23-May-06 19:02 xia_scw_mongodb-0.0.2.dist-info/RECORD
-8 files, 577981 bytes uncompressed, 237258 bytes compressed:  59.0%
+Zip file size: 191572 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      295 b- defN 23-May-07 06:50 xia_scw_mongodb/__init__.py
+-rw-r--r--  2.0 unx   287760 b- defN 23-May-07 06:50 xia_scw_mongodb/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx   235512 b- defN 23-May-07 06:50 xia_scw_mongodb/mongo.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      150 b- defN 23-May-07 06:50 xia_scw_mongodb-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      674 b- defN 23-May-07 06:50 xia_scw_mongodb-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-07 06:50 xia_scw_mongodb-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-07 06:50 xia_scw_mongodb-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      717 b- defN 23-May-07 06:50 xia_scw_mongodb-0.0.3.dist-info/RECORD
+8 files, 525232 bytes uncompressed, 190308 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: xia_scw_mongodb/__init__.py
 Comment: 
 
-Filename: xia_scw_mongodb/engine.cp39-win_amd64.pyd
+Filename: xia_scw_mongodb/engine.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_scw_mongodb/mongo.cp39-win_amd64.pyd
+Filename: xia_scw_mongodb/mongo.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_scw_mongodb-0.0.2.dist-info/LICENSE.txt
+Filename: xia_scw_mongodb-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_mongodb-0.0.2.dist-info/METADATA
+Filename: xia_scw_mongodb-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_mongodb-0.0.2.dist-info/WHEEL
+Filename: xia_scw_mongodb-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_mongodb-0.0.2.dist-info/top_level.txt
+Filename: xia_scw_mongodb-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_mongodb-0.0.2.dist-info/RECORD
+Filename: xia_scw_mongodb-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_mongodb/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
     "ScwMongoAdmParam", "ScwMongoAdmClient", "ScwMongoAdmEngine",
     "ScwMongodb", "ScwMongoInstance"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

