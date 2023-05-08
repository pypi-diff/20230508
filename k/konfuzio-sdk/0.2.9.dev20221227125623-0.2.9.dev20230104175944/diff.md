# Comparing `tmp/konfuzio_sdk-0.2.9.dev20221227125623.tar.gz` & `tmp/konfuzio_sdk-0.2.9.dev20230104175944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.2.9.dev20221227125623.tar", last modified: Wed Dec 28 03:29:41 2022, max compression
+gzip compressed data, was "konfuzio_sdk-0.2.9.dev20230104175944.tar", last modified: Thu Jan  5 03:29:15 2023, max compression
```

## Comparing `konfuzio_sdk-0.2.9.dev20221227125623.tar` & `konfuzio_sdk-0.2.9.dev20230104175944.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 03:29:41.719931 konfuzio_sdk-0.2.9.dev20221227125623/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2022-12-28 03:29:41.719931 konfuzio_sdk-0.2.9.dev20221227125623/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 03:29:41.715931 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   123558 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24739 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 03:29:41.719931 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 03:29:41.719931 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (123)   108856 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    40041 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 03:29:41.715931 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2022-12-28 03:29:41.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2022-12-28 03:29:41.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 03:29:41.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-28 03:29:41.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2022-12-28 03:29:41.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-28 03:29:41.000000 konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-28 03:29:41.719931 konfuzio_sdk-0.2.9.dev20221227125623/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2022-12-28 03:29:32.000000 konfuzio_sdk-0.2.9.dev20221227125623/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.630517 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123551 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107540 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40041 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/setup.py
```

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/LICENSE.md` & `konfuzio_sdk-0.2.9.dev20230104175944/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/PKG-INFO` & `konfuzio_sdk-0.2.9.dev20230104175944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.2.9.dev20221227125623
+Version: 0.2.9.dev20230104175944
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
```

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/README.md` & `konfuzio_sdk-0.2.9.dev20230104175944/README.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/api.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/data.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,15 +780,15 @@
             logger.error(f"We cannot find annotations for Label {self} and Category {category}.")
             return []
 
         label_regex_token = self.base_regex(category=category, annotations=all_annotations)
 
         search = [1, 3, 5]
         regex_to_remove_groupnames = re.compile(r'<.*?>')
-        regex_to_remove_groupnames_full = re.compile(r'\(\?:\(\?P<[^>]+>([^\)]+)\)\)')
+        regex_to_remove_groupnames_full = re.compile(r'\?P<.*?>')
 
         naive_proposal = label_regex_token
         regex_made = []
         regex_found = set()
 
         for annotation in all_annotations:
             new_proposals = []
@@ -806,17 +806,15 @@
                         if before_span.annotation.label is self.project.no_label:
                             to_rep_offset_string = before_span.annotation.document.text[
                                 max(before_start_offset, before_span.start_offset) : before_span.end_offset
                             ]
                             before_regex += suggest_regex_for_string(to_rep_offset_string, replace_characters=True)
                         else:
                             base_before_regex = before_span.annotation.label.base_regex(category)
