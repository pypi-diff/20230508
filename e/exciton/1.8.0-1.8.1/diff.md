# Comparing `tmp/exciton-1.8.0-py3-none-any.whl.zip` & `tmp/exciton-1.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 57718 bytes, number of entries: 60
+Zip file size: 57742 bytes, number of entries: 60
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/ml/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-26 00:50 exciton/ml/classification/__init__.py
 -rw-rw-r--  2.0 unx     1461 b- defN 23-Mar-26 01:24 exciton/ml/classification/utils.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Mar-26 03:49 exciton/ml/classification/bert/__init__.py
 -rw-rw-r--  2.0 unx     5860 b- defN 23-Mar-29 15:08 exciton/ml/classification/bert/model.py
 -rw-rw-r--  2.0 unx     1966 b- defN 23-Mar-29 14:55 exciton/ml/classification/bert/trainer.py
@@ -48,15 +48,15 @@
 -rw-rw-r--  2.0 unx       59 b- defN 23-May-05 01:21 exciton/nlp/sentence_tokenizer/__init__.py
 -rw-rw-r--  2.0 unx     4879 b- defN 23-May-07 10:31 exciton/nlp/sentence_tokenizer/exciton_sbd.py
 -rw-rw-r--  2.0 unx     3977 b- defN 23-May-02 03:18 exciton/nlp/sentence_tokenizer/service.py
 -rw-rw-r--  2.0 unx       84 b- defN 23-May-01 15:45 exciton/nlp/text_matching/__init__.py
 -rw-rw-r--  2.0 unx     2565 b- defN 23-May-08 00:57 exciton/nlp/text_matching/exciton_matching.py
 -rw-rw-r--  2.0 unx       50 b- defN 23-Mar-12 04:02 exciton/nlp/translation/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 23:23 exciton/nlp/translation/m2m100/__init__.py
--rw-rw-r--  2.0 unx     4525 b- defN 23-May-08 01:01 exciton/nlp/translation/m2m100/service.py
+-rw-rw-r--  2.0 unx     4718 b- defN 23-May-08 13:23 exciton/nlp/translation/m2m100/service.py
 -rw-rw-r--  2.0 unx     2172 b- defN 23-Mar-12 03:47 exciton/nlp/translation/m2m100/utils.py
--rw-r--r--  2.0 unx    11417 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1598 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5584 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/RECORD
-60 files, 153640 bytes uncompressed, 48608 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx    11417 b- defN 23-May-08 13:23 exciton-1.8.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1598 b- defN 23-May-08 13:23 exciton-1.8.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-08 13:23 exciton-1.8.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-May-08 13:23 exciton-1.8.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5584 b- defN 23-May-08 13:23 exciton-1.8.1.dist-info/RECORD
+60 files, 153833 bytes uncompressed, 48632 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -159,23 +159,23 @@
 
 Filename: exciton/nlp/translation/m2m100/service.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/utils.py
 Comment: 
 
-Filename: exciton-1.8.0.dist-info/LICENSE
+Filename: exciton-1.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: exciton-1.8.0.dist-info/METADATA
+Filename: exciton-1.8.1.dist-info/METADATA
 Comment: 
 
-Filename: exciton-1.8.0.dist-info/WHEEL
+Filename: exciton-1.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: exciton-1.8.0.dist-info/top_level.txt
+Filename: exciton-1.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: exciton-1.8.0.dist-info/RECORD
+Filename: exciton-1.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## exciton/nlp/translation/m2m100/service.py

