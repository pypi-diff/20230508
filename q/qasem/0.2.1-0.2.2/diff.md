# Comparing `tmp/qasem-0.2.1.tar.gz` & `tmp/qasem-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qasem-0.2.1.tar", last modified: Mon May  8 07:20:42 2023, max compression
+gzip compressed data, was "dist/qasem-0.2.2.tar", last modified: Mon May  8 09:09:32 2023, max compression
```

## Comparing `qasem-0.2.1.tar` & `qasem-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 07:20:42.000000 qasem-0.2.1/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)       88 2022-07-17 10:30:16.000000 qasem-0.2.1/MANIFEST.in
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-05-08 07:20:42.000000 qasem-0.2.1/PKG-INFO
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8708 2023-04-17 06:10:03.000000 qasem-0.2.1/README.md
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      200 2022-07-17 11:03:06.000000 qasem-0.2.1/qasem/__init__.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7443 2023-03-16 08:20:42.000000 qasem-0.2.1/qasem/candidates_finder.py
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem/data/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5934 2023-01-31 18:04:55.000000 qasem-0.2.1/qasem/data/connectives_small_set.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)    17746 2023-03-16 08:12:00.000000 qasem-0.2.1/qasem/end_to_end_pipeline.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5039 2023-01-04 13:57:20.000000 qasem-0.2.1/qasem/openie_converter.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5041 2023-03-16 08:22:36.000000 qasem-0.2.1/qasem/qa_adj_pipeline.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     4616 2023-01-04 13:57:20.000000 qasem-0.2.1/qasem/qa_discourse_pipeline.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     3232 2023-01-31 14:13:37.000000 qasem-0.2.1/qasem/question_contextualizer.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      845 2023-03-16 08:20:10.000000 qasem-0.2.1/qasem/spacy_loader.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2364 2023-02-05 09:41:21.000000 qasem-0.2.1/qasem/test_end_to_end_pipeline.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      271 2023-02-05 09:41:21.000000 qasem-0.2.1/qasem/utils.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        5 2023-05-08 07:19:34.000000 qasem-0.2.1/qasem/version.txt
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/PKG-INFO
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      499 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/SOURCES.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        1 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/dependency_links.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)       53 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/requires.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        6 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/top_level.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)       79 2023-05-08 07:20:42.000000 qasem-0.2.1/setup.cfg
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1235 2023-05-08 07:19:23.000000 qasem-0.2.1/setup.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 09:09:32.000000 qasem-0.2.2/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       88 2022-07-17 10:30:16.000000 qasem-0.2.2/MANIFEST.in
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-05-08 09:09:32.000000 qasem-0.2.2/PKG-INFO
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8708 2023-04-17 06:10:03.000000 qasem-0.2.2/README.md
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 09:09:32.000000 qasem-0.2.2/qasem/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      200 2022-07-17 11:03:06.000000 qasem-0.2.2/qasem/__init__.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7489 2023-05-08 09:03:16.000000 qasem-0.2.2/qasem/candidates_finder.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 09:09:32.000000 qasem-0.2.2/qasem/data/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5934 2023-01-31 18:04:55.000000 qasem-0.2.2/qasem/data/connectives_small_set.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    17906 2023-05-08 09:07:37.000000 qasem-0.2.2/qasem/end_to_end_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5039 2023-01-04 13:57:20.000000 qasem-0.2.2/qasem/openie_converter.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5041 2023-03-16 08:22:36.000000 qasem-0.2.2/qasem/qa_adj_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     4703 2023-05-08 09:03:19.000000 qasem-0.2.2/qasem/qa_discourse_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     3232 2023-01-31 14:13:37.000000 qasem-0.2.2/qasem/question_contextualizer.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      845 2023-03-16 08:20:10.000000 qasem-0.2.2/qasem/spacy_loader.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2364 2023-02-05 09:41:21.000000 qasem-0.2.2/qasem/test_end_to_end_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      271 2023-02-05 09:41:21.000000 qasem-0.2.2/qasem/utils.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        5 2023-05-08 09:06:53.000000 qasem-0.2.2/qasem/version.txt
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 09:09:32.000000 qasem-0.2.2/qasem.egg-info/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-05-08 09:09:32.000000 qasem-0.2.2/qasem.egg-info/PKG-INFO
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      499 2023-05-08 09:09:32.000000 qasem-0.2.2/qasem.egg-info/SOURCES.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        1 2023-05-08 09:09:32.000000 qasem-0.2.2/qasem.egg-info/dependency_links.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       53 2023-05-08 09:09:32.000000 qasem-0.2.2/qasem.egg-info/requires.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        6 2023-05-08 09:09:32.000000 qasem-0.2.2/qasem.egg-info/top_level.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       79 2023-05-08 09:09:32.000000 qasem-0.2.2/setup.cfg
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1235 2023-05-08 07:19:23.000000 qasem-0.2.2/setup.py
```

### Comparing `qasem-0.2.1/PKG-INFO` & `qasem-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qasem
-Version: 0.2.1
+Version: 0.2.2
 Summary: package for QA-based Semantics - representing textual information via question-answer pairs
 Home-page: https://github.com/kleinay/QASem
 Author: Ayal Klein, Ruben Wolhandler, Ron Eliav
 Author-email: ayal.s.klein@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qasem-0.2.1/README.md` & `qasem-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qasem-0.2.1/qasem/candidates_finder.py` & `qasem-0.2.2/qasem/candidates_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,19 @@
     return splitlist
     
     
     
     
 class CandidateFinder():
 
