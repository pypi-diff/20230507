# Comparing `tmp/AudioProcessor-0.2.0.tar.gz` & `tmp/AudioProcessor-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AudioProcessor-0.2.0.tar", last modified: Sun Apr 30 06:17:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

