# Comparing `tmp/qanom-0.0.6.tar.gz` & `tmp/qanom-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qanom-0.0.6.tar", last modified: Thu Dec  2 11:58:25 2021, max compression
+gzip compressed data, was "dist/qanom-0.0.9.tar", last modified: Sun Jan  9 22:09:31 2022, max compression
```

## Comparing `qanom-0.0.6.tar` & `qanom-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2021-12-02 11:58:25.899799 qanom-0.0.6/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1077 2021-09-30 07:40:14.000000 qanom-0.0.6/LICENSE
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      174 2021-12-02 11:31:59.000000 qanom-0.0.6/MANIFEST.in
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)    13046 2021-12-02 11:58:25.899799 qanom-0.0.6/PKG-INFO
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)    12533 2021-12-01 19:52:06.000000 qanom-0.0.6/README.md
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2021-12-02 11:58:25.899799 qanom-0.0.6/qanom/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      233 2021-12-02 11:05:52.000000 qanom-0.0.6/qanom/__init__.py
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2021-12-02 11:58:25.899799 qanom-0.0.6/qanom/annotations/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        0 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/annotations/__init__.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5902 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/annotations/analyze.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     6768 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/annotations/common.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8564 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/annotations/consolidation.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8202 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/annotations/decode_encode_answers.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)    21547 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/annotations/post_processing.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7621 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/annotations/qasrlv2_jsonl.py
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2021-12-02 11:58:25.899799 qanom-0.0.6/qanom/candidate_extraction/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        0 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/candidate_extraction/__init__.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      941 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/candidate_extraction/cand_utils.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)    12551 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/candidate_extraction/candidate_extraction.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1404 2021-12-01 19:55:48.000000 qanom-0.0.6/qanom/candidate_extraction/catvar.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7494 2021-12-02 11:51:27.000000 qanom-0.0.6/qanom/candidate_extraction/verb_to_nom.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2668 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/candidate_extraction/wordnet_util.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      207 2021-12-02 11:05:29.000000 qanom-0.0.6/qanom/config.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      676 2021-10-13 11:01:44.000000 qanom-0.0.6/qanom/evaluate.py
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2021-12-02 11:58:25.899799 qanom-0.0.6/qanom/evaluation/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        0 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/evaluation/__init__.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2410 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/evaluation/alignment.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)    10674 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/evaluation/evaluate.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7441 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/evaluation/evaluate_inter_annotator.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2349 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/evaluation/evaluate_worker.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5842 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/evaluation/metrics.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     4155 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/evaluation/roles.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2168 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/extract_candidates.py
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2021-12-02 11:58:25.889799 qanom-0.0.6/qanom/resources/
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2021-12-02 11:58:25.899799 qanom-0.0.6/qanom/resources/catvar/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9751 2021-12-01 20:07:53.000000 qanom-0.0.6/qanom/resources/catvar/LICENSE.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5464 2021-12-01 20:07:53.000000 qanom-0.0.6/qanom/resources/catvar/README.md
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)  1158210 2021-12-01 20:07:53.000000 qanom-0.0.6/qanom/resources/catvar/catvar21.signed
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     6593 2021-09-30 07:40:14.000000 qanom-0.0.6/qanom/utils.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        5 2021-12-02 11:58:08.000000 qanom-0.0.6/qanom/version.txt
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2021-12-02 11:58:25.899799 qanom-0.0.6/qanom.egg-info/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)    13046 2021-12-02 11:58:25.000000 qanom-0.0.6/qanom.egg-info/PKG-INFO
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1125 2021-12-02 11:58:25.000000 qanom-0.0.6/qanom.egg-info/SOURCES.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        1 2021-12-02 11:58:25.000000 qanom-0.0.6/qanom.egg-info/dependency_links.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)       77 2021-12-02 11:58:25.000000 qanom-0.0.6/qanom.egg-info/requires.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        6 2021-12-02 11:58:25.000000 qanom-0.0.6/qanom.egg-info/top_level.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)       79 2021-12-02 11:58:25.899799 qanom-0.0.6/setup.cfg
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1136 2021-12-02 11:22:47.000000 qanom-0.0.6/setup.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2022-01-09 22:09:31.000000 qanom-0.0.9/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1077 2022-01-06 13:11:12.000000 qanom-0.0.9/LICENSE
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      174 2022-01-06 13:11:12.000000 qanom-0.0.9/MANIFEST.in
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    13046 2022-01-09 22:09:31.000000 qanom-0.0.9/PKG-INFO
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    12533 2022-01-06 13:11:12.000000 qanom-0.0.9/README.md
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      233 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/__init__.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom/annotations/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        0 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/annotations/__init__.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5902 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/annotations/analyze.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     6768 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/annotations/common.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8564 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/annotations/consolidation.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8202 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/annotations/decode_encode_answers.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    21547 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/annotations/post_processing.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7621 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/annotations/qasrlv2_jsonl.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom/candidate_extraction/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        0 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/candidate_extraction/__init__.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      941 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/candidate_extraction/cand_utils.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    12551 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/candidate_extraction/candidate_extraction.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1404 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/candidate_extraction/catvar.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7494 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/candidate_extraction/verb_to_nom.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2668 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/candidate_extraction/wordnet_util.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      207 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/config.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      676 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/evaluate.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom/evaluation/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        0 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/evaluation/__init__.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2410 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/evaluation/alignment.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    10674 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/evaluation/evaluate.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7441 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/evaluation/evaluate_inter_annotator.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2349 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/evaluation/evaluate_worker.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5842 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/evaluation/metrics.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     4155 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/evaluation/roles.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2168 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/extract_candidates.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5188 2022-01-09 22:03:57.000000 qanom-0.0.9/qanom/nominalization_detector.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom/resources/
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom/resources/catvar/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9751 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/resources/catvar/LICENSE.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5464 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/resources/catvar/README.md
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)  1158210 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/resources/catvar/catvar21.signed
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     6593 2022-01-06 13:11:12.000000 qanom-0.0.9/qanom/utils.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        5 2022-01-09 22:06:18.000000 qanom-0.0.9/qanom/version.txt
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom.egg-info/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    13046 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom.egg-info/PKG-INFO
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1158 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom.egg-info/SOURCES.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        1 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom.egg-info/dependency_links.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       77 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom.egg-info/requires.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        6 2022-01-09 22:09:31.000000 qanom-0.0.9/qanom.egg-info/top_level.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       79 2022-01-09 22:09:31.000000 qanom-0.0.9/setup.cfg
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1136 2022-01-06 13:11:12.000000 qanom-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `qanom-0.0.6/LICENSE` & `qanom-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/PKG-INFO` & `qanom-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qanom
-Version: 0.0.6
+Version: 0.0.9
 Summary: package for Question-Answer driven Semantic Role Labeling for Nominalizations (QANom)
 Home-page: https://github.com/kleinay/QANom
 Author: Ayal Klein
 Author-email: ayal.s.klein@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -37,15 +37,15 @@
 The original QANom Dataset can be downloaded from this
  [google drive directory](https://drive.google.com/drive/folders/15PHKVdPm65ysgdkV47z6J_73kETk7_of).
  
  Alternatively, if you are working with Huggingface's [Datasets](https://github.com/huggingface/datasets) library or are willing to install it (`pip install datasets`), 
  you can retrieve the QANom datasets by:
  ```python
  import datasets
