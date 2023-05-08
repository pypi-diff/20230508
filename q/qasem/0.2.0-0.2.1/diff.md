# Comparing `tmp/qasem-0.2.0.tar.gz` & `tmp/qasem-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qasem-0.2.0.tar", last modified: Mon Apr 17 06:11:34 2023, max compression
+gzip compressed data, was "dist/qasem-0.2.1.tar", last modified: Mon May  8 07:20:42 2023, max compression
```

## Comparing `qasem-0.2.0.tar` & `qasem-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-04-17 06:11:34.000000 qasem-0.2.0/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)       88 2022-07-17 10:30:16.000000 qasem-0.2.0/MANIFEST.in
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-04-17 06:11:34.000000 qasem-0.2.0/PKG-INFO
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8708 2023-04-17 06:10:03.000000 qasem-0.2.0/README.md
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      200 2022-07-17 11:03:06.000000 qasem-0.2.0/qasem/__init__.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7443 2023-03-16 08:20:42.000000 qasem-0.2.0/qasem/candidates_finder.py
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem/data/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5934 2023-01-31 18:04:55.000000 qasem-0.2.0/qasem/data/connectives_small_set.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)    17746 2023-03-16 08:12:00.000000 qasem-0.2.0/qasem/end_to_end_pipeline.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5039 2023-01-04 13:57:20.000000 qasem-0.2.0/qasem/openie_converter.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5041 2023-03-16 08:22:36.000000 qasem-0.2.0/qasem/qa_adj_pipeline.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     4616 2023-01-04 13:57:20.000000 qasem-0.2.0/qasem/qa_discourse_pipeline.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     3232 2023-01-31 14:13:37.000000 qasem-0.2.0/qasem/question_contextualizer.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      845 2023-03-16 08:20:10.000000 qasem-0.2.0/qasem/spacy_loader.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2364 2023-02-05 09:41:21.000000 qasem-0.2.0/qasem/test_end_to_end_pipeline.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      271 2023-02-05 09:41:21.000000 qasem-0.2.0/qasem/utils.py
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        5 2023-04-17 06:09:51.000000 qasem-0.2.0/qasem/version.txt
-drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/PKG-INFO
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)      499 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/SOURCES.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        1 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/dependency_links.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)       53 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/requires.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)        6 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/top_level.txt
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)       79 2023-04-17 06:11:34.000000 qasem-0.2.0/setup.cfg
--rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1235 2023-03-16 08:23:45.000000 qasem-0.2.0/setup.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 07:20:42.000000 qasem-0.2.1/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       88 2022-07-17 10:30:16.000000 qasem-0.2.1/MANIFEST.in
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-05-08 07:20:42.000000 qasem-0.2.1/PKG-INFO
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8708 2023-04-17 06:10:03.000000 qasem-0.2.1/README.md
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      200 2022-07-17 11:03:06.000000 qasem-0.2.1/qasem/__init__.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7443 2023-03-16 08:20:42.000000 qasem-0.2.1/qasem/candidates_finder.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem/data/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5934 2023-01-31 18:04:55.000000 qasem-0.2.1/qasem/data/connectives_small_set.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    17746 2023-03-16 08:12:00.000000 qasem-0.2.1/qasem/end_to_end_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5039 2023-01-04 13:57:20.000000 qasem-0.2.1/qasem/openie_converter.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5041 2023-03-16 08:22:36.000000 qasem-0.2.1/qasem/qa_adj_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     4616 2023-01-04 13:57:20.000000 qasem-0.2.1/qasem/qa_discourse_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     3232 2023-01-31 14:13:37.000000 qasem-0.2.1/qasem/question_contextualizer.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      845 2023-03-16 08:20:10.000000 qasem-0.2.1/qasem/spacy_loader.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2364 2023-02-05 09:41:21.000000 qasem-0.2.1/qasem/test_end_to_end_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      271 2023-02-05 09:41:21.000000 qasem-0.2.1/qasem/utils.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        5 2023-05-08 07:19:34.000000 qasem-0.2.1/qasem/version.txt
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/PKG-INFO
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      499 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/SOURCES.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        1 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/dependency_links.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       53 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/requires.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        6 2023-05-08 07:20:42.000000 qasem-0.2.1/qasem.egg-info/top_level.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       79 2023-05-08 07:20:42.000000 qasem-0.2.1/setup.cfg
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1235 2023-05-08 07:19:23.000000 qasem-0.2.1/setup.py
```

### Comparing `qasem-0.2.0/PKG-INFO` & `qasem-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qasem
-Version: 0.2.0
+Version: 0.2.1
 Summary: package for QA-based Semantics - representing textual information via question-answer pairs
 Home-page: https://github.com/kleinay/QASem
 Author: Ayal Klein, Ruben Wolhandler, Ron Eliav
 Author-email: ayal.s.klein@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qasem-0.2.0/README.md` & `qasem-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/candidates_finder.py` & `qasem-0.2.1/qasem/candidates_finder.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/data/connectives_small_set.txt` & `qasem-0.2.1/qasem/data/connectives_small_set.txt`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/end_to_end_pipeline.py` & `qasem-0.2.1/qasem/end_to_end_pipeline.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/openie_converter.py` & `qasem-0.2.1/qasem/openie_converter.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/qa_adj_pipeline.py` & `qasem-0.2.1/qasem/qa_adj_pipeline.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/qa_discourse_pipeline.py` & `qasem-0.2.1/qasem/qa_discourse_pipeline.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/question_contextualizer.py` & `qasem-0.2.1/qasem/question_contextualizer.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/spacy_loader.py` & `qasem-0.2.1/qasem/spacy_loader.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem/test_end_to_end_pipeline.py` & `qasem-0.2.1/qasem/test_end_to_end_pipeline.py`

 * *Files identical despite different names*

### Comparing `qasem-0.2.0/qasem.egg-info/PKG-INFO` & `qasem-0.2.1/qasem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qasem
-Version: 0.2.0
+Version: 0.2.1
 Summary: package for QA-based Semantics - representing textual information via question-answer pairs
 Home-page: https://github.com/kleinay/QASem
 Author: Ayal Klein, Ruben Wolhandler, Ron Eliav
 Author-email: ayal.s.klein@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qasem-0.2.0/setup.py` & `qasem-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     author_email="ayal.s.klein@gmail.com",
     description="package for QA-based Semantics - representing textual information via question-answer pairs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kleinay/QASem",
     packages=setuptools.find_packages(),
     install_requires=[
-        'qanom>=0.0.31',
+        'qanom>=0.0.32',
         'transformers>=4.15.0',
         'spacy>=3.0.0,<4.0',
         # 'constrained_decoding',
         # 'markupsafe==2.1.2', # downgrade because of bug in 2.1.1, https://stackoverflow.com/questions/72191560/importerror-cannot-import-name-soft-unicode-from-markupsafe
     ],
     package_data={
         "": ["qasem/data/connectives_small_set.txt"],
```

