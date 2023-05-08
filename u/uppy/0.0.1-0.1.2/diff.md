# Comparing `tmp/uppy-0.0.1-py3-none-any.whl.zip` & `tmp/uppy-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,13 @@
-Zip file size: 1103 bytes, number of entries: 5
--rw-rw-r--  2.0 unx       27 b- defN 22-Mar-16 10:17 uppy/__init__.py
--rw-rw-r--  2.0 unx       72 b- defN 23-Jan-09 22:16 uppy-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-09 22:16 uppy-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jan-09 22:16 uppy-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      354 b- defN 23-Jan-09 22:16 uppy-0.0.1.dist-info/RECORD
-5 files, 550 bytes uncompressed, 437 bytes compressed:  20.5%
+Zip file size: 15163 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-08 13:26 uppy-0.1.2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-08 13:26 uppy/
+-rw-r--r--  2.0 unx     2884 b- stor 23-May-08 13:27 uppy-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       34 b- stor 23-May-08 13:26 uppy-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- stor 23-May-08 13:26 uppy-0.1.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1048 b- stor 23-May-08 13:26 uppy-0.1.2.dist-info/RECORD
+-rw-r--r--  2.0 unx       92 b- stor 23-May-08 13:26 uppy-0.1.2.dist-info/WHEEL
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-08 13:27 uppy/_agg/
+-rw-r--r--  2.0 unx       54 b- stor 23-May-08 13:26 uppy/__init__.py
+-rw-r--r--  2.0 unx       33 b- stor 23-May-08 13:27 uppy/_agg/__init__.py
+-rw-r--r--  2.0 unx     9659 b- stor 23-May-08 13:27 uppy/_agg/__init__.dat
+11 files, 13809 bytes uncompressed, 13809 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,16 +1,34 @@
-Filename: uppy/__init__.py
+Filename: uppy-0.1.2.dist-info/
+Comment: 
+
+Filename: uppy/
+Comment: 
+
+Filename: uppy-0.1.2.dist-info/METADATA
+Comment: 
+
+Filename: uppy-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: uppy-0.0.1.dist-info/METADATA
+Filename: uppy-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: uppy-0.0.1.dist-info/WHEEL
+Filename: uppy-0.1.2.dist-info/RECORD
+Comment: 
+
+Filename: uppy-0.1.2.dist-info/WHEEL
+Comment: 
+
+Filename: uppy/_agg/
+Comment: 
+
+Filename: uppy/__init__.py
 Comment: 
 
-Filename: uppy-0.0.1.dist-info/top_level.txt
+Filename: uppy/_agg/__init__.py
 Comment: 
 
-Filename: uppy-0.0.1.dist-info/RECORD
+Filename: uppy/_agg/__init__.dat
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## uppy/__init__.py

```diff
@@ -1,2 +1 @@
-def solve():
-    return 42
+from ._agg import _ZS2n1 as __version__, _ojeje as cli
```

