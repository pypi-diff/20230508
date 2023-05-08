# Comparing `tmp/llmpool-0.0.6-py3-none-any.whl.zip` & `tmp/llmpool-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8075 bytes, number of entries: 10
--rw-rw-rw-  2.0 unx       78 b- defN 23-May-08 07:37 llmpool/__init__.py
--rw-rw-rw-  2.0 unx     3958 b- defN 23-May-08 07:37 llmpool/local_model.py
+Zip file size: 8063 bytes, number of entries: 10
+-rw-rw-rw-  2.0 unx       78 b- defN 23-May-08 07:39 llmpool/__init__.py
+-rw-rw-rw-  2.0 unx     3897 b- defN 23-May-08 07:39 llmpool/local_model.py
 -rw-rw-rw-  2.0 unx      591 b- defN 23-May-08 07:36 llmpool/model.py
 -rw-rw-rw-  2.0 unx      261 b- defN 23-May-07 13:49 llmpool/model_pool.py
 -rw-rw-rw-  2.0 unx     1866 b- defN 23-May-08 04:12 llmpool/remote_model.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 07:37 llmpool-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 unx      796 b- defN 23-May-08 07:37 llmpool-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 07:37 llmpool-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 07:37 llmpool-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      767 b- defN 23-May-08 07:37 llmpool-0.0.6.dist-info/RECORD
-10 files, 19774 bytes uncompressed, 6773 bytes compressed:  65.7%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 07:39 llmpool-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx      796 b- defN 23-May-08 07:39 llmpool-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 07:39 llmpool-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 07:39 llmpool-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      767 b- defN 23-May-08 07:39 llmpool-0.0.7.dist-info/RECORD
+10 files, 19713 bytes uncompressed, 6761 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: llmpool/model_pool.py
 Comment: 
 
 Filename: llmpool/remote_model.py
 Comment: 
 
-Filename: llmpool-0.0.6.dist-info/LICENSE
+Filename: llmpool-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: llmpool-0.0.6.dist-info/METADATA
+Filename: llmpool-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: llmpool-0.0.6.dist-info/WHEEL
+Filename: llmpool-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: llmpool-0.0.6.dist-info/top_level.txt
+Filename: llmpool-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: llmpool-0.0.6.dist-info/RECORD
+Filename: llmpool-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llmpool/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 from .local_model import LocalLLModel, LocalLoRALLModel
```

## llmpool/local_model.py

```diff
@@ -99,15 +99,14 @@
 class LocalLoRALLModel(LocalLLModel):
     def __init__(
         self, name, base, ckpt, device='cuda',
         model_cls=AutoModel, tokenizer_cls=AutoTokenizer,
         load_in_8bit=True, apply_bettertransformer=False
     ):
         super().__init__(
-            name, base, device, load_in_8bit, 
-            model_cls=model_cls, tokenizer_cls=tokenizer_cls,
-            apply_bettertransformer=apply_bettertransformer)
+            name, base, device, model_cls, tokenizer_cls,
+            load_in_8bit, apply_bettertransformer)
 
         self.model = PeftModel.from_pretrained(
             self.model, ckpt, 
             device_map={'': 0}
         )
```

## Comparing `llmpool-0.0.6.dist-info/LICENSE` & `llmpool-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llmpool-0.0.6.dist-info/METADATA` & `llmpool-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmpool
-Version: 0.0.6
+Version: 0.0.7
 Summary: Large Language Models' pool management library
 Home-page: https://github.com/deep-diver/LLM-Pool
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,instance pool,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `llmpool-0.0.6.dist-info/RECORD` & `llmpool-0.0.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-llmpool/__init__.py,sha256=MYJ5G753ZHauyXUGKJwHppR8TuzMxPQf99h4CReorjM,78
-llmpool/local_model.py,sha256=s5R8ZxufWtoMJFCWaJG3dIHmsrjdBbvuDvwGprx8r8c,3958
+llmpool/__init__.py,sha256=ubTFIpI4Hx-IL9GOsm9Dei3WHcMV8WeX54r0iuyn-EU,78
+llmpool/local_model.py,sha256=T7-CcFrINOEiu-Aq37yRMcQ0GZRtjHWDy8119rOjetQ,3897
 llmpool/model.py,sha256=l29Usepsgp3z--CB0sJh-8VdGJlmWJIyzqLiZ3ep1Gs,591
 llmpool/model_pool.py,sha256=lmpjZLJH1Jsja9WpbrzcjoP1Hu1G-EADuu8cNIwyeB8,261
 llmpool/remote_model.py,sha256=VP6oPR9iNeKG-nY_GGpl4POMP31zmnRCNgjuJb-XZiQ,1866
-llmpool-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-llmpool-0.0.6.dist-info/METADATA,sha256=McBWiwecBVyystSPgdGTM7Oadsi-sFa2FJh3YAVW8Qw,796
-llmpool-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-llmpool-0.0.6.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
-llmpool-0.0.6.dist-info/RECORD,,
+llmpool-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+llmpool-0.0.7.dist-info/METADATA,sha256=eoebOp0hhg4kc0qgVjSnhAYyeuO_yV5PlRvIizX7_J4,796
+llmpool-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+llmpool-0.0.7.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
+llmpool-0.0.7.dist-info/RECORD,,
```

