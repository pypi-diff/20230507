# Comparing `tmp/tiktoken-0.3.3.tar.gz` & `tmp/tiktoken-0.4.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktoken-0.3.3.tar", last modified: Tue Mar 28 20:47:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

