# Comparing `tmp/bgnlp-0.1.4.tar.gz` & `tmp/bgnlp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgnlp-0.1.4.tar", last modified: Fri Apr  7 15:29:30 2023, max compression
+gzip compressed data, was "bgnlp-0.2.0.tar", last modified: Mon May  8 09:18:36 2023, max compression
```

## Comparing `bgnlp-0.1.4.tar` & `bgnlp-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.676992 bgnlp-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 15:29:19.000000 bgnlp-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 15:29:19.000000 bgnlp-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-07 15:29:30.672992 bgnlp-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-07 15:29:19.000000 bgnlp-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/models/seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/serialized/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/serialized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/serialized/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/serialized/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/serialized/vocabs/
--rw-r--r--   0 runner    (1001) docker     (123)    82097 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/serialized/vocabs/cb-vocab.pt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/taggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-07 15:29:19.000000 bgnlp-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:29:30.676992 bgnlp-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-07 15:29:19.000000 bgnlp-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-08 09:18:25.000000 bgnlp-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 09:18:25.000000 bgnlp-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-08 09:18:36.782844 bgnlp-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-08 09:18:25.000000 bgnlp-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/models/seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/serialized/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/serialized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/serialized/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/serialized/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/serialized/vocabs/
+-rw-r--r--   0 runner    (1001) docker     (123)    82097 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/serialized/vocabs/cb-vocab.pt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/taggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 09:18:25.000000 bgnlp-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:18:36.782844 bgnlp-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-08 09:18:25.000000 bgnlp-0.2.0/setup.py
```

### Comparing `bgnlp-0.1.4/LICENSE` & `bgnlp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/PKG-INFO` & `bgnlp-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgnlp
-Version: 0.1.4
+Version: 0.2.0
 Summary: Package for Bulgarian Natural Language Processing (NLP)
 Author: Adam Fauzi
 Author-email: adamfzh98@gmail.com
 Keywords: pytorch,nlp,bulgaria,machine learning,deep learning,AI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
@@ -34,19 +34,17 @@
 ```
 
 ## Package functionalities
 
 ### Part-of-speech (PoS) tagging
 
 ```python
-from bgnlp import PosTagger, PosTaggerConfig
+from bgnlp import pos
 
 
-config = PosTaggerConfig()
-pos = PosTagger(config=config)
 print(pos("Това е библиотека за обработка на естествен език."))
 ```
 
 ```json
 [{
     "word": "Това",
     "tag": "PDOsn",
@@ -94,47 +92,45 @@
     "en_desc": "punctuation"
 }]
 ```
 
 ### Lemmatization
 
 ```python
-from bgnlp import LemmaTaggerConfig, LemmaTagger
+from bgnlp import lemmatize
 
 
-lemma = LemmaTagger(config=LemmaTaggerConfig())
 text = "Добре дошли!"
-print(lemma(text))
+print(lemmatize(text))
 ```
 
 ```bash
 [{'word': 'Добре', 'lemma': 'Добре'}, {'word': 'дошли', 'lemma': 'дойда'}, {'word': '!', 'lemma': '!'}]
 ```
 
 ```python
 # Generating a string of lemmas.
-print(lemma(text, as_string=True))
+print(lemmatize(text, as_string=True))
 ```
 
 ```bash
 Добре дойда!
 ```
 
 ### Named Entity Recognition (NER) tagging
 
 Currently, the available NER tags are:
 - `PER` - Person
 - `ORG` - Organization
 - `LOC` - Location
 
 ```python
-from bgnlp import NerTagger, NerTaggerConfig
+from bgnlp import ner
 
 
-ner = NerTagger(config=NerTaggerConfig())
 text = "Барух Спиноза е роден в Амстердам"
 
 print(f"Input: {text}")
 print("Result:", ner(text))
 ```
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bgnlp Version: 0.1.4 Summary: Package for Bulgarian
+Metadata-Version: 2.1 Name: bgnlp Version: 0.2.0 Summary: Package for Bulgarian
 Natural Language Processing (NLP) Author: Adam Fauzi Author-email:
 adamfzh98@gmail.com Keywords: pytorch,nlp,bulgaria,machine learning,deep
 learning,AI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
@@ -14,46 +14,44 @@
 System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown License-File: LICENSE # **bgnlp**:
 Model-first approach to Bulgarian NLP [Open_In_Colab] [![Downloads](https://
 static.pepy.tech/personalized-badge/
 bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)]
 (https://pypi.org/project/bgnlp/) ```sh pip install bgnlp ``` ## Package
 functionalities ### Part-of-speech (PoS) tagging ```python from bgnlp import
