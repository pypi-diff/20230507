# Comparing `tmp/codefast-23.5.5.11.tar.gz` & `tmp/codefast-23.5.7.16-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codefast-23.5.5.11.tar", last modified: Fri May  5 03:21:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

