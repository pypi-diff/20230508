# Comparing `tmp/nexus_api-2.0.0b8-py3-none-any.whl.zip` & `tmp/nexus_api-2.0.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 14072 bytes, number of entries: 6
--rw-r--r--  2.0 unx       26 b- defN 23-Apr-24 12:59 nexus_api/__init__.py
--rw-r--r--  2.0 unx   104006 b- defN 23-Apr-24 12:59 nexus_api/_nexus_api.py
--rw-r--r--  2.0 unx      658 b- defN 23-Apr-24 13:03 nexus_api-2.0.0b8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 13:03 nexus_api-2.0.0b8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-24 13:03 nexus_api-2.0.0b8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      471 b- defN 23-Apr-24 13:03 nexus_api-2.0.0b8.dist-info/RECORD
+-rw-r--r--  2.0 unx       26 b- defN 23-Apr-25 12:02 nexus_api/__init__.py
+-rw-r--r--  2.0 unx   104006 b- defN 23-Apr-25 12:02 nexus_api/_nexus_api.py
+-rw-r--r--  2.0 unx      658 b- defN 23-Apr-25 12:07 nexus_api-2.0.0b9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 12:07 nexus_api-2.0.0b9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-25 12:07 nexus_api-2.0.0b9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      471 b- defN 23-Apr-25 12:07 nexus_api-2.0.0b9.dist-info/RECORD
 6 files, 105263 bytes uncompressed, 13218 bytes compressed:  87.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: nexus_api/__init__.py
 Comment: 
 
 Filename: nexus_api/_nexus_api.py
 Comment: 
 
-Filename: nexus_api-2.0.0b8.dist-info/METADATA
+Filename: nexus_api-2.0.0b9.dist-info/METADATA
 Comment: 
 
-Filename: nexus_api-2.0.0b8.dist-info/WHEEL
+Filename: nexus_api-2.0.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: nexus_api-2.0.0b8.dist-info/top_level.txt
+Filename: nexus_api-2.0.0b9.dist-info/top_level.txt
 Comment: 
 
-Filename: nexus_api-2.0.0b8.dist-info/RECORD
+Filename: nexus_api-2.0.0b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nexus_api-2.0.0b8.dist-info/METADATA` & `nexus_api-2.0.0b9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-api
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Client for the Nexus system.
 Home-page: https://github.com/malstroem-labs/nexus
 Author: https://github.com/malstroem-labs
 License: MIT
 Project-URL: Project, https://malstroem-labs.github.io/Nexus
 Project-URL: Repository, https://github.com/malstroem-labs/nexus
 Keywords: Nexus time-series data lake
```

