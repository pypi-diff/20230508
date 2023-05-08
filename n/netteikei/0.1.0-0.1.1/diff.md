# Comparing `tmp/netteikei-0.1.0-py3-none-any.whl.zip` & `tmp/netteikei-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6485 bytes, number of entries: 12
--rw-------  2.0 unx       64 b- defN 23-May-07 15:22 netteikei/__init__.py
--rw-------  2.0 unx     2801 b- defN 23-May-07 17:27 netteikei/core.py
+Zip file size: 6519 bytes, number of entries: 12
+-rw-------  2.0 unx       64 b- defN 23-May-08 13:50 netteikei/__init__.py
+-rw-------  2.0 unx     2801 b- defN 23-May-08 13:39 netteikei/core.py
 -rw-------  2.0 unx        0 b- defN 23-May-07 09:41 netteikei/py.typed
--rw-------  2.0 unx     1055 b- defN 23-May-07 13:44 netteikei/typedefs.py
+-rw-------  2.0 unx     1055 b- defN 23-May-08 13:39 netteikei/typedefs.py
 -rw-------  2.0 unx        0 b- defN 23-May-07 13:53 netteikei/contrib/__init__.py
--rw-------  2.0 unx     2487 b- defN 23-May-07 17:38 netteikei/contrib/download.py
--rw-------  2.0 unx     1144 b- defN 23-May-07 13:53 netteikei/contrib/utils.py
--rw-------  2.0 unx     1068 b- defN 23-May-07 18:08 netteikei-0.1.0.dist-info/LICENSE
--rw-------  2.0 unx     1165 b- defN 23-May-07 18:08 netteikei-0.1.0.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 23-May-07 18:08 netteikei-0.1.0.dist-info/WHEEL
--rw-------  2.0 unx       10 b- defN 23-May-07 18:08 netteikei-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      948 b- defN 23-May-07 18:08 netteikei-0.1.0.dist-info/RECORD
-12 files, 10834 bytes uncompressed, 4891 bytes compressed:  54.9%
+-rw-------  2.0 unx     2487 b- defN 23-May-08 13:39 netteikei/contrib/download.py
+-rw-------  2.0 unx     1144 b- defN 23-May-08 13:39 netteikei/contrib/utils.py
+-rw-------  2.0 unx     1068 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/LICENSE
+-rw-------  2.0 unx     1325 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/WHEEL
+-rw-------  2.0 unx       10 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      948 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/RECORD
+12 files, 10994 bytes uncompressed, 4925 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: netteikei/contrib/download.py
 Comment: 
 
 Filename: netteikei/contrib/utils.py
 Comment: 
 
-Filename: netteikei-0.1.0.dist-info/LICENSE
+Filename: netteikei-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: netteikei-0.1.0.dist-info/METADATA
+Filename: netteikei-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: netteikei-0.1.0.dist-info/WHEEL
+Filename: netteikei-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: netteikei-0.1.0.dist-info/top_level.txt
+Filename: netteikei-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: netteikei-0.1.0.dist-info/RECORD
+Filename: netteikei-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netteikei/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 from .core import Client, RequestHandler
```

## Comparing `netteikei-0.1.0.dist-info/LICENSE` & `netteikei-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netteikei-0.1.0.dist-info/METADATA` & `netteikei-0.1.1.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netteikei
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility library for making concurrent HTTP requests using aiohttp
 Home-page: https://github.com/fernofsigma/netteikei
 Author: FernOfSigma
 Author-email: fernofsigma@tuta.io
 License: MIT
 Project-URL: GitHub: issues, https://github.com/fernofsigma/netteikei/issues
 Project-URL: GitHub: repo, https://github.com/fernofsigma/netteikei
@@ -21,10 +21,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 License-File: LICENSE
 Requires-Dist: aiohttp (<4.0.0,>=3.8.4)
+Provides-Extra: download
+Requires-Dist: aiofiles ; extra == 'download'
+Requires-Dist: pyrfc6266 ; extra == 'download'
+Requires-Dist: tqdm ; extra == 'download'
 Provides-Extra: speedups
 Requires-Dist: aiohttp[speedups] ; extra == 'speedups'
```

## Comparing `netteikei-0.1.0.dist-info/RECORD` & `netteikei-0.1.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-netteikei/__init__.py,sha256=mqVGWjMOswuf39bYez1fKggybZ2PLGp6TN903Hk7T94,64
+netteikei/__init__.py,sha256=Q5RWyjANksYTANd5T034RArj6BC9pTRauz-ud9U5VjY,64
 netteikei/core.py,sha256=et2XxAkQhs4QSkbBEfH811BJ7QqakxbLwiO_1qJnCcw,2801
 netteikei/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netteikei/typedefs.py,sha256=UjwEfJvuwJ0693C5OQ8Eg-bivCQbWwwJ5cB0I-ULYXI,1055
 netteikei/contrib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netteikei/contrib/download.py,sha256=l2GEBdBCWBqfgVPQ41fF94nKSGU91wT44ZYXlxVgFTk,2487
 netteikei/contrib/utils.py,sha256=JDqp5rH9fb1nBejde0_0sNQpRsK1BoqMeV46371-zCI,1144
-netteikei-0.1.0.dist-info/LICENSE,sha256=37AgUwjy1RqDbLVahc_zXbHKIRzTEKjlDpKfzB6a-6g,1068
-netteikei-0.1.0.dist-info/METADATA,sha256=B75xC9Fg-4dJRc9I9ll5ntRQGu_H_1RME7Rh-iYBC0A,1165
-netteikei-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-netteikei-0.1.0.dist-info/top_level.txt,sha256=1TkkZh-n9Ys0kU95kW0keVBeiiY87lC-pR-FF7FFGB0,10
-netteikei-0.1.0.dist-info/RECORD,,
+netteikei-0.1.1.dist-info/LICENSE,sha256=37AgUwjy1RqDbLVahc_zXbHKIRzTEKjlDpKfzB6a-6g,1068
+netteikei-0.1.1.dist-info/METADATA,sha256=JaE51vox1d1QfsBCrQdJcwdtfoEDsxCI1KzhSL6Kmbo,1325
+netteikei-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+netteikei-0.1.1.dist-info/top_level.txt,sha256=1TkkZh-n9Ys0kU95kW0keVBeiiY87lC-pR-FF7FFGB0,10
+netteikei-0.1.1.dist-info/RECORD,,
```

