# Comparing `tmp/audit_flask-0.23.tar.gz` & `tmp/audit_flask-0.24-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audit_flask-0.23.tar", last modified: Mon Jan  3 23:37:24 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

