# Comparing `tmp/sj_tool-1.0.8-py3-none-any.whl.zip` & `tmp/sj_tool-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 13138 bytes, number of entries: 29
+Zip file size: 13444 bytes, number of entries: 30
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:37 sj_tool/__init__.py
 -rw-rw-rw-  2.0 fat      226 b- defN 23-Apr-10 10:09 sj_tool/decorator.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email_sender.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Mar-14 09:42 sj_tool/file.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-04 05:43 sj_tool/json.py
+-rw-rw-rw-  2.0 fat      273 b- defN 23-Apr-23 03:10 sj_tool/language.py
 -rw-rw-rw-  2.0 fat      335 b- defN 23-Apr-14 09:33 sj_tool/parallel.py
 -rw-rw-rw-  2.0 fat     2180 b- defN 23-Apr-10 10:28 sj_tool/scheduler.py
 -rw-rw-rw-  2.0 fat      245 b- defN 23-Apr-04 05:43 sj_tool/system.py
 -rw-rw-rw-  2.0 fat     1002 b- defN 23-Apr-10 10:05 sj_tool/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:40 sj_tool/db/__init__.py
 -rw-rw-rw-  2.0 fat     5626 b- defN 23-Apr-08 09:02 sj_tool/db/mongo.py
 -rw-rw-rw-  2.0 fat     1237 b- defN 23-Apr-08 08:39 sj_tool/db/mysql.py
@@ -18,14 +19,14 @@
 -rw-rw-rw-  2.0 fat      897 b- defN 23-Apr-10 09:07 sj_tool/fjsp/entity/fjsp_pool.py
 -rw-rw-rw-  2.0 fat      897 b- defN 23-Apr-10 09:07 sj_tool/fjsp/entity/global_pool.py
 -rw-rw-rw-  2.0 fat      736 b- defN 23-Apr-15 11:54 sj_tool/fjsp/entity/job.py
 -rw-rw-rw-  2.0 fat      411 b- defN 23-Apr-09 05:22 sj_tool/fjsp/entity/machine.py
 -rw-rw-rw-  2.0 fat      829 b- defN 23-Apr-15 11:54 sj_tool/fjsp/entity/operation.py
 -rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-09 09:02 sj_tool/fjsp/entity/product.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-30 02:45 sj_tool/logger/__init__.py
--rw-rw-rw-  2.0 fat     2256 b- defN 23-Apr-19 09:16 sj_tool/logger/text_logger.py
+-rw-rw-rw-  2.0 fat     2250 b- defN 23-Apr-21 10:38 sj_tool/logger/text_logger.py
 -rw-rw-rw-  2.0 fat     2753 b- defN 23-Apr-19 09:41 sj_tool/logger/visual_logger.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-19 09:41 sj_tool-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 09:41 sj_tool-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-19 09:41 sj_tool-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2289 b- defN 23-Apr-19 09:41 sj_tool-1.0.8.dist-info/RECORD
-29 files, 24624 bytes uncompressed, 9462 bytes compressed:  61.6%
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-23 03:35 sj_tool-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 03:35 sj_tool-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-23 03:35 sj_tool-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2364 b- defN 23-Apr-23 03:35 sj_tool-1.0.9.dist-info/RECORD
+30 files, 24966 bytes uncompressed, 9654 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: sj_tool/file.py
 Comment: 
 
 Filename: sj_tool/json.py
 Comment: 
 
+Filename: sj_tool/language.py
+Comment: 
+
 Filename: sj_tool/parallel.py
 Comment: 
 
 Filename: sj_tool/scheduler.py
 Comment: 
 
 Filename: sj_tool/system.py
@@ -69,20 +72,20 @@
 
 Filename: sj_tool/logger/text_logger.py
 Comment: 
 
 Filename: sj_tool/logger/visual_logger.py
 Comment: 
 
-Filename: sj_tool-1.0.8.dist-info/METADATA
+Filename: sj_tool-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: sj_tool-1.0.8.dist-info/WHEEL
+Filename: sj_tool-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: sj_tool-1.0.8.dist-info/top_level.txt
+Filename: sj_tool-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sj_tool-1.0.8.dist-info/RECORD
+Filename: sj_tool-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sj_tool/logger/text_logger.py

