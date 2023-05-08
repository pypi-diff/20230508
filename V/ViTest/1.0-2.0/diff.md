# Comparing `tmp/ViTest-1.0.tar.gz` & `tmp/ViTest-2.0-py38-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ViTest-1.0.tar", last modified: Mon May  8 06:18:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