-PosTagger, PosTaggerConfig config = PosTaggerConfig() pos = PosTagger
-(config=config) print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð°
-Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð° ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word":
-"Ð¢Ð¾Ð²Ð°", "tag": "PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc":
-"pronoun" }, { "word": "Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»",
-"en_desc": "verb" }, { "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof",
-"bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word":
-"Ð·Ð°", "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" },
-{ "word": "Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°",
+pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð°
+ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag":
+"PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word":
+"Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" },
+{ "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc":
+"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°",
 "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word":
-"ÐµÑÑÐµÑÑÐ²ÐµÐ½", "tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾
-Ð¸Ð¼Ðµ", "en_desc": "adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom",
-"bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word":
-".", "tag": "U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc":
-"punctuation" }] ``` ### Lemmatization ```python from bgnlp import
-LemmaTaggerConfig, LemmaTagger lemma = LemmaTagger(config=LemmaTaggerConfig())
-text = "ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemma(text)) ``` ```bash [{'word':
+"Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
+Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc":
+"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½",
+"tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
+"adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc":
+"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": ".", "tag":
+"U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation"
+}] ``` ### Lemmatization ```python from bgnlp import lemmatize text =
+"ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word':
 'ÐÐ¾Ð±ÑÐµ', 'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma':
 'Ð´Ð¾Ð¹Ð´Ð°'}, {'word': '!', 'lemma': '!'}] ``` ```python # Generating a string
