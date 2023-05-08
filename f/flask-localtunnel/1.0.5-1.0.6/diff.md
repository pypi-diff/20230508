# Comparing `tmp/flask-localtunnel-1.0.5.tar.gz` & `tmp/flask_localtunnel-1.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-localtunnel-1.0.5.tar", last modified: Mon Jun 20 06:22:47 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

