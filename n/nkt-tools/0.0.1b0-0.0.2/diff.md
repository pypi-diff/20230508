# Comparing `tmp/nkt_tools-0.0.1b0.tar.gz` & `tmp/nkt_tools-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkt_tools-0.0.1b0.tar", last modified: Sun May  7 03:25:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

