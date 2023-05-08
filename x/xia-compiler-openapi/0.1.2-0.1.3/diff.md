# Comparing `tmp/xia_compiler_openapi-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_openapi-0.1.3-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 222882 bytes, number of entries: 7
--rw-r--r--  2.0 unx      126 b- defN 23-Apr-23 11:49 xia_compiler_openapi/__init__.py
--rw-r--r--  2.0 unx   620544 b- defN 23-Apr-23 11:56 xia_compiler_openapi/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      695 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      648 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/RECORD
-7 files, 622285 bytes uncompressed, 221712 bytes compressed:  64.4%
+Zip file size: 181334 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      126 b- defN 23-May-08 08:57 xia_compiler_openapi/__init__.py
+-rw-r--r--  2.0 unx   507200 b- defN 23-May-08 08:57 xia_compiler_openapi/compiler.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      150 b- defN 23-May-08 08:57 xia_compiler_openapi-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      658 b- defN 23-May-08 08:57 xia_compiler_openapi-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-08 08:57 xia_compiler_openapi-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-08 08:57 xia_compiler_openapi-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      652 b- defN 23-May-08 08:57 xia_compiler_openapi-0.1.3.dist-info/RECORD
+7 files, 508915 bytes uncompressed, 180158 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_openapi/__init__.py
 Comment: 
 
-Filename: xia_compiler_openapi/compiler.cp39-win_amd64.pyd
+Filename: xia_compiler_openapi/compiler.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.2.dist-info/LICENSE.txt
+Filename: xia_compiler_openapi-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.2.dist-info/METADATA
+Filename: xia_compiler_openapi-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.2.dist-info/WHEEL
+Filename: xia_compiler_openapi-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.2.dist-info/top_level.txt
+Filename: xia_compiler_openapi-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.2.dist-info/RECORD
+Filename: xia_compiler_openapi-0.1.3.dist-info/RECORD
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
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_compiler_openapi-0.1.2.dist-info/METADATA` & `xia_compiler_openapi-0.1.3.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-compiler-openapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-api
 
 .. image:: https://img.shields.io/pypi/v/xia-compiler-openapi.svg?color=blue
    :alt: PyPI-Server
@@ -26,9 +24,7 @@
 =============================
 
 Install the package::
 
     pip install xia-compiler-openai
 
 
-
-
```

## Comparing `xia_compiler_openapi-0.1.2.dist-info/RECORD` & `xia_compiler_openapi-0.1.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_openapi/__init__.py,sha256=-dE50s7Ppx66LRhMtlDLJtVjeYwkH8Fzg-lsQ6kyTn0,126
-xia_compiler_openapi/compiler.cp39-win_amd64.pyd,sha256=PR9oDoY8i3F7DixUy3bG9eZfsDvmne7_IUfFLXJNdC0,620544
-xia_compiler_openapi-0.1.2.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_compiler_openapi-0.1.2.dist-info/METADATA,sha256=BF0bqAQUpYhayB1ThyWvbta2ttxNr7SmZTbD-rcUvqY,695
-xia_compiler_openapi-0.1.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_compiler_openapi-0.1.2.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
-xia_compiler_openapi-0.1.2.dist-info/RECORD,,
+xia_compiler_openapi/__init__.py,sha256=z0yw_NMiCx4km8HpM_v-35AluV9BcCj3yTg4lTHOsm0,126
+xia_compiler_openapi/compiler.cpython-310-darwin.so,sha256=BO_vejIFxJJ6mdRGUeEnEam-Imoyvk57qhUSSu-2klw,507200
+xia_compiler_openapi-0.1.3.dist-info/LICENSE.txt,sha256=6lRgf9k2ZgrG5cDYuhNoHP6c9esKOIPd28rlbHJdX-g,150
+xia_compiler_openapi-0.1.3.dist-info/METADATA,sha256=YH4zjoB2ZWs3-HX2aajdksIri9JmdL4rIknYpCbi8ag,658
+xia_compiler_openapi-0.1.3.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_compiler_openapi-0.1.3.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
+xia_compiler_openapi-0.1.3.dist-info/RECORD,,
```

