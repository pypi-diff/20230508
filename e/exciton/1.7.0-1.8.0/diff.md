# Comparing `tmp/exciton-1.7.0-py3-none-any.whl.zip` & `tmp/exciton-1.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 57677 bytes, number of entries: 60
+Zip file size: 57718 bytes, number of entries: 60
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/ml/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-26 00:50 exciton/ml/classification/__init__.py
 -rw-rw-r--  2.0 unx     1461 b- defN 23-Mar-26 01:24 exciton/ml/classification/utils.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Mar-26 03:49 exciton/ml/classification/bert/__init__.py
 -rw-rw-r--  2.0 unx     5860 b- defN 23-Mar-29 15:08 exciton/ml/classification/bert/model.py
 -rw-rw-r--  2.0 unx     1966 b- defN 23-Mar-29 14:55 exciton/ml/classification/bert/trainer.py
@@ -45,18 +45,18 @@
 -rw-rw-r--  2.0 unx     3782 b- defN 23-Mar-22 19:09 exciton/nlp/named_entity_recogonition/service.py
 -rw-rw-r--  2.0 unx     3192 b- defN 23-Mar-23 02:02 exciton/nlp/named_entity_recogonition/utils.py
 -rw-rw-r--  2.0 unx     3876 b- defN 23-Mar-23 02:49 exciton/nlp/named_entity_recogonition/xlmroberta.py
 -rw-rw-r--  2.0 unx       59 b- defN 23-May-05 01:21 exciton/nlp/sentence_tokenizer/__init__.py
 -rw-rw-r--  2.0 unx     4879 b- defN 23-May-07 10:31 exciton/nlp/sentence_tokenizer/exciton_sbd.py
 -rw-rw-r--  2.0 unx     3977 b- defN 23-May-02 03:18 exciton/nlp/sentence_tokenizer/service.py
 -rw-rw-r--  2.0 unx       84 b- defN 23-May-01 15:45 exciton/nlp/text_matching/__init__.py
--rw-rw-r--  2.0 unx     2562 b- defN 23-May-01 17:44 exciton/nlp/text_matching/exciton_matching.py
+-rw-rw-r--  2.0 unx     2565 b- defN 23-May-08 00:57 exciton/nlp/text_matching/exciton_matching.py
 -rw-rw-r--  2.0 unx       50 b- defN 23-Mar-12 04:02 exciton/nlp/translation/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 23:23 exciton/nlp/translation/m2m100/__init__.py
--rw-rw-r--  2.0 unx     4289 b- defN 23-Apr-22 11:14 exciton/nlp/translation/m2m100/service.py
+-rw-rw-r--  2.0 unx     4525 b- defN 23-May-08 01:01 exciton/nlp/translation/m2m100/service.py
 -rw-rw-r--  2.0 unx     2172 b- defN 23-Mar-12 03:47 exciton/nlp/translation/m2m100/utils.py
--rw-r--r--  2.0 unx    11417 b- defN 23-May-07 10:31 exciton-1.7.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1598 b- defN 23-May-07 10:31 exciton-1.7.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-07 10:31 exciton-1.7.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-May-07 10:31 exciton-1.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5584 b- defN 23-May-07 10:31 exciton-1.7.0.dist-info/RECORD
-60 files, 153401 bytes uncompressed, 48567 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx    11417 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1598 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5584 b- defN 23-May-08 01:22 exciton-1.8.0.dist-info/RECORD
+60 files, 153640 bytes uncompressed, 48608 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -159,23 +159,23 @@
 
 Filename: exciton/nlp/translation/m2m100/service.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/utils.py
 Comment: 
 
-Filename: exciton-1.7.0.dist-info/LICENSE
+Filename: exciton-1.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: exciton-1.7.0.dist-info/METADATA
+Filename: exciton-1.8.0.dist-info/METADATA
 Comment: 
 
-Filename: exciton-1.7.0.dist-info/WHEEL
+Filename: exciton-1.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: exciton-1.7.0.dist-info/top_level.txt
+Filename: exciton-1.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: exciton-1.7.0.dist-info/RECORD
+Filename: exciton-1.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## exciton/nlp/text_matching/exciton_matching.py

