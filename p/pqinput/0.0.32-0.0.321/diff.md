# Comparing `tmp/pqinput-0.0.32.tar.gz` & `tmp/pqinput-0.0.321-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.32.tar", last modified: Mon May  8 12:38:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

