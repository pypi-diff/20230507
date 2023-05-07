# Comparing `tmp/cshogi-0.5.1.tar.gz` & `tmp/cshogi-0.5.2-cp39-cp39-manylinux_2_12_x86_64.manylinux2010_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshogi-0.5.1.tar", last modified: Thu Mar 23 07:50:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

