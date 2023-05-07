# Comparing `tmp/xia_engine_firestore-0.3.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_firestore-0.3.1-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 158195 bytes, number of entries: 7
--rw-r--r--  2.0 unx      117 b- defN 23-Apr-26 18:54 xia_engine_firestore/__init__.py
--rw-r--r--  2.0 unx   398336 b- defN 23-Apr-26 18:57 xia_engine_firestore/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 18:57 xia_engine_firestore-0.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      817 b- defN 23-Apr-26 18:57 xia_engine_firestore-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 18:57 xia_engine_firestore-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-26 18:57 xia_engine_firestore-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-26 18:57 xia_engine_firestore-0.3.0.dist-info/RECORD
-7 files, 400188 bytes uncompressed, 157029 bytes compressed:  60.8%
+Zip file size: 128753 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      117 b- defN 23-May-07 20:08 xia_engine_firestore/__init__.py
+-rw-r--r--  2.0 unx   354544 b- defN 23-May-07 20:09 xia_engine_firestore/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      150 b- defN 23-May-07 20:09 xia_engine_firestore-0.3.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      780 b- defN 23-May-07 20:09 xia_engine_firestore-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-07 20:09 xia_engine_firestore-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-07 20:09 xia_engine_firestore-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      650 b- defN 23-May-07 20:09 xia_engine_firestore-0.3.1.dist-info/RECORD
+7 files, 356370 bytes uncompressed, 127581 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_firestore/__init__.py
 Comment: 
 
-Filename: xia_engine_firestore/engine.cp39-win_amd64.pyd
+Filename: xia_engine_firestore/engine.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_firestore-0.3.0.dist-info/LICENSE.txt
+Filename: xia_engine_firestore-0.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.3.0.dist-info/METADATA
+Filename: xia_engine_firestore-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_firestore-0.3.0.dist-info/WHEEL
+Filename: xia_engine_firestore-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_firestore-0.3.0.dist-info/top_level.txt
+Filename: xia_engine_firestore-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.3.0.dist-info/RECORD
+Filename: xia_engine_firestore-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_firestore/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_firestore.engine import FirestoreEngine
 
 
 __all__ = [
     "FirestoreEngine"
 ]
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

