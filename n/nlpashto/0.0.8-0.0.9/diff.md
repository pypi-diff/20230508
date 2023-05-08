# Comparing `tmp/nlpashto-0.0.8.tar.gz` & `tmp/nlpashto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpashto-0.0.8.tar", last modified: Wed Mar  1 11:29:51 2023, max compression
+gzip compressed data, was "nlpashto-0.0.9.tar", last modified: Sat May  6 11:50:42 2023, max compression
```

## Comparing `nlpashto-0.0.8.tar` & `nlpashto-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 11:29:51.229967 nlpashto-0.0.8/
--rw-rw-rw-   0        0        0     1096 2023-02-28 10:10:26.000000 nlpashto-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2005 2023-03-01 11:29:51.228966 nlpashto-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-03-01 07:54:59.000000 nlpashto-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 11:29:51.219052 nlpashto-0.0.8/nlpashto/
--rw-rw-rw-   0        0        0       89 2023-03-01 11:28:52.000000 nlpashto-0.0.8/nlpashto/__init__.py
--rw-rw-rw-   0        0        0      314 2023-03-01 11:18:38.000000 nlpashto-0.0.8/nlpashto/char_replace.py
--rw-rw-rw-   0        0        0     1608 2023-03-01 11:28:37.000000 nlpashto-0.0.8/nlpashto/functions.py
--rw-rw-rw-   0        0        0     4881 2023-03-01 11:28:44.000000 nlpashto-0.0.8/nlpashto/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-01 11:29:51.227966 nlpashto-0.0.8/nlpashto.egg-info/
--rw-rw-rw-   0        0        0     2005 2023-03-01 11:29:51.000000 nlpashto-0.0.8/nlpashto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-03-01 11:29:51.000000 nlpashto-0.0.8/nlpashto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 11:29:51.000000 nlpashto-0.0.8/nlpashto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-01 11:29:51.000000 nlpashto-0.0.8/nlpashto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      545 2023-03-01 11:29:20.000000 nlpashto-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-01 11:29:51.229967 nlpashto-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 11:50:42.739075 nlpashto-0.0.9/
+-rw-rw-rw-   0        0        0     1096 2023-02-28 10:10:26.000000 nlpashto-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3154 2023-05-06 11:50:42.737058 nlpashto-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2697 2023-03-01 12:20:36.000000 nlpashto-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:50:42.725502 nlpashto-0.0.9/nlpashto/
+-rw-rw-rw-   0        0        0      125 2023-05-06 11:41:57.000000 nlpashto-0.0.9/nlpashto/__init__.py
+-rw-rw-rw-   0        0        0      689 2023-04-02 14:06:28.000000 nlpashto-0.0.9/nlpashto/helpers.py
+-rw-rw-rw-   0        0        0       35 2023-05-06 09:13:19.000000 nlpashto-0.0.9/nlpashto/pos_tagging.py
+-rw-rw-rw-   0        0        0     1374 2023-05-06 11:42:05.000000 nlpashto-0.0.9/nlpashto/spelling_correction.py
+-rw-rw-rw-   0        0        0      976 2023-05-06 11:43:03.000000 nlpashto-0.0.9/nlpashto/utils.py
+-rw-rw-rw-   0        0        0       41 2023-05-06 09:12:59.000000 nlpashto-0.0.9/nlpashto/word_segmentation.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:50:42.736070 nlpashto-0.0.9/nlpashto.egg-info/
+-rw-rw-rw-   0        0        0     3154 2023-05-06 11:50:42.000000 nlpashto-0.0.9/nlpashto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-06 11:50:42.000000 nlpashto-0.0.9/nlpashto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:50:42.000000 nlpashto-0.0.9/nlpashto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 11:50:42.000000 nlpashto-0.0.9/nlpashto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      545 2023-05-06 11:50:27.000000 nlpashto-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:50:42.740075 nlpashto-0.0.9/setup.cfg
```

### Comparing `nlpashto-0.0.8/LICENSE` & `nlpashto-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpashto-0.0.8/PKG-INFO` & `nlpashto-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-Metadata-Version: 2.1
-Name: nlpashto
-Version: 0.0.8
-Summary: Pashto Natural Language Processing Toolkit
-Author-email: Ijazul Haq <ijazse@hotmail.com>
-Project-URL: Homepage, https://github.com/ijazul-haq/nlpashto
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NLPashto – NLP Toolkit for Pashto
-NLPashto is a python suite for supporting research and development in Pashto Natural Language Processing. NLPashto project is initiated at Shanghai Jiao Tong University, China
+![GitHub](https://img.shields.io/github/license/ijazul-haq/nlpashto) ![GitHub contributors](https://img.shields.io/github/contributors/ijazul-haq/nlpashto) ![code size](https://img.shields.io/github/languages/code-size/ijazul-haq/nlpashto)
+
+NLPashto is a Python suite for Pashto Natural Language Processing, initiated at Shanghai Jiao Tong University. 
+A sample of the Pashto Corpus is available [here](https://github.com/ijazul-haq/pashto_pos) that is used to train some of the models in NLPashto.
 
 ## Prerequisites
 To use NLPashto you will need:
 * Python 3.8+
 
 ## Installing NLPashto
-You can install pashto from PyPi using this command
+NLPashto can be installed from PyPi using this command
 ```bash
 pip install nlpashto
 ```
 
 ## Using NLPashto
 
-### Word Segmentation
-```bash
+### Sentence Tokenizer
+```python
+from nlpashto import sentence_tokenizer
+sentences_list = sentence_tokenizer(content)
+tagged = pos_tagger(tokenized)
+```
+
+### Word Tokenizer
+```python
 from nlpashto import word_tokenizer
 
 text = 'همدارنګه تیره شپه او ورځ په هیواد کې د کرونا ویروس له امله ۵ تنه مړه شوي'
 tokenized = word_tokenizer(text)
 print(tokenized)
+['همدارنګه', 'تیره', 'شپه', 'او', 'ورځ', 'په', 'هیواد', 'کې', 'د', 'کرونا ویروس', 'له امله', '۵', 'تنه', 'مړه', 'شوي']
+```
+
+### Whitespace Tokenizer (Proofing)
+Whitespace Tokenizer can be used as a proofing tool to remove the space-omission and space-insertion errors. It will remove extra spaces from the text and will insert space where necessary. It’s a beta version and only recommended if the input text is extremely noisy. 
+
+```python
+from nlpashto import tokenizer
+
+noisy_text = 'ه  م  د  ا  ر  ن  ګ ه ت ی ر ه ش پ ه ا وورځپههیوادکېدکروناویروسلهامله۵تنهمړهشوي'
+corrected = tokenizer(noisy_text)
+print(corrected)
+همدارنګه تیره شپه او ورځ په هیواد کې د کرونا ویروس له امله ۵ تنه مړه شوي
 ```
-Output: ['همدارنګه', 'تیره', 'شپه', 'او', 'ورځ', 'په', 'هیواد', 'کې', 'د', 'کرونا ویروس', 'له امله', '۵', 'تنه', 'مړه', 'شوي']
+
 ### POS Tagging
-```bash
+```python
 from nlpashto import pos_tagger
 
 text = 'همدارنګه تیره شپه او ورځ په هیواد کې د کرونا ویروس له امله ۵ تنه مړه شوي'
 tokenized = word_tokenizer(text)
 tagged = pos_tagger(tokenized)
 print(tagged) 
+[['همدارنګه', 'RB'], ['تیره', 'JJ'], ['شپه', 'NNF'], ['او', 'CC'], ['ورځ', 'NNM'], ['په', 'IN'], ['هیواد', 'NNM'], ['کې', 'PT'], ['د', 'IN'], ['کرونا ویروس', 'NNP'], ['له امله', 'RB'], ['۵', 'NB'], ['تنه', 'NNS'], ['مړه', 'JJ'], ['شوي', 'VBDX']]
 ```
-Output: [['همدارنګه', 'RB'], ['تیره', 'JJ'], ['شپه', 'NNF'], ['او', 'CC'], ['ورځ', 'NNM'], ['په', 'IN'], ['هیواد', 'NNM'], ['کې', 'PT'], ['د', 'IN'], ['کرونا ویروس', 'NNP'], ['له امله', 'RB'], ['۵', 'NB'], ['تنه', 'NNS'], ['مړه', 'JJ'], ['شوي', 'VBDX']]
-
-### Whitespace Correction (Proofing)
 
 ### Offensive Comments Detection
-
+Coming soon…
```

### Comparing `nlpashto-0.0.8/pyproject.toml` & `nlpashto-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nlpashto"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Ijazul Haq", email="ijazse@hotmail.com" },
 ]
 description = "Pashto Natural Language Processing Toolkit"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

