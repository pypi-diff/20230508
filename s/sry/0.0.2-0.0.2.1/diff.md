# Comparing `tmp/sry-0.0.2.tar.gz` & `tmp/sry-0.0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sry-0.0.2.tar", last modified: Sun May  7 02:32:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

