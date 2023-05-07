# Comparing `tmp/usearch-0.1.8-cp311-cp311-macosx_10_9_universal2.whl.zip` & `tmp/usearch-0.1.9-cp39-cp39-manylinux_2_24_x86_64.manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 225863 bytes, number of entries: 5
--rwxr-xr-x  2.0 unx   762843 b- defN 23-May-02 19:47 usearch.cpython-311-darwin.so
--rw-rw-r--  2.0 unx      391 b- defN 23-May-02 19:47 usearch-0.1.8.dist-info/RECORD
--rw-r--r--  2.0 unx      115 b- defN 23-May-02 19:47 usearch-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-02 19:47 usearch-0.1.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx     6182 b- defN 23-May-02 19:47 usearch-0.1.8.dist-info/METADATA
-5 files, 769539 bytes uncompressed, 225147 bytes compressed:  70.7%
+Zip file size: 126619 bytes, number of entries: 7
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 15:31 usearch./
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 15:31 usearch-0.1.9.dist-info/
+-rwxr-xr-x  2.0 unx   307168 b- defN 23-May-03 15:31 usearch.cpython-39-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx      401 b- defN 23-May-03 15:31 usearch-0.1.9.dist-info/RECORD
+-rw-r--r--  2.0 unx    17819 b- defN 23-May-03 15:31 usearch-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx        8 b- defN 23-May-03 15:31 usearch-0.1.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      149 b- defN 23-May-03 15:31 usearch-0.1.9.dist-info/WHEEL
+7 files, 325545 bytes uncompressed, 125667 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
-Filename: usearch.cpython-311-darwin.so
+Filename: usearch./
 Comment: 
 
-Filename: usearch-0.1.8.dist-info/RECORD
+Filename: usearch-0.1.9.dist-info/
 Comment: 
 
-Filename: usearch-0.1.8.dist-info/WHEEL
+Filename: usearch.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: usearch-0.1.8.dist-info/top_level.txt
+Filename: usearch-0.1.9.dist-info/RECORD
 Comment: 
 
-Filename: usearch-0.1.8.dist-info/METADATA
+Filename: usearch-0.1.9.dist-info/METADATA
+Comment: 
+
+Filename: usearch-0.1.9.dist-info/top_level.txt
+Comment: 
+
+Filename: usearch-0.1.9.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

