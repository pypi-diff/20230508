# Comparing `tmp/pyscisci-0.8.11.tar.gz` & `tmp/pyscisci-0.8.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscisci-0.8.11.tar", last modified: Mon May  8 13:36:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