-of lemmas. print(lemma(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
+of lemmas. print(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
 Ð´Ð¾Ð¹Ð´Ð°! ``` ### Named Entity Recognition (NER) tagging Currently, the
 available NER tags are: - `PER` - Person - `ORG` - Organization - `LOC` -
-Location ```python from bgnlp import NerTagger, NerTaggerConfig ner = NerTagger
-(config=NerTaggerConfig()) text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
-ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner(text)) ```
-```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼
-Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°', 'entity_group': 'PER'}, {'word':
-'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}] ``` ### Using a Config object A
-tagger Config is used to define the underlying model. You can change the device
-on which it makes inference: ```python # Make inference using the GPU (by
-default it is "cpu"): config = NerTaggerConfig(device="cuda") ner = NerTagger
-(config=config) # ... ``` You can also change the path to the model weights.
-For `NerTagger` you can directly pass the HuggingFace's Model Hub path. All
-other taggers use weights uploaded to Google Drive. ```python # Define the path
-to the model weights. It can be a single .pt file or a path to HuggingFace's
-Model Hub (only for NerTagger). config = NerTaggerConfig(model_path="path/to/
-model") ner = NerTagger(config=config) # ... ``` Please, note that the model
-should be of the same architecture as the one used by the certain Tagger.
+Location ```python from bgnlp import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ
+ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner
+(text)) ``` ```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
+ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼ Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°',
+'entity_group': 'PER'}, {'word': 'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}]
+``` ### Using a Config object A tagger Config is used to define the underlying
+model. You can change the device on which it makes inference: ```python # Make
+inference using the GPU (by default it is "cpu"): config = NerTaggerConfig
+(device="cuda") ner = NerTagger(config=config) # ... ``` You can also change
+the path to the model weights. For `NerTagger` you can directly pass the
+HuggingFace's Model Hub path. All other taggers use weights uploaded to Google
+Drive. ```python # Define the path to the model weights. It can be a single .pt
+file or a path to HuggingFace's Model Hub (only for NerTagger). config =
+NerTaggerConfig(model_path="path/to/model") ner = NerTagger(config=config) #
+... ``` Please, note that the model should be of the same architecture as the
+one used by the certain Tagger.
```

### Comparing `bgnlp-0.1.4/README.md` & `bgnlp-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 ```
 
 ## Package functionalities
 
 ### Part-of-speech (PoS) tagging
 
 ```python
-from bgnlp import PosTagger, PosTaggerConfig
+from bgnlp import pos
 
 
-config = PosTaggerConfig()
-pos = PosTagger(config=config)
 print(pos("Това е библиотека за обработка на естествен език."))
 ```
 
 ```json
 [{
     "word": "Това",
     "tag": "PDOsn",
@@ -68,47 +66,45 @@
     "en_desc": "punctuation"
 }]
 ```
 
 ### Lemmatization
 
 ```python
-from bgnlp import LemmaTaggerConfig, LemmaTagger
+from bgnlp import lemmatize
 
 
-lemma = LemmaTagger(config=LemmaTaggerConfig())
 text = "Добре дошли!"
-print(lemma(text))
+print(lemmatize(text))
 ```
 
 ```bash
 [{'word': 'Добре', 'lemma': 'Добре'}, {'word': 'дошли', 'lemma': 'дойда'}, {'word': '!', 'lemma': '!'}]
 ```
 
 ```python
 # Generating a string of lemmas.
-print(lemma(text, as_string=True))
+print(lemmatize(text, as_string=True))
 ```
 
 ```bash
 Добре дойда!
 ```
 
 ### Named Entity Recognition (NER) tagging
 
 Currently, the available NER tags are:
 - `PER` - Person
 - `ORG` - Organization
 - `LOC` - Location
 
 ```python
-from bgnlp import NerTagger, NerTaggerConfig
+from bgnlp import ner
 
 
-ner = NerTagger(config=NerTaggerConfig())
 text = "Барух Спиноза е роден в Амстердам"
 
 print(f"Input: {text}")
 print("Result:", ner(text))
 ```
 
 ```bash
```

#### html2text {}

```diff
@@ -1,44 +1,42 @@
 # **bgnlp**: Model-first approach to Bulgarian NLP [Open_In_Colab] [!
 [Downloads](https://static.pepy.tech/personalized-badge/
 bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)]
 (https://pypi.org/project/bgnlp/) ```sh pip install bgnlp ``` ## Package
 functionalities ### Part-of-speech (PoS) tagging ```python from bgnlp import
-PosTagger, PosTaggerConfig config = PosTaggerConfig() pos = PosTagger
-(config=config) print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð°
-Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð° ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word":
-"Ð¢Ð¾Ð²Ð°", "tag": "PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc":
-"pronoun" }, { "word": "Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»",
-"en_desc": "verb" }, { "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof",
-"bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word":
-"Ð·Ð°", "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" },
-{ "word": "Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°",
+pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð°
+ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag":
+"PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word":
+"Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" },
+{ "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc":
+"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°",
 "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word":
-"ÐµÑÑÐµÑÑÐ²ÐµÐ½", "tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾
-Ð¸Ð¼Ðµ", "en_desc": "adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom",
-"bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word":
-".", "tag": "U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc":
-"punctuation" }] ``` ### Lemmatization ```python from bgnlp import
-LemmaTaggerConfig, LemmaTagger lemma = LemmaTagger(config=LemmaTaggerConfig())
-text = "ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemma(text)) ``` ```bash [{'word':
+"Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
+Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc":
+"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½",
+"tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
+"adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc":
+"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": ".", "tag":
+"U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation"
+}] ``` ### Lemmatization ```python from bgnlp import lemmatize text =
+"ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word':
 'ÐÐ¾Ð±ÑÐµ', 'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma':
 'Ð´Ð¾Ð¹Ð´Ð°'}, {'word': '!', 'lemma': '!'}] ``` ```python # Generating a string