-                            stripped_base_before_regex = re.sub(
-                                regex_to_remove_groupnames_full, r'\1', base_before_regex
-                            )
+                            stripped_base_before_regex = re.sub(regex_to_remove_groupnames_full, '', base_before_regex)
                             before_regex += stripped_base_before_regex
                     before_reg_dict[spacer] = before_regex
 
                     after_regex = ''
                     after_end_offset = span.end_offset + spacer
                     for after_span in annotation.document.spans(
                         fill=True, start_offset=span.end_offset, end_offset=after_end_offset
@@ -824,15 +822,15 @@
                         if after_span.annotation.label is self.project.no_label:
                             to_rep_offset_string = after_span.annotation.document.text[
                                 after_span.start_offset : min(after_end_offset, after_span.end_offset)
                             ]
                             after_regex += suggest_regex_for_string(to_rep_offset_string, replace_characters=True)
                         else:
                             base_after_regex = after_span.annotation.label.base_regex(category)
-                            stripped_base_after_regex = re.sub(regex_to_remove_groupnames_full, r'\1', base_after_regex)
+                            stripped_base_after_regex = re.sub(regex_to_remove_groupnames_full, '', base_after_regex)
                             after_regex += stripped_base_after_regex
 
                     after_reg_dict[spacer] = after_regex
 
                     spacer_proposals = [
                         before_regex + label_regex_token + after_regex,
                         before_reg_dict[search[0]] + label_regex_token + after_regex,
@@ -2375,14 +2373,15 @@
 
     def merge_vertical(self, only_multiline_labels=True):
         """
         Merge Annotations with the same Label.
 
         :param only_multiline_labels: Only merge if multiline Label Annotation in category training set
         """
+        logger.info("Vertical merging Annotations.")
         labels_dict = {}
         for label in self.project.labels:
             if not only_multiline_labels or label.has_multiline_annotations(categories=[self.category]):
                 labels_dict[label.id_local] = []
 
         for annotation in self.annotations(use_correct=False, ignore_below_threshold=True):
             if annotation.label.id_local in labels_dict:
@@ -2875,14 +2874,15 @@
         for category in self.categories:
             category.lose_weight()
         for label_set in self.label_sets:
             label_set.lose_weight()
         for label in self.labels:
             label.lose_weight()
         self._documents = []
+        self._meta_data = []
         return self
 
 
 def download_training_and_test_data(id_: int):
     """
     Migrate your project to another HOST.
```

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/settings_importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,23 @@
 
 LOG_FILE_PATH = os.path.join(os.getcwd(), 'konfuzio_sdk.log')
 LOG_FORMAT = (
     "%(asctime)s [%(name)-20.20s] [%(threadName)-10.10s] [%(levelname)-8.8s] "
     "[%(funcName)-20.20s][%(lineno)-4.4d] %(message)-10s"
 )
 
-handlers = [logging.StreamHandler()]
 
-if config('LOG_TO_FILE', cast=bool, default=True):
-    with open(LOG_FILE_PATH, "a") as f:
-        if f.writable():
-            handlers.append(logging.FileHandler(LOG_FILE_PATH))
+def get_handlers():
+    """Get logging handlers based on environment variables."""
+    handlers = [logging.StreamHandler()]
 
+    if config('LOG_TO_FILE', cast=bool, default=True):
+        with open(LOG_FILE_PATH, "a") as f:
+            if f.writable():
+                handlers.append(logging.FileHandler(LOG_FILE_PATH))
 
-logging.basicConfig(level=config('LOGGING_LEVEL', default=logging.INFO, cast=int), format=LOG_FORMAT, handlers=handlers)
+    return handlers
+
+
+logging.basicConfig(
+    level=config('LOGGING_LEVEL', default=logging.INFO, cast=int), format=LOG_FORMAT, handlers=get_handlers()
+)
```

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/document_categorization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/information_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Sun, H., Kuang, Z., Yue, X., Lin, C., & Zhang, W. (2021). Spatial Dual-Modality Graph Reasoning for Key Information
 Extraction. arXiv. https://doi.org/10.48550/ARXIV.2103.14470
 """
 import bz2
 import collections
 import difflib
 import functools
+import itertools
 import logging
 import os
 import pathlib
 import shutil
 import sys
 import time
 import unicodedata
@@ -34,16 +35,15 @@
 import pandas
 import cloudpickle
 from pympler import asizeof
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.utils.validation import check_is_fitted
 from tabulate import tabulate
 
-import konfuzio_sdk
-from konfuzio_sdk.data import Document, Annotation, Category, AnnotationSet, Label, LabelSet, Span
+from konfuzio_sdk.data import Data, Document, Annotation, Category, AnnotationSet, Label, LabelSet, Span
 from konfuzio_sdk.normalize import (
     normalize_to_float,
     normalize_to_date,
     normalize_to_percentage,
     normalize_to_positive_float,
 )
 from konfuzio_sdk.regex import regex_matches
@@ -67,14 +67,17 @@
     :raises OSError: When the data is corrupted or invalid and cannot be loaded.
     :raises TypeError: When the loaded pickle isn't recognized as a Konfuzio AI model.
     :return: Extraction AI model.
     """
     if not os.path.isfile(pickle_path):
         raise FileNotFoundError("Invalid pickle file path:", pickle_path)
 
+    # The current local id iterator might otherwise be overriden
+    prev_local_id = next(Data.id_iter)
+
     try:
         with bz2.open(pickle_path, 'rb') as file:
             model = cloudpickle.load(file)
     except OSError:
         raise OSError(f"Pickle file {pickle_path} data is invalid.")
     except AttributeError as err:
         if "__forward_module__" in str(err) and '3.9' in sys.version:
@@ -99,14 +102,17 @@
         "SeparateLabelsAnnotationMultiClassModel",
         "SeparateLabelsEntityMultiClassModel",
     }:
         logger.warning(f"Loading legacy {model.name} AI model.")
     else:
         logger.info(f"Loading {model.name} AI model.")
 
+    curr_local_id = next(Data.id_iter)
+    Data.id_iter = itertools.count(max(prev_local_id, curr_local_id))
+
     return model
 
 
 def get_offsets_per_page(doc_text: str) -> Dict:
     """Get the first start and last end offsets per page."""
     page_text = doc_text.split('\f')
     start = 0
@@ -1204,100 +1210,37 @@
     """Base Model to extract information from unstructured human readable text."""
 
     def __init__(self, *args, **kwargs):
         """Initialize ExtractionModel."""
         # Go through keyword arguments, and either save their values to our
         # instance, or raise an error.
         self.clf = None
-        self.category = None
         self.name = self.__class__.__name__
         self.label_feature_list = None  # will be set later
 
         self.df_train = None
-        self.df_test = None
 
         self.evaluation = None
 
-    def build(self, **kwargs):
-        """Build an ExtractionModel using train valid split."""
-        self.create_candidates_dataset()
-        self.train_valid_split()
-        self.fit()
-        self.evaluate()
-        self.lose_weight()
-        return self
-
     def name_lower(self):
         """Convert class name to machine readable name."""
         return f'{self.name.lower().strip()}'
 
-    def lose_weight(self):
-        """Delete everything that is not necessary for extraction."""
-        self.df_valid = None
-        self.df_train = None
-        self.df_test = None
-
-        self.X_train = None
-        self.y_train = None
-        self.X_valid = None
-        self.y_valid = None
-        self.X_test = None
-        self.y_test = None
-
-        # TODO what is this?
-        self.valid_data = None
-        self.training_data = None
-        self.test_data = None
-
-        self.df_data_list = None
-
-        for label in self.category.project.labels:
-            label.lose_weight()
-
-        for label_set in self.category.label_sets or []:
-            label_set.lose_weight()
-
-        logger.info(f'Lose weight was executed on {self.name}')
-
-    # def get_ai_model(self):
-    #     """Try to load the latest pickled model."""
-    #     try:
-    #         return load_pickle(get_latest_document_model(f'*_{self.name_lower()}.pkl'))
-    #     except FileNotFoundError:
-    #         return None
-
-    def create_candidates_dataset(self):
-        """Use as placeholder Function."""
-        logger.warning(f'{self} does not train a classifier.')
-        pass
-
-    def train_valid_split(self):
-        """Use as placeholder Function."""
-        logger.warning(f'{self} does not use a valid and train data split.')
-        pass
-
     def fit(self):
         """Use as placeholder Function."""
         logger.warning(f'{self} does not train a classifier.')
         pass
 
-    def fit_label_set_clf(self):
-        """Use as placeholder Function."""
-        logger.warning(f'{self} does not train a label set classifier.')
-        pass
-
     def evaluate(self):
         """Use as placeholder Function."""
         logger.warning(f'{self} does not evaluate results.')
         pass
 
-    def extract(self, *args, **kwargs):
+    def extract(self):
         """Use as placeholder Function."""
-        # todo: extract should return a Document
-        #  see https://github.com/konfuzio-ai/konfuzio-sdk/blob/64fd8792/konfuzio_sdk/data.py#L1182
         logger.warning(f'{self} does not extract.')
         pass
 
     def extraction_result_to_document(self, document: Document, extraction_result: dict) -> Document:
         """Return a virtual Document annotated with AI Model output."""
         virtual_doc = deepcopy(document)
         virtual_annotation_set_id = 1  # counter for across mult. Annotation Set groups of a Label Set
@@ -1484,43 +1427,45 @@
         :param include_konfuzio: Boolean whether to include konfuzio_sdk package in pickle file.
         :param reduce_weight: Remove all non-strictly necessary parameters before saving.
         :param max_ram: Specify maximum memory usage condition to save model.
         :raises MemoryError: When the size of the model in memory is greater than the maximum value.
         :return: Path of the saved model file.
         """
         logger.info('Saving model')
+
+        self.check_is_ready_for_extraction()
+
+        logger.info(f'{output_dir=}')
         logger.info(f'{include_konfuzio=}')
         logger.info(f'{reduce_weight=}')
         logger.info(f'{keep_documents=}')
         logger.info(f'{max_ram=}')
 
-        # Keep Documents of the Category so that we can restore them later
-
-        # TODO: add Document.lose_weight in SDK - remove NO_LABEL Annotations from the Documents
-        # for document in category_documents:
-        #     no_label_annotations = document.annotations(label=self.category.project.no_label)
-        #     clean_annotations = list(set(document.annotations()) - set(no_label_annotations))
-        #     document._annotations = clean_annotations
-
         # if no argument passed, get project max_ram
         if not max_ram and self.category is not None:
             max_ram = self.category.project.max_ram
+            logger.info(f'project {max_ram=}')
 
         if not output_dir:
             output_dir = self.category.project.model_folder
+            logger.info(f'new {output_dir=}')
 
         temp_pkl_file_path = os.path.join(output_dir, f'{get_timestamp()}_{self.category.name.lower()}.cloudpickle')
         pkl_file_path = os.path.join(output_dir, f'{get_timestamp()}_{self.category.name.lower()}.pkl')
 
         if reduce_weight:
+            logger.info('reducing weight before save')
             self.df_train = None
             self.category.project.lose_weight()
             self.tokenizer.lose_weight()
 
         if not keep_documents:
+            logger.info('removing documents before save')
+            restore_documents = self.documents
+            restore_test_documents = self.test_documents
             self.documents = []
             self.test_documents = []
 
         logger.info(f'Model size: {asizeof.asizeof(self) / 1_000_000} MB')
 
         max_ram = normalize_memory(max_ram)
 
@@ -1528,20 +1473,19 @@
             raise MemoryError(f"AI model memory use ({asizeof.asizeof(self)}) exceeds maximum ({max_ram=}).")
 
         sys.setrecursionlimit(999999)  # ?
 
         logger.info('Getting save paths')
 
         if include_konfuzio:
+            import konfuzio_sdk
+
             cloudpickle.register_pickle_by_value(konfuzio_sdk)
             # todo register all dependencies?
 
-        if not output_dir:
-            output_dir = self.category.project.model_folder
-
         # make sure output dir exists
         pathlib.Path(output_dir).mkdir(parents=True, exist_ok=True)
 
         logger.info('Saving model with cloudpickle')
         # first save with cloudpickle
         with open(temp_pkl_file_path, 'wb') as f:  # see: https://stackoverflow.com/a/9519016/5344492
             cloudpickle.dump(self, f)
@@ -1557,30 +1501,33 @@
         # then delete cloudpickle file
         os.remove(temp_pkl_file_path)
 
         size_string = f'{os.path.getsize(pkl_file_path) / 1_000_000} MB'
         logger.info(f'Model ({size_string}) {self.name_lower()} was saved to {pkl_file_path}')
 
         # restore Documents of the Category so that we can run the evaluation later
-        # self.category.project._documents = category_documents
+        self.documents = restore_documents
+        self.test_documents = restore_test_documents
+        if reduce_weight:
+            self.category.project.init_or_update_document()
 
         return pkl_file_path
 
 
 class GroupAnnotationSets:
     """Groups Annotation into Annotation Sets."""
 
     def __init__(self):
         """Initialize TemplateClf."""
         self.n_nearest_template = 5
         self.max_depth = 100
         self.n_estimators = 100
-        self.template_clf = None
+        self.label_set_clf = None
 
-    def fit_template_clf(self) -> Tuple[Optional[object], Optional[List['str']]]:
+    def fit_label_set_clf(self) -> Tuple[Optional[object], Optional[List['str']]]:
         """
         Fit classifier to predict start lines of Sections.
 
         :param documents:
         :return:
         """
         # Only train template clf is there are non default templates
@@ -1647,19 +1594,21 @@
         # No features available
         if x_train.empty:
             logger.error(
                 'No features available to train template classifier, ' 'probably because there are no annotations.'
             )
             return None, None
 
-        clf = RandomForestClassifier(n_estimators=self.n_estimators, max_depth=self.max_depth, random_state=420)
-        clf.fit(x_train, y_train)
+        label_set_clf = RandomForestClassifier(
+            n_estimators=self.n_estimators, max_depth=self.max_depth, random_state=420
+        )
+        label_set_clf.fit(x_train, y_train)
 
-        self.template_clf = clf
-        return self.template_clf, self.template_feature_list
+        self.label_set_clf = label_set_clf
+        return self.label_set_clf, self.template_feature_list
 
     def generate_relative_line_features(self, n_nearest: int, df_features: pandas.DataFrame) -> pandas.DataFrame:
         """Add the features of the n_nearest previous and next lines."""
         if n_nearest == 0:
             return df_features
 
         min_row = 0
@@ -1692,15 +1641,15 @@
 
         return pandas.DataFrame(df_features_new_list)
 
     def convert_label_features_to_template_features(
         self, feature_df_label: pandas.DataFrame, document_text
     ) -> pandas.DataFrame:
         """
-        Convert the feature_df for the label_clf to a feature_df for the template_clf.
+        Convert the feature_df for the label_clf to a feature_df for the label_set_clf.
 
         The input is the Feature-Dataframe and text for one document.
         """
         # reset indices to avoid bugs with stupid NaN's as label_text
         feature_df_label.reset_index(drop=True, inplace=True)
 
         # predict and transform the DataFrame to be compatible with the other functions
@@ -1813,15 +1762,15 @@
         n_nearest = self.n_nearest_template if hasattr(self, 'n_nearest_template') else 0
         feature_df = self.build_document_template_feature_X(text, dict_to_dataframe(res_dict)).filter(
             self.template_feature_list, axis=1
         )
         feature_df = feature_df.reindex(columns=self.template_feature_list).fillna(0)
         feature_df = self.generate_relative_line_features(n_nearest, feature_df)
 
-        res_series = self.template_clf.predict(feature_df)
+        res_series = self.label_set_clf.predict(feature_df)
         res_templates = pandas.DataFrame(res_series)
         # res_templates['text'] = text.replace('\f', '\n').split('\n')  # Debug code.
 
         # TODO improve ordering. What happens if Annotations are not matched?
         logger.info('Building new res dict')
         new_res_dict = {}
         text_replaced = text.replace('\f', '\n')
@@ -1945,38 +1894,36 @@
         use_separate_labels: bool = False,
         category: Category = None,
         tokenizer=None,
         *args,
         **kwargs,
     ):
         """RFExtractionAI."""
-        logging.info("Initializing RFExtractionAI.")
+        logger.info("Initializing RFExtractionAI.")
         super().__init__(*args, **kwargs)
         GroupAnnotationSets.__init__(self)
 
         self.label_feature_list = None
 
-        self.use_separate_labels = use_separate_labels
+        logger.info("RFExtractionAI settings:")
         logger.info(f"{use_separate_labels=}")
-
-        self.category: Category = category
         logger.info(f"{category=}")
-
-        self.n_nearest = n_nearest
         logger.info(f"{n_nearest=}")
-
-        self.first_word = first_word
         logger.info(f"{first_word=}")
-
-        self.max_depth = max_depth
         logger.info(f"{max_depth=}")
-
-        self.n_estimators = n_estimators
         logger.info(f"{n_estimators=}")
+        logger.info(f"{no_label_limit=}")
+        logger.info(f"{n_nearest_across_lines=}")
 
+        self.use_separate_labels = use_separate_labels
+        self.category = category
+        self.n_nearest = n_nearest
+        self.first_word = first_word
+        self.max_depth = max_depth
+        self.n_estimators = n_estimators
         self.no_label_limit = no_label_limit
         self.n_nearest_across_lines = n_nearest_across_lines
 
         self.substring_features = kwargs.get('substring_features', None)
         self.catchphrase_features = kwargs.get('catchphrase_features', None)
 
         self.tokenizer = tokenizer
@@ -2005,37 +1952,45 @@
         )
         if self.use_separate_labels:
             df['target'] = df['label_set_name'] + '__' + df['label_name']
         else:
             df['target'] = df['label_name']
         return df, _feature_list, _temp_df_raw_errors
 
