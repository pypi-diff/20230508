# Comparing `tmp/madai-0.1.2.tar.gz` & `tmp/madai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madai-0.1.2.tar", max compression
+gzip compressed data, was "madai-0.1.3.tar", max compression
```

## Comparing `madai-0.1.2.tar` & `madai-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      553 2023-05-04 14:53:17.872677 madai-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.2/madai/__init__.py
--rw-r--r--   0        0        0     5355 2023-05-08 06:08:13.693984 madai-0.1.2/madai/main.py
--rw-r--r--   0        0        0     1285 2023-05-08 06:06:04.806489 madai-0.1.2/madai/utils.py
--rw-r--r--   0        0        0      576 2023-05-08 06:08:28.852634 madai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 madai-0.1.2/setup.py
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 madai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      553 2023-05-04 14:53:17.872677 madai-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.3/madai/__init__.py
+-rw-r--r--   0        0        0     5389 2023-05-08 06:33:44.469548 madai-0.1.3/madai/main.py
+-rw-r--r--   0        0        0     1357 2023-05-08 06:34:11.409000 madai-0.1.3/madai/utils.py
+-rw-r--r--   0        0        0      576 2023-05-08 06:34:32.017549 madai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 madai-0.1.3/setup.py
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 madai-0.1.3/PKG-INFO
```

### Comparing `madai-0.1.2/README.md` & `madai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `madai-0.1.2/madai/main.py` & `madai-0.1.3/madai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 @click.command()
 @click.argument("a", type=str)
 @click.argument("b", type=str)
 @click.option("--lang", type=str, default="en")
 @click.option("--slice-size", type=float, default=0.25)
 @click.option("--n-iter", type=int, default=50)
 @click.option("--top-n", type=int, default=1000)
-@click.option("--remove-stopwords", is_flag=True)
+@click.option("--remove-stopwords", is_flag=True, show_default=True, default=False)
 def run(
     a: str,
     b: str,
     lang: str,
     slice_size: float,
     n_iter: int,
     top_n: int,
```

### Comparing `madai-0.1.2/madai/utils.py` & `madai-0.1.3/madai/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,10 +38,14 @@
         "zh": Chinese(),
     }[lang]
     return nlp.tokenizer
 
 
 def tokenize(tok: Tokenizer, remove_stopwords: bool, text: str) -> List[str]:
     if remove_stopwords:
-        return [word for word in tok(text) if word.text.lower() not in stopwords]
+        return [
+            word.text.lower()
+            for word in tok(text)
+            if word.text.lower() not in stopwords
+        ]
     else:
-        return [word for word in tok(text)]
+        return [word.text.lower() for word in tok(text)]
```

### Comparing `madai-0.1.2/pyproject.toml` & `madai-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "madai"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["sobamchan <oh.sore.sore.soutarou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 scipy = "^1.10.1"
```

### Comparing `madai-0.1.2/setup.py` & `madai-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'spacy>=3.5.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['madai = madai.main:run']}
 
 setup_kwargs = {
     'name': 'madai',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '# madai\n\nCompute difference between two corpus by using chi2.\nImplementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).\n\nI am not fully sure if this implementation is perfectly follow this paper.\nFeel free to make issues to point out some problems if you find.\n\n## Installation\n\n```\npip install madai\n```\n\n## Usage\n\nTwo target corpus need to be text files, each line containing one document/sentence.\n\n```\nmadai /path/to/corpus/a /path/to/corpus/b\n```\n\nTo view parameters, run,\n```\nmadai --help\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `madai-0.1.2/PKG-INFO` & `madai-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madai
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