-of lemmas. print(lemma(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
+of lemmas. print(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
 Ð´Ð¾Ð¹Ð´Ð°! ``` ### Named Entity Recognition (NER) tagging Currently, the
 available NER tags are: - `PER` - Person - `ORG` - Organization - `LOC` -
-Location ```python from bgnlp import NerTagger, NerTaggerConfig ner = NerTagger
-(config=NerTaggerConfig()) text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
-ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner(text)) ```
-```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼
-Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°', 'entity_group': 'PER'}, {'word':
-'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}] ``` ### Using a Config object A
-tagger Config is used to define the underlying model. You can change the device
-on which it makes inference: ```python # Make inference using the GPU (by
-default it is "cpu"): config = NerTaggerConfig(device="cuda") ner = NerTagger
-(config=config) # ... ``` You can also change the path to the model weights.
-For `NerTagger` you can directly pass the HuggingFace's Model Hub path. All
-other taggers use weights uploaded to Google Drive. ```python # Define the path
-to the model weights. It can be a single .pt file or a path to HuggingFace's
-Model Hub (only for NerTagger). config = NerTaggerConfig(model_path="path/to/
-model") ner = NerTagger(config=config) # ... ``` Please, note that the model
-should be of the same architecture as the one used by the certain Tagger.
+Location ```python from bgnlp import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ
+ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner
+(text)) ``` ```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
+ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼ Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°',
+'entity_group': 'PER'}, {'word': 'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}]
+``` ### Using a Config object A tagger Config is used to define the underlying
+model. You can change the device on which it makes inference: ```python # Make
+inference using the GPU (by default it is "cpu"): config = NerTaggerConfig
+(device="cuda") ner = NerTagger(config=config) # ... ``` You can also change
+the path to the model weights. For `NerTagger` you can directly pass the
+HuggingFace's Model Hub path. All other taggers use weights uploaded to Google
+Drive. ```python # Define the path to the model weights. It can be a single .pt
+file or a path to HuggingFace's Model Hub (only for NerTagger). config =
+NerTaggerConfig(model_path="path/to/model") ner = NerTagger(config=config) #
+... ``` Please, note that the model should be of the same architecture as the
+one used by the certain Tagger.
```

### Comparing `bgnlp-0.1.4/bgnlp/models/bert.py` & `bgnlp-0.2.0/bgnlp/models/bert.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/bgnlp/models/seq2seq.py` & `bgnlp-0.2.0/bgnlp/models/seq2seq.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/bgnlp/serialized/vocabs/cb-vocab.pt` & `bgnlp-0.2.0/bgnlp/serialized/vocabs/cb-vocab.pt`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/bgnlp/tools/configs.py` & `bgnlp-0.2.0/bgnlp/tools/configs.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/bgnlp/tools/mappings.py` & `bgnlp-0.2.0/bgnlp/tools/mappings.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/bgnlp/tools/mixins.py` & `bgnlp-0.2.0/bgnlp/tools/mixins.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/bgnlp/tools/taggers.py` & `bgnlp-0.2.0/bgnlp/tools/taggers.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/bgnlp/tools/tokenizers.py` & `bgnlp-0.2.0/bgnlp/tools/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/bgnlp.egg-info/PKG-INFO` & `bgnlp-0.2.0/bgnlp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgnlp
-Version: 0.1.4
+Version: 0.2.0
 Summary: Package for Bulgarian Natural Language Processing (NLP)
 Author: Adam Fauzi
 Author-email: adamfzh98@gmail.com
 Keywords: pytorch,nlp,bulgaria,machine learning,deep learning,AI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
@@ -34,19 +34,17 @@
 ```
 
 ## Package functionalities
 
 ### Part-of-speech (PoS) tagging
 
 ```python
-from bgnlp import PosTagger, PosTaggerConfig
+from bgnlp import pos
 
 
-config = PosTaggerConfig()
-pos = PosTagger(config=config)
 print(pos("Това е библиотека за обработка на естествен език."))
 ```
 
 ```json
 [{
     "word": "Това",
     "tag": "PDOsn",
@@ -94,47 +92,45 @@
     "en_desc": "punctuation"
 }]
 ```
 
 ### Lemmatization
 
 ```python
-from bgnlp import LemmaTaggerConfig, LemmaTagger
+from bgnlp import lemmatize
 
 
-lemma = LemmaTagger(config=LemmaTaggerConfig())
 text = "Добре дошли!"
-print(lemma(text))
+print(lemmatize(text))
 ```
 
 ```bash
 [{'word': 'Добре', 'lemma': 'Добре'}, {'word': 'дошли', 'lemma': 'дойда'}, {'word': '!', 'lemma': '!'}]
 ```
 
 ```python
 # Generating a string of lemmas.
-print(lemma(text, as_string=True))
+print(lemmatize(text, as_string=True))
 ```
 
 ```bash
 Добре дойда!
 ```
 
 ### Named Entity Recognition (NER) tagging
 
 Currently, the available NER tags are:
 - `PER` - Person
 - `ORG` - Organization
 - `LOC` - Location
 
 ```python
-from bgnlp import NerTagger, NerTaggerConfig
+from bgnlp import ner
 
 
-ner = NerTagger(config=NerTaggerConfig())
 text = "Барух Спиноза е роден в Амстердам"
 
 print(f"Input: {text}")
 print("Result:", ner(text))
 ```
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bgnlp Version: 0.1.4 Summary: Package for Bulgarian
+Metadata-Version: 2.1 Name: bgnlp Version: 0.2.0 Summary: Package for Bulgarian
 Natural Language Processing (NLP) Author: Adam Fauzi Author-email:
 adamfzh98@gmail.com Keywords: pytorch,nlp,bulgaria,machine learning,deep
 learning,AI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
@@ -14,46 +14,44 @@
 System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown License-File: LICENSE # **bgnlp**:
 Model-first approach to Bulgarian NLP [Open_In_Colab] [![Downloads](https://
 static.pepy.tech/personalized-badge/
 bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)]
 (https://pypi.org/project/bgnlp/) ```sh pip install bgnlp ``` ## Package
 functionalities ### Part-of-speech (PoS) tagging ```python from bgnlp import
-PosTagger, PosTaggerConfig config = PosTaggerConfig() pos = PosTagger
-(config=config) print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð°
-Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð° ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word":
-"Ð¢Ð¾Ð²Ð°", "tag": "PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc":
-"pronoun" }, { "word": "Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»",
-"en_desc": "verb" }, { "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof",
-"bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word":
-"Ð·Ð°", "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" },
-{ "word": "Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°",
+pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð°
+ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag":
+"PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word":
+"Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" },
+{ "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc":
+"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°",
 "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word":
-"ÐµÑÑÐµÑÑÐ²ÐµÐ½", "tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾
-Ð¸Ð¼Ðµ", "en_desc": "adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom",
-"bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word":
-".", "tag": "U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc":
-"punctuation" }] ``` ### Lemmatization ```python from bgnlp import
-LemmaTaggerConfig, LemmaTagger lemma = LemmaTagger(config=LemmaTaggerConfig())
-text = "ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemma(text)) ``` ```bash [{'word':
+"Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
+Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc":
+"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½",
+"tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
+"adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc":
+"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": ".", "tag":
+"U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation"
+}] ``` ### Lemmatization ```python from bgnlp import lemmatize text =
+"ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word':
 'ÐÐ¾Ð±ÑÐµ', 'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma':
 'Ð´Ð¾Ð¹Ð´Ð°'}, {'word': '!', 'lemma': '!'}] ``` ```python # Generating a string
