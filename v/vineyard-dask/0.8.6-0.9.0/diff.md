# Comparing `tmp/vineyard_dask-0.8.6-py3-none-any.whl.zip` & `tmp/vineyard_dask-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 21449 bytes, number of entries: 11
--rw-r--r--  2.0 unx      650 b- defN 22-Sep-26 01:59 vineyard/contrib/dask/__init__.py
--rw-r--r--  2.0 unx     5125 b- defN 22-Sep-26 01:59 vineyard/contrib/dask/dask.py
--rw-r--r--  2.0 unx      650 b- defN 22-Sep-26 01:59 vineyard/contrib/dask/tests/__init__.py
--rw-r--r--  2.0 unx      735 b- defN 22-Sep-26 01:59 vineyard/contrib/dask/tests/conftest.py
--rw-r--r--  2.0 unx     5329 b- defN 22-Sep-26 01:59 vineyard/contrib/dask/tests/test_dask.py
--rw-r--r--  2.0 unx    63232 b- defN 22-Sep-26 02:32 vineyard_dask-0.8.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    18247 b- defN 22-Sep-26 02:32 vineyard_dask-0.8.6.dist-info/METADATA
--rw-r--r--  2.0 unx     2068 b- defN 22-Sep-26 02:32 vineyard_dask-0.8.6.dist-info/NOTICE.txt
--rw-r--r--  2.0 unx       93 b- defN 22-Sep-26 02:32 vineyard_dask-0.8.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Sep-26 02:32 vineyard_dask-0.8.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      976 b- defN 22-Sep-26 02:32 vineyard_dask-0.8.6.dist-info/RECORD
-11 files, 97114 bytes uncompressed, 19773 bytes compressed:  79.6%
+Zip file size: 21450 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      650 b- defN 22-Sep-28 08:01 vineyard/contrib/dask/__init__.py
+-rw-r--r--  2.0 unx     5125 b- defN 22-Sep-28 08:01 vineyard/contrib/dask/dask.py
+-rw-r--r--  2.0 unx      650 b- defN 22-Sep-28 08:01 vineyard/contrib/dask/tests/__init__.py
+-rw-r--r--  2.0 unx      735 b- defN 22-Sep-28 08:01 vineyard/contrib/dask/tests/conftest.py
+-rw-r--r--  2.0 unx     5329 b- defN 22-Sep-28 08:01 vineyard/contrib/dask/tests/test_dask.py
+-rw-r--r--  2.0 unx    63232 b- defN 22-Sep-28 08:30 vineyard_dask-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18247 b- defN 22-Sep-28 08:30 vineyard_dask-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx     2068 b- defN 22-Sep-28 08:30 vineyard_dask-0.9.0.dist-info/NOTICE.txt
+-rw-r--r--  2.0 unx       93 b- defN 22-Sep-28 08:30 vineyard_dask-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 22-Sep-28 08:30 vineyard_dask-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      976 b- defN 22-Sep-28 08:30 vineyard_dask-0.9.0.dist-info/RECORD
+11 files, 97114 bytes uncompressed, 19774 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: vineyard/contrib/dask/tests/conftest.py
 Comment: 
 
 Filename: vineyard/contrib/dask/tests/test_dask.py
 Comment: 
 
-Filename: vineyard_dask-0.8.6.dist-info/LICENSE
+Filename: vineyard_dask-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: vineyard_dask-0.8.6.dist-info/METADATA
+Filename: vineyard_dask-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: vineyard_dask-0.8.6.dist-info/NOTICE.txt
+Filename: vineyard_dask-0.9.0.dist-info/NOTICE.txt
 Comment: 
 
-Filename: vineyard_dask-0.8.6.dist-info/WHEEL
+Filename: vineyard_dask-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: vineyard_dask-0.8.6.dist-info/top_level.txt
+Filename: vineyard_dask-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vineyard_dask-0.8.6.dist-info/RECORD
+Filename: vineyard_dask-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vineyard_dask-0.8.6.dist-info/LICENSE` & `vineyard_dask-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vineyard_dask-0.8.6.dist-info/METADATA` & `vineyard_dask-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vineyard-dask
-Version: 0.8.6
+Version: 0.9.0
 Summary: Vineyard integration with Dask
 Home-page: https://v6d.io
 Author: The vineyard team
 Author-email: developers@v6d.io
 License: Apache License 2.0
 Project-URL: Documentation, https://v6d.io
 Project-URL: Source, https://github.com/v6d-io/v6d
```

## Comparing `vineyard_dask-0.8.6.dist-info/NOTICE.txt` & `vineyard_dask-0.9.0.dist-info/NOTICE.txt`

 * *Files identical despite different names*

## Comparing `vineyard_dask-0.8.6.dist-info/RECORD` & `vineyard_dask-0.9.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 vineyard/contrib/dask/__init__.py,sha256=_0yOizmKx9a303beW2e7us-ccMusdwRyiVcNAolQZe8,650
 vineyard/contrib/dask/dask.py,sha256=MwCNaCeqrM0FTii-96PiLrUwvqciZn9CeXBXgoW2jnk,5125
 vineyard/contrib/dask/tests/__init__.py,sha256=_0yOizmKx9a303beW2e7us-ccMusdwRyiVcNAolQZe8,650
 vineyard/contrib/dask/tests/conftest.py,sha256=rJNw5QD4rkyIG_uNHnFzKm6gCikOrCmKxr7a14dQ5GA,735
 vineyard/contrib/dask/tests/test_dask.py,sha256=vbtpOOsK4dw4fnRCijUZVtcnBrXO7NA4Xjgr3gX2DNA,5329
-vineyard_dask-0.8.6.dist-info/LICENSE,sha256=AO754ryHkzyqDpd_eYB59Jdofwxj_FIm999rrBhFqwk,63232
-vineyard_dask-0.8.6.dist-info/METADATA,sha256=AYeFLcNs_7znsX22KCesNdwQTt79I6ZkBgzEvq7HvY4,18247
-vineyard_dask-0.8.6.dist-info/NOTICE.txt,sha256=CpvNDiG8l4g1bbhN--L33Abkv4QLO3-T7tEe6-8HdW8,2068
-vineyard_dask-0.8.6.dist-info/WHEEL,sha256=7S85KtyFD8rVLcRtbU_ImUEvhGsQLjg2zj19rOEAGNM,93
-vineyard_dask-0.8.6.dist-info/top_level.txt,sha256=eZrYkLRbDypCZAYVfMwFNTMYj4dRG-c-6B5uV6vu4Sk,9
-vineyard_dask-0.8.6.dist-info/RECORD,,
+vineyard_dask-0.9.0.dist-info/LICENSE,sha256=AO754ryHkzyqDpd_eYB59Jdofwxj_FIm999rrBhFqwk,63232
+vineyard_dask-0.9.0.dist-info/METADATA,sha256=SisGegU4TXWtyUR7Ph4fdEDtDprTUOEK2rjIw65OHxw,18247
+vineyard_dask-0.9.0.dist-info/NOTICE.txt,sha256=CpvNDiG8l4g1bbhN--L33Abkv4QLO3-T7tEe6-8HdW8,2068
+vineyard_dask-0.9.0.dist-info/WHEEL,sha256=7S85KtyFD8rVLcRtbU_ImUEvhGsQLjg2zj19rOEAGNM,93
+vineyard_dask-0.9.0.dist-info/top_level.txt,sha256=eZrYkLRbDypCZAYVfMwFNTMYj4dRG-c-6B5uV6vu4Sk,9
+vineyard_dask-0.9.0.dist-info/RECORD,,
```