```diff
@@ -15,15 +15,15 @@
         if path_to_model is None:
             HOME = os.path.expanduser("~")
             MODEL_DIR = "exciton/models/nlp/text_matching/exciton_matching"
             path_to_model = f"{HOME}/{MODEL_DIR}"
         self.tokenizer = AutoTokenizer.from_pretrained(f"{path_to_model}/tokenizer")
 
     @staticmethod
-    def count_tokens(tokens: List[str]) -> Dict[str, int]:
+    def _count_tokens(tokens: List[str]) -> Dict[str, int]:
         """Tokens Count
 
         Args:
             tokens (List[str]): List of tokens.
 
         Returns:
             Dict[str, int]: Tokens Count.
@@ -67,16 +67,16 @@
             tokensB = self.tokenizer.tokenize(textB)
         except Exception:
             tokensA = list(textA)
             tokensB = list(textB)
         output["tokensA"] = tokensA
         output["tokensB"] = tokensB
         # Calculate score
-        set_a = self.count_tokens(tokensA)
-        set_b = self.count_tokens(tokensB)
+        set_a = self._count_tokens(tokensA)
+        set_b = self._count_tokens(tokensB)
         match = 0.0
         for token in set_a.keys():
             if token in set_b.keys():
                 match += min(set_a[token], set_b[token])
         AinB = match / len(tokensA)
         BinA = match / len(tokensB)
         output["prob_AinB"] = AinB
```

## exciton/nlp/translation/m2m100/service.py

```diff
@@ -6,46 +6,52 @@
 import transformers
 
 
 class M2M100(object):
     """Machine Translation Module.
 
     Args:
-        model (Literal[&quot;m2m100_1.2b&quot;, &quot;m2m100_418m&quot;], optional): Model Options. Defaults to "m2m100_1.2b".
-        device (Literal[&quot;cpu&quot;, &quot;cuda&quot;], optional): Device. Defaults to "cpu".
         path_to_model (str, optional): path to the models. Defaults to None.
+        device (Literal[&quot;cpu&quot;, &quot;cuda&quot;], optional): Device. Defaults to "cpu".
     """
 
     def __init__(
         self,
-        model: Literal["m2m100_1.2b", "m2m100_418m"] = None,
         path_to_model: str = None,
         device: Literal["cpu", "cuda"] = "cpu",
     ) -> None:
         if not path_to_model:
-            assert model is not None
             HOME = os.path.expanduser("~")
-            MODEL_DIR = "exciton/models/nlp/translation/m2m100"
-            path_to_model = f"{HOME}/{MODEL_DIR}/{model}"
+            MODEL_DIR = "exciton/models/nlp/translation/m2m100/m2m100_1.2b"
+            path_to_model = f"{HOME}/{MODEL_DIR}"
         self.translator = ctranslate2.Translator(path_to_model, device=device)
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(
             f"{path_to_model}/tokenizer/"
         )
-        with open(f"{path_to_model}/support_languages.json") as fp:
-            self.support_languages = json.load(fp)
+        with open(f"{path_to_model}/languages.json") as fp:
+            languages = json.load(fp)
+        languages = {
+            key: languages[key] for key in languages if languages[key]["mt"] == "m2m100"
+        }
+        self.languages = languages
+        self.lang_mm = []
+        self.lang_map = {}
+        for key in languages:
+            self.lang_mm.append(languages[key]["code_mt"])
+            self.lang_map[languages[key]["code2"]] = languages[key]["code_mt"]
 
     def get_support_languages(self) -> List[Dict[str, str]]:
         """Suppport Languages for M2M100
 
         Returns:
             List[Dict[str, str]]: List of languages supported by M2M100 models.
         """
         return [
-            {"code": wd, "name": self.support_languages[wd]}
-            for wd in self.support_languages
+            {"code": self.languages[key]["code2"], "name": self.languages[key]["name2"]}
+            for key in self.languages
         ]
 
     def _batch(
         self, source: List[Dict[str, Any]], batch_size: int = 10
     ) -> List[List[Dict[str, Any]]]:
         """Create Batch.
 
@@ -90,15 +96,17 @@
         output = []
         for batch in self._batch(source):
             sen_list = []
             target_prefix = []
             for itm in batch:
                 slang = itm["source_lang"]
                 tlang = itm["target_lang"]
-                if slang in self.support_languages and tlang in self.support_languages:
+                if slang in self.lang_map and tlang in self.lang_map:
+                    slang = self.lang_map[slang]
+                    tlang = self.lang_map[tlang]
                     self.tokenizer.src_lang = slang
                     sen = self.tokenizer.encode(itm["source"])
                     sen = self.tokenizer.convert_ids_to_tokens(sen)
                     sen_list.append(sen)
                     target_prefix.append([self.tokenizer.lang_code_to_token[tlang]])
                 else:
                     itm["target"] = None
```

