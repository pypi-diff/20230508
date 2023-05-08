# Comparing `tmp/llmpool-0.0.4-py3-none-any.whl.zip` & `tmp/llmpool-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8049 bytes, number of entries: 10
--rw-rw-rw-  2.0 unx       78 b- defN 23-May-08 07:25 llmpool/__init__.py
--rw-rw-rw-  2.0 unx     3782 b- defN 23-May-08 07:23 llmpool/local_model.py
+Zip file size: 8068 bytes, number of entries: 10
+-rw-rw-rw-  2.0 unx       78 b- defN 23-May-08 07:34 llmpool/__init__.py
+-rw-rw-rw-  2.0 unx     3839 b- defN 23-May-08 07:33 llmpool/local_model.py
 -rw-rw-rw-  2.0 unx      591 b- defN 23-May-08 04:52 llmpool/model.py
 -rw-rw-rw-  2.0 unx      261 b- defN 23-May-07 13:49 llmpool/model_pool.py
 -rw-rw-rw-  2.0 unx     1866 b- defN 23-May-08 04:12 llmpool/remote_model.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 07:25 llmpool-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 unx      796 b- defN 23-May-08 07:25 llmpool-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 07:25 llmpool-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 07:25 llmpool-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      767 b- defN 23-May-08 07:25 llmpool-0.0.4.dist-info/RECORD
-10 files, 19598 bytes uncompressed, 6747 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 07:34 llmpool-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx      796 b- defN 23-May-08 07:34 llmpool-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 07:34 llmpool-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 07:34 llmpool-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      767 b- defN 23-May-08 07:34 llmpool-0.0.5.dist-info/RECORD
+10 files, 19655 bytes uncompressed, 6766 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: llmpool/model_pool.py
 Comment: 
 
 Filename: llmpool/remote_model.py
 Comment: 
 
-Filename: llmpool-0.0.4.dist-info/LICENSE
+Filename: llmpool-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: llmpool-0.0.4.dist-info/METADATA
+Filename: llmpool-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: llmpool-0.0.4.dist-info/WHEEL
+Filename: llmpool-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: llmpool-0.0.4.dist-info/top_level.txt
+Filename: llmpool-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: llmpool-0.0.4.dist-info/RECORD
+Filename: llmpool-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llmpool/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 from .local_model import LocalLLModel, LocalLoRALLModel
```

## llmpool/local_model.py

```diff
@@ -6,22 +6,23 @@
 from transformers import TextIteratorStreamer
 from optimum.bettertransformer import BetterTransformer
 
 from llmpool.model import LLModel
 
 class LocalLLModel(LLModel):
     def __init__(
-        self, name, base, device='cuda', 
+        self, name, base, device='cuda',
+        model_cls=AutoModel, tokenizer_cls=AutoTokenizer,
         load_in_8bit=True, apply_bettertransformer=False
     ):
         super().__init__(name)
 
         self.device = device
-        self.tokenizer = AutoTokenizer.from_pretrained(base)
-        self.model = AutoModel.from_pretrained(
+        self.tokenizer = tokenizer_cls.from_pretrained(base)
+        self.model = model_cls.from_pretrained(
             base,
             load_in_8bit=load_in_8bit,
             device_map="auto",
         )
         
         if apply_bettertransformer:
             self.model = BetterTransformer.transform(self.model)
```

## Comparing `llmpool-0.0.4.dist-info/LICENSE` & `llmpool-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llmpool-0.0.4.dist-info/METADATA` & `llmpool-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmpool
-Version: 0.0.4
+Version: 0.0.5
 Summary: Large Language Models' pool management library
 Home-page: https://github.com/deep-diver/LLM-Pool
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,instance pool,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

