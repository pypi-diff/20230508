# Comparing `tmp/madai-0.1.0.tar.gz` & `tmp/madai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madai-0.1.0.tar", max compression
+gzip compressed data, was "madai-0.1.1.tar", max compression
```

## Comparing `madai-0.1.0.tar` & `madai-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      174 2023-05-04 14:37:18.418476 madai-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.0/madai/__init__.py
--rw-r--r--   0        0        0     5513 2023-05-04 14:34:54.346498 madai-0.1.0/madai/main.py
--rw-r--r--   0        0        0      945 2023-05-04 13:23:09.019390 madai-0.1.0/madai/utils.py
--rw-r--r--   0        0        0      576 2023-05-04 13:33:32.629454 madai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 madai-0.1.0/setup.py
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 madai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      553 2023-05-04 14:53:17.872677 madai-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.1/madai/__init__.py
+-rw-r--r--   0        0        0     5545 2023-05-05 15:45:40.927013 madai-0.1.1/madai/main.py
+-rw-r--r--   0        0        0      945 2023-05-04 13:23:09.019390 madai-0.1.1/madai/utils.py
+-rw-r--r--   0        0        0      576 2023-05-08 04:59:05.242194 madai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 madai-0.1.1/setup.py
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 madai-0.1.1/PKG-INFO
```

### Comparing `madai-0.1.0/madai/main.py` & `madai-0.1.1/madai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,21 @@
     b: list[str],
     tok: Tokenizer,
     slice_size: Union[int, float],
     top_n: int = 500,
     n_iter: int = 5,
     remove_stopwords: bool = False,
 ) -> np.ndarray:
-    # Tokenize corpus
+
     a_doc_n = len(a)
     b_doc_n = len(b)
+
     doc_n = min(a_doc_n, b_doc_n)
+    a = a[:doc_n]
+    b = b[:doc_n]
 
     # Number of sample for each slice
     slice_size = slice_size if isinstance(slice_size, int) else int(doc_n * slice_size)
 
     # Tokenization for freq word counting
     a_words = [
         word.text.lower()
@@ -98,21 +101,21 @@
     )
     assert len(freq_words) <= top_n
 
     a_fc = FreqCounter(seed_words=freq_words)
     b_fc = FreqCounter(seed_words=freq_words)
 
     # Split corpus into slices
-    a_sliices = [a[i : i + slice_size] for i in range(0, len(a), slice_size)]
-    b_sliices = [b[i : i + slice_size] for i in range(0, len(b), slice_size)]
+    a_sliices = [a[i : i + slice_size] for i in range(0, doc_n, slice_size)]
+    b_sliices = [b[i : i + slice_size] for i in range(0, doc_n, slice_size)]
 
     # A list of scores, further taken avg, std
     scores: list[float] = []
 
-    # A number of slices to be used for each iter
+    # A number of slices to be used for each iter (50% of a corpus)
     n_slices_to_sample = min(len(a_sliices), len(b_sliices)) // 2
 
     for _ in tqdm(range(n_iter), total=n_iter):
         a_fc.init_counter()
         b_fc.init_counter()
 
         sub_a = [
```

### Comparing `madai-0.1.0/madai/utils.py` & `madai-0.1.1/madai/utils.py`

 * *Files identical despite different names*

### Comparing `madai-0.1.0/pyproject.toml` & `madai-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "madai"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["sobamchan <oh.sore.sore.soutarou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 scipy = "^1.10.1"
```

### Comparing `madai-0.1.0/setup.py` & `madai-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'spacy>=3.5.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['madai = madai.main:run']}
 
 setup_kwargs = {
     'name': 'madai',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '# madai\n\nCompute difference between two corpus by using chi2.\nImplementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).\n',
+    'long_description': '# madai\n\nCompute difference between two corpus by using chi2.\nImplementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).\n\nI am not fully sure if this implementation is perfectly follow this paper.\nFeel free to make issues to point out some problems if you find.\n\n## Installation\n\n```\npip install madai\n```\n\n## Usage\n\nTwo target corpus need to be text files, each line containing one document/sentence.\n\n```\nmadai /path/to/corpus/a /path/to/corpus/b\n```\n\nTo view parameters, run,\n```\nmadai --help\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

