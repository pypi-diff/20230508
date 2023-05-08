# Comparing `tmp/grismconf-1.39.tar.gz` & `tmp/grismconf-1.40-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grismconf-1.39.tar", last modified: Tue Feb 28 14:23:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

