# Comparing `tmp/shellfoundry-1.2.4.tar.gz` & `tmp/shellfoundry-1.2.8.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\shellfoundry-1.2.4.tar", last modified: Wed Sep 26 16:15:33 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

