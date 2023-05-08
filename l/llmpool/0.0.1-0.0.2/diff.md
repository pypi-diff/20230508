# Comparing `tmp/llmpool-0.0.1-py3-none-any.whl.zip` & `tmp/llmpool-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8052 bytes, number of entries: 10
--rw-rw-rw-  2.0 unx       90 b- defN 23-May-08 02:23 llmpool/__init__.py
--rw-rw-rw-  2.0 unx     3804 b- defN 23-May-08 04:29 llmpool/local_model.py
+Zip file size: 8076 bytes, number of entries: 10
+-rw-rw-rw-  2.0 unx       90 b- defN 23-May-08 07:15 llmpool/__init__.py
+-rw-rw-rw-  2.0 unx     3856 b- defN 23-May-08 06:37 llmpool/local_model.py
 -rw-rw-rw-  2.0 unx      591 b- defN 23-May-08 04:52 llmpool/model.py
 -rw-rw-rw-  2.0 unx      261 b- defN 23-May-07 13:49 llmpool/model_pool.py
 -rw-rw-rw-  2.0 unx     1866 b- defN 23-May-08 04:12 llmpool/remote_model.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 05:04 llmpool-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 unx      796 b- defN 23-May-08 05:04 llmpool-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 05:04 llmpool-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 05:04 llmpool-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      767 b- defN 23-May-08 05:04 llmpool-0.0.1.dist-info/RECORD
-10 files, 19632 bytes uncompressed, 6750 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx      796 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      767 b- defN 23-May-08 07:16 llmpool-0.0.2.dist-info/RECORD
+10 files, 19684 bytes uncompressed, 6774 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: llmpool/model_pool.py
 Comment: 
 
 Filename: llmpool/remote_model.py
 Comment: 
 
-Filename: llmpool-0.0.1.dist-info/LICENSE
+Filename: llmpool-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: llmpool-0.0.1.dist-info/METADATA
+Filename: llmpool-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: llmpool-0.0.1.dist-info/WHEEL
+Filename: llmpool-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: llmpool-0.0.1.dist-info/top_level.txt
+Filename: llmpool-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: llmpool-0.0.1.dist-info/RECORD
+Filename: llmpool-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llmpool/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 from .local_model import LocalCausalLLModel, LocalLoRACausalLLModel
```

## llmpool/local_model.py

```diff
@@ -5,24 +5,26 @@
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from transformers import TextIteratorStreamer
 from optimum.bettertransformer import BetterTransformer
 
 from llmpool.model import LLModel
 
 class LocalLLModel(LLModel):
-    def stream_gen(self, prompt, gen_config: GenerationConfig, stopping_criteria=None):
+    def stream_gen(self, prompt, gen_config: GenerationConfig, stopping_criteria=None, start=True):
         super().stream_gen(prompt, gen_config, stopping_criteria)
 
         model_inputs = self._build_model_inputs(prompt)
         streamer = self._build_streamer()
         gen_kwargs = self._build_gen_kwargs(
             model_inputs, gen_config, streamer, stopping_criteria
         )
 
         t = Thread(target=self.model.generate, kwargs=gen_kwargs)
+        if start:
+            t.start()
         return t, streamer
 
     def _build_gen_kwargs(self, model_inputs, gen_config, streamer, stopping_criteria):
         gen_kwargs = dict(
             model_inputs,
             streamer=streamer,
             stopping_criteria=stopping_criteria
```

## Comparing `llmpool-0.0.1.dist-info/LICENSE` & `llmpool-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llmpool-0.0.1.dist-info/METADATA` & `llmpool-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmpool
-Version: 0.0.1
+Version: 0.0.2
 Summary: Large Language Models' pool management library
 Home-page: https://github.com/deep-diver/LLM-Pool
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,instance pool,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `llmpool-0.0.1.dist-info/RECORD` & `llmpool-0.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-llmpool/__init__.py,sha256=-BNrswWy6dZBc3oWbuqbn_-GvBSqx3V5jdHnHfbicR4,90
-llmpool/local_model.py,sha256=-jpUKR9IyY-ZUrIdYHrlYrCT0xBwP-iLqcWW-HR9-nc,3804
+llmpool/__init__.py,sha256=krI9YBCzbAd54uYrSZZr6cKhGYQJSXJDaJoIeKoJxTc,90
+llmpool/local_model.py,sha256=uneZkKt1uUoPAM-KHuA5wqi3qfzXJ7E2TGt-OHmzfLQ,3856
 llmpool/model.py,sha256=l29Usepsgp3z--CB0sJh-8VdGJlmWJIyzqLiZ3ep1Gs,591
 llmpool/model_pool.py,sha256=lmpjZLJH1Jsja9WpbrzcjoP1Hu1G-EADuu8cNIwyeB8,261
 llmpool/remote_model.py,sha256=VP6oPR9iNeKG-nY_GGpl4POMP31zmnRCNgjuJb-XZiQ,1866
-llmpool-0.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-llmpool-0.0.1.dist-info/METADATA,sha256=bmOMduLRCDozIQW6pXadpPVe9N_9KLiq4WkiXuar0r8,796
-llmpool-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-llmpool-0.0.1.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
-llmpool-0.0.1.dist-info/RECORD,,
+llmpool-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+llmpool-0.0.2.dist-info/METADATA,sha256=KwH1u98BPcpX7vPW8C9-poTQHnPbb_wW5_zRTm7AD4s,796
+llmpool-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+llmpool-0.0.2.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
+llmpool-0.0.2.dist-info/RECORD,,
```

