# Comparing `tmp/madai-0.1.1.tar.gz` & `tmp/madai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madai-0.1.1.tar", max compression
+gzip compressed data, was "madai-0.1.2.tar", max compression
```

## Comparing `madai-0.1.1.tar` & `madai-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      553 2023-05-04 14:53:17.872677 madai-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.1/madai/__init__.py
--rw-r--r--   0        0        0     5545 2023-05-05 15:45:40.927013 madai-0.1.1/madai/main.py
--rw-r--r--   0        0        0      945 2023-05-04 13:23:09.019390 madai-0.1.1/madai/utils.py
--rw-r--r--   0        0        0      576 2023-05-08 04:59:05.242194 madai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 madai-0.1.1/setup.py
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 madai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      553 2023-05-04 14:53:17.872677 madai-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.2/madai/__init__.py
+-rw-r--r--   0        0        0     5355 2023-05-08 06:08:13.693984 madai-0.1.2/madai/main.py
+-rw-r--r--   0        0        0     1285 2023-05-08 06:06:04.806489 madai-0.1.2/madai/utils.py
+-rw-r--r--   0        0        0      576 2023-05-08 06:08:28.852634 madai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 madai-0.1.2/setup.py
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 madai-0.1.2/PKG-INFO
```

### Comparing `madai-0.1.1/README.md` & `madai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `madai-0.1.1/madai/main.py` & `madai-0.1.2/madai/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from argparse import ArgumentParser
 from collections import Counter
 from dataclasses import dataclass, field
+from functools import partial
 from random import sample
 from typing import Union
 
 import click
 import numpy as np
 import scipy.stats as stats
 import sienna
-from nltk.corpus import stopwords
 from spacy.tokenizer import Tokenizer
 from tqdm import tqdm
 
-from madai.utils import get_tokenizer
-
-stopwords = stopwords.words("english")
+from madai.utils import get_tokenizer, tokenize
 
 
 @dataclass
 class FreqCounter:
     seed_words: set[str]
     w2idx: dict[str, int] = field(init=False)
     counter: list[int] = field(init=False)
@@ -63,38 +61,28 @@
     b: list[str],
     tok: Tokenizer,
     slice_size: Union[int, float],
     top_n: int = 500,
     n_iter: int = 5,
     remove_stopwords: bool = False,
 ) -> np.ndarray:
-
     a_doc_n = len(a)
     b_doc_n = len(b)
 
     doc_n = min(a_doc_n, b_doc_n)
     a = a[:doc_n]
     b = b[:doc_n]
 
     # Number of sample for each slice
     slice_size = slice_size if isinstance(slice_size, int) else int(doc_n * slice_size)
 
     # Tokenization for freq word counting
-    a_words = [
-        word.text.lower()
-        for doc in a
-        for word in tok(doc)
-        if remove_stopwords and (word.text.lower() not in stopwords)
-    ]
-    b_words = [
-        word.text.lower()
-        for doc in b
-        for word in tok(doc)
-        if remove_stopwords and (word.text.lower() not in stopwords)
-    ]
+    tokenizer = partial(tokenize, tok, remove_stopwords)
+    a_words = [word for doc in a for word in tokenizer(doc)]
+    b_words = [word for doc in b for word in tokenizer(doc)]
 
     assert isinstance(a_words, list)
     assert isinstance(a_words[0], str)
 
     # Find Top N words
     freq_words = set(
         [word for word, _ in Counter(a_words + b_words).most_common(top_n)]
```

### Comparing `madai-0.1.1/pyproject.toml` & `madai-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "madai"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["sobamchan <oh.sore.sore.soutarou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 scipy = "^1.10.1"
```

### Comparing `madai-0.1.1/setup.py` & `madai-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'spacy>=3.5.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['madai = madai.main:run']}
 
 setup_kwargs = {
     'name': 'madai',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '# madai\n\nCompute difference between two corpus by using chi2.\nImplementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).\n\nI am not fully sure if this implementation is perfectly follow this paper.\nFeel free to make issues to point out some problems if you find.\n\n## Installation\n\n```\npip install madai\n```\n\n## Usage\n\nTwo target corpus need to be text files, each line containing one document/sentence.\n\n```\nmadai /path/to/corpus/a /path/to/corpus/b\n```\n\nTo view parameters, run,\n```\nmadai --help\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `madai-0.1.1/PKG-INFO` & `madai-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madai
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

