# Comparing `tmp/atlas-finance-2.0.0.tar.gz` & `tmp/atlas_finance-2.0.1-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\atlas-finance-2.0.0.tar", last modified: Fri May  5 03:25:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

