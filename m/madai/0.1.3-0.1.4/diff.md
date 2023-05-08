# Comparing `tmp/madai-0.1.3.tar.gz` & `tmp/madai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madai-0.1.3.tar", max compression
+gzip compressed data, was "madai-0.1.4.tar", max compression
```

## Comparing `madai-0.1.3.tar` & `madai-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      553 2023-05-04 14:53:17.872677 madai-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.3/madai/__init__.py
--rw-r--r--   0        0        0     5389 2023-05-08 06:33:44.469548 madai-0.1.3/madai/main.py
--rw-r--r--   0        0        0     1357 2023-05-08 06:34:11.409000 madai-0.1.3/madai/utils.py
--rw-r--r--   0        0        0      576 2023-05-08 06:34:32.017549 madai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 madai-0.1.3/setup.py
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 madai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      553 2023-05-04 14:53:17.872677 madai-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.4/madai/__init__.py
+-rw-r--r--   0        0        0     5175 2023-05-08 06:56:54.882501 madai-0.1.4/madai/main.py
+-rw-r--r--   0        0        0     1357 2023-05-08 06:34:11.409000 madai-0.1.4/madai/utils.py
+-rw-r--r--   0        0        0      576 2023-05-08 06:57:01.610645 madai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 madai-0.1.4/setup.py
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 madai-0.1.4/PKG-INFO
```

### Comparing `madai-0.1.3/README.md` & `madai-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `madai-0.1.3/madai/main.py` & `madai-0.1.4/madai/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,26 +112,16 @@
         sub_b = [
             doc for slice in sample(b_sliices, k=n_slices_to_sample) for doc in slice
         ]
 
         assert isinstance(sub_a[0], str)
         assert isinstance(sub_b[0], str)
 
-        a_words = [
-            word.text.lower()
-            for doc in sub_a
-            for word in tok(doc)
-            if word.text.lower() not in stopwords
-        ]
-        b_words = [
-            word.text.lower()
-            for doc in sub_b
-            for word in tok(doc)
-            if word.text.lower() not in stopwords
-        ]
+        a_words = [word for doc in a for word in tokenizer(doc)]
+        b_words = [word for doc in b for word in tokenizer(doc)]
 
         a_fc.load_words(a_words)
         b_fc.load_words(b_words)
 
         score = sim(a_fc, b_fc)
         scores.append(score)
```

### Comparing `madai-0.1.3/madai/utils.py` & `madai-0.1.4/madai/utils.py`

 * *Files identical despite different names*

### Comparing `madai-0.1.3/pyproject.toml` & `madai-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "madai"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["sobamchan <oh.sore.sore.soutarou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 scipy = "^1.10.1"
```

### Comparing `madai-0.1.3/setup.py` & `madai-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'spacy>=3.5.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['madai = madai.main:run']}
 
 setup_kwargs = {
     'name': 'madai',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '# madai\n\nCompute difference between two corpus by using chi2.\nImplementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).\n\nI am not fully sure if this implementation is perfectly follow this paper.\nFeel free to make issues to point out some problems if you find.\n\n## Installation\n\n```\npip install madai\n```\n\n## Usage\n\nTwo target corpus need to be text files, each line containing one document/sentence.\n\n```\nmadai /path/to/corpus/a /path/to/corpus/b\n```\n\nTo view parameters, run,\n```\nmadai --help\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `madai-0.1.3/PKG-INFO` & `madai-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madai
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

