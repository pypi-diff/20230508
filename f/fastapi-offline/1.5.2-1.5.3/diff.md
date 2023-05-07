# Comparing `tmp/fastapi_offline-1.5.2.tar.gz` & `tmp/fastapi_offline-1.5.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_offline-1.5.2.tar", last modified: Sat Jan 14 17:22:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