```diff
@@ -97,23 +97,27 @@
         for batch in self._batch(source):
             sen_list = []
             target_prefix = []
             for itm in batch:
                 slang = itm["source_lang"]
                 tlang = itm["target_lang"]
                 if slang in self.lang_map and tlang in self.lang_map:
-                    slang = self.lang_map[slang]
-                    tlang = self.lang_map[tlang]
-                    self.tokenizer.src_lang = slang
-                    sen = self.tokenizer.encode(itm["source"])
-                    sen = self.tokenizer.convert_ids_to_tokens(sen)
-                    sen_list.append(sen)
-                    target_prefix.append([self.tokenizer.lang_code_to_token[tlang]])
+                    if isinstance(itm["source"], str):
+                        slang = self.lang_map[slang]
+                        tlang = self.lang_map[tlang]
+                        self.tokenizer.src_lang = slang
+                        sen = self.tokenizer.encode(itm["source"])
+                        sen = self.tokenizer.convert_ids_to_tokens(sen)
+                        sen_list.append(sen)
+                        target_prefix.append([self.tokenizer.lang_code_to_token[tlang]])
+                    else:
+                        itm["target"] = ""
+                        output.append(itm)
                 else:
-                    itm["target"] = None
+                    itm["target"] = ""
                     output.append(itm)
             results = self.translator.translate_batch(
                 sen_list,
                 target_prefix=target_prefix,
                 beam_size=3,
                 no_repeat_ngram_size=2,
                 repetition_penalty=1.2,
```

## Comparing `exciton-1.8.0.dist-info/LICENSE` & `exciton-1.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `exciton-1.8.0.dist-info/METADATA` & `exciton-1.8.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exciton
-Version: 1.8.0
+Version: 1.8.1
 Summary: Domain-specific Natural Language Processing with exciton
 Home-page: https://exciton.com
 Author: The ExcitonX Team
 Author-email: excitonx@gmail.com
 License: UNKNOWN
 Keywords: exciton NLP Deep Learning
 Platform: UNKNOWN
```

## Comparing `exciton-1.8.0.dist-info/RECORD` & `exciton-1.8.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,14 @@
 exciton/nlp/sentence_tokenizer/__init__.py,sha256=1hIgq6ayPk2yVdhBgLHe5vXxU2fcDrenz51iKXhx28s,59
 exciton/nlp/sentence_tokenizer/exciton_sbd.py,sha256=EG0kV16yXsv2EuYblN7kEVrN1FgoYTZTgAn7V7Cga7k,4879
 exciton/nlp/sentence_tokenizer/service.py,sha256=3Ssq2UNmhDCezhBJq4V8csacA_0XenYmgPLZfmBtBYc,3977
 exciton/nlp/text_matching/__init__.py,sha256=tgQvyWZupI0QAHlnLAJldpOPBCF01OFq2poLH49tAVg,84
 exciton/nlp/text_matching/exciton_matching.py,sha256=a99bzY5117DLAGb_AgV_4ai6buVYrMmyvengo18CeIU,2565
 exciton/nlp/translation/__init__.py,sha256=gE0YV-s4pB7VQWdsg04hALOBBpuWaQ3AUqpY9rvgI_8,50
 exciton/nlp/translation/m2m100/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-exciton/nlp/translation/m2m100/service.py,sha256=YbGM7sKTwAa8XkF54ZOKmx-3A0Yt7ZQ9OH1RmV_-vSo,4525
+exciton/nlp/translation/m2m100/service.py,sha256=FIXc5sUtZzywzis_CZ2doF6sqrPcKcyMO8EhLgFTwjY,4718
 exciton/nlp/translation/m2m100/utils.py,sha256=GE8qg2deaHBMVMIHS32Hb5TCxO453kuncQrdJsnRIoU,2172
-exciton-1.8.0.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
-exciton-1.8.0.dist-info/METADATA,sha256=XVGgE_Y-UJiHZ4MebxOXUuUH4Ub1SuDmn1ow2YNJ72s,1598
-exciton-1.8.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-exciton-1.8.0.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
-exciton-1.8.0.dist-info/RECORD,,
+exciton-1.8.1.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
+exciton-1.8.1.dist-info/METADATA,sha256=_PtyNrih9rHSLaHHpnuRRkJX1gjICyMc5IweNYcm2Yc,1598
+exciton-1.8.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+exciton-1.8.1.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
+exciton-1.8.1.dist-info/RECORD,,
```

