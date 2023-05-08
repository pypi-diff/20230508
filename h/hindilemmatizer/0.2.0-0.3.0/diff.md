# Comparing `tmp/hindilemmatizer-0.2.0.tar.gz` & `tmp/hindilemmatizer-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hindilemmatizer-0.2.0.tar", last modified: Sat May  6 13:40:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