+    def check_is_ready_for_extraction(self):
+        """Check if tokenizer is set and the classifiers set and trained."""
+        if self.tokenizer is None:
+            raise AttributeError(f'{self} missing Tokenizer.')
+
+        if not self.category:
+            raise AttributeError(f'{self} requires a Category.')
+
+        if self.clf is None:
+            raise AttributeError(f'{self} does not provide a Label Classifier. Please add it.')
+        else:
+            check_is_fitted(self.clf)
+
+        if self.label_set_clf is None:
+            logger.warning('{self} does not provide a LabelSet Classfier.')
+
     def extract(self, document: Document) -> Document:
         """
         Infer information from a given Document.
 
         :param document: Document object
         :return: Document with predicted labels
 
         :raises:
          AttributeError: When missing a Tokenizer
          NotFittedError: When CLF is not fitted
 
         """
         logger.info(f"Starting extraction of {document}.")
-        if self.tokenizer is None:
-            raise AttributeError(f'{self} missing Tokenizer.')
 
-        if self.clf is None:
-            raise AttributeError(f'{self} does not provide a Label Classifier. Please add it.')
-        else:
-            check_is_fitted(self.clf)
-
-        if self.template_clf is None:
-            logger.warning('{self} does not provide a LabelSet Classfier.')
+        self.check_is_ready_for_extraction()
 
         # Main Logic -------------------------
         # 1. start inference with new document
         inference_document = deepcopy(document)
         # 2. tokenize
         self.tokenizer.tokenize(inference_document)
         if not inference_document.spans():
