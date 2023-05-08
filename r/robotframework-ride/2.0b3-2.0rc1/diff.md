# Comparing `tmp/robotframework-ride-2.0b3.tar.gz` & `tmp/robotframework-ride-2.0rc1.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-ride-2.0b3.tar", last modified: Sun Jan 15 16:47:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