-    def __init__(self, conn_file: Optional[str] = None):
+    def __init__(self, conn_file: Optional[str] = None, spacy_model: Optional[str] = None):
         conn_file = conn_file or connective_file_default_path
         self.connectives = get_connectives(conn_file)
         self.detokenizer = TreebankWordDetokenizer()
-        self.nlp = get_spacy()
+        self.nlp = get_spacy(spacy_model)
         self.covered = defaultdict(lambda : '')
         
         
     def num_candidates(self, sentence):
         sentence = sentence.strip().split('\t')
         text = sentence[0]
         text = text.replace(' -LRB- ', ' ')
```

### Comparing `qasem-0.2.1/qasem/data/connectives_small_set.txt` & `qasem-0.2.2/qasem/data/connectives_small_set.txt`

 * *Files identical despite different names*

### Comparing `qasem-0.2.1/qasem/end_to_end_pipeline.py` & `qasem-0.2.2/qasem/end_to_end_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 qadiscourse_model_name = "RonEliav/QA_discourse_v2"
 question_contextualization_model_name = "biu-nlp/contextualizer_qasrl"
 
 # Defaults
 default_annotation_layers = ['qanom', 'qasrl', 'qadiscourse']
 default_nominalization_detection_threshold = 0.7
 NO_REPEAT = True