@@ -2106,15 +2061,15 @@
         no_label_res_dict = self.remove_empty_dataframes_from_extraction(no_label_res_dict)
 
         # res_dict = self.filter_low_confidence_extractions(res_dict)
 
         res_dict = self.merge_horizontal(res_dict, inference_document.text)
 
         # Try to calculate sections based on template classifier.
-        if self.template_clf is not None:  # todo smarter handling of multiple clf
+        if self.label_set_clf is not None:  # todo smarter handling of multiple clf
             res_dict = self.extract_template_with_clf(inference_document.text, res_dict)
             res_dict[self.no_label_set_name] = no_label_res_dict
 
         if self.use_separate_labels:
             res_dict = self.separate_labels(res_dict)
 
         virtual_doc = self.extraction_result_to_document(inference_document, res_dict)
@@ -2436,15 +2391,15 @@
         # balanced gives every label the same weight so that the sample_number doesn't effect the results
         self.clf = RandomForestClassifier(
             class_weight="balanced", n_estimators=self.n_estimators, max_depth=self.max_depth, random_state=420
         )
 
         self.clf.fit(self.df_train[self.label_feature_list], self.df_train['target'])
 
-        self.fit_template_clf()
+        self.fit_label_set_clf()
 
         return self.clf
 
     def evaluate_full(self, strict: bool = True, use_training_docs: bool = False) -> Evaluation:
         """
         Evaluate the full pipeline on the pipeline's Test Documents.
 
@@ -2507,20 +2462,20 @@
             predicted_doc = self.extract_from_df(feats_df, virtual_doc)
             eval_list.append((document, predicted_doc))
 
         clf_evaluation = Evaluation(eval_list)
 
         return clf_evaluation
 
-    def evaluate_template_clf(self, use_training_docs: bool = False) -> Evaluation:
+    def evaluate_label_set_clf(self, use_training_docs: bool = False) -> Evaluation:
         """Evaluate the LabelSet classifier."""
-        if self.template_clf is None:
+        if self.label_set_clf is None:
             raise AttributeError(f'{self} does not provide a LabelSet Classifier.')
         else:
-            check_is_fitted(self.template_clf)
+            check_is_fitted(self.label_set_clf)
 
         eval_list = []
         if not use_training_docs:
             eval_docs = self.test_documents
         else:
             eval_docs = self.documents
 
@@ -2542,10 +2497,10 @@
             if self.use_separate_labels:
                 res_dict = self.separate_labels(res_dict)
 
             predicted_doc = self.extraction_result_to_document(document, res_dict)
 
             eval_list.append((document, predicted_doc))
 
-        template_clf_evaluation = Evaluation(eval_list)
+        label_set_clf_evaluation = Evaluation(eval_list)
 
-        return template_clf_evaluation
+        return label_set_clf_evaluation
```

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio-sdk
-Version: 0.2.9.dev20221227125623
+Version: 0.2.9.dev20230104175944
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
```

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20221227125623/setup.py` & `konfuzio_sdk-0.2.9.dev20230104175944/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         'Pillow>=7.1.2',
         'python-dateutil',
         'python-decouple',  # todo add ==3.3 ?
         'requests',  # todo add ==2.24.0 ?
         'regex>=2020.6.8',  # re module but better
         'tabulate==0.8.7',  # Used to pretty print DataFrames
         'tqdm',
-        'pathos==0.2.6',
         'pympler==1.0.1',  # Use to get pickle file size.
         'scikit-learn==1.0.2',
     ],
     extras_require={
         'dev': [
             'flake8',
             'pydocstyle',
```

