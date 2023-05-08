# Comparing `tmp/llmpool-0.0.2-py3-none-any.whl.zip` & `tmp/llmpool-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8076 bytes, number of entries: 10
--rw-rw-rw-  2.0 unx       90 b- defN 23-May-08 07:15 llmpool/__init__.py
--rw-rw-rw-  2.0 unx     3856 b- defN 23-May-08 06:37 llmpool/local_model.py
+Zip file size: 8055 bytes, number of entries: 10
+-rw-rw-rw-  2.0 unx       90 b- defN 23-May-08 07:22 llmpool/__init__.py
+-rw-rw-rw-  2.0 unx     3782 b- defN 23-May-08 07:23 llmpool/local_model.py
 -rw-rw-rw-  2.0 unx      591 b- defN 23-May-08 04:52 llmpool/model.py
 -rw-rw-rw-  2.0 unx      261 b- defN 23-May-07 13:49 llmpool/model_pool.py
 -rw-rw-rw-  2.0 unx     1866 b- defN 23-May-08 04:12 llmpool/remote_model.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 unx      796 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      767 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/RECORD
-10 files, 19684 bytes uncompressed, 6774 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 07:23 llmpool-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx      796 b- defN 23-May-08 07:23 llmpool-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 07:23 llmpool-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 07:23 llmpool-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      767 b- defN 23-May-08 07:23 llmpool-0.0.3.dist-info/RECORD
+10 files, 19610 bytes uncompressed, 6753 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: llmpool/model_pool.py
 Comment: 
 
 Filename: llmpool/remote_model.py
 Comment: 
 
-Filename: llmpool-0.0.2.dist-info/LICENSE
+Filename: llmpool-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: llmpool-0.0.2.dist-info/METADATA
+Filename: llmpool-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: llmpool-0.0.2.dist-info/WHEEL
+Filename: llmpool-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: llmpool-0.0.2.dist-info/top_level.txt
+Filename: llmpool-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: llmpool-0.0.2.dist-info/RECORD
+Filename: llmpool-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llmpool/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 from .local_model import LocalCausalLLModel, LocalLoRACausalLLModel
```

## llmpool/local_model.py

```diff
@@ -1,18 +1,38 @@
 from threading import Thread
 
 from peft import PeftModel
 from transformers import GenerationConfig
-from transformers import AutoModelForCausalLM, AutoTokenizer
+from transformers import AutoModel, AutoTokenizer
 from transformers import TextIteratorStreamer
 from optimum.bettertransformer import BetterTransformer
 
 from llmpool.model import LLModel
 
 class LocalLLModel(LLModel):
+    def __init__(
+        self, name, base, device='cuda', 
+        load_in_8bit=True, apply_bettertransformer=False
+    ):
+        super().__init__(name)
+
+        self.device = device
+        self.tokenizer = AutoTokenizer.from_pretrained(base)
+        self.model = AutoModel.from_pretrained(
+            base,
+            load_in_8bit=load_in_8bit,
+            device_map="auto",
+        )
+        
+        if apply_bettertransformer:
+            self.model = BetterTransformer.transform(self.model)
+
+        if not load_in_8bit:
+            self.model.half()
+
     def stream_gen(self, prompt, gen_config: GenerationConfig, stopping_criteria=None, start=True):
         super().stream_gen(prompt, gen_config, stopping_criteria)
 
         model_inputs = self._build_model_inputs(prompt)
         streamer = self._build_streamer()
         gen_kwargs = self._build_gen_kwargs(
             model_inputs, gen_config, streamer, stopping_criteria
@@ -71,36 +91,15 @@
             )
 
             decoded = self.tokenizer.batch_decode(
                 generated_ids, skip_prompt=True, skip_special_tokens=True
             )
             return decoded              
 
-class LocalCausalLLModel(LocalLLModel):
-    def __init__(
-        self, name, base, device='cuda', 
-        load_in_8bit=True, apply_bettertransformer=False
-    ):
-        super().__init__(name)
-
-        self.device = device
-        self.tokenizer = AutoTokenizer.from_pretrained(base)
-        self.model = AutoModelForCausalLM.from_pretrained(
-            base,
-            load_in_8bit=load_in_8bit,
-            device_map="auto",
-        )
-        
-        if apply_bettertransformer:
-            self.model = BetterTransformer.transform(self.model)
-
-        if not load_in_8bit:
-            self.model.half()
-
-class LocalLoRACausalLLModel(LocalCausalLLModel):
+class LocalLoRALLModel(LocalLLModel):
     def __init__(
         self, name, base, ckpt, device='cuda', 
         load_in_8bit=True, apply_bettertransformer=False
     ):
         super().__init__(
             name, base, device, load_in_8bit, 
             apply_bettertransformer=apply_bettertransformer)
```

## Comparing `llmpool-0.0.2.dist-info/LICENSE` & `llmpool-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llmpool-0.0.2.dist-info/METADATA` & `llmpool-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmpool
-Version: 0.0.2
+Version: 0.0.3
 Summary: Large Language Models' pool management library
 Home-page: https://github.com/deep-diver/LLM-Pool
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,instance pool,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

