# Comparing `tmp/amps-0.0.2.tar.gz` & `tmp/amps-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amps-0.0.2.tar", last modified: Tue Apr  4 07:32:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

