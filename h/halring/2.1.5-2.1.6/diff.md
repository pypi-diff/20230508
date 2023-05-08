# Comparing `tmp/halring-2.1.5-py3-none-any.whl.zip` & `tmp/halring-2.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 142847 bytes, number of entries: 111
+Zip file size: 142864 bytes, number of entries: 111
 -rw-r--r--  2.0 unx      133 b- defN 23-Feb-22 02:05 halring/__init__.py
 -rw-r--r--  2.0 unx     2097 b- defN 23-Feb-07 10:16 halring/_unittest/666666.py
 -rw-r--r--  2.0 unx       52 b- defN 23-Feb-06 06:33 halring/_unittest/77777.py
 -rw-r--r--  2.0 unx       24 b- defN 23-Feb-15 07:13 halring/_unittest/__init__.py
 -rw-r--r--  2.0 unx     1572 b- defN 23-Feb-03 08:55 halring/_unittest/cty.py
 -rw-r--r--  2.0 unx     1556 b- defN 23-Feb-21 07:39 halring/_unittest/dk.py
 -rw-r--r--  2.0 unx    10373 b- defN 23-Feb-15 07:13 halring/_unittest/test_apollo_opr_util.py
@@ -101,13 +101,13 @@
 -rw-r--r--  2.0 unx    13521 b- defN 23-Feb-06 07:38 halring/svn/halring_svn.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-10 11:00 halring/windows/__init__.py
 -rw-r--r--  2.0 unx    18031 b- defN 23-Mar-01 05:15 halring/windows/halring_os.py
 -rw-r--r--  2.0 unx       23 b- defN 23-Jan-31 08:47 halring/windows_exec/__init__.py
 -rw-r--r--  2.0 unx     1292 b- defN 23-Feb-22 02:13 halring/windows_exec/halring_exec.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-10 11:00 halring/xml_lib/__init__.py
 -rw-r--r--  2.0 unx     3280 b- defN 23-Feb-15 07:18 halring/xml_lib/halring_xml.py
--rw-rw-r--  2.0 unx     1081 b- defN 23-May-08 05:26 halring-2.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    30444 b- defN 23-May-08 05:26 halring-2.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 05:26 halring-2.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-08 05:26 halring-2.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     9792 b- defN 23-May-08 05:26 halring-2.1.5.dist-info/RECORD
-111 files, 613302 bytes uncompressed, 127221 bytes compressed:  79.3%
+-rw-rw-r--  2.0 unx     1081 b- defN 23-May-08 09:09 halring-2.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    30509 b- defN 23-May-08 09:09 halring-2.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 09:09 halring-2.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-08 09:09 halring-2.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9792 b- defN 23-May-08 09:09 halring-2.1.6.dist-info/RECORD
+111 files, 613367 bytes uncompressed, 127238 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -312,23 +312,23 @@
 
 Filename: halring/xml_lib/__init__.py
 Comment: 
 
 Filename: halring/xml_lib/halring_xml.py
 Comment: 
 
-Filename: halring-2.1.5.dist-info/LICENSE
+Filename: halring-2.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: halring-2.1.5.dist-info/METADATA
+Filename: halring-2.1.6.dist-info/METADATA
 Comment: 
 
-Filename: halring-2.1.5.dist-info/WHEEL
+Filename: halring-2.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: halring-2.1.5.dist-info/top_level.txt
+Filename: halring-2.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: halring-2.1.5.dist-info/RECORD
+Filename: halring-2.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `halring-2.1.5.dist-info/LICENSE` & `halring-2.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `halring-2.1.5.dist-info/METADATA` & `halring-2.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halring
-Version: 2.1.5
+Version: 2.1.6
 Summary: python常用底层库封装
 Home-page: https://www.python.org
 Author: peixiaodong
 License: MIT Licence
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,16 @@
 Requires-Dist: chardet (==5.0.0)
 Requires-Dist: pymssql
 Requires-Dist: pika (==1.3.1)
 Requires-Dist: pandas (==1.1.5)
 Requires-Dist: urllib3 (==1.26.0)
 Requires-Dist: redis (==4.3.5)
 Requires-Dist: python-docx (==0.8.10)
+Requires-Dist: pypandoc (==1.11)
+Requires-Dist: pdfkit (==1.0.0)
 
 # halring
 **pip源配置方法confluence页面**  
 *http://eqops.tc.com/confluence/pages/viewpage.action?pageId=29300773*  
 ---
 **安装**:
 *pip install halring*
```

## Comparing `halring-2.1.5.dist-info/RECORD` & `halring-2.1.6.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -100,12 +100,12 @@
 halring/svn/halring_svn.py,sha256=4PbEEKzstKYGOoH03hVIKPKBsltt2oow06lt8UcZ_ak,13521
 halring/windows/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 halring/windows/halring_os.py,sha256=UxfnoMpuEYr1eKmb2hBh0TfneYHNuacUyxSYDtXKDfU,18031
 halring/windows_exec/__init__.py,sha256=-yYBDkgMDSHYf_F_uX23wZsDSjrudhppJvm34su8_I4,23
 halring/windows_exec/halring_exec.py,sha256=eNGSDpgQY00nRXhuKuqe_gNYhcnIXsoZqx9tCVAOYz0,1292
 halring/xml_lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 halring/xml_lib/halring_xml.py,sha256=iVmMxKlBG0wHWLuRyw80p7qyTrD8af9LD8MHjU1LqEM,3280
-halring-2.1.5.dist-info/LICENSE,sha256=yqFUGhMTJIiCb6lO2jZMqb7QsWUlTlga41Zs63k4hO8,1081
-halring-2.1.5.dist-info/METADATA,sha256=1S111dWSN4csnubV68EcMVWEY8H6tnpyNLECJxp1o6c,30444
-halring-2.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-halring-2.1.5.dist-info/top_level.txt,sha256=ERP_SRKUCSsvbZVXILxFESdERdLfSgMM_RKYdUJ52m4,8
-halring-2.1.5.dist-info/RECORD,,
+halring-2.1.6.dist-info/LICENSE,sha256=yqFUGhMTJIiCb6lO2jZMqb7QsWUlTlga41Zs63k4hO8,1081
+halring-2.1.6.dist-info/METADATA,sha256=iMGSPXDm7DPJXd9xpXpBYiBLFZHw0hefuEWULdReFoU,30509
+halring-2.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+halring-2.1.6.dist-info/top_level.txt,sha256=ERP_SRKUCSsvbZVXILxFESdERdLfSgMM_RKYdUJ52m4,8
+halring-2.1.6.dist-info/RECORD,,
```

