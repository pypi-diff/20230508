# Comparing `tmp/souJpg_comm-1.0.6-py3-none-any.whl.zip` & `tmp/souJpg_comm-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 47522 bytes, number of entries: 45
+Zip file size: 47527 bytes, number of entries: 45
 -rw-r--r--  2.0 unx      505 b- defN 23-May-07 01:53 souJpg/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 00:48 souJpg/comm/__init__.py
 -rw-r--r--  2.0 unx     2645 b- defN 23-May-01 00:48 souJpg/comm/apiResponse.py
 -rw-r--r--  2.0 unx     1603 b- defN 23-May-01 00:48 souJpg/comm/contextManagers.py
 -rw-r--r--  2.0 unx     2026 b- defN 23-May-01 01:13 souJpg/comm/cos.py
 -rw-r--r--  2.0 unx     1383 b- defN 23-May-01 02:47 souJpg/comm/dbHelper.py
 -rw-r--r--  2.0 unx     3816 b- defN 23-May-01 01:03 souJpg/comm/dbsCL.py
@@ -36,12 +36,12 @@
 -rw-r--r--  2.0 unx     9783 b- defN 23-May-01 02:47 souJpg/comm/fs/distributeFs.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 00:48 souJpg/comm/ops/__init__.py
 -rw-r--r--  2.0 unx     7783 b- defN 23-May-01 00:48 souJpg/comm/ops/ops.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 00:48 souJpg/comm/ops/test/__init__.py
 -rw-r--r--  2.0 unx     6989 b- defN 23-May-01 01:12 souJpg/comm/ops/test/test.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 00:48 souJpg/comm/test/__init__.py
 -rw-r--r--  2.0 unx    21234 b- defN 23-May-07 01:40 souJpg/comm/test/test.py
--rw-r--r--  2.0 unx     2721 b- defN 23-May-08 02:10 souJpg_comm-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 02:10 souJpg_comm-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-08 02:10 souJpg_comm-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3658 b- defN 23-May-08 02:10 souJpg_comm-1.0.6.dist-info/RECORD
-45 files, 155153 bytes uncompressed, 41714 bytes compressed:  73.1%
+-rw-r--r--  2.0 unx     2723 b- defN 23-May-08 02:13 souJpg_comm-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 02:13 souJpg_comm-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-08 02:13 souJpg_comm-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3658 b- defN 23-May-08 02:13 souJpg_comm-1.0.7.dist-info/RECORD
+45 files, 155155 bytes uncompressed, 41719 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -117,20 +117,20 @@
 
 Filename: souJpg/comm/test/__init__.py
 Comment: 
 
 Filename: souJpg/comm/test/test.py
 Comment: 
 
-Filename: souJpg_comm-1.0.6.dist-info/METADATA
+Filename: souJpg_comm-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: souJpg_comm-1.0.6.dist-info/WHEEL
+Filename: souJpg_comm-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: souJpg_comm-1.0.6.dist-info/top_level.txt
+Filename: souJpg_comm-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: souJpg_comm-1.0.6.dist-info/RECORD
+Filename: souJpg_comm-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `souJpg_comm-1.0.6.dist-info/METADATA` & `souJpg_comm-1.0.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: souJpg-comm
-Version: 1.0.6
+Version: 1.0.7
 Summary: souJpg-comm
 Home-page: 
 Author: zhaoyufei
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.80
+Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 Requires-Dist: mysql-connector-python
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: pymongo
 Requires-Dist: PyYAML
 Requires-Dist: selectivesearch
```

## Comparing `souJpg_comm-1.0.6.dist-info/RECORD` & `souJpg_comm-1.0.7.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -35,11 +35,11 @@
 souJpg/comm/fs/distributeFs.py,sha256=A0u0qLs45eJWVn9-H_eGt3rojDBB1GChRtoFW7bj8iI,9783
 souJpg/comm/ops/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 souJpg/comm/ops/ops.py,sha256=HQAmz_bJ449YByogkkwq56dHUBoGrTG6oo45_OZ4E_4,7783
 souJpg/comm/ops/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 souJpg/comm/ops/test/test.py,sha256=9zZojTrnw_5EE0K_8cAFwznKKZ1qvJgCo1Qmtb1WYNI,6989
 souJpg/comm/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 souJpg/comm/test/test.py,sha256=IH_D86gJst9IdAspR8sB0--MXS9fMt0MO11eakpceS0,21234
-souJpg_comm-1.0.6.dist-info/METADATA,sha256=-ZwUO-mKPgvv027B0zJpOGHbOzvLeTUF5SRcOEf0_r8,2721
-souJpg_comm-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-souJpg_comm-1.0.6.dist-info/top_level.txt,sha256=pfOQRG1ECW8irsyGTyFOJxdejDSy3IufYfr8R2RHd1c,7
-souJpg_comm-1.0.6.dist-info/RECORD,,
+souJpg_comm-1.0.7.dist-info/METADATA,sha256=uwzmcUd0NzfMcWyCorhgww14mH8XQkvnSMJE2i5Y57w,2723
+souJpg_comm-1.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+souJpg_comm-1.0.7.dist-info/top_level.txt,sha256=pfOQRG1ECW8irsyGTyFOJxdejDSy3IufYfr8R2RHd1c,7
+souJpg_comm-1.0.7.dist-info/RECORD,,
```