- qanom_dataset = datasets.load_dataset('kleinay/qanom')
+ qanom_dataset = datasets.load_dataset('biu-nlp/qanom')
  ```
 
 ## Crowdsourcing QANom via MTurk
 
 The QANom dataset was collected through [Amazon Mechanical Turk](https://www.mturk.com/) (MTurk). 
 It was annotated by pre-selected crowd workers who exhibited good performance when previously annotating QA-SRL.
 Workers first thoroughly read and comprehend the **annotation guidelines** -
```

### Comparing `qanom-0.0.6/README.md` & `qanom-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 The original QANom Dataset can be downloaded from this
  [google drive directory](https://drive.google.com/drive/folders/15PHKVdPm65ysgdkV47z6J_73kETk7_of).
  
  Alternatively, if you are working with Huggingface's [Datasets](https://github.com/huggingface/datasets) library or are willing to install it (`pip install datasets`), 
  you can retrieve the QANom datasets by:
  ```python
  import datasets
- qanom_dataset = datasets.load_dataset('kleinay/qanom')
+ qanom_dataset = datasets.load_dataset('biu-nlp/qanom')
  ```
 
 ## Crowdsourcing QANom via MTurk
 
 The QANom dataset was collected through [Amazon Mechanical Turk](https://www.mturk.com/) (MTurk). 
 It was annotated by pre-selected crowd workers who exhibited good performance when previously annotating QA-SRL.
 Workers first thoroughly read and comprehend the **annotation guidelines** -
```

### Comparing `qanom-0.0.6/qanom/annotations/analyze.py` & `qanom-0.0.9/qanom/annotations/analyze.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/annotations/common.py` & `qanom-0.0.9/qanom/annotations/common.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/annotations/consolidation.py` & `qanom-0.0.9/qanom/annotations/consolidation.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/annotations/decode_encode_answers.py` & `qanom-0.0.9/qanom/annotations/decode_encode_answers.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/annotations/post_processing.py` & `qanom-0.0.9/qanom/annotations/post_processing.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/annotations/qasrlv2_jsonl.py` & `qanom-0.0.9/qanom/annotations/qasrlv2_jsonl.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/candidate_extraction/cand_utils.py` & `qanom-0.0.9/qanom/candidate_extraction/cand_utils.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/candidate_extraction/candidate_extraction.py` & `qanom-0.0.9/qanom/candidate_extraction/candidate_extraction.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/candidate_extraction/catvar.py` & `qanom-0.0.9/qanom/candidate_extraction/catvar.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/candidate_extraction/verb_to_nom.py` & `qanom-0.0.9/qanom/candidate_extraction/verb_to_nom.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/candidate_extraction/wordnet_util.py` & `qanom-0.0.9/qanom/candidate_extraction/wordnet_util.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/evaluate.py` & `qanom-0.0.9/qanom/evaluate.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/evaluation/alignment.py` & `qanom-0.0.9/qanom/evaluation/alignment.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/evaluation/evaluate.py` & `qanom-0.0.9/qanom/evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/evaluation/evaluate_inter_annotator.py` & `qanom-0.0.9/qanom/evaluation/evaluate_inter_annotator.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/evaluation/evaluate_worker.py` & `qanom-0.0.9/qanom/evaluation/evaluate_worker.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/evaluation/metrics.py` & `qanom-0.0.9/qanom/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/evaluation/roles.py` & `qanom-0.0.9/qanom/evaluation/roles.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/extract_candidates.py` & `qanom-0.0.9/qanom/extract_candidates.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/resources/catvar/LICENSE.txt` & `qanom-0.0.9/qanom/resources/catvar/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/resources/catvar/README.md` & `qanom-0.0.9/qanom/resources/catvar/README.md`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/resources/catvar/catvar21.signed` & `qanom-0.0.9/qanom/resources/catvar/catvar21.signed`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom/utils.py` & `qanom-0.0.9/qanom/utils.py`

 * *Files identical despite different names*

### Comparing `qanom-0.0.6/qanom.egg-info/PKG-INFO` & `qanom-0.0.9/qanom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qanom
-Version: 0.0.6
+Version: 0.0.9
 Summary: package for Question-Answer driven Semantic Role Labeling for Nominalizations (QANom)
 Home-page: https://github.com/kleinay/QANom
 Author: Ayal Klein
 Author-email: ayal.s.klein@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -37,15 +37,15 @@
 The original QANom Dataset can be downloaded from this
  [google drive directory](https://drive.google.com/drive/folders/15PHKVdPm65ysgdkV47z6J_73kETk7_of).
  
  Alternatively, if you are working with Huggingface's [Datasets](https://github.com/huggingface/datasets) library or are willing to install it (`pip install datasets`), 
  you can retrieve the QANom datasets by:
  ```python
  import datasets
- qanom_dataset = datasets.load_dataset('kleinay/qanom')
+ qanom_dataset = datasets.load_dataset('biu-nlp/qanom')
  ```
 
 ## Crowdsourcing QANom via MTurk
 
 The QANom dataset was collected through [Amazon Mechanical Turk](https://www.mturk.com/) (MTurk). 
 It was annotated by pre-selected crowd workers who exhibited good performance when previously annotating QA-SRL.
 Workers first thoroughly read and comprehend the **annotation guidelines** -
```

### Comparing `qanom-0.0.6/qanom.egg-info/SOURCES.txt` & `qanom-0.0.9/qanom.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.cfg
 setup.py
 qanom/__init__.py
 qanom/config.py
 qanom/evaluate.py
 qanom/extract_candidates.py
+qanom/nominalization_detector.py
 qanom/utils.py
 qanom/version.txt
 qanom.egg-info/PKG-INFO
 qanom.egg-info/SOURCES.txt
 qanom.egg-info/dependency_links.txt
 qanom.egg-info/requires.txt
 qanom.egg-info/top_level.txt
```

### Comparing `qanom-0.0.6/setup.py` & `qanom-0.0.9/setup.py`

 * *Files identical despite different names*