-DEFAULT_SPACY_MODEL = 'en_core_web_trf'
+DEFAULT_SPACY_MODEL = 'en_core_web_lg'
 
 class QASemEndToEndPipeline():
     """
     This pipeline currently wraps QA-SRL, QANom and QADiscourse pipelines.
     """
     def __init__(self,
                  annotation_layers: Optional[List[str]] = None,
@@ -57,14 +57,15 @@
             qanom_model (Optional[str], optional): Underlying nominal QASRL (=QANom) model. Can be a key for `qanom_models` or a Huggingface Hub URL.
                 Defaults to "joint".
             contextualize (bool, optional): . 
             openie_converter_kwargs (Dict[str, Any], optional): key-word args to pass to `OpenIEConverter` constructor. Defaults to empty dict().
         """
         self.device_int = device # represent device in HF convention
         self.device_str = f"cuda:{device}" if device >= 0 else "cpu"# represent device in pytorch convention
+        self.spacy_model_name = spacy_model or DEFAULT_SPACY_MODEL
         self.annotation_layers = annotation_layers or default_annotation_layers
         qasrl_model = qasrl_model or default_qasrl_model
         qanom_model = qanom_model or default_qanom_model
         # Either a name from dict or the actual model name in HF
         qasrl_model_url = qasrl_models[qasrl_model] if qasrl_model in qasrl_models else qasrl_model
         qanom_model_url = qanom_models[qanom_model] if qanom_model in qanom_models else qanom_model
         # Init QANom predicate detection model
@@ -86,20 +87,21 @@
         else:
             if 'qasrl' in self.annotation_layers:
                 self.qasrl_pipelines = {"verbal": QASRL_Pipeline(qasrl_model_url, **qasrl_pipeline_kwargs)}
             if 'qanom' in self.annotation_layers:
                 self.qasrl_pipelines = {"nominal": QASRL_Pipeline(qasrl_model_url, **qasrl_pipeline_kwargs)}
 
         if 'qadiscourse' in self.annotation_layers:
-            self.qa_discourse_pipeline = QADiscourse_Pipeline(qadiscourse_model_name, device=device)
+            self.qa_discourse_pipeline = QADiscourse_Pipeline(qadiscourse_model_name, 
+                                                              device=device, 
+                                                              spacy_model=self.spacy_model_name)
 
         self.contextualize = contextualize
         self.return_qasrl_slots = return_qasrl_slots
         self.return_qasrl_discrete_role = return_qasrl_discrete_role
-        self.spacy_model_name = spacy_model or DEFAULT_SPACY_MODEL
 
         if self.contextualize:
             self.q_translator = QuestionContextualizer.from_pretrained(question_contextualization_model_name, device_id=device)
 
         self.openie_converter = OpenIEConverter(**openie_converter_kwargs)
```

### Comparing `qasem-0.2.1/qasem/openie_converter.py` & `qasem-0.2.2/qasem/openie_converter.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.1/qasem/qa_adj_pipeline.py` & `qasem-0.2.2/qasem/qa_adj_pipeline.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.1/qasem/qa_discourse_pipeline.py` & `qasem-0.2.2/qasem/qa_discourse_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from argparse import Namespace
 from transformers import Text2TextGenerationPipeline, AutoModelForSeq2SeqLM, AutoTokenizer
 from qasem.candidates_finder import CandidateFinder
 
 def get_markers_for_model():
     special_tokens_constants = Namespace()
     special_tokens_constants.separator_different_qa = "&&&"
@@ -21,21 +22,21 @@
     """
     words1 = str1.split()
     words2 = str2.split()
     covered = [w for w in words1 if w in words2]
     return len(covered) / len(words1)
 
 class QADiscourse_Pipeline(Text2TextGenerationPipeline):
-    def __init__(self, model_repo: str, device=-1, **kwargs):
+    def __init__(self, model_repo: str, device=-1, spacy_model: Optional[str] = None, **kwargs):
         " :param device: -1 for CPU (default), >=0 refers to CUDA device ordinal. "
         model, tokenizer = load_trained_model(model_repo)
         super().__init__(model, tokenizer, device=device, framework="pt")
         self.special_tokens = get_markers_for_model()
         self._update_config(**kwargs)
-        self.cand_finder = CandidateFinder()
+        self.cand_finder = CandidateFinder(spacy_model=spacy_model)
 
     def _update_config(self, **kwargs):
         " Update self.model.config with initialization parameters and necessary defaults. "
         # set default values that will always override model.config, but can overriden by __init__ kwargs
         kwargs["max_length"] = kwargs.get("max_length", 120)
         # override model.config with kwargs
         for k, v in kwargs.items():
```

### Comparing `qasem-0.2.1/qasem/question_contextualizer.py` & `qasem-0.2.2/qasem/question_contextualizer.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.1/qasem/spacy_loader.py` & `qasem-0.2.2/qasem/spacy_loader.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.1/qasem/test_end_to_end_pipeline.py` & `qasem-0.2.2/qasem/test_end_to_end_pipeline.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.1/qasem.egg-info/PKG-INFO` & `qasem-0.2.2/qasem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qasem
-Version: 0.2.1
+Version: 0.2.2
 Summary: package for QA-based Semantics - representing textual information via question-answer pairs
 Home-page: https://github.com/kleinay/QASem
 Author: Ayal Klein, Ruben Wolhandler, Ron Eliav
 Author-email: ayal.s.klein@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qasem-0.2.1/setup.py` & `qasem-0.2.2/setup.py`

 * *Files identical despite different names*