```diff
@@ -37,15 +37,15 @@
 
 
 def init(level: str, save_log=True, logdir=None, comment="", filename="text.log", max_filesize=None) -> loguru.logger:
     """
     初始化日志框架
     :param level: 最低的日志level，如LogLevel.INFO
     :param save_log: 是否保存log到文件
-    :param logdir: 保存log到文件
+    :param logdir: 日志目录
     :param comment: log文件夹名后缀(仅在logdir为None时有效)
     :param filename: 日志文件名
     :param max_filesize: 最大文件大小
     :param replace: 是否替换已有文件（如果文件存在）
     :return:
     """
     logger.remove()
```

## Comparing `sj_tool-1.0.8.dist-info/RECORD` & `sj_tool-1.0.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 sj_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/decorator.py,sha256=nUTxQpiRjmV37SqojRz46vbYmV6N8-wbhF1tejJVeco,226
 sj_tool/email.py,sha256=qxNj5bQ31yzF1bi2XLIxJq5akw-vksZLOS9L5HdM5p8,476
 sj_tool/email_sender.py,sha256=qxNj5bQ31yzF1bi2XLIxJq5akw-vksZLOS9L5HdM5p8,476
 sj_tool/file.py,sha256=NsbZm_9UGni8CKoZEL9mMFwX7u2R2DXA-HtuUS1iaPw,155
 sj_tool/json.py,sha256=yG7paERY6nUtF51kz5ZXp396TKT-UgIyb0teAXeKD5Q,313
+sj_tool/language.py,sha256=jFRkGOrnHoIfGb3UDwzcMLa9XUYtif6KMg4k-1pbtUU,273
 sj_tool/parallel.py,sha256=ocC1AoHAZqSJToS-0o8DaxdANAsbJvRH-Y-wfmLt1PI,335
 sj_tool/scheduler.py,sha256=nSQm7feMCZ8SMeaOqQQ6KkFkwytWXHlMW1fVX7xHYU4,2180
 sj_tool/system.py,sha256=xQxxnAKZ8yW8LJZlw0MhpRyQ_p1LnqwlKnuwgiFdqgI,245
 sj_tool/util.py,sha256=oqnYmmzOa3dPRCNWSHDU_NziY7hODzi73A7xHQ6gcVw,1002
 sj_tool/db/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/db/mongo.py,sha256=oUDrhYV_sOq8M9KNFK_QDExCWQ070T1nksp8XzGtDs4,5626
 sj_tool/db/mysql.py,sha256=o9tidq_q9TkDbJXUb6KTMf9O9cJMZeL3rCsADCmroBQ,1237
@@ -17,13 +18,13 @@
 sj_tool/fjsp/entity/fjsp_pool.py,sha256=9-pE3_NIZqVWDM0TrGosycMfzaE1iQov8mSZ3-LZEPo,897
 sj_tool/fjsp/entity/global_pool.py,sha256=9-pE3_NIZqVWDM0TrGosycMfzaE1iQov8mSZ3-LZEPo,897
 sj_tool/fjsp/entity/job.py,sha256=r4DGShXcv-K6rnKn5602-X2t6bs3yE1nfcAd3qIMe28,736
 sj_tool/fjsp/entity/machine.py,sha256=zBjVt5VYEuJlqA4yHzzEw9wlbVSAaJHlgj0lweSNaSw,411
 sj_tool/fjsp/entity/operation.py,sha256=nJaMbjFyTJTGkjBg4yokXgwqldMkdbqs7psG-9d6nmo,829
 sj_tool/fjsp/entity/product.py,sha256=IzErQu-Hm0d8rSdWA3Z-HYaYBDmNUbyOMBumYc1dwuU,113
 sj_tool/logger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sj_tool/logger/text_logger.py,sha256=P_V4ABz7_PZ09PoaZzWuVk5bcrvlMuYwfEIQ026rdvA,2256
+sj_tool/logger/text_logger.py,sha256=ZGf91tWl78hCoggYL2GkExQwWGLQ9yTLSpPh_Lz6I7Q,2250
 sj_tool/logger/visual_logger.py,sha256=-OLn2lG2DUZiuSeTklO7h4sXHBeT6pXkN_tjfBeJBGE,2753
-sj_tool-1.0.8.dist-info/METADATA,sha256=M7ZCcAEY10e3dLOkU9_I13oopuJ6vVSsFG_VPvAqLgY,492
-sj_tool-1.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sj_tool-1.0.8.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
-sj_tool-1.0.8.dist-info/RECORD,,
+sj_tool-1.0.9.dist-info/METADATA,sha256=N0K5fu6vU2GJzw3w4mJ7IQz08RnYnPyzAeGAvGtQWeQ,492
+sj_tool-1.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sj_tool-1.0.9.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
+sj_tool-1.0.9.dist-info/RECORD,,
```

