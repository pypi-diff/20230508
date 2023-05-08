# Comparing `tmp/fovus-1.0.0-py3-none-any.whl.zip` & `tmp/fovus-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -7,15 +7,15 @@
 -rw-r--r--  2.0 unx     8348 b- defN 23-Apr-05 06:40 fovus/adapter/fovus_s3_adapter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/cli/__init__.py
 -rw-r--r--  2.0 unx    13184 b- defN 23-Apr-05 06:40 fovus/cli/cli_action_runner.py
 -rw-r--r--  2.0 unx      161 b- defN 23-Apr-05 06:56 fovus/cli/documenter.py
 -rw-r--r--  2.0 unx      475 b- defN 23-Apr-05 06:40 fovus/cli/fovus_cli.py
 -rw-r--r--  2.0 unx    24001 b- defN 23-Apr-13 20:39 fovus/cli/fovus_cli_argument_parser.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/config/__init__.py
--rw-r--r--  2.0 unx      138 b- defN 23-Apr-13 20:39 fovus/config/config.py
+-rw-r--r--  2.0 unx      138 b- defN 23-May-08 15:59 fovus/config/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/constants/__init__.py
 -rw-r--r--  2.0 unx       59 b- defN 23-Apr-05 06:40 fovus/constants/cli_action_runner_constants.py
 -rw-r--r--  2.0 unx     8309 b- defN 23-Apr-05 06:40 fovus/constants/cli_constants.py
 -rw-r--r--  2.0 unx     1446 b- defN 23-Apr-05 06:40 fovus/constants/fovus_api_constants.py
 -rw-r--r--  2.0 unx      194 b- defN 23-Apr-05 06:40 fovus/constants/util_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/exception/__init__.py
 -rw-r--r--  2.0 unx      291 b- defN 23-Apr-05 06:40 fovus/exception/status_code_exception.py
@@ -35,14 +35,14 @@
 -rw-r--r--  2.0 unx     4208 b- defN 23-Apr-05 06:40 fovus/util/file_util.py
 -rw-r--r--  2.0 unx     2871 b- defN 23-Apr-05 06:40 fovus/util/fovus_api_util.py
 -rw-r--r--  2.0 unx     1740 b- defN 23-Apr-05 06:40 fovus/util/fovus_cli_argument_parser_util.py
 -rw-r--r--  2.0 unx     1519 b- defN 23-Apr-05 06:40 fovus/util/fovus_s3_adapter_util.py
 -rw-r--r--  2.0 unx      533 b- defN 23-Apr-05 06:40 fovus/util/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/validator/__init__.py
 -rw-r--r--  2.0 unx     2914 b- defN 23-Apr-05 06:40 fovus/validator/fovus_api_validator.py
--rw-r--r--  2.0 unx    14101 b- defN 23-Apr-13 20:41 fovus-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8883 b- defN 23-Apr-13 20:41 fovus-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 20:41 fovus-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-13 20:41 fovus-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-13 20:41 fovus-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4089 b- defN 23-Apr-13 20:41 fovus-1.0.0.dist-info/RECORD
+-rw-r--r--  2.0 unx    14101 b- defN 23-May-08 16:01 fovus-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8883 b- defN 23-May-08 16:01 fovus-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 16:01 fovus-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-May-08 16:01 fovus-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-08 16:01 fovus-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4089 b- defN 23-May-08 16:01 fovus-1.0.1.dist-info/RECORD
 46 files, 131126 bytes uncompressed, 36705 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -114,26 +114,26 @@
 
 Filename: fovus/validator/__init__.py
 Comment: 
 
 Filename: fovus/validator/fovus_api_validator.py
 Comment: 
 
-Filename: fovus-1.0.0.dist-info/LICENSE.txt
+Filename: fovus-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fovus-1.0.0.dist-info/METADATA
+Filename: fovus-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: fovus-1.0.0.dist-info/WHEEL
+Filename: fovus-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: fovus-1.0.0.dist-info/entry_points.txt
+Filename: fovus-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: fovus-1.0.0.dist-info/top_level.txt
+Filename: fovus-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fovus-1.0.0.dist-info/RECORD
+Filename: fovus-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fovus-1.0.0.dist-info/LICENSE.txt` & `fovus-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fovus-1.0.0.dist-info/METADATA` & `fovus-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fovus
-Version: 1.0.0
+Version: 1.0.1
 Summary: The Fovus Python CLI
 Author: Fovus Corporation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: boto3 (>=1.26.60)
 Requires-Dist: jsonschema (>=3.2.0)
```

## Comparing `fovus-1.0.0.dist-info/RECORD` & `fovus-1.0.1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
 fovus/util/file_util.py,sha256=RK-2wtW4bFRNXZ79NgbfWceofxJV59sudr8-0-ewpmM,4208
 fovus/util/fovus_api_util.py,sha256=7Auhoqjh0drGODn9U4zWG6e2eXlvCvRiuqQDpQCZz2A,2871
 fovus/util/fovus_cli_argument_parser_util.py,sha256=kuVUIibYr_9crVH34aX-MotOwj_KBBt8R_bbbrEmiIw,1740
 fovus/util/fovus_s3_adapter_util.py,sha256=WQwqgaeVttAUTJ2MyO9KFXpaIsVFwzcUM3K6xZ5oeFU,1519
 fovus/util/util.py,sha256=i_mzAJDsIvvWEEOTVGYckYZInZe6EddwyJiiVQca7R4,533
 fovus/validator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/validator/fovus_api_validator.py,sha256=AYPynKV5WHrdKhrlBINl2LHPg17qoSeTBtcIP1OtcMc,2914
-fovus-1.0.0.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
-fovus-1.0.0.dist-info/METADATA,sha256=OPcJYmaNX4tlnKK2tI6sMXt_Cxcx0rdQ_3z3i0xWA78,8883
-fovus-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fovus-1.0.0.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
-fovus-1.0.0.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
-fovus-1.0.0.dist-info/RECORD,,
+fovus-1.0.1.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
+fovus-1.0.1.dist-info/METADATA,sha256=-clHPzp9B5Ye-pScg9Xp6Lt6ZPnK5J6B07DigIWXJYw,8883
+fovus-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fovus-1.0.1.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
+fovus-1.0.1.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
+fovus-1.0.1.dist-info/RECORD,,
```

