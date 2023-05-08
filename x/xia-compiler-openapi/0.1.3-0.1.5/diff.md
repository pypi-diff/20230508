# Comparing `tmp/xia_compiler_openapi-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_openapi-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 222880 bytes, number of entries: 7
--rw-r--r--  2.0 unx      126 b- defN 23-May-08 08:56 xia_compiler_openapi/__init__.py
--rw-r--r--  2.0 unx   620544 b- defN 23-May-08 08:59 xia_compiler_openapi/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-08 08:59 xia_compiler_openapi-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      695 b- defN 23-May-08 08:59 xia_compiler_openapi-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-08 08:59 xia_compiler_openapi-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-08 08:59 xia_compiler_openapi-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      648 b- defN 23-May-08 08:59 xia_compiler_openapi-0.1.3.dist-info/RECORD
-7 files, 622283 bytes uncompressed, 221710 bytes compressed:  64.4%
+Zip file size: 237762 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      126 b- defN 23-May-08 19:53 xia_compiler_openapi/__init__.py
+-rw-r--r--  2.0 unx   663552 b- defN 23-May-08 19:56 xia_compiler_openapi/compiler.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-08 19:56 xia_compiler_openapi-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      695 b- defN 23-May-08 19:56 xia_compiler_openapi-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-08 19:56 xia_compiler_openapi-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-08 19:56 xia_compiler_openapi-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      648 b- defN 23-May-08 19:56 xia_compiler_openapi-0.1.5.dist-info/RECORD
+7 files, 665291 bytes uncompressed, 236592 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_openapi/__init__.py
 Comment: 
 
 Filename: xia_compiler_openapi/compiler.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.3.dist-info/LICENSE.txt
+Filename: xia_compiler_openapi-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.3.dist-info/METADATA
+Filename: xia_compiler_openapi-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.3.dist-info/WHEEL
+Filename: xia_compiler_openapi-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.3.dist-info/top_level.txt
+Filename: xia_compiler_openapi-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.3.dist-info/RECORD
+Filename: xia_compiler_openapi-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_openapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_openapi.compiler import XiaCompilerOpenapi
 
 
 __all__ = [
     "XiaCompilerOpenapi",
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.5"
```

## Comparing `xia_compiler_openapi-0.1.3.dist-info/METADATA` & `xia_compiler_openapi-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-openapi
-Version: 0.1.3
+Version: 0.1.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_compiler_openapi-0.1.3.dist-info/RECORD` & `xia_compiler_openapi-0.1.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_openapi/__init__.py,sha256=z0yw_NMiCx4km8HpM_v-35AluV9BcCj3yTg4lTHOsm0,126
-xia_compiler_openapi/compiler.cp39-win_amd64.pyd,sha256=L2IZpV-WZXW-cJg-UV83F5GfJj0YCGEX1sLvqmMyfjI,620544
-xia_compiler_openapi-0.1.3.dist-info/LICENSE.txt,sha256=6lRgf9k2ZgrG5cDYuhNoHP6c9esKOIPd28rlbHJdX-g,150
-xia_compiler_openapi-0.1.3.dist-info/METADATA,sha256=Nkv95Th7Ap36S6dNvZrSaHRwsTcWYlO2ZH-E-TGwlRU,695
-xia_compiler_openapi-0.1.3.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_compiler_openapi-0.1.3.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
-xia_compiler_openapi-0.1.3.dist-info/RECORD,,
+xia_compiler_openapi/__init__.py,sha256=u9x1LUPIXf5dDlfrCl1gRFFu-8QcuYMoVkGfpgUDNI8,126
+xia_compiler_openapi/compiler.cp39-win_amd64.pyd,sha256=IY2KgLog3kbtR8XyF4EJy7sVLgB8MtarvcWCjHl6F7o,663552
+xia_compiler_openapi-0.1.5.dist-info/LICENSE.txt,sha256=6lRgf9k2ZgrG5cDYuhNoHP6c9esKOIPd28rlbHJdX-g,150
+xia_compiler_openapi-0.1.5.dist-info/METADATA,sha256=6xPME8HYOZc1T3pWCp1f49clnIilSwEsohTieAHRyEI,695
+xia_compiler_openapi-0.1.5.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_compiler_openapi-0.1.5.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
+xia_compiler_openapi-0.1.5.dist-info/RECORD,,
```