## Comparing `exciton-1.7.0.dist-info/LICENSE` & `exciton-1.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `exciton-1.7.0.dist-info/METADATA` & `exciton-1.8.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exciton
-Version: 1.7.0
+Version: 1.8.0
 Summary: Domain-specific Natural Language Processing with exciton
 Home-page: https://exciton.com
 Author: The ExcitonX Team
 Author-email: excitonx@gmail.com
 License: UNKNOWN
 Keywords: exciton NLP Deep Learning
 Platform: UNKNOWN
```

## Comparing `exciton-1.7.0.dist-info/RECORD` & `exciton-1.8.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 exciton/nlp/named_entity_recogonition/service.py,sha256=hb9VxtZ_eiF578oC621Wu5jU5TgaZ-fzOzKf6EjU3NY,3782
 exciton/nlp/named_entity_recogonition/utils.py,sha256=0GaerSJudvinee0rxL6zRtrSOhvGSUzbNoNci7KTzl4,3192
 exciton/nlp/named_entity_recogonition/xlmroberta.py,sha256=av4mSyZ5DNaN0KmmpEw4WkzGsrgupR8X0FiU1cdA4dw,3876
 exciton/nlp/sentence_tokenizer/__init__.py,sha256=1hIgq6ayPk2yVdhBgLHe5vXxU2fcDrenz51iKXhx28s,59
 exciton/nlp/sentence_tokenizer/exciton_sbd.py,sha256=EG0kV16yXsv2EuYblN7kEVrN1FgoYTZTgAn7V7Cga7k,4879
 exciton/nlp/sentence_tokenizer/service.py,sha256=3Ssq2UNmhDCezhBJq4V8csacA_0XenYmgPLZfmBtBYc,3977
 exciton/nlp/text_matching/__init__.py,sha256=tgQvyWZupI0QAHlnLAJldpOPBCF01OFq2poLH49tAVg,84
-exciton/nlp/text_matching/exciton_matching.py,sha256=Co3l9H_HH5dx_IlOlUL8j1jrbsMOfvP-F9TmpXj2SBs,2562
+exciton/nlp/text_matching/exciton_matching.py,sha256=a99bzY5117DLAGb_AgV_4ai6buVYrMmyvengo18CeIU,2565
 exciton/nlp/translation/__init__.py,sha256=gE0YV-s4pB7VQWdsg04hALOBBpuWaQ3AUqpY9rvgI_8,50
 exciton/nlp/translation/m2m100/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-exciton/nlp/translation/m2m100/service.py,sha256=5YlJWxetgB7sIE-93Wsa-3ngJBqCPsqifpPim1oHag4,4289
+exciton/nlp/translation/m2m100/service.py,sha256=YbGM7sKTwAa8XkF54ZOKmx-3A0Yt7ZQ9OH1RmV_-vSo,4525
 exciton/nlp/translation/m2m100/utils.py,sha256=GE8qg2deaHBMVMIHS32Hb5TCxO453kuncQrdJsnRIoU,2172
-exciton-1.7.0.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
-exciton-1.7.0.dist-info/METADATA,sha256=IMkquEJbbX_j15V3-EJ5l71l1JgWXWSyrUKx-DgohEM,1598
-exciton-1.7.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-exciton-1.7.0.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
-exciton-1.7.0.dist-info/RECORD,,
+exciton-1.8.0.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
+exciton-1.8.0.dist-info/METADATA,sha256=XVGgE_Y-UJiHZ4MebxOXUuUH4Ub1SuDmn1ow2YNJ72s,1598
+exciton-1.8.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+exciton-1.8.0.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
+exciton-1.8.0.dist-info/RECORD,,
```

