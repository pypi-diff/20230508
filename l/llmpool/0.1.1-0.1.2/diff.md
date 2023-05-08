# Comparing `tmp/llmpool-0.1.1-py3-none-any.whl.zip` & `tmp/llmpool-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9076 bytes, number of entries: 11
--rw-rw-rw-  2.0 unx      114 b- defN 23-May-08 14:31 llmpool/__init__.py
+Zip file size: 9107 bytes, number of entries: 11
+-rw-rw-rw-  2.0 unx      114 b- defN 23-May-08 14:35 llmpool/__init__.py
 -rw-rw-rw-  2.0 unx     3897 b- defN 23-May-08 14:27 llmpool/local_model.py
 -rw-rw-rw-  2.0 unx      591 b- defN 23-May-08 07:36 llmpool/model.py
 -rw-rw-rw-  2.0 unx      919 b- defN 23-May-08 09:30 llmpool/model_pool.py
 -rw-rw-rw-  2.0 unx     1868 b- defN 23-May-08 09:20 llmpool/remote_model.py
--rw-rw-rw-  2.0 unx      890 b- defN 23-May-08 14:28 llmpool/utils.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 14:31 llmpool-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     1632 b- defN 23-May-08 14:31 llmpool-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 14:31 llmpool-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 14:31 llmpool-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      841 b- defN 23-May-08 14:31 llmpool-0.1.1.dist-info/RECORD
-11 files, 22209 bytes uncompressed, 7666 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 unx     1031 b- defN 23-May-08 14:34 llmpool/utils.py
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 14:35 llmpool-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     1632 b- defN 23-May-08 14:35 llmpool-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 14:35 llmpool-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 14:35 llmpool-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      842 b- defN 23-May-08 14:35 llmpool-0.1.2.dist-info/RECORD
+11 files, 22351 bytes uncompressed, 7697 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: llmpool/remote_model.py
 Comment: 
 
 Filename: llmpool/utils.py
 Comment: 
 
-Filename: llmpool-0.1.1.dist-info/LICENSE
+Filename: llmpool-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: llmpool-0.1.1.dist-info/METADATA
+Filename: llmpool-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: llmpool-0.1.1.dist-info/WHEEL
+Filename: llmpool-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: llmpool-0.1.1.dist-info/top_level.txt
+Filename: llmpool-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: llmpool-0.1.1.dist-info/RECORD
+Filename: llmpool-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llmpool/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 from .local_model import LocalLLModel, LocalLoRALLModel
 from .model_pool import LLModelPool
```

## llmpool/utils.py

```diff
@@ -16,14 +16,17 @@
     model_type = model_spec['type']
     metadata = model_spec['metadata']
     model_ckpt = model_spec['model']
     load_config = model_spec['load']
     gen_config = model_spec['generation_config']
 
     model_type = eval(model_type)
+    load_config['model_cls'] = eval(load_config['model_cls'])
+    load_config['tokenizer_cls'] = eval(load_config['tokenizer_cls'])
+        
     model = model_type(
         name=name,
         **model_ckpt,
         **load_config
     )
 
     return model
```

## Comparing `llmpool-0.1.1.dist-info/LICENSE` & `llmpool-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llmpool-0.1.1.dist-info/METADATA` & `llmpool-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmpool
-Version: 0.1.1
+Version: 0.1.2
 Summary: Large Language Models' pool management library
 Home-page: https://github.com/deep-diver/LLM-Pool
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,instance pool,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `llmpool-0.1.1.dist-info/RECORD` & `llmpool-0.1.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-llmpool/__init__.py,sha256=UloeKJMm9bGesvjJznqs4Q02yBMH41MDoKuEhd9511I,114
+llmpool/__init__.py,sha256=9SM_UuiRAW3_8v49sB6qSdULddaO1wRqCKffj3F0kW0,114
 llmpool/local_model.py,sha256=zzGAdpzAgG5nzox6usdTd0rnB8A2K0YUVBy22zkPGAI,3897
 llmpool/model.py,sha256=l29Usepsgp3z--CB0sJh-8VdGJlmWJIyzqLiZ3ep1Gs,591
 llmpool/model_pool.py,sha256=NazsR-AfxSzxew6DGB5-bePhwgSecuBsv-lB6WmOpt0,919
 llmpool/remote_model.py,sha256=NI2xu2GSUI8u4q35fP_BNUpjnD8eUDiKiPUgFyCjViY,1868
-llmpool/utils.py,sha256=InYpAXLNHCNIcdpcqWndtthuvGXYsbh85ou8ebrdKT0,890
-llmpool-0.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-llmpool-0.1.1.dist-info/METADATA,sha256=NqRJeiVnqvU1jgBJnckDMThSxbmOm-zMWXaXRaGfzew,1632
-llmpool-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-llmpool-0.1.1.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
-llmpool-0.1.1.dist-info/RECORD,,
+llmpool/utils.py,sha256=t-gxZXBAV5qhb2YqliJJlnbjxNin37qIIwX7dIZ5Ytc,1031
+llmpool-0.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+llmpool-0.1.2.dist-info/METADATA,sha256=ZGpaZczUpzCX-XxozzoZc3euLhzBcGc2c4U8EAZUiks,1632
+llmpool-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+llmpool-0.1.2.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
+llmpool-0.1.2.dist-info/RECORD,,
```

