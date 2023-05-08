# Comparing `tmp/fischer-0.1.2.tar.gz` & `tmp/fischer-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fischer-0.1.2.tar", last modified: Sat Apr 29 12:35:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