-of lemmas. print(lemma(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
+of lemmas. print(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
 Ð´Ð¾Ð¹Ð´Ð°! ``` ### Named Entity Recognition (NER) tagging Currently, the
 available NER tags are: - `PER` - Person - `ORG` - Organization - `LOC` -
-Location ```python from bgnlp import NerTagger, NerTaggerConfig ner = NerTagger
-(config=NerTaggerConfig()) text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
-ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner(text)) ```
-```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼
-Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°', 'entity_group': 'PER'}, {'word':
-'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}] ``` ### Using a Config object A
-tagger Config is used to define the underlying model. You can change the device
-on which it makes inference: ```python # Make inference using the GPU (by
-default it is "cpu"): config = NerTaggerConfig(device="cuda") ner = NerTagger
-(config=config) # ... ``` You can also change the path to the model weights.
-For `NerTagger` you can directly pass the HuggingFace's Model Hub path. All
-other taggers use weights uploaded to Google Drive. ```python # Define the path
-to the model weights. It can be a single .pt file or a path to HuggingFace's
-Model Hub (only for NerTagger). config = NerTaggerConfig(model_path="path/to/
-model") ner = NerTagger(config=config) # ... ``` Please, note that the model
-should be of the same architecture as the one used by the certain Tagger.
+Location ```python from bgnlp import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ
+ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner
+(text)) ``` ```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
+ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼ Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°',
+'entity_group': 'PER'}, {'word': 'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}]
+``` ### Using a Config object A tagger Config is used to define the underlying
+model. You can change the device on which it makes inference: ```python # Make
+inference using the GPU (by default it is "cpu"): config = NerTaggerConfig
+(device="cuda") ner = NerTagger(config=config) # ... ``` You can also change
+the path to the model weights. For `NerTagger` you can directly pass the
+HuggingFace's Model Hub path. All other taggers use weights uploaded to Google
+Drive. ```python # Define the path to the model weights. It can be a single .pt
+file or a path to HuggingFace's Model Hub (only for NerTagger). config =
+NerTaggerConfig(model_path="path/to/model") ner = NerTagger(config=config) #
+... ``` Please, note that the model should be of the same architecture as the
+one used by the certain Tagger.
```

### Comparing `bgnlp-0.1.4/bgnlp.egg-info/SOURCES.txt` & `bgnlp-0.2.0/bgnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.4/setup.py` & `bgnlp-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.abspath(os.path.dirname(__file__))
 README_PATH = os.path.join(ROOT, "README.md")
 REQUIREMENTS_PATH = os.path.join(ROOT, "requirements.txt")
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.1.4'
+VERSION = '0.2.0'
 DESCRIPTION = 'Package for Bulgarian Natural Language Processing (NLP)'
 
 
 def _get_requirements(path):
     with open(path, "r") as f:
         requirements_str = f.read()
         packages = re.findall(r"(.+=?=?[^\n]+)\n", requirements_str)
```

