# Comparing `tmp/askedith-0.9.6-py3-none-any.whl.zip` & `tmp/askedith-0.9.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 7255 bytes, number of entries: 7
--rw-r--r--  2.0 unx     1388 b- defN 23-Jan-01 01:20 askedith/__init__.py
--rw-r--r--  2.0 unx      203 b- defN 23-Jan-01 01:20 askedith/config.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Jan-01 01:20 askedith-0.9.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2495 b- defN 23-Jan-01 01:20 askedith-0.9.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-01 01:20 askedith-0.9.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jan-01 01:20 askedith-0.9.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      542 b- defN 23-Jan-01 01:20 askedith-0.9.6.dist-info/RECORD
+-rw-r--r--  2.0 unx     1388 b- defN 23-Jan-05 17:12 askedith/__init__.py
+-rw-r--r--  2.0 unx      203 b- defN 23-Jan-05 17:12 askedith/config.py
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Jan-05 17:12 askedith-0.9.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2495 b- defN 23-Jan-05 17:12 askedith-0.9.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-05 17:12 askedith-0.9.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jan-05 17:12 askedith-0.9.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      542 b- defN 23-Jan-05 17:12 askedith-0.9.7.dist-info/RECORD
 7 files, 16086 bytes uncompressed, 6297 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: askedith/__init__.py
 Comment: 
 
 Filename: askedith/config.py
 Comment: 
 
-Filename: askedith-0.9.6.dist-info/LICENSE
+Filename: askedith-0.9.7.dist-info/LICENSE
 Comment: 
 
-Filename: askedith-0.9.6.dist-info/METADATA
+Filename: askedith-0.9.7.dist-info/METADATA
 Comment: 
 
-Filename: askedith-0.9.6.dist-info/WHEEL
+Filename: askedith-0.9.7.dist-info/WHEEL
 Comment: 
 
-Filename: askedith-0.9.6.dist-info/top_level.txt
+Filename: askedith-0.9.7.dist-info/top_level.txt
 Comment: 
 
-Filename: askedith-0.9.6.dist-info/RECORD
+Filename: askedith-0.9.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `askedith-0.9.6.dist-info/LICENSE` & `askedith-0.9.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `askedith-0.9.6.dist-info/METADATA` & `askedith-0.9.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askedith
-Version: 0.9.6
+Version: 0.9.7
 Summary: Natural Language Query Engine for Pandas
 Home-page: https://askedith.ai
 Author: Jared Zhao
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -35,15 +35,15 @@
         <img
             src="https://img.shields.io/badge/Discord-Join-%237289DA?style=flat-square&logo=appveyor"
             alt="Badge"
         >
     </a>
     <a href="https://pypi.org/project/askedith/">
         <img
-            src="https://img.shields.io/badge/Release-0.9.6-blue?style=flat-square&logo=appveyor"
+            src="https://img.shields.io/badge/Release-0.9.7-blue?style=flat-square&logo=appveyor"
             alt="Badge"
         >
     </a>
     <a href="https://pypi.org/project/askedith/">
         <img
             src="https://img.shields.io/badge/CI%2FCD-passing-green?style=flat-square&logo=appveyor"
             alt="Badge"
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: askedith Version: 0.9.6 Summary: Natural Language
+Metadata-Version: 2.1 Name: askedith Version: 0.9.7 Summary: Natural Language
 Query Engine for Pandas Home-page: https://askedith.ai Author: Jared Zhao
 License: Apache 2.0 Platform: UNKNOWN Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
 (>=2.0.0) Requires-Dist: pandas
```

