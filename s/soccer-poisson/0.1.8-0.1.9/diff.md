# Comparing `tmp/soccer_poisson-0.1.8.tar.gz` & `tmp/soccer_poisson-0.1.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/soccer_poisson-0.1.8.tar", last modified: Tue Apr  4 08:36:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

